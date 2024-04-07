# Comparing `tmp/tb1_parser-0.3.tar.gz` & `tmp/tb1_parser-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-0.3.tar", last modified: Sun Apr  7 12:33:13 2024, max compression
+gzip compressed data, was "tb1_parser-0.4.tar", last modified: Sun Apr  7 12:39:13 2024, max compression
```

## Comparing `tb1_parser-0.3.tar` & `tb1_parser-0.4.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 12:33:13.410726 tb1_parser-0.3/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:33:13.410726 tb1_parser-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 12:33:13.411732 tb1_parser-0.3/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-04-07 12:33:07.000000 tb1_parser-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:33:13.398732 tb1_parser-0.3/tb1_parser/
--rw-rw-rw-   0        0        0      262 2024-04-07 12:32:58.000000 tb1_parser-0.3/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5797 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2118 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2204 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4381 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1758 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0     1651 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:33:13.409730 tb1_parser-0.3/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 12:28:34.000000 tb1_parser-0.3/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 12:39:13.049894 tb1_parser-0.4/
+-rw-rw-rw-   0        0        0      219 2024-04-07 12:39:13.049894 tb1_parser-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:39:13.051902 tb1_parser-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-04-07 12:38:59.000000 tb1_parser-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:39:13.037896 tb1_parser-0.4/tb1_parser/
+-rw-rw-rw-   0        0        0      371 2024-04-07 12:38:15.000000 tb1_parser-0.4/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5797 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2118 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2204 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4381 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_signal.py
+-rw-rw-rw-   0        0        0     1758 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0      541 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/ai_signal.py
+-rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/di_signal.py
+-rw-rw-rw-   0        0        0      354 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/do_signal.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/parsed_tb1_collection.py
+-rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/signals_collection.py
+-rw-rw-rw-   0        0        0     1651 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/tb1_parser.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/tb1_readed_sheets_collection.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:39:13.047898 tb1_parser-0.4/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      219 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-0.3/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-0.4/tb1_parser/_ai_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.3/tb1_parser/_di_sheet_parser.py` & `tb1_parser-0.4/tb1_parser/_di_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.3/tb1_parser/_do_sheet_parser.py` & `tb1_parser-0.4/tb1_parser/_do_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.3/tb1_parser/_regex_lib.py` & `tb1_parser-0.4/tb1_parser/_regex_lib.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.3/tb1_parser/_sheet_parser.py` & `tb1_parser-0.4/tb1_parser/_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.3/tb1_parser/_tb1_file_reader.py` & `tb1_parser-0.4/tb1_parser/_tb1_file_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.3/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-0.4/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.3/tb1_parser/tb1_parser.py` & `tb1_parser-0.4/tb1_parser/tb1_parser.py`

 * *Files identical despite different names*

