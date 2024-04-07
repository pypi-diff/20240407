# Comparing `tmp/mfoci-0.1.1.tar.gz` & `tmp/mfoci-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfoci-0.1.1.tar", max compression
+gzip compressed data, was "mfoci-0.1.2.tar", max compression
```

## Comparing `mfoci-0.1.1.tar` & `mfoci-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      466 2024-04-07 13:43:46.157714 mfoci-0.1.1/mfoci/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 12:30:19.184929 mfoci-0.1.1/mfoci/factors/__init__.py
--rw-r--r--   0        0        0     2087 2024-04-07 12:37:06.216614 mfoci-0.1.1/mfoci/factors/esg_factors.py
--rw-r--r--   0        0        0      706 2024-04-07 13:13:28.373738 mfoci-0.1.1/mfoci/factors/fama_french.py
--rw-r--r--   0        0        0        0 2024-04-07 13:23:36.730502 mfoci-0.1.1/mfoci/helpers/__init__.py
--rw-r--r--   0        0        0      712 2024-04-07 13:30:58.556054 mfoci-0.1.1/mfoci/helpers/filterer.py
--rw-r--r--   0        0        0      957 2024-04-07 13:53:49.215591 mfoci-0.1.1/mfoci/methods/__init__.py
--rw-r--r--   0        0        0     1089 2024-04-07 13:53:46.987093 mfoci-0.1.1/mfoci/methods/kfoci.py
--rw-r--r--   0        0        0      666 2024-04-07 13:49:57.241245 mfoci-0.1.1/mfoci/methods/kfoci.R
--rw-r--r--   0        0        0     1146 2024-04-07 13:43:46.148861 mfoci-0.1.1/mfoci/methods/lasso.py
--rw-r--r--   0        0        0     1856 2024-04-07 13:56:24.633549 mfoci-0.1.1/mfoci/methods/mfoci_func.py
--rw-r--r--   0        0        0     2347 2024-04-07 12:47:46.625086 mfoci-0.1.1/mfoci/methods/multivar_chatterjee.py
--rw-r--r--   0        0        0       36 2024-04-07 13:46:55.896317 mfoci-0.1.1/mfoci/methods/selected_cols_gaussian.csv
--rw-r--r--   0        0        0       22 2024-04-07 13:46:20.382554 mfoci-0.1.1/mfoci/methods/selected_cols_linear.csv
--rw-r--r--   0        0        0   132738 2024-04-07 12:27:09.602881 mfoci-0.1.1/mfoci/methods/x.csv
--rw-r--r--   0        0        0   160194 2024-04-07 12:27:09.611395 mfoci-0.1.1/mfoci/methods/y.csv
--rw-r--r--   0        0        0       36 2024-04-07 13:53:22.699812 mfoci-0.1.1/mfoci/methodsselected_cols_gaussian.csv
--rw-r--r--   0        0        0       22 2024-04-07 13:52:47.163309 mfoci-0.1.1/mfoci/methodsselected_cols_linear.csv
--rw-r--r--   0        0        0        0 2024-04-07 12:31:23.708556 mfoci-0.1.1/mfoci/response_vars/__init__.py
--rw-r--r--   0        0        0      732 2024-04-07 12:37:06.222288 mfoci-0.1.1/mfoci/response_vars/etf_vars.py
--rw-r--r--   0        0        0      373 2024-04-07 13:46:35.155042 mfoci-0.1.1/mfoci/response_vars/stock_return_vars.py
--rw-r--r--   0        0        0      965 2024-04-07 13:20:49.318061 mfoci-0.1.1/mfoci/response_vars/volatility_vars.py
--rw-r--r--   0        0        0      620 2024-04-07 14:13:23.283502 mfoci-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2156 2024-04-07 14:13:23.285506 mfoci-0.1.1/README.md
--rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 mfoci-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      466 2024-04-07 13:43:46.157714 mfoci-0.1.2/mfoci/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 12:30:19.184929 mfoci-0.1.2/mfoci/factors/__init__.py
+-rw-r--r--   0        0        0     2087 2024-04-07 12:37:06.216614 mfoci-0.1.2/mfoci/factors/esg_factors.py
+-rw-r--r--   0        0        0      706 2024-04-07 13:13:28.373738 mfoci-0.1.2/mfoci/factors/fama_french.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:23:36.730502 mfoci-0.1.2/mfoci/helpers/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-07 13:30:58.556054 mfoci-0.1.2/mfoci/helpers/filterer.py
+-rw-r--r--   0        0        0      957 2024-04-07 13:53:49.215591 mfoci-0.1.2/mfoci/methods/__init__.py
+-rw-r--r--   0        0        0     1089 2024-04-07 13:53:46.987093 mfoci-0.1.2/mfoci/methods/kfoci.py
+-rw-r--r--   0        0        0      666 2024-04-07 13:49:57.241245 mfoci-0.1.2/mfoci/methods/kfoci.R
+-rw-r--r--   0        0        0     1146 2024-04-07 13:43:46.148861 mfoci-0.1.2/mfoci/methods/lasso.py
+-rw-r--r--   0        0        0     1856 2024-04-07 13:56:24.633549 mfoci-0.1.2/mfoci/methods/mfoci_func.py
+-rw-r--r--   0        0        0     2347 2024-04-07 12:47:46.625086 mfoci-0.1.2/mfoci/methods/multivar_chatterjee.py
+-rw-r--r--   0        0        0       36 2024-04-07 13:46:55.896317 mfoci-0.1.2/mfoci/methods/selected_cols_gaussian.csv
+-rw-r--r--   0        0        0       22 2024-04-07 13:46:20.382554 mfoci-0.1.2/mfoci/methods/selected_cols_linear.csv
+-rw-r--r--   0        0        0   132738 2024-04-07 12:27:09.602881 mfoci-0.1.2/mfoci/methods/x.csv
+-rw-r--r--   0        0        0   160194 2024-04-07 12:27:09.611395 mfoci-0.1.2/mfoci/methods/y.csv
+-rw-r--r--   0        0        0       36 2024-04-07 13:53:22.699812 mfoci-0.1.2/mfoci/methodsselected_cols_gaussian.csv
+-rw-r--r--   0        0        0       22 2024-04-07 13:52:47.163309 mfoci-0.1.2/mfoci/methodsselected_cols_linear.csv
+-rw-r--r--   0        0        0        0 2024-04-07 12:31:23.708556 mfoci-0.1.2/mfoci/response_vars/__init__.py
+-rw-r--r--   0        0        0      732 2024-04-07 12:37:06.222288 mfoci-0.1.2/mfoci/response_vars/etf_vars.py
+-rw-r--r--   0        0        0      373 2024-04-07 13:46:35.155042 mfoci-0.1.2/mfoci/response_vars/stock_return_vars.py
+-rw-r--r--   0        0        0      965 2024-04-07 13:20:49.318061 mfoci-0.1.2/mfoci/response_vars/volatility_vars.py
+-rw-r--r--   0        0        0      620 2024-04-07 14:16:02.338896 mfoci-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2093 2024-04-07 14:16:02.340922 mfoci-0.1.2/README.md
+-rw-r--r--   0        0        0     2817 1970-01-01 00:00:00.000000 mfoci-0.1.2/PKG-INFO
```

### Comparing `mfoci-0.1.1/mfoci/factors/esg_factors.py` & `mfoci-0.1.2/mfoci/factors/esg_factors.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/factors/fama_french.py` & `mfoci-0.1.2/mfoci/factors/fama_french.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/helpers/filterer.py` & `mfoci-0.1.2/mfoci/helpers/filterer.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/__init__.py` & `mfoci-0.1.2/mfoci/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/kfoci.py` & `mfoci-0.1.2/mfoci/methods/kfoci.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/kfoci.R` & `mfoci-0.1.2/mfoci/methods/kfoci.R`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/lasso.py` & `mfoci-0.1.2/mfoci/methods/lasso.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/mfoci_func.py` & `mfoci-0.1.2/mfoci/methods/mfoci_func.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/multivar_chatterjee.py` & `mfoci-0.1.2/mfoci/methods/multivar_chatterjee.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/x.csv` & `mfoci-0.1.2/mfoci/methods/x.csv`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/methods/y.csv` & `mfoci-0.1.2/mfoci/methods/y.csv`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/response_vars/etf_vars.py` & `mfoci-0.1.2/mfoci/response_vars/etf_vars.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/mfoci/response_vars/volatility_vars.py` & `mfoci-0.1.2/mfoci/response_vars/volatility_vars.py`

 * *Files identical despite different names*

