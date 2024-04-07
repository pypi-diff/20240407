# Comparing `tmp/astromcad-0.1.2.tar.gz` & `tmp/astromcad-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.2.tar", last modified: Sun Apr  7 16:22:16 2024, max compression
+gzip compressed data, was "astromcad-0.1.3.tar", last modified: Sun Apr  7 16:28:28 2024, max compression
```

## Comparing `astromcad-0.1.2.tar` & `astromcad-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:22:16.756628 astromcad-0.1.2/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:22:16.755981 astromcad-0.1.2/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.2/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:22:16.745156 astromcad-0.1.2/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.2/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     9276 2024-04-07 16:21:54.000000 astromcad-0.1.2/astromcad/astromcad.py
--rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.2/astromcad/iforests.pickle
--rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.2/astromcad/pretrained.keras
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:22:16.755457 astromcad-0.1.2/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       63 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:22:16.000000 astromcad-0.1.2/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:22:16.756816 astromcad-0.1.2/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      775 2024-04-07 16:22:06.000000 astromcad-0.1.2/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:28:28.524918 astromcad-0.1.3/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:28:28.524109 astromcad-0.1.3/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.3/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:28:28.513179 astromcad-0.1.3/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.3/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9280 2024-04-07 16:28:01.000000 astromcad-0.1.3/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.3/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.3/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:28:28.523372 astromcad-0.1.3/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       63 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:28:28.525105 astromcad-0.1.3/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      775 2024-04-07 16:28:18.000000 astromcad-0.1.3/setup.py
```

### Comparing `astromcad-0.1.2/PKG-INFO` & `astromcad-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.2
+Version: 0.1.3
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.2/README.md` & `astromcad-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.2/astromcad/astromcad.py` & `astromcad-0.1.3/astromcad/astromcad.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     @classmethod
     def init(cls):
         pretrained_model = os.path.join(SCRIPT_DIR, "pretrained.keras")
         iforests = os.path.join(SCRIPT_DIR, "iforests.pickle")
         cls.mod = Custom(656, 4, 2, 9, 12)
         model = keras.models.load_model(pretrained_model)
         cls.mod.custom_model(model, 'lc', 'host', 'latent')
-        mod.create_encoder()
+        cls.mod.create_encoder()
         cls.mod.mcif = mcif()
         with open(iforests, 'rb') as f:
             cls.mcif.iforests = pickle.load(f)
 
         
         # cls.mod = Custom(ntimesteps, 4, 2, 9, y_train.shape[-1])
         # cls.mod.custom_model(best.model, 'lc', 'host', 'latent')
```

### Comparing `astromcad-0.1.2/astromcad/iforests.pickle` & `astromcad-0.1.3/astromcad/iforests.pickle`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.2/astromcad/pretrained.keras` & `astromcad-0.1.3/astromcad/pretrained.keras`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.2/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.3/astromcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.2
+Version: 0.1.3
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.2/setup.py` & `astromcad-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Classifier-Based Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = long_description
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
```

