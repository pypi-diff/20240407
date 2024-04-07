# Comparing `tmp/apple_health_extractor-0.1.2.tar.gz` & `tmp/apple_health_extractor-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_health_extractor-0.1.2.tar", max compression
+gzip compressed data, was "apple_health_extractor-0.1.3.tar", max compression
```

## Comparing `apple_health_extractor-0.1.2.tar` & `apple_health_extractor-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-28 18:43:57.946591 apple_health_extractor-0.1.2/LICENSE
--rw-r--r--   0        0        0     1195 2024-04-07 18:31:05.053129 apple_health_extractor-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-03-28 20:15:44.388449 apple_health_extractor-0.1.2/extractor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 20:54:40.201856 apple_health_extractor-0.1.2/extractor/constants/__init__.py
--rw-r--r--   0        0        0       35 2024-03-28 23:35:27.884226 apple_health_extractor-0.1.2/extractor/constants/metadata.py
--rw-r--r--   0        0        0     1892 2024-04-06 23:34:10.275376 apple_health_extractor-0.1.2/extractor/extractor.py
--rw-r--r--   0        0        0      709 2024-04-06 22:49:02.657856 apple_health_extractor-0.1.2/extractor/record.py
--rw-r--r--   0        0        0      704 2024-04-07 18:33:35.215677 apple_health_extractor-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2020 1970-01-01 00:00:00.000000 apple_health_extractor-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-28 18:43:57.946591 apple_health_extractor-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1195 2024-04-07 18:31:05.053129 apple_health_extractor-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-03-28 20:15:44.388449 apple_health_extractor-0.1.3/extractor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 20:54:40.201856 apple_health_extractor-0.1.3/extractor/constants/__init__.py
+-rw-r--r--   0        0        0       35 2024-03-28 23:35:27.884226 apple_health_extractor-0.1.3/extractor/constants/metadata.py
+-rw-r--r--   0        0        0     1892 2024-04-06 23:34:10.275376 apple_health_extractor-0.1.3/extractor/extractor.py
+-rw-r--r--   0        0        0      709 2024-04-06 22:49:02.657856 apple_health_extractor-0.1.3/extractor/record.py
+-rw-r--r--   0        0        0      703 2024-04-07 21:35:39.177767 apple_health_extractor-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2170 1970-01-01 00:00:00.000000 apple_health_extractor-0.1.3/PKG-INFO
```

### Comparing `apple_health_extractor-0.1.2/LICENSE` & `apple_health_extractor-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.2/README.md` & `apple_health_extractor-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.2/extractor/extractor.py` & `apple_health_extractor-0.1.3/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.2/extractor/record.py` & `apple_health_extractor-0.1.3/extractor/record.py`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.2/PKG-INFO` & `apple_health_extractor-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: apple-health-extractor
-Version: 0.1.2
+Version: 0.1.3
 Summary: This library provides functionality to parse and extract data from the XML exports of Apple Health app, enabling users to analyze and utilize their health data conveniently.
 Home-page: https://github.com/martinkelly23/apple-health-extractor
 License: MIT
 Keywords: data extractor,apple health data
 Author: martinkelly23
 Author-email: martkelly92@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: black (>=24.3.0,<25.0.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
```

