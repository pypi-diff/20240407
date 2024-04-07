# Comparing `tmp/csv_test_package-0.1.0.tar.gz` & `tmp/csv_test_package-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_test_package-0.1.0.tar", max compression
+gzip compressed data, was "csv_test_package-0.1.1.tar", max compression
```

## Comparing `csv_test_package-0.1.0.tar` & `csv_test_package-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1211 2024-04-05 22:52:38.000000 csv_test_package-0.1.0/LICENSE
--rw-r--r--   0        0        0      135 2024-04-06 22:44:04.000000 csv_test_package-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-06 20:08:08.000000 csv_test_package-0.1.0/csv_test_package/__init__.py
--rw-r--r--   0        0        0      208 2024-04-06 23:19:50.000000 csv_test_package-0.1.0/csv_test_package/compare.py
--rw-r--r--   0        0        0      291 2024-04-06 20:08:08.000000 csv_test_package-0.1.0/csv_test_package/csvfile.py
--rw-r--r--   0        0        0        0 2024-04-06 20:08:08.000000 csv_test_package-0.1.0/csv_test_package/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-06 20:08:08.000000 csv_test_package-0.1.0/csv_test_package/utils.py
--rw-r--r--   0        0        0      472 2024-04-06 23:18:17.000000 csv_test_package-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 csv_test_package-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-05 22:52:38.000000 csv_test_package-0.1.1/LICENSE
+-rw-r--r--   0        0        0      135 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/__init__.py
+-rw-r--r--   0        0        0      208 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/compare.py
+-rw-r--r--   0        0        0      291 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/csvfile.py
+-rw-r--r--   0        0        0        0 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-06 23:52:52.000000 csv_test_package-0.1.1/csv_test_package/utils.py
+-rw-r--r--   0        0        0      472 2024-04-07 00:03:58.000000 csv_test_package-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      515 1970-01-01 00:00:00.000000 csv_test_package-0.1.1/PKG-INFO
```

### Comparing `csv_test_package-0.1.0/LICENSE` & `csv_test_package-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_test_package-0.1.0/PKG-INFO` & `csv_test_package-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv_test_package
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python package for comparing CSV files
 Author: Wassim SASSI
 Author-email: wassim.sassi.ws@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.2.1,<3.0.0)
```

