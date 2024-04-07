# Comparing `tmp/ig_trading_lib-0.2.0.tar.gz` & `tmp/ig_trading_lib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ig_trading_lib-0.2.0.tar", max compression
+gzip compressed data, was "ig_trading_lib-0.3.0.tar", max compression
```

## Comparing `ig_trading_lib-0.2.0.tar` & `ig_trading_lib-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1071 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/LICENSE
--rw-r--r--   0        0        0     1310 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/README.md
--rw-r--r--   0        0        0      278 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/__init__.py
--rw-r--r--   0        0        0      136 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/authentication/__init__.py
--rw-r--r--   0        0        0      296 2024-03-26 23:46:50.927108 ig_trading_lib-0.2.0/ig_trading_lib/authentication/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5065 2024-03-26 23:46:51.103110 ig_trading_lib-0.2.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc
--rw-r--r--   0        0        0     1927 2024-03-26 23:46:51.123110 ig_trading_lib-0.2.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     4752 2024-03-26 23:46:50.927108 ig_trading_lib-0.2.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0     4636 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/authentication/cache.py
--rw-r--r--   0        0        0     1117 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/authentication/models.py
--rw-r--r--   0        0        0     4578 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/authentication/service.py
--rw-r--r--   0        0        0        0 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/markets/__init__.py
--rw-r--r--   0        0        0        0 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/trading/__init__.py
--rw-r--r--   0        0        0      173 2024-03-26 23:46:51.331112 ig_trading_lib-0.2.0/ig_trading_lib/trading/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      850 2024-03-26 23:46:51.343112 ig_trading_lib-0.2.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0      643 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/trading/models.py
--rw-r--r--   0        0        0      134 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/__init__.py
--rw-r--r--   0        0        0      345 2024-03-26 23:46:51.331112 ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     5424 2024-03-26 23:46:51.331112 ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     2732 2024-03-26 23:46:51.363112 ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0     5097 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/models.py
--rw-r--r--   0        0        0     2531 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/service.py
--rw-r--r--   0        0        0      315 2024-03-26 23:46:34.390895 ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/__init__.py
--rw-r--r--   0        0        0      452 2024-03-26 23:46:51.471114 ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    10549 2024-03-26 23:46:51.475113 ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc
--rw-r--r--   0        0        0     5566 2024-03-26 23:46:51.503114 ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc
--rw-r--r--   0        0        0    11119 2024-03-26 23:46:34.394895 ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/models.py
--rw-r--r--   0        0        0     5901 2024-03-26 23:46:34.394895 ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/service.py
--rw-r--r--   0        0        0      522 2024-03-26 23:46:34.394895 ig_trading_lib-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 ig_trading_lib-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1310 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/README.md
+-rw-r--r--   0        0        0      278 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/__init__.py
+-rw-r--r--   0        0        0      136 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__init__.py
+-rw-r--r--   0        0        0      296 2024-04-07 21:42:39.687569 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5065 2024-04-07 21:42:39.863568 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc
+-rw-r--r--   0        0        0     1927 2024-04-07 21:42:39.879568 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     4752 2024-04-07 21:42:39.691569 ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0     4636 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/cache.py
+-rw-r--r--   0        0        0     1117 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/models.py
+-rw-r--r--   0        0        0     4578 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/authentication/service.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/markets/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/__init__.py
+-rw-r--r--   0        0        0      173 2024-04-07 21:42:40.215566 ig_trading_lib-0.3.0/ig_trading_lib/trading/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      850 2024-04-07 21:42:40.223566 ig_trading_lib-0.3.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0      643 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/models.py
+-rw-r--r--   0        0        0      134 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__init__.py
+-rw-r--r--   0        0        0      345 2024-04-07 21:42:40.215566 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     5424 2024-04-07 21:42:40.215566 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     2732 2024-04-07 21:42:40.247566 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0     5097 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/models.py
+-rw-r--r--   0        0        0     2531 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/service.py
+-rw-r--r--   0        0        0      315 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__init__.py
+-rw-r--r--   0        0        0      452 2024-04-07 21:42:40.295566 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    10549 2024-04-07 21:42:40.299566 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0        0        0     5566 2024-04-07 21:42:40.327566 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc
+-rw-r--r--   0        0        0    11119 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/models.py
+-rw-r--r--   0        0        0     5901 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/service.py
+-rw-r--r--   0        0        0      547 2024-04-07 21:42:19.487648 ig_trading_lib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2092 1970-01-01 00:00:00.000000 ig_trading_lib-0.3.0/PKG-INFO
```

### Comparing `ig_trading_lib-0.2.0/LICENSE` & `ig_trading_lib-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/README.md` & `ig_trading_lib-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/cache.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 4636 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 1c12 0000  a.......Z^.f....
+00000000: 610d 0d0a 0000 0000 3b13 1366 1c12 0000  a.......;..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 6d04 5a04 0100 6400  d.l.m.Z.m.Z...d.
 00000050: 6403 6c05 6d06 5a06 0100 6400 6404 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 0100 6400 6405 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 6d0b 5a0b 0100 6406 6407 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 1117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 5d04 0000  a.......Z^.f]...
