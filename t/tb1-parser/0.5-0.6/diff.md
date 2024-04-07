# Comparing `tmp/tb1_parser-0.5.tar.gz` & `tmp/tb1_parser-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-0.5.tar", last modified: Sun Apr  7 12:42:33 2024, max compression
+gzip compressed data, was "tb1_parser-0.6.tar", last modified: Sun Apr  7 12:50:32 2024, max compression
```

## Comparing `tb1_parser-0.5.tar` & `tb1_parser-0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 12:42:33.338738 tb1_parser-0.5/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:42:33.338738 tb1_parser-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.5/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 12:42:33.340736 tb1_parser-0.5/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-04-07 12:42:27.000000 tb1_parser-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:42:33.324731 tb1_parser-0.5/tb1_parser/
--rw-rw-rw-   0        0        0      371 2024-04-07 12:38:15.000000 tb1_parser-0.5/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5783 2024-04-07 12:41:15.000000 tb1_parser-0.5/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2104 2024-04-07 12:41:27.000000 tb1_parser-0.5/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-0.5/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-0.5/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/_signal.py
--rw-rw-rw-   0        0        0     1752 2024-04-07 12:41:51.000000 tb1_parser-0.5/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0      541 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/ai_signal.py
--rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/di_signal.py
--rw-rw-rw-   0        0        0      354 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/do_signal.py
--rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/parsed_tb1_collection.py
--rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/signals_collection.py
--rw-rw-rw-   0        0        0     1639 2024-04-07 12:42:05.000000 tb1_parser-0.5/tb1_parser/tb1_parser.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/tb1_readed_sheets_collection.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:42:33.336735 tb1_parser-0.5/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 12:50:32.988659 tb1_parser-0.6/
+-rw-rw-rw-   0        0        0      249 2024-04-07 12:50:32.988659 tb1_parser-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:50:32.990659 tb1_parser-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-04-07 12:45:55.000000 tb1_parser-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:50:32.976657 tb1_parser-0.6/tb1_parser/
+-rw-rw-rw-   0        0        0      660 2024-04-07 12:50:10.000000 tb1_parser-0.6/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5783 2024-04-07 12:41:15.000000 tb1_parser-0.6/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2104 2024-04-07 12:41:27.000000 tb1_parser-0.6/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-0.6/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-0.6/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1753 2024-04-07 12:48:50.000000 tb1_parser-0.6/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/_tb1_readed_sheets_collection.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0      540 2024-04-07 12:50:13.000000 tb1_parser-0.6/tb1_parser/ai_signal.py
+-rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/di_signal.py
+-rw-rw-rw-   0        0        0      353 2024-04-07 12:50:12.000000 tb1_parser-0.6/tb1_parser/do_signal.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/parsed_tb1_collection.py
+-rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/signal.py
+-rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/signals_collection.py
+-rw-rw-rw-   0        0        0     1640 2024-04-07 12:48:50.000000 tb1_parser-0.6/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:50:32.987657 tb1_parser-0.6/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-0.5/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-0.6/tb1_parser/_ai_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.5/tb1_parser/_di_sheet_parser.py` & `tb1_parser-0.6/tb1_parser/_di_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.5/tb1_parser/_do_sheet_parser.py` & `tb1_parser-0.6/tb1_parser/_do_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.5/tb1_parser/_regex_lib.py` & `tb1_parser-0.6/tb1_parser/_regex_lib.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.5/tb1_parser/_sheet_parser.py` & `tb1_parser-0.6/tb1_parser/_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.5/tb1_parser/_signal.py` & `tb1_parser-0.6/tb1_parser/signal.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.5/tb1_parser/_tb1_file_reader.py` & `tb1_parser-0.6/tb1_parser/_tb1_file_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from typing import Any, Literal
 
 from pandas import DataFrame, ExcelFile
 
 from ._regex_lib import TB1 as config
 from ._tb1_sheet_reader import TB1SheetReader
-from .tb1_readed_sheets_collection import TB1ReadedSheetsCollection
+from ._tb1_readed_sheets_collection import TB1ReadedSheetsCollection
 
 
 all_avaible_sheets = list(config)
 
 
 class TB1FileReader:
```

### Comparing `tb1_parser-0.5/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-0.6/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.5/tb1_parser/ai_signal.py` & `tb1_parser-0.6/tb1_parser/ai_signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from ._signal import Signal
+from .signal import Signal
 
 
 class AiSignal(Signal):
 
     def __init__(self) -> None:
         '''
         Дата-класс для аналоговых входных сигналов, потомок 'Signal'.
```

### Comparing `tb1_parser-0.5/tb1_parser/tb1_parser.py` & `tb1_parser-0.6/tb1_parser/tb1_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ._ai_sheet_parser import AiSheetParser
 from ._di_sheet_parser import DiSheetParser
 from ._do_sheet_parser import DoSheetParser
 from ._tb1_file_reader import TB1FileReader
 from .parsed_tb1_collection import ParsedTB1Collection
-from .tb1_readed_sheets_collection import TB1ReadedSheetsCollection
+from ._tb1_readed_sheets_collection import TB1ReadedSheetsCollection
 
 
 class TB1Parser:
 
     def __init__(self, filepath: str) -> None:
         self.__logs_owner: str = self.__class__.__name__
         self.__filepath: str = filepath
```

### Comparing `tb1_parser-0.5/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-0.6/tb1_parser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 setup.py
 tb1_parser/__init__.py
 tb1_parser/_ai_sheet_parser.py
 tb1_parser/_di_sheet_parser.py
 tb1_parser/_do_sheet_parser.py
 tb1_parser/_regex_lib.py
 tb1_parser/_sheet_parser.py
-tb1_parser/_signal.py
 tb1_parser/_tb1_file_reader.py
+tb1_parser/_tb1_readed_sheets_collection.py
 tb1_parser/_tb1_sheet_reader.py
 tb1_parser/ai_signal.py
 tb1_parser/di_signal.py
 tb1_parser/do_signal.py
 tb1_parser/parsed_tb1_collection.py
+tb1_parser/signal.py
 tb1_parser/signals_collection.py
 tb1_parser/tb1_parser.py
-tb1_parser/tb1_readed_sheets_collection.py
 tb1_parser.egg-info/PKG-INFO
 tb1_parser.egg-info/SOURCES.txt
 tb1_parser.egg-info/dependency_links.txt
 tb1_parser.egg-info/not-zip-safe
 tb1_parser.egg-info/requires.txt
 tb1_parser.egg-info/top_level.txt
```

