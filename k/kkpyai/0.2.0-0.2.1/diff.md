# Comparing `tmp/kkpyai-0.2.0.tar.gz` & `tmp/kkpyai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kkpyai-0.2.0.tar", max compression
+gzip compressed data, was "kkpyai-0.2.1.tar", max compression
```

## Comparing `kkpyai-0.2.0.tar` & `kkpyai-0.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.2.0/LICENSE
--rw-r--r--   0        0        0       47 2024-04-07 15:06:36.235438 kkpyai-0.2.0/README.md
--rw-r--r--   0        0        0     1544 2024-04-07 17:21:56.093160 kkpyai-0.2.0/kkpyai/kktorch.py
--rw-r--r--   0        0        0      344 2024-04-07 17:25:15.523731 kkpyai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 kkpyai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:06:36.235377 kkpyai-0.2.1/LICENSE
+-rw-r--r--   0        0        0       47 2024-04-07 15:06:36.235438 kkpyai-0.2.1/README.md
+-rw-r--r--   0        0        0     1668 2024-04-07 19:19:31.834471 kkpyai-0.2.1/kkpyai/kktorch.py
+-rw-r--r--   0        0        0      344 2024-04-07 19:19:31.833129 kkpyai-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      437 1970-01-01 00:00:00.000000 kkpyai-0.2.1/PKG-INFO
```

### Comparing `kkpyai-0.2.0/LICENSE` & `kkpyai-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kkpyai-0.2.0/kkpyai/kktorch.py` & `kkpyai-0.2.1/kkpyai/kktorch.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,20 +12,23 @@
     def __init__(self, device='cpu', dtype=tc.float32, requires_grad=False):
         self.device = device
         self.dtype = dtype
         self.requires_grad = requires_grad
 
     def init(self, device=None, dtype=tc.float32, requires_grad=False):
         gpu = 'mps' if util.PLATFORM == 'Darwin' else 'cuda'
-        self.device = device or (gpu if self.can_use_gpu() else 'cpu')
+        self.device = tc.device(device or (gpu if self.can_use_gpu() else 'cpu'))
         self.dtype = dtype
         self.requires_grad = requires_grad
 
     @staticmethod
     def can_use_gpu():
+        """
+        - Apple Silicon uses Apple's own Metal Performance Shaders (MPS) instead of CUDA
+        """
         return tc.backends.mps.is_available() if util.PLATFORM == 'Darwin' else tc.cuda.is_available()
 
     def ramp(self, size: typing.Union[list, tuple], start=1):
         """
         - ramp is easier to understand than random numbers
         - so they can come in handy for debugging and test-drive
         """
```

