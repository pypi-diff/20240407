# Comparing `tmp/py_libtrust-2.0.0.tar.gz` & `tmp/py_libtrust-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_libtrust-2.0.0.tar", max compression
+gzip compressed data, was "py_libtrust-2.1.0.tar", max compression
```

## Comparing `py_libtrust-2.0.0.tar` & `py_libtrust-2.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/LICENSE
--rw-r--r--   0        0        0     1881 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/README.md
--rw-r--r--   0        0        0      373 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/__init__.py
--rw-r--r--   0        0        0      137 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/exceptions.py
--rw-r--r--   0        0        0     9432 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/jsonsign.py
--rw-r--r--   0        0        0        0 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/__init__.py
--rw-r--r--   0        0        0     8898 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/ec_key.py
--rw-r--r--   0        0        0     3677 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/protocol.py
--rw-r--r--   0        0        0     7247 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/rs_key.py
--rw-r--r--   0        0        0     2601 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/keys/utils.py
--rw-r--r--   0        0        0     1409 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/libtrust/utils.py
--rw-r--r--   0        0        0      812 2024-04-07 07:13:33.594837 py_libtrust-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 py_libtrust-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/LICENSE
+-rw-r--r--   0        0        0     1881 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/README.md
+-rw-r--r--   0        0        0      373 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/__init__.py
+-rw-r--r--   0        0        0      137 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/exceptions.py
+-rw-r--r--   0        0        0     9432 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/jsonsign.py
+-rw-r--r--   0        0        0        0 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/keys/__init__.py
+-rw-r--r--   0        0        0     8898 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/keys/ec_key.py
+-rw-r--r--   0        0        0     3677 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/keys/protocol.py
+-rw-r--r--   0        0        0     7247 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/keys/rs_key.py
+-rw-r--r--   0        0        0     2601 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/keys/utils.py
+-rw-r--r--   0        0        0     1409 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/libtrust/utils.py
+-rw-r--r--   0        0        0      812 2024-04-07 07:18:42.533922 py_libtrust-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2684 1970-01-01 00:00:00.000000 py_libtrust-2.1.0/PKG-INFO
```

### Comparing `py_libtrust-2.0.0/LICENSE` & `py_libtrust-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/README.md` & `py_libtrust-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/libtrust/jsonsign.py` & `py_libtrust-2.1.0/libtrust/jsonsign.py`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/libtrust/keys/ec_key.py` & `py_libtrust-2.1.0/libtrust/keys/ec_key.py`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/libtrust/keys/protocol.py` & `py_libtrust-2.1.0/libtrust/keys/protocol.py`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/libtrust/keys/rs_key.py` & `py_libtrust-2.1.0/libtrust/keys/rs_key.py`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/libtrust/keys/utils.py` & `py_libtrust-2.1.0/libtrust/keys/utils.py`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/libtrust/utils.py` & `py_libtrust-2.1.0/libtrust/utils.py`

 * *Files identical despite different names*

### Comparing `py_libtrust-2.0.0/pyproject.toml` & `py_libtrust-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "py-libtrust"
-version = "2.0.0"
+version = "2.1.0"
 description = "Yet another docker/libtrust implement by python."
 license = "Apache-2.0"
 authors = ["shabbywu <shabbywu@qq.com>"]
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/py-libtrust"
 homepage = "https://github.com/shabbywu/py-libtrust"
 
 packages = [
     {include = "libtrust"}
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.6"
+python = ">=3.8"
 cryptography = ">= 37"
 typing-extensions = ">= 3.6.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
```

### Comparing `py_libtrust-2.0.0/PKG-INFO` & `py_libtrust-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 Metadata-Version: 2.1
 Name: py-libtrust
-Version: 2.0.0
+Version: 2.1.0
 Summary: Yet another docker/libtrust implement by python.
 Home-page: https://github.com/shabbywu/py-libtrust
 License: Apache-2.0
 Author: shabbywu
 Author-email: shabbywu@qq.com
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cryptography (>=37)
 Requires-Dist: typing-extensions (>=3.6.5)
```

