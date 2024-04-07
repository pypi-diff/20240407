# Comparing `tmp/python-geoacumen-2024.3.31.tar.gz` & `tmp/python-geoacumen-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-geoacumen-2024.3.31.tar", last modified: Sun Mar 31 04:10:13 2024, max compression
+gzip compressed data, was "python-geoacumen-2024.4.7.tar", last modified: Sun Apr  7 04:10:53 2024, max compression
```

## Comparing `python-geoacumen-2024.3.31.tar` & `python-geoacumen-2024.4.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 04:10:13.761412 python-geoacumen-2024.3.31/
--rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-03-31 04:09:57.000000 python-geoacumen-2024.3.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-31 04:09:57.000000 python-geoacumen-2024.3.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-31 04:10:13.761412 python-geoacumen-2024.3.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-31 04:09:57.000000 python-geoacumen-2024.3.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 04:10:13.749412 python-geoacumen-2024.3.31/geoacumen/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-31 04:10:08.000000 python-geoacumen-2024.3.31/geoacumen/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 04:10:13.749412 python-geoacumen-2024.3.31/geoacumen/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-31 04:09:57.000000 python-geoacumen-2024.3.31/geoacumen/db/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127) 10682499 2024-03-31 04:10:13.000000 python-geoacumen-2024.3.31/geoacumen/db/Geoacumen-Country.mmdb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 04:10:13.761412 python-geoacumen-2024.3.31/python_geoacumen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-31 04:10:13.000000 python-geoacumen-2024.3.31/python_geoacumen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-03-31 04:10:13.000000 python-geoacumen-2024.3.31/python_geoacumen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 04:10:13.000000 python-geoacumen-2024.3.31/python_geoacumen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-31 04:10:13.000000 python-geoacumen-2024.3.31/python_geoacumen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-31 04:10:13.000000 python-geoacumen-2024.3.31/python_geoacumen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 04:10:13.761412 python-geoacumen-2024.3.31/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-31 04:09:57.000000 python-geoacumen-2024.3.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:10:53.033494 python-geoacumen-2024.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11338 2024-04-07 04:10:41.000000 python-geoacumen-2024.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 04:10:41.000000 python-geoacumen-2024.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 04:10:53.033494 python-geoacumen-2024.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-07 04:10:41.000000 python-geoacumen-2024.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:10:53.021494 python-geoacumen-2024.4.7/geoacumen/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 04:10:48.000000 python-geoacumen-2024.4.7/geoacumen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:10:53.021494 python-geoacumen-2024.4.7/geoacumen/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:10:41.000000 python-geoacumen-2024.4.7/geoacumen/db/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127) 10709891 2024-04-07 04:10:52.000000 python-geoacumen-2024.4.7/geoacumen/db/Geoacumen-Country.mmdb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:10:53.033494 python-geoacumen-2024.4.7/python_geoacumen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 04:10:52.000000 python-geoacumen-2024.4.7/python_geoacumen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-07 04:10:52.000000 python-geoacumen-2024.4.7/python_geoacumen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:10:52.000000 python-geoacumen-2024.4.7/python_geoacumen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 04:10:52.000000 python-geoacumen-2024.4.7/python_geoacumen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 04:10:52.000000 python-geoacumen-2024.4.7/python_geoacumen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 04:10:53.033494 python-geoacumen-2024.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-07 04:10:41.000000 python-geoacumen-2024.4.7/setup.py
```

### Comparing `python-geoacumen-2024.3.31/LICENSE` & `python-geoacumen-2024.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-geoacumen-2024.3.31/PKG-INFO` & `python-geoacumen-2024.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-geoacumen
-Version: 2024.3.31
+Version: 2024.4.7
 Summary: Library to access/distribute Geoacumen IP databases
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@nyu.edu
 License: Apache 2.0
 Description: # python-geoacumen
```

### Comparing `python-geoacumen-2024.3.31/python_geoacumen.egg-info/PKG-INFO` & `python-geoacumen-2024.4.7/python_geoacumen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-geoacumen
-Version: 2024.3.31
+Version: 2024.4.7
 Summary: Library to access/distribute Geoacumen IP databases
 Home-page: UNKNOWN
 Author: Kevin Chung
 Author-email: kchung@nyu.edu
 License: Apache 2.0
 Description: # python-geoacumen
```

### Comparing `python-geoacumen-2024.3.31/setup.py` & `python-geoacumen-2024.4.7/setup.py`

 * *Files identical despite different names*

