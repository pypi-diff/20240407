# Comparing `tmp/tb1_parser-0.2.tar.gz` & `tmp/tb1_parser-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-0.2.tar", last modified: Sun Apr  7 12:28:34 2024, max compression
+gzip compressed data, was "tb1_parser-0.3.tar", last modified: Sun Apr  7 12:33:13 2024, max compression
```

## Comparing `tb1_parser-0.2.tar` & `tb1_parser-0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 12:28:34.621620 tb1_parser-0.2/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:28:34.621620 tb1_parser-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 12:28:34.623621 tb1_parser-0.2/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-04-07 12:25:12.000000 tb1_parser-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:28:34.612617 tb1_parser-0.2/tb1_parser/
--rw-rw-rw-   0        0        0      261 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5797 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2118 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2204 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4381 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1758 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0     1651 2024-04-07 12:17:14.000000 tb1_parser-0.2/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:28:34.619618 tb1_parser-0.2/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:28:34.000000 tb1_parser-0.2/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2024-04-07 12:28:34.000000 tb1_parser-0.2/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 12:28:34.000000 tb1_parser-0.2/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 12:28:34.000000 tb1_parser-0.2/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-04-07 12:28:34.000000 tb1_parser-0.2/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 12:28:34.000000 tb1_parser-0.2/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 12:33:13.410726 tb1_parser-0.3/
+-rw-rw-rw-   0        0        0      219 2024-04-07 12:33:13.410726 tb1_parser-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:33:13.411732 tb1_parser-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-04-07 12:33:07.000000 tb1_parser-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:33:13.398732 tb1_parser-0.3/tb1_parser/
+-rw-rw-rw-   0        0        0      262 2024-04-07 12:32:58.000000 tb1_parser-0.3/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5797 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2118 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2204 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4381 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1758 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0     1651 2024-04-07 12:17:14.000000 tb1_parser-0.3/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:33:13.409730 tb1_parser-0.3/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      219 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 12:28:34.000000 tb1_parser-0.3/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 12:33:13.000000 tb1_parser-0.3/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-0.2/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-0.3/tb1_parser/_ai_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.2/tb1_parser/_di_sheet_parser.py` & `tb1_parser-0.3/tb1_parser/_di_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.2/tb1_parser/_do_sheet_parser.py` & `tb1_parser-0.3/tb1_parser/_do_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.2/tb1_parser/_regex_lib.py` & `tb1_parser-0.3/tb1_parser/_regex_lib.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.2/tb1_parser/_sheet_parser.py` & `tb1_parser-0.3/tb1_parser/_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.2/tb1_parser/_tb1_file_reader.py` & `tb1_parser-0.3/tb1_parser/_tb1_file_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.2/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-0.3/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.2/tb1_parser/tb1_parser.py` & `tb1_parser-0.3/tb1_parser/tb1_parser.py`

 * *Files identical despite different names*
