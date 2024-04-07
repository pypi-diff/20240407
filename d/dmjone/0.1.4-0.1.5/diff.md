# Comparing `tmp/dmjone-0.1.4.tar.gz` & `tmp/dmjone-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.4.tar", last modified: Sun Apr  7 07:34:23 2024, max compression
+gzip compressed data, was "dmjone-0.1.5.tar", last modified: Sun Apr  7 08:20:46 2024, max compression
```

## Comparing `dmjone-0.1.4.tar` & `dmjone-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 07:34:11.000000 dmjone-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 07:34:11.000000 dmjone-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 07:34:23.549579 dmjone-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-07 07:34:11.000000 dmjone-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 07:34:11.000000 dmjone-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 07:34:23.549579 dmjone-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-07 07:34:11.000000 dmjone-0.1.4/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 07:34:11.000000 dmjone-0.1.4/src/dmjone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 07:34:11.000000 dmjone-0.1.4/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:34:23.549579 dmjone-0.1.4/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 07:34:23.000000 dmjone-0.1.4/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.351397 dmjone-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 08:20:41.000000 dmjone-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 08:20:41.000000 dmjone-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:20:46.351397 dmjone-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-04-07 08:20:41.000000 dmjone-0.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-07 08:20:41.000000 dmjone-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:20:46.351397 dmjone-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.347397 dmjone-0.1.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.347397 dmjone-0.1.5/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12688 2024-04-07 08:20:41.000000 dmjone-0.1.5/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 08:20:41.000000 dmjone-0.1.5/src/dmjone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 08:20:41.000000 dmjone-0.1.5/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:20:46.351397 dmjone-0.1.5/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44497 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 08:20:46.000000 dmjone-0.1.5/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.4/LICENSE` & `dmjone-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.4/PKG-INFO` & `dmjone-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.4
+Version: 0.1.5
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `dmjone-0.1.4/README.md` & `dmjone-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dmjone-0.1.4/pyproject.toml` & `dmjone-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dmjone"
-version = "0.1.4"
+version = "0.1.5"
 description = "Public Welfare initiatives by dmj.one - Educational Initiative"
 readme = "README.md"
 license = {file = "LICENSE"}
 # license-files = ["LICENSE"]  # Explicitly list license files if you have multiple or non-standard ones.
 authors = [
     {name = "Divya Mohan"},
     {name = "Aarushi Sharma"},
```

### Comparing `dmjone-0.1.4/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.5/src/dmjone/StudentManagementSystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# Run when dmjone.StudentManagementSystem() or dmjone.projectsms() is called
+# Run when dmjone.projectsms() is called
 
-import mysql.connector
-import getpass
-import random
-import os
-import platform
-import shutil
-from datetime import datetime
-from faker import Faker
+def projectsms():
+    import mysql.connector
+    import getpass
+    import random
+    import os
+    import platform
+    import shutil
+    from datetime import datetime
+    from faker import Faker
 
-def StudentManagementSystem():
     faker = Faker()
 
     project_info = """
     Student Management System
 
     A Cybersecurity, DBMS, & Python Class Project by dmj.one crafted with care to empower education.\nYour journey is important to us.
     ________________________________________________________________________________
@@ -192,28 +192,34 @@
                 print_centered("Thank you for using the Student Management System, a project for you by the team of dmj.one\nThis project was created as part of public welfare initiative of dmj.one\nLet us know if you have any queries or need any help.\n\nVisit https://dmj.one for more projects. May the world be educated! See you again!")
                 exit()
             elif choice in visible_options:
                 visible_options[choice][1]()
             else:
                 print("Invalid option or insufficient permissions.\n")
 
-    def start_from_init():
+    def start():
         try:
             conn = connect_db()
             authenticate_user(conn)
         except mysql.connector.Error as err:
             print(f"Database connection failed: {err}")
         finally:
             conn.close()
+    # if __name__ == "__main__":
+        # try:
+            # conn = connect_db()
+            # authenticate_user(conn)
+        # except mysql.connector.Error as err:
+            # print(f"Database connection failed: {err}")
+        # finally:
+            # conn.close()
 
     def authenticate_user(conn):
         clear_terminal()
         default_admin_user(conn)
         user_info = user_login(conn)
         main_menu(conn, user_info)
 
     def branding():
         print_fancy_header(project_info)
-
-    start_from_init()
-
-projectsms = StudentManagementSystem()
+    
+    start()
```

### Comparing `dmjone-0.1.4/src/dmjone.egg-info/PKG-INFO` & `dmjone-0.1.5/src/dmjone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dmjone
-Version: 0.1.4
+Version: 0.1.5
 Summary: Public Welfare initiatives by dmj.one - Educational Initiative
 Author: Divya Mohan, Aarushi Sharma, Anshuman Mohanty, Ashutosh Rana, Jatin Sharma, Kaustuv Sharma, Lakshika Tanwar, Vedansh Sharma
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

