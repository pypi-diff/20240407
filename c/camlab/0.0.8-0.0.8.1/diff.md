# Comparing `tmp/camlab-0.0.8.tar.gz` & `tmp/camlab-0.0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camlab-0.0.8.tar", last modified: Sun Apr  7 14:38:11 2024, max compression
+gzip compressed data, was "camlab-0.0.8.1.tar", last modified: Sun Apr  7 14:44:58 2024, max compression
```

## Comparing `camlab-0.0.8.tar` & `camlab-0.0.8.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.860918 camlab-0.0.8/
--rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8/LICENSE
--rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-04-07 14:38:11.860753 camlab-0.0.8/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8/README.md
--rw-r--r--   0 muzhan     (501) staff       (20)      539 2024-04-07 14:12:41.000000 camlab-0.0.8/pyproject.toml
--rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 14:38:11.860956 camlab-0.0.8/setup.cfg
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.858969 camlab-0.0.8/src/
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.859915 camlab-0.0.8/src/camlab/
--rw-r--r--   0 muzhan     (501) staff       (20)      483 2024-04-07 14:23:13.000000 camlab-0.0.8/src/camlab/__init__.py
--rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-04-07 14:11:59.000000 camlab-0.0.8/src/camlab/camera.py
-drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:38:11.860585 camlab-0.0.8/src/camlab.egg-info/
--rw-r--r--   0 muzhan     (501) staff       (20)     2028 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/PKG-INFO
--rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/SOURCES.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/dependency_links.txt
--rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 14:38:11.000000 camlab-0.0.8/src/camlab.egg-info/top_level.txt
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.474491 camlab-0.0.8.1/
+-rw-r--r--   0 muzhan     (501) staff       (20)     1075 2024-04-07 14:11:59.000000 camlab-0.0.8.1/LICENSE
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:44:58.474316 camlab-0.0.8.1/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)     1549 2024-04-07 14:11:59.000000 camlab-0.0.8.1/README.md
+-rw-r--r--   0 muzhan     (501) staff       (20)      541 2024-04-07 14:42:23.000000 camlab-0.0.8.1/pyproject.toml
+-rw-r--r--   0 muzhan     (501) staff       (20)       38 2024-04-07 14:44:58.474531 camlab-0.0.8.1/setup.cfg
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.472492 camlab-0.0.8.1/src/
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.473465 camlab-0.0.8.1/src/camlab/
+-rw-r--r--   0 muzhan     (501) staff       (20)      649 2024-04-07 14:43:15.000000 camlab-0.0.8.1/src/camlab/__init__.py
+-rw-r--r--   0 muzhan     (501) staff       (20)     6895 2024-04-07 14:11:59.000000 camlab-0.0.8.1/src/camlab/camera.py
+drwxr-xr-x   0 muzhan     (501) staff       (20)        0 2024-04-07 14:44:58.474162 camlab-0.0.8.1/src/camlab.egg-info/
+-rw-r--r--   0 muzhan     (501) staff       (20)     2030 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/PKG-INFO
+-rw-r--r--   0 muzhan     (501) staff       (20)      212 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/SOURCES.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        1 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/dependency_links.txt
+-rw-r--r--   0 muzhan     (501) staff       (20)        7 2024-04-07 14:44:58.000000 camlab-0.0.8.1/src/camlab.egg-info/top_level.txt
```

### Comparing `camlab-0.0.8/LICENSE` & `camlab-0.0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8/PKG-INFO` & `camlab-0.0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `camlab-0.0.8/README.md` & `camlab-0.0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8/pyproject.toml` & `camlab-0.0.8.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "camlab"
-version = "0.0.8"
+version = "0.0.8.1"
 authors = [
   { name="Levi", email="levio.pku@gmail.com" },
 ]
 description = "play with camera poses"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `camlab-0.0.8/src/camlab/camera.py` & `camlab-0.0.8.1/src/camlab/camera.py`

 * *Files identical despite different names*

### Comparing `camlab-0.0.8/src/camlab.egg-info/PKG-INFO` & `camlab-0.0.8.1/src/camlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camlab
-Version: 0.0.8
+Version: 0.0.8.1
 Summary: play with camera poses
 Author-email: Levi <levio.pku@gmail.com>
 Project-URL: Homepage, https://github.com/leviome/camlab
 Project-URL: Bug Tracker, https://github.com/leviome/camlab/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

