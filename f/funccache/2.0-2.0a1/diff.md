# Comparing `tmp/funccache-2.0.tar.gz` & `tmp/funccache-2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funccache-2.0.tar", last modified: Sun Apr  7 01:41:51 2024, max compression
+gzip compressed data, was "funccache-2.0a1.tar", last modified: Mon Apr  1 02:09:47 2024, max compression
```

## Comparing `funccache-2.0.tar` & `funccache-2.0a1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:41:51.167873 funccache-2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-07 01:41:44.000000 funccache-2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-07 01:41:51.167873 funccache-2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-07 01:41:44.000000 funccache-2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:41:51.167873 funccache-2.0/funccache/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-04-07 01:41:44.000000 funccache-2.0/funccache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-07 01:41:44.000000 funccache-2.0/funccache/i funccache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:41:51.167873 funccache-2.0/funccache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-04-07 01:41:51.000000 funccache-2.0/funccache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-07 01:41:51.000000 funccache-2.0/funccache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:41:51.000000 funccache-2.0/funccache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 01:41:51.000000 funccache-2.0/funccache.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:41:51.167873 funccache-2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-07 01:41:44.000000 funccache-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:09:47.288896 funccache-2.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-04-01 02:09:43.000000 funccache-2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-01 02:09:47.288896 funccache-2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-01 02:09:43.000000 funccache-2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:09:47.288896 funccache-2.0a1/funccache/
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-01 02:09:43.000000 funccache-2.0a1/funccache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17522 2024-04-01 02:09:43.000000 funccache-2.0a1/funccache/i funccache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 02:09:47.288896 funccache-2.0a1/funccache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-01 02:09:47.000000 funccache-2.0a1/funccache.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 02:09:47.288896 funccache-2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-01 02:09:43.000000 funccache-2.0a1/setup.py
```

### Comparing `funccache-2.0/LICENSE` & `funccache-2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `funccache-2.0/PKG-INFO` & `funccache-2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 2.0
+Version: 2.0a1
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Development Status :: 4 - Beta
```

### Comparing `funccache-2.0/README.md` & `funccache-2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `funccache-2.0/funccache/__init__.py` & `funccache-2.0a1/funccache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     >>> class Alpha(metaclass=funccache):
     >>>     ...
 
     >>> @funccache
     >>> def alpha():
     >>>     ...
 
-    @version: 2.0
+    @version: 2.0alpha1
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/funccache
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022-2024 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

### Comparing `funccache-2.0/funccache/i funccache.py` & `funccache-2.0a1/funccache/i funccache.py`

 * *Files identical despite different names*

### Comparing `funccache-2.0/funccache.egg-info/PKG-INFO` & `funccache-2.0a1/funccache.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funccache
-Version: 2.0
+Version: 2.0a1
 Summary: 如其名，它实现缓存功能，可缓存某个函数或某个类中定义的所有方法的返回值。
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/funccache
 Classifier: Development Status :: 4 - Beta
```

### Comparing `funccache-2.0/setup.py` & `funccache-2.0a1/setup.py`

 * *Files identical despite different names*

