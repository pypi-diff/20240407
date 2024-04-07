# Comparing `tmp/scbsp-0.2.3.tar.gz` & `tmp/scbsp-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scbsp-0.2.3.tar", last modified: Thu Mar  7 04:39:05 2024, max compression
+gzip compressed data, was "scbsp-0.2.4.tar", last modified: Sun Apr  7 08:56:29 2024, max compression
```

## Comparing `scbsp-0.2.3.tar` & `scbsp-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:39:05.119252 scbsp-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-07 04:39:01.000000 scbsp-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-07 04:39:05.119252 scbsp-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-03-07 04:39:01.000000 scbsp-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:39:05.119252 scbsp-0.2.3/scbsp/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-07 04:39:01.000000 scbsp-0.2.3/scbsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-03-07 04:39:01.000000 scbsp-0.2.3/scbsp/scbsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:39:05.119252 scbsp-0.2.3/scbsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-03-07 04:39:05.000000 scbsp-0.2.3/scbsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-07 04:39:05.000000 scbsp-0.2.3/scbsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 04:39:05.000000 scbsp-0.2.3/scbsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-07 04:39:05.000000 scbsp-0.2.3/scbsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-07 04:39:05.000000 scbsp-0.2.3/scbsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 04:39:05.119252 scbsp-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-07 04:39:03.000000 scbsp-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 04:39:05.119252 scbsp-0.2.3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5483 2024-03-07 04:39:01.000000 scbsp-0.2.3/test/test_scbsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:56:29.331592 scbsp-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 08:56:26.000000 scbsp-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-07 08:56:29.331592 scbsp-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-07 08:56:26.000000 scbsp-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:56:29.331592 scbsp-0.2.4/scbsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-07 08:56:26.000000 scbsp-0.2.4/scbsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8657 2024-04-07 08:56:26.000000 scbsp-0.2.4/scbsp/scbsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:56:29.331592 scbsp-0.2.4/scbsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-07 08:56:29.000000 scbsp-0.2.4/scbsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-07 08:56:29.000000 scbsp-0.2.4/scbsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:56:29.000000 scbsp-0.2.4/scbsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-07 08:56:29.000000 scbsp-0.2.4/scbsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 08:56:29.000000 scbsp-0.2.4/scbsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:56:29.331592 scbsp-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-07 08:56:28.000000 scbsp-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:56:29.331592 scbsp-0.2.4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     5250 2024-04-07 08:56:26.000000 scbsp-0.2.4/test/test_scbsp.py
```

### Comparing `scbsp-0.2.3/LICENSE` & `scbsp-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scbsp-0.2.3/PKG-INFO` & `scbsp-0.2.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,67 @@
-Metadata-Version: 2.1
-Name: scbsp
-Version: 0.2.3
-Summary: A package that efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data
-Home-page: https://github.com/YQ-Wang/scBSP
-Author: Yiqing Wang, Jinpu Li
-Author-email: yqw@wangemail.com, lijinp@health.missouri.edu
-License: GPLv3
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
+# scBSP
 
-\n# scBSP
-
-scBSP is a specialized package designed for processing biological data, specifically in the analysis of gene expression and cell coordinates. It efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data.
+scBSP is a dedicated software package crafted for the nuanced domain of biological data processing, emphasizing gene expression analysis and cell coordinate evaluation. It offers a streamlined method to calculate p-values for a set of genes by leveraging input matrices that encapsulate cell coordinates and gene expression data.
 
 ## Installation
 
 ### Dependencies
-scBSP requires:
+To ensure scBSP functions optimally, the following dependencies are required:
 - Python (>= 3.8)
 - NumPy (>= 1.24.4)
 - Pandas (>= 1.3.5)
 - SciPy (>= 1.10.1)
+- scikit-learn (>=1.3.2)
+
+For enhanced scBSP using HNSW for distance calculation:
 - hnswlib (>= 0.8.0)
 
-To install scBSP, run the following command:
+### Installation Commands
+For Standard Installation (Using Ball Tree):
 
 `pip install scbsp`
 
+For Installation with HNSW (Hierarchical Navigable Small World Graphs):
+
+`pip install scbsp[hnsw]`
+
 ## Usage
 
 To use scBSP, you need to provide two primary inputs:
 
 1. **Cell Coordinates Matrix (`input_sp_mat`)**: 
    - Format: Numpy array.
    - Dimensions: N x D, where N is the number of cells and D is the dimension of coordinates.
 
 2. **Gene Expression Matrix (`input_exp_mat_raw`)**:
    - Format: Numpy array, Pandas DataFrame, or CSR matrix.
    - Dimensions: N x P, where N is the number of cells and P is the number of genes.
 
