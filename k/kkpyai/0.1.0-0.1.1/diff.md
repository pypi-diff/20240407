# Comparing `tmp/kkpyai-0.1.0.tar.gz` & `tmp/kkpyai-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.1.0.tar", max compression
+gzip compressed data, was "kkpyai-0.1.1.tar", max compression
```

## Comparing `kkpyai-0.1.0.tar` & `kkpyai-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.1.0/LICENSE
--rw-r--r--   0        0        0       47 2024-04-07 15:06:36.235438 kkpyai-0.1.0/README.md
--rw-r--r--   0        0        0     1037 2024-04-07 15:32:24.512282 kkpyai-0.1.0/kkpyai/kktorch.py
--rw-r--r--   0        0        0      344 2024-04-07 15:10:21.295249 kkpyai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 kkpyai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.1.1/LICENSE
+-rw-r--r--   0        0        0       47 2024-04-07 15:06:36.235438 kkpyai-0.1.1/README.md
+-rw-r--r--   0        0        0     1126 2024-04-07 15:39:20.872738 kkpyai-0.1.1/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      344 2024-04-07 15:40:52.091373 kkpyai-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 kkpyai-0.1.1/PKG-INFO
```

### Comparing `kkpyai-0.1.0/LICENSE` & `kkpyai-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyai-0.1.0/kkpyai/kktorch.py` & `kkpyai-0.1.1/kkpyai/kktorch.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import functools
+import operator
 import typing
 # 3rd party
 import kkpyutil as util
 import torch as tc
 
 
 # region tensor ops
@@ -13,15 +15,16 @@
         self.requires_grad = requires_grad
 
     def init(self, device='cpu', dtype=tc.float32, requires_grad=False):
         self.device = device
         self.dtype = dtype
         self.requires_grad = requires_grad
 
-    def ramp(self, size: typing.Union[list, tuple], start, end):
+    def ramp(self, size: typing.Union[list, tuple], start=1):
+        end = start + functools.reduce(operator.mul, size)
         return tc.arange(start, end).reshape(*size).to(self.device, self.dtype, self.requires_grad)
 
     def rand_repro(self, size: typing.Union[list, tuple], seed=42):
         """
         - to reproduce a random tensor n times, simply call this method with the same seed
         - to start a new reproducible sequence, call this method with a new seed
         """
```

