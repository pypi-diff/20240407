# Comparing `tmp/many-0.6.9.tar.gz` & `tmp/many-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "many-0.6.9.tar", max compression
+gzip compressed data, was "many-0.7.0.tar", max compression
```

## Comparing `many-0.6.9.tar` & `many-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1065 2020-07-31 23:16:16.000000 many-0.6.9/LICENSE
--rw-r--r--   0        0        0     2388 2020-09-29 03:52:53.000000 many-0.6.9/README.md
--rw-r--r--   0        0        0       52 2020-08-24 20:21:51.000000 many-0.6.9/many/__init__.py
--rw-r--r--   0        0        0      499 2020-11-20 20:32:45.000000 many-0.6.9/many/stats/__init__.py
--rw-r--r--   0        0        0     9712 2020-11-21 01:21:01.000000 many-0.6.9/many/stats/categorical_categorical.py
--rw-r--r--   0        0        0       59 2020-08-13 18:21:10.000000 many-0.6.9/many/stats/config.py
--rw-r--r--   0        0        0    16108 2021-08-25 17:03:51.764519 many-0.6.9/many/stats/continuous_categorical.py
--rw-r--r--   0        0        0    15312 2021-01-17 01:50:34.529344 many-0.6.9/many/stats/continuous_continuous.py
--rw-r--r--   0        0        0    14184 2020-11-16 21:31:48.000000 many-0.6.9/many/stats/continuous_continuous_cmap.py
--rw-r--r--   0        0        0    11048 2020-11-16 21:31:48.000000 many-0.6.9/many/stats/fisher.py
--rw-r--r--   0        0        0     1307 2020-08-23 22:33:36.000000 many-0.6.9/many/stats/utils.py
--rw-r--r--   0        0        0      327 2020-08-27 04:46:22.000000 many-0.6.9/many/visuals/__init__.py
--rw-r--r--   0        0        0     1928 2021-01-17 01:50:34.349048 many-0.6.9/many/visuals/categorical_categorical.py
--rw-r--r--   0        0        0    13457 2021-01-17 01:50:34.525521 many-0.6.9/many/visuals/continuous_categorical.py
--rw-r--r--   0        0        0    10518 2021-01-17 01:50:34.496365 many-0.6.9/many/visuals/continuous_continuous.py
--rw-r--r--   0        0        0     1205 2020-08-23 22:33:36.000000 many-0.6.9/many/visuals/utils.py
--rw-r--r--   0        0        0     1003 2022-01-09 04:51:19.908409 many-0.6.9/pyproject.toml
--rw-r--r--   0        0        0     3321 2022-01-09 04:51:31.885535 many-0.6.9/setup.py
--rw-r--r--   0        0        0     3399 2022-01-09 04:51:31.885807 many-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1065 2020-07-31 23:16:16.000000 many-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2388 2020-09-29 03:52:53.000000 many-0.7.0/README.md
+-rw-r--r--   0        0        0       52 2020-08-24 20:21:51.000000 many-0.7.0/many/__init__.py
+-rw-r--r--   0        0        0      499 2020-11-20 20:32:45.000000 many-0.7.0/many/stats/__init__.py
+-rw-r--r--   0        0        0     9712 2020-11-21 01:21:01.000000 many-0.7.0/many/stats/categorical_categorical.py
+-rw-r--r--   0        0        0       59 2020-08-13 18:21:10.000000 many-0.7.0/many/stats/config.py
+-rw-r--r--   0        0        0    16108 2021-08-25 17:03:51.764519 many-0.7.0/many/stats/continuous_categorical.py
+-rw-r--r--   0        0        0    15312 2021-01-17 01:50:34.529344 many-0.7.0/many/stats/continuous_continuous.py
+-rw-r--r--   0        0        0    14184 2020-11-16 21:31:48.000000 many-0.7.0/many/stats/continuous_continuous_cmap.py
+-rw-r--r--   0        0        0    11048 2020-11-16 21:31:48.000000 many-0.7.0/many/stats/fisher.py
+-rw-r--r--   0        0        0     1307 2020-08-23 22:33:36.000000 many-0.7.0/many/stats/utils.py
+-rw-r--r--   0        0        0      327 2020-08-27 04:46:22.000000 many-0.7.0/many/visuals/__init__.py
+-rw-r--r--   0        0        0     1928 2021-01-17 01:50:34.349048 many-0.7.0/many/visuals/categorical_categorical.py
+-rw-r--r--   0        0        0    13457 2021-01-17 01:50:34.525521 many-0.7.0/many/visuals/continuous_categorical.py
+-rw-r--r--   0        0        0    10518 2021-01-17 01:50:34.496365 many-0.7.0/many/visuals/continuous_continuous.py
+-rw-r--r--   0        0        0     1205 2020-08-23 22:33:36.000000 many-0.7.0/many/visuals/utils.py
+-rw-r--r--   0        0        0     1003 2024-04-07 17:04:15.865676 many-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3407 1970-01-01 00:00:00.000000 many-0.7.0/PKG-INFO
```

### Comparing `many-0.6.9/LICENSE` & `many-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `many-0.6.9/README.md` & `many-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/stats/categorical_categorical.py` & `many-0.7.0/many/stats/categorical_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/stats/continuous_categorical.py` & `many-0.7.0/many/stats/continuous_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/stats/continuous_continuous.py` & `many-0.7.0/many/stats/continuous_continuous.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/stats/continuous_continuous_cmap.py` & `many-0.7.0/many/stats/continuous_continuous_cmap.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/stats/fisher.py` & `many-0.7.0/many/stats/fisher.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/stats/utils.py` & `many-0.7.0/many/stats/utils.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/visuals/categorical_categorical.py` & `many-0.7.0/many/visuals/categorical_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/visuals/continuous_categorical.py` & `many-0.7.0/many/visuals/continuous_categorical.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/visuals/continuous_continuous.py` & `many-0.7.0/many/visuals/continuous_continuous.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/many/visuals/utils.py` & `many-0.7.0/many/visuals/utils.py`

 * *Files identical despite different names*

