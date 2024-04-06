# Comparing `tmp/ffats-1.3.6.tar.gz` & `tmp/ffats-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffats-1.3.6.tar", last modified: Sat Apr  6 19:23:38 2024, max compression
+gzip compressed data, was "ffats-1.3.7.tar", last modified: Sat Apr  6 22:11:12 2024, max compression
```

## Comparing `ffats-1.3.6.tar` & `ffats-1.3.7.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 19:23:38.403493 ffats-1.3.6/
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 19:23:38.400160 ffats-1.3.6/FFATS/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      166 2024-04-04 07:15:17.000000 ffats-1.3.6/FFATS/Base.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     7007 2024-04-04 07:31:13.000000 ffats-1.3.6/FFATS/Feature.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)    36492 2024-04-05 23:43:13.000000 ffats-1.3.6/FFATS/FeatureFunctionLib.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      785 2024-04-04 07:15:55.000000 ffats-1.3.6/FFATS/PreprocessLC.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      221 2024-04-04 07:01:49.000000 ffats-1.3.6/FFATS/__init__.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1945 2024-04-04 08:05:18.000000 ffats-1.3.6/FFATS/alignLC.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      157 2024-04-04 07:30:52.000000 ffats-1.3.6/FFATS/featureFunction.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      706 2024-04-04 07:15:38.000000 ffats-1.3.6/FFATS/import_lc_cluster.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      724 2024-04-04 07:15:42.000000 ffats-1.3.6/FFATS/import_lightcurve.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     6572 2024-04-04 07:37:28.000000 ffats-1.3.6/FFATS/lomb.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)    11062 2024-04-05 19:13:56.000000 ffats-1.3.6/FFATS/test_library.py
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1079 2024-04-04 06:18:41.000000 ffats-1.3.6/LICENSE
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       25 2024-04-06 18:59:03.000000 ffats-1.3.6/MANIFEST.in
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-06 19:23:38.403493 ffats-1.3.6/PKG-INFO
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      581 2024-04-06 18:30:47.000000 ffats-1.3.6/README.rst
-drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 19:23:38.403493 ffats-1.3.6/ffats.egg-info/
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-06 19:23:38.000000 ffats-1.3.6/ffats.egg-info/PKG-INFO
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      474 2024-04-06 19:23:38.000000 ffats-1.3.6/ffats.egg-info/SOURCES.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 19:23:38.000000 ffats-1.3.6/ffats.egg-info/dependency_links.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 19:23:38.000000 ffats-1.3.6/ffats.egg-info/not-zip-safe
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 19:23:38.000000 ffats-1.3.6/ffats.egg-info/requires.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)        6 2024-04-06 19:23:38.000000 ffats-1.3.6/ffats.egg-info/top_level.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)      116 2024-04-06 18:09:17.000000 ffats-1.3.6/pyproject.toml
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 18:19:27.000000 ffats-1.3.6/requirements.txt
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)       38 2024-04-06 19:23:38.403493 ffats-1.3.6/setup.cfg
--rw-r--r--   0 vladimir  (1000) vladimir  (1000)     4570 2024-04-06 19:23:14.000000 ffats-1.3.6/setup.py
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      347 2024-04-06 21:16:24.000000 ffats-1.3.7/CMakeLists.txt
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/FFATS/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      166 2024-04-04 07:15:17.000000 ffats-1.3.7/FFATS/Base.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     7007 2024-04-04 07:31:13.000000 ffats-1.3.7/FFATS/Feature.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)    36472 2024-04-06 21:53:29.000000 ffats-1.3.7/FFATS/FeatureFunctionLib.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      785 2024-04-04 07:15:55.000000 ffats-1.3.7/FFATS/PreprocessLC.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      221 2024-04-04 07:01:49.000000 ffats-1.3.7/FFATS/__init__.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1945 2024-04-04 08:05:18.000000 ffats-1.3.7/FFATS/alignLC.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      157 2024-04-04 07:30:52.000000 ffats-1.3.7/FFATS/featureFunction.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      706 2024-04-04 07:15:38.000000 ffats-1.3.7/FFATS/import_lc_cluster.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      724 2024-04-04 07:15:42.000000 ffats-1.3.7/FFATS/import_lightcurve.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     6572 2024-04-04 07:37:28.000000 ffats-1.3.7/FFATS/lomb.py
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/FFATS/pybind11_CAR/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1975 2024-04-06 19:52:30.000000 ffats-1.3.7/FFATS/pybind11_CAR/fast_CAR.cpp
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)    11062 2024-04-06 19:33:32.000000 ffats-1.3.7/FFATS/test_library.py
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1079 2024-04-04 06:18:41.000000 ffats-1.3.7/LICENSE
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       64 2024-04-06 21:21:16.000000 ffats-1.3.7/MANIFEST.in
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-06 22:11:12.316820 ffats-1.3.7/PKG-INFO
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      581 2024-04-06 18:30:47.000000 ffats-1.3.7/README.rst
+drwxr-xr-x   0 vladimir  (1000) vladimir  (1000)        0 2024-04-06 22:11:12.316820 ffats-1.3.7/ffats.egg-info/
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     1464 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/PKG-INFO
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      521 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/SOURCES.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/dependency_links.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)        1 2024-04-06 20:10:00.000000 ffats-1.3.7/ffats.egg-info/not-zip-safe
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/requires.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       15 2024-04-06 22:11:12.000000 ffats-1.3.7/ffats.egg-info/top_level.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)      143 2024-04-06 21:50:16.000000 ffats-1.3.7/pyproject.toml
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       52 2024-04-06 18:19:27.000000 ffats-1.3.7/requirements.txt
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)       38 2024-04-06 22:11:12.316820 ffats-1.3.7/setup.cfg
+-rw-r--r--   0 vladimir  (1000) vladimir  (1000)     9421 2024-04-06 21:55:51.000000 ffats-1.3.7/setup.py
```

### Comparing `ffats-1.3.6/FFATS/Feature.py` & `ffats-1.3.7/FFATS/Feature.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/FFATS/FeatureFunctionLib.py` & `ffats-1.3.7/FFATS/FeatureFunctionLib.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from scipy.optimize import curve_fit
 from statsmodels.tsa import stattools
 from scipy.interpolate import interp1d
 
 from .Base import Base
 from . import lomb
 
