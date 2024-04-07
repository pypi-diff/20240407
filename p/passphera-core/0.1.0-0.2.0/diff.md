# Comparing `tmp/passphera-core-0.1.0.tar.gz` & `tmp/passphera-core-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passphera-core-0.1.0.tar", last modified: Fri Apr  5 01:53:54 2024, max compression
+gzip compressed data, was "passphera-core-0.2.0.tar", last modified: Sun Apr  7 16:29:28 2024, max compression
```

## Comparing `passphera-core-0.1.0.tar` & `passphera-core-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-05 01:53:54.504895 passphera-core-0.1.0/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-05 01:53:54.504895 passphera-core-0.1.0/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.1.0/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-05 01:53:54.502895 passphera-core-0.1.0/passphera_core/
--rw-r--r--   0 fathi     (1000) fathi     (1000)     3465 2024-04-05 01:39:31.000000 passphera-core-0.1.0/passphera_core/__init__.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-05 01:53:54.503895 passphera-core-0.1.0/passphera_core.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-05 01:53:54.000000 passphera-core-0.1.0/passphera_core.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)      197 2024-04-05 01:53:54.000000 passphera-core-0.1.0/passphera_core.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-05 01:53:54.000000 passphera-core-0.1.0/passphera_core.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-05 01:53:54.000000 passphera-core-0.1.0/passphera_core.egg-info/top_level.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-05 01:53:54.504895 passphera-core-0.1.0/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-05 01:53:43.000000 passphera-core-0.1.0/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-07 16:29:28.641326 passphera-core-0.2.0/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-07 16:29:28.640325 passphera-core-0.2.0/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       54 2024-04-05 01:50:44.000000 passphera-core-0.2.0/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-07 16:29:28.638326 passphera-core-0.2.0/passphera_core/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     7845 2024-04-07 16:27:57.000000 passphera-core-0.2.0/passphera_core/__init__.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-07 16:29:28.640325 passphera-core-0.2.0/passphera_core.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      627 2024-04-07 16:29:28.000000 passphera-core-0.2.0/passphera_core.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      197 2024-04-07 16:29:28.000000 passphera-core-0.2.0/passphera_core.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-07 16:29:28.000000 passphera-core-0.2.0/passphera_core.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       15 2024-04-07 16:29:28.000000 passphera-core-0.2.0/passphera_core.egg-info/top_level.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-07 16:29:28.641326 passphera-core-0.2.0/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      792 2024-04-07 16:20:14.000000 passphera-core-0.2.0/setup.py
```

### Comparing `passphera-core-0.1.0/PKG-INFO` & `passphera-core-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.1.0
+Version: 0.2.0
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.1.0/passphera_core.egg-info/PKG-INFO` & `passphera-core-0.2.0/passphera_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: passphera-core
-Version: 0.1.0
+Version: 0.2.0
 Summary: The core system of passphera project
 Home-page: https://github.com/passphera/core
 Author: Fathi Abdelmalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `passphera-core-0.1.0/setup.py` & `passphera-core-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='passphera-core',
-    version='0.1.0',
+    version='0.2.0',
     author='Fathi Abdelmalek',
     author_email='abdelmalek.fathi.2001@gmail.com',
     url='https://github.com/passphera/core',
     description='The core system of passphera project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['passphera_core'],
```

