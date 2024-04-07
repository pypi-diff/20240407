# Comparing `tmp/meter-digits-recognizer-0.2.0.tar.gz` & `tmp/meter-digits-recognizer-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meter-digits-recognizer-0.2.0.tar", last modified: Tue Dec 26 22:37:31 2023, max compression
+gzip compressed data, was "meter-digits-recognizer-0.2.1.tar", last modified: Sun Apr  7 16:08:05 2024, max compression
```

## Comparing `meter-digits-recognizer-0.2.0.tar` & `meter-digits-recognizer-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:37:31.205454 meter-digits-recognizer-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-12-26 22:37:31.205454 meter-digits-recognizer-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:37:31.201454 meter-digits-recognizer-0.2.0/meter_digits_recognizer/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer/_meter_digits_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer/_net.py
--rw-r--r--   0 runner    (1001) docker     (127)  1286708 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer/model.onnx
--rw-r--r--   0 runner    (1001) docker     (127)  1210083 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer/model_weights.pt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:37:31.205454 meter-digits-recognizer-0.2.0/meter_digits_recognizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2202 2023-12-26 22:37:31.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-26 22:37:31.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 22:37:31.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2023-12-26 22:37:31.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-26 22:37:31.000000 meter-digits-recognizer-0.2.0/meter_digits_recognizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 22:37:31.205454 meter-digits-recognizer-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-26 22:37:11.000000 meter-digits-recognizer-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:08:05.146421 meter-digits-recognizer-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-07 16:08:05.146421 meter-digits-recognizer-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:08:05.146421 meter-digits-recognizer-0.2.1/meter_digits_recognizer/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer/_meter_digits_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer/_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1286708 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer/model.onnx
+-rw-r--r--   0 runner    (1001) docker     (127)  1210083 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer/model_weights.pt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:08:05.146421 meter-digits-recognizer-0.2.1/meter_digits_recognizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-04-07 16:08:04.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-07 16:08:05.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:08:04.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-07 16:08:04.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 16:08:04.000000 meter-digits-recognizer-0.2.1/meter_digits_recognizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:08:05.146421 meter-digits-recognizer-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 16:07:49.000000 meter-digits-recognizer-0.2.1/setup.py
```

### Comparing `meter-digits-recognizer-0.2.0/PKG-INFO` & `meter-digits-recognizer-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: meter-digits-recognizer
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: repository, https://github.com/ardiloot/meter-digits-recognizer
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
-Requires-Dist: opencv-python<=4.6.0.66
+Requires-Dist: opencv-python
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipympl; extra == "dev"
```

### Comparing `meter-digits-recognizer-0.2.0/README.md` & `meter-digits-recognizer-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `meter-digits-recognizer-0.2.0/meter_digits_recognizer/_meter_digits_recognizer.py` & `meter-digits-recognizer-0.2.1/meter_digits_recognizer/_meter_digits_recognizer.py`

 * *Files identical despite different names*

### Comparing `meter-digits-recognizer-0.2.0/meter_digits_recognizer/_net.py` & `meter-digits-recognizer-0.2.1/meter_digits_recognizer/_net.py`

 * *Files identical despite different names*

### Comparing `meter-digits-recognizer-0.2.0/meter_digits_recognizer/model.onnx` & `meter-digits-recognizer-0.2.1/meter_digits_recognizer/model.onnx`

 * *Files identical despite different names*

### Comparing `meter-digits-recognizer-0.2.0/meter_digits_recognizer/model_weights.pt` & `meter-digits-recognizer-0.2.1/meter_digits_recognizer/model_weights.pt`

 * *Files identical despite different names*

### Comparing `meter-digits-recognizer-0.2.0/meter_digits_recognizer.egg-info/PKG-INFO` & `meter-digits-recognizer-0.2.1/meter_digits_recognizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: meter-digits-recognizer
-Version: 0.2.0
+Version: 0.2.1
 Project-URL: repository, https://github.com/ardiloot/meter-digits-recognizer
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
-Requires-Dist: opencv-python<=4.6.0.66
+Requires-Dist: opencv-python
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipympl; extra == "dev"
```

### Comparing `meter-digits-recognizer-0.2.0/pyproject.toml` & `meter-digits-recognizer-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 requires-python = ">=3.10.0"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy",
-    "opencv-python<=4.6.0.66",
+    "opencv-python",
 ]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/ardiloot/meter-digits-recognizer"
 
 [project.optional-dependencies]
```