-Additionally, you must specify the following parameters:
+Additional parameters to specify include:
 
-- `d1`: A floating-point number.
-- `d2`: A floating-point number.
+- `d1`: A floating-point number. Default value is 1.0.
+- `d2`: A floating-point number. Default value is 3.0.
+- `leaf_size`: Optional integer defining the maximum point threshold for the Ball Tree algorithm to revert to brute-force search (default = 80). Not required for installations using HNSW.
 
 
 ### Example
 
-Here's a simple example to demonstrate how to compute p-values using scBSP:
+Below is a straightforward example showcasing how to compute p-values with scBSP:
 
 ```python
 import scbsp
 
 # Load your data into these variables
 input_sp_mat = ...  # Cell Coordinates Matrix
 input_exp_mat_raw = ...  # Gene Expression Matrix
 
 # Set the optional parameters
-d1 = 1.0  # Example value
-d2 = 3.0  # Example value
+d1 = 1.0
+d2 = 3.0
 
-# Execute the calculation
+# Compute p-values
 p_values = scbsp.granp(input_sp_mat, input_exp_mat_raw, d1, d2)
 ```
 
 ## Output
 
 The function returns a list of p-values, each corresponding to the genes in the provided gene expression matrix. These p-values help in identifying significant differences in gene expression across different cell coordinates, facilitating advanced biological data analysis.
-
-
```

### Comparing `scbsp-0.2.3/scbsp/scbsp.py` & `scbsp-0.2.4/scbsp/scbsp.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,20 +5,28 @@
 big-small patch (scBSP), implementing sparse matrix operation and HNSW method
 for distance calculation, for the identification of spatially variable genes
 on large-scale data.
 """
 
 from typing import List, Tuple, Union
 
-import hnswlib
 import numpy as np
 import pandas as pd  # type: ignore
 from scipy.sparse import csr_matrix, diags, identity, isspmatrix_csr  # type: ignore
 from scipy.stats import gmean, lognorm
 
+try:
+    import hnswlib
+
+    use_hnsw = True
+except ImportError:
+    from sklearn.neighbors import BallTree
+
+    use_hnsw = False
+
 
 def _scale_sparse_matrix(input_exp_mat: csr_matrix) -> csr_matrix:
     """
     Scales a sparse matrix such that each row is divided by its maximum value.
 
     Args:
         input_exp_mat: A csr_matrix representing the input expression matrix.
@@ -47,37 +55,46 @@
     data_scaled = data / np.repeat(row_max, row_indices)
     scaled_matrix = csr_matrix((data_scaled, (rows, cols)), shape=input_exp_mat.shape)
 
     return scaled_matrix
 
 
 def _binary_distance_matrix_threshold(
-    labels: np.ndarray,
-    distances: np.ndarray,
-    input_sparse_mat_array: np.ndarray,
-    d_val: float,
+    input_sparse_mat_array: np.ndarray, d_val: float, leaf_size: int
 ) -> csr_matrix:
     """
     Creates a binary distance matrix where distances below a threshold are marked as 1.
 
     Args:
-        labels: An array of labels for each point.
-        distances: An array of distances between points.
         input_sparse_mat_array: The input sparse matrix array.
         d_val: The distance threshold.
+        leaf_size: An integer that determines the maximum number of points after which the Ball Tree algorithm opts for a brute-force search approach.
 
     Returns:
         A csr_matrix representing the binary distance matrix.
     """
 
-    within_d_val = distances <= d_val
-    rows = np.repeat(np.arange(labels.shape[0]), labels.shape[1])[
-        within_d_val.flatten()
-    ]
-    cols = labels.flatten()[within_d_val.flatten()]
+    if use_hnsw is True:
+        labels, distances = _query_hnsw_index(input_sparse_mat_array)
+        within_d_val = distances <= d_val**2
+        rows = np.repeat(np.arange(labels.shape[0]), labels.shape[1])[
+            within_d_val.flatten()
+        ]
+        cols = labels.flatten()[within_d_val.flatten()]
+    else:
+        ball_tree = BallTree(input_sparse_mat_array, leaf_size=leaf_size)
+        indices = ball_tree.query_radius(
+            input_sparse_mat_array, r=d_val, return_distance=False
+        )
+        rows = np.repeat(
+            np.arange(input_sparse_mat_array.shape[0]), [len(i) for i in indices]
+        )
+        cols = np.concatenate(indices)
+
+    # Construct binary csr_matrix
     data = np.ones_like(rows)
 
     sparse_mat = csr_matrix(
         (data, (rows, cols)),
         shape=(input_sparse_mat_array.shape[0], input_sparse_mat_array.shape[0]),
     )
     sparse_mat += identity(input_sparse_mat_array.shape[0], format="csr", dtype=bool)
