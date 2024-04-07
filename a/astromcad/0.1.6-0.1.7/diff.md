# Comparing `tmp/astromcad-0.1.6.tar.gz` & `tmp/astromcad-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.6.tar", last modified: Sun Apr  7 20:16:07 2024, max compression
+gzip compressed data, was "astromcad-0.1.7.tar", last modified: Sun Apr  7 20:17:56 2024, max compression
```

## Comparing `astromcad-0.1.6.tar` & `astromcad-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:16:07.229188 astromcad-0.1.6/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:16:07.228558 astromcad-0.1.6/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.6/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:16:07.216489 astromcad-0.1.6/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.6/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     9359 2024-04-07 20:15:26.000000 astromcad-0.1.6/astromcad/astromcad.py
--rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.6/astromcad/iforests.pickle
--rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.6/astromcad/pretrained.keras
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:16:07.227965 astromcad-0.1.6/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 20:16:07.229333 astromcad-0.1.6/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 20:16:02.000000 astromcad-0.1.6/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:17:56.341840 astromcad-0.1.7/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:17:56.341259 astromcad-0.1.7/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.7/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:17:56.329341 astromcad-0.1.7/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.7/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9371 2024-04-07 20:17:29.000000 astromcad-0.1.7/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.7/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.7/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:17:56.340740 astromcad-0.1.7/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 20:17:56.341977 astromcad-0.1.7/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 20:17:46.000000 astromcad-0.1.7/setup.py
```

### Comparing `astromcad-0.1.6/PKG-INFO` & `astromcad-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.6
+Version: 0.1.7
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.6/README.md` & `astromcad-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.6/astromcad/astromcad.py` & `astromcad-0.1.7/astromcad/astromcad.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         self.features=features
         self.contextual=contextual
         self.latent_size = latent_size
         self.timesteps=timesteps
 
     def pad(self, x_data):
         for ind in range(len(x_data)):
-            np.pad(x_data[ind], ((0, self.timesteps - len(x_data[ind])), (0, 0)))
+            x_data[ind]=np.pad(x_data[ind], ((0, self.timesteps - len(x_data[ind])), (0, 0)))
         return x_data
 
     def create_model(self):
         input_1 = Input((self.timesteps, self.features), name='lc')  # X.shape = (Nobjects, Ntimesteps, 4) CHANGE
         self.lc_name = 'lc'
         masking_input1 = Masking(mask_value=0.)(input_1)
```

### Comparing `astromcad-0.1.6/astromcad/iforests.pickle` & `astromcad-0.1.7/astromcad/iforests.pickle`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.6/astromcad/pretrained.keras` & `astromcad-0.1.7/astromcad/pretrained.keras`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.6/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.7/astromcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.6
+Version: 0.1.7
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.6/setup.py` & `astromcad-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Classifier-Based Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = long_description
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
```

