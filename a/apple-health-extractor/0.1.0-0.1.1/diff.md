# Comparing `tmp/apple_health_extractor-0.1.0.tar.gz` & `tmp/apple_health_extractor-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_health_extractor-0.1.0.tar", max compression
+gzip compressed data, was "apple_health_extractor-0.1.1.tar", max compression
```

## Comparing `apple_health_extractor-0.1.0.tar` & `apple_health_extractor-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-28 18:43:57.946591 apple_health_extractor-0.1.0/LICENSE
--rw-r--r--   0        0        0     1193 2024-04-07 17:43:37.812043 apple_health_extractor-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-03-28 20:15:44.388449 apple_health_extractor-0.1.0/extractor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 20:54:40.201856 apple_health_extractor-0.1.0/extractor/constants/__init__.py
--rw-r--r--   0        0        0       35 2024-03-28 23:35:27.884226 apple_health_extractor-0.1.0/extractor/constants/metadata.py
--rw-r--r--   0        0        0     1892 2024-04-06 23:34:10.275376 apple_health_extractor-0.1.0/extractor/extractor.py
--rw-r--r--   0        0        0      709 2024-04-06 22:49:02.657856 apple_health_extractor-0.1.0/extractor/record.py
--rw-r--r--   0        0        0      635 2024-04-07 18:13:47.115376 apple_health_extractor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1951 1970-01-01 00:00:00.000000 apple_health_extractor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-28 18:43:57.946591 apple_health_extractor-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1193 2024-04-07 17:43:37.812043 apple_health_extractor-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-28 20:15:44.388449 apple_health_extractor-0.1.1/extractor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 20:54:40.201856 apple_health_extractor-0.1.1/extractor/constants/__init__.py
+-rw-r--r--   0        0        0       35 2024-03-28 23:35:27.884226 apple_health_extractor-0.1.1/extractor/constants/metadata.py
+-rw-r--r--   0        0        0     1892 2024-04-06 23:34:10.275376 apple_health_extractor-0.1.1/extractor/extractor.py
+-rw-r--r--   0        0        0      709 2024-04-06 22:49:02.657856 apple_health_extractor-0.1.1/extractor/record.py
+-rw-r--r--   0        0        0      704 2024-04-07 18:21:44.535198 apple_health_extractor-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 apple_health_extractor-0.1.1/PKG-INFO
```

### Comparing `apple_health_extractor-0.1.0/LICENSE` & `apple_health_extractor-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.0/README.md` & `apple_health_extractor-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.0/extractor/extractor.py` & `apple_health_extractor-0.1.1/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.0/extractor/record.py` & `apple_health_extractor-0.1.1/extractor/record.py`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.0/pyproject.toml` & `apple_health_extractor-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "apple-health-extractor"
-version = "0.1.0"
+version = "0.1.1"
 description = "This library provides functionality to parse and extract data from the XML exports of Apple Health app, enabling users to analyze and utilize their health data conveniently."
 authors = ["martinkelly23 <martkelly92@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+homepage = "https://github.com/martinkelly23/apple-health-extractor"
 
 keywords = [
   "data extractor",
   "apple health data",
 ]
 packages = [
   { include = "extractor" },
```

### Comparing `apple_health_extractor-0.1.0/PKG-INFO` & `apple_health_extractor-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: apple-health-extractor
-Version: 0.1.0
+Version: 0.1.1
 Summary: This library provides functionality to parse and extract data from the XML exports of Apple Health app, enabling users to analyze and utilize their health data conveniently.
+Home-page: https://github.com/martinkelly23/apple-health-extractor
 License: MIT
 Keywords: data extractor,apple health data
 Author: martinkelly23
 Author-email: martkelly92@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

