# Comparing `tmp/mfoci-0.1.2.tar.gz` & `tmp/mfoci-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfoci-0.1.2.tar", max compression
+gzip compressed data, was "mfoci-0.1.3.tar", max compression
```

## Comparing `mfoci-0.1.2.tar` & `mfoci-0.1.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      466 2024-04-07 13:43:46.157714 mfoci-0.1.2/mfoci/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 12:30:19.184929 mfoci-0.1.2/mfoci/factors/__init__.py
--rw-r--r--   0        0        0     2087 2024-04-07 12:37:06.216614 mfoci-0.1.2/mfoci/factors/esg_factors.py
--rw-r--r--   0        0        0      706 2024-04-07 13:13:28.373738 mfoci-0.1.2/mfoci/factors/fama_french.py
--rw-r--r--   0        0        0        0 2024-04-07 13:23:36.730502 mfoci-0.1.2/mfoci/helpers/__init__.py
--rw-r--r--   0        0        0      712 2024-04-07 13:30:58.556054 mfoci-0.1.2/mfoci/helpers/filterer.py
--rw-r--r--   0        0        0      957 2024-04-07 13:53:49.215591 mfoci-0.1.2/mfoci/methods/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-07 13:53:46.987093 mfoci-0.1.2/mfoci/methods/kfoci.py
--rw-r--r--   0        0        0      666 2024-04-07 13:49:57.241245 mfoci-0.1.2/mfoci/methods/kfoci.R
--rw-r--r--   0        0        0     1146 2024-04-07 13:43:46.148861 mfoci-0.1.2/mfoci/methods/lasso.py
--rw-r--r--   0        0        0     1856 2024-04-07 13:56:24.633549 mfoci-0.1.2/mfoci/methods/mfoci_func.py
--rw-r--r--   0        0        0     2347 2024-04-07 12:47:46.625086 mfoci-0.1.2/mfoci/methods/multivar_chatterjee.py
--rw-r--r--   0        0        0       36 2024-04-07 13:46:55.896317 mfoci-0.1.2/mfoci/methods/selected_cols_gaussian.csv
--rw-r--r--   0        0        0       22 2024-04-07 13:46:20.382554 mfoci-0.1.2/mfoci/methods/selected_cols_linear.csv
--rw-r--r--   0        0        0   132738 2024-04-07 12:27:09.602881 mfoci-0.1.2/mfoci/methods/x.csv
--rw-r--r--   0        0        0   160194 2024-04-07 12:27:09.611395 mfoci-0.1.2/mfoci/methods/y.csv
--rw-r--r--   0        0        0       36 2024-04-07 13:53:22.699812 mfoci-0.1.2/mfoci/methodsselected_cols_gaussian.csv
--rw-r--r--   0        0        0       22 2024-04-07 13:52:47.163309 mfoci-0.1.2/mfoci/methodsselected_cols_linear.csv
--rw-r--r--   0        0        0        0 2024-04-07 12:31:23.708556 mfoci-0.1.2/mfoci/response_vars/__init__.py
--rw-r--r--   0        0        0      732 2024-04-07 12:37:06.222288 mfoci-0.1.2/mfoci/response_vars/etf_vars.py
--rw-r--r--   0        0        0      373 2024-04-07 13:46:35.155042 mfoci-0.1.2/mfoci/response_vars/stock_return_vars.py
--rw-r--r--   0        0        0      965 2024-04-07 13:20:49.318061 mfoci-0.1.2/mfoci/response_vars/volatility_vars.py
--rw-r--r--   0        0        0      620 2024-04-07 14:16:02.338896 mfoci-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2093 2024-04-07 14:16:02.340922 mfoci-0.1.2/README.md
--rw-r--r--   0        0        0     2817 1970-01-01 00:00:00.000000 mfoci-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      466 2024-04-07 13:43:46.157714 mfoci-0.1.3/mfoci/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:30:19.184929 mfoci-0.1.3/mfoci/factors/__init__.py
+-rw-r--r--   0        0        0     2087 2024-04-07 12:37:06.216614 mfoci-0.1.3/mfoci/factors/esg_factors.py
+-rw-r--r--   0        0        0      706 2024-04-07 13:13:28.373738 mfoci-0.1.3/mfoci/factors/fama_french.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:23:36.730502 mfoci-0.1.3/mfoci/helpers/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-07 13:30:58.556054 mfoci-0.1.3/mfoci/helpers/filterer.py
+-rw-r--r--   0        0        0      957 2024-04-07 13:53:49.215591 mfoci-0.1.3/mfoci/methods/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-07 13:53:46.987093 mfoci-0.1.3/mfoci/methods/kfoci.py
+-rw-r--r--   0        0        0      666 2024-04-07 13:49:57.241245 mfoci-0.1.3/mfoci/methods/kfoci.R
+-rw-r--r--   0        0        0     1146 2024-04-07 13:43:46.148861 mfoci-0.1.3/mfoci/methods/lasso.py
+-rw-r--r--   0        0        0     1856 2024-04-07 13:56:24.633549 mfoci-0.1.3/mfoci/methods/mfoci_func.py
+-rw-r--r--   0        0        0     2347 2024-04-07 12:47:46.625086 mfoci-0.1.3/mfoci/methods/multivar_chatterjee.py
+-rw-r--r--   0        0        0       36 2024-04-07 13:46:55.896317 mfoci-0.1.3/mfoci/methods/selected_cols_gaussian.csv
+-rw-r--r--   0        0        0       22 2024-04-07 13:46:20.382554 mfoci-0.1.3/mfoci/methods/selected_cols_linear.csv
+-rw-r--r--   0        0        0   132738 2024-04-07 12:27:09.602881 mfoci-0.1.3/mfoci/methods/x.csv
+-rw-r--r--   0        0        0   160194 2024-04-07 12:27:09.611395 mfoci-0.1.3/mfoci/methods/y.csv
+-rw-r--r--   0        0        0       36 2024-04-07 13:53:22.699812 mfoci-0.1.3/mfoci/methodsselected_cols_gaussian.csv
+-rw-r--r--   0        0        0       22 2024-04-07 13:52:47.163309 mfoci-0.1.3/mfoci/methodsselected_cols_linear.csv
+-rw-r--r--   0        0        0        0 2024-04-07 12:31:23.708556 mfoci-0.1.3/mfoci/response_vars/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-07 12:37:06.222288 mfoci-0.1.3/mfoci/response_vars/etf_vars.py
+-rw-r--r--   0        0        0      373 2024-04-07 13:46:35.155042 mfoci-0.1.3/mfoci/response_vars/stock_return_vars.py
+-rw-r--r--   0        0        0      440 2024-04-07 14:24:51.227734 mfoci-0.1.3/mfoci/response_vars/volatility_vars.py
+-rw-r--r--   0        0        0      597 2024-04-07 14:26:46.412520 mfoci-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2090 2024-04-07 14:19:46.797565 mfoci-0.1.3/README.md
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 mfoci-0.1.3/PKG-INFO
```

### Comparing `mfoci-0.1.2/mfoci/factors/esg_factors.py` & `mfoci-0.1.3/mfoci/factors/esg_factors.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/factors/fama_french.py` & `mfoci-0.1.3/mfoci/factors/fama_french.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/helpers/filterer.py` & `mfoci-0.1.3/mfoci/helpers/filterer.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/__init__.py` & `mfoci-0.1.3/mfoci/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/kfoci.py` & `mfoci-0.1.3/mfoci/methods/kfoci.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/kfoci.R` & `mfoci-0.1.3/mfoci/methods/kfoci.R`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/lasso.py` & `mfoci-0.1.3/mfoci/methods/lasso.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/mfoci_func.py` & `mfoci-0.1.3/mfoci/methods/mfoci_func.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/multivar_chatterjee.py` & `mfoci-0.1.3/mfoci/methods/multivar_chatterjee.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/x.csv` & `mfoci-0.1.3/mfoci/methods/x.csv`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/methods/y.csv` & `mfoci-0.1.3/mfoci/methods/y.csv`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/mfoci/response_vars/etf_vars.py` & `mfoci-0.1.3/mfoci/response_vars/etf_vars.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.2/pyproject.toml` & `mfoci-0.1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "mfoci"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Marcus Rockel <corram@outlook.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 # stock_loader = {path = "../../finadvisor/stock-loader", develop = true}
 # eikon_api_wrapper = {path = "../../eikon_api_wrapper", develop = true}
-numpy = "^1.26.4"
-pandas = "^2.2.1"
-pandas-datareader = "^0.10.0"
-scikit-learn = "^1.4.1.post1"
-matplotlib = "^3.8.4"
-statsmodels = "^0.14.1"
-jinja2 = "^3.1.3"
-yfinance = "^0.2.37"
+numpy = "^1.26"
+pandas = "^2.2"
+pandas-datareader = "^0.10"
+scikit-learn = "^1.4"
+matplotlib = "^3.8"
+statsmodels = "^0.14"
+jinja2 = "^3.1"
+yfinance = "^0.2"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `mfoci-0.1.2/README.md` & `mfoci-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -52,10 +52,10 @@
 
 # KFOCI factor selection (ensure Rscript is installed and path is set)
 r_path = "C:/Program Files/R/R-4.3.3/bin/x64/Rscript"
 kfoci_linear_selected, kfoci_gaussian_selected = select_factors(
     factors, response_vars, "kfoci", r_path=r_path
 )
 
