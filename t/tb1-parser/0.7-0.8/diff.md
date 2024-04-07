# Comparing `tmp/tb1_parser-0.7.tar.gz` & `tmp/tb1_parser-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tb1_parser-0.7.tar", last modified: Sun Apr  7 12:56:58 2024, max compression
+gzip compressed data, was "tb1_parser-0.8.tar", last modified: Sun Apr  7 13:07:07 2024, max compression
```

## Comparing `tb1_parser-0.7.tar` & `tb1_parser-0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 12:56:58.379049 tb1_parser-0.7/
--rw-rw-rw-   0        0        0      249 2024-04-07 12:56:58.378043 tb1_parser-0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.7/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 12:56:58.385048 tb1_parser-0.7/setup.cfg
--rw-rw-rw-   0        0        0      383 2024-04-07 12:56:45.000000 tb1_parser-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:56:58.368042 tb1_parser-0.7/tb1_parser/
--rw-rw-rw-   0        0        0      585 2024-04-07 12:56:12.000000 tb1_parser-0.7/tb1_parser/__init__.py
--rw-rw-rw-   0        0        0     5785 2024-04-07 12:54:57.000000 tb1_parser-0.7/tb1_parser/_ai_sheet_parser.py
--rw-rw-rw-   0        0        0     2106 2024-04-07 12:55:01.000000 tb1_parser-0.7/tb1_parser/_di_sheet_parser.py
--rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-0.7/tb1_parser/_do_sheet_parser.py
--rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/_regex_lib.py
--rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-0.7/tb1_parser/_sheet_parser.py
--rw-rw-rw-   0        0        0     1753 2024-04-07 12:48:50.000000 tb1_parser-0.7/tb1_parser/_tb1_file_reader.py
--rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/_tb1_readed_sheets_collection.py
--rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/_tb1_sheet_reader.py
--rw-rw-rw-   0        0        0      540 2024-04-07 12:50:13.000000 tb1_parser-0.7/tb1_parser/ai_signal.py
--rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/di_signal.py
--rw-rw-rw-   0        0        0      353 2024-04-07 12:50:12.000000 tb1_parser-0.7/tb1_parser/do_signal.py
--rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/parsed_tb1_collection.py
--rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/signal.py
--rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.7/tb1_parser/signals_collection.py
--rw-rw-rw-   0        0        0     1640 2024-04-07 12:55:41.000000 tb1_parser-0.7/tb1_parser/tb1_parser.py
-drwxrwxrwx   0        0        0        0 2024-04-07 12:56:58.377041 tb1_parser-0.7/tb1_parser.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-07 12:56:58.000000 tb1_parser-0.7/tb1_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 13:07:07.570034 tb1_parser-0.8/
+-rw-rw-rw-   0        0        0      249 2024-04-07 13:07:07.570034 tb1_parser-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 12:17:14.000000 tb1_parser-0.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 13:07:07.577043 tb1_parser-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      383 2024-04-07 13:07:00.000000 tb1_parser-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:07:07.558035 tb1_parser-0.8/tb1_parser/
+-rw-rw-rw-   0        0        0      585 2024-04-07 12:56:12.000000 tb1_parser-0.8/tb1_parser/__init__.py
+-rw-rw-rw-   0        0        0     5785 2024-04-07 12:54:57.000000 tb1_parser-0.8/tb1_parser/_ai_sheet_parser.py
+-rw-rw-rw-   0        0        0     2106 2024-04-07 12:55:01.000000 tb1_parser-0.8/tb1_parser/_di_sheet_parser.py
+-rw-rw-rw-   0        0        0     2192 2024-04-07 12:41:35.000000 tb1_parser-0.8/tb1_parser/_do_sheet_parser.py
+-rw-rw-rw-   0        0        0     5918 2024-04-07 12:17:14.000000 tb1_parser-0.8/tb1_parser/_regex_lib.py
+-rw-rw-rw-   0        0        0     4375 2024-04-07 12:41:43.000000 tb1_parser-0.8/tb1_parser/_sheet_parser.py
+-rw-rw-rw-   0        0        0     1767 2024-04-07 13:05:56.000000 tb1_parser-0.8/tb1_parser/_tb1_file_reader.py
+-rw-rw-rw-   0        0        0       48 2024-04-07 12:17:14.000000 tb1_parser-0.8/tb1_parser/_tb1_readed_sheets_collection.py
+-rw-rw-rw-   0        0        0     9218 2024-04-07 12:17:14.000000 tb1_parser-0.8/tb1_parser/_tb1_sheet_reader.py
+-rw-rw-rw-   0        0        0      540 2024-04-07 12:50:13.000000 tb1_parser-0.8/tb1_parser/ai_signal.py
+-rw-rw-rw-   0        0        0      455 2024-04-07 12:17:14.000000 tb1_parser-0.8/tb1_parser/di_signal.py
+-rw-rw-rw-   0        0        0      353 2024-04-07 12:50:12.000000 tb1_parser-0.8/tb1_parser/do_signal.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:17:14.000000 tb1_parser-0.8/tb1_parser/parsed_tb1_collection.py
+-rw-rw-rw-   0        0        0      571 2024-04-07 12:17:14.000000 tb1_parser-0.8/tb1_parser/signal.py
+-rw-rw-rw-   0        0        0       74 2024-04-07 12:17:14.000000 tb1_parser-0.8/tb1_parser/signals_collection.py
+-rw-rw-rw-   0        0        0     1640 2024-04-07 12:55:41.000000 tb1_parser-0.8/tb1_parser/tb1_parser.py
+drwxrwxrwx   0        0        0        0 2024-04-07 13:07:07.569033 tb1_parser-0.8/tb1_parser.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-07 13:07:07.000000 tb1_parser-0.8/tb1_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      693 2024-04-07 13:07:07.000000 tb1_parser-0.8/tb1_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 13:07:07.000000 tb1_parser-0.8/tb1_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 13:07:07.000000 tb1_parser-0.8/tb1_parser.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2024-04-07 13:07:07.000000 tb1_parser-0.8/tb1_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 13:07:07.000000 tb1_parser-0.8/tb1_parser.egg-info/top_level.txt
```

### Comparing `tb1_parser-0.7/tb1_parser/__init__.py` & `tb1_parser-0.8/tb1_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/_ai_sheet_parser.py` & `tb1_parser-0.8/tb1_parser/_ai_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/_di_sheet_parser.py` & `tb1_parser-0.8/tb1_parser/_di_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/_do_sheet_parser.py` & `tb1_parser-0.8/tb1_parser/_do_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/_regex_lib.py` & `tb1_parser-0.8/tb1_parser/_regex_lib.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/_sheet_parser.py` & `tb1_parser-0.8/tb1_parser/_sheet_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/_tb1_file_reader.py` & `tb1_parser-0.8/tb1_parser/_tb1_file_reader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import sys
-from typing import Any, Literal
+from typing import Literal
 
 from pandas import DataFrame, ExcelFile
 
 from ._regex_lib import TB1 as config
 from ._tb1_sheet_reader import TB1SheetReader
 from ._tb1_readed_sheets_collection import TB1ReadedSheetsCollection
 
