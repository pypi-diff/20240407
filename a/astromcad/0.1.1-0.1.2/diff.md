# Comparing `tmp/astromcad-0.1.1.tar.gz` & `tmp/astromcad-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.1.tar", last modified: Sun Apr  7 16:19:13 2024, max compression
+gzip compressed data, was "astromcad-0.1.2.tar", last modified: Sun Apr  7 16:22:16 2024, max compression
```

## Comparing `astromcad-0.1.1.tar` & `astromcad-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:19:13.385697 astromcad-0.1.1/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:19:13.385170 astromcad-0.1.1/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.1/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:19:13.371108 astromcad-0.1.1/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.1/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     9263 2024-04-07 16:11:54.000000 astromcad-0.1.1/astromcad/astromcad.py
--rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.1/astromcad/iforests.pickle
--rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.1/astromcad/pretrained.keras
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:19:13.384435 astromcad-0.1.1/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       47 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:19:13.385826 astromcad-0.1.1/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      759 2024-04-07 16:18:58.000000 astromcad-0.1.1/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:22:16.756628 astromcad-0.1.2/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:22:16.755981 astromcad-0.1.2/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.2/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:22:16.745156 astromcad-0.1.2/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.2/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9276 2024-04-07 16:21:54.000000 astromcad-0.1.2/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.2/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.2/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:22:16.755457 astromcad-0.1.2/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       63 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:22:16.756816 astromcad-0.1.2/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      775 2024-04-07 16:22:06.000000 astromcad-0.1.2/setup.py
```

### Comparing `astromcad-0.1.1/PKG-INFO` & `astromcad-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.1
+Version: 0.1.2
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.1/README.md` & `astromcad-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.1/astromcad/astromcad.py` & `astromcad-0.1.2/astromcad/astromcad.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras import Model
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.ensemble import IsolationForest
 import pickle
 import os
+import keras
   
 SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 
 class Detect:
     ntimesteps=656
     classes = []
     @classmethod
```

### Comparing `astromcad-0.1.1/astromcad/iforests.pickle` & `astromcad-0.1.2/astromcad/iforests.pickle`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.1/astromcad/pretrained.keras` & `astromcad-0.1.2/astromcad/pretrained.keras`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.1/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.2/astromcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.1
+Version: 0.1.2
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.1/setup.py` & `astromcad-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Classifier-Based Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = long_description
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
     author="Rithwik Gupta",
     author_email="<rithwikca2020@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=['numpy', 'keras', 'tensorflow', 'matplotlib', 'scikit-learn'],
+    install_requires=['numpy', 'keras==2.15.0', 'tensorflow==2.15.0', 'matplotlib', 'scikit-learn'],
     keywords=[],
     package_data={'astromcad': ['*.keras', '*.pickle']},
     include_package_data=True,
     
 )
```

