# Comparing `tmp/pymer4-0.8.1.tar.gz` & `tmp/pymer4-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymer4-0.8.1.tar", last modified: Fri Sep  8 19:57:11 2023, max compression
+gzip compressed data, was "pymer4-0.8.2.tar", last modified: Sun Apr  7 02:24:08 2024, max compression
```

## Comparing `pymer4-0.8.1.tar` & `pymer4-0.8.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 19:57:11.357894 pymer4-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-09-08 19:34:50.000000 pymer4-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-09-08 19:34:50.000000 pymer4-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-09-08 19:57:11.357894 pymer4-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2023-09-08 19:34:50.000000 pymer4-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 19:57:11.353893 pymer4-0.8.1/pymer4/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 19:57:11.353893 pymer4-0.8.1/pymer4/models/
--rw-r--r--   0 runner    (1001) docker     (127)    28713 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/models/Lm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20376 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/models/Lm2.py
--rw-r--r--   0 runner    (1001) docker     (127)    71233 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/models/Lmer.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 19:57:11.357894 pymer4-0.8.1/pymer4/resources/
--rw-r--r--   0 runner    (1001) docker     (127)   258401 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/resources/gammas.csv
--rw-r--r--   0 runner    (1001) docker     (127)    18358 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/resources/sample_data.csv
--rw-r--r--   0 runner    (1001) docker     (127)    13410 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)    26523 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/test_install.py
--rw-r--r--   0 runner    (1001) docker     (127)    22582 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2023-09-08 19:34:50.000000 pymer4-0.8.1/pymer4/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 19:57:11.353893 pymer4-0.8.1/pymer4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2023-09-08 19:57:11.000000 pymer4-0.8.1/pymer4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      509 2023-09-08 19:57:11.000000 pymer4-0.8.1/pymer4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 19:57:11.000000 pymer4-0.8.1/pymer4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-09-08 19:57:11.000000 pymer4-0.8.1/pymer4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-08 19:57:11.000000 pymer4-0.8.1/pymer4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-09-08 19:34:50.000000 pymer4-0.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-09-08 19:57:11.357894 pymer4-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2023-09-08 19:34:50.000000 pymer4-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:24:08.307377 pymer4-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-07 02:17:41.000000 pymer4-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 02:17:41.000000 pymer4-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-07 02:24:08.307377 pymer4-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-07 02:17:41.000000 pymer4-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:24:08.303377 pymer4-0.8.2/pymer4/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:24:08.303377 pymer4-0.8.2/pymer4/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    28713 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/models/Lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20376 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/models/Lm2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71233 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/models/Lmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:24:08.307377 pymer4-0.8.2/pymer4/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)   258401 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/resources/gammas.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    18358 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/resources/sample_data.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26523 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/test_install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22580 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-07 02:17:41.000000 pymer4-0.8.2/pymer4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:24:08.307377 pymer4-0.8.2/pymer4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-07 02:24:08.000000 pymer4-0.8.2/pymer4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-07 02:24:08.000000 pymer4-0.8.2/pymer4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 02:24:08.000000 pymer4-0.8.2/pymer4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-07 02:24:08.000000 pymer4-0.8.2/pymer4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 02:24:08.000000 pymer4-0.8.2/pymer4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-07 02:17:41.000000 pymer4-0.8.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-07 02:24:08.307377 pymer4-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-07 02:17:41.000000 pymer4-0.8.2/setup.py
```

### Comparing `pymer4-0.8.1/LICENSE.txt` & `pymer4-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/PKG-INFO` & `pymer4-0.8.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymer4
-Version: 0.8.1
+Version: 0.8.2
 Summary: pymer4: all the convenience of lme4 in python
 Home-page: http://eshinjolly.com/pymer4/
 Author: Eshin Jolly
 Author-email: eshin.jolly.GR@dartmouth.edu
 License: MIT
 Keywords: statistics,multi-level-modeling,regression,analysis
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymer4-0.8.1/README.md` & `pymer4-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/bridge.py` & `pymer4-0.8.2/pymer4/bridge.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/io.py` & `pymer4-0.8.2/pymer4/io.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/models/Lm.py` & `pymer4-0.8.2/pymer4/models/Lm.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/models/Lm2.py` & `pymer4-0.8.2/pymer4/models/Lm2.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/models/Lmer.py` & `pymer4-0.8.2/pymer4/models/Lmer.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/resources/gammas.csv` & `pymer4-0.8.2/pymer4/resources/gammas.csv`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/resources/sample_data.csv` & `pymer4-0.8.2/pymer4/resources/sample_data.csv`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/simulate.py` & `pymer4-0.8.2/pymer4/simulate.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/stats.py` & `pymer4-0.8.2/pymer4/stats.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/test_install.py` & `pymer4-0.8.2/pymer4/test_install.py`

 * *Files identical despite different names*

### Comparing `pymer4-0.8.1/pymer4/utils.py` & `pymer4-0.8.2/pymer4/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -404,15 +404,15 @@
         return b
 
 
 def _logregress(x, y, all_stats=True):
     # Design matrix already has intercept. We want no regularization and the newton
     # solver to match as closely with R
 
-    model = LogisticRegression(penalty="none", solver="newton-cg", fit_intercept=False)
+    model = LogisticRegression(penalty=None, solver="newton-cg", fit_intercept=False)
     _ = model.fit(x, y)
     b = model.coef_
     fits = model.decision_function(x)
     # We only return probs for positive class
     fit_probs = model.predict_proba(x)[:, 1]
     fit_classes = model.predict(x)
```

### Comparing `pymer4-0.8.1/pymer4.egg-info/PKG-INFO` & `pymer4-0.8.2/pymer4.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymer4
-Version: 0.8.1
+Version: 0.8.2
 Summary: pymer4: all the convenience of lme4 in python
 Home-page: http://eshinjolly.com/pymer4/
 Author: Eshin Jolly
 Author-email: eshin.jolly.GR@dartmouth.edu
 License: MIT
 Keywords: statistics,multi-level-modeling,regression,analysis
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pymer4-0.8.1/setup.py` & `pymer4-0.8.2/setup.py`

 * *Files identical despite different names*

