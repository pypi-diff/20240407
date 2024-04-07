# Comparing `tmp/many-0.7.0.tar.gz` & `tmp/many-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "many-0.7.0.tar", max compression
+gzip compressed data, was "many-0.7.1.tar", max compression
```

## Comparing `many-0.7.0.tar` & `many-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1065 2020-07-31 23:16:16.000000 many-0.7.0/LICENSE
--rw-r--r--   0        0        0     2388 2020-09-29 03:52:53.000000 many-0.7.0/README.md
--rw-r--r--   0        0        0       52 2020-08-24 20:21:51.000000 many-0.7.0/many/__init__.py
--rw-r--r--   0        0        0      499 2020-11-20 20:32:45.000000 many-0.7.0/many/stats/__init__.py
--rw-r--r--   0        0        0     9712 2020-11-21 01:21:01.000000 many-0.7.0/many/stats/categorical_categorical.py
--rw-r--r--   0        0        0       59 2020-08-13 18:21:10.000000 many-0.7.0/many/stats/config.py
--rw-r--r--   0        0        0    16108 2021-08-25 17:03:51.764519 many-0.7.0/many/stats/continuous_categorical.py
--rw-r--r--   0        0        0    15312 2021-01-17 01:50:34.529344 many-0.7.0/many/stats/continuous_continuous.py
--rw-r--r--   0        0        0    14184 2020-11-16 21:31:48.000000 many-0.7.0/many/stats/continuous_continuous_cmap.py
--rw-r--r--   0        0        0    11048 2020-11-16 21:31:48.000000 many-0.7.0/many/stats/fisher.py
--rw-r--r--   0        0        0     1307 2020-08-23 22:33:36.000000 many-0.7.0/many/stats/utils.py
--rw-r--r--   0        0        0      327 2020-08-27 04:46:22.000000 many-0.7.0/many/visuals/__init__.py
--rw-r--r--   0        0        0     1928 2021-01-17 01:50:34.349048 many-0.7.0/many/visuals/categorical_categorical.py
--rw-r--r--   0        0        0    13457 2021-01-17 01:50:34.525521 many-0.7.0/many/visuals/continuous_categorical.py
--rw-r--r--   0        0        0    10518 2021-01-17 01:50:34.496365 many-0.7.0/many/visuals/continuous_continuous.py
--rw-r--r--   0        0        0     1205 2020-08-23 22:33:36.000000 many-0.7.0/many/visuals/utils.py
--rw-r--r--   0        0        0     1003 2024-04-07 17:04:15.865676 many-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 many-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2020-07-31 23:16:16.000000 many-0.7.1/LICENSE
+-rw-r--r--   0        0        0     2388 2020-09-29 03:52:53.000000 many-0.7.1/README.md
+-rw-r--r--   0        0        0       52 2020-08-24 20:21:51.000000 many-0.7.1/many/__init__.py
+-rw-r--r--   0        0        0      499 2020-11-20 20:32:45.000000 many-0.7.1/many/stats/__init__.py
+-rw-r--r--   0        0        0     9712 2020-11-21 01:21:01.000000 many-0.7.1/many/stats/categorical_categorical.py
+-rw-r--r--   0        0        0       59 2020-08-13 18:21:10.000000 many-0.7.1/many/stats/config.py
+-rw-r--r--   0        0        0    16108 2021-08-25 17:03:51.764519 many-0.7.1/many/stats/continuous_categorical.py
+-rw-r--r--   0        0        0    15076 2024-04-07 17:37:06.529886 many-0.7.1/many/stats/continuous_continuous.py
+-rw-r--r--   0        0        0    14184 2020-11-16 21:31:48.000000 many-0.7.1/many/stats/continuous_continuous_cmap.py
+-rw-r--r--   0        0        0    11048 2020-11-16 21:31:48.000000 many-0.7.1/many/stats/fisher.py
+-rw-r--r--   0        0        0     1307 2020-08-23 22:33:36.000000 many-0.7.1/many/stats/utils.py
+-rw-r--r--   0        0        0      327 2020-08-27 04:46:22.000000 many-0.7.1/many/visuals/__init__.py
+-rw-r--r--   0        0        0     1928 2021-01-17 01:50:34.349048 many-0.7.1/many/visuals/categorical_categorical.py
+-rw-r--r--   0        0        0    13457 2021-01-17 01:50:34.525521 many-0.7.1/many/visuals/continuous_categorical.py
+-rw-r--r--   0        0        0    10518 2021-01-17 01:50:34.496365 many-0.7.1/many/visuals/continuous_continuous.py
+-rw-r--r--   0        0        0     1205 2020-08-23 22:33:36.000000 many-0.7.1/many/visuals/utils.py
+-rw-r--r--   0        0        0     1003 2024-04-07 17:37:19.598340 many-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 many-0.7.1/PKG-INFO
```

### Comparing `many-0.7.0/LICENSE` & `many-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `many-0.7.0/README.md` & `many-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/stats/categorical_categorical.py` & `many-0.7.1/many/stats/categorical_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/stats/continuous_categorical.py` & `many-0.7.1/many/stats/continuous_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/stats/continuous_continuous.py` & `many-0.7.1/many/stats/continuous_continuous.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import sys
-import warnings
 
 import numpy as np
 import pandas as pd
 import scipy.special as special
 from scipy.stats import (
-    PearsonRConstantInputWarning,
-    SpearmanRConstantInputWarning,
     pearsonr,
     spearmanr,
 )
 from statsmodels.stats.multitest import multipletests
 from tqdm import tqdm_notebook as tqdm
 
 from . import config
@@ -100,37 +97,31 @@
     pvals = np.zeros((a_num_cols, b_num_cols))
     sample_counts = np.zeros((a_num_cols, b_num_cols))
 
     if pbar:
         sys.stderr.flush()
         progress = tqdm(total=a_num_cols * b_num_cols)
 
-    warnings.simplefilter("ignore", SpearmanRConstantInputWarning)
-    warnings.simplefilter("ignore", PearsonRConstantInputWarning)
-
     for a_col_idx, a_col_name in enumerate(a_names):
         for b_col_idx, b_col_name in enumerate(b_names):
-
             # select columns to correlate
             a_col = a_mat[a_col_name].dropna()
             b_col = b_mat[b_col_name].dropna()
 
             a_col, b_col = a_col.align(b_col, join="inner", axis=0)
 
             num_samples = len(a_col)
 
             if num_samples > 2:
-
                 if method == "pearson":
                     corr, pval = pearsonr(a_col, b_col)
                 elif method == "spearman":
                     corr, pval = spearmanr(a_col, b_col)
 
             elif num_samples <= 2:
-
                 corr, pval = np.nan, np.nan
 
             # add in correlation
             corrs[a_col_idx][b_col_idx] = corr
             pvals[a_col_idx][b_col_idx] = pval
             sample_counts[a_col_idx][b_col_idx] = num_samples
 
@@ -152,15 +143,14 @@
 
     corrs = corrs.fillna(0)
     pvals = pvals.fillna(1)
 
     pvals = -np.log10(pvals)
 
     if melt:
-
         return melt_corr(corrs, pvals, sample_counts, method)
 
     return corrs, pvals
 
 
 def mat_corr(a_mat, b_mat, melt: bool, method: str):
     """
@@ -205,16 +195,16 @@
     a_mat, b_mat = np.array(a_mat), np.array(b_mat)
 
     # Subtract column means
     residuals_a = a_mat - a_mat.mean(axis=0)
     residuals_b = b_mat - b_mat.mean(axis=0)
 
     # Sum squares across columns
-    sums_a = (residuals_a ** 2).sum(axis=0)
-    sums_b = (residuals_b ** 2).sum(axis=0)
+    sums_a = (residuals_a**2).sum(axis=0)
+    sums_b = (residuals_b**2).sum(axis=0)
 
     # Compute correlations
     residual_products = np.dot(residuals_a.T, residuals_b)
     sum_products = np.sqrt(np.dot(sums_a[:, None], sums_b[None]))
 
     sum_zeros = sum_products == 0
     sum_products[sum_zeros] = 1
@@ -240,15 +230,14 @@
     corrs = pd.DataFrame(corrs, index=a_names, columns=b_names)
     pvals = pd.DataFrame(pvals, index=a_names, columns=b_names)
     sample_counts = pd.DataFrame(num_samples, index=a_names, columns=b_names)
 
     pvals = -np.log10(pvals)
 
     if melt:
-
         return melt_corr(corrs, pvals, sample_counts, method)
 
     return corrs, pvals
 
 
 def pearson_significance(row):
     corr = row["corr"]
@@ -300,15 +289,14 @@
     b_num_cols = len(b_names)
 
     num_samples = len(a_mat.index)  # number of samples
 
     # compute column ranks, as Spearman correlation is equivalent
     # to Pearson correlation between ranks
     if method == "spearman":
-
         b_nan = b_mat.isna()
         b_mat = b_mat.rank(na_option="top", method="average")
         b_mat[b_mat <= b_nan.sum()] = np.nan
         b_mat = b_mat - b_nan.sum()
 
         # construct mirrored A matrix
         b_num_cols = b_mat.shape[1]
@@ -335,16 +323,16 @@
     b_mat = np.ma.array(b_mat, mask=np.isnan(b_mat))
 
     # subtract column means
     residuals_b = b_mat - np.ma.mean(b_mat, axis=0)
     residuals_a_nan = a_nan - np.ma.mean(a_nan, axis=0)
 
     # sum squares across columns
-    sums_b = np.ma.sum(residuals_b ** 2, axis=0)
-    sums_a_nan = np.ma.sum(residuals_a_nan ** 2, axis=0)
+    sums_b = np.ma.sum(residuals_b**2, axis=0)
+    sums_a_nan = np.ma.sum(residuals_a_nan**2, axis=0)
 
     # compute correlations
     residual_products = np.ma.sum(residuals_a_nan * residuals_b, axis=0)
     sum_products = np.sqrt(sums_a_nan * sums_b)
 
     corrs = np.array(residual_products / sum_products).reshape(-1)
 
@@ -378,15 +366,15 @@
     a_mat,
     b_mat,
     subtypes,
     min_count: int,
     stack: bool,
     mat_method,
     pbar=False,
-    **kwargs
+    **kwargs,
 ):
     """
     Compute correlations between a_mat and every column of b_mat, within
     each subsample specified by subtypes. a_mat must be a Series for this
     method to work. Allows for missing values in b_mat.
 
     Parameters
@@ -454,30 +442,26 @@
 
     if pbar:
         sys.stderr.flush()
         progress = tqdm(total=len(unique_subtypes))
 
     # compute correlation within each subtype
     for subtype in unique_subtypes:
-
         subtype_rows = list(subtypes[subtypes == subtype].index)
 
         a_subset = a_mat.loc[subtype_rows]
         b_subset = b_mat.loc[subtype_rows]
 
         if mat_method == "mat_corr_naive":
-
             res = mat_corr_naive(a_subset, b_subset, **kwargs, melt=True)
 
         elif mat_method == "mat_corr_nan":
-
             res = mat_corr_nan(a_subset, b_subset, **kwargs, melt=True)
 
         else:
-
             error = "mat_method must be 'mat_corr_naive' or 'mat_corr_nan'"
 
             raise ValueError(error)
 
         # rename columns for merging
         res.columns = [subtype + "_" + x for x in res.columns]
```

