# Comparing `tmp/astromcad-0.1.3.tar.gz` & `tmp/astromcad-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.3.tar", last modified: Sun Apr  7 16:28:28 2024, max compression
+gzip compressed data, was "astromcad-0.1.4.tar", last modified: Sun Apr  7 16:32:52 2024, max compression
```

## Comparing `astromcad-0.1.3.tar` & `astromcad-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:28:28.524918 astromcad-0.1.3/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:28:28.524109 astromcad-0.1.3/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.3/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:28:28.513179 astromcad-0.1.3/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.3/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     9280 2024-04-07 16:28:01.000000 astromcad-0.1.3/astromcad/astromcad.py
--rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.3/astromcad/iforests.pickle
--rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.3/astromcad/pretrained.keras
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:28:28.523372 astromcad-0.1.3/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       63 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:28:28.000000 astromcad-0.1.3/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:28:28.525105 astromcad-0.1.3/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      775 2024-04-07 16:28:18.000000 astromcad-0.1.3/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:32:52.814188 astromcad-0.1.4/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:32:52.813701 astromcad-0.1.4/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.4/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:32:52.802984 astromcad-0.1.4/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.4/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9284 2024-04-07 16:32:01.000000 astromcad-0.1.4/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.4/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.4/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:32:52.813203 astromcad-0.1.4/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:32:52.814328 astromcad-0.1.4/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 16:32:47.000000 astromcad-0.1.4/setup.py
```

### Comparing `astromcad-0.1.3/PKG-INFO` & `astromcad-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.3
+Version: 0.1.4
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.3/README.md` & `astromcad-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.3/astromcad/astromcad.py` & `astromcad-0.1.4/astromcad/astromcad.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         iforests = os.path.join(SCRIPT_DIR, "iforests.pickle")
         cls.mod = Custom(656, 4, 2, 9, 12)
         model = keras.models.load_model(pretrained_model)
         cls.mod.custom_model(model, 'lc', 'host', 'latent')
         cls.mod.create_encoder()
         cls.mod.mcif = mcif()
         with open(iforests, 'rb') as f:
-            cls.mcif.iforests = pickle.load(f)
+            cls.mod.mcif.iforests = pickle.load(f)
 
         
         # cls.mod = Custom(ntimesteps, 4, 2, 9, y_train.shape[-1])
         # cls.mod.custom_model(best.model, 'lc', 'host', 'latent')
         # cls.mod.create_encoder()
         # cls.mod.mcif = mcif()
         # cls.mod.mcif.iforests = best.iso_forests
```

### Comparing `astromcad-0.1.3/astromcad/iforests.pickle` & `astromcad-0.1.4/astromcad/iforests.pickle`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.3/astromcad/pretrained.keras` & `astromcad-0.1.4/astromcad/pretrained.keras`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.3/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.4/astromcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.3
+Version: 0.1.4
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.3/setup.py` & `astromcad-0.1.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
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
-    install_requires=['numpy', 'keras==2.15.0', 'tensorflow==2.15.0', 'matplotlib', 'scikit-learn'],
+    install_requires=['numpy', 'keras==2.15.0', 'tensorflow==2.15.0', 'matplotlib', 'scikit-learn==1.2.2'],
     keywords=[],
     package_data={'astromcad': ['*.keras', '*.pickle']},
     include_package_data=True,
     
 )
```