@@ -122,80 +139,85 @@
         input_sp_mat, k=min(80, input_sp_mat.shape[0])
     )
 
     return labels, distances
 
 
 def _get_test_scores(
-    input_sp_mat: np.ndarray, input_exp_mat_raw: csr_matrix, d1: float, d2: float
+    input_sp_mat: np.ndarray,
+    input_exp_mat_raw: csr_matrix,
+    d1: float,
+    d2: float,
+    leaf_size: int,
 ) -> List[float]:
     """
     Calculates test scores for genomic data based on input sparse matrices and distance thresholds.
 
     Args:
         input_sp_mat: The input spatial matrix as a numpy array.
         input_exp_mat_raw: The raw expression matrix in csr_matrix format.
         d1: Distance threshold 1.
         d2: Distance threshold 2.
+        leaf_size: An integer that determines the maximum number of points after which the Ball Tree algorithm opts for a brute-force search approach.
 
     Returns:
         A list of test scores.
     """
 
     input_exp_mat_norm = _scale_sparse_matrix(input_exp_mat_raw).transpose()
     input_exp_mat_raw = input_exp_mat_raw.transpose()
 
     def _get_inverted_diag_matrix(sum_axis_0: np.ndarray) -> csr_matrix:
         with np.errstate(divide="ignore", invalid="ignore"):
             diag_data = np.reciprocal(sum_axis_0, where=sum_axis_0 != 0)
         return diags(diag_data, offsets=0, format="csr")
 
     def _var_local_means(
-        labels: np.ndarray,
-        distances: np.ndarray,
         input_sp_mat: csr_matrix,
         d_val: float,
         input_exp_mat_norm: csr_matrix,
+        leaf_size: int,
     ) -> List[float]:
         patches_cells = _binary_distance_matrix_threshold(
-            labels, distances, input_sp_mat, d_val**2
+            input_sp_mat, d_val, leaf_size
         )
         patches_cells_centroid = diags(
             (patches_cells.sum(axis=1) > 1).astype(float).A.ravel(),
             offsets=0,
             format="csr",
         )
         patches_cells -= patches_cells_centroid
         sum_axis_0 = patches_cells.sum(axis=0).A.ravel()
         diag_matrix_sparse = _get_inverted_diag_matrix(sum_axis_0)
         x_kj = input_exp_mat_norm.dot(patches_cells.dot(diag_matrix_sparse))
         return _calculate_sparse_variances(x_kj, axis=1)
 