@@ -20,23 +20,23 @@
 
         self.sheets: TB1ReadedSheetsCollection[str, DataFrame] = {}
 
 
     def __read_file(self) -> ExcelFile:
         logging.info(f'{self.__logs_owner}: открытие файла "{self.__filepath}"..')
         try:
-            logging.info(f'{self.__logs_owner}: файл успешно открыт')
             excel_file = ExcelFile(self.__filepath)
+            logging.info(f'{self.__logs_owner}: файл успешно открыт')
             return excel_file
-        except Exception:
-            logging.error(f'{self.__logs_owner}: не удалось открыть файл')
+        except Exception as error:
+            logging.error(f'{self.__logs_owner}: не удалось открыть файл - {error}')
             sys.exit(1)
 
 
-    def isvalid_sheet_type(self, input: Any) -> bool:
+    def isvalid_sheet_type(self, input: str) -> bool:
         return input in all_avaible_sheets
 
 
     def read(self, sheets: str | list[Literal['Ai', 'Di', 'Do']] = all_avaible_sheets):
         logging.info(f'{self.__logs_owner}: начало чтения ТБ1..')
 
         if not self.isvalid_sheet_type(sheets):
```

### Comparing `tb1_parser-0.7/tb1_parser/_tb1_sheet_reader.py` & `tb1_parser-0.8/tb1_parser/_tb1_sheet_reader.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/ai_signal.py` & `tb1_parser-0.8/tb1_parser/ai_signal.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/signal.py` & `tb1_parser-0.8/tb1_parser/signal.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser/tb1_parser.py` & `tb1_parser-0.8/tb1_parser/tb1_parser.py`

 * *Files identical despite different names*

### Comparing `tb1_parser-0.7/tb1_parser.egg-info/SOURCES.txt` & `tb1_parser-0.8/tb1_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

