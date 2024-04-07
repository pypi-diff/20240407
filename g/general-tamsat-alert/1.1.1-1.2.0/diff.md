# Comparing `tmp/general_tamsat_alert-1.1.1.tar.gz` & `tmp/general_tamsat_alert-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general_tamsat_alert-1.1.1.tar", last modified: Tue Apr  2 15:23:03 2024, max compression
+gzip compressed data, was "general_tamsat_alert-1.2.0.tar", last modified: Sun Apr  7 09:34:21 2024, max compression
```

## Comparing `general_tamsat_alert-1.1.1.tar` & `general_tamsat_alert-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/
--rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      448 2024-02-18 17:35:53.000000 general_tamsat_alert-1.1.1/README.md
--rw-rw-r--   0 john      (1001) john      (1001)      536 2024-04-02 15:22:54.000000 general_tamsat_alert-1.1.1/pyproject.toml
--rw-rw-r--   0 john      (1001) john      (1001)       38 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/setup.cfg
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/src/
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/src/general_tamsat_alert/
--rw-rw-r--   0 john      (1001) john      (1001)     2904 2024-04-02 15:14:12.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/__init__.py
--rw-rw-r--   0 john      (1001) john      (1001)     5898 2024-04-02 15:14:12.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/ensembles.py
--rw-rw-r--   0 john      (1001) john      (1001)     3269 2024-04-02 15:01:21.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/misc.py
--rw-rw-r--   0 john      (1001) john      (1001)     4842 2023-12-29 13:21:49.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/periodicity.py
--rw-rw-r--   0 john      (1001) john      (1001)     1881 2024-04-02 15:14:12.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/roc_auc.py
--rw-rw-r--   0 john      (1001) john      (1001)     3652 2024-04-02 15:06:02.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert/weighting_functions.py
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/
--rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1001) john      (1001)      545 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1001) john      (1001)        1 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1001) john      (1001)       27 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/requires.txt
--rw-rw-r--   0 john      (1001) john      (1001)       21 2024-04-02 15:23:03.000000 general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/top_level.txt
-drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-02 15:23:03.382694 general_tamsat_alert-1.1.1/tests/
--rw-rw-r--   0 john      (1001) john      (1001)        0 2023-12-29 18:10:31.000000 general_tamsat_alert-1.1.1/tests/test_ensembles.py
--rw-rw-r--   0 john      (1001) john      (1001)     1764 2023-12-29 19:04:08.000000 general_tamsat_alert-1.1.1/tests/test_periodicity.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 09:34:21.507160 general_tamsat_alert-1.2.0/
+-rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-07 09:34:21.507160 general_tamsat_alert-1.2.0/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      448 2024-02-18 17:35:53.000000 general_tamsat_alert-1.2.0/README.md
+-rw-rw-r--   0 john      (1001) john      (1001)      536 2024-04-07 09:32:55.000000 general_tamsat_alert-1.2.0/pyproject.toml
+-rw-rw-r--   0 john      (1001) john      (1001)       38 2024-04-07 09:34:21.507160 general_tamsat_alert-1.2.0/setup.cfg
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 09:34:21.503160 general_tamsat_alert-1.2.0/src/
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 09:34:21.503160 general_tamsat_alert-1.2.0/src/general_tamsat_alert/
+-rw-rw-r--   0 john      (1001) john      (1001)     6969 2024-04-07 09:28:13.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert/__init__.py
+-rw-rw-r--   0 john      (1001) john      (1001)     5946 2024-04-07 09:22:22.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert/ensembles.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3269 2024-04-02 15:01:21.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert/misc.py
+-rw-rw-r--   0 john      (1001) john      (1001)     4842 2023-12-29 13:21:49.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert/periodicity.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1881 2024-04-02 15:14:12.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert/roc_auc.py
+-rw-rw-r--   0 john      (1001) john      (1001)     3652 2024-04-02 15:06:02.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert/weighting_functions.py
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 09:34:21.503160 general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/
+-rw-r--r--   0 john      (1001) john      (1001)      761 2024-04-07 09:34:21.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1001) john      (1001)      545 2024-04-07 09:34:21.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1001) john      (1001)        1 2024-04-07 09:34:21.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       27 2024-04-07 09:34:21.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/requires.txt
+-rw-rw-r--   0 john      (1001) john      (1001)       21 2024-04-07 09:34:21.000000 general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/top_level.txt
+drwxrwxr-x   0 john      (1001) john      (1001)        0 2024-04-07 09:34:21.503160 general_tamsat_alert-1.2.0/tests/
+-rw-rw-r--   0 john      (1001) john      (1001)        0 2023-12-29 18:10:31.000000 general_tamsat_alert-1.2.0/tests/test_ensembles.py
+-rw-rw-r--   0 john      (1001) john      (1001)     1764 2023-12-29 19:04:08.000000 general_tamsat_alert-1.2.0/tests/test_periodicity.py
```

### Comparing `general_tamsat_alert-1.1.1/PKG-INFO` & `general_tamsat_alert-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_tamsat_alert
-Version: 1.1.1
+Version: 1.2.0
 Author-email: John Ellis <12johnellis@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: scipy
```

### Comparing `general_tamsat_alert-1.1.1/pyproject.toml` & `general_tamsat_alert-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "general_tamsat_alert"
-version = "1.1.1"
+version = "1.2.0"
 dependencies = [
     "numpy",
     "xarray",
     "scipy",
     "fastroc",
 ]
 authors = [
```

### Comparing `general_tamsat_alert-1.1.1/src/general_tamsat_alert/ensembles.py` & `general_tamsat_alert-1.2.0/src/general_tamsat_alert/ensembles.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     if do_increments == 1:
         ensembles[...] -= ensembles[look_back, ...]
         ensembles[...] += da.isel({time_label: initiation_index})
 
     ensembles[:look_back+1, ...] = da.isel(
         {time_label: slice(initiation_index - look_back, initiation_index+1)}
     ).values[..., np.newaxis]
-
+    weights.values[np.isnan(weights.values)] = 0
     return ensembles, weights
 
 
 def get_ensemble_indices(
     da: xr.DataArray,
     prediction_date: str,
     start_dates: List[str],
```

### Comparing `general_tamsat_alert-1.1.1/src/general_tamsat_alert/misc.py` & `general_tamsat_alert-1.2.0/src/general_tamsat_alert/misc.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.1.1/src/general_tamsat_alert/periodicity.py` & `general_tamsat_alert-1.2.0/src/general_tamsat_alert/periodicity.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.1.1/src/general_tamsat_alert/roc_auc.py` & `general_tamsat_alert-1.2.0/src/general_tamsat_alert/roc_auc.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.1.1/src/general_tamsat_alert/weighting_functions.py` & `general_tamsat_alert-1.2.0/src/general_tamsat_alert/weighting_functions.py`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/PKG-INFO` & `general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general_tamsat_alert
-Version: 1.1.1
+Version: 1.2.0
 Author-email: John Ellis <12johnellis@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 Requires-Dist: xarray
 Requires-Dist: scipy
```

### Comparing `general_tamsat_alert-1.1.1/src/general_tamsat_alert.egg-info/SOURCES.txt` & `general_tamsat_alert-1.2.0/src/general_tamsat_alert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `general_tamsat_alert-1.1.1/tests/test_periodicity.py` & `general_tamsat_alert-1.2.0/tests/test_periodicity.py`

 * *Files identical despite different names*