-    labels, distances = _query_hnsw_index(input_sp_mat)
-    var_x = np.column_stack([_var_local_means(labels, distances, input_sp_mat, d_val, input_exp_mat_norm).A.ravel() for d_val in (d1, d2)])  # type: ignore
+    var_x = np.column_stack([_var_local_means(input_sp_mat, d_val, input_exp_mat_norm, leaf_size).A.ravel() for d_val in (d1, d2)])  # type: ignore
     var_x_0_add = _calculate_sparse_variances(input_exp_mat_raw, axis=1).A.ravel()  # type: ignore
     var_x_0_add /= max(var_x_0_add)
     t_matrix = (var_x[:, 1] / var_x[:, 0]) * var_x_0_add
     return t_matrix.tolist()
 
 
 def granp(
     input_sp_mat: np.ndarray,
     input_exp_mat_raw: Union[np.ndarray, pd.DataFrame, csr_matrix],
     d1: float = 1.0,
     d2: float = 3.0,
+    leaf_size: int = 80,
 ) -> List[float]:
     """
     Calculates the p-values for genomic data.
 
     Args:
         input_sp_mat: The input spatial matrix as a numpy array. The dimension is N x D, where N is the number of cells and D is the dimension of coordinates.
         input_exp_mat_raw: The raw expression matrix, which can be a numpy array, pandas DataFrame, or csr_matrix. The dimension is N x P, where N is the number of cells and P is the number of genes.
         d1: Distance threshold 1.
         d2: Distance threshold 2.
+        leaf_size: An integer that determines the maximum number of points after which the Ball Tree algorithm opts for a brute-force search approach.
 
     Returns:
         A list of p-values.
     """
 
     # Scale the distance thresholds according to the geometric mean of data spread.
     scale_factor = (
@@ -209,15 +231,15 @@
     d1 *= scale_factor
     d2 *= scale_factor
 
     # Ensure the expression matrix is in csr_matrix format.
     if not isspmatrix_csr(input_exp_mat_raw):
         input_exp_mat_raw = csr_matrix(input_exp_mat_raw)
 
-    t_matrix_sum = _get_test_scores(input_sp_mat, input_exp_mat_raw, d1, d2)
+    t_matrix_sum = _get_test_scores(input_sp_mat, input_exp_mat_raw, d1, d2, leaf_size)
 
     # Calculate p-values
     t_matrix_sum_upper90 = np.quantile(t_matrix_sum, 0.90)
     t_matrix_sum_mid = [val for val in t_matrix_sum if val < t_matrix_sum_upper90]
     log_t_matrix_sum_mid = np.log(t_matrix_sum_mid)
     log_norm_params = (log_t_matrix_sum_mid.mean(), log_t_matrix_sum_mid.std(ddof=1))
```

### Comparing `scbsp-0.2.3/scbsp.egg-info/PKG-INFO` & `scbsp-0.2.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scbsp
-Version: 0.2.3
+Version: 0.2.4
 Summary: A package that efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data
 Home-page: https://github.com/YQ-Wang/scBSP
 Author: Yiqing Wang, Jinpu Li
 Author-email: yqw@wangemail.com, lijinp@health.missouri.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -13,69 +13,78 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
+Provides-Extra: hnsw
 License-File: LICENSE
 
 \n# scBSP
 
-scBSP is a specialized package designed for processing biological data, specifically in the analysis of gene expression and cell coordinates. It efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data.
+scBSP is a dedicated software package crafted for the nuanced domain of biological data processing, emphasizing gene expression analysis and cell coordinate evaluation. It offers a streamlined method to calculate p-values for a set of genes by leveraging input matrices that encapsulate cell coordinates and gene expression data.
 
 ## Installation
 
 ### Dependencies
-scBSP requires:
+To ensure scBSP functions optimally, the following dependencies are required:
 - Python (>= 3.8)
 - NumPy (>= 1.24.4)
 - Pandas (>= 1.3.5)
 - SciPy (>= 1.10.1)
+- scikit-learn (>=1.3.2)
+
+For enhanced scBSP using HNSW for distance calculation:
 - hnswlib (>= 0.8.0)
 
-To install scBSP, run the following command:
+### Installation Commands
+For Standard Installation (Using Ball Tree):
 
 `pip install scbsp`
 
+For Installation with HNSW (Hierarchical Navigable Small World Graphs):
+
+`pip install scbsp[hnsw]`
+
 ## Usage
 
 To use scBSP, you need to provide two primary inputs:
 
 1. **Cell Coordinates Matrix (`input_sp_mat`)**: 
    - Format: Numpy array.
    - Dimensions: N x D, where N is the number of cells and D is the dimension of coordinates.
 
 2. **Gene Expression Matrix (`input_exp_mat_raw`)**:
    - Format: Numpy array, Pandas DataFrame, or CSR matrix.
    - Dimensions: N x P, where N is the number of cells and P is the number of genes.
 
-Additionally, you must specify the following parameters:
+Additional parameters to specify include:
 
-- `d1`: A floating-point number.
-- `d2`: A floating-point number.
+- `d1`: A floating-point number. Default value is 1.0.
+- `d2`: A floating-point number. Default value is 3.0.
+- `leaf_size`: Optional integer defining the maximum point threshold for the Ball Tree algorithm to revert to brute-force search (default = 80). Not required for installations using HNSW.
 
 
 ### Example
 
-Here's a simple example to demonstrate how to compute p-values using scBSP:
+Below is a straightforward example showcasing how to compute p-values with scBSP:
 
 ```python
 import scbsp
 
 # Load your data into these variables
 input_sp_mat = ...  # Cell Coordinates Matrix
 input_exp_mat_raw = ...  # Gene Expression Matrix
 
 # Set the optional parameters
-d1 = 1.0  # Example value
-d2 = 3.0  # Example value
+d1 = 1.0
+d2 = 3.0
 
-# Execute the calculation
+# Compute p-values
 p_values = scbsp.granp(input_sp_mat, input_exp_mat_raw, d1, d2)
 ```
 
 ## Output
 
 The function returns a list of p-values, each corresponding to the genes in the provided gene expression matrix. These p-values help in identifying significant differences in gene expression across different cell coordinates, facilitating advanced biological data analysis.
```

### Comparing `scbsp-0.2.3/setup.py` & `scbsp-0.2.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\\n" + fh.read()
 
 setup(
     name="scbsp",
-    version="0.2.3",
+    version="0.2.4",
     description="A package that efficiently computes p-values for a given set of genes based on input matrices representing cell coordinates and gene expression data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["scbsp"],
     url="https://github.com/YQ-Wang/scBSP",
     author="Yiqing Wang, Jinpu Li",
     author_email="yqw@wangemail.com, lijinp@health.missouri.edu",
@@ -24,13 +24,13 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent",
     ],
-    install_requires=["numpy >= 1.24.4", "pandas >= 1.3.5", "scipy >= 1.10.1", "hnswlib >= 0.8.0"],
+    install_requires=["numpy >= 1.24.4", "pandas >= 1.3.5", "scipy >= 1.10.1", "scikit-learn>=1.3.2"],
     extras_require={
-        "dev": ["mypy>=1.7.0"],
+        "hnsw": ["hnswlib >= 0.8.0"],
     },
     python_requires=">=3.8",
 )
