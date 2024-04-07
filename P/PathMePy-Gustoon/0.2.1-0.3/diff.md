# Comparing `tmp/PathMePy-Gustoon-0.2.1.tar.gz` & `tmp/PathMePy-Gustoon-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PathMePy-Gustoon-0.2.1.tar", last modified: Sat Apr  6 08:49:48 2024, max compression
+gzip compressed data, was "PathMePy-Gustoon-0.3.tar", last modified: Sat Apr  6 18:11:15 2024, max compression
```

## Comparing `PathMePy-Gustoon-0.2.1.tar` & `PathMePy-Gustoon-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 08:49:48.785003 PathMePy-Gustoon-0.2.1/
--rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-Gustoon-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0      839 2024-04-06 08:49:48.777421 PathMePy-Gustoon-0.2.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 08:49:48.733813 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon/
--rw-rw-rw-   0        0        0     1162 2024-04-06 08:41:04.000000 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon/PathMePy.py
--rw-rw-rw-   0        0        0      112 2024-04-06 08:49:11.000000 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 08:49:48.775420 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon.egg-info/
--rw-rw-rw-   0        0        0      839 2024-04-06 08:49:48.000000 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-06 08:49:48.000000 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 08:49:48.000000 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-06 08:49:48.000000 PathMePy-Gustoon-0.2.1/PathMePy_Gustoon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      456 2024-03-31 08:33:03.000000 PathMePy-Gustoon-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 08:49:48.786002 PathMePy-Gustoon-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      909 2024-04-06 08:49:21.000000 PathMePy-Gustoon-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:11:15.755360 PathMePy-Gustoon-0.3/
+-rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-Gustoon-0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      837 2024-04-06 18:11:15.748366 PathMePy-Gustoon-0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 18:11:15.715384 PathMePy-Gustoon-0.3/PathMePy_Gustoon/
+-rw-rw-rw-   0        0        0     1483 2024-04-06 18:10:19.000000 PathMePy-Gustoon-0.3/PathMePy_Gustoon/PathMePy.py
+-rw-rw-rw-   0        0        0      148 2024-04-06 18:09:36.000000 PathMePy-Gustoon-0.3/PathMePy_Gustoon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 18:11:15.745367 PathMePy-Gustoon-0.3/PathMePy_Gustoon.egg-info/
+-rw-rw-rw-   0        0        0      837 2024-04-06 18:11:15.000000 PathMePy-Gustoon-0.3/PathMePy_Gustoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-06 18:11:15.000000 PathMePy-Gustoon-0.3/PathMePy_Gustoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 18:11:15.000000 PathMePy-Gustoon-0.3/PathMePy_Gustoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 18:11:15.000000 PathMePy-Gustoon-0.3/PathMePy_Gustoon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      456 2024-03-31 08:33:03.000000 PathMePy-Gustoon-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 18:11:15.756360 PathMePy-Gustoon-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      907 2024-04-06 18:10:29.000000 PathMePy-Gustoon-0.3/setup.py
```

### Comparing `PathMePy-Gustoon-0.2.1/LICENSE.txt` & `PathMePy-Gustoon-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PathMePy-Gustoon-0.2.1/PKG-INFO` & `PathMePy-Gustoon-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy-Gustoon
-Version: 0.2.1
+Version: 0.3
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PathMePy-Gustoon-0.2.1/PathMePy_Gustoon/PathMePy.py` & `PathMePy-Gustoon-0.3/PathMePy_Gustoon/PathMePy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,43 @@
 import os
 import platform
 import site
 import sys
 
+Current_Path = os.environ.get("PATH")
+
+if platform.system() != "Windows" and platform.system() != "Linux" :
+    Current_Path_Formated = Current_Path.replace(":", "\n")
+if platform.system() == "Windows" :
+    Current_Path_Formated = Current_Path.replace(";", "\n")
+elif platform.system() == "Linux":
+    Current_Path_Formated = Current_Path.replace(":", "\n")
+
+class PathNotFoundError(Exception):
+    def __init__(self, message):
+        self.message = message
+
+def IsAlreadyOnPath(path):
+    if path in Current_Path_Formated:
+        return True
+    else:
+        return False
+
 def PathMePyDir(path):
     path = os.path.abspath(path)
+    if not os.path.exists(path):
+        raise PathNotFoundError("The path is not found.")
     if platform.system() != "Windows" and platform.system() != "Linux" :
         os.system('export PATH=$PATH:' + path)
     if platform.system() == "Windows" :
         os.system('set Path="%Path%;' + path + '"')
     elif platform.system() == "Linux":
         os.system('export PATH=$PATH:' + path)
 
 def PathMePyUserScriptFolder():
     path = site.getusersitepackages()
     if platform.system() != "Windows" and platform.system() != "Linux" :
         os.system('export PATH=$PATH:' + path)
     if platform.system() == "Windows" :
         os.system('set Path="%Path%;' + path + '"')
     elif platform.system() == "Linux":
-        os.system('export PATH=$PATH:' + path)
-
-Current_Path = os.environ.get("PATH")
-
-if platform.system() != "Windows" and platform.system() != "Linux" :
-    Current_Path_Formated = Current_Path.replace(":", "\n")
-if platform.system() == "Windows" :
-    Current_Path_Formated = Current_Path.replace(";", "\n")
-elif platform.system() == "Linux":
-    Current_Path_Formated = Current_Path.replace(":", "\n")
+        os.system('export PATH=$PATH:' + path)
```

### Comparing `PathMePy-Gustoon-0.2.1/PathMePy_Gustoon.egg-info/PKG-INFO` & `PathMePy-Gustoon-0.3/PathMePy_Gustoon.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy-Gustoon
-Version: 0.2.1
+Version: 0.3
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PathMePy-Gustoon-0.2.1/setup.py` & `PathMePy-Gustoon-0.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 name='PathMePy-Gustoon',
-version='0.2.1',
+version='0.3',
 author='Gustoon',
 author_email='',
 description='A tool to add scripts to Path',
 long_description='''
 # PathMePy
 
 A tool to add scripts to Path
```