### Comparing `many-0.7.0/many/stats/continuous_continuous_cmap.py` & `many-0.7.1/many/stats/continuous_continuous_cmap.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/stats/fisher.py` & `many-0.7.1/many/stats/fisher.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/stats/utils.py` & `many-0.7.1/many/stats/utils.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/visuals/categorical_categorical.py` & `many-0.7.1/many/visuals/categorical_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/visuals/continuous_categorical.py` & `many-0.7.1/many/visuals/continuous_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/visuals/continuous_continuous.py` & `many-0.7.1/many/visuals/continuous_continuous.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/many/visuals/utils.py` & `many-0.7.1/many/visuals/utils.py`

 * *Files identical despite different names*

### Comparing `many-0.7.0/pyproject.toml` & `many-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "many"
-version = "0.7.0"
+version = "0.7.1"
 description = "Statistical methods for computing many correlations"
 authors = ["Kevin Hu <kevinhuwest@gmail.com>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kevinhu/many"
 repository = "https://github.com/kevinhu/many"
```

### Comparing `many-0.7.0/PKG-INFO` & `many-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: many
-Version: 0.7.0
+Version: 0.7.1
 Summary: Statistical methods for computing many correlations
 Home-page: https://github.com/kevinhu/many
 License: MIT
 Author: Kevin Hu
 Author-email: kevinhuwest@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