### Comparing `mfoci-0.1.1/pyproject.toml` & `mfoci-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mfoci"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Marcus Rockel <corram@outlook.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 # stock_loader = {path = "../../finadvisor/stock-loader", develop = true}
```

### Comparing `mfoci-0.1.1/README.md` & `mfoci-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -14,22 +14,20 @@
 
 ## Quick Usage
 
 ```python
 from mfoci import get_fama_french_data, load_stock_returns
 from mfoci import select_factors
 
-# Fetch Fama-French factors
-factors = get_fama_french_data("2004-01-01", end_date="2024-01-01")
-
-# Load stock returns for specific tickers
+# Fetch data
 tickers = ["MSFT", "AAPL", "NVDA", "AMZN", "META", "GOOG"]
 response_vars = load_stock_returns(tickers, start_date="2013-01-01", end_date="2024-01-01")
+factors = get_fama_french_data("2013-01-01", end_date="2024-01-01")
 
-# m´MFOCI factor selection
+# MFOCI factor selection
 mfoci_selected, t_values = select_factors(factors, response_vars, "mfoci")
 ```
 
 
 ## Further usage
 
 ```python
```

### Comparing `mfoci-0.1.1/PKG-INFO` & `mfoci-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mfoci
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Marcus Rockel
 Author-email: corram@outlook.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -36,22 +36,20 @@
 
 ## Quick Usage
 
 ```python
 from mfoci import get_fama_french_data, load_stock_returns
 from mfoci import select_factors
 
-# Fetch Fama-French factors
-factors = get_fama_french_data("2004-01-01", end_date="2024-01-01")
-
-# Load stock returns for specific tickers
+# Fetch data
 tickers = ["MSFT", "AAPL", "NVDA", "AMZN", "META", "GOOG"]
 response_vars = load_stock_returns(tickers, start_date="2013-01-01", end_date="2024-01-01")
+factors = get_fama_french_data("2013-01-01", end_date="2024-01-01")
 
-# m´MFOCI factor selection
+# MFOCI factor selection
 mfoci_selected, t_values = select_factors(factors, response_vars, "mfoci")
 ```
 
 
 ## Further usage
 
 ```python
```

