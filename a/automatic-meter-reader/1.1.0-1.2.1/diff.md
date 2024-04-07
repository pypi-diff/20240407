# Comparing `tmp/automatic-meter-reader-1.1.0.tar.gz` & `tmp/automatic-meter-reader-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automatic-meter-reader-1.1.0.tar", last modified: Tue Dec 26 22:40:59 2023, max compression
+gzip compressed data, was "automatic-meter-reader-1.2.1.tar", last modified: Sun Apr  7 16:11:37 2024, max compression
```

## Comparing `automatic-meter-reader-1.1.0.tar` & `automatic-meter-reader-1.2.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.131040 automatic-meter-reader-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-26 22:40:59.131040 automatic-meter-reader-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.123040 automatic-meter-reader-1.1.0/automatic_meter_reader/
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.127040 automatic-meter-reader-1.1.0/automatic_meter_reader/cameras/
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/cameras/espcam_120_deg.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.123040 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.127040 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.127040 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.127040 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.127040 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.131040 automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      663 2023-12-26 22:40:59.000000 automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-26 22:40:59.000000 automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-26 22:40:59.000000 automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-12-26 22:40:59.000000 automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-26 22:40:59.000000 automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-26 22:40:59.131040 automatic-meter-reader-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-26 22:40:59.127040 automatic-meter-reader-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    40523 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/tests/test_image.jpg
--rw-r--r--   0 runner    (1001) docker     (127)    34548 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/tests/test_image2.jpg
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-12-26 22:40:33.000000 automatic-meter-reader-1.1.0/tests/test_readout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.012122 automatic-meter-reader-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-07 16:11:37.012122 automatic-meter-reader-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.004123 automatic-meter-reader-1.2.1/automatic_meter_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/cameras/
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/cameras/espcam_120_deg.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.004123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/
+-rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-07 16:11:37.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 16:11:36.000000 automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:11:37.012122 automatic-meter-reader-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:11:37.008123 automatic-meter-reader-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40523 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/tests/test_image.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)    34548 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/tests/test_image2.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 16:11:13.000000 automatic-meter-reader-1.2.1/tests/test_readout.py
```

### Comparing `automatic-meter-reader-1.1.0/PKG-INFO` & `automatic-meter-reader-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: automatic-meter-reader
-Version: 1.1.0
+Version: 1.2.1
 Project-URL: repository, https://github.com/ardiloot/automatic-meter-reader
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
-Requires-Dist: meter-digits-recognizer==0.2.0
+Requires-Dist: meter-digits-recognizer==0.2.1
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipympl; extra == "dev"
```

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/__init__.py` & `automatic-meter-reader-1.2.1/automatic_meter_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/cameras/espcam_120_deg.json` & `automatic-meter-reader-1.2.1/automatic_meter_reader/cameras/espcam_120_deg.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/meter_config.json` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/gas_bk25/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/lorenz_1997/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_cold/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/meter_config.json`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_0.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_1.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg` & `automatic-meter-reader-1.2.1/automatic_meter_reader/meter_models/wehrle_hot/template_2.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/PKG-INFO` & `automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: automatic-meter-reader
-Version: 1.1.0
+Version: 1.2.1
 Project-URL: repository, https://github.com/ardiloot/automatic-meter-reader
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: opencv-python
-Requires-Dist: meter-digits-recognizer==0.2.0
+Requires-Dist: meter-digits-recognizer==0.2.1
 Provides-Extra: dev
 Requires-Dist: matplotlib; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Requires-Dist: ipympl; extra == "dev"
```

### Comparing `automatic-meter-reader-1.1.0/automatic_meter_reader.egg-info/SOURCES.txt` & `automatic-meter-reader-1.2.1/automatic_meter_reader.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/dev-requirements.txt` & `automatic-meter-reader-1.2.1/dev-requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,167 +1,165 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --extra=dev --output-file=dev-requirements.txt
 #
-asttokens==2.2.1
+asttokens==2.4.1
     # via stack-data
-backcall==0.2.0
-    # via ipython
-build==0.10.0
+build==1.2.1
     # via pip-tools
-click==8.1.3
+click==8.1.7
     # via pip-tools
-colorama==0.4.6
+comm==0.2.2
     # via
-    #   build
-    #   click
-    #   ipython
-    #   pytest
-comm==0.1.3
-    # via ipykernel
-contourpy==1.0.7
+    #   ipykernel
+    #   ipywidgets
+contourpy==1.2.1
     # via matplotlib
-cycler==0.11.0
+cycler==0.12.1
     # via matplotlib
-debugpy==1.6.7
+debugpy==1.8.1
     # via ipykernel
 decorator==5.1.1
     # via ipython
-executing==1.2.0
+executing==2.0.1
     # via stack-data
-flake8==6.0.0
+flake8==7.0.0
     # via automatic-meter-reader (setup.py)
-fonttools==4.39.3
+fonttools==4.51.0
     # via matplotlib
 iniconfig==2.0.0
     # via pytest
-ipykernel==6.23.3
-    # via
-    #   automatic-meter-reader (setup.py)
-    #   ipywidgets
+ipykernel==6.29.4
+    # via automatic-meter-reader (setup.py)
 ipympl==0.9.3
     # via automatic-meter-reader (setup.py)
