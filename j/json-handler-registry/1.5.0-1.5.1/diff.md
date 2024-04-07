# Comparing `tmp/json-handler-registry-1.5.0.tar.gz` & `tmp/json-handler-registry-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-handler-registry-1.5.0.tar", last modified: Sat Apr  6 14:00:49 2024, max compression
+gzip compressed data, was "/home/pawel/workspace/repo/json-handler-registry/dist/.tmp-k9ira1lo/json-handler-registry-1.5.1.tar", last modified: Sun Apr  7 16:56:55 2024, max compression
```

## Comparing `json-handler-registry-1.5.0.tar` & `json-handler-registry-1.5.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-03-25 18:49:27.000000 json-handler-registry-1.5.0/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.5.0/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5037 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4520 2024-04-06 13:57:30.000000 json-handler-registry-1.5.0/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-04-06 13:55:25.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2466 2024-04-04 15:46:19.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/decoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1295 2024-04-04 15:46:10.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/encoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/py.typed
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4703 2024-04-06 13:54:01.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/registry.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-06 13:53:39.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      358 2024-04-04 15:57:40.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/config.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      380 2024-04-06 13:54:11.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1250 2024-04-06 13:41:51.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/dataclasses_json.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      842 2024-04-06 13:53:19.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/manager.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     5037 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      716 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-25 19:03:21.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/not-zip-safe
--rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/setup.cfg
--rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2329 2024-03-25 19:37:00.000000 json-handler-registry-1.5.0/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1072 2024-04-06 19:49:23.000000 json-handler-registry-1.5.1/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.5.1/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5151 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4520 2024-04-06 13:57:30.000000 json-handler-registry-1.5.1/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-04-07 16:55:52.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2466 2024-04-04 15:46:19.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/decoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1295 2024-04-04 15:46:10.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/encoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/py.typed
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4703 2024-04-06 13:54:01.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/registry.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/support/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-06 13:53:39.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/support/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      358 2024-04-04 15:57:40.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/support/config.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/support/impl/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      380 2024-04-06 13:54:11.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/support/impl/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1250 2024-04-06 13:41:51.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/support/impl/dataclasses_json.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      842 2024-04-06 13:53:19.000000 json-handler-registry-1.5.1/pkg/json_handler_registry/support/manager.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5151 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      674 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/pkg/json_handler_registry.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      886 2024-04-07 16:51:30.000000 json-handler-registry-1.5.1/pyproject.toml
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-07 16:56:55.000000 json-handler-registry-1.5.1/setup.cfg
```

### Comparing `json-handler-registry-1.5.0/LICENSE.txt` & `json-handler-registry-1.5.1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2022 P.J. Grochowski
+Copyright (c) 2024 P.J. Grochowski
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `json-handler-registry-1.5.0/PKG-INFO` & `json-handler-registry-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: json-handler-registry
-Version: 1.5.0
+Version: 1.5.1
 Summary: Standardized way of registering custom JSON serializers/deserializers.
-Home-page: https://bitbucket.org/massultidev/tunit/
-Author: P.J. Grochowski
-Author-email: pawel.grochowski.dev@gmail.com
+Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
+Project-URL: Repository, https://bitbucket.org/massultidev/json-handler-registry
+Keywords: json,serialization,deserialization
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI license](https://img.shields.io/pypi/l/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
```

### Comparing `json-handler-registry-1.5.0/README.md` & `json-handler-registry-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.5.0/pkg/json_handler_registry/decoder.py` & `json-handler-registry-1.5.1/pkg/json_handler_registry/decoder.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.5.0/pkg/json_handler_registry/encoder.py` & `json-handler-registry-1.5.1/pkg/json_handler_registry/encoder.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.5.0/pkg/json_handler_registry/registry.py` & `json-handler-registry-1.5.1/pkg/json_handler_registry/registry.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/dataclasses_json.py` & `json-handler-registry-1.5.1/pkg/json_handler_registry/support/impl/dataclasses_json.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.5.0/pkg/json_handler_registry/support/manager.py` & `json-handler-registry-1.5.1/pkg/json_handler_registry/support/manager.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/PKG-INFO` & `json-handler-registry-1.5.1/pkg/json_handler_registry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: json-handler-registry
-Version: 1.5.0
+Version: 1.5.1
 Summary: Standardized way of registering custom JSON serializers/deserializers.
-Home-page: https://bitbucket.org/massultidev/tunit/
-Author: P.J. Grochowski
-Author-email: pawel.grochowski.dev@gmail.com
+Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
+Project-URL: Repository, https://bitbucket.org/massultidev/json-handler-registry
+Keywords: json,serialization,deserialization
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI license](https://img.shields.io/pypi/l/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
```

### Comparing `json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/SOURCES.txt` & `json-handler-registry-1.5.1/pkg/json_handler_registry.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
 pkg/json_handler_registry/__init__.py
 pkg/json_handler_registry/decoder.py
 pkg/json_handler_registry/encoder.py
 pkg/json_handler_registry/py.typed
 pkg/json_handler_registry/registry.py
 pkg/json_handler_registry.egg-info/PKG-INFO
 pkg/json_handler_registry.egg-info/SOURCES.txt
 pkg/json_handler_registry.egg-info/dependency_links.txt
-pkg/json_handler_registry.egg-info/not-zip-safe
 pkg/json_handler_registry.egg-info/top_level.txt
 pkg/json_handler_registry/support/__init__.py
 pkg/json_handler_registry/support/config.py
 pkg/json_handler_registry/support/manager.py
 pkg/json_handler_registry/support/impl/__init__.py
 pkg/json_handler_registry/support/impl/dataclasses_json.py
```

