# Comparing `tmp/camlab-0.0.8.1.tar.gz` & `tmp/camlab-0.0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.0.8.1.tar", last modified: Sun Apr  7 14:44:58 2024, max compression
+gzip compressed data, was "camlab-0.0.8.2.tar", last modified: Sun Apr  7 14:47:24 2024, max compression
```

## Comparing `camlab-0.0.8.1.tar` & `camlab-0.0.8.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.474491 camlab-0.0.8.1/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.1/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:44:58.474316 camlab-0.0.8.1/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.1/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-07 14:42:23.000000 camlab-0.0.8.1/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 14:44:58.474531 camlab-0.0.8.1/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.472492 camlab-0.0.8.1/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.473465 camlab-0.0.8.1/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)      649 2024-04-07 14:43:15.000000 camlab-0.0.8.1/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-04-07 14:11:59.000000 camlab-0.0.8.1/src/camlab/camera.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.474162 camlab-0.0.8.1/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.686025 camlab-0.0.8.2/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.2/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:47:24.685859 camlab-0.0.8.2/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.2/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-07 14:46:55.000000 camlab-0.0.8.2/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 14:47:24.686059 camlab-0.0.8.2/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.684071 camlab-0.0.8.2/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.685004 camlab-0.0.8.2/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)      649 2024-04-07 14:46:31.000000 camlab-0.0.8.2/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-04-07 14:11:59.000000 camlab-0.0.8.2/src/camlab/camera.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:47:24.685700 camlab-0.0.8.2/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 14:47:24.000000 camlab-0.0.8.2/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.0.8.1/LICENSE` & `camlab-0.0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.1/PKG-INFO` & `camlab-0.0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.1
+Version: 0.0.8.2
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camlab-0.0.8.1/README.md` & `camlab-0.0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.1/pyproject.toml` & `camlab-0.0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.0.8.1"
+version = "0.0.8.2"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.0.8.1/src/camlab/__init__.py` & `camlab-0.0.8.2/src/camlab/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     return pixels / (2 * math.tan(fov / 2))
 
 
 def focal2fov(focal, pixels):
     return 2 * math.atan(pixels / (2 * focal))
 
 
-def load_3dgs_camera(gs_cam):
+def load_3dgs_camera(cam_gs):
     """
     Support 3D Gaussian Splatting Camera-Class Object
     """
     cam = CameraObj()
     cam.manual_init(focal=fov2focal(cam_gs.FoVx, cam_gs.image_width),
                     w=cam_gs.image_width, h=cam_gs.image_height)
```

### Comparing `camlab-0.0.8.1/src/camlab/camera.py` & `camlab-0.0.8.2/src/camlab/camera.py`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8.1/src/camlab.egg-info/PKG-INFO` & `camlab-0.0.8.2/src/camlab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8.1
+Version: 0.0.8.2
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

