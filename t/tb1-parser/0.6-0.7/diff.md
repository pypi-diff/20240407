# Comparing `tmp/tb1_parser-0.6.tar.gz` & `tmp/tb1_parser-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-0.6.tar", last modified: Sun Apr  7 12:50:32 2024, max compression
+gzip compressed data, was "tb1_parser-0.7.tar", last modified: Sun Apr  7 12:56:58 2024, max compression
```

## Comparing `tb1_parser-0.6.tar` & `tb1_parser-0.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 12:50:32.988659 tb1_parser-0.6/
--rw-rw-rw-   0        0        0      249 2024-04-07 12:50:32.988659 tb1_parser-0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 12:50:32.990659 tb1_parser-0.6/setup.cfg
--rw-rw-rw-   0        0        0      383 2024-04-07 12:45:55.000000 tb1_parser-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:50:32.976657 tb1_parser-0.6/tb1_parser/
--rw-rw-rw-   0        0        0      660 2024-04-07 12:50:10.000000 tb1_parser-0.6/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5783 2024-04-07 12:41:15.000000 tb1_parser-0.6/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2104 2024-04-07 12:41:27.000000 tb1_parser-0.6/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-0.6/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-0.6/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1753 2024-04-07 12:48:50.000000 tb1_parser-0.6/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/_tb1_readed_sheets_collection.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0      540 2024-04-07 12:50:13.000000 tb1_parser-0.6/tb1_parser/ai_signal.py
--rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/di_signal.py
--rw-rw-rw-   0        0        0      353 2024-04-07 12:50:12.000000 tb1_parser-0.6/tb1_parser/do_signal.py
--rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/parsed_tb1_collection.py
--rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/signal.py
--rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.6/tb1_parser/signals_collection.py
--rw-rw-rw-   0        0        0     1640 2024-04-07 12:48:50.000000 tb1_parser-0.6/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:50:32.987657 tb1_parser-0.6/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 12:50:32.000000 tb1_parser-0.6/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 12:56:58.379049 tb1_parser-0.7/
+-rw-rw-rw-   0        0        0      249 2024-04-07 12:56:58.378043 tb1_parser-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:56:58.385048 tb1_parser-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-04-07 12:56:45.000000 tb1_parser-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:56:58.368042 tb1_parser-0.7/tb1_parser/
+-rw-rw-rw-   0        0        0      585 2024-04-07 12:56:12.000000 tb1_parser-0.7/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5785 2024-04-07 12:54:57.000000 tb1_parser-0.7/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2106 2024-04-07 12:55:01.000000 tb1_parser-0.7/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-0.7/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-0.7/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1753 2024-04-07 12:48:50.000000 tb1_parser-0.7/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/_tb1_readed_sheets_collection.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0      540 2024-04-07 12:50:13.000000 tb1_parser-0.7/tb1_parser/ai_signal.py
+-rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/di_signal.py
+-rw-rw-rw-   0        0        0      353 2024-04-07 12:50:12.000000 tb1_parser-0.7/tb1_parser/do_signal.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/parsed_tb1_collection.py
+-rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/signal.py
+-rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/signals_collection.py
+-rw-rw-rw-   0        0        0     1640 2024-04-07 12:55:41.000000 tb1_parser-0.7/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:56:58.377041 tb1_parser-0.7/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-0.6/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-0.7/tb1_parser/_ai_sheet_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import re
 
 from pandas import DataFrame
 
 from ._regex_lib import TB1
 from ._sheet_parser import SheetParser
-from ai_signal import AiSignal
-from signals_collection import SignalsCollection
+from .ai_signal import AiSignal
+from .signals_collection import SignalsCollection
 
 
 config = TB1['Ai']['regex']
 
 
 class AiSheetParser(SheetParser):
```

### Comparing `tb1_parser-0.6/tb1_parser/_di_sheet_parser.py` & `tb1_parser-0.7/tb1_parser/_di_sheet_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from pandas import DataFrame
 
 from ._do_sheet_parser import DoSheetParser
 from ._regex_lib import TB1 as config
-from di_signal import DiSignal
-from signals_collection import SignalsCollection
+from .di_signal import DiSignal
+from .signals_collection import SignalsCollection
 
 
 class DiSheetParser(DoSheetParser):
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
```

### Comparing `tb1_parser-0.6/tb1_parser/_do_sheet_parser.py` & `tb1_parser-0.7/tb1_parser/_do_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.6/tb1_parser/_regex_lib.py` & `tb1_parser-0.7/tb1_parser/_regex_lib.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.6/tb1_parser/_sheet_parser.py` & `tb1_parser-0.7/tb1_parser/_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.6/tb1_parser/_tb1_file_reader.py` & `tb1_parser-0.7/tb1_parser/_tb1_file_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.6/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-0.7/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.6/tb1_parser/ai_signal.py` & `tb1_parser-0.7/tb1_parser/ai_signal.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.6/tb1_parser/signal.py` & `tb1_parser-0.7/tb1_parser/signal.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.6/tb1_parser/tb1_parser.py` & `tb1_parser-0.7/tb1_parser/tb1_parser.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ._ai_sheet_parser import AiSheetParser
 from ._di_sheet_parser import DiSheetParser
 from ._do_sheet_parser import DoSheetParser
 from ._tb1_file_reader import TB1FileReader
-from .parsed_tb1_collection import ParsedTB1Collection
 from ._tb1_readed_sheets_collection import TB1ReadedSheetsCollection
+from .parsed_tb1_collection import ParsedTB1Collection
 
 
 class TB1Parser:
 
     def __init__(self, filepath: str) -> None:
         self.__logs_owner: str = self.__class__.__name__
         self.__filepath: str = filepath
```

### Comparing `tb1_parser-0.6/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-0.7/tb1_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

