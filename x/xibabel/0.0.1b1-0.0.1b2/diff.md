# Comparing `tmp/xibabel-0.0.1b1.tar.gz` & `tmp/xibabel-0.0.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xibabel-0.0.1b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xibabel-0.0.1b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xibabel-0.0.1b1.tar` & `xibabel-0.0.1b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3241 2024-04-06 17:55:02.342516 xibabel-0.0.1b1/README.md
--rw-r--r--   0        0        0     1172 2024-04-06 22:04:37.266298 xibabel-0.0.1b1/pyproject.toml
--rw-r--r--   0        0        0      114 2024-04-06 22:03:34.775306 xibabel-0.0.1b1/src/xibabel/__init__.py
--rw-r--r--   0        0        0      571 2024-04-06 17:55:02.346667 xibabel-0.0.1b1/src/xibabel/bench/bench_nib_xib_load.py
--rw-r--r--   0        0        0    26374 2024-04-06 17:55:02.346881 xibabel-0.0.1b1/src/xibabel/loaders.py
--rw-r--r--   0        0        0       20 2024-04-06 17:55:02.347197 xibabel-0.0.1b1/src/xibabel/testing/.gitignore
--rw-r--r--   0        0        0     2584 2024-04-06 17:55:02.347343 xibabel-0.0.1b1/src/xibabel/testing/__init__.py
--rw-r--r--   0        0        0      627 2024-04-06 17:55:02.347577 xibabel-0.0.1b1/src/xibabel/testing/__main__.py
--rw-r--r--   0        0        0     5225 2024-04-06 17:55:02.347801 xibabel-0.0.1b1/src/xibabel/testing/fetcher.py
--rw-r--r--   0        0        0      463 2024-04-06 17:55:02.348095 xibabel-0.0.1b1/src/xibabel/testing/test_files.yml
--rw-r--r--   0        0        0      396 2024-04-06 17:55:02.348320 xibabel-0.0.1b1/src/xibabel/testing/test_sets.yml
--rw-r--r--   0        0        0        0 2024-04-06 17:55:02.348361 xibabel-0.0.1b1/src/xibabel/tests/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-06 17:55:02.348672 xibabel-0.0.1b1/src/xibabel/tests/conftest.py
--rw-r--r--   0        0        0      332 2024-04-06 17:55:02.348819 xibabel-0.0.1b1/src/xibabel/tests/markers.py
--rw-r--r--   0        0        0     1306 2024-04-06 17:55:02.349085 xibabel-0.0.1b1/src/xibabel/tests/run_server.py
--rw-r--r--   0        0        0    20938 2024-04-06 17:55:02.349301 xibabel-0.0.1b1/src/xibabel/tests/test_loaders.py
--rw-r--r--   0        0        0     1205 2024-04-06 17:55:02.349677 xibabel-0.0.1b1/src/xibabel/tests/test_merge.py
--rw-r--r--   0        0        0     2855 2024-04-06 17:55:02.349851 xibabel-0.0.1b1/src/xibabel/tests/test_scripting.py
--rw-r--r--   0        0        0     2264 2024-04-06 17:55:02.350007 xibabel-0.0.1b1/src/xibabel/tests/test_testing.py
--rw-r--r--   0        0        0      794 2024-04-06 17:55:02.350222 xibabel-0.0.1b1/src/xibabel/xutils.py
--rw-r--r--   0        0        0     4808 1970-01-01 00:00:00.000000 xibabel-0.0.1b1/PKG-INFO
+-rw-r--r--   0        0        0     3241 2024-04-06 17:55:02.342516 xibabel-0.0.1b2/README.md
+-rw-r--r--   0        0        0     1172 2024-04-06 22:04:37.266298 xibabel-0.0.1b2/pyproject.toml
+-rw-r--r--   0        0        0      200 2024-04-06 22:48:04.482036 xibabel-0.0.1b2/src/xibabel/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-06 17:55:02.346667 xibabel-0.0.1b2/src/xibabel/bench/bench_nib_xib_load.py
+-rw-r--r--   0        0        0    26374 2024-04-06 17:55:02.346881 xibabel-0.0.1b2/src/xibabel/loaders.py
+-rw-r--r--   0        0        0       20 2024-04-06 17:55:02.347197 xibabel-0.0.1b2/src/xibabel/testing/.gitignore
+-rw-r--r--   0        0        0     2584 2024-04-06 17:55:02.347343 xibabel-0.0.1b2/src/xibabel/testing/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-06 17:55:02.347577 xibabel-0.0.1b2/src/xibabel/testing/__main__.py
+-rw-r--r--   0        0        0     5225 2024-04-06 17:55:02.347801 xibabel-0.0.1b2/src/xibabel/testing/fetcher.py
+-rw-r--r--   0        0        0      463 2024-04-06 17:55:02.348095 xibabel-0.0.1b2/src/xibabel/testing/test_files.yml
+-rw-r--r--   0        0        0      396 2024-04-06 17:55:02.348320 xibabel-0.0.1b2/src/xibabel/testing/test_sets.yml
+-rw-r--r--   0        0        0        0 2024-04-06 17:55:02.348361 xibabel-0.0.1b2/src/xibabel/tests/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-06 17:55:02.348672 xibabel-0.0.1b2/src/xibabel/tests/conftest.py
+-rw-r--r--   0        0        0      332 2024-04-06 17:55:02.348819 xibabel-0.0.1b2/src/xibabel/tests/markers.py
+-rw-r--r--   0        0        0     1306 2024-04-06 17:55:02.349085 xibabel-0.0.1b2/src/xibabel/tests/run_server.py
+-rw-r--r--   0        0        0    20938 2024-04-06 17:55:02.349301 xibabel-0.0.1b2/src/xibabel/tests/test_loaders.py
+-rw-r--r--   0        0        0     1205 2024-04-06 17:55:02.349677 xibabel-0.0.1b2/src/xibabel/tests/test_merge.py
+-rw-r--r--   0        0        0     2855 2024-04-06 17:55:02.349851 xibabel-0.0.1b2/src/xibabel/tests/test_scripting.py
+-rw-r--r--   0        0        0     2264 2024-04-06 17:55:02.350007 xibabel-0.0.1b2/src/xibabel/tests/test_testing.py
+-rw-r--r--   0        0        0      794 2024-04-06 17:55:02.350222 xibabel-0.0.1b2/src/xibabel/xutils.py
+-rw-r--r--   0        0        0     4814 1970-01-01 00:00:00.000000 xibabel-0.0.1b2/PKG-INFO
```

### Comparing `xibabel-0.0.1b1/README.md` & `xibabel-0.0.1b2/README.md`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/pyproject.toml` & `xibabel-0.0.1b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/bench/bench_nib_xib_load.py` & `xibabel-0.0.1b2/src/xibabel/bench/bench_nib_xib_load.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/loaders.py` & `xibabel-0.0.1b2/src/xibabel/loaders.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/testing/__init__.py` & `xibabel-0.0.1b2/src/xibabel/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/testing/__main__.py` & `xibabel-0.0.1b2/src/xibabel/testing/__main__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/testing/fetcher.py` & `xibabel-0.0.1b2/src/xibabel/testing/fetcher.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/tests/conftest.py` & `xibabel-0.0.1b2/src/xibabel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/tests/run_server.py` & `xibabel-0.0.1b2/src/xibabel/tests/run_server.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/tests/test_loaders.py` & `xibabel-0.0.1b2/src/xibabel/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/tests/test_merge.py` & `xibabel-0.0.1b2/src/xibabel/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/tests/test_scripting.py` & `xibabel-0.0.1b2/src/xibabel/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/tests/test_testing.py` & `xibabel-0.0.1b2/src/xibabel/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/src/xibabel/xutils.py` & `xibabel-0.0.1b2/src/xibabel/xutils.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1b1/PKG-INFO` & `xibabel-0.0.1b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: xibabel
-Version: 0.0.1b1
-Summary: Init for Xibabel package
+Version: 0.0.1b2
+Summary: Xibabel neuroimaging interface
 Author-email: Matthew Brett <matthew.brett@gmail.com>, Paul Ivanov <pi@berkeley.edu>, "Christopher J. Markiewicz" <markiewicz@stanford.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: xarray
 Requires-Dist: dask
```

