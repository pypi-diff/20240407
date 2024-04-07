# Comparing `tmp/camlab-0.0.8.2.tar.gz` & `tmp/camlab-0.0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.0.8.2.tar", last modified: Sun Apr  7 14:47:24 2024, max compression
+gzip compressed data, was "camlab-0.0.8.3.tar", last modified: Sun Apr  7 15:40:21 2024, max compression
```

## Comparing `camlab-0.0.8.2.tar` & `camlab-0.0.8.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.686025 camlab-0.0.8.2/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.2/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:47:24.685859 camlab-0.0.8.2/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.2/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-07 14:46:55.000000 camlab-0.0.8.2/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 14:47:24.686059 camlab-0.0.8.2/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.684071 camlab-0.0.8.2/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.685004 camlab-0.0.8.2/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)      649 2024-04-07 14:46:31.000000 camlab-0.0.8.2/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-04-07 14:11:59.000000 camlab-0.0.8.2/src/camlab/camera.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.685700 camlab-0.0.8.2/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:40:21.048370 camlab-0.0.8.3/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.3/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 15:40:21.048204 camlab-0.0.8.3/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.3/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-07 15:39:52.000000 camlab-0.0.8.3/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 15:40:21.048407 camlab-0.0.8.3/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:40:21.046347 camlab-0.0.8.3/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:40:21.047252 camlab-0.0.8.3/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)      649 2024-04-07 14:46:31.000000 camlab-0.0.8.3/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     6966 2024-04-07 15:39:19.000000 camlab-0.0.8.3/src/camlab/camera.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 15:40:21.048036 camlab-0.0.8.3/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 15:40:21.000000 camlab-0.0.8.3/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 15:40:21.000000 camlab-0.0.8.3/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 15:40:21.000000 camlab-0.0.8.3/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 15:40:21.000000 camlab-0.0.8.3/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.0.8.2/LICENSE` & `camlab-0.0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.2/PKG-INFO` & `camlab-0.0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.2
+Version: 0.0.8.3
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camlab-0.0.8.2/README.md` & `camlab-0.0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.2/pyproject.toml` & `camlab-0.0.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.0.8.2"
+version = "0.0.8.3"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.0.8.2/src/camlab/__init__.py` & `camlab-0.0.8.3/src/camlab/__init__.py`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.2/src/camlab/camera.py` & `camlab-0.0.8.3/src/camlab/camera.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 
 class CameraObj:
-    def __init__(self, intri_mat=None):
+    def __init__(self, intri_mat=None, image_path=None):
         # intrinsic
         self.focal_x = None
         self.focal_y = None
         self.o_x = None
         self.o_y = None
         self.K = None
 
@@ -13,14 +13,17 @@
         self.h = None
         self.w = None
 
         # extrinsic
         self.R = None
         self.T = None
         self.is_intri_set = False
+
+        # image
+        self.image_path = image_path
         
         self.touch = 0
 
         if intri_mat:
             self.K = intri_mat
             self.focal_x = intri_mat[0][0]
             self.focal_y = intri_mat[1][1]
```

### Comparing `camlab-0.0.8.2/src/camlab.egg-info/PKG-INFO` & `camlab-0.0.8.3/src/camlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.2
+Version: 0.0.8.3
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

