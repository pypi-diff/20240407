# Comparing `tmp/feature-eval-0.0.13.tar.gz` & `tmp/feature-eval-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature-eval-0.0.13.tar", last modified: Sun Apr  7 14:52:53 2024, max compression
+gzip compressed data, was "C:\workspace\feature-eval\dist\.tmp-bgszl8i4\feature-eval-0.0.7.tar", last modified: Mon Oct  2 07:39:52 2023, max compression
```

## Comparing `feature-eval-0.0.13.tar` & `feature-eval-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 14:52:53.726152 feature-eval-0.0.13/
--rw-rw-rw-   0        0        0     1087 2023-09-29 02:02:52.000000 feature-eval-0.0.13/LICENSE
--rw-rw-rw-   0        0        0     3787 2024-04-07 14:52:53.724157 feature-eval-0.0.13/PKG-INFO
--rw-rw-rw-   0        0        0     3110 2023-10-14 14:26:32.000000 feature-eval-0.0.13/README.md
--rw-rw-rw-   0        0        0      747 2024-04-07 14:52:13.000000 feature-eval-0.0.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 14:52:53.726152 feature-eval-0.0.13/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-07 14:52:53.688115 feature-eval-0.0.13/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 14:52:53.723159 feature-eval-0.0.13/src/feature_eval.egg-info/
--rw-rw-rw-   0        0        0     3787 2024-04-07 14:52:53.000000 feature-eval-0.0.13/src/feature_eval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-04-07 14:52:53.000000 feature-eval-0.0.13/src/feature_eval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 14:52:53.000000 feature-eval-0.0.13/src/feature_eval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 14:52:53.000000 feature-eval-0.0.13/src/feature_eval.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-07 14:52:53.721165 feature-eval-0.0.13/src/featureval/
--rw-rw-rw-   0        0        0      970 2023-10-12 09:12:02.000000 feature-eval-0.0.13/src/featureval/__init__.py
--rw-rw-rw-   0        0        0    13529 2024-04-07 14:51:16.000000 feature-eval-0.0.13/src/featureval/binning.py
--rw-rw-rw-   0        0        0     1313 2024-04-07 08:42:34.000000 feature-eval-0.0.13/src/featureval/metrics.py
--rw-rw-rw-   0        0        0     2234 2023-10-04 11:11:18.000000 feature-eval-0.0.13/src/featureval/preprocess.py
--rw-rw-rw-   0        0        0     4579 2024-04-07 08:55:42.000000 feature-eval-0.0.13/src/featureval/redrel.py
--rw-rw-rw-   0        0        0     4761 2023-10-04 11:11:18.000000 feature-eval-0.0.13/src/featureval/selection.py
+drwxrwxrwx   0        0        0        0 2023-10-02 07:39:52.000000 feature-eval-0.0.7/
+-rw-rw-rw-   0        0        0     1087 2023-09-30 10:21:06.000000 feature-eval-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1853 2023-10-02 07:39:52.000000 feature-eval-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-10-01 09:19:42.000000 feature-eval-0.0.7/README.md
+-rw-rw-rw-   0        0        0      652 2023-10-02 07:38:49.000000 feature-eval-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-10-02 07:39:52.000000 feature-eval-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-10-02 07:39:52.000000 feature-eval-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-10-02 07:39:52.000000 feature-eval-0.0.7/src/feature_eval.egg-info/
+-rw-rw-rw-   0        0        0     1853 2023-10-02 07:39:52.000000 feature-eval-0.0.7/src/feature_eval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-10-02 07:39:52.000000 feature-eval-0.0.7/src/feature_eval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-10-02 07:39:52.000000 feature-eval-0.0.7/src/feature_eval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-10-02 07:39:52.000000 feature-eval-0.0.7/src/feature_eval.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-10-02 07:39:52.000000 feature-eval-0.0.7/src/featureval/
+-rw-rw-rw-   0        0        0      904 2023-10-02 07:36:47.000000 feature-eval-0.0.7/src/featureval/__init__.py
+-rw-rw-rw-   0        0        0     1554 2023-10-02 07:26:45.000000 feature-eval-0.0.7/src/featureval/metrics.py
+-rw-rw-rw-   0        0        0      605 2023-10-02 06:44:07.000000 feature-eval-0.0.7/src/featureval/preprocess.py
+-rw-rw-rw-   0        0        0     4490 2023-10-01 09:16:45.000000 feature-eval-0.0.7/src/featureval/redrel.py
+-rw-rw-rw-   0        0        0     3809 2023-10-02 07:26:31.000000 feature-eval-0.0.7/src/featureval/selection.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `feature-eval-0.0.13/LICENSE` & `feature-eval-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `feature-eval-0.0.13/pyproject.toml` & `feature-eval-0.0.7/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feature-eval"
-version = "0.0.13"
+version = "0.0.7"
 authors = [
   { name="Jingxiao Zhang", email="rex.zhang2016@foxmail.com" },
 ]
 description = "A user-friendly feature evaluation and selection package."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/rexzhang2014/feature-eval"
