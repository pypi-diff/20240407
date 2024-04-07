# Comparing `tmp/dmjone-0.1.9.tar.gz` & `tmp/dmjone-0.1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.9.tar", last modified: Sun Apr  7 14:58:32 2024, max compression
+gzip compressed data, was "dmjone-0.1.9.1.tar", last modified: Sun Apr  7 15:03:05 2024, max compression
```

## Comparing `dmjone-0.1.9.tar` & `dmjone-0.1.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.002574 dmjone-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 14:58:17.000000 dmjone-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 14:58:17.000000 dmjone-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-07 14:58:32.002574 dmjone-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-07 14:58:17.000000 dmjone-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 14:58:17.000000 dmjone-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:58:32.002574 dmjone-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.994574 dmjone-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.998574 dmjone-0.1.9/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/aarushi_TodoList.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.998574 dmjone-0.1.9/src/dmjone/kaustuv/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv/kaustuv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv/kaustuv_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/kaustuv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:31.998574 dmjone-0.1.9/src/dmjone/lakshika/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/lakshika_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 14:58:17.000000 dmjone-0.1.9/src/dmjone/lakshika/typecasting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.002574 dmjone-0.1.9/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45221 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 14:58:31.000000 dmjone-0.1.9/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:05.511474 dmjone-0.1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:03:05.511474 dmjone-0.1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:03:05.511474 dmjone-0.1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:05.507474 dmjone-0.1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:05.507474 dmjone-0.1.9.1/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/aarushi_TodoList.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:05.511474 dmjone-0.1.9.1/src/dmjone/kaustuv/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/kaustuv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/kaustuv/kaustuv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/kaustuv/kaustuv_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/kaustuv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:05.511474 dmjone-0.1.9.1/src/dmjone/lakshika/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/lakshika/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/lakshika/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/lakshika/lakshika_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:02:56.000000 dmjone-0.1.9.1/src/dmjone/lakshika/typecasting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:05.511474 dmjone-0.1.9.1/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:03:05.000000 dmjone-0.1.9.1/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 15:03:05.000000 dmjone-0.1.9.1/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:03:05.000000 dmjone-0.1.9.1/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 15:03:05.000000 dmjone-0.1.9.1/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 15:03:05.000000 dmjone-0.1.9.1/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.9/LICENSE` & `dmjone-0.1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9/PKG-INFO` & `dmjone-0.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dmjone-0.1.9/README.md` & `dmjone-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9/pyproject.toml` & `dmjone-0.1.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.9"
+version = "0.1.9.1"
 description = "Public Welfare initiatives by dmj.one - Educational Initiative"
 readme = "README.md"
 license = {file = "LICENSE"}
 # license-files = ["LICENSE"]  # Explicitly list license files if you have multiple or non-standard ones.
 authors = [
     {name = "Divya Mohan"},
     {name = "Aarushi Sharma"},
```

### Comparing `dmjone-0.1.9/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.9.1/src/dmjone/StudentManagementSystem.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9/src/dmjone/aarushi_TodoList.py` & `dmjone-0.1.9.1/src/dmjone/aarushi_TodoList.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9/src/dmjone/lakshika/lakshika_functions.py` & `dmjone-0.1.9.1/src/dmjone/lakshika/lakshika_functions.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.1.9.1/src/dmjone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dmjone-0.1.9/src/dmjone.egg-info/SOURCES.txt` & `dmjone-0.1.9.1/src/dmjone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

