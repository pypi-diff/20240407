# Comparing `tmp/tb1_parser-0.4.tar.gz` & `tmp/tb1_parser-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-0.4.tar", last modified: Sun Apr  7 12:39:13 2024, max compression
+gzip compressed data, was "tb1_parser-0.5.tar", last modified: Sun Apr  7 12:42:33 2024, max compression
```

## Comparing `tb1_parser-0.4.tar` & `tb1_parser-0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 12:39:13.049894 tb1_parser-0.4/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:39:13.049894 tb1_parser-0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 12:39:13.051902 tb1_parser-0.4/setup.cfg
--rw-rw-rw-   0        0        0      366 2024-04-07 12:38:59.000000 tb1_parser-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:39:13.037896 tb1_parser-0.4/tb1_parser/
--rw-rw-rw-   0        0        0      371 2024-04-07 12:38:15.000000 tb1_parser-0.4/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5797 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2118 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2204 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4381 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_signal.py
--rw-rw-rw-   0        0        0     1758 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0      541 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/ai_signal.py
--rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/di_signal.py
--rw-rw-rw-   0        0        0      354 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/do_signal.py
--rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/parsed_tb1_collection.py
--rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/signals_collection.py
--rw-rw-rw-   0        0        0     1651 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/tb1_parser.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.4/tb1_parser/tb1_readed_sheets_collection.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:39:13.047898 tb1_parser-0.4/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      219 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 12:39:12.000000 tb1_parser-0.4/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 12:42:33.338738 tb1_parser-0.5/
+-rw-rw-rw-   0        0        0      219 2024-04-07 12:42:33.338738 tb1_parser-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:42:33.340736 tb1_parser-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-04-07 12:42:27.000000 tb1_parser-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:42:33.324731 tb1_parser-0.5/tb1_parser/
+-rw-rw-rw-   0        0        0      371 2024-04-07 12:38:15.000000 tb1_parser-0.5/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5783 2024-04-07 12:41:15.000000 tb1_parser-0.5/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2104 2024-04-07 12:41:27.000000 tb1_parser-0.5/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-0.5/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-0.5/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/_signal.py
+-rw-rw-rw-   0        0        0     1752 2024-04-07 12:41:51.000000 tb1_parser-0.5/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0      541 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/ai_signal.py
+-rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/di_signal.py
+-rw-rw-rw-   0        0        0      354 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/do_signal.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/parsed_tb1_collection.py
+-rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/signals_collection.py
+-rw-rw-rw-   0        0        0     1639 2024-04-07 12:42:05.000000 tb1_parser-0.5/tb1_parser/tb1_parser.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.5/tb1_parser/tb1_readed_sheets_collection.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:42:33.336735 tb1_parser-0.5/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      219 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 12:42:33.000000 tb1_parser-0.5/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-0.4/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-0.5/tb1_parser/_ai_sheet_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import re
 
 from pandas import DataFrame
 
 from ._regex_lib import TB1
 from ._sheet_parser import SheetParser
-from .types.ai_signal import AiSignal
-from .types.signals_collection import SignalsCollection
+from ai_signal import AiSignal
+from signals_collection import SignalsCollection
 
 
 config = TB1['Ai']['regex']
 
 
 class AiSheetParser(SheetParser):
```

### Comparing `tb1_parser-0.4/tb1_parser/_di_sheet_parser.py` & `tb1_parser-0.5/tb1_parser/_di_sheet_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from pandas import DataFrame
 
 from ._do_sheet_parser import DoSheetParser
 from ._regex_lib import TB1 as config
-from .types.di_signal import DiSignal
-from .types.signals_collection import SignalsCollection
+from di_signal import DiSignal
+from signals_collection import SignalsCollection
 
 
 class DiSheetParser(DoSheetParser):
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
```

### Comparing `tb1_parser-0.4/tb1_parser/_do_sheet_parser.py` & `tb1_parser-0.5/tb1_parser/_do_sheet_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from pandas import DataFrame
 
 from ._regex_lib import TB1 as config
 from ._sheet_parser import SheetParser
-from .types.do_signal import DoSignal
-from .types.signals_collection import SignalsCollection
+from .do_signal import DoSignal
+from .signals_collection import SignalsCollection
 
 
 class DoSheetParser(SheetParser):
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
```

### Comparing `tb1_parser-0.4/tb1_parser/_regex_lib.py` & `tb1_parser-0.5/tb1_parser/_regex_lib.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.4/tb1_parser/_sheet_parser.py` & `tb1_parser-0.5/tb1_parser/_sheet_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import re
 
 from pandas import DataFrame
 from transliterate import translit
 
 from ._regex_lib import PARSER as config
-from .types.signals_collection import SignalsCollection
+from .signals_collection import SignalsCollection
 
 
 class SheetParser:
 
     def __init__(self, sheet: DataFrame) -> None:
         self._logs_owner: str = self.__class__.__name__
         self._sheet = sheet
```

### Comparing `tb1_parser-0.4/tb1_parser/_signal.py` & `tb1_parser-0.5/tb1_parser/_signal.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.4/tb1_parser/_tb1_file_reader.py` & `tb1_parser-0.5/tb1_parser/_tb1_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 from typing import Any, Literal
 
 from pandas import DataFrame, ExcelFile
 
 from ._regex_lib import TB1 as config
 from ._tb1_sheet_reader import TB1SheetReader
-from .types.tb1_readed_sheets_collection import TB1ReadedSheetsCollection
+from .tb1_readed_sheets_collection import TB1ReadedSheetsCollection
 
 
 all_avaible_sheets = list(config)
 
 
 class TB1FileReader:
```

### Comparing `tb1_parser-0.4/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-0.5/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.4/tb1_parser/ai_signal.py` & `tb1_parser-0.5/tb1_parser/ai_signal.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.4/tb1_parser/tb1_parser.py` & `tb1_parser-0.5/tb1_parser/tb1_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 
 from ._ai_sheet_parser import AiSheetParser
 from ._di_sheet_parser import DiSheetParser
 from ._do_sheet_parser import DoSheetParser
 from ._tb1_file_reader import TB1FileReader
-from .types.parsed_tb1_collection import ParsedTB1Collection
-from .types.tb1_readed_sheets_collection import TB1ReadedSheetsCollection
+from .parsed_tb1_collection import ParsedTB1Collection
+from .tb1_readed_sheets_collection import TB1ReadedSheetsCollection
 
 
 class TB1Parser:
 
     def __init__(self, filepath: str) -> None:
         self.__logs_owner: str = self.__class__.__name__
         self.__filepath: str = filepath
```

### Comparing `tb1_parser-0.4/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-0.5/tb1_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