-"Bug Tracker" = "https://github.com/rexzhang2014/feature-eval/issues"
-"Example Code" = "https://github.com/rexzhang2014/feature-eval/blob/master/tests/example.py"
+"Bug Tracker" = "https://github.com/rexzhang2014/feature-eval/issues"
```

### Comparing `feature-eval-0.0.13/src/featureval/__init__.py` & `feature-eval-0.0.7/src/featureval/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,18 +24,15 @@
 from featureval.selection import (
     mRMR # Only provide this default algorithm for convinience.
 )
 
 from featureval.preprocess import(
     categories_to_integer,
     zscore_normalize,
-    detect_variable_type,
-    weight_of_evidence,
 )
 
 from featureval import (
-    binning,
     metrics,
     preprocess,
     selection,
     redrel
 )
```

### Comparing `feature-eval-0.0.13/src/featureval/metrics.py` & `feature-eval-0.0.7/src/featureval/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import pandas as pd
 import numpy as np
 
 from scipy.stats import entropy
-from featureval.preprocess import get_woe_df
 
 def info_value(x, y, bins=20) : 
-    '''
-    This is called IV
-    '''
-    x, y = np.asarray(x), np.asarray(y)
-    xbins = pd.qcut(x, bins, duplicates='drop')
+    xbins = pd.qcut(x, 20, duplicates='drop')
 
+    df = np.concatenate(
+        [x.reshape(len(x),1), y.reshape(len(y),1), xbins.reshape(len(xbins),1)],
+        axis=1,
+    )
+    df = pd.DataFrame(df, columns=['x', 'y', 'xbins'])
+    
+    df = df.groupby('xbins').agg({'y': [sum, lambda x: len(x)-sum(x)]}).astype(float)
+    df.columns = ['cnt1', 'cnt0']
+    
     N1 = (y==1).sum()
     N0 = y.shape[0] - N1
-        
-    df = get_woe_df(x, y, xbins)
+    df = df.assign(
+        woe = np.log(df['cnt1'] / N1) - np.log(df['cnt0'] / N0)
+    )
 
     iv = ((df['cnt1'] / N1 - df['cnt0'] / N0) * df['woe']).sum()
     
     return iv
 
 def corr_coef(x, y) :
     return ((x-x.mean()) * (y-y.mean())).mean() / (x.std() * y.std())
```

### Comparing `feature-eval-0.0.13/src/featureval/redrel.py` & `feature-eval-0.0.7/src/featureval/redrel.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,16 @@
         return self.pairwise
     
     def _calc(self, agg_method='mean') :
         
         pairwise = self._calc_pairwise()
         
         if isinstance(agg_method, str) :
-            agg_method1 = eval('np.'+agg_method)
-            # pairwise calc, scaled.
-            agg_method = lambda x : agg_method1(x) / len(x) 
-
+            agg_method = eval('np.'+agg_method)
+            
         fsetwise = pairwise.groupby('y')[self.name].agg(agg_method)
         
         self.redundancy = fsetwise.reset_index()
         return self.redundancy
 
 class PearsonCorrelation(Relevance) :
```