```

### Comparing `scbsp-0.2.3/test/test_scbsp.py` & `scbsp-0.2.4/test/test_scbsp.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import numpy as np
 import pandas as pd
 from scipy.sparse import csr_matrix
 from scipy.sparse import random as sparse_random
 
 from scbsp.scbsp import (
     _binary_distance_matrix_threshold,
-    _query_hnsw_index,
-    _scale_sparse_matrix,
     _calculate_sparse_variances,
     _get_test_scores,
+    _scale_sparse_matrix,
     granp,
 )
 
 
 class TestScaleSparseMinmax(unittest.TestCase):
     def test_scale_sparse_matrix(self):
         # Creating a small sparse matrix with known values
@@ -66,31 +65,27 @@
         self.assertIsInstance(scaled_matrix_dense, np.ndarray)
 
 
 class TestBinaryDistanceMatrixThreshold(unittest.TestCase):
     def test_non_empty_array(self):
         input_array = np.array([[0, 1], [1, 0], [1, 1]])
         d_val = 1.5
-        labels, distances = _query_hnsw_index(input_array)
+        leaf_size = 80
 
-        result = _binary_distance_matrix_threshold(
-            labels, distances, input_array, d_val
-        )
+        result = _binary_distance_matrix_threshold(input_array, d_val, leaf_size)
 
         self.assertIsInstance(result, csr_matrix)
         self.assertEqual(result.shape, (input_array.shape[0], input_array.shape[0]))
 
     def test_distance_threshold(self):
         input_array = np.array([[0, 0], [3, 3], [6, 6]])
         d_val = 5
-        labels, distances = _query_hnsw_index(input_array)
+        leaf_size = 80
 
-        result = _binary_distance_matrix_threshold(
-            labels, distances, input_array, d_val
-        )
+        result = _binary_distance_matrix_threshold(input_array, d_val, leaf_size)
 
         self.assertIsInstance(result, csr_matrix)
         self.assertTrue((result[result > d_val].count_nonzero()) == 0)
 
 
 class TestSpvars(unittest.TestCase):
     def test_non_empty_matrix(self):
@@ -130,16 +125,17 @@
         rows = np.array([0, 1, 2, 0, 1, 2])
         cols = np.array([0, 0, 0, 1, 1, 1])
         input_exp_mat_raw = csr_matrix((data, (rows, cols)), shape=(3, 2))
 
         # Define d1 and d2
         d1 = 1.0
         d2 = 3.0
+        leaf_size = 80
 
-        result = _get_test_scores(input_sp_mat, input_exp_mat_raw, d1, d2)
+        result = _get_test_scores(input_sp_mat, input_exp_mat_raw, d1, d2, leaf_size)
 
         # Check if the result is a numpy.ndarray
         self.assertIsInstance(result, list)
         # Check the shape of the result
         self.assertEqual(len(result), 2)  # Shape depends on your function's logic
 
 
@@ -149,14 +145,11 @@
         input_date = pd.read_csv(input_file)
         input_sp_mat = input_date[["x", "y", "z"]].to_numpy()
         input_exp_mat_raw = input_date.iloc[:, 3:]
 
         p_values = granp(input_sp_mat, input_exp_mat_raw)
 
         self.assertEqual(sum([(i < 0.0001).astype(int) for i in p_values[0:999]]), 996)
-        self.assertEqual(
-            sum([(i < 0.0001).astype(int) for i in p_values[1000:9999]]), 0
-        )
 
 
 if __name__ == "__main__":
     unittest.main()
```

