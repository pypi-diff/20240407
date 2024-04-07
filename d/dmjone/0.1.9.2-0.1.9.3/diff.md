# Comparing `tmp/dmjone-0.1.9.2.tar.gz` & `tmp/dmjone-0.1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.9.2.tar", last modified: Sun Apr  7 15:12:26 2024, max compression
+gzip compressed data, was "dmjone-0.1.9.3.tar", last modified: Sun Apr  7 15:27:48 2024, max compression
```

## Comparing `dmjone-0.1.9.2.tar` & `dmjone-0.1.9.3.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:26.852465 dmjone-0.1.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:12:26.848465 dmjone-0.1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:12:26.852465 dmjone-0.1.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:26.844465 dmjone-0.1.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:26.848465 dmjone-0.1.9.2/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/aarushi_TodoList.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/hello.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:26.848465 dmjone-0.1.9.2/src/dmjone/kaustuv/
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/kaustuv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/kaustuv/kaustuv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/kaustuv/kaustuv_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/kaustuv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:26.848465 dmjone-0.1.9.2/src/dmjone/lakshika/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/lakshika/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/lakshika/calculator.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/lakshika/lakshika_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:12:19.000000 dmjone-0.1.9.2/src/dmjone/lakshika/typecasting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:26.848465 dmjone-0.1.9.2/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:12:26.000000 dmjone-0.1.9.2/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 15:12:26.000000 dmjone-0.1.9.2/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:12:26.000000 dmjone-0.1.9.2/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 15:12:26.000000 dmjone-0.1.9.2/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 15:12:26.000000 dmjone-0.1.9.2/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:27:48.848898 dmjone-0.1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:27:48.848898 dmjone-0.1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:27:48.848898 dmjone-0.1.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:27:48.840898 dmjone-0.1.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:27:48.844898 dmjone-0.1.9.3/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:27:48.844898 dmjone-0.1.9.3/src/dmjone/aarushi/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/aarushi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/aarushi/aarushi_todolist.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/hello.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:27:48.844898 dmjone-0.1.9.3/src/dmjone/kaustuv/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/kaustuv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/kaustuv/kaustuv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/kaustuv/kaustuv_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:27:48.844898 dmjone-0.1.9.3/src/dmjone/lakshika/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/lakshika/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/lakshika/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/lakshika/lakshika_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-07 15:27:41.000000 dmjone-0.1.9.3/src/dmjone/lakshika/typecasting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:27:48.844898 dmjone-0.1.9.3/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45223 2024-04-07 15:27:48.000000 dmjone-0.1.9.3/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 15:27:48.000000 dmjone-0.1.9.3/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:27:48.000000 dmjone-0.1.9.3/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 15:27:48.000000 dmjone-0.1.9.3/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 15:27:48.000000 dmjone-0.1.9.3/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.9.2/LICENSE` & `dmjone-0.1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.2/PKG-INFO` & `dmjone-0.1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dmjone-0.1.9.2/README.md` & `dmjone-0.1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.2/pyproject.toml` & `dmjone-0.1.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.9.2"
+version = "0.1.9.3"
 description = "Public Welfare initiatives by dmj.one - Educational Initiative"
 readme = "README.md"
 license = {file = "LICENSE"}
 # license-files = ["LICENSE"]  # Explicitly list license files if you have multiple or non-standard ones.
 authors = [
     {name = "Divya Mohan"},
     {name = "Aarushi Sharma"},
```

### Comparing `dmjone-0.1.9.2/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.9.3/src/dmjone/StudentManagementSystem.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.2/src/dmjone/__init__.py` & `dmjone-0.1.9.3/src/dmjone/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # src/dmjone/__init__.py
 
 from .lab4 import lab4
 from .hello import hello
 from .StudentManagementSystem import projectsms
 
 # Section: Aarushi Sharma
-from .aarushi_TodoList import TodoList
+from .aarushi import *
 
 # Section: Kaustuv Sharma
 # import src.dmjone.kaustuv_common as kaustuv
 # import src.dmjone.kaustuv_function2 as kaustuv_function2
 # kaustuv.__dict__.update(kaustuv_function2.__dict__)
-
 # import src.dmjone.kaustuv as kaustuv
+from .kaustuv import *
 
 # Section: Lakshika Tanwar
 # import src.dmjone.lakshika as lakshika
+from .lakshika import *
+
 
-from .kaustuv import *
-# from .lakshika import *
```

### Comparing `dmjone-0.1.9.2/src/dmjone/aarushi_TodoList.py` & `dmjone-0.1.9.3/src/dmjone/aarushi/aarushi_todolist.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.2/src/dmjone/lakshika/lakshika_functions.py` & `dmjone-0.1.9.3/src/dmjone/lakshika/lakshika_functions.py`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.9.2/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.1.9.3/src/dmjone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.9.2
+Version: 0.1.9.3
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dmjone-0.1.9.2/src/dmjone.egg-info/SOURCES.txt` & `dmjone-0.1.9.3/src/dmjone.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 src/dmjone/StudentManagementSystem.py
 src/dmjone/__init__.py
-src/dmjone/aarushi_TodoList.py
 src/dmjone/hello.py
-src/dmjone/kaustuv_common.py
 src/dmjone/lab4.py
 src/dmjone.egg-info/PKG-INFO
 src/dmjone.egg-info/SOURCES.txt
 src/dmjone.egg-info/dependency_links.txt
 src/dmjone.egg-info/requires.txt
 src/dmjone.egg-info/top_level.txt
+src/dmjone/aarushi/__init__.py
+src/dmjone/aarushi/aarushi_todolist.py
 src/dmjone/kaustuv/__init__.py
 src/dmjone/kaustuv/kaustuv_common.py
 src/dmjone/kaustuv/kaustuv_project.py
 src/dmjone/lakshika/__init__.py
 src/dmjone/lakshika/calculator.py
 src/dmjone/lakshika/lakshika_functions.py
 src/dmjone/lakshika/typecasting.py
```

