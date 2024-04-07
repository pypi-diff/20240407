# Comparing `tmp/ramanspy-0.2.8.tar.gz` & `tmp/ramanspy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ramanspy-0.2.8.tar", last modified: Fri Mar 15 10:30:19 2024, max compression
+gzip compressed data, was "ramanspy-0.2.9.tar", last modified: Sun Apr  7 09:13:58 2024, max compression
```

## Comparing `ramanspy-0.2.8.tar` & `ramanspy-0.2.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.676329 ramanspy-0.2.8/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.2.8/LICENSE
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       88 2023-09-28 13:11:06.000000 ramanspy-0.2.8/MANIFEST.in
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5698 2024-03-15 10:30:19.676142 ramanspy-0.2.8/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2909 2023-10-02 06:49:44.000000 ramanspy-0.2.8/README.md
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1209 2023-12-18 14:08:53.000000 ramanspy-0.2.8/pyproject.toml
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2024-03-15 10:30:19.676393 ramanspy-0.2.8/setup.cfg
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.668582 ramanspy-0.2.8/src/
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.670971 ramanspy-0.2.8/src/ramanspy/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      503 2023-09-28 11:40:17.000000 ramanspy-0.2.8/src/ramanspy/__init__.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.672862 ramanspy-0.2.8/src/ramanspy/analysis/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/analysis/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/analysis/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/analysis/cluster.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2284 2023-07-04 16:22:48.000000 ramanspy-0.2.8/src/ramanspy/analysis/decompose.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7553 2023-07-04 18:23:45.000000 ramanspy-0.2.8/src/ramanspy/analysis/unmix.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    12290 2024-03-15 10:18:25.000000 ramanspy-0.2.8/src/ramanspy/core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18768 2023-12-06 12:00:24.000000 ramanspy-0.2.8/src/ramanspy/datasets.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     9227 2024-03-15 10:12:12.000000 ramanspy-0.2.8/src/ramanspy/load.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/metrics.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.673395 ramanspy-0.2.8/src/ramanspy/plot/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/plot/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/plot/_core.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/plot/plot.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.674981 ramanspy-0.2.8/src/ramanspy/preprocessing/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/Pipeline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/Step.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    16856 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/baseline.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4143 2023-12-06 13:32:21.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/denoise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/despike.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2149 2023-12-06 13:32:21.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/misc.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/normalise.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5764 2023-12-06 13:49:06.000000 ramanspy-0.2.8/src/ramanspy/preprocessing/protocols.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.675494 ramanspy-0.2.8/src/ramanspy/synth/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      203 2023-09-29 13:28:14.000000 ramanspy-0.2.8/src/ramanspy/synth/__init__.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    11637 2023-09-29 16:47:37.000000 ramanspy-0.2.8/src/ramanspy/synth/synth.py
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      465 2023-06-26 22:05:02.000000 ramanspy-0.2.8/src/ramanspy/utils.py
-drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-03-15 10:30:19.675896 ramanspy-0.2.8/src/ramanspy.egg-info/
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5698 2024-03-15 10:30:19.000000 ramanspy-0.2.8/src/ramanspy.egg-info/PKG-INFO
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1009 2024-03-15 10:30:19.000000 ramanspy-0.2.8/src/ramanspy.egg-info/SOURCES.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2024-03-15 10:30:19.000000 ramanspy-0.2.8/src/ramanspy.egg-info/dependency_links.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2024-03-15 10:30:19.000000 ramanspy-0.2.8/src/ramanspy.egg-info/requires.txt
--rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2024-03-15 10:30:19.000000 ramanspy-0.2.8/src/ramanspy.egg-info/top_level.txt
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.891000 ramanspy-0.2.9/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1503 2023-06-26 11:18:57.000000 ramanspy-0.2.9/LICENSE
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       88 2023-09-28 13:11:06.000000 ramanspy-0.2.9/MANIFEST.in
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5698 2024-04-07 09:13:58.890832 ramanspy-0.2.9/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2909 2023-10-02 06:49:44.000000 ramanspy-0.2.9/README.md
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1209 2024-04-07 08:32:41.000000 ramanspy-0.2.9/pyproject.toml
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       38 2024-04-07 09:13:58.891037 ramanspy-0.2.9/setup.cfg
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.882254 ramanspy-0.2.9/src/
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.884782 ramanspy-0.2.9/src/ramanspy/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      503 2023-09-28 11:40:17.000000 ramanspy-0.2.9/src/ramanspy/__init__.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.887865 ramanspy-0.2.9/src/ramanspy/analysis/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3187 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/analysis/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       85 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/analysis/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1035 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/analysis/cluster.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2284 2023-07-04 16:22:48.000000 ramanspy-0.2.9/src/ramanspy/analysis/decompose.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7553 2023-07-04 18:23:45.000000 ramanspy-0.2.9/src/ramanspy/analysis/unmix.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    12290 2024-03-15 10:18:25.000000 ramanspy-0.2.9/src/ramanspy/core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    18768 2023-12-06 12:00:24.000000 ramanspy-0.2.9/src/ramanspy/datasets.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     9227 2024-03-15 10:12:12.000000 ramanspy-0.2.9/src/ramanspy/load.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4974 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/metrics.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.888369 ramanspy-0.2.9/src/ramanspy/plot/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      196 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/plot/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     7777 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/plot/_core.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    25767 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/plot/plot.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.889948 ramanspy-0.2.9/src/ramanspy/preprocessing/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5493 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/Pipeline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4862 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/Step.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      262 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    17160 2024-04-07 08:46:49.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/baseline.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     4143 2023-12-06 13:32:21.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/denoise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2370 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/despike.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     2149 2023-12-06 13:32:21.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/misc.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     3573 2023-06-26 11:18:57.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/normalise.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5764 2023-12-06 13:49:06.000000 ramanspy-0.2.9/src/ramanspy/preprocessing/protocols.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.890375 ramanspy-0.2.9/src/ramanspy/synth/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      203 2023-09-29 13:28:14.000000 ramanspy-0.2.9/src/ramanspy/synth/__init__.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)    12723 2024-04-02 20:05:46.000000 ramanspy-0.2.9/src/ramanspy/synth/synth.py
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)      465 2023-06-26 22:05:02.000000 ramanspy-0.2.9/src/ramanspy/utils.py
+drwxr-xr-x   0 dimitargeorgiev   (501) staff       (20)        0 2024-04-07 09:13:58.890632 ramanspy-0.2.9/src/ramanspy.egg-info/
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     5698 2024-04-07 09:13:58.000000 ramanspy-0.2.9/src/ramanspy.egg-info/PKG-INFO
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)     1009 2024-04-07 09:13:58.000000 ramanspy-0.2.9/src/ramanspy.egg-info/SOURCES.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        1 2024-04-07 09:13:58.000000 ramanspy-0.2.9/src/ramanspy.egg-info/dependency_links.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)       90 2024-04-07 09:13:58.000000 ramanspy-0.2.9/src/ramanspy.egg-info/requires.txt
+-rw-r--r--   0 dimitargeorgiev   (501) staff       (20)        9 2024-04-07 09:13:58.000000 ramanspy-0.2.9/src/ramanspy.egg-info/top_level.txt
```

### Comparing `ramanspy-0.2.8/LICENSE` & `ramanspy-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/PKG-INFO` & `ramanspy-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.2.8
+Version: 0.2.9
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ramanspy-0.2.8/README.md` & `ramanspy-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/pyproject.toml` & `ramanspy-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ramanspy"
-version = "0.2.8"
+version = "0.2.9"
 description = "RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis"
 readme = "README.md"
 authors = [{ name = "Dimitar Georgiev", email = "d.georgiev21@imperial.ac.uk" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
```

### Comparing `ramanspy-0.2.8/src/ramanspy/analysis/Step.py` & `ramanspy-0.2.9/src/ramanspy/analysis/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/analysis/cluster.py` & `ramanspy-0.2.9/src/ramanspy/analysis/cluster.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/analysis/decompose.py` & `ramanspy-0.2.9/src/ramanspy/analysis/decompose.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/analysis/unmix.py` & `ramanspy-0.2.9/src/ramanspy/analysis/unmix.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/core.py` & `ramanspy-0.2.9/src/ramanspy/core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/datasets.py` & `ramanspy-0.2.9/src/ramanspy/datasets.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/load.py` & `ramanspy-0.2.9/src/ramanspy/load.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/metrics.py` & `ramanspy-0.2.9/src/ramanspy/metrics.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/plot/_core.py` & `ramanspy-0.2.9/src/ramanspy/plot/_core.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/plot/plot.py` & `ramanspy-0.2.9/src/ramanspy/plot/plot.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/Pipeline.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/Pipeline.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/Step.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/Step.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/baseline.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/baseline.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,14 +286,19 @@
     Parameters
     ----------
     **kwargs :
         Check original `implementation <https://pybaselines.readthedocs.io/en/latest/api/pybaselines/api/index.html#pybaselines.polynomial.penalized_poly>`_ for information about parameters.
 
 
     .. note :: Implementation based on `pybaselines <https://pybaselines.readthedocs.io>`_.
+
+
+    References
+    ----------
+    Mazet, V., et al. Background removal from spectra by designing and minimising a non-quadratic cost function. Chemometrics and Intelligent Laboratory Systems, 2005, 76(2), 121-133.
     """
     def __init__(self, *, poly_order=2, tol=0.001, max_iter=250, weights=None, cost_function='asymmetric_truncated_quadratic', threshold=None, alpha_factor=0.99):
         super().__init__(pybaselines.polynomial.penalized_poly, poly_order=poly_order, tol=tol, max_iter=max_iter, weights=weights, cost_function=cost_function, threshold=threshold, alpha_factor=alpha_factor)
 
 
 class IModPoly(PybaselinesCorrector):
     """
@@ -390,11 +395,11 @@
 
 
     .. note :: Implementation based on `pybaselines <https://pybaselines.readthedocs.io>`_.
 
 
     References
     ----------
-    Liu, Y.J., et al. A Concise Iterative Method with Bezier Technique for Baseline Construction. Analyst, 2015, 140(23), 7984-7996.
+    Cobas, J.C., Bernstein, M.A., Martín-Pastor, M. and Tahoces, P.G., 2006. A new general-purpose fully automatic baseline-correction procedure for 1D and 2D NMR data. Journal of Magnetic Resonance, 183(1), pp.145-151.
     """
     def __init__(self, *, lam=1000000.0, scale=None, num_std=3.0, diff_order=2, min_length=2, weights=None, weights_as_mask=False, x_data=None, **pad_kwargs):
         super().__init__(pybaselines.classification.fabc, lam=lam, scale=scale, num_std=num_std, diff_order=diff_order, min_length=min_length, weights=weights, weights_as_mask=weights_as_mask, x_data=x_data, **pad_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/denoise.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/denoise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/despike.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/despike.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/misc.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/misc.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/normalise.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/normalise.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/preprocessing/protocols.py` & `ramanspy-0.2.9/src/ramanspy/preprocessing/protocols.py`

 * *Files identical despite different names*

### Comparing `ramanspy-0.2.8/src/ramanspy/synth/synth.py` & `ramanspy-0.2.9/src/ramanspy/synth/synth.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,14 +60,18 @@
 
         # Generate synthetic spectra
         spectra = rp.synth.generate_spectra(5, 100, realistic=True)
 
         rp.plot.spectra(spectra)
         rp.plot.show()
 
+
+    References
+    ----------
+    Georgiev, D., Fernández-Galiana, A., Pedersen, S.V., Papadopoulos, G., Xie, R., Stevens, M.M. and Barahona, M., 2024. Hyperspectral unmixing for Raman spectroscopy via physics-constrained autoencoders. arXiv preprint arXiv:2403.04526.
     """
     if spectral_axis is not None:
         assert len(spectral_axis) == n_bands, 'The spectral axis should match the number of bands.'
     else:
         spectral_axis = np.arange(n_bands)
 
     np.random.seed(seed)
@@ -140,14 +144,19 @@
     seed : int, optional
         The seed to use for the random number generator.
 
     Returns
     -------
     mixtures : array_like
         The mixed spectra.
+
+
+    References
+    ----------
+    Georgiev, D., Fernández-Galiana, A., Pedersen, S.V., Papadopoulos, G., Xie, R., Stevens, M.M. and Barahona, M., 2024. Hyperspectral unmixing for Raman spectroscopy via physics-constrained autoencoders. arXiv preprint arXiv:2403.04526.
     """
     spectral_axis = endmembers[0].spectral_axis
 
     endmembers = np.array([endmember.spectral_data for endmember in endmembers])
     assert abundances.shape[-1] == endmembers.shape[
         0], 'The number of endmembers and the number of abundance maps must match.'
 
@@ -210,14 +219,19 @@
     seed : int, optional
         The seed to use for the random number generator.
 
     Returns
     -------
     image : array_like, shape (size, size, num_endmembers)
         The generated abundance image.
+
+
+    References
+    ----------
+    Georgiev, D., Fernández-Galiana, A., Pedersen, S.V., Papadopoulos, G., Xie, R., Stevens, M.M. and Barahona, M., 2024. Hyperspectral unmixing for Raman spectroscopy via physics-constrained autoencoders. arXiv preprint arXiv:2403.04526.
     """
     assert scene_type in SCENES, 'The mode must be one of {}'.format(SCENES)
 
     np.random.seed(seed)
 
     image = np.zeros((size, size, num_endmembers))
 
@@ -319,14 +333,18 @@
     .. code::
 
         import ramanspy as rp
 
         # Generate synthetic data
         mixture, endmebers, abundance_image = rp.synth.generate_image_dataset(5, 1000, 100, 'chessboard', mixture_mode='linear')
 
+
+    References
+    ----------
+    Georgiev, D., Fernández-Galiana, A., Pedersen, S.V., Papadopoulos, G., Xie, R., Stevens, M.M. and Barahona, M., 2024. Hyperspectral unmixing for Raman spectroscopy via physics-constrained autoencoders. arXiv preprint arXiv:2403.04526.
     """
 
     endmebers = generate_spectra(num_endmembers, num_spectral_bands, realistic=realistic_endmembers, seed=seed)
     abundance_image = generate_abundance_scene(image_size, num_endmembers, image_type, seed=seed)
 
     mixture = mix(endmebers, abundance_image, mixture_mode=mixture_mode, noise=noise, noise_amplitude=noise_amplitude,
                   baseline=baseline, baseline_amplitude=baseline_amplitude, baseline_probability=baseline_probability,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ramanspy-0.2.8/src/ramanspy.egg-info/PKG-INFO` & `ramanspy-0.2.9/src/ramanspy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ramanspy
-Version: 0.2.8
+Version: 0.2.9
 Summary: RamanSPy: An open-source Python package for integrative Raman spectroscopy data analysis
 Author-email: Dimitar Georgiev <d.georgiev21@imperial.ac.uk>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Dimitar Georgiev
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `ramanspy-0.2.8/src/ramanspy.egg-info/SOURCES.txt` & `ramanspy-0.2.9/src/ramanspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