-# m´MFOCI factor selection
+# MFOCI factor selection
 mfoci_selected, t_values = select_factors(factors, response_vars, "mfoci")
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mfoci-0.1.2/PKG-INFO` & `mfoci-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: mfoci
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Marcus Rockel
 Author-email: corram@outlook.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pandas (>=2.2.1,<3.0.0)
-Requires-Dist: pandas-datareader (>=0.10.0,<0.11.0)
-Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
-Requires-Dist: statsmodels (>=0.14.1,<0.15.0)
-Requires-Dist: yfinance (>=0.2.37,<0.3.0)
+Requires-Dist: jinja2 (>=3.1,<4.0)
+Requires-Dist: matplotlib (>=3.8,<4.0)
+Requires-Dist: numpy (>=1.26,<2.0)
+Requires-Dist: pandas (>=2.2,<3.0)
+Requires-Dist: pandas-datareader (>=0.10,<0.11)
+Requires-Dist: scikit-learn (>=1.4,<2.0)
+Requires-Dist: statsmodels (>=0.14,<0.15)
+Requires-Dist: yfinance (>=0.2,<0.3)
 Description-Content-Type: text/markdown
 
 # Factor selection with MFOCI
 
 `mfoci` is a Python package designed for financial analysts and researchers who need to retrieve and analyze stock market data.
  This package implements the MFOCI algorithm for factor selection in financial data. Supported are also LASSO and k-FOCI factor selection methods as well as data retrieval from Fama-French and Yahoo Finance.
 
@@ -74,11 +74,11 @@
 
 # KFOCI factor selection (ensure Rscript is installed and path is set)
 r_path = "C:/Program Files/R/R-4.3.3/bin/x64/Rscript"
 kfoci_linear_selected, kfoci_gaussian_selected = select_factors(
     factors, response_vars, "kfoci", r_path=r_path
 )
 
-# m´MFOCI factor selection
+# MFOCI factor selection
 mfoci_selected, t_values = select_factors(factors, response_vars, "mfoci")
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

