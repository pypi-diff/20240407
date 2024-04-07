# Comparing `tmp/automatic-meter-reader-1.2.1.tar.gz` & `tmp/automatic-meter-reader-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-meter-reader-1.2.1.tar", last modified: Sun Apr  7 16:11:37 2024, max compression
+gzip compressed data, was "automatic-meter-reader-1.2.2.tar", last modified: Sun Apr  7 19:34:00 2024, max compression
```

## Comparing `automatic-meter-reader-1.2.1.tar` & `automatic-meter-reader-1.2.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.012122 automatic-meter-reader-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-07 16:11:37.012122 automatic-meter-reader-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.004123 automatic-meter-reader-1.2.1/automatic_meter_reader/
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/cameras/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/cameras/espcam_120_deg.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.004123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-07 16:11:37.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:11:37.012122 automatic-meter-reader-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    40523 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/tests/test_image.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    34548 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/tests/test_image2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/tests/test_readout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.544206 automatic-meter-reader-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-07 19:34:00.544206 automatic-meter-reader-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.540206 automatic-meter-reader-1.2.2/automatic_meter_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.540206 automatic-meter-reader-1.2.2/automatic_meter_reader/cameras/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/cameras/espcam_120_deg.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.536206 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.540206 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.540206 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.540206 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.544206 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.544206 automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-07 19:34:00.000000 automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-07 19:34:00.000000 automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:34:00.000000 automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 19:34:00.000000 automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 19:34:00.000000 automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:34:00.544206 automatic-meter-reader-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:34:00.544206 automatic-meter-reader-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40523 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/tests/test_image.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    34548 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/tests/test_image2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 19:33:40.000000 automatic-meter-reader-1.2.2/tests/test_readout.py
```

### Comparing `automatic-meter-reader-1.2.1/PKG-INFO` & `automatic-meter-reader-1.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: automatic-meter-reader
-Version: 1.2.1
+Version: 1.2.2
 Project-URL: repository, https://github.com/ardiloot/automatic-meter-reader
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: meter-digits-recognizer==0.2.1
+Requires-Dist: meter-digits-recognizer==0.2.2
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipympl; extra == "dev"
```

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/__init__.py` & `automatic-meter-reader-1.2.2/automatic_meter_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/cameras/espcam_120_deg.json` & `automatic-meter-reader-1.2.2/automatic_meter_reader/cameras/espcam_120_deg.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/meter_config.json` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg` & `automatic-meter-reader-1.2.2/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/PKG-INFO` & `automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 Metadata-Version: 2.1
 Name: automatic-meter-reader
-Version: 1.2.1
+Version: 1.2.2
 Project-URL: repository, https://github.com/ardiloot/automatic-meter-reader
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: opencv-python
-Requires-Dist: meter-digits-recognizer==0.2.1
+Requires-Dist: meter-digits-recognizer==0.2.2
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipympl; extra == "dev"
```

### Comparing `automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/SOURCES.txt` & `automatic-meter-reader-1.2.2/automatic_meter_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/dev-requirements.txt` & `automatic-meter-reader-1.2.2/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/pyproject.toml` & `automatic-meter-reader-1.2.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 readme = "README.md"
 requires-python = ">=3.10.0"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
-    "numpy",
-    "opencv-python",
-    "meter-digits-recognizer==0.2.1",
+    "meter-digits-recognizer==0.2.2",
 ]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/ardiloot/automatic-meter-reader"
 
 [project.optional-dependencies]
```

### Comparing `automatic-meter-reader-1.2.1/tests/test_image.jpg` & `automatic-meter-reader-1.2.2/tests/test_image.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.2.1/tests/test_image2.jpg` & `automatic-meter-reader-1.2.2/tests/test_image2.jpg`

 * *Files identical despite different names*

