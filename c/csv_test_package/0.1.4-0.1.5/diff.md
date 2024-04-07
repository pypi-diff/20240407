# Comparing `tmp/csv_test_package-0.1.4.tar.gz` & `tmp/csv_test_package-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_test_package-0.1.4.tar", max compression
+gzip compressed data, was "csv_test_package-0.1.5.tar", max compression
```

## Comparing `csv_test_package-0.1.4.tar` & `csv_test_package-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1211 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/LICENSE
--rw-r--r--   0        0        0      135 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/csv_test_package/__init__.py
--rw-r--r--   0        0        0      208 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/csv_test_package/compare.py
--rw-r--r--   0        0        0      291 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/csv_test_package/csvfile.py
--rw-r--r--   0        0        0        0 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/csv_test_package/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/csv_test_package/utils.py
--rw-r--r--   0        0        0      472 2024-04-07 19:56:43.722219 csv_test_package-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 csv_test_package-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/LICENSE
+-rw-r--r--   0        0        0      135 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/csv_test_package/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/csv_test_package/compare.py
+-rw-r--r--   0        0        0      291 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/csv_test_package/csvfile.py
+-rw-r--r--   0        0        0        0 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/csv_test_package/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/csv_test_package/utils.py
+-rw-r--r--   0        0        0      472 2024-04-07 20:01:05.580860 csv_test_package-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 csv_test_package-0.1.5/PKG-INFO
```

### Comparing `csv_test_package-0.1.4/LICENSE` & `csv_test_package-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_test_package-0.1.4/PKG-INFO` & `csv_test_package-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv_test_package
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for comparing CSV files
 Author: Wassim SASSI
 Author-email: wassim.sassi.ws@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

