# Comparing `tmp/kkpyai-0.2.1.tar.gz` & `tmp/kkpyai-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.2.1.tar", max compression
+gzip compressed data, was "kkpyai-0.2.2.tar", max compression
```

## Comparing `kkpyai-0.2.1.tar` & `kkpyai-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.2.1/LICENSE
--rw-r--r--   0        0        0       47 2024-04-07 15:06:36.235438 kkpyai-0.2.1/README.md
--rw-r--r--   0        0        0     1668 2024-04-07 19:19:31.834471 kkpyai-0.2.1/kkpyai/kktorch.py
--rw-r--r--   0        0        0      344 2024-04-07 19:19:31.833129 kkpyai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 kkpyai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.2.2/LICENSE
+-rw-r--r--   0        0        0       47 2024-04-07 15:06:36.235438 kkpyai-0.2.2/README.md
+-rw-r--r--   0        0        0     1822 2024-04-07 20:38:29.520230 kkpyai-0.2.2/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      409 2024-04-07 20:40:45.907885 kkpyai-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 kkpyai-0.2.2/PKG-INFO
```

### Comparing `kkpyai-0.2.1/LICENSE` & `kkpyai-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyai-0.2.1/kkpyai/kktorch.py` & `kkpyai-0.2.2/kkpyai/kktorch.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 import kkpyutil as util
 import torch as tc
 
 
 # region tensor ops
 
 class TensorFactory:
-    def __init__(self, device='cpu', dtype=tc.float32, requires_grad=False):
-        self.device = device
+    def __init__(self, device=None, dtype=tc.float32, requires_grad=False):
+        self.device = tc.device(device) if device else self.find_fastest_device()
         self.dtype = dtype
         self.requires_grad = requires_grad
 
-    def init(self, device=None, dtype=tc.float32, requires_grad=False):
-        gpu = 'mps' if util.PLATFORM == 'Darwin' else 'cuda'
-        self.device = tc.device(device or (gpu if self.can_use_gpu() else 'cpu'))
+    def init(self, device: str = '', dtype=tc.float32, requires_grad=False):
+        self.device = tc.device(device) if device else self.find_fastest_device()
         self.dtype = dtype
         self.requires_grad = requires_grad
 
     @staticmethod
-    def can_use_gpu():
+    def find_fastest_device():
         """
         - Apple Silicon uses Apple's own Metal Performance Shaders (MPS) instead of CUDA
         """
-        return tc.backends.mps.is_available() if util.PLATFORM == 'Darwin' else tc.cuda.is_available()
+        if util.PLATFORM == 'Darwin':
+            return 'mps' if tc.backends.mps.is_available() else 'cpu'
+        if tc.cuda.is_available():
+            return 'cuda'
+        return 'cpu'
 
     def ramp(self, size: typing.Union[list, tuple], start=1):
         """
         - ramp is easier to understand than random numbers
         - so they can come in handy for debugging and test-drive
         """
         end = start + functools.reduce(operator.mul, size)
@@ -41,7 +44,15 @@
         - to start a new reproducible sequence, call this method with a new seed
         """
         tc.manual_seed(seed)
         return tc.rand(size, device=self.device, dtype=self.dtype, requires_grad=self.requires_grad)
 
 
 # endregion
+
+
+def test():
+    pass
+
+
+if __name__ == '__main__':
+    test()
```