+00000000: 610d 0d0a 0000 0000 3b13 1366 5d04 0000  a.......;..f]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a00 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 0100 6400 6403 6c05  m.Z.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6501 6404 6405 6406 6702  m.Z...e.d.d.d.g.
 00000060: 8302 5a07 4700 6407 6408 8400 6408 6506  ..Z.G.d.d...d.e.
 00000070: 8303 5a08 4700 6409 640a 8400 640a 6506  ..Z.G.d.d...d.e.
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/authentication/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 4578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 e211 0000  a.......Z^.f....
+00000000: 610d 0d0a 0000 0000 3b13 1366 e211 0000  a.......;..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7800 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d01 5a01  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c02 6d03 5a03 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6401 6c04 5a04 6400 6404 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6405 6406 6c07 6d08 5a08 0100 6405  ..d.d.l.m.Z...d.
 00000070: 6407 6c09 6d0a 5a0a 0100 6500 a00b 650c  d.l.m.Z...e...e.
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/authentication/cache.py` & `ig_trading_lib-0.3.0/ig_trading_lib/authentication/cache.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/authentication/models.py` & `ig_trading_lib-0.3.0/ig_trading_lib/authentication/models.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/authentication/service.py` & `ig_trading_lib-0.3.0/ig_trading_lib/authentication/service.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 643 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 8302 0000  a.......Z^.f....
+00000000: 610d 0d0a 0000 0000 3b13 1366 8302 0000  a.......;..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6503 8303 5a04 6501 6405 1900 5a05 6501  e...Z.e.d...Z.e.
 00000060: 6406 1900 5a06 6407 5300 2908 e900 0000  d...Z.d.S.).....
 00000070: 0029 01da 074c 6974 6572 616c 2901 da09  .)...Literal)...
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/models.py` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/models.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 5097 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 e913 0000  a.......Z^.f....
+00000000: 610d 0d0a 0000 0000 3b13 1366 e913 0000  a.......;..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6400  m.Z.m.Z.m.Z...d.
 00000060: 6404 6c08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  d.l.m.Z.m.Z.m.Z.
 00000070: 6d0c 5a0c 6d0d 5a0d 6d0e 5a0e 0100 6405  m.Z.m.Z.m.Z...d.
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 2531 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 e309 0000  a.......Z^.f....
+00000000: 610d 0d0a 0000 0000 3b13 1366 e309 0000  a.......;..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7000 0000 6400  .....@...sp...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 0100 6406 6407 6c06 6d09 5a09  m.Z...d.d.l.m.Z.
 00000070: 0100 6500 a00a 650b a101 5a0c 4700 6408  ..e...e...Z.G.d.
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/models.py` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/models.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/orders/service.py` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/orders/service.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/models.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 11119 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 6f2b 0000  a.......Z^.fo+..
+00000000: 610d 0d0a 0000 0000 3b13 1366 6f2b 0000  a.......;..fo+..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 e000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000060: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6404 6405 6c0e 6d0f 5a0f 6d10 5a10  ..d.d.l.m.Z.m.Z.
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/__pycache__/service.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Mar 26 23:46:34 2024 UTC, .py size: 5901 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5a5e 0366 0d17 0000  a.......Z^.f....
+00000000: 610d 0d0a 0000 0000 3b13 1366 0d17 0000  a.......;..f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7c00 0000 6400  .....@...s|...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6404 6405 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b 5a0b  m.Z.m.Z.m.Z.m.Z.
 00000070: 0100 6406 6407 6c06 6d0c 5a0c 0100 6500  ..d.d.l.m.Z...e.
```

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/models.py` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/models.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/ig_trading_lib/trading/positions/service.py` & `ig_trading_lib-0.3.0/ig_trading_lib/trading/positions/service.py`

 * *Files identical despite different names*

### Comparing `ig_trading_lib-0.2.0/pyproject.toml` & `ig_trading_lib-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
-name = "ig_trading_lib"
-version = "0.2.0"
+name = "ig-trading-lib"
+version = "0.3.0"
 description = "A Python library for IG Trading."
 authors = ["Evgeny Aleshin"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.31.0"
 pydantic = "^2.6.3"
 cryptography = "^42.0.5"
+python-dotenv = "^1.0.1"
 
 [tool.poetry.extras]
 trading = []
 markets = []
 account = []
 streaming = []
```

### Comparing `ig_trading_lib-0.2.0/PKG-INFO` & `ig_trading_lib-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ig_trading_lib
-Version: 0.2.0
+Name: ig-trading-lib
+Version: 0.3.0
 Summary: A Python library for IG Trading.
 License: MIT
 Author: Evgeny Aleshin
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: account
 Provides-Extra: markets
 Provides-Extra: streaming
 Provides-Extra: trading
 Requires-Dist: cryptography (>=42.0.5,<43.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
+Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # IG Trading Library
 
 This is a Python library designed to interface with the IG Trading platform. It provides a straightforward and Pythonic way to interact with the IG Trading API, allowing for the automation of trading tasks, management of accounts, access to market data, and more.
```