-ipython==8.13.1
+ipython==8.23.0
     # via
     #   ipykernel
     #   ipympl
     #   ipywidgets
 ipython-genutils==0.2.0
     # via ipympl
-ipywidgets==8.0.6
+ipywidgets==8.1.2
     # via ipympl
-jedi==0.18.2
+jedi==0.19.1
     # via ipython
-jupyter-client==8.2.0
+jupyter-client==8.6.1
     # via ipykernel
-jupyter-core==5.3.0
+jupyter-core==5.7.2
     # via
     #   ipykernel
     #   jupyter-client
-jupyterlab-widgets==3.0.7
+jupyterlab-widgets==3.0.10
     # via ipywidgets
-kiwisolver==1.4.4
+kiwisolver==1.4.5
     # via matplotlib
-matplotlib==3.7.1
+matplotlib==3.8.4
     # via
     #   automatic-meter-reader (setup.py)
     #   ipympl
 matplotlib-inline==0.1.6
     # via
     #   ipykernel
     #   ipython
 mccabe==0.7.0
     # via flake8
-meter-digits-recognizer==0.1.13
+meter-digits-recognizer==0.2.1
     # via automatic-meter-reader (setup.py)
-nest-asyncio==1.5.6
+nest-asyncio==1.6.0
     # via ipykernel
-numpy==1.24.3
+numpy==1.26.4
     # via
     #   automatic-meter-reader (setup.py)
     #   contourpy
     #   ipympl
     #   matplotlib
     #   meter-digits-recognizer
     #   opencv-python
-opencv-python==4.6.0.66
+opencv-python==4.9.0.80
     # via
     #   automatic-meter-reader (setup.py)
     #   meter-digits-recognizer
-packaging==23.1
+packaging==24.0
     # via
     #   build
     #   ipykernel
     #   matplotlib
     #   pytest
-parso==0.8.3
+parso==0.8.4
     # via jedi
-pickleshare==0.7.5
+pexpect==4.9.0
     # via ipython
-pillow==9.5.0
+pillow==10.3.0
     # via
     #   ipympl
     #   matplotlib
-pip-tools==6.13.0
+pip-tools==7.4.1
     # via automatic-meter-reader (setup.py)
-platformdirs==3.5.0
+platformdirs==4.2.0
     # via jupyter-core
-pluggy==1.0.0
+pluggy==1.4.0
     # via pytest
-prompt-toolkit==3.0.38
+prompt-toolkit==3.0.43
     # via ipython
-psutil==5.9.5
+psutil==5.9.8
     # via ipykernel
+ptyprocess==0.7.0
+    # via pexpect
 pure-eval==0.2.2
     # via stack-data
-pycodestyle==2.10.0
+pycodestyle==2.11.1
     # via flake8
-pyflakes==3.0.1
+pyflakes==3.2.0
     # via flake8
-pygments==2.15.1
+pygments==2.17.2
     # via ipython
-pyparsing==3.0.9
+pyparsing==3.1.2
     # via matplotlib
 pyproject-hooks==1.0.0
-    # via build
-pytest==7.3.1
+    # via
+    #   build
+    #   pip-tools
+pytest==8.1.1
     # via automatic-meter-reader (setup.py)
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via
     #   jupyter-client
     #   matplotlib
-pywin32==306
-    # via jupyter-core
-pyzmq==25.1.0
+pyzmq==25.1.2
     # via
     #   ipykernel
     #   jupyter-client
 six==1.16.0
-    # via python-dateutil
-stack-data==0.6.2
+    # via
+    #   asttokens
+    #   python-dateutil
+stack-data==0.6.3
     # via ipython
-tornado==6.3.2
+tornado==6.4
     # via
     #   ipykernel
     #   jupyter-client
-traitlets==5.9.0
+traitlets==5.14.2
     # via
     #   comm
     #   ipykernel
     #   ipympl
     #   ipython
     #   ipywidgets
     #   jupyter-client
     #   jupyter-core
     #   matplotlib-inline
-wcwidth==0.2.6
+typing-extensions==4.11.0
+    # via ipython
+wcwidth==0.2.13
     # via prompt-toolkit
-wheel==0.40.0
+wheel==0.43.0
     # via pip-tools
-widgetsnbextension==4.0.7
+widgetsnbextension==4.0.10
     # via ipywidgets
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `automatic-meter-reader-1.1.0/pyproject.toml` & `automatic-meter-reader-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy",
     "opencv-python",
-    "meter-digits-recognizer==0.2.0",
+    "meter-digits-recognizer==0.2.1",
 ]
 dynamic = ["version"]
 
 [project.urls]
 repository = "https://github.com/ardiloot/automatic-meter-reader"
 
 [project.optional-dependencies]
```

### Comparing `automatic-meter-reader-1.1.0/tests/test_image.jpg` & `automatic-meter-reader-1.2.1/tests/test_image.jpg`

 * *Files identical despite different names*

### Comparing `automatic-meter-reader-1.1.0/tests/test_image2.jpg` & `automatic-meter-reader-1.2.1/tests/test_image2.jpg`

 * *Files identical despite different names*

