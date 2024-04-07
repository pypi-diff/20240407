# Comparing `tmp/astromcad-0.1.7.tar.gz` & `tmp/astromcad-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.7.tar", last modified: Sun Apr  7 20:17:56 2024, max compression
+gzip compressed data, was "astromcad-0.1.8.tar", last modified: Sun Apr  7 21:07:36 2024, max compression
```

## Comparing `astromcad-0.1.7.tar` & `astromcad-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:17:56.341840 astromcad-0.1.7/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:17:56.341259 astromcad-0.1.7/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.7/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:17:56.329341 astromcad-0.1.7/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.7/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     9371 2024-04-07 20:17:29.000000 astromcad-0.1.7/astromcad/astromcad.py
--rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.7/astromcad/iforests.pickle
--rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.7/astromcad/pretrained.keras
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:17:56.340740 astromcad-0.1.7/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 20:17:56.000000 astromcad-0.1.7/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 20:17:56.341977 astromcad-0.1.7/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 20:17:46.000000 astromcad-0.1.7/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 21:07:36.156653 astromcad-0.1.8/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 21:07:36.156070 astromcad-0.1.8/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.8/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 21:07:36.146395 astromcad-0.1.8/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.8/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9498 2024-04-07 21:05:55.000000 astromcad-0.1.8/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.8/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.8/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 21:07:36.155539 astromcad-0.1.8/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 21:07:35.000000 astromcad-0.1.8/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 21:07:35.000000 astromcad-0.1.8/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 21:07:35.000000 astromcad-0.1.8/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 21:07:35.000000 astromcad-0.1.8/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 21:07:35.000000 astromcad-0.1.8/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 21:07:36.156788 astromcad-0.1.8/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 21:07:24.000000 astromcad-0.1.8/setup.py
```

### Comparing `astromcad-0.1.7/PKG-INFO` & `astromcad-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.7
+Version: 0.1.8
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.7/README.md` & `astromcad-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.7/astromcad/astromcad.py` & `astromcad-0.1.8/astromcad/astromcad.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,14 +193,18 @@
             prv=diff
         
         return ans
 
 
     def plot_real_time(self, x_data, bands, time_, flux_, error_, host_gal=None, names = [], colors = []):
         classification_scores = self.get_anomaly_real_time([x_data], [host_gal])[0]
+        tot = len(classification_scores)
+        time_ = time_[:tot]
+        flux_ = flux_[:tot]
+        error_ = error_[:tot]
 
         assert(len(classification_scores) == len(time_));
 
         time = {i : [] for i in bands}
         flux = {i : [] for i in bands}
         error = {i : [] for i in bands}
```

### Comparing `astromcad-0.1.7/astromcad/iforests.pickle` & `astromcad-0.1.8/astromcad/iforests.pickle`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.7/astromcad/pretrained.keras` & `astromcad-0.1.8/astromcad/pretrained.keras`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.7/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.8/astromcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.7
+Version: 0.1.8
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.7/setup.py` & `astromcad-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Classifier-Based Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = long_description
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
```

