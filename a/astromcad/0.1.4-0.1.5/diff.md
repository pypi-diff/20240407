# Comparing `tmp/astromcad-0.1.4.tar.gz` & `tmp/astromcad-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.4.tar", last modified: Sun Apr  7 16:32:52 2024, max compression
+gzip compressed data, was "astromcad-0.1.5.tar", last modified: Sun Apr  7 20:03:33 2024, max compression
```

## Comparing `astromcad-0.1.4.tar` & `astromcad-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:32:52.814188 astromcad-0.1.4/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:32:52.813701 astromcad-0.1.4/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.4/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:32:52.802984 astromcad-0.1.4/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.4/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     9284 2024-04-07 16:32:01.000000 astromcad-0.1.4/astromcad/astromcad.py
--rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.4/astromcad/iforests.pickle
--rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.4/astromcad/pretrained.keras
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:32:52.813203 astromcad-0.1.4/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:32:52.000000 astromcad-0.1.4/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:32:52.814328 astromcad-0.1.4/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 16:32:47.000000 astromcad-0.1.4/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:03:33.341929 astromcad-0.1.5/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:03:33.341364 astromcad-0.1.5/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.5/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:03:33.322498 astromcad-0.1.5/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.5/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9298 2024-04-07 16:43:13.000000 astromcad-0.1.5/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.5/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.5/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:03:33.340835 astromcad-0.1.5/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 20:03:33.342053 astromcad-0.1.5/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 20:03:07.000000 astromcad-0.1.5/setup.py
```

### Comparing `astromcad-0.1.4/PKG-INFO` & `astromcad-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.4
+Version: 0.1.5
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.4/README.md` & `astromcad-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.4/astromcad/astromcad.py` & `astromcad-0.1.5/astromcad/astromcad.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class Detect:
     ntimesteps=656
     classes = []
     @classmethod
     def pad(cls, x_data):
         for ind in range(len(x_data)):
-            np.pad(x_data[ind], ((0, cls.ntimesteps - len(x_data[ind])), (0, 0)))
+            x_data[ind] = np.pad(x_data[ind], ((0, cls.ntimesteps - len(x_data[ind])), (0, 0)))
         return x_data
 
     @classmethod
     def init(cls):
         pretrained_model = os.path.join(SCRIPT_DIR, "pretrained.keras")
         iforests = os.path.join(SCRIPT_DIR, "iforests.pickle")
         cls.mod = Custom(656, 4, 2, 9, 12)
```

### Comparing `astromcad-0.1.4/astromcad/iforests.pickle` & `astromcad-0.1.5/astromcad/iforests.pickle`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.4/astromcad/pretrained.keras` & `astromcad-0.1.5/astromcad/pretrained.keras`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.4/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.5/astromcad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.4
+Version: 0.1.5
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.4/setup.py` & `astromcad-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Classifier-Based Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = long_description
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
```

