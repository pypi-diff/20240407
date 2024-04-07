# Comparing `tmp/astromcad-0.1.5.tar.gz` & `tmp/astromcad-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.5.tar", last modified: Sun Apr  7 20:03:33 2024, max compression
+gzip compressed data, was "astromcad-0.1.6.tar", last modified: Sun Apr  7 20:16:07 2024, max compression
```

## Comparing `astromcad-0.1.5.tar` & `astromcad-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:03:33.341929 astromcad-0.1.5/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:03:33.341364 astromcad-0.1.5/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.5/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:03:33.322498 astromcad-0.1.5/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.5/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     9298 2024-04-07 16:43:13.000000 astromcad-0.1.5/astromcad/astromcad.py
--rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.5/astromcad/iforests.pickle
--rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.5/astromcad/pretrained.keras
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:03:33.340835 astromcad-0.1.5/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 20:03:33.000000 astromcad-0.1.5/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 20:03:33.342053 astromcad-0.1.5/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 20:03:07.000000 astromcad-0.1.5/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:16:07.229188 astromcad-0.1.6/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:16:07.228558 astromcad-0.1.6/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.6/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:16:07.216489 astromcad-0.1.6/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.6/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9359 2024-04-07 20:15:26.000000 astromcad-0.1.6/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.6/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.6/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 20:16:07.227965 astromcad-0.1.6/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       70 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 20:16:07.000000 astromcad-0.1.6/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 20:16:07.229333 astromcad-0.1.6/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      782 2024-04-07 20:16:02.000000 astromcad-0.1.6/setup.py
```

### Comparing `astromcad-0.1.5/PKG-INFO` & `astromcad-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.5
+Version: 0.1.6
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.5/README.md` & `astromcad-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.5/astromcad/astromcad.py` & `astromcad-0.1.6/astromcad/astromcad.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     @classmethod
     def anomaly_score(cls, x_data, host_gal):
         return cls.mod.score(x_data, host_gal)
 
     @classmethod
     def plot_real_time(cls, x_data, host_gal):
-        cls.mod.plot_real_time(x_data, host_gal, [0.4827, 0.6223], x_data[:, 1] * 100 - 30, x_data[:, 2] * 500, x_data[:, 3] * 500, colors=['red', 'g'], names=['r', 'g'])
+        cls.mod.plot_real_time(x_data, [0.4827, 0.6223], x_data[:, 1] * 100 - 30, x_data[:, 2] * 500, x_data[:, 3] * 500, host_gal, colors=['red', 'g'], names=['r', 'g'])
     
         
     
 
 class Custom:
     def __init__(self, timesteps, features, contextual, latent_size, n_classes):
         self.n_classes=n_classes
@@ -194,14 +194,16 @@
         
         return ans
 
 
     def plot_real_time(self, x_data, bands, time_, flux_, error_, host_gal=None, names = [], colors = []):
         classification_scores = self.get_anomaly_real_time([x_data], [host_gal])[0]
 
+        assert(len(classification_scores) == len(time_));
+
         time = {i : [] for i in bands}
         flux = {i : [] for i in bands}
         error = {i : [] for i in bands}
 
         
     
         for ind, i in enumerate(x_data[:len(classification_scores)]):
@@ -221,15 +223,15 @@
         axs[0].set_ylabel('Flux', fontsize=27)
         for ind, i in enumerate(bands):
             axs[0].errorbar(time[i], flux[i], yerr=error[i], fmt='.', label = names[ind] if len(names) else None, color = colors[ind] if len(colors) else None)
     
     
         axs[1].set_ylabel('Anomaly Score', fontsize=27)
         axs[1].set_xlabel('Time Since Trigger', fontsize=27)
-        axs[1].plot(cur, classification_scores)
+        axs[1].plot(time_, classification_scores)
     
         axs[1].set_ylim(-0.3, 0.3)
         axs[1].set_yticks(ticks=np.arange(-0.3, 0.3, 0.1))
     
         axs[0].tick_params(axis='both', labelsize=27)
         axs[1].tick_params(axis='both', labelsize=27)
```

### Comparing `astromcad-0.1.5/astromcad/iforests.pickle` & `astromcad-0.1.6/astromcad/iforests.pickle`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.5/astromcad/pretrained.keras` & `astromcad-0.1.6/astromcad/pretrained.keras`

 * *Files identical despite different names*

### Comparing `astromcad-0.1.5/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.6/astromcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.5
+Version: 0.1.6
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.5/setup.py` & `astromcad-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 DESCRIPTION = 'Classifier-Based Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = long_description
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
```

