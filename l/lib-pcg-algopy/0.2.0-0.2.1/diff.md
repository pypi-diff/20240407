# Comparing `tmp/lib_pcg_algopy-0.2.0.tar.gz` & `tmp/lib_pcg_algopy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib_pcg_algopy-0.2.0.tar", max compression
+gzip compressed data, was "lib_pcg_algopy-0.2.1.tar", max compression
```

## Comparing `lib_pcg_algopy-0.2.0.tar` & `lib_pcg_algopy-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    11636 2024-03-30 21:47:34.838689 lib_pcg_algopy-0.2.0/README.md
--rw-r--r--   0        0        0      303 2024-04-06 15:54:14.290298 lib_pcg_algopy-0.2.0/lib_pcg/__init__.py
--rw-r--r--   0        0        0      251 2024-04-06 13:55:27.698575 lib_pcg_algopy-0.2.0/lib_pcg/consts.py
--rw-r--r--   0        0        0     2957 2024-04-06 13:55:57.606432 lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_64_32.py
--rw-r--r--   0        0        0     2364 2024-04-06 13:56:18.658332 lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_double_64_32.py
--rw-r--r--   0        0        0     4166 2024-04-06 15:39:05.592300 lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_quadruple_64_32.py
--rw-r--r--   0        0        0     1535 2024-04-06 15:56:58.465767 lib_pcg_algopy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 lib_pcg_algopy-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11636 2024-03-30 21:47:34.838689 lib_pcg_algopy-0.2.1/README.md
+-rw-r--r--   0        0        0      303 2024-04-06 15:54:14.290298 lib_pcg_algopy-0.2.1/lib_pcg/__init__.py
+-rw-r--r--   0        0        0      251 2024-04-06 13:55:27.698575 lib_pcg_algopy-0.2.1/lib_pcg/consts.py
+-rw-r--r--   0        0        0        0 2024-04-07 17:16:51.217844 lib_pcg_algopy-0.2.1/lib_pcg/py.typed
+-rw-r--r--   0        0        0     2844 2024-04-07 16:32:17.909072 lib_pcg_algopy-0.2.1/lib_pcg/xsh_rr_64_32.py
+-rw-r--r--   0        0        0     2364 2024-04-06 13:56:18.658332 lib_pcg_algopy-0.2.1/lib_pcg/xsh_rr_double_64_32.py
+-rw-r--r--   0        0        0     4166 2024-04-06 15:39:05.592300 lib_pcg_algopy-0.2.1/lib_pcg/xsh_rr_quadruple_64_32.py
+-rw-r--r--   0        0        0     1549 2024-04-07 17:19:18.377164 lib_pcg_algopy-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    12130 1970-01-01 00:00:00.000000 lib_pcg_algopy-0.2.1/PKG-INFO
```

### Comparing `lib_pcg_algopy-0.2.0/README.md` & `lib_pcg_algopy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_64_32.py` & `lib_pcg_algopy-0.2.1/lib_pcg/xsh_rr_64_32.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,25 @@
-from typing import TypeAlias
-
 from algopy import Bytes, UInt64, arc4, op, subroutine, urange
 
 from lib_pcg.consts import PCG_DEFAULT_INCREMENT, PCG_DEFAULT_MULTIPLIER
 
-PCG32_STATE: TypeAlias = UInt64
-
 
 @subroutine
-def pcg32_init(initial_state: PCG32_STATE) -> PCG32_STATE:
+def pcg32_init(initial_state: UInt64) -> UInt64:
     return __pcg32_init(initial_state, UInt64(PCG_DEFAULT_INCREMENT))
 
 
 @subroutine
 def pcg32_random(
-    state: PCG32_STATE,
+    state: UInt64,
     bit_size: UInt64,
     lower_bound: UInt64,
     upper_bound: UInt64,
     length: UInt64,
-) -> tuple[PCG32_STATE, Bytes]:
+) -> tuple[UInt64, Bytes]:
     result = Bytes()
 
     assert length < 2**16
     result += arc4.UInt16(length).bytes
 
     assert bit_size == 8 or bit_size == 16 or bit_size == 32
     byte_size = bit_size >> 3
@@ -59,31 +55,31 @@
                 byte_size,
             )
 
     return state, result
 
 
 @subroutine
-def __pcg32_init(initial_state: PCG32_STATE, incr: UInt64) -> PCG32_STATE:
+def __pcg32_init(initial_state: UInt64, incr: UInt64) -> UInt64:
     state = __pcg32_step(UInt64(0), incr)
     _high_addw, state = op.addw(state, initial_state)
 
     return __pcg32_step(state, incr)
 
 
 @subroutine
-def __pcg32_step(state: PCG32_STATE, incr: UInt64) -> PCG32_STATE:
+def __pcg32_step(state: UInt64, incr: UInt64) -> UInt64:
     _high_mul, low_mul = op.mulw(state, PCG_DEFAULT_MULTIPLIER)
     _high_add, low_add = op.addw(low_mul, incr)
 
     return low_add
 
 
 @subroutine
-def __pcg32_random(state: PCG32_STATE) -> tuple[PCG32_STATE, UInt64]:
+def __pcg32_random(state: UInt64) -> tuple[UInt64, UInt64]:
     return __pcg32_step(state, UInt64(PCG_DEFAULT_INCREMENT)), __pcg32_output(state)
 
 
 @subroutine
 def __pcg32_output(value: UInt64) -> UInt64:
     return __pcg32_rotation(
         __mask_to_32bits(((value >> 18) ^ value) >> 27), value >> 59
```

### Comparing `lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_double_64_32.py` & `lib_pcg_algopy-0.2.1/lib_pcg/xsh_rr_double_64_32.py`

 * *Files identical despite different names*

### Comparing `lib_pcg_algopy-0.2.0/lib_pcg/xsh_rr_quadruple_64_32.py` & `lib_pcg_algopy-0.2.1/lib_pcg/xsh_rr_quadruple_64_32.py`

 * *Files identical despite different names*

### Comparing `lib_pcg_algopy-0.2.0/pyproject.toml` & `lib_pcg_algopy-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lib-pcg-algopy"
-version = "0.2.0"
+version = "0.2.1"
 description = "PCG library implemented using Algorand Python"
 authors = ["CiottiGiorgio <giorgio.ciotti@algorand.foundation>"]
 readme = "README.md"
 packages = [{include = "lib_pcg"}]
 
 [tool.poetry.dependencies]
 python = "^3.12"
@@ -38,15 +38,15 @@
 allow-star-arg-any = true
 suppress-none-returning = true
 
 [tool.pytest.ini_options]
 pythonpath = ["smart_contracts", "tests"]
 
 [tool.mypy]
-files = "smart_contracts/"
+files = ["smart_contracts/", "lib_pcg/"]
 python_version = "3.12"
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
```

### Comparing `lib_pcg_algopy-0.2.0/PKG-INFO` & `lib_pcg_algopy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-pcg-algopy
-Version: 0.2.0
+Version: 0.2.1
 Summary: PCG library implemented using Algorand Python
 Author: CiottiGiorgio
 Author-email: giorgio.ciotti@algorand.foundation
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: algokit-utils (>=2.2.0,<3.0.0)
```

