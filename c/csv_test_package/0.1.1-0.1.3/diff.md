# Comparing `tmp/csv_test_package-0.1.1.tar.gz` & `tmp/csv_test_package-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_test_package-0.1.1.tar", max compression
+gzip compressed data, was "csv_test_package-0.1.3.tar", max compression
```

## Comparing `csv_test_package-0.1.1.tar` & `csv_test_package-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1211 2024-04-05 22:52:38.000000 csv_test_package-0.1.1/LICENSE
--rw-r--r--   0        0        0      135 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/__init__.py
--rw-r--r--   0        0        0      208 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/compare.py
--rw-r--r--   0        0        0      291 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/csvfile.py
--rw-r--r--   0        0        0        0 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/utils.py
--rw-r--r--   0        0        0      472 2024-04-07 00:03:58.000000 csv_test_package-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 csv_test_package-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-07 19:49:31.737645 csv_test_package-0.1.3/LICENSE
+-rw-r--r--   0        0        0      135 2024-04-07 19:49:31.737645 csv_test_package-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 19:49:31.741645 csv_test_package-0.1.3/csv_test_package/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-07 19:49:31.741645 csv_test_package-0.1.3/csv_test_package/compare.py
+-rw-r--r--   0        0        0      291 2024-04-07 19:49:31.741645 csv_test_package-0.1.3/csv_test_package/csvfile.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:49:31.741645 csv_test_package-0.1.3/csv_test_package/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:49:31.741645 csv_test_package-0.1.3/csv_test_package/utils.py
+-rw-r--r--   0        0        0      472 2024-04-07 19:49:31.741645 csv_test_package-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      566 1970-01-01 00:00:00.000000 csv_test_package-0.1.3/PKG-INFO
```

### Comparing `csv_test_package-0.1.1/LICENSE` & `csv_test_package-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_test_package-0.1.1/PKG-INFO` & `csv_test_package-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: csv_test_package
-Version: 0.1.1
+Version: 0.1.3
 Summary: A Python package for comparing CSV files
 Author: Wassim SASSI
 Author-email: wassim.sassi.ws@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 [![codecov](https://codecov.io/gh/WasassiM/csv_comparer/graph/badge.svg?token=F8AG4KV512)](https://codecov.io/gh/WasassiM/csv_comparer)
```

