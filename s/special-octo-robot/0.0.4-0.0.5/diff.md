# Comparing `tmp/special-octo-robot-0.0.4.tar.gz` & `tmp/special-octo-robot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "special-octo-robot-0.0.4.tar", last modified: Sun Apr  7 13:16:26 2024, max compression
+gzip compressed data, was "special-octo-robot-0.0.5.tar", last modified: Sun Apr  7 14:12:27 2024, max compression
```

## Comparing `special-octo-robot-0.0.4.tar` & `special-octo-robot-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/LICENSE
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/MANIFEST.in
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3564 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     3022 2024-04-07 04:26:45.000000 special-octo-robot-0.0.4/README.md
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/app/
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/app/__init__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.4/app/__main__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-07 12:40:37.000000 special-octo-robot-0.0.4/app/__version__.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     6022 2024-04-07 12:36:04.000000 special-octo-robot-0.0.4/app/application.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     3423 2024-04-07 11:46:37.000000 special-octo-robot-0.0.4/app/console.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      396 2024-04-07 11:44:42.000000 special-octo-robot-0.0.4/app/constants.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1904 2024-04-07 12:35:34.000000 special-octo-robot-0.0.4/app/database.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     5662 2024-04-07 12:36:04.000000 special-octo-robot-0.0.4/devcord.py
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/setup.cfg
--rw-rw-r--   0 nginx     (1000) nginx     (1000)     1053 2024-04-03 14:57:12.000000 special-octo-robot-0.0.4/setup.py
-drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 13:16:26.881548 special-octo-robot-0.0.4/special_octo_robot.egg-info/
--rw-r--r--   0 nginx     (1000) nginx     (1000)     3564 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/PKG-INFO
--rw-rw-r--   0 nginx     (1000) nginx     (1000)      421 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/SOURCES.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/dependency_links.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/entry_points.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/requires.txt
--rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-07 13:16:26.000000 special-octo-robot-0.0.4/special_octo_robot.egg-info/top_level.txt
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 14:12:27.915836 special-octo-robot-0.0.5/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)    35149 2024-03-17 03:53:33.000000 special-octo-robot-0.0.5/LICENSE
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.5/MANIFEST.in
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     3718 2024-04-07 14:12:27.915836 special-octo-robot-0.0.5/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     3022 2024-04-07 04:26:45.000000 special-octo-robot-0.0.5/README.md
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 14:12:27.915836 special-octo-robot-0.0.5/app/
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.5/app/__init__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        0 2024-03-17 03:53:33.000000 special-octo-robot-0.0.5/app/__main__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       18 2024-04-07 14:12:20.000000 special-octo-robot-0.0.5/app/__version__.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     6075 2024-04-07 14:10:26.000000 special-octo-robot-0.0.5/app/application.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     3423 2024-04-07 11:46:37.000000 special-octo-robot-0.0.5/app/console.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      396 2024-04-07 11:44:42.000000 special-octo-robot-0.0.5/app/constants.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1904 2024-04-07 14:10:51.000000 special-octo-robot-0.0.5/app/database.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     5680 2024-04-07 14:05:02.000000 special-octo-robot-0.0.5/devcord.py
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       38 2024-04-07 14:12:27.915836 special-octo-robot-0.0.5/setup.cfg
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)     1200 2024-04-07 13:24:59.000000 special-octo-robot-0.0.5/setup.py
+drwxrwxr-x   0 nginx     (1000) nginx     (1000)        0 2024-04-07 14:12:27.915836 special-octo-robot-0.0.5/special_octo_robot.egg-info/
+-rw-r--r--   0 nginx     (1000) nginx     (1000)     3718 2024-04-07 14:12:27.000000 special-octo-robot-0.0.5/special_octo_robot.egg-info/PKG-INFO
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)      421 2024-04-07 14:12:27.000000 special-octo-robot-0.0.5/special_octo_robot.egg-info/SOURCES.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)        1 2024-04-07 14:12:27.000000 special-octo-robot-0.0.5/special_octo_robot.egg-info/dependency_links.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       40 2024-04-07 14:12:27.000000 special-octo-robot-0.0.5/special_octo_robot.egg-info/entry_points.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       26 2024-04-07 14:12:27.000000 special-octo-robot-0.0.5/special_octo_robot.egg-info/requires.txt
+-rw-rw-r--   0 nginx     (1000) nginx     (1000)       12 2024-04-07 14:12:27.000000 special-octo-robot-0.0.5/special_octo_robot.egg-info/top_level.txt
```

### Comparing `special-octo-robot-0.0.4/LICENSE` & `special-octo-robot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.4/PKG-INFO` & `special-octo-robot-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
+Platform: Windows
+Platform: MacOS X
+Platform: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.0.1
 Requires-Dist: rich>=13.7.0
```

### Comparing `special-octo-robot-0.0.4/README.md` & `special-octo-robot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.4/app/application.py` & `special-octo-robot-0.0.5/app/application.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,15 +203,17 @@
     if updated_data["status"] == "Completed":
         current_date = datetime.now().strftime("%Y-%m-%d")
         updated_data["completed"] = str(current_date)
     else:
         updated_data["completed"] = updated_data["deadline"]
 
     for key, value in updated_data.items():
-        if type(value) is str:
+
+        print(type(value), value, key)
+        if type(value) is str or not value:
             updated_data[key] = f'"{value}"'
 
     database.update_table("tasks", updated_data)
 
 
 def convert_to_console_date(date_str):
     """
```

### Comparing `special-octo-robot-0.0.4/app/console.py` & `special-octo-robot-0.0.5/app/console.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.4/app/database.py` & `special-octo-robot-0.0.5/app/database.py`

 * *Files identical despite different names*

### Comparing `special-octo-robot-0.0.4/devcord.py` & `special-octo-robot-0.0.5/devcord.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 pending=pending,
                 label=label,
             ),
             output,
             path,
         )
     elif add:
-        description = None
+        description = "No given description"
         add = add
         if desc:
             description = click.edit()
         if parent:
             val = application.search_task(parent)
             if not val:
                 click.echo(
```

### Comparing `special-octo-robot-0.0.4/setup.py` & `special-octo-robot-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,16 +19,19 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/geekNero/special-octo-robot.git",
     py_modules=["devcord", "app"],
     packages=find_packages(),
     install_requires=[requirements],
     python_requires=">=3.8",
+    platforms=["Windows", "MacOS X", "Linux"],
     classifiers=[
         "Programming Language :: Python :: 3",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX :: Linux",
     ],
     entry_points={
         "console_scripts": [
             "devcord=devcord:cli",
         ],
     },
```

### Comparing `special-octo-robot-0.0.4/special_octo_robot.egg-info/PKG-INFO` & `special-octo-robot-0.0.5/special_octo_robot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 Metadata-Version: 2.1
 Name: special-octo-robot
-Version: 0.0.4
+Version: 0.0.5
 Summary: Creating my own version of what a CLI Task manager and To-do-list would look like
 Home-page: https://github.com/geekNero/special-octo-robot.git
 Author: Jahan Chaware
 Author-email: sg550js@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
+Platform: Windows
+Platform: MacOS X
+Platform: Linux
 Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.0.1
 Requires-Dist: rich>=13.7.0
```

