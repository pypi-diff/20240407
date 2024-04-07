# Comparing `tmp/corentin_regent_test-1.0.0.tar.gz` & `tmp/corentin_regent_test-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corentin_regent_test-1.0.0.tar", max compression
+gzip compressed data, was "corentin_regent_test-1.0.1.tar", max compression
```

## Comparing `corentin_regent_test-1.0.0.tar` & `corentin_regent_test-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1073 2024-04-07 06:04:23.838101 corentin_regent_test-1.0.0/LICENSE
--rw-r--r--   0        0        0     3294 2024-04-07 06:04:23.838101 corentin_regent_test-1.0.0/README.rst
--rw-r--r--   0        0        0       51 2024-04-07 06:04:23.838101 corentin_regent_test-1.0.0/corentin_regent_test/__init__.py
--rw-r--r--   0        0        0      116 2024-04-07 06:04:23.838101 corentin_regent_test-1.0.0/corentin_regent_test/_main.py
--rw-r--r--   0        0        0        0 2024-04-07 06:04:23.838101 corentin_regent_test-1.0.0/corentin_regent_test/py.typed
--rw-r--r--   0        0        0     1884 2024-04-07 06:04:23.838101 corentin_regent_test-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4180 1970-01-01 00:00:00.000000 corentin_regent_test-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-07 06:12:19.662191 corentin_regent_test-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3294 2024-04-07 06:12:19.662191 corentin_regent_test-1.0.1/README.rst
+-rw-r--r--   0        0        0       51 2024-04-07 06:12:19.662191 corentin_regent_test-1.0.1/corentin_regent_test/__init__.py
+-rw-r--r--   0        0        0      116 2024-04-07 06:12:19.662191 corentin_regent_test-1.0.1/corentin_regent_test/_main.py
+-rw-r--r--   0        0        0        0 2024-04-07 06:12:19.662191 corentin_regent_test-1.0.1/corentin_regent_test/py.typed
+-rw-r--r--   0        0        0     1884 2024-04-07 06:12:38.214189 corentin_regent_test-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4180 1970-01-01 00:00:00.000000 corentin_regent_test-1.0.1/PKG-INFO
```

### Comparing `corentin_regent_test-1.0.0/LICENSE` & `corentin_regent_test-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `corentin_regent_test-1.0.0/README.rst` & `corentin_regent_test-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `corentin_regent_test-1.0.0/pyproject.toml` & `corentin_regent_test-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "corentin-regent-test"
-version = "1.0.0"
+version = "1.0.1"
 homepage = "https://github.com/corentin-regent/corentin-regent-test"
 description = "Cool project built with Tempoet"
 authors = ["Corentin Régent <corentin.regent.pro@gmail.com>"]
 readme = "README.rst"
 license =  "MIT"
 
 classifiers = [
```

### Comparing `corentin_regent_test-1.0.0/PKG-INFO` & `corentin_regent_test-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corentin-regent-test
-Version: 1.0.0
+Version: 1.0.1
 Summary: Cool project built with Tempoet
 Home-page: https://github.com/corentin-regent/corentin-regent-test
 License: MIT
 Author: Corentin Régent
 Author-email: corentin.regent.pro@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