### Comparing `many-0.6.9/pyproject.toml` & `many-0.7.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 [tool.poetry]
 name = "many"
-version = "0.6.9"
+version = "0.7.0"
 description = "Statistical methods for computing many correlations"
 authors = ["Kevin Hu <kevinhuwest@gmail.com>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kevinhu/many"
 repository = "https://github.com/kevinhu/many"
 
-include = [
-    "LICENSE",
-]
+include = ["LICENSE"]
 
 [tool.poetry.dependencies]
-python = ">=3.6.1,<4.0"
-numpy = "^1.19.1"
-pandas = "^1.1.0"
-scipy = "^1.5.2"
-statsmodels = ">=0.11.1,<0.14.0"
-tqdm = "^4.48.2"
-matplotlib = "^3.3.0"
-sklearn = "^0.0"
-adjusttext = "^0.7.3"
+python = ">=3.9,<4.0"
+numpy = "^1.26.4"
+pandas = "^2.2.1"
+scipy = "^1.13.0"
+statsmodels = ">=0.14.1"
+tqdm = "^4.66.2"
+matplotlib = "^3.8.4"
+adjusttext = "^1.1.1"
 seaborn = "^0.11.0"
+scikit-learn = "^1.4.1.post1"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2"
-black = "^20.8b1"
-isort = "^5.9.3"
-pylint = "^2.10.2"
+pytest = "^8.1.1"
+black = "^24.3.0"
+isort = "^5.13.2"
+pylint = "^3.1.0"
 poethepoet = "^0.10.0"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
@@ -42,9 +40,9 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poe.tasks]
 black = "black ./many"
 isort = "isort ./many"
-format = ["black","isort"]
+format = ["black", "isort"]
 lint = "pylint ./many"
```

### Comparing `many-0.6.9/PKG-INFO` & `many-0.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: many
-Version: 0.6.9
+Version: 0.7.0
 Summary: Statistical methods for computing many correlations
 Home-page: https://github.com/kevinhu/many
 License: MIT
 Author: Kevin Hu
 Author-email: kevinhuwest@gmail.com
-Requires-Python: >=3.6.1,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: adjusttext (>=0.7.3,<0.8.0)
-Requires-Dist: matplotlib (>=3.3.0,<4.0.0)
-Requires-Dist: numpy (>=1.19.1,<2.0.0)
-Requires-Dist: pandas (>=1.1.0,<2.0.0)
-Requires-Dist: scipy (>=1.5.2,<2.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: adjusttext (>=1.1.1,<2.0.0)
+Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: scikit-learn (>=1.4.1.post1,<2.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
 Requires-Dist: seaborn (>=0.11.0,<0.12.0)
-Requires-Dist: sklearn (>=0.0,<0.1)
-Requires-Dist: statsmodels (>=0.11.1,<0.14.0)
-Requires-Dist: tqdm (>=4.48.2,<5.0.0)
+Requires-Dist: statsmodels (>=0.14.1)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/kevinhu/many
 Description-Content-Type: text/markdown
 
 # many
 
 This package provides a general-use toolkit for frequently-implemented statistical and visual methods. See the [blog post](https://kevinhu.io/2020/09/17/many.html) for an explanation of the purpose of this package and the methods used.
```

