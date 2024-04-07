# Comparing `tmp/xlutil-0.1.2.tar.gz` & `tmp/xlutil-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xlutil-0.1.2.tar", max compression
+gzip compressed data, was "xlutil-0.1.3.tar", max compression
```

## Comparing `xlutil-0.1.2.tar` & `xlutil-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0     1071 2024-02-16 22:59:28.337802 xlutil-0.1.2/LICENSE
--rw-r--r--   0        0        0       59 2024-02-16 22:59:28.337901 xlutil-0.1.2/README.md
--rw-r--r--   0        0        0      636 2024-02-17 01:11:50.168491 xlutil-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      105 2024-02-16 23:10:04.597242 xlutil-0.1.2/xlutil/__init__.py
--rw-r--r--   0        0        0     3691 2024-02-17 01:09:39.152882 xlutil-0.1.2/xlutil/core/__init__.py
--rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 xlutil-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-02-16 22:59:28.337802 xlutil-0.1.3/LICENSE
+-rw-r--r--   0        0        0       59 2024-02-16 22:59:28.337901 xlutil-0.1.3/README.md
+-rw-r--r--   0        0        0      657 2024-04-07 07:50:18.552169 xlutil-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      105 2024-02-16 23:10:04.597242 xlutil-0.1.3/xlutil/__init__.py
+-rw-r--r--   0        0        0       35 2024-04-06 13:14:09.813167 xlutil-0.1.3/xlutil/constants.py
+-rw-r--r--   0        0        0     9962 2024-04-07 08:31:53.284593 xlutil-0.1.3/xlutil/core/__init__.py
+-rw-r--r--   0        0        0     4907 2024-04-06 20:41:19.046124 xlutil-0.1.3/xlutil/core/utils.py
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 xlutil-0.1.3/PKG-INFO
```

### Comparing `xlutil-0.1.2/LICENSE` & `xlutil-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xlutil-0.1.2/pyproject.toml` & `xlutil-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "xlutil"
-version = "0.1.2"
+version = "0.1.3"
 description = "Excel utilities for easier workflow when dealing with dataframes and excel files"
 authors = ["Santo K Thomas <santokalayil@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/santokalayil/xlutil"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pandas = "^2.2.0"
 pyarrow = "^15.0.0"
 openpyxl = "^3.1.2"
 matplotlib = "^3.8.3"
 seaborn = "^0.13.2"
 pydantic = "^2.6.1"
+xlsxwriter = "^3.2.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pytest = "^8.0.1"
 ipykernel = "^6.29.2"
 
 [build-system]
```

### Comparing `xlutil-0.1.2/PKG-INFO` & `xlutil-0.1.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 Metadata-Version: 2.1
 Name: xlutil
-Version: 0.1.2
+Version: 0.1.3
 Summary: Excel utilities for easier workflow when dealing with dataframes and excel files
 Home-page: https://github.com/santokalayil/xlutil
 License: MIT
 Author: Santo K Thomas
 Author-email: santokalayil@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.3,<4.0.0)
 Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0)
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: seaborn (>=0.13.2,<0.14.0)
+Requires-Dist: xlsxwriter (>=3.2.0,<4.0.0)
 Project-URL: Repository, https://github.com/santokalayil/xlutil
 Description-Content-Type: text/markdown
 
 # xlutil
 Excel Utilities library created by Santo K Thomas
```