-from .pybind11_CAR.build.fast_CAR import *
+from fast_CAR import *
 
 
 class Amplitude(Base):
     """Half the difference between the maximum and the minimum magnitude"""
 
     def __init__(self):
         self.Data = ['magnitude']
```

### Comparing `ffats-1.3.6/FFATS/PreprocessLC.py` & `ffats-1.3.7/FFATS/PreprocessLC.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/FFATS/alignLC.py` & `ffats-1.3.7/FFATS/alignLC.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/FFATS/import_lc_cluster.py` & `ffats-1.3.7/FFATS/import_lc_cluster.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/FFATS/import_lightcurve.py` & `ffats-1.3.7/FFATS/import_lightcurve.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/FFATS/lomb.py` & `ffats-1.3.7/FFATS/lomb.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/FFATS/test_library.py` & `ffats-1.3.7/FFATS/test_library.py`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/LICENSE` & `ffats-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/PKG-INFO` & `ffats-1.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffats
-Version: 1.3.6
+Version: 1.3.7
 Summary: Library with compilation of features for time series
 Home-page: https://github.com/vBazilevich/FFATS
 Download-URL: https://github.com/vBazilevich/FFATS
 Author: Vladimir Bazilevich
 Author-email: bazilevichvl@gmail.com
 License: MIT licence
 Keywords: times series features,light curves
```

### Comparing `ffats-1.3.6/README.rst` & `ffats-1.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `ffats-1.3.6/ffats.egg-info/PKG-INFO` & `ffats-1.3.7/ffats.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffats
-Version: 1.3.6
+Version: 1.3.7
 Summary: Library with compilation of features for time series
 Home-page: https://github.com/vBazilevich/FFATS
 Download-URL: https://github.com/vBazilevich/FFATS
 Author: Vladimir Bazilevich
 Author-email: bazilevichvl@gmail.com
 License: MIT licence
 Keywords: times series features,light curves
```

