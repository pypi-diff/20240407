# Comparing `tmp/apple_health_extractor-0.1.1.tar.gz` & `tmp/apple_health_extractor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apple_health_extractor-0.1.1.tar", max compression
+gzip compressed data, was "apple_health_extractor-0.1.2.tar", max compression
```

## Comparing `apple_health_extractor-0.1.1.tar` & `apple_health_extractor-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-03-28 18:43:57.946591 apple_health_extractor-0.1.1/LICENSE
--rw-r--r--   0        0        0     1193 2024-04-07 17:43:37.812043 apple_health_extractor-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-28 20:15:44.388449 apple_health_extractor-0.1.1/extractor/__init__.py
--rw-r--r--   0        0        0        0 2024-03-28 20:54:40.201856 apple_health_extractor-0.1.1/extractor/constants/__init__.py
--rw-r--r--   0        0        0       35 2024-03-28 23:35:27.884226 apple_health_extractor-0.1.1/extractor/constants/metadata.py
--rw-r--r--   0        0        0     1892 2024-04-06 23:34:10.275376 apple_health_extractor-0.1.1/extractor/extractor.py
--rw-r--r--   0        0        0      709 2024-04-06 22:49:02.657856 apple_health_extractor-0.1.1/extractor/record.py
--rw-r--r--   0        0        0      704 2024-04-07 18:21:44.535198 apple_health_extractor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2018 1970-01-01 00:00:00.000000 apple_health_extractor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-03-28 18:43:57.946591 apple_health_extractor-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1195 2024-04-07 18:31:05.053129 apple_health_extractor-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-28 20:15:44.388449 apple_health_extractor-0.1.2/extractor/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-28 20:54:40.201856 apple_health_extractor-0.1.2/extractor/constants/__init__.py
+-rw-r--r--   0        0        0       35 2024-03-28 23:35:27.884226 apple_health_extractor-0.1.2/extractor/constants/metadata.py
+-rw-r--r--   0        0        0     1892 2024-04-06 23:34:10.275376 apple_health_extractor-0.1.2/extractor/extractor.py
+-rw-r--r--   0        0        0      709 2024-04-06 22:49:02.657856 apple_health_extractor-0.1.2/extractor/record.py
+-rw-r--r--   0        0        0      704 2024-04-07 18:33:35.215677 apple_health_extractor-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2020 1970-01-01 00:00:00.000000 apple_health_extractor-0.1.2/PKG-INFO
```

### Comparing `apple_health_extractor-0.1.1/LICENSE` & `apple_health_extractor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.1/README.md` & `apple_health_extractor-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 Convert health data from XML format to JSON and CSV.
 Retrieve types of records present in the health data.
 Extract records of a specific type.
 
 ### Installation
 You can install the library via pip:
 ```python
-pip install health-data-extractor
+pip install apple-health-extractor
 ```
 
 ### Usage
 ```python
-from health_data_extractor import Extractor
+from apple_health_extractor import Extractor
 
 # Initialize the extractor with the path to the XML file
 extractor = Extractor("path/to/health_data.xml")
 
 # Get the health data as JSON
 json_data = extractor.get_json()
```

### Comparing `apple_health_extractor-0.1.1/extractor/extractor.py` & `apple_health_extractor-0.1.2/extractor/extractor.py`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.1/extractor/record.py` & `apple_health_extractor-0.1.2/extractor/record.py`

 * *Files identical despite different names*

### Comparing `apple_health_extractor-0.1.1/pyproject.toml` & `apple_health_extractor-0.1.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apple-health-extractor"
-version = "0.1.1"
+version = "0.1.2"
 description = "This library provides functionality to parse and extract data from the XML exports of Apple Health app, enabling users to analyze and utilize their health data conveniently."
 authors = ["martinkelly23 <martkelly92@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/martinkelly23/apple-health-extractor"
 
 keywords = [
```

### Comparing `apple_health_extractor-0.1.1/PKG-INFO` & `apple_health_extractor-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apple-health-extractor
-Version: 0.1.1
+Version: 0.1.2
 Summary: This library provides functionality to parse and extract data from the XML exports of Apple Health app, enabling users to analyze and utilize their health data conveniently.
 Home-page: https://github.com/martinkelly23/apple-health-extractor
 License: MIT
 Keywords: data extractor,apple health data
 Author: martinkelly23
 Author-email: martkelly92@gmail.com
 Requires-Python: >=3.11,<4.0
@@ -24,20 +24,20 @@
 Convert health data from XML format to JSON and CSV.
 Retrieve types of records present in the health data.
 Extract records of a specific type.
 
 ### Installation
 You can install the library via pip:
 ```python
-pip install health-data-extractor
+pip install apple-health-extractor
 ```
 
 ### Usage
 ```python
-from health_data_extractor import Extractor
+from apple_health_extractor import Extractor
 
 # Initialize the extractor with the path to the XML file
 extractor = Extractor("path/to/health_data.xml")
 
 # Get the health data as JSON
 json_data = extractor.get_json()
```

