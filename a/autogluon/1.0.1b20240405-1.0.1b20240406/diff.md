# Comparing `tmp/autogluon-1.0.1b20240405.tar.gz` & `tmp/autogluon-1.0.1b20240406.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-1.0.1b20240405.tar", last modified: Fri Apr  5 09:05:13 2024, max compression
+gzip compressed data, was "autogluon-1.0.1b20240406.tar", last modified: Sat Apr  6 09:05:39 2024, max compression
```

## Comparing `autogluon-1.0.1b20240405.tar` & `autogluon-1.0.1b20240406.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:13.909105 autogluon-1.0.1b20240405/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-05 09:05:13.909105 autogluon-1.0.1b20240405/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:05:13.909105 autogluon-1.0.1b20240405/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-05 09:03:41.000000 autogluon-1.0.1b20240405/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:13.909105 autogluon-1.0.1b20240405/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:13.909105 autogluon-1.0.1b20240405/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:13.909105 autogluon-1.0.1b20240405/src/autogluon/_internal_/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 09:03:41.000000 autogluon-1.0.1b20240405/src/autogluon/_internal_/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 09:05:13.909105 autogluon-1.0.1b20240405/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-05 09:05:13.000000 autogluon-1.0.1b20240405/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-05 09:05:13.000000 autogluon-1.0.1b20240405/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:05:13.000000 autogluon-1.0.1b20240405/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:05:13.000000 autogluon-1.0.1b20240405/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-05 09:05:13.000000 autogluon-1.0.1b20240405/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 09:05:13.000000 autogluon-1.0.1b20240405/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 09:05:13.000000 autogluon-1.0.1b20240405/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:39.120137 autogluon-1.0.1b20240406/
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-06 09:05:39.120137 autogluon-1.0.1b20240406/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:05:39.120137 autogluon-1.0.1b20240406/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-06 09:04:13.000000 autogluon-1.0.1b20240406/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:39.116137 autogluon-1.0.1b20240406/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:39.116137 autogluon-1.0.1b20240406/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:39.120137 autogluon-1.0.1b20240406/src/autogluon/_internal_/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 09:04:13.000000 autogluon-1.0.1b20240406/src/autogluon/_internal_/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 09:05:39.120137 autogluon-1.0.1b20240406/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-04-06 09:05:39.000000 autogluon-1.0.1b20240406/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-06 09:05:39.000000 autogluon-1.0.1b20240406/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:05:39.000000 autogluon-1.0.1b20240406/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:05:39.000000 autogluon-1.0.1b20240406/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 09:05:39.000000 autogluon-1.0.1b20240406/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 09:05:39.000000 autogluon-1.0.1b20240406/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 09:05:39.000000 autogluon-1.0.1b20240406/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-1.0.1b20240405/PKG-INFO` & `autogluon-1.0.1b20240406/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.0.1b20240405
+Version: 1.0.1b20240406
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-1.0.1b20240405/setup.py` & `autogluon-1.0.1b20240406/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-1.0.1b20240405/src/autogluon.egg-info/PKG-INFO` & `autogluon-1.0.1b20240406/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 1.0.1b20240405
+Version: 1.0.1b20240406
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

