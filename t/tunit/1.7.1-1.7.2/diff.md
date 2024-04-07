# Comparing `tmp/tunit-1.7.1.tar.gz` & `tmp/tunit-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tunit-1.7.1.tar", last modified: Sat Apr  6 13:32:41 2024, max compression
+gzip compressed data, was "/home/pawel/workspace/repo/tunit/dist/.tmp-w23waes7/tunit-1.7.2.tar", last modified: Sun Apr  7 17:05:24 2024, max compression
```

## Comparing `tunit-1.7.1.tar` & `tunit-1.7.2.tar`

### file list

```diff
@@ -1,30 +1,29 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2022-04-24 18:13:16.000000 tunit-1.7.1/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)      127 2024-04-02 15:00:40.000000 tunit-1.7.1/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4912 2024-04-06 13:32:41.000000 tunit-1.7.1/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4362 2024-04-06 13:30:05.000000 tunit-1.7.1/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      167 2024-04-06 13:30:29.000000 tunit-1.7.1/pkg/tunit/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      920 2024-04-03 16:55:59.000000 tunit-1.7.1/pkg/tunit/config.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)    10100 2024-03-28 17:47:12.000000 tunit-1.7.1/pkg/tunit/core.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit/markup/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-02 15:19:52.000000 tunit-1.7.1/pkg/tunit/markup/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1734 2024-04-03 17:01:40.000000 tunit-1.7.1/pkg/tunit/markup/json.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2571 2024-04-03 17:02:12.000000 tunit-1.7.1/pkg/tunit/markup/yaml.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 tunit-1.7.1/pkg/tunit/py.typed
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1577 2024-03-28 17:38:44.000000 tunit-1.7.1/pkg/tunit/unit.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4912 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      495 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/not-zip-safe
--rw-r--r--   0 pawel     (1000) pawel     (1000)      157 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/requires.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        6 2024-04-06 13:32:41.000000 tunit-1.7.1/pkg/tunit.egg-info/top_level.txt
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/requirements/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 13:32:41.000000 tunit-1.7.1/requirements/extra/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       31 2024-03-28 22:08:02.000000 tunit-1.7.1/requirements/extra/json.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       42 2024-04-02 16:04:05.000000 tunit-1.7.1/requirements/extra/yaml.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:05:26.000000 tunit-1.7.1/requirements/release.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-06 13:32:41.000000 tunit-1.7.1/setup.cfg
--rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2974 2024-04-06 13:28:00.000000 tunit-1.7.1/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 17:05:24.000000 tunit-1.7.2/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-04-07 16:15:16.000000 tunit-1.7.2/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      127 2024-04-02 15:00:40.000000 tunit-1.7.2/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5025 2024-04-07 17:05:24.000000 tunit-1.7.2/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4362 2024-04-06 13:30:05.000000 tunit-1.7.2/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      167 2024-04-07 16:59:23.000000 tunit-1.7.2/pkg/tunit/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      920 2024-04-03 16:55:59.000000 tunit-1.7.2/pkg/tunit/config.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)    10100 2024-03-28 17:47:12.000000 tunit-1.7.2/pkg/tunit/core.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit/markup/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-02 15:19:52.000000 tunit-1.7.2/pkg/tunit/markup/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1734 2024-04-03 17:01:40.000000 tunit-1.7.2/pkg/tunit/markup/json.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2571 2024-04-03 17:02:12.000000 tunit-1.7.2/pkg/tunit/markup/yaml.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 tunit-1.7.2/pkg/tunit/py.typed
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1577 2024-03-28 17:38:44.000000 tunit-1.7.2/pkg/tunit/unit.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5025 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      469 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      148 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit.egg-info/requires.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        6 2024-04-07 17:05:24.000000 tunit-1.7.2/pkg/tunit.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1193 2024-04-07 16:48:58.000000 tunit-1.7.2/pyproject.toml
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 17:05:24.000000 tunit-1.7.2/requirements/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-07 17:05:24.000000 tunit-1.7.2/requirements/extra/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       31 2024-04-07 17:01:51.000000 tunit-1.7.2/requirements/extra/json.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       42 2024-04-02 16:04:05.000000 tunit-1.7.2/requirements/extra/yaml.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-03 17:05:26.000000 tunit-1.7.2/requirements/release.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-07 17:05:24.000000 tunit-1.7.2/setup.cfg
```

### Comparing `tunit-1.7.1/LICENSE.txt` & `tunit-1.7.2/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021-2022 P.J. Grochowski
+Copyright (c) 2023-2024 P.J. Grochowski
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `tunit-1.7.1/PKG-INFO` & `tunit-1.7.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tunit
-Version: 1.7.1
+Version: 1.7.2
 Summary: Time unit types. For transparency safety and readability.
-Home-page: https://bitbucket.org/massultidev/tunit/
-Author: P.J. Grochowski
-Author-email: pawel.grochowski.dev@gmail.com
+Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
+Project-URL: Repository, https://bitbucket.org/massultidev/tunit/
+Keywords: time,units,timestamp,chrono,seconds,milliseconds
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: all
 Provides-Extra: json
 Provides-Extra: yaml
-Provides-Extra: all
 License-File: LICENSE.txt
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI license](https://img.shields.io/pypi/l/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![Downloads](https://static.pepy.tech/badge/tunit)](https://pepy.tech/project/tunit)
```

### Comparing `tunit-1.7.1/README.md` & `tunit-1.7.2/README.md`

 * *Files identical despite different names*

### Comparing `tunit-1.7.1/pkg/tunit/config.py` & `tunit-1.7.2/pkg/tunit/config.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.1/pkg/tunit/core.py` & `tunit-1.7.2/pkg/tunit/core.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.1/pkg/tunit/markup/json.py` & `tunit-1.7.2/pkg/tunit/markup/json.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.1/pkg/tunit/markup/yaml.py` & `tunit-1.7.2/pkg/tunit/markup/yaml.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.1/pkg/tunit/unit.py` & `tunit-1.7.2/pkg/tunit/unit.py`

 * *Files identical despite different names*

### Comparing `tunit-1.7.1/pkg/tunit.egg-info/PKG-INFO` & `tunit-1.7.2/pkg/tunit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: tunit
-Version: 1.7.1
+Version: 1.7.2
 Summary: Time unit types. For transparency safety and readability.
-Home-page: https://bitbucket.org/massultidev/tunit/
-Author: P.J. Grochowski
-Author-email: pawel.grochowski.dev@gmail.com
+Author-email: "P.J. Grochowski" <pawel.grochowski.dev@gmail.com>
 License: MIT
+Project-URL: Repository, https://bitbucket.org/massultidev/tunit/
+Keywords: time,units,timestamp,chrono,seconds,milliseconds
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: all
 Provides-Extra: json
 Provides-Extra: yaml
-Provides-Extra: all
 License-File: LICENSE.txt
 
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![PyPI license](https://img.shields.io/pypi/l/tunit.svg)](https://pypi.python.org/pypi/tunit)
 [![Downloads](https://static.pepy.tech/badge/tunit)](https://pepy.tech/project/tunit)
```

