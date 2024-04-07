# Comparing `tmp/PyQvd-1.0.2.tar.gz` & `tmp/PyQvd-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQvd-1.0.2.tar", last modified: Tue Apr  2 11:18:02 2024, max compression
+gzip compressed data, was "PyQvd-1.1.0.tar", last modified: Sun Apr  7 10:49:23 2024, max compression
```

## Comparing `PyQvd-1.0.2.tar` & `PyQvd-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:18:02.803867 PyQvd-1.0.2/
--rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 PyQvd-1.0.2/LICENSE.md
--rw-rw-rw-   0        0        0    11944 2024-04-02 11:18:02.803867 PyQvd-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 11:18:02.803867 PyQvd-1.0.2/PyQvd.egg-info/
--rw-rw-rw-   0        0        0    11944 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-04-02 11:18:02.000000 PyQvd-1.0.2/PyQvd.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9734 2024-03-27 12:50:40.000000 PyQvd-1.0.2/README.md
--rw-rw-rw-   0        0        0     1288 2024-04-02 11:12:07.000000 PyQvd-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-04-02 11:18:02.801249 PyQvd-1.0.2/pyqvd/
--rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 PyQvd-1.0.2/pyqvd/__init__.py
--rw-rw-rw-   0        0        0    36067 2024-04-02 11:00:04.000000 PyQvd-1.0.2/pyqvd/qvd.py
--rw-rw-rw-   0        0        0       42 2024-04-02 11:18:02.803867 PyQvd-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 10:49:23.544315 PyQvd-1.1.0/
+-rw-rw-rw-   0        0        0     1096 2024-03-27 12:50:40.000000 PyQvd-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0    12492 2024-04-07 10:49:23.543112 PyQvd-1.1.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 10:49:23.540811 PyQvd-1.1.0/PyQvd.egg-info/
+-rw-rw-rw-   0        0        0    12492 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-07 10:49:23.000000 PyQvd-1.1.0/PyQvd.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    10282 2024-04-07 10:48:20.000000 PyQvd-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1288 2024-04-07 10:48:28.000000 PyQvd-1.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-07 10:49:23.534321 PyQvd-1.1.0/pyqvd/
+-rw-rw-rw-   0        0        0       88 2024-04-02 10:45:55.000000 PyQvd-1.1.0/pyqvd/__init__.py
+-rw-rw-rw-   0        0        0    37372 2024-04-07 10:48:20.000000 PyQvd-1.1.0/pyqvd/qvd.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 10:49:23.545661 PyQvd-1.1.0/setup.cfg
```

### Comparing `PyQvd-1.0.2/LICENSE.md` & `PyQvd-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PyQvd-1.0.2/PKG-INFO` & `PyQvd-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.0.2
+Version: 1.1.0
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,23 +57,25 @@
 - [QVD File Format](#qvd-file-format)
   - [XML Header](#xml-header)
   - [Symbol Table](#symbol-table)
   - [Index Table](#index-table)
 - [API Documentation](#api-documentation)
   - [QvdDataFrame](#qvddataframe)
     - [`@staticmethod from_qvd(path: str) -> QvdDataFrame`](#staticmethod-from_qvdpath-str---qvddataframe)
-    - [`@staticmethod from_dict(data: dict[str, list[any]]) -> QvdDataFrame`](#staticmethod-from_dictdata-dictstr-listany---qvddataframe)
+    - [`@staticmethod from_stream(source: BinaryIO) -> QvdDataFrame`](#staticmethod-from_streamsource-binaryio---qvddataframe)
+    - [`@staticmethod from_dict(data: Dict[str, List[any]]) -> QvdDataFrame`](#staticmethod-from_dictdata-dictstr-listany---qvddataframe)
     - [`@staticmethod from_pandas(data: pandas.DataFrame) -> QvdDataFrame`](#staticmethod-from_pandasdata-pandasdataframe---qvddataframe)
     - [`head(n: int) -> QvdDataFrame`](#headn-int---qvddataframe)
     - [`tail(n: int) -> QvdDataFrame`](#tailn-int---qvddataframe)
     - [`select(*args: str) -> QvdDataFrame`](#selectargs-str---qvddataframe)
     - [`rows(*args: int) -> QvdDataFrame`](#rowsargs-int---qvddataframe)
     - [`at(row: int, column: str) -> any`](#atrow-int-column-str---any)
-    - [`to_dict() -> dict[str, list[any]]`](#to_dict---dictstr-listany)
+    - [`to_dict() -> Dict[str, List[any]]`](#to_dict---dictstr-listany)
     - [`to_qvd(path: str) -> None`](#to_qvdpath-str---none)
+    - [`to_stream(target: BinaryIO) -> None`](#to_streamtarget-binaryio---none)
     - [`to_pandas() -> pandas.DataFrame`](#to_pandas---pandasdataframe)
 - [License](#license)
   - [Forbidden](#forbidden)
 
 ---
 
 ## Install
@@ -150,15 +152,19 @@
 | `data`    | `list[list[any]]` | The actual data. The first dimension represents the single rows.                            |
 | `columns` | `list[str]`       | The names of the fields that are contained in the QVD file.                                 |
 
 #### `@staticmethod from_qvd(path: str) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_qvd` loads a QVD file from the given path and parses it. The method returns a `QvdDataFrame` instance.
 
-#### `@staticmethod from_dict(data: dict[str, list[any]]) -> QvdDataFrame`
+#### `@staticmethod from_stream(source: BinaryIO) -> QvdDataFrame`
+
+The static method `QvdDataFrame.from_stream` loads a QVD file from the given binary stream. The method returns a `QvdDataFrame` instance.
+
+#### `@staticmethod from_dict(data: Dict[str, List[any]]) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_dict` constructs a data frame from a dictionary. The dictionary must contain the columns and the actual data as properties. The columns property is an array of strings that contains the names of the fields in the QVD file. The data property is an array of arrays that contains the actual data records. The order of the values in the inner arrays corresponds to the order of the fields in the QVD file.
 
 #### `@staticmethod from_pandas(data: pandas.DataFrame) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_pandas` constructs a data frame from a pandas data frame.
 
@@ -178,22 +184,26 @@
 
 The method `rows` returns a new data frame that contains only the specified rows.
 
 #### `at(row: int, column: str) -> any`
 
 The method `at` returns the value at the specified row and column.
 
-#### `to_dict() -> dict[str, list[any]]`
+#### `to_dict() -> Dict[str, List[any]]`
 
 The method `to_dict` returns the data frame as a dictionary. The dictionary contains the columns and the actual data as properties. The columns property is an array of strings that contains the names of the fields in the QVD file. The data property is an array of arrays that contains the actual data records. The order of the values in the inner arrays corresponds to the order of the fields in the QVD file.
 
 #### `to_qvd(path: str) -> None`
 
 The method `to_qvd` writes the data frame to a QVD file at the specified path.
 
+#### `to_stream(target: BinaryIO) -> None`
+
+The method `to_stream` writes the data frame as a QVD file to a binary stream.
+
 #### `to_pandas() -> pandas.DataFrame`
 
 The method `to_pandas` returns the data frame as a pandas data frame.
 
 ## License
 
 Copyright (c) 2024 Constantin Müller
```

### Comparing `PyQvd-1.0.2/PyQvd.egg-info/PKG-INFO` & `PyQvd-1.1.0/PyQvd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQvd
-Version: 1.0.2
+Version: 1.1.0
 Summary: Utility library for reading/writing Qlik View Data (QVD) files in Python.
 Author-email: Constantin Müller <info@mueller-constantin.de>
 License: MIT License
         
         Copyright (c) 2024 Constantin Müller
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -57,23 +57,25 @@
 - [QVD File Format](#qvd-file-format)
   - [XML Header](#xml-header)
   - [Symbol Table](#symbol-table)
   - [Index Table](#index-table)
 - [API Documentation](#api-documentation)
   - [QvdDataFrame](#qvddataframe)
     - [`@staticmethod from_qvd(path: str) -> QvdDataFrame`](#staticmethod-from_qvdpath-str---qvddataframe)
-    - [`@staticmethod from_dict(data: dict[str, list[any]]) -> QvdDataFrame`](#staticmethod-from_dictdata-dictstr-listany---qvddataframe)
+    - [`@staticmethod from_stream(source: BinaryIO) -> QvdDataFrame`](#staticmethod-from_streamsource-binaryio---qvddataframe)
+    - [`@staticmethod from_dict(data: Dict[str, List[any]]) -> QvdDataFrame`](#staticmethod-from_dictdata-dictstr-listany---qvddataframe)
     - [`@staticmethod from_pandas(data: pandas.DataFrame) -> QvdDataFrame`](#staticmethod-from_pandasdata-pandasdataframe---qvddataframe)
     - [`head(n: int) -> QvdDataFrame`](#headn-int---qvddataframe)
     - [`tail(n: int) -> QvdDataFrame`](#tailn-int---qvddataframe)
     - [`select(*args: str) -> QvdDataFrame`](#selectargs-str---qvddataframe)
     - [`rows(*args: int) -> QvdDataFrame`](#rowsargs-int---qvddataframe)
     - [`at(row: int, column: str) -> any`](#atrow-int-column-str---any)
-    - [`to_dict() -> dict[str, list[any]]`](#to_dict---dictstr-listany)
+    - [`to_dict() -> Dict[str, List[any]]`](#to_dict---dictstr-listany)
     - [`to_qvd(path: str) -> None`](#to_qvdpath-str---none)
+    - [`to_stream(target: BinaryIO) -> None`](#to_streamtarget-binaryio---none)
     - [`to_pandas() -> pandas.DataFrame`](#to_pandas---pandasdataframe)
 - [License](#license)
   - [Forbidden](#forbidden)
 
 ---
 
 ## Install
@@ -150,15 +152,19 @@
 | `data`    | `list[list[any]]` | The actual data. The first dimension represents the single rows.                            |
 | `columns` | `list[str]`       | The names of the fields that are contained in the QVD file.                                 |
 
 #### `@staticmethod from_qvd(path: str) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_qvd` loads a QVD file from the given path and parses it. The method returns a `QvdDataFrame` instance.
 
-#### `@staticmethod from_dict(data: dict[str, list[any]]) -> QvdDataFrame`
+#### `@staticmethod from_stream(source: BinaryIO) -> QvdDataFrame`
+
+The static method `QvdDataFrame.from_stream` loads a QVD file from the given binary stream. The method returns a `QvdDataFrame` instance.
+
+#### `@staticmethod from_dict(data: Dict[str, List[any]]) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_dict` constructs a data frame from a dictionary. The dictionary must contain the columns and the actual data as properties. The columns property is an array of strings that contains the names of the fields in the QVD file. The data property is an array of arrays that contains the actual data records. The order of the values in the inner arrays corresponds to the order of the fields in the QVD file.
 
 #### `@staticmethod from_pandas(data: pandas.DataFrame) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_pandas` constructs a data frame from a pandas data frame.
 
@@ -178,22 +184,26 @@
 
 The method `rows` returns a new data frame that contains only the specified rows.
 
 #### `at(row: int, column: str) -> any`
 
 The method `at` returns the value at the specified row and column.
 
-#### `to_dict() -> dict[str, list[any]]`
+#### `to_dict() -> Dict[str, List[any]]`
 
 The method `to_dict` returns the data frame as a dictionary. The dictionary contains the columns and the actual data as properties. The columns property is an array of strings that contains the names of the fields in the QVD file. The data property is an array of arrays that contains the actual data records. The order of the values in the inner arrays corresponds to the order of the fields in the QVD file.
 
 #### `to_qvd(path: str) -> None`
 
 The method `to_qvd` writes the data frame to a QVD file at the specified path.
 
+#### `to_stream(target: BinaryIO) -> None`
+
+The method `to_stream` writes the data frame as a QVD file to a binary stream.
+
 #### `to_pandas() -> pandas.DataFrame`
 
 The method `to_pandas` returns the data frame as a pandas data frame.
 
 ## License
 
 Copyright (c) 2024 Constantin Müller
```

### Comparing `PyQvd-1.0.2/README.md` & `PyQvd-1.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -13,23 +13,25 @@
 - [QVD File Format](#qvd-file-format)
   - [XML Header](#xml-header)
   - [Symbol Table](#symbol-table)
   - [Index Table](#index-table)
 - [API Documentation](#api-documentation)
   - [QvdDataFrame](#qvddataframe)
     - [`@staticmethod from_qvd(path: str) -> QvdDataFrame`](#staticmethod-from_qvdpath-str---qvddataframe)
-    - [`@staticmethod from_dict(data: dict[str, list[any]]) -> QvdDataFrame`](#staticmethod-from_dictdata-dictstr-listany---qvddataframe)
+    - [`@staticmethod from_stream(source: BinaryIO) -> QvdDataFrame`](#staticmethod-from_streamsource-binaryio---qvddataframe)
+    - [`@staticmethod from_dict(data: Dict[str, List[any]]) -> QvdDataFrame`](#staticmethod-from_dictdata-dictstr-listany---qvddataframe)
     - [`@staticmethod from_pandas(data: pandas.DataFrame) -> QvdDataFrame`](#staticmethod-from_pandasdata-pandasdataframe---qvddataframe)
     - [`head(n: int) -> QvdDataFrame`](#headn-int---qvddataframe)
     - [`tail(n: int) -> QvdDataFrame`](#tailn-int---qvddataframe)
     - [`select(*args: str) -> QvdDataFrame`](#selectargs-str---qvddataframe)
     - [`rows(*args: int) -> QvdDataFrame`](#rowsargs-int---qvddataframe)
     - [`at(row: int, column: str) -> any`](#atrow-int-column-str---any)
-    - [`to_dict() -> dict[str, list[any]]`](#to_dict---dictstr-listany)
+    - [`to_dict() -> Dict[str, List[any]]`](#to_dict---dictstr-listany)
     - [`to_qvd(path: str) -> None`](#to_qvdpath-str---none)
+    - [`to_stream(target: BinaryIO) -> None`](#to_streamtarget-binaryio---none)
     - [`to_pandas() -> pandas.DataFrame`](#to_pandas---pandasdataframe)
 - [License](#license)
   - [Forbidden](#forbidden)
 
 ---
 
 ## Install
@@ -106,15 +108,19 @@
 | `data`    | `list[list[any]]` | The actual data. The first dimension represents the single rows.                            |
 | `columns` | `list[str]`       | The names of the fields that are contained in the QVD file.                                 |
 
 #### `@staticmethod from_qvd(path: str) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_qvd` loads a QVD file from the given path and parses it. The method returns a `QvdDataFrame` instance.
 
-#### `@staticmethod from_dict(data: dict[str, list[any]]) -> QvdDataFrame`
+#### `@staticmethod from_stream(source: BinaryIO) -> QvdDataFrame`
+
+The static method `QvdDataFrame.from_stream` loads a QVD file from the given binary stream. The method returns a `QvdDataFrame` instance.
+
+#### `@staticmethod from_dict(data: Dict[str, List[any]]) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_dict` constructs a data frame from a dictionary. The dictionary must contain the columns and the actual data as properties. The columns property is an array of strings that contains the names of the fields in the QVD file. The data property is an array of arrays that contains the actual data records. The order of the values in the inner arrays corresponds to the order of the fields in the QVD file.
 
 #### `@staticmethod from_pandas(data: pandas.DataFrame) -> QvdDataFrame`
 
 The static method `QvdDataFrame.from_pandas` constructs a data frame from a pandas data frame.
 
@@ -134,22 +140,26 @@
 
 The method `rows` returns a new data frame that contains only the specified rows.
 
 #### `at(row: int, column: str) -> any`
 
 The method `at` returns the value at the specified row and column.
 
-#### `to_dict() -> dict[str, list[any]]`
+#### `to_dict() -> Dict[str, List[any]]`
 
 The method `to_dict` returns the data frame as a dictionary. The dictionary contains the columns and the actual data as properties. The columns property is an array of strings that contains the names of the fields in the QVD file. The data property is an array of arrays that contains the actual data records. The order of the values in the inner arrays corresponds to the order of the fields in the QVD file.
 
 #### `to_qvd(path: str) -> None`
 
 The method `to_qvd` writes the data frame to a QVD file at the specified path.
 
+#### `to_stream(target: BinaryIO) -> None`
+
+The method `to_stream` writes the data frame as a QVD file to a binary stream.
+
 #### `to_pandas() -> pandas.DataFrame`
 
 The method `to_pandas` returns the data frame as a pandas data frame.
 
 ## License
 
 Copyright (c) 2024 Constantin Müller
```

### Comparing `PyQvd-1.0.2/pyproject.toml` & `PyQvd-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyQvd"
-version = "1.0.2"
+version = "1.1.0"
 description = "Utility library for reading/writing Qlik View Data (QVD) files in Python."
 readme = {file = "README.md", content-type = "text/markdown"}
 license = {file = "LICENSE.md"}
 authors = [
     {name = "Constantin Müller", email = "info@mueller-constantin.de"},
 ]
 keywords = ["qlik", "qvd", "qlik sense", "qlik view", "pandas"]
```

### Comparing `PyQvd-1.0.2/pyqvd/qvd.py` & `PyQvd-1.1.0/pyqvd/qvd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """
 Contains classes for parsing and representing QVD files.
 """
 
 import uuid
 import time
-import os
 import struct
-from typing import TYPE_CHECKING, Union, List, Tuple, Dict
+import io
+from typing import TYPE_CHECKING, Union, List, Tuple, Dict, BinaryIO
 import xml.etree.ElementTree as ET
 from xml.dom import minidom
 from tabulate import tabulate
 
 if TYPE_CHECKING:
     import pandas as pd
 
@@ -79,32 +79,32 @@
     def to_byte_representation(self) -> bytes:
         """
         Converts the symbol to its byte representation.
 
         :return: The byte representation of the symbol.
         """
         if self._int_value is not None and self._string_value is not None:
-            return (b'\05' +
-                    self._int_value.to_bytes(4, byteorder='little', signed=True) +
+            return (b"\05" +
+                    self._int_value.to_bytes(4, byteorder="little", signed=True) +
                     str.encode(self._string_value) +
-                    b'\0')
+                    b"\0")
 
         if self._double_value is not None and self._string_value is not None:
-            return b'\06' + struct.pack('<d', self._double_value) + str.encode(self._string_value) + b'\0'
+            return b"\06" + struct.pack("<d", self._double_value) + str.encode(self._string_value) + b"\0"
 
         if self._int_value is not None:
-            return b'\01' + self._int_value.to_bytes(4, byteorder='little', signed=True)
+            return b"\01" + self._int_value.to_bytes(4, byteorder="little", signed=True)
 
         if self._double_value is not None:
-            return b'\02' + struct.pack('<d', self._double_value)
+            return b"\02" + struct.pack("<d", self._double_value)
 
         if self._string_value is not None:
-            return b'\04' + str.encode(self._string_value) + b'\0'
+            return b"\04" + str.encode(self._string_value) + b"\0"
 
-        raise ValueError('The symbol does not contain any value.')
+        raise ValueError("The symbol does not contain any value.")
 
     def __eq__(self, __value: object) -> bool:
         """
         Determines whether this symbol is equal to another object.
 
         :param __value: The other object.
         :return: True if the objects are equal, otherwise False.
@@ -197,33 +197,33 @@
         """
         Returns the shape of the data frame.
 
         :return: The shape.
         """
         return len(self._data), len(self._columns)
 
-    def head(self, n: int = 5) -> 'QvdDataFrame':
+    def head(self, n: int = 5) -> "QvdDataFrame":
         """
         Returns the first n rows of the data frame.
 
         :param n: The number of rows to return.
         :return: The first n rows.
         """
         return QvdDataFrame(self._data[:n], self._columns)
 
-    def tail(self, n: int = 5) -> 'QvdDataFrame':
+    def tail(self, n: int = 5) -> "QvdDataFrame":
         """
         Returns the last n rows of the data frame.
 
         :param n: The number of rows to return.
         :return: The last n rows.
         """
         return QvdDataFrame(self._data[-n:], self._columns)
 
-    def rows(self, *args: int) -> 'QvdDataFrame':
+    def rows(self, *args: int) -> "QvdDataFrame":
         """
         Returns the specified rows of the data frame.
 
         :param args: The rows to return.
         :return: The specified rows.
         """
         return QvdDataFrame([self._data[index] for index in args], self._columns)
@@ -234,15 +234,15 @@
 
         :param row: The row index.
         :param column: The column name.
         :return: The value at the specified row and column.
         """
         return self._data[row][self._columns.index(column)]
 
-    def select(self, *args: str) -> 'QvdDataFrame':
+    def select(self, *args: str) -> "QvdDataFrame":
         """
         Selects the specified columns from the data frame.
 
         :param args: The columns to select.
         :return: The data frame with the selected columns.
         """
         indices = [self._columns.index(arg) for arg in args]
@@ -254,23 +254,31 @@
         """
         Persists the data frame to a QVD file.
 
         :param path: The path to the QVD file.
         """
         QvdFileWriter(path, self).save()
 
+    def to_stream(self, target: BinaryIO):
+        """
+        Writes the QVD file to a binary stream.
+
+        :param target: The binary stream to write to.
+        """
+        QvdFileWriter(target, self).save()
+
     def to_dict(self) -> Dict[str, List[any]]:
         """
         Converts the data frame to a dictionary.
 
         :return: The dictionary representation of the data frame.
         """
-        return {'columns': self._columns, 'data': self._data}
+        return {"columns": self._columns, "data": self._data}
 
-    def to_pandas(self) -> 'pd.DataFrame':
+    def to_pandas(self) -> "pd.DataFrame":
         """
         Converts the data frame to a pandas data frame.
 
         :return: The pandas data frame.
         """
         try:
             import pandas as pd
@@ -286,200 +294,214 @@
         Returns a string representation of the data frame.
 
         :return: The string representation.
         """
         return tabulate(self._data, headers=self._columns)
 
     @staticmethod
-    def from_qvd(path: str) -> 'QvdDataFrame':
+    def from_qvd(path: str) -> "QvdDataFrame":
         """
         Loads a QVD file and returns its data frame.
 
         :param path: The path to the QVD file.
         :return: The data frame of the QVD file.
         """
         return QvdFileReader(path).load()
 
     @staticmethod
-    def from_dict(data: Dict[str, List[any]]) -> 'QvdDataFrame':
+    def from_dict(data: Dict[str, List[any]]) -> "QvdDataFrame":
         """
         Constructs a new QVD data frame from a dictionary.
 
         :param data: The dictionary representation of the data frame.
         :return: The QVD data frame.
         """
-        return QvdDataFrame(data['data'], data['columns'])
+        return QvdDataFrame(data["data"], data["columns"])
 
     @staticmethod
-    def from_pandas(df: 'pd.DataFrame') -> 'QvdDataFrame':
+    def from_pandas(df: "pd.DataFrame") -> "QvdDataFrame":
         """
         Constructs a new QVD data frame from a pandas data frame.
 
         :param df: The pandas data frame.
         :return: The QVD data frame.
         """
         return QvdDataFrame(df.values.tolist(), df.columns.tolist())
 
+    @staticmethod
+    def from_stream(source: BinaryIO) -> "QvdDataFrame":
+        """
+        Constructs a new QVD data frame from a stream.
+
+        :param source: The source to the QVD file.
+        """
+        return QvdFileReader(source).load()
+
 class QvdFileReader:
     """
     Parses a QVD file and loads it into memory.
     """
-    def __init__(self, path: str):
+    def __init__(self, source: Union[str, BinaryIO]):
         """
         Constructs a new QVD file parser.
 
-        :param path: The path to the QVD file.
+        :param source: The source to the QVD file.
         """
-        self._path = path
+        self._source = source
         self._buffer = None
         self._header_offset = None
         self._symbol_table_offset = None
         self._index_table_offset = None
         self._header = None
         self._symbol_table = None
         self._index_table = None
 
     def _read_data(self):
         """
         Reads the data of the QVD file into memory.
         """
-        with open(self._path, 'rb') as file:
-            self._buffer = file.read()
+        if isinstance(self._source, str):
+            with open(self._source, "rb") as file:
+                self._buffer = file.read()
+        elif isinstance(self._source, (io.RawIOBase, io.BufferedIOBase)):
+            self._buffer = self._source.read()
+        else:
+            raise ValueError("Unsupported source type. Please provide either a file path or a BinaryIO object.")
 
     def _parse_header(self):
         """
         Parses the header of the QVD file.
         """
         if not self._buffer:
-            raise ValueError('The QVD file has not been loaded in the proper order or has not been loaded at all.')
+            raise ValueError("The QVD file has not been loaded in the proper order or has not been loaded at all.")
 
-        HEADER_DELIMITER = '\r\n\0'
+        HEADER_DELIMITER = "\r\n\0"
 
         header_begin_index = 0
         header_delimiter_index = self._buffer.find(str.encode(HEADER_DELIMITER), header_begin_index)
 
         if header_delimiter_index == -1:
-            raise ValueError('The XML header section does not exist or is not properly delimited from the binary data.')
+            raise ValueError("The XML header section does not exist or is not properly delimited from the binary data.")
 
         header_end_index = header_delimiter_index + len(HEADER_DELIMITER)
         header_buffer = self._buffer[header_begin_index:header_end_index].decode()
 
         self._header = ET.fromstring(header_buffer[:-1])
 
         if self._header is None:
-            raise ValueError('The XML header could not be parsed.')
+            raise ValueError("The XML header could not be parsed.")
 
         self._header_offset = header_begin_index
         self._symbol_table_offset = header_end_index
-        self._index_table_offset = self._symbol_table_offset + int(self._header.find('./Offset').text, 10)
+        self._index_table_offset = self._symbol_table_offset + int(self._header.find("./Offset").text, 10)
 
     def _parse_symbol_table(self):
         """
         Parses the symbol table of the QVD file.
         """
         if (self._buffer is None or
             self._header is None or
             self._symbol_table_offset is None or
             self._index_table_offset is None):
-            raise ValueError('The QVD file has not been loaded in the proper order or has not been loaded at all.')
+            raise ValueError("The QVD file has not been loaded in the proper order or has not been loaded at all.")
 
-        fields = self._header.find('./Fields').findall('./QvdFieldHeader')
+        fields = self._header.find("./Fields").findall("./QvdFieldHeader")
         symbol_buffer = self._buffer[self._symbol_table_offset:self._index_table_offset]
 
         self._symbol_table = [None] * len(fields)
 
         for index, field in enumerate(fields):
-            symbols_offset = int(field.find('./Offset').text, 10)
-            symbols_length = int(field.find('./Length').text, 10)
+            symbols_offset = int(field.find("./Offset").text, 10)
+            symbols_length = int(field.find("./Length").text, 10)
 
             symbols = []
             pointer = symbols_offset
 
             while pointer < symbols_offset + symbols_length:
                 type_byte = symbol_buffer[pointer]
                 pointer += 1
 
                 if type_byte == 1:
                     byte_data = symbol_buffer[pointer:pointer + 4]
-                    value = int.from_bytes(byte_data, byteorder='little', signed=True)
+                    value = int.from_bytes(byte_data, byteorder="little", signed=True)
                     pointer += 4
                     symbols.append(QvdSymbol.from_int_value(value))
                 elif type_byte == 2:
                     byte_data = symbol_buffer[pointer:pointer + 8]
-                    value = struct.unpack('<d', byte_data)[0]
+                    value = struct.unpack("<d", byte_data)[0]
                     pointer += 8
                     symbols.append(QvdSymbol.from_double_value(value))
                 elif type_byte == 4:
-                    value = ''
+                    value = ""
 
                     while symbol_buffer[pointer] != 0:
                         value += chr(symbol_buffer[pointer])
                         pointer += 1
 
                     pointer += 1
                     symbols.append(QvdSymbol.from_string_value(value))
                 elif type_byte == 5:
                     byte_data = symbol_buffer[pointer:pointer + 4]
-                    int_value = int.from_bytes(byte_data, byteorder='little', signed=True)
+                    int_value = int.from_bytes(byte_data, byteorder="little", signed=True)
                     pointer += 4
 
-                    string_value = ''
+                    string_value = ""
                     while symbol_buffer[pointer] != 0:
                         string_value += chr(symbol_buffer[pointer])
                         pointer += 1
 
                     pointer += 1
                     symbols.append(QvdSymbol.from_dual_int_value(int_value, string_value))
                 elif type_byte == 6:
                     byte_data = symbol_buffer[pointer:pointer + 8]
-                    double_value = struct.unpack('<d', byte_data)[0]
+                    double_value = struct.unpack("<d", byte_data)[0]
                     pointer += 8
 
-                    string_value = ''
+                    string_value = ""
                     while symbol_buffer[pointer] != 0:
                         string_value += chr(symbol_buffer[pointer])
                         pointer += 1
 
                     pointer += 1
                     symbols.append(QvdSymbol.from_dual_double_value(double_value, string_value))
                 else:
-                    raise ValueError('The symbol type byte is not recognized. Unknown data type: ' + hex(type_byte))
+                    raise ValueError("The symbol type byte is not recognized. Unknown data type: " + hex(type_byte))
 
             self._symbol_table[index] = symbols
 
     def _parse_index_table(self):
         """
         Parses the index table of the QVD file.
         """
         if self._buffer is None or self._header is None or self._index_table_offset is None:
-            raise ValueError('The QVD file has not been loaded in the proper order or has not been loaded at all.')
+            raise ValueError("The QVD file has not been loaded in the proper order or has not been loaded at all.")
 
-        fields = self._header.find('./Fields').findall('./QvdFieldHeader')
-        record_size = int(self._header.find('RecordByteSize').text, 10)
-        length = int(self._header.find('Length').text, 10)
+        fields = self._header.find("./Fields").findall("./QvdFieldHeader")
+        record_size = int(self._header.find("RecordByteSize").text, 10)
+        length = int(self._header.find("Length").text, 10)
 
         index_buffer = self._buffer[self._index_table_offset:self._index_table_offset + length + 1]
         self._index_table = []
 
         pointer = 0
         while pointer < len(index_buffer):
             buffer_bytes = index_buffer[pointer:pointer + record_size]
             buffer_bytes = buffer_bytes[::-1]
-            buffer_bytes = struct.unpack('<' + 'B' * len(buffer_bytes), buffer_bytes)
+            buffer_bytes = struct.unpack("<" + "B" * len(buffer_bytes), buffer_bytes)
 
-            mask = ''.join(format(byte, '08b') for byte in buffer_bytes)
+            mask = "".join(format(byte, "08b") for byte in buffer_bytes)
             mask = mask[::-1]
             mask = [int(bit) for bit in mask]
 
             symbol_indices = []
 
             for field in fields:
-                bit_offset = int(field.find('BitOffset').text, 10)
-                bit_width = int(field.find('BitWidth').text, 10)
-                bias = int(field.find('Bias').text, 10)
+                bit_offset = int(field.find("BitOffset").text, 10)
+                bit_width = int(field.find("BitWidth").text, 10)
+                bias = int(field.find("Bias").text, 10)
 
                 if bit_width == 0:
                     symbol_index = 0
                 else:
                     symbol_index = QvdFileReader._convert_bits_to_int32(mask[bit_offset:bit_offset + bit_width])
 
                 symbol_index += bias
@@ -497,15 +519,15 @@
         self._read_data()
         self._parse_header()
         self._parse_symbol_table()
         self._parse_index_table()
 
         def _get_row(index: int) -> List[any]:
             if index >= len(self._index_table):
-                raise ValueError('Index is out of bounds')
+                raise ValueError("Index is out of bounds")
 
             row = [None] * len(self._symbol_table)
 
             for field_index, symbol_index in enumerate(self._index_table[index]):
                 if symbol_index < 0:
                     row[field_index] = None
                 else:
@@ -521,15 +543,15 @@
                                 pass
 
                     row[field_index] = symbol
 
             return row
 
         data = [_get_row(index) for index in range(len(self._index_table))]
-        columns = [field.find('FieldName').text for field in self._header.find('./Fields').findall('./QvdFieldHeader')]
+        columns = [field.find("FieldName").text for field in self._header.find("./Fields").findall("./QvdFieldHeader")]
 
         return QvdDataFrame(data, columns)
 
     @staticmethod
     def _convert_bits_to_int32(bits: List[int]) -> int:
         """
         Converts a list of bits to an integer.
@@ -539,235 +561,243 @@
 
         return sum(bit * (2 ** index) for index, bit in enumerate(bits))
 
 class QvdFileWriter:
     """
     Persists a QVD file to disk.
     """
-    def __init__(self, path: str, df: QvdDataFrame):
+    def __init__(self, target: Union[str, BinaryIO], df: QvdDataFrame):
         """
         Constructs a new QVD file writer.
 
-        :param path: The path to the QVD file.
+        :param target: The destination to which the Qvd file should be written.
         :param df: The data to persist.
         """
-        self._path = path
+        self._target = target
         self._df = df
         self._header = None
         self._symbol_buffer = None
         self._symbol_table = None
         self._symbol_table_metadata = None
         self._index_buffer = None
         self._index_table = None
         self._index_table_metadata = None
         self._record_byte_size = None
 
     def _write_data(self):
         """
         Writes the data to the QVD file.
         """
-        with open(self._path, 'wb') as file:
-            file.write(self._header.encode())
-            file.write(b'\0')
-            file.write(self._symbol_buffer)
-            file.write(self._index_buffer)
+        if isinstance(self._target, str):
+            with open(self._target, "wb") as file:
+                file.write(self._header.encode())
+                file.write(b"\0")
+                file.write(self._symbol_buffer)
+                file.write(self._index_buffer)
+        elif isinstance(self._target, (io.RawIOBase, io.BufferedIOBase)):
+            self._target.write(self._header.encode())
+            self._target.write(b"\0")
+            self._target.write(self._symbol_buffer)
+            self._target.write(self._index_buffer)
+        else:
+            raise ValueError("Unsupported target type. Please provide either a file path or a BinaryIO object.")
 
     def _build_header(self):
         """
         Builds the XML header of the QVD file.
         """
 
         doc = minidom.Document()
 
-        header_element = doc.createElement('QvdTableHeader')
+        header_element = doc.createElement("QvdTableHeader")
 
         # The following fields before the field definitions are undocumented and Qlik Sense specific. These fields
         # seems to be not technically necessary for parsing a QVD file, but are mandatory for Qlik Sense to recognize
         # the QVD file as a valid QVD file. Hence, some of these fields are hardcoded and some are generated randomly.
 
-        qv_build_no_element = doc.createElement('QvBuildNo')
-        qv_build_no_element.appendChild(doc.createTextNode('50667'))
+        qv_build_no_element = doc.createElement("QvBuildNo")
+        qv_build_no_element.appendChild(doc.createTextNode("50667"))
         header_element.appendChild(qv_build_no_element)
 
-        creator_doc_element = doc.createElement('CreatorDoc')
+        creator_doc_element = doc.createElement("CreatorDoc")
         creator_doc_element.appendChild(doc.createTextNode(str(uuid.uuid4())))
         header_element.appendChild(creator_doc_element)
 
-        create_utc_time_element = doc.createElement('CreateUtcTime')
-        create_utc_time_element.appendChild(doc.createTextNode(time.strftime('%Y-%m-%d %H:%M:%S', time.gmtime())))
+        create_utc_time_element = doc.createElement("CreateUtcTime")
+        create_utc_time_element.appendChild(doc.createTextNode(time.strftime("%Y-%m-%d %H:%M:%S", time.gmtime())))
         header_element.appendChild(create_utc_time_element)
 
-        source_create_utc_time_element = doc.createElement('SourceCreateUtcTime')
-        source_create_utc_time_element.appendChild(doc.createTextNode(''))
+        source_create_utc_time_element = doc.createElement("SourceCreateUtcTime")
+        source_create_utc_time_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(source_create_utc_time_element)
 
-        source_file_utc_time_element = doc.createElement('SourceFileUtcTime')
-        source_file_utc_time_element.appendChild(doc.createTextNode(''))
+        source_file_utc_time_element = doc.createElement("SourceFileUtcTime")
+        source_file_utc_time_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(source_file_utc_time_element)
 
-        source_file_size_element = doc.createElement('SourceFileSize')
-        source_file_size_element.appendChild(doc.createTextNode('-1'))
+        source_file_size_element = doc.createElement("SourceFileSize")
+        source_file_size_element.appendChild(doc.createTextNode("-1"))
         header_element.appendChild(source_file_size_element)
 
-        stale_utc_time_element = doc.createElement('StaleUtcTime')
-        stale_utc_time_element.appendChild(doc.createTextNode(''))
+        stale_utc_time_element = doc.createElement("StaleUtcTime")
+        stale_utc_time_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(stale_utc_time_element)
 
-        table_name_element = doc.createElement('TableName')
-        table_name_element.appendChild(doc.createTextNode(os.path.splitext(os.path.basename(self._path))[0]))
+        table_name_element = doc.createElement("TableName")
+        table_name_element.appendChild(doc.createTextNode("DATA"))
         header_element.appendChild(table_name_element)
 
-        fields_element = doc.createElement('Fields')
+        fields_element = doc.createElement("Fields")
 
         for column_index, column_name in enumerate(self._df.columns):
-            field_element = doc.createElement('QvdFieldHeader')
+            field_element = doc.createElement("QvdFieldHeader")
 
-            field_name_element = doc.createElement('FieldName')
+            field_name_element = doc.createElement("FieldName")
             field_name_element.appendChild(doc.createTextNode(column_name))
             field_element.appendChild(field_name_element)
 
-            bit_offset_element = doc.createElement('BitOffset')
+            bit_offset_element = doc.createElement("BitOffset")
             bit_offset_element.appendChild(doc.createTextNode(str(self._index_table_metadata[column_index][0])))
             field_element.appendChild(bit_offset_element)
 
-            bit_width_element = doc.createElement('BitWidth')
+            bit_width_element = doc.createElement("BitWidth")
             bit_width_element.appendChild(doc.createTextNode(str(self._index_table_metadata[column_index][1])))
             field_element.appendChild(bit_width_element)
 
-            bias_element = doc.createElement('Bias')
+            bias_element = doc.createElement("Bias")
             bias_element.appendChild(doc.createTextNode(str(self._index_table_metadata[column_index][2])))
             field_element.appendChild(bias_element)
 
-            no_of_symbols_element = doc.createElement('NoOfSymbols')
+            no_of_symbols_element = doc.createElement("NoOfSymbols")
             no_of_symbols_element.appendChild(doc.createTextNode(str(len(self._symbol_table[column_index]))))
             field_element.appendChild(no_of_symbols_element)
 
-            offset_element = doc.createElement('Offset')
+            offset_element = doc.createElement("Offset")
             offset_element.appendChild(doc.createTextNode(str(self._symbol_table_metadata[column_index][0])))
             field_element.appendChild(offset_element)
 
-            length_element = doc.createElement('Length')
+            length_element = doc.createElement("Length")
             length_element.appendChild(doc.createTextNode(str(self._symbol_table_metadata[column_index][1])))
             field_element.appendChild(length_element)
 
-            comment_element = doc.createElement('Comment')
-            comment_element.appendChild(doc.createTextNode(''))
+            comment_element = doc.createElement("Comment")
+            comment_element.appendChild(doc.createTextNode(""))
             field_element.appendChild(comment_element)
 
-            number_format_element = doc.createElement('NumberFormat')
+            number_format_element = doc.createElement("NumberFormat")
 
-            number_format_type_element = doc.createElement('Type')
-            number_format_type_element.appendChild(doc.createTextNode('UNKNOWN'))
+            number_format_type_element = doc.createElement("Type")
+            number_format_type_element.appendChild(doc.createTextNode("UNKNOWN"))
             number_format_element.appendChild(number_format_type_element)
 
-            number_format_n_dec_element = doc.createElement('nDec')
-            number_format_n_dec_element.appendChild(doc.createTextNode('0'))
+            number_format_n_dec_element = doc.createElement("nDec")
+            number_format_n_dec_element.appendChild(doc.createTextNode("0"))
             number_format_element.appendChild(number_format_n_dec_element)
 
-            number_format_use_thou_element = doc.createElement('UseThou')
-            number_format_use_thou_element.appendChild(doc.createTextNode('0'))
+            number_format_use_thou_element = doc.createElement("UseThou")
+            number_format_use_thou_element.appendChild(doc.createTextNode("0"))
             number_format_element.appendChild(number_format_use_thou_element)
 
-            number_format_fmt_element = doc.createElement('Fmt')
-            number_format_fmt_element.appendChild(doc.createTextNode(''))
+            number_format_fmt_element = doc.createElement("Fmt")
+            number_format_fmt_element.appendChild(doc.createTextNode(""))
             number_format_element.appendChild(number_format_fmt_element)
 
-            number_format_dec_element = doc.createElement('Dec')
-            number_format_dec_element.appendChild(doc.createTextNode(''))
+            number_format_dec_element = doc.createElement("Dec")
+            number_format_dec_element.appendChild(doc.createTextNode(""))
             number_format_element.appendChild(number_format_dec_element)
 
-            number_format_thou_element = doc.createElement('Thou')
-            number_format_thou_element.appendChild(doc.createTextNode(''))
+            number_format_thou_element = doc.createElement("Thou")
+            number_format_thou_element.appendChild(doc.createTextNode(""))
             number_format_element.appendChild(number_format_thou_element)
 
             field_element.appendChild(number_format_element)
 
-            tags_element = doc.createElement('Tags')
+            tags_element = doc.createElement("Tags")
             field_element.appendChild(tags_element)
 
             fields_element.appendChild(field_element)
 
         header_element.appendChild(fields_element)
 
-        record_byte_size_element = doc.createElement('RecordByteSize')
+        record_byte_size_element = doc.createElement("RecordByteSize")
         record_byte_size_element.appendChild(doc.createTextNode(str(self._record_byte_size)))
         header_element.appendChild(record_byte_size_element)
 
-        no_of_records_element = doc.createElement('NoOfRecords')
+        no_of_records_element = doc.createElement("NoOfRecords")
         no_of_records_element.appendChild(doc.createTextNode(str(len(self._df.data))))
         header_element.appendChild(no_of_records_element)
 
-        offset_element = doc.createElement('Offset')
+        offset_element = doc.createElement("Offset")
         offset_element.appendChild(doc.createTextNode(str(self._symbol_table_metadata[-1][0] +
                                                           self._symbol_table_metadata[-1][1])))
         header_element.appendChild(offset_element)
 
-        length_element = doc.createElement('Length')
+        length_element = doc.createElement("Length")
         length_element.appendChild(doc.createTextNode(str(len(self._index_buffer))))
         header_element.appendChild(length_element)
 
-        compression_element = doc.createElement('Compression')
-        compression_element.appendChild(doc.createTextNode(''))
+        compression_element = doc.createElement("Compression")
+        compression_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(compression_element)
 
-        comment_element = doc.createElement('Comment')
-        comment_element.appendChild(doc.createTextNode(''))
+        comment_element = doc.createElement("Comment")
+        comment_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(comment_element)
 
-        encryption_info_element = doc.createElement('EncryptionInfo')
-        encryption_info_element.appendChild(doc.createTextNode(''))
+        encryption_info_element = doc.createElement("EncryptionInfo")
+        encryption_info_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(encryption_info_element)
 
-        table_tags_element = doc.createElement('TableTags')
-        table_tags_element.appendChild(doc.createTextNode(''))
+        table_tags_element = doc.createElement("TableTags")
+        table_tags_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(table_tags_element)
 
-        profiling_data_element = doc.createElement('ProfilingData')
-        profiling_data_element.appendChild(doc.createTextNode(''))
+        profiling_data_element = doc.createElement("ProfilingData")
+        profiling_data_element.appendChild(doc.createTextNode(""))
         header_element.appendChild(profiling_data_element)
 
-        lineage_element = doc.createElement('Lineage')
+        lineage_element = doc.createElement("Lineage")
 
-        lineage_info_element = doc.createElement('LineageInfo')
+        lineage_info_element = doc.createElement("LineageInfo")
 
-        discriminator_element = doc.createElement('Discriminator')
-        discriminator_element.appendChild(doc.createTextNode('INLINE;'))
+        discriminator_element = doc.createElement("Discriminator")
+        discriminator_element.appendChild(doc.createTextNode("INLINE;"))
         lineage_info_element.appendChild(discriminator_element)
 
-        statement_element = doc.createElement('Statement')
-        statement_element.appendChild(doc.createTextNode(''))
+        statement_element = doc.createElement("Statement")
+        statement_element.appendChild(doc.createTextNode(""))
         lineage_info_element.appendChild(statement_element)
 
         lineage_element.appendChild(lineage_info_element)
 
         header_element.appendChild(lineage_element)
 
         doc.appendChild(header_element)
 
-        self._header = doc.toprettyxml(indent="  ", encoding='utf-8', standalone=True, newl='\r\n').decode()
-        self._header = ' '.join([line + '\r\n' for line in self._header.splitlines() if line.strip()])
+        self._header = doc.toprettyxml(indent="  ", encoding="utf-8", standalone=True, newl="\r\n").decode()
+        self._header = " ".join([line + "\r\n" for line in self._header.splitlines() if line.strip()])
 
     def _build_symbol_table(self):
         """
         Builds the symbol table of the QVD file.
         """
 
         self._symbol_table = [None] * len(self._df.columns)
         self._symbol_table_metadata = [None] * len(self._df.columns)
-        self._symbol_buffer = b''
+        self._symbol_buffer = b""
 
         for column_index, _ in enumerate(self._df.columns):
             unique_values = QvdFileWriter._get_unique_values([row[column_index] for row in self._df.data])
 
             symbols = []
 
             for value in unique_values:
                 symbols.append(self._convert_raw_to_symbol(value))
 
-            current_symbol_buffer = b''.join([symbol.to_byte_representation() for symbol in symbols])
+            current_symbol_buffer = b"".join([symbol.to_byte_representation() for symbol in symbols])
             self._symbol_buffer += current_symbol_buffer
 
             symbols_length = len(current_symbol_buffer)
             symbols_offset = sum([self._symbol_table_metadata[index][1] for index in range(column_index)])
 
             self._symbol_table_metadata[column_index] = (symbols_offset, symbols_length)
             self._symbol_table[column_index] = symbols
@@ -775,15 +805,15 @@
     def _build_index_table(self):
         """
         Builds the index table of the QVD file.
         """
 
         self._index_table = [None] * len(self._df.data)
         self._index_table_metadata = [None] * len(self._df.columns)
-        self._index_buffer = b''
+        self._index_buffer = b""
 
         # Each row in the index table is represented by one or more bytes, the number of bytes used to represent a
         # row is the so called record byte size. These bytes are used to store the indices of the symbols in the symbol
         # table for each row. Therefore, the value indices of a row are concatenated in a binary representation in
         # the order of the columns of the data frame.
         #
         # Let's assume the flowing data frame and the corresponding symbol table:
@@ -832,16 +862,16 @@
                 symbol = self._convert_raw_to_symbol(value)
                 symbol_index = self._symbol_table[column_index].index(symbol)
                 indices[column_index] = symbol_index
 
             # Convert the integer indices to binary representation
             for index_index, index in enumerate(indices):
                 bits = self._convert_int32_to_bits(index, 8)
-                bits = ''.join([str(bit) for bit in bits])
-                bits = bits.lstrip('0') or '0'
+                bits = "".join([str(bit) for bit in bits])
+                bits = bits.lstrip("0") or "0"
                 indices[index_index] = bits
 
             self._index_table[row_index] = indices
 
         # Normalize the bit representation of the indices by padding with zeros
         for column_index, _ in enumerate(self._df.columns):
             # Bit offset is the sum of the bit widths of all previous columns
@@ -850,24 +880,24 @@
             # Bit width is the maximum bit width of all indices of the column
             bit_width = max([len(bit_indices[column_index]) for bit_indices in self._index_table])
             bias = 0
             self._index_table_metadata[column_index] = (bit_offset, bit_width, bias)
 
             # Pad the bit representation of the indices with zeros to match the bit width
             for bit_indices in self._index_table:
-                bit_indices[column_index] = bit_indices[column_index].rjust(bit_width, '0')
+                bit_indices[column_index] = bit_indices[column_index].rjust(bit_width, "0")
 
         # Concatenate the bit representation of the indices of each row to a single binary string per row
         for bit_indices in self._index_table:
             bit_indices = bit_indices[::-1]
-            bits = ''.join(bit_indices)
+            bits = "".join(bit_indices)
             padding_width = (8 - len(bits) % 8) % 8
-            padded_bits = '0' * padding_width + bits
+            padded_bits = "0" * padding_width + bits
             byte_values = [int(padded_bits[index:index + 8], 2) for index in range(0, len(padded_bits), 8)]
-            byte_representation = struct.pack('<' + 'B' * len(byte_values), *byte_values)
+            byte_representation = struct.pack("<" + "B" * len(byte_values), *byte_values)
             byte_representation = byte_representation[::-1]
 
             self._index_buffer += byte_representation
 
         self._record_byte_size = len(self._index_buffer) // len(self._df.data)
 
     def _convert_raw_to_symbol(self, raw: any) -> QvdSymbol:
@@ -893,15 +923,15 @@
         """
         Converts an integer to a list of bits.
 
         :param value: The integer value.
         :param width: The width of the bits.
         :return: The list of bits.
         """
-        return [int(bit) for bit in format(value, '0' + str(width) + 'b')]
+        return [int(bit) for bit in format(value, "0" + str(width) + "b")]
 
     @staticmethod
     def _get_unique_values(values: List[any]) -> List[any]:
         """
         Determines the unique values of a given list.
         """
         unique_values = []
```

