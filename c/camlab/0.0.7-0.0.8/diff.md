# Comparing `tmp/camlab-0.0.7.tar.gz` & `tmp/camlab-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.0.7.tar", last modified: Fri Nov 17 08:07:25 2023, max compression
+gzip compressed data, was "camlab-0.0.8.tar", last modified: Sun Apr  7 14:38:11 2024, max compression
```

## Comparing `camlab-0.0.7.tar` & `camlab-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2023-11-17 08:07:25.502910 camlab-0.0.7/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2023-11-09 18:01:12.000000 camlab-0.0.7/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     1907 2023-11-17 08:07:25.502748 camlab-0.0.7/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1428 2023-11-13 15:12:42.000000 camlab-0.0.7/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      539 2023-11-17 08:06:53.000000 camlab-0.0.7/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2023-11-17 08:07:25.502996 camlab-0.0.7/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2023-11-17 08:07:25.500916 camlab-0.0.7/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2023-11-17 08:07:25.501956 camlab-0.0.7/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)       22 2023-11-09 19:06:22.000000 camlab-0.0.7/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     6895 2023-11-17 08:06:25.000000 camlab-0.0.7/src/camlab/camera.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2023-11-17 08:07:25.502575 camlab-0.0.7/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     1907 2023-11-17 08:07:25.000000 camlab-0.0.7/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      212 2023-11-17 08:07:25.000000 camlab-0.0.7/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2023-11-17 08:07:25.000000 camlab-0.0.7/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2023-11-17 08:07:25.000000 camlab-0.0.7/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.860918 camlab-0.0.8/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-04-07 14:38:11.860753 camlab-0.0.8/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      539 2024-04-07 14:12:41.000000 camlab-0.0.8/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 14:38:11.860956 camlab-0.0.8/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.858969 camlab-0.0.8/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.859915 camlab-0.0.8/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)      483 2024-04-07 14:23:13.000000 camlab-0.0.8/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-04-07 14:11:59.000000 camlab-0.0.8/src/camlab/camera.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.860585 camlab-0.0.8/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.0.7/LICENSE` & `camlab-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.0.7/PKG-INFO` & `camlab-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.7
+Version: 0.0.8
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CamLab
 ## play with camera pose
 
+```sh
+pip install camlab
+```
+
+<p float="center">
+  <img src="assets/camera_system_calibration.gif" width="78%" />
+</p>
+
 project a world-coordinate point to screen coordniate:
 
 ```python
 import numpy as np
 from camlab import CameraObj
 
 
@@ -71,7 +79,8 @@
 # (rayd - rayo) represents a point at the ray.
 p_ = cam_obj.world2screen(rayd - rayo, to_int=True)
 # reproject the ray point to screen
 print(p_)
 # (400, 400)
 
 ``` 
+
```

### Comparing `camlab-0.0.7/README.md` & `camlab-0.0.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 # CamLab
 ## play with camera pose
 
+```sh
+pip install camlab
+```
+
+<p float="center">
+  <img src="assets/camera_system_calibration.gif" width="78%" />
+</p>
+
 project a world-coordinate point to screen coordniate:
 
 ```python
 import numpy as np
 from camlab import CameraObj
 
 
@@ -57,7 +65,8 @@
 # (rayd - rayo) represents a point at the ray.
 p_ = cam_obj.world2screen(rayd - rayo, to_int=True)
 # reproject the ray point to screen
 print(p_)
 # (400, 400)
 
 ``` 
+
```

### Comparing `camlab-0.0.7/pyproject.toml` & `camlab-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.0.7/src/camlab/camera.py` & `camlab-0.0.8/src/camlab/camera.py`

 * *Files identical despite different names*

### Comparing `camlab-0.0.7/src/camlab.egg-info/PKG-INFO` & `camlab-0.0.8/src/camlab.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.7
+Version: 0.0.8
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CamLab
 ## play with camera pose
 
+```sh
+pip install camlab
+```
+
+<p float="center">
+  <img src="assets/camera_system_calibration.gif" width="78%" />
+</p>
+
 project a world-coordinate point to screen coordniate:
 
 ```python
 import numpy as np
 from camlab import CameraObj
 
 
@@ -71,7 +79,8 @@
 # (rayd - rayo) represents a point at the ray.
 p_ = cam_obj.world2screen(rayd - rayo, to_int=True)
 # reproject the ray point to screen
 print(p_)
 # (400, 400)
 
 ``` 
+
```

