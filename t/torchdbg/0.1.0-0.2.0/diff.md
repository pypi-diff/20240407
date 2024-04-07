# Comparing `tmp/torchdbg-0.1.0.tar.gz` & `tmp/torchdbg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchdbg-0.1.0.tar", max compression
+gzip compressed data, was "torchdbg-0.2.0.tar", max compression
```

## Comparing `torchdbg-0.1.0.tar` & `torchdbg-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       53 2024-04-06 16:55:02.300964 torchdbg-0.1.0/README.md
--rw-r--r--   0        0        0      325 2024-04-06 16:54:00.000318 torchdbg-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5293 2024-04-06 16:43:53.997398 torchdbg-0.1.0/torchdbg/__init__.py
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 torchdbg-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       53 2024-04-06 16:55:02.300964 torchdbg-0.2.0/README.md
+-rw-r--r--   0        0        0      325 2024-04-07 16:44:20.408291 torchdbg-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5727 2024-04-07 16:35:25.564922 torchdbg-0.2.0/torchdbg/__init__.py
+-rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 torchdbg-0.2.0/PKG-INFO
```

### Comparing `torchdbg-0.1.0/torchdbg/__init__.py` & `torchdbg-0.2.0/torchdbg/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Usage: TORCH_TRACE=/tmp/test python torchdbg.py  && cat /tmp/test/*
 
 import torch
-from torch.utils._python_dispatch import TorchDispatchMode
+from torch.overrides import TorchFunctionMode, resolve_name
 from torch.utils._pytree import tree_map
 import torch.overrides
 from torch.utils.weak import WeakTensorKeyDictionary
 from torch._logging._internal import trace_structured
 from torch._logging.structured import from_traceback, intern_string
 
 import inspect
@@ -13,37 +13,38 @@
 import json
 import logging
 import weakref
 from functools import partial
 import itertools
 import os
 import types
+from collections import defaultdict
 
 
 uninteresting_dirs = (
     os.path.dirname(__file__),
     os.path.dirname(inspect.getfile(torch)),
 )
 
 
-def translate_args(f_locals, func):
+def translate_args(f_lcls, func):
     sig = inspect.signature(func)
     args = []
     kwargs = {}
 
     for param in sig.parameters.values():
-        if param.name in f_locals:
+        if param.name in f_lcls:
             if param.kind in (param.POSITIONAL_ONLY, param.POSITIONAL_OR_KEYWORD):
-                args.append(f_locals[param.name])
+                args.append(f_lcls[param.name])
             elif param.kind == param.KEYWORD_ONLY:
-                kwargs[param.name] = f_locals[param.name]
+                kwargs[param.name] = f_lcls[param.name]
             elif param.kind == param.VAR_POSITIONAL:
-                args.extend(f_locals[param.name])
+                args.extend(f_lcls[param.name])
             elif param.kind == param.VAR_KEYWORD:
-                kwargs.update(f_locals[param.name])
+                kwargs.update(f_lcls[param.name])
 
     return args, kwargs
 
 
 SOURCE_DUMPED = set()
 
 def dump_source(filename: str):
@@ -53,20 +54,33 @@
     trace_structured(
         "dump_source",
         metadata_fn=lambda: {"filename": intern_string(filename)},
         payload_fn=lambda: open(filename, 'r').read()
     )
 
 
-class LoggingMode(TorchDispatchMode):
+class LoggingMode(TorchFunctionMode):
     next_id: int
 
-    def __init__(self):
+    def __init__(self, skip=0):
         self.memo = WeakTensorKeyDictionary()
         self.next_id = 0
+        self.skip = skip
+        self.lines_traversed = defaultdict(set)
+
+    def __enter__(self):
+        frame = inspect.currentframe()
+        for _ in range(self.skip + 1):
+            frame = frame.f_back
+        self.frame = frame
+        super().__enter__()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        super().__exit__(exc_type, exc_val, exc_tb)
+        del self.frame  # clear reference cycle
 
     def _shortid(self, t: torch.Tensor) -> int:
         if t not in self.memo:
             self.memo[t] = self.next_id
             self.next_id += 1
         return self.memo[t]
 
@@ -83,61 +97,70 @@
                 "dtype": repr(a.dtype),
                 "shape": a.shape,
                 # TODO: other metadata; consider using MetaTensorDesc
             }
         else:
             return repr(a)
 
-    def __torch_dispatch__(self, func, tys, args=(), kwargs=None):
+    def __torch_function__(self, func, tys, args=(), kwargs=None):
         if kwargs is None:
             kwargs = {}
 
-        # Although we know the args/kwargs of the aten operator call,
-        # this may be several layers removed from the user code we're
-        # actually interested in instrumenting (e.g., imagine a torch
-        # API which is implemented in Python and eventually calls into
-        # C binding).  We'd like to report the args/kargs of the user
-        # call because this is more interpretable to the user.  To do
-        # this, we walk up the stack looking for the first frame that
-        # looks like user code.
+        # The more complicated user frame plan
+        #
+        # We would like to record multiple levels of frames, so that we can implement
+        # both step and next functionality in the debugger.  However, we don't want to
+        # unconditionally dump all the frames, as it's pretty common to be dozens of
+        # frame deep from top level launcher code that doesn't matter from the
+        # perspective of debugging.
+        #
+        # Intuitively, we do not need to record source code for any frame whose line
+        # number never changes over the course of execution.  Furthermore, once
+        # we have identified an unchanged frame, we can bypass traversing all of
+        # its parents (which necessarily must also be unchanged).
+
+        stack = []
+
+        # We'll maintain both the inner frame (callee) and the outer frame
+        # (caller), because we'd like to report args/kwargs of call sites, and
+        # to do that we need to look at the inner frame.  The outer frame is
+        # what you traditionally think of as going in the call stack though!
         cur_frame = inner_frame = inspect.currentframe()
         assert inner_frame is not None
         frame = inner_frame.f_back
+
+        def handle_frame(frame, lcls):
+            # The first frame is special, because I don't want to actually report
+            # the f_lcls of the torch function dispatch, it will often not be
+            # well defined
+            filename = frame.f_code.co_filename
+            file_id = intern_string(filename)
+            stack.append({
+                'name': frame.f_code.co_name,
+                'line': frame.f_lineno,
+                'filename': file_id,
+                'locals': self._json(lcls),
+            })
+            self.lines_traversed[file_id].add(frame.f_lineno)
+            if len(self.lines_traversed[file_id]) > 1:
+                dump_source(filename)
+
         while frame:
             if not frame.f_code.co_filename.startswith(uninteresting_dirs):
+                handle_frame(frame, frame.f_locals if frame.f_back is not None else {})
+
+            # Stop traversing once we've hit the context manager frame
+            if frame is self.frame:
                 break
+
             inner_frame = frame
             frame = frame.f_back
-        # At this point, frame is the user frame (caller), and inner_frame is
-        # the callee frame which has the f_locals of the call.  Now we extract
-        # the arguments.
-        if inner_frame is cur_frame:
-            # When the user frame is immediately before the inner frame, that
-            # means that the user actually did directly call into a C binding.
-            # In this case, the args/kwargs here are accurate-ish.  (The -ish
-            # is because our Python bindings sometimes do nontrivial
-            # translations of arguments so these args/kwargs may not be
-            # exactly what the user actually passed in.  However, these
-            # transformations are in principle all known to us and reversible.)
-            user_args, user_kwargs = args, kwargs
-        else:
-            # f_locals is all kwargs, we try to stuff as many positionally as
-            # possible, because the user might not even know what a function
-            # had named the positional args.
-            user_args, user_kwargs = translate_args(
-                inner_frame.f_locals,
-                types.FunctionType(inner_frame.f_code, inner_frame.f_globals)
-            )
+
         rs = func(*args, **kwargs)
-        dump_source(frame.f_code.co_filename)
         trace_structured("eager_dispatch", metadata_fn=lambda: {
-            "func": str(func),
+            "target": resolve_name(func),
+            "stack": stack,
             "args": self._json(args),
             "kwargs": self._json(kwargs),
-            "user_args": self._json(user_args),
-            "user_kwargs": self._json(user_kwargs),
-            "user_line": frame.f_lineno,
-            "user_name": frame.f_code.co_name,
-            "user_filename": intern_string(frame.f_code.co_filename),
-            "ret": self._json(rs)
+            "ret": self._json(rs),
         })
         return rs
```

### Comparing `torchdbg-0.1.0/PKG-INFO` & `torchdbg-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchdbg
-Version: 0.1.0
+Version: 0.2.0
 Summary: PyTorch centric eager mode debugger/tracer
 License: BSD-3
 Author: Edward Z. Yang
 Author-email: ezyang@meta.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

