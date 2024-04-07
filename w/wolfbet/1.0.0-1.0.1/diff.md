# Comparing `tmp/wolfbet-1.0.0.tar.gz` & `tmp/wolfbet-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolfbet-1.0.0.tar", max compression
+gzip compressed data, was "wolfbet-1.0.1.tar", max compression
```

## Comparing `wolfbet-1.0.0.tar` & `wolfbet-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      337 2024-04-07 16:16:49.221697 wolfbet-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 12:14:41.841727 wolfbet-1.0.0/README.md
--rw-r--r--   0        0        0    24347 2024-04-07 16:14:31.567613 wolfbet-1.0.0/wolfbet/__init__.py
--rw-r--r--   0        0        0      295 2024-04-07 12:44:21.812871 wolfbet-1.0.0/wolfbet/core/__init__.py
--rw-r--r--   0        0        0     4821 2024-04-07 13:41:29.471150 wolfbet-1.0.0/wolfbet/core/Config.py
--rw-r--r--   0        0        0     2120 2024-04-07 14:21:41.503109 wolfbet-1.0.0/wolfbet/core/Connections.py
--rw-r--r--   0        0        0     2049 2024-04-07 14:31:43.297770 wolfbet-1.0.0/wolfbet/core/Constant.py
--rw-r--r--   0        0        0      734 2024-04-07 14:16:23.772817 wolfbet-1.0.0/wolfbet/core/PPrint.py
--rw-r--r--   0        0        0     1201 2024-04-07 15:01:19.266816 wolfbet-1.0.0/wolfbet/core/Response.py
--rw-r--r--   0        0        0     1820 2024-04-07 13:45:21.219254 wolfbet-1.0.0/wolfbet/core/type.py
--rw-r--r--   0        0        0     3877 2024-04-07 15:58:37.263099 wolfbet-1.0.0/wolfbet/core/Utils.py
--rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 wolfbet-1.0.0/setup.py
--rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 wolfbet-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      337 2024-04-07 16:17:40.262196 wolfbet-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 12:14:41.841727 wolfbet-1.0.1/README.md
+-rw-r--r--   0        0        0    24347 2024-04-07 16:14:31.567613 wolfbet-1.0.1/wolfbet/__init__.py
+-rw-r--r--   0        0        0      295 2024-04-07 12:44:21.812871 wolfbet-1.0.1/wolfbet/core/__init__.py
+-rw-r--r--   0        0        0     4821 2024-04-07 13:41:29.471150 wolfbet-1.0.1/wolfbet/core/Config.py
+-rw-r--r--   0        0        0     2120 2024-04-07 14:21:41.503109 wolfbet-1.0.1/wolfbet/core/Connections.py
+-rw-r--r--   0        0        0     2049 2024-04-07 14:31:43.297770 wolfbet-1.0.1/wolfbet/core/Constant.py
+-rw-r--r--   0        0        0      734 2024-04-07 14:16:23.772817 wolfbet-1.0.1/wolfbet/core/PPrint.py
+-rw-r--r--   0        0        0     1201 2024-04-07 15:01:19.266816 wolfbet-1.0.1/wolfbet/core/Response.py
+-rw-r--r--   0        0        0     1820 2024-04-07 13:45:21.219254 wolfbet-1.0.1/wolfbet/core/type.py
+-rw-r--r--   0        0        0     3877 2024-04-07 15:58:37.263099 wolfbet-1.0.1/wolfbet/core/Utils.py
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 wolfbet-1.0.1/setup.py
+-rw-r--r--   0        0        0      533 1970-01-01 00:00:00.000000 wolfbet-1.0.1/PKG-INFO
```

### Comparing `wolfbet-1.0.0/wolfbet/__init__.py` & `wolfbet-1.0.1/wolfbet/__init__.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/wolfbet/core/Config.py` & `wolfbet-1.0.1/wolfbet/core/Config.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/wolfbet/core/Connections.py` & `wolfbet-1.0.1/wolfbet/core/Connections.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/wolfbet/core/Constant.py` & `wolfbet-1.0.1/wolfbet/core/Constant.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/wolfbet/core/PPrint.py` & `wolfbet-1.0.1/wolfbet/core/PPrint.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/wolfbet/core/Response.py` & `wolfbet-1.0.1/wolfbet/core/Response.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/wolfbet/core/type.py` & `wolfbet-1.0.1/wolfbet/core/type.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/wolfbet/core/Utils.py` & `wolfbet-1.0.1/wolfbet/core/Utils.py`

 * *Files identical despite different names*

### Comparing `wolfbet-1.0.0/setup.py` & `wolfbet-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['colorama>=0.4.6,<0.5.0', 'http-injector>=1.0.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'wolfbet',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': '',
     'long_description': '',
     'author': 'DesKaOne',
     'author_email': 'DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `wolfbet-1.0.0/PKG-INFO` & `wolfbet-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfbet
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: DesKaOne
 Author-email: DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

