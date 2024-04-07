# Comparing `tmp/RelaDB-2.0.0.tar.gz` & `tmp/RelaDB-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RelaDB-2.0.0.tar", last modified: Sat Apr  6 03:35:26 2024, max compression
+gzip compressed data, was "RelaDB-2.0.1.tar", last modified: Sun Apr  7 20:41:06 2024, max compression
```

## Comparing `RelaDB-2.0.0.tar` & `RelaDB-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.320013 RelaDB-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-06 03:35:26.320013 RelaDB-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-06 03:35:22.000000 RelaDB-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:35:26.320013 RelaDB-2.0.0/RelaDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-06 03:35:26.000000 RelaDB-2.0.0/RelaDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 03:35:26.000000 RelaDB-2.0.0/RelaDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:35:26.000000 RelaDB-2.0.0/RelaDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:35:26.000000 RelaDB-2.0.0/RelaDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 03:35:26.320013 RelaDB-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-06 03:35:22.000000 RelaDB-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:41:06.990519 RelaDB-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-07 20:41:06.990519 RelaDB-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3534 2024-04-07 20:41:03.000000 RelaDB-2.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:41:06.990519 RelaDB-2.0.1/RelaDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2024-04-07 20:41:06.000000 RelaDB-2.0.1/RelaDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-07 20:41:06.000000 RelaDB-2.0.1/RelaDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:41:06.000000 RelaDB-2.0.1/RelaDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:41:06.000000 RelaDB-2.0.1/RelaDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 20:41:06.990519 RelaDB-2.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3940 2024-04-07 20:41:03.000000 RelaDB-2.0.1/setup.py
```

### Comparing `RelaDB-2.0.0/PKG-INFO` & `RelaDB-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RelaDB
-Version: 2.0.0
+Version: 2.0.1
 Summary: A fast and lightweight relational db
 Home-page: https://github.com/D4r3d3vil/RelaDB
 Author: Mulham Alamry
 Author-email: mulhamreacts@gmail.com
 License: UNKNOWN
 Description: # RelaDB
```

### Comparing `RelaDB-2.0.0/README.md` & `RelaDB-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `RelaDB-2.0.0/RelaDB.egg-info/PKG-INFO` & `RelaDB-2.0.1/RelaDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RelaDB
-Version: 2.0.0
+Version: 2.0.1
 Summary: A fast and lightweight relational db
 Home-page: https://github.com/D4r3d3vil/RelaDB
 Author: Mulham Alamry
 Author-email: mulhamreacts@gmail.com
 License: UNKNOWN
 Description: # RelaDB
```

### Comparing `RelaDB-2.0.0/setup.py` & `RelaDB-2.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RelaDB',
-    version='2.0.0',
+    version='2.0.1',
     author='Mulham Alamry',
     author_email='mulhamreacts@gmail.com',
     description='A fast and lightweight relational db',
     long_description="""# RelaDB
 
 🔥 RelaDB is a lightweight set of classes for a relational database system designed for simplicity and speed. It integrates with SQLite and provides an easy-to-use API for managing database schemas, tables, and records in Python.
```

