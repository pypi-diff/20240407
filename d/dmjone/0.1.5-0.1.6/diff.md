# Comparing `tmp/dmjone-0.1.5.tar.gz` & `tmp/dmjone-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.5.tar", last modified: Sun Apr  7 08:20:46 2024, max compression
+gzip compressed data, was "dmjone-0.1.6.tar", last modified: Sun Apr  7 08:34:07 2024, max compression
```

## Comparing `dmjone-0.1.5.tar` & `dmjone-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.351397 dmjone-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 08:20:41.000000 dmjone-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 08:20:41.000000 dmjone-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:20:46.351397 dmjone-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-07 08:20:41.000000 dmjone-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 08:20:41.000000 dmjone-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:20:46.351397 dmjone-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.347397 dmjone-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.347397 dmjone-0.1.5/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 08:20:41.000000 dmjone-0.1.5/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 08:20:41.000000 dmjone-0.1.5/src/dmjone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 08:20:41.000000 dmjone-0.1.5/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.351397 dmjone-0.1.5/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:34:07.266746 dmjone-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 08:34:00.000000 dmjone-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 08:34:00.000000 dmjone-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:34:07.266746 dmjone-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-07 08:34:00.000000 dmjone-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 08:34:00.000000 dmjone-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:34:07.266746 dmjone-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:34:07.262746 dmjone-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:34:07.262746 dmjone-0.1.6/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12669 2024-04-07 08:34:00.000000 dmjone-0.1.6/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 08:34:00.000000 dmjone-0.1.6/src/dmjone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 08:34:00.000000 dmjone-0.1.6/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:34:07.266746 dmjone-0.1.6/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:34:07.000000 dmjone-0.1.6/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 08:34:07.000000 dmjone-0.1.6/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:34:07.000000 dmjone-0.1.6/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:34:07.000000 dmjone-0.1.6/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 08:34:07.000000 dmjone-0.1.6/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.5/LICENSE` & `dmjone-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.5/PKG-INFO` & `dmjone-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.5
+Version: 0.1.6
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dmjone-0.1.5/README.md` & `dmjone-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.5/pyproject.toml` & `dmjone-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.5"
+version = "0.1.6"
 description = "Public Welfare initiatives by dmj.one - Educational Initiative"
 readme = "README.md"
 license = {file = "LICENSE"}
 # license-files = ["LICENSE"]  # Explicitly list license files if you have multiple or non-standard ones.
 authors = [
     {name = "Divya Mohan"},
     {name = "Aarushi Sharma"},
```

### Comparing `dmjone-0.1.5/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.6/src/dmjone/StudentManagementSystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,9 +217,7 @@
         clear_terminal()
         default_admin_user(conn)
         user_info = user_login(conn)
         main_menu(conn, user_info)
 
     def branding():
         print_fancy_header(project_info)
-    
-    start()
```

### Comparing `dmjone-0.1.5/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.1.6/src/dmjone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.5
+Version: 0.1.6
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```
