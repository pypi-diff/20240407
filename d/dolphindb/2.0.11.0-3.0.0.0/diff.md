# Comparing `tmp/dolphindb-2.0.11.0-cp39-cp39-win_amd64.whl.zip` & `tmp/dolphindb-3.0.0.0-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,23 @@
-Zip file size: 1593472 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat     1933 b- defN 24-Jan-16 10:01 dolphindb/__init__.py
--rw-rw-rw-  2.0 fat  4129280 b- defN 24-Jan-30 03:32 dolphindb/_dolphindbcpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     6490 b- defN 23-Oct-12 02:33 dolphindb/database.py
--rw-rw-rw-  2.0 fat    68243 b- defN 24-Jan-29 01:04 dolphindb/session.py
--rw-rw-rw-  2.0 fat     4821 b- defN 23-Nov-23 01:44 dolphindb/settings.py
--rw-rw-rw-  2.0 fat    86085 b- defN 24-Jan-29 02:52 dolphindb/table.py
--rw-rw-rw-  2.0 fat     1216 b- defN 24-Jan-25 09:38 dolphindb/utils.py
--rw-rw-rw-  2.0 fat     7146 b- defN 24-Jan-11 01:35 dolphindb/vector.py
--rw-rw-rw-  2.0 fat    11596 b- defN 24-Jan-30 03:32 dolphindb-2.0.11.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1841 b- defN 24-Jan-30 03:32 dolphindb-2.0.11.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Jan-30 03:32 dolphindb-2.0.11.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 24-Jan-30 03:32 dolphindb-2.0.11.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1054 b- defN 24-Jan-30 03:32 dolphindb-2.0.11.0.dist-info/RECORD
-13 files, 4319815 bytes uncompressed, 1591734 bytes compressed:  63.2%
+Zip file size: 2052663 bytes, number of entries: 21
+drwxr-x---  2.0 unx        0 b- stor 24-Apr-01 06:19 dolphindb/
+drwxr-x---  2.0 unx        0 b- stor 24-Apr-01 06:19 dolphindb-3.0.0.0.dist-info/
+drwxr-x---  2.0 unx        0 b- stor 24-Apr-01 06:19 dolphindb.libs/
+drwxr-x---  2.0 unx        0 b- stor 24-Apr-01 06:19 dolphindb/_core/
+-rw-r-----  2.0 unx     1869 b- defN 24-Apr-01 06:19 dolphindb/__init__.py
+-rwxr-x---  2.0 unx  5876936 b- defN 24-Apr-01 06:19 dolphindb/_dolphindbcpp.cpython-311-aarch64-linux-gnu.so
+-rw-r-----  2.0 unx    11790 b- defN 24-Apr-01 06:19 dolphindb/cep.py
+-rw-r-----  2.0 unx     6353 b- defN 24-Apr-01 06:19 dolphindb/database.py
+-rw-r-----  2.0 unx    67757 b- defN 24-Apr-01 06:19 dolphindb/session.py
+-rw-r-----  2.0 unx     4598 b- defN 24-Apr-01 06:19 dolphindb/settings.py
+-rw-r-----  2.0 unx    83703 b- defN 24-Apr-01 06:19 dolphindb/table.py
+-rw-r-----  2.0 unx     3406 b- defN 24-Apr-01 06:19 dolphindb/typing.py
+-rw-r-----  2.0 unx     1167 b- defN 24-Apr-01 06:19 dolphindb/utils.py
+-rw-r-----  2.0 unx     6912 b- defN 24-Apr-01 06:19 dolphindb/vector.py
+-rw-r-----  2.0 unx      527 b- defN 24-Apr-01 06:19 dolphindb/_core/__init__.py
+-rw-------  2.0 unx    11392 b- defN 24-Apr-01 06:19 dolphindb-3.0.0.0.dist-info/LICENSE
+-rw-r-----  2.0 unx     1770 b- defN 24-Apr-01 06:19 dolphindb-3.0.0.0.dist-info/METADATA
+-rw-r-----  2.0 unx      154 b- defN 24-Apr-01 06:19 dolphindb-3.0.0.0.dist-info/WHEEL
+-rw-r-----  2.0 unx       10 b- defN 24-Apr-01 06:19 dolphindb-3.0.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1412 b- defN 24-Apr-01 06:19 dolphindb-3.0.0.0.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   132048 b- defN 24-Apr-01 06:19 dolphindb.libs/libuuid-330f215f.so.1.3.0
+21 files, 6211804 bytes uncompressed, 2049957 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -1,40 +1,64 @@
+Filename: dolphindb/
+Comment: 
+
+Filename: dolphindb-3.0.0.0.dist-info/
+Comment: 
+
+Filename: dolphindb.libs/
+Comment: 
+
+Filename: dolphindb/_core/
+Comment: 
+
 Filename: dolphindb/__init__.py
 Comment: 
 
-Filename: dolphindb/_dolphindbcpp.cp39-win_amd64.pyd
+Filename: dolphindb/_dolphindbcpp.cpython-311-aarch64-linux-gnu.so
+Comment: 
+
+Filename: dolphindb/cep.py
 Comment: 
 
 Filename: dolphindb/database.py
 Comment: 
 
 Filename: dolphindb/session.py
 Comment: 
 
 Filename: dolphindb/settings.py
 Comment: 
 
 Filename: dolphindb/table.py
 Comment: 
 
+Filename: dolphindb/typing.py
+Comment: 
+
 Filename: dolphindb/utils.py
 Comment: 
 
 Filename: dolphindb/vector.py
 Comment: 
 
-Filename: dolphindb-2.0.11.0.dist-info/LICENSE
+Filename: dolphindb/_core/__init__.py
+Comment: 
+
+Filename: dolphindb-3.0.0.0.dist-info/LICENSE
+Comment: 
+
+Filename: dolphindb-3.0.0.0.dist-info/METADATA
 Comment: 
 
-Filename: dolphindb-2.0.11.0.dist-info/METADATA
+Filename: dolphindb-3.0.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: dolphindb-2.0.11.0.dist-info/WHEEL
+Filename: dolphindb-3.0.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dolphindb-2.0.11.0.dist-info/top_level.txt
+Filename: dolphindb-3.0.0.0.dist-info/RECORD
 Comment: 
 
-Filename: dolphindb-2.0.11.0.dist-info/RECORD
+Filename: dolphindb.libs/libuuid-330f215f.so.1.3.0
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## dolphindb/__init__.py

```diff
@@ -1,74 +1,75 @@
-from .session import Session
-from .session import Session as session
-from .session import DBConnectionPool
-from .session import BlockReader
-from .session import PartitionedTableAppender
-from .session import TableAppender
-from .session import TableAppender as tableAppender
-from .session import TableUpserter
-from .session import TableUpserter as tableUpsert
-from .session import BatchTableWriter
-from .session import MultithreadedTableWriter
-from .session import MultithreadedTableWriterStatus
-from .session import MultithreadedTableWriterThreadStatus
-from .session import streamDeserializer
-from .table import Table, TableUpdate, TableDelete, TableGroupby, TablePivotBy, TableContextby, Counter
-from .table import wavg, wsum, covar, corr, count, max, min, sum, sum2, size, avg, std, prod, var, first, last
-from .table import eachPre, cumsum, cumprod, cummax, cummin
-from .vector import Vector, FilterCond
-from .database import Database
-from .utils import month
-
-__version__ = "2.0.11.0"
-
-name = "dolphindb"
-
-__all__ = [
-    "Session", "session",
-    "DBConnectionPool",
-    "BlockReader",
-    "PartitionedTableAppender",
-    "TableAppender", "tableAppender",
-    "TableUpserter", "tableUpsert",
-    "BatchTableWriter",
-    "MultithreadedTableWriter",
-    "MultithreadedTableWriterStatus",
-    "MultithreadedTableWriterThreadStatus",
-    "streamDeserializer",
-    "Table",
-    "TableUpdate",
-    "TableDelete",
-    "TableGroupby",
-    "TablePivotBy",
-    "TableContextby",
-    "Counter",
-    "Vector",
-    "FilterCond",
-    "Database",
-    "month",
-    "settings",
-    "__version__",
-    "name",
-
-    "wavg",
-    "wsum",
-    "covar",
-    "corr",
-    "count",
-    "max",
-    "min",
-    "sum",
-    "sum2",
-    "size",
-    "avg",
-    "std",
-    "prod",
-    "var",
-    "first",
-    "last",
-    "eachPre",
-    "cumsum",
-    "cumprod",
-    "cummax",
-    "cummin"
-]
+from .session import Session
+from .session import Session as session
+from .session import DBConnectionPool
+from .session import BlockReader
+from .session import PartitionedTableAppender
+from .session import TableAppender
+from .session import TableAppender as tableAppender
+from .session import TableUpserter
+from .session import TableUpserter as tableUpsert
+from .session import BatchTableWriter
+from .session import MultithreadedTableWriter
+from .session import MultithreadedTableWriterStatus
+from .session import MultithreadedTableWriterThreadStatus
+from .session import streamDeserializer
+from .table import Table, TableUpdate, TableDelete, TableGroupby, TablePivotBy, TableContextby, Counter
+from .table import wavg, wsum, covar, corr, count, max, min, sum, sum2, size, avg, std, prod, var, first, last
+from .table import eachPre, cumsum, cumprod, cummax, cummin
+from .vector import Vector, FilterCond
+from .database import Database
+from .utils import month
+
+__version__ = "3.0.0.0"
+
+name = "dolphindb"
+
+__all__ = [
+    "Session", "session",
+    "DBConnectionPool",
+    "BlockReader",
+    "PartitionedTableAppender",
+    "TableAppender", "tableAppender",
+    "TableUpserter", "tableUpsert",
+    "BatchTableWriter",
+    "MultithreadedTableWriter",
+    "MultithreadedTableWriterStatus",
+    "MultithreadedTableWriterThreadStatus",
+    "streamDeserializer",
+    "Table",
+    "TableUpdate",
+    "TableDelete",
+    "TableGroupby",
+    "TablePivotBy",
+    "TableContextby",
+    "Counter",
+    "Vector",
+    "FilterCond",
+    "Database",
+    "month",
+    "settings",
+    "__version__",
+    "name",
+    "cep",
+
+    "wavg",
+    "wsum",
+    "covar",
+    "corr",
+    "count",
+    "max",
+    "min",
+    "sum",
+    "sum2",
+    "size",
+    "avg",
+    "std",
+    "prod",
+    "var",
+    "first",
+    "last",
+    "eachPre",
+    "cumsum",
+    "cumprod",
+    "cummax",
+    "cummin"
+]
```

## dolphindb/database.py

 * *Ordering differences only*

```diff
@@ -1,137 +1,137 @@
-from typing import Dict, List, Union
-
-from dolphindb.table import Table
-from dolphindb.utils import _generate_tablename
-
-
-class Database(object):
-    """DolphinDB database objects.
-
-    Args:
-        dbName : database name. Defaults to None.
-        s : connected Session object. Defaults to None.
-    """
-
-    def __init__(self, dbName: str, s):
-        """Constructor of Database."""
-        self.__dbName = dbName
-        self.__session = s
-
-    def _getDbName(self):
-        return self.__dbName
-
-    def createTable(
-        self, table: Table, tableName: str,
-        sortColumns: Union[str, List[str]] = None
-    ) -> Table:
-        """Create an empty dimension table based on the given schema.
-
-        Args:
-            table : a table. DolphinDB server will create an empty dimension table based on the schema of the passed table.
-            tableName : name of the dimension table.
-            sortColumns : string or a list of strings, indicating the sort column of a table. If specified, data with the same key are stored together in a partition in order. Defaults to None.
-
-        Returns:
-            DolphinDB Table object.
-        """
-        if not isinstance(table, Table):
-            raise RuntimeError("Only DolphinDB Table object is accepted")
-
-        tHandle = table._getTableName()
-        ctHandle = _generate_tablename()
-        runstr = ctHandle + "=" + self.__dbName + ".createTable(" + tHandle + "," + "`" + tableName
-
-        if sortColumns is not None:
-            if type(sortColumns) == str:
-                runstr += ",sortColumns=`"+sortColumns
-            elif type(sortColumns) == list:
-                runstr += ",sortColumns="
-                for key in sortColumns:
-                    runstr += "`"+key
-
-        runstr += ");"
-
-        self.__session.run(runstr)
-        return self.__session.loadTable(ctHandle)
-
-    def createPartitionedTable(
-            self, table: Table, tableName: str, partitionColumns: Union[str, List[str]],
-            compressMethods: Dict[str, str] = {}, sortColumns: Union[str, List[str]] = None,
-            keepDuplicates: str = None, sortKeyMappingFunction: Union[str, List[str]] = None
-            ) -> Table:
-        """Create an empty dimension table based on the given schema.
-
-        Args:
-            table : a table. DolphinDB server will create an empty dimension table based on the schema of the passed table.
-            tableName : name of the dimension table.
-            partitionColumns : string or list of strings indicating the partition columns. For a compo domain database, it is a string; for non-sequential domain, this parameter is required.
-            compressMethods : a list of the compression methods used for each column. If unspecified, the columns are not compressed. Defaults to {}.
-            sortColumns : string or a list of strings, indicating the sort column of a table. If specified, data with the same key are stored together in a partition in order. Defaults to None.
-            keepDuplicates : how to deal with records with duplicate sortColumns values. 
-                                  It can have the following values:
-                                  | Value   | Meanings                   |
-                                  | :----   | :----                      |
-                                  | "ALL"   | keep all records           |
-                                  | "LAST"  | only keep the last record  |
-                                  | "FIRST" | only keep the first record |
-            sortKeyMappingFunction : a vector of functions, which is of the same length as sortKey. 
-                                     The specified mapping functions are applied to each sort columns (except the temporal column) so as to reduce the dimensionality of sort keys.
-
-        Returns:
-            DolphinDB Table object.
-        """
-        if not isinstance(table, Table):
-            raise RuntimeError("Only DolphinDB Table object is accepted")
-
-        tHandle = table._getTableName()
-        cptHandle = _generate_tablename()
-
-        partitionColumns_str = ''
-        if type(partitionColumns) == str:
-            partitionColumns_str = "`" + partitionColumns
-        elif type(partitionColumns) == list:
-            for col in partitionColumns:
-                partitionColumns_str += '`'
-                partitionColumns_str += col
-        else:
-            raise RuntimeError("Only String or List of String is accepted for partitionColumns")
-
-        runstr = cptHandle + "=" + self.__dbName + ".createPartitionedTable(" + tHandle + "," + "`" + tableName + ","  + partitionColumns_str
-
-        if len(compressMethods) > 0:
-            runstr += ",compressMethods={"
-            for key, value in compressMethods.items():
-                runstr += key+":'"+value+"',"
-            runstr = runstr[:-1]+"}"
-        if sortColumns is not None:
-            if type(sortColumns) == str:
-                runstr += ",sortColumns=`"+sortColumns
-            elif type(sortColumns) == list:
-                runstr += ",sortColumns="
-                for key in sortColumns:
-                    runstr += "`"+key
-
-        if keepDuplicates is not None:
-            if isinstance(keepDuplicates, str):
-                runstr += ",keepDuplicates="+keepDuplicates
-            else:
-                raise RuntimeError("Only str is accepted for keepDuplicates")
-
-        if sortKeyMappingFunction is not None:
-            if type(sortKeyMappingFunction) == str:
-                runstr += ",sortKeyMappingFunction=["+sortKeyMappingFunction+"]"
-            elif type(sortKeyMappingFunction) == list:
-                runstr += ",sortKeyMappingFunction=["
-                for i in range(len(sortKeyMappingFunction)):
-                    if i != 0:
-                        runstr += ","
-                    if type(sortKeyMappingFunction[i]) == str:
-                        runstr += sortKeyMappingFunction[i]
-                    else:
-                        raise RuntimeError('The "sortKeyMappingFunction" parameter must be a string or a list of strings.')
-                runstr += "]"
-            else:
-                raise RuntimeError('The "sortKeyMappingFunction" parameter must be a string or a list of strings.')
-        runstr += ");"
-        self.__session.run(runstr)
-        return self.__session.loadTable(cptHandle)
+from typing import Dict, List, Union
+
+from dolphindb.table import Table
+from dolphindb.utils import _generate_tablename
+
+
+class Database(object):
+    """DolphinDB database objects.
+
+    Args:
+        dbName : database name. Defaults to None.
+        s : connected Session object. Defaults to None.
+    """
+
+    def __init__(self, dbName: str, s):
+        """Constructor of Database."""
+        self.__dbName = dbName
+        self.__session = s
+
+    def _getDbName(self):
+        return self.__dbName
+
+    def createTable(
+        self, table: Table, tableName: str,
+        sortColumns: Union[str, List[str]] = None
+    ) -> Table:
+        """Create an empty dimension table based on the given schema.
+
+        Args:
+            table : a table. DolphinDB server will create an empty dimension table based on the schema of the passed table.
+            tableName : name of the dimension table.
+            sortColumns : string or a list of strings, indicating the sort column of a table. If specified, data with the same key are stored together in a partition in order. Defaults to None.
+
+        Returns:
+            DolphinDB Table object.
+        """
+        if not isinstance(table, Table):
+            raise RuntimeError("Only DolphinDB Table object is accepted")
+
+        tHandle = table._getTableName()
+        ctHandle = _generate_tablename()
+        runstr = ctHandle + "=" + self.__dbName + ".createTable(" + tHandle + "," + "`" + tableName
+
+        if sortColumns is not None:
+            if type(sortColumns) == str:
+                runstr += ",sortColumns=`"+sortColumns
+            elif type(sortColumns) == list:
+                runstr += ",sortColumns="
+                for key in sortColumns:
+                    runstr += "`"+key
+
+        runstr += ");"
+
+        self.__session.run(runstr)
+        return self.__session.loadTable(ctHandle)
+
+    def createPartitionedTable(
+            self, table: Table, tableName: str, partitionColumns: Union[str, List[str]],
+            compressMethods: Dict[str, str] = {}, sortColumns: Union[str, List[str]] = None,
+            keepDuplicates: str = None, sortKeyMappingFunction: Union[str, List[str]] = None
+            ) -> Table:
+        """Create an empty dimension table based on the given schema.
+
+        Args:
+            table : a table. DolphinDB server will create an empty dimension table based on the schema of the passed table.
+            tableName : name of the dimension table.
+            partitionColumns : string or list of strings indicating the partition columns. For a compo domain database, it is a string; for non-sequential domain, this parameter is required.
+            compressMethods : a list of the compression methods used for each column. If unspecified, the columns are not compressed. Defaults to {}.
+            sortColumns : string or a list of strings, indicating the sort column of a table. If specified, data with the same key are stored together in a partition in order. Defaults to None.
+            keepDuplicates : how to deal with records with duplicate sortColumns values. 
+                                  It can have the following values:
+                                  | Value   | Meanings                   |
+                                  | :----   | :----                      |
+                                  | "ALL"   | keep all records           |
+                                  | "LAST"  | only keep the last record  |
+                                  | "FIRST" | only keep the first record |
+            sortKeyMappingFunction : a vector of functions, which is of the same length as sortKey. 
+                                     The specified mapping functions are applied to each sort columns (except the temporal column) so as to reduce the dimensionality of sort keys.
+
+        Returns:
+            DolphinDB Table object.
+        """
+        if not isinstance(table, Table):
+            raise RuntimeError("Only DolphinDB Table object is accepted")
+
+        tHandle = table._getTableName()
+        cptHandle = _generate_tablename()
+
+        partitionColumns_str = ''
+        if type(partitionColumns) == str:
+            partitionColumns_str = "`" + partitionColumns
+        elif type(partitionColumns) == list:
+            for col in partitionColumns:
+                partitionColumns_str += '`'
+                partitionColumns_str += col
+        else:
+            raise RuntimeError("Only String or List of String is accepted for partitionColumns")
+
+        runstr = cptHandle + "=" + self.__dbName + ".createPartitionedTable(" + tHandle + "," + "`" + tableName + ","  + partitionColumns_str
+
+        if len(compressMethods) > 0:
+            runstr += ",compressMethods={"
+            for key, value in compressMethods.items():
+                runstr += key+":'"+value+"',"
+            runstr = runstr[:-1]+"}"
+        if sortColumns is not None:
+            if type(sortColumns) == str:
+                runstr += ",sortColumns=`"+sortColumns
+            elif type(sortColumns) == list:
+                runstr += ",sortColumns="
+                for key in sortColumns:
+                    runstr += "`"+key
+
+        if keepDuplicates is not None:
+            if isinstance(keepDuplicates, str):
+                runstr += ",keepDuplicates="+keepDuplicates
+            else:
+                raise RuntimeError("Only str is accepted for keepDuplicates")
+
+        if sortKeyMappingFunction is not None:
+            if type(sortKeyMappingFunction) == str:
+                runstr += ",sortKeyMappingFunction=["+sortKeyMappingFunction+"]"
+            elif type(sortKeyMappingFunction) == list:
+                runstr += ",sortKeyMappingFunction=["
+                for i in range(len(sortKeyMappingFunction)):
+                    if i != 0:
+                        runstr += ","
+                    if type(sortKeyMappingFunction[i]) == str:
+                        runstr += sortKeyMappingFunction[i]
+                    else:
+                        raise RuntimeError('The "sortKeyMappingFunction" parameter must be a string or a list of strings.')
+                runstr += "]"
+            else:
+                raise RuntimeError('The "sortKeyMappingFunction" parameter must be a string or a list of strings.')
+        runstr += ");"
+        self.__session.run(runstr)
+        return self.__session.loadTable(cptHandle)
```

## dolphindb/session.py

```diff
@@ -1,1629 +1,1643 @@
-"""Session
-Package: session package.
-        including classes Session, DBConnectionPool, BatchTableWriter, MultithreadedTableWriter
-"""
-
-
-import asyncio
-import os
-import platform
-import re
-import sys
-import warnings
-from concurrent.futures import Future
-from datetime import date, datetime
-from threading import Lock, Thread
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
-
-import numpy as np
-from dolphindb.database import Database
-from dolphindb.settings import (DDB_EPSILON, PROTOCOL_ARROW, PROTOCOL_DDB,
-                                PROTOCOL_DEFAULT, PROTOCOL_PICKLE)
-from dolphindb.table import Table
-from dolphindb.utils import _generate_dbname, _generate_tablename, month
-from pandas import DataFrame
-
-sys.path.append(os.path.dirname(__file__))
-ddbcpp = __import__("_dolphindbcpp")
-ddbcpp.init()
-
-
-class DBConnectionPool(object):
-    """DBConnectionPool is the connection pool object where multiple threads can be created to execute scripts in parallel and improve task efficiency.
-
-    Note:
-        To improve efficiency, methods such as run of class DBConnectionPool are packaged into coroutine functions in python.
-
-    Args:
-        host : server address. It can be IP address, domain, or LAN hostname, etc.
-        port : port name.
-        threadNum : number of threads. Defaults to 10.
-        userid : username. Defaults to None.
-        password : password. Defaults to None.
-        loadBalance : whether to enable load balancing. True means enabled (the connections will be distributed evenly across the cluster), otherwise False. Defaults to False.
-        highAvailability : whether to enable high availability. True means enabled, otherwise False. Defaults to False.
-        compress : whether to enable compression. True means enabled, otherwise False. Defaults to False.
-        reConnect : whether to enable reconnection. True means enabled, otherwise False. Defaults to False.
-        enablePickle : whether to enable the Pickle protocol. Defaults to False.
-        python : whether to enable the Python parser. True means enabled, otherwise False. Defaults to False.
-        protocol : the data transmission protocol. Defaults to PROTOCOL_DEFAULT, which is equivalant to PROTOCOL_PICKLE.
-
-    Kwargs:
-        show_output : whether to display the output of print statements in the script after execution. Defaults to True.
-
-    Note:
-        If the parameter python is True, the script is parsed in Python rather than DolphinDB language.
-    """
-    def __init__(
-        self, host: str, port: int, threadNum: int = 10, userid: str = None, password: str = None,
-        loadBalance: bool = False, highAvailability: bool = False, compress: bool = False,
-        reConnect: bool = False, python: bool = False, protocol: int = PROTOCOL_DEFAULT,
-        *, show_output: bool = True
-    ):
-        """Constructor of DBConnectionPool, including the number of threads, load balancing, high availability, reconnection, compression and Pickle protocol."""
-        userid = userid if userid is not None else ""
-        password = password if password is not None else ""
-        if protocol == PROTOCOL_DEFAULT:
-            protocol = PROTOCOL_PICKLE
-        if protocol not in [PROTOCOL_DEFAULT, PROTOCOL_DDB, PROTOCOL_PICKLE, PROTOCOL_ARROW]:
-            raise RuntimeError(f"Protocol {protocol} is not supported. ")
-
-        if protocol == PROTOCOL_ARROW and compress:
-            raise RuntimeError("The Arrow protocol does not support compression.")
-
-        if protocol == PROTOCOL_ARROW:
-            __import__("pyarrow")
-
-        self.mutex = Lock()
-        self.pool = ddbcpp.dbConnectionPoolImpl(host, port, threadNum, userid, password, loadBalance, highAvailability, compress, reConnect, python, protocol, show_output)
-        self.host = host
-        self.port = port
-        self.userid = userid
-        self.password = password
-        self.taskId = 0
-        self.loop = None
-        self.thread = None
-        self.protocol = protocol
-        self.shutdown_flag = False
-
-    def __del__(self):
-        if hasattr(self, "pool") and self.pool is not None:
-            self.shutDown()
-
-    async def run(self, script: str, *args, **kwargs):
-        """Coroutine function.
-
-        Pass the script to the connection pool to call the thread execution with the run method.
-
-        Args:
-            script : DolphinDB script to be executed.
-            args : arguments to be passed to the function.
-
-        Note:
-            args is only required when script is the function name.
-
-        Kwargs:
-            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
-            pickleTableToList : whether to convert table to list or DataFrame. True: to list, False: to DataFrame. Defaults to False.
-            priority : a job priority system with 10 priority levels (0 to 9), allocating thread resources to high-priority jobs and using round-robin allocation for jobs of the same priority. Defaults to 4.
-            parallelism : parallelism determines the maximum number of threads to execute a job's tasks simultaneously on a data node; the system optimizes resource utilization by allocating all available threads to a job if there's only one job running and multiple local executors are available. Defaults to 2.
-
-        Returns:
-            execution result.
-
-        Note:
-            When setting pickleTableToList=True and enablePickle=True, if the table contains array vectors, it will be converted to a NumPy 2d array.
-            If the length of each row is different, the execution fails.
-        """
-        priority = kwargs.get('priority', 4)
-        parallelism = kwargs.get('parallelism', 2)
-        if type(priority) is not int or priority > 9 or priority < 0:
-            raise RuntimeError("priority must be an integer from 0 to 9")
-        if type(parallelism) is not int or parallelism <= 0:
-            raise RuntimeError("parallelism must be an integer greater than 0")
-
-        self.mutex.acquire()
-        self.taskId = self.taskId + 1
-        tid = self.taskId
-        self.mutex.release()
-        if "clearMemory" not in kwargs.keys():
-            kwargs["clearMemory"] = True
-        self.pool.run(script, tid, *args, **kwargs)
-        while True:
-            isFinished = self.pool.isFinished(tid)
-            if isFinished == 0:
-                await asyncio.sleep(0.01)
-            else:
-                return self.pool.getData(tid)
-
-    def addTask(self, script: str, taskId: int, *args, **kwargs):
-        """Add a task and specify the task ID to execute the script.
-
-        Args:
-            script : script to be executed.
-            taskId : the task ID.
-            args : arguments to be passed to the function.
-
-        Note:
-            args is only required when script is the function name.
-
-        Kwargs:
-            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
-
-        Returns:
-            execution result.
-        """
-        if "clearMemory" not in kwargs.keys():
-            kwargs["clearMemory"] = True
-        return self.pool.run(script, taskId, *args, **kwargs)
-
-    def isFinished(self, taskId: int) -> bool:
-        """Get the completion status of the specified task.
-
-        Args:
-            taskId : the task ID.
-
-        Returns:
-            True if the task is finished, otherwise False.
-        """
-        return self.pool.isFinished(taskId)
-
-    def getData(self, taskId: int):
-        """Get data of the specified task.
-
-        Args:
-            taskId : the task ID.
-
-        Returns:
-            data of the task.
-
-        Note:
-            For each task, the data can only be obtained once and will be cleared immediately after the data is obtained.
-        """
-        return self.pool.getData(taskId)
-
-    def __start_thread_loop(self, loop):
-        asyncio.set_event_loop(loop)
-        loop.run_forever()
-
-    def startLoop(self):
-        """Create and start an event loop.
-
-        Raises:
-            the event loop has been created.
-        """
-        if self.loop is not None:
-            raise RuntimeError("Event loop is already started!")
-        self.loop = asyncio.new_event_loop()
-        self.thread = Thread(target=self.__start_thread_loop, args=(self.loop,))
-        self.thread.setDaemon(True)
-        self.thread.start()
-
-    async def stopLoop(self):
-        """Stop the event loop."""
-        await asyncio.sleep(0.01)
-        self.loop.stop()
-
-    def runTaskAsync(self, script: str, *args, **kwargs) -> Future:
-        """Execute script tasks asynchronously.
-
-        Args:
-            script : script to be executed.
-            args : arguments to be passed to the function.
-
-        Kwargs:
-            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
-
-        Returns:
-            concurrent.futures.Future object for receiving data.
-        """
-        if self.loop is None:
-            self.startLoop()
-        if "clearMemory" not in kwargs.keys():
-            kwargs["clearMemory"] = True
-        task = asyncio.run_coroutine_threadsafe(self.run(script, *args, **kwargs), self.loop)
-        return task
-
-    def runTaskAsyn(self, script: str, *args, **kwargs) -> Future:
-        """Execute script tasks asynchronously.
-
-        Deprecated:
-            Please use runTaskAsync instead of runTaskAsyn.
-
-        Args:
-            script : script to be executed.
-            args : arguments to be passed to the function.
-
-        Kwargs:
-            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
-
-        Returns:
-            concurrent.futures.Future object for receiving data.
-        """
-        if "clearMemory" not in kwargs.keys():
-            kwargs["clearMemory"] = True
-        warnings.warn("Please use runTaskAsync instead of runTaskAsyn.", DeprecationWarning, stacklevel=2)
-        return self.runTaskAsync(script, *args, **kwargs)
-
-    def shutDown(self):
-        """Close the DBConnectionPool, stop the event loop and terminate all asynchronous tasks."""
-        with self.mutex:
-            if self.shutdown_flag:
-                return
-            self.shutdown_flag = True
-        self.host = None
-        self.port = None
-        if self.loop is not None:
-            asyncio.run_coroutine_threadsafe(self.stopLoop(), self.loop)
-            self.thread.join()
-            if self.loop.is_running():
-                self.loop.stop()
-            else:
-                self.loop.close()
-        if self.pool is not None:
-            self.pool.shutDown()
-            self.pool = None
-        self.loop = None
-        self.thread = None
-
-    def getSessionId(self) -> List[str]:
-        """Obtain Session ID of all sessions.
-
-        Returns:
-            list of thread ID.
-        """
-        return self.pool.getSessionId()
-
-    def is_shutdown(self) -> bool:
-        with self.mutex:
-            return self.shutdown_flag
-
-
-class streamDeserializer(object):
-    """Deserializer stream blob in multistreamingtable reply.
-
-    Args:
-        sym2table : a dict object indicating the corresponding relationship between the unique identifiers of the tables and the table objects.
-        session : a Session object. Defaults to None.
-    """
-    def __init__(self, sym2table: Dict[str, Union[List[str], str]], session=None):
-        """Constructor of streamDeserializer."""
-        self.cpp = ddbcpp.streamDeserializer(sym2table)
-        if session is not None:
-            self.cpp.setSession(session.cpp)
-
-
-class Session(object):
-    """Session is the connection object to execute scripts.
-
-    Args:
-        host : server address. It can be IP address, domain, or LAN hostname, etc. Defaults to None.
-        port : port name. Defaults to None.
-
-    Note:
-        If neither host nor port is set to None, a connection will be established.
-
-    Args:
-        userid : username. Defaults to "", meaning not to log in.
-        password : password. Defaults to "", meaning not to log in.
-        enableSSL : whether to enable SSL. True means to enable SSL. Defaults to False.
-        enableASYNC(enableASYN) : whether to enable asynchronous communication. Defaults to False.
-
-    Deprecated:
-        Please use enableASYNC instead of enableASYN.
-
-    Args:
-        keepAliveTime : the duration between two keepalive transmissions to detect the TCP connection status. Defaults to 30 (seconds). Set the parameter to release half-open TCP connections timely when the network is unstable.
-        enableChunkGranularityConfig : whether to enable chunk granularity configuration. Defaults to False.
-        compress : whether to enable compressed communication. Defaults to False.
-        enablePickle : whether to enable the Pickle protocol. Defaults to True.
-        protocol: the data transmission protocol. Defaults to PROTOCOL_DEFAULT, which is equivalant to PROTOCOL_PICKLE.
-        python : whether to enable python parser. Defaults to False.
-
-    Kwargs:
-        show_output : whether to display the output of print statements in the script after execution. Defaults to True.
-
-    Note:
-        set enableSSL =True to enable encrypted communication. It's also required to configure enableHTTPS =true in the server.
-
-    Note:
-        set enableASYNC =True to enable asynchronous mode and the communication with the server can only be done through the session.run method. As there is no return value, it is suitable for asynchronous writes.
-    """
-    def __init__(
-        self, host: Optional[str] = None, port: Optional[int] = None,
-        userid: Optional[str] = "", password: Optional[str] = "", enableSSL: bool = False,
-        enableASYNC: bool = False, keepAliveTime: int = 30, enableChunkGranularityConfig: bool = False,
-        compress: bool = False, enablePickle: bool = None, protocol: int = PROTOCOL_DEFAULT,
-        python: bool = False, *, show_output: bool = True, **kwargs
-    ):
-        """Constructor of Session, inluding OpenSSL encryption, asynchronous mode, TCP detection, block granularity matching, compression, Pickle protocol."""
-        if 'enableASYN' in kwargs.keys():
-            enableASYNC = kwargs['enableASYN']
-            warnings.warn("Please use enableASYNC instead of enableASYN.", DeprecationWarning, stacklevel=2)
-
-        default_protocol = PROTOCOL_PICKLE
-        if protocol == PROTOCOL_DEFAULT:
-            protocol = PROTOCOL_PICKLE if enablePickle else PROTOCOL_DDB
-            if enablePickle is None:
-                protocol = default_protocol
-        elif enablePickle:
-            raise RuntimeError("When enablePickle=true, the parameter protocol must not be specified. ")
-
-        if protocol not in [PROTOCOL_DEFAULT, PROTOCOL_DDB, PROTOCOL_PICKLE, PROTOCOL_ARROW]:
-            raise RuntimeError(f"Protocol {protocol} is not supported. ")
-
-        if protocol == PROTOCOL_ARROW and compress:
-            raise RuntimeError("The Arrow protocol does not support compression.")
-
-        if protocol == PROTOCOL_ARROW:
-            __import__("pyarrow")
-
-        self.cpp = ddbcpp.sessionimpl(enableSSL, enableASYNC, keepAliveTime, compress, python, protocol, show_output)
-        self.host = host
-        self.port = port
-        self.userid = userid
-        self.password = password
-        self.mutex = Lock()
-        self.enableEncryption = True
-        self.enableChunkGranularityConfig = enableChunkGranularityConfig
-        self.enablePickle = enablePickle
-        self.protocol = protocol
-        if self.host is not None and self.port is not None:
-            self.connect(host, port, userid, password, keepAliveTime=keepAliveTime)
-
-    def __del__(self):
-        if hasattr(self, "cpp"):
-            self.cpp.close()
-
-    def connect(
-        self, host: str, port: int, userid: str = None, password: str = None, startup: str = None,
-        highAvailability: bool = False, highAvailabilitySites: Optional[List[str]] = None,
-        keepAliveTime: Optional[int] = None, reconnect: bool = False
-    ) -> bool:
-        """Establish connection, including initialization script, high availability, TCP detection.
-
-        Args:
-            host : server address. It can be IP address, domain, or LAN hostname, etc.
-            port : port name.
-            userid : username. Defaults to None, indicating no login.
-            password : password. Defaults to None, indicating no login..
-            startup : the startup script to execute the preloaded tasks immediately after the connection is established. Defaults to None.
-            highAvailability : whether to enable high availability. True means enabled, otherwise False. Defaults to False.
-            highAvailabilitySites : a list of high-availability nodes. Defaults to None.
-            keepAliveTime : the duration between two keepalive transmissions to detect the TCP connection status. Defaults to None, meaning keepAliveTime = 30 (seconds). Set the parameter to release half-open TCP connections timely when the network is unstable.
-            reconnect : whether to enable reconnection. True means enabled, otherwise False. Defaults to False.
-
-        Returns:
-            whether the connection is established. True if established, otherwise False.
-        """
-        if highAvailabilitySites is None:
-            highAvailabilitySites = []
-        if keepAliveTime is None:
-            keepAliveTime = -1
-        if userid is None:
-            userid = ""
-        if password is None:
-            password = ""
-        if startup is None:
-            startup = ""
-        if self.cpp.connect(host, port, userid, password, startup, highAvailability, highAvailabilitySites, keepAliveTime, reconnect):
-            self.host = host
-            self.port = port
-            self.userid = userid
-            self.password = password
-            return True
-        else:
-            return False
-
-    def login(self, userid: str, password: str, enableEncryption: bool = True):
-        """Manually log in to the server.
-
-        Args:
-            userid : username.
-            password : password.
-            enableEncryption : whether to enable encrypted transmission for username and password. Defaults to True.
-
-        Note:
-            Specify the userid and password in the connect() method to log in automatically.
-        """
-        self.mutex.acquire()
-        try:
-            self.userid = userid
-            self.password = password
-            self.enableEncryption = enableEncryption
-            self.cpp.login(userid, password, enableEncryption)
-        finally:
-            self.mutex.release()
-
-    def close(self):
-        """Close Session connection."""
-        self.host = None
-        self.port = None
-        self.cpp.close()
-
-    def isClosed(self) -> bool:
-        """Check if the current Session has been closed.
-
-        Returns:
-            bool: True if closed, otherwise False.
-        """
-        return self.host is None
-
-    def upload(self, nameObjectDict):
-        """Upload Python objects to DolphinDB server.
-
-        Args:
-            nameObjectDict : Python dictionary object. The keys of the dictionary are the variable names in DolphinDB and the values are Python objects, which can be numbers, strings, lists, DataFrame, etc.
-
-        Returns:
-            the server address of the uploaded object.
-
-        Note:
-            A pandas DataFrame corresponds to DolphinDB table.
-        """
-        return self.cpp.upload(nameObjectDict)
-
-    def run(self, script: str, *args, **kwargs):
-        """Execute script.
-
-        Args:
-            script : DolphinDB script to be executed.
-            args : arguments to be passed to the function.
-
-        Note:
-            args is only required when script is the function name.
-
-        Kwargs:
-            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to False.
-            pickleTableToList : whether to convert table to list or DataFrame. True: to list, False: to DataFrame.  Defaults to False.
-            priority : a job priority system with 10 priority levels (0 to 9), allocating thread resources to high-priority jobs and using round-robin allocation for jobs of the same priority. Defaults to 4.
-            parallelism : parallelism determines the maximum number of threads to execute a job's tasks simultaneously on a data node; the system optimizes resource utilization by allocating all available threads to a job if there's only one job running and multiple local executors are available. Defaults to 2.
-            fetchSize : the size of a block.
-
-        Note:
-            fetchSize cannot be less than 8192 Bytes.
-
-        Returns:
-            execution result. If fetchSize is specified, a BlockReader object will be returned. Each block can be read with the read() method.
-
-        Note:
-            When setting pickleTableToList=True and enablePickle=True, if the table contains array vectors, it will be converted to a NumPy 2d array. If the length of each row is different, the execution fails.
-        """
-        priority = kwargs.get('priority', 4)
-        parallelism = kwargs.get('parallelism', 2)
-        if type(priority) is not int or priority > 9 or priority < 0:
-            raise RuntimeError("priority must be an integer from 0 to 9")
-        if type(parallelism) is not int or parallelism <= 0:
-            raise RuntimeError("parallelism must be an integer greater than 0")
-
-        if kwargs:
-            if "fetchSize" in kwargs.keys():
-                return BlockReader(self.cpp.runBlock(script, **kwargs))
-        return self.cpp.run(script, *args, **kwargs)
-
-    def runFile(self, filepath: str, *args, **kwargs):
-        """Execute script.
-
-        Args:
-            filepath : the path of the file on the server to be executed.
-            args : arguments to be passed to the function.
-
-        Note:
-            args is only required when script is the function name.
-
-        Kwargs:
-            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to False.
-            pickleTableToList : whether to convert table to list or DataFrame. True: to list, False: to DataFrame.  Defaults to False.
-
-        Returns:
-            execution result.
-
-        Note:
-            When setting pickleTableToList=True and enablePickle=True, if the table contains array vectors, it will be converted to a NumPy 2d array. If the length of each row is different, the execution fails.
-        """
-        with open(filepath, "r") as fp:
-            script = fp.read()
-            return self.run(script, *args, **kwargs)
-
-    def getSessionId(self) -> str:
-        """Get the Session ID of the current Session.
-
-        Returns:
-            Session ID.
-        """
-        return self.cpp.getSessionId()
-
-    def enableStreaming(self, port: int = 0, threadCount: int = 1) -> None:
-        """Enable streaming.
-
-        Args:
-            port : the subscription port for incoming data. The server will connect to the port automatically.
-            threadCount : the number of threads. Defaults to 1.
-
-        Note:
-            If the server you're connecting to supports transferring subscribed data using the connection initiated by the subsriber, 
-            do not specify this port. Otherwise, the port must be specified.
-
-        """
-        self.cpp.enableStreaming(port, threadCount)
-
-    def subscribe(
-        self, host: str, port: int, handler: Callable, tableName: str, actionName: str = None,
-        offset: int = -1, resub: bool = False, filter=None,
-        msgAsTable: bool = False, batchSize: int = 0, throttle: float = 1.0,
-        userName: str = None, password: str = None, streamDeserializer: Optional["streamDeserializer"] = None
-    ) -> None:
-        """Subscribe to stream tables in DolphinDB.
-
-        Args:
-            host : server address. It can be IP address, domain, or LAN hostname, etc.
-            port : port name.
-            handler : user-defined callback function for processing incoming data.
-            tableName : name of the published table.
-            actionName : name of the subscription task. Defaults to "".
-            offset : an integer indicating the position of the first message where the subscription begins. Defaults to -1.
-
-        Note:
-            If offset is -1 or exceeding the number of rows in the stream table, the subscription starts with the next new message. It cannot be other negative values.
-
-        Args:
-            resub : True means to keep trying to subscribe to table after the subscription attempt fails. Defaults to False.
-            filter : a vector indicating the filtering columns. Only the rows with values of the filtering column in the vector are published to the subscriber. Defaults to None.
-            msgAsTable : whether to convert the subscribed data to dataframe. If msgAsTable = True, the subscribed data is ingested into handler as a DataFrame. Defaults to False, which means the subscribed data is ingested into handler as a List of nparrays. This optional parameter has no effect if batchSize is not specified.
-            batchSize : an integer indicating the number of unprocessed messages to trigger the handler. If it is positive, the handler does not process messages until the number of unprocessed messages reaches batchSize. If it is unspecified or non-positive, the handler processes incoming messages as soon as they come in. Defaults to 0.
-            throttle : a float indicating the maximum waiting time (in seconds) before the handler processes the incoming messages. Defaults to 1. This optional parameter has no effect if batchSize is not specified.
-            userName : username. Defaults to None, indicating no login.
-            password : password. Defaults to None, indicating no login.
-            streamDeserializer : A deserializer of heterogeneous stream table. Defaults to None.
-        """
-        if not isinstance(msgAsTable, bool):
-            raise TypeError("msgAsTable must be a bool.")
-        if not isinstance(batchSize, int):
-            raise TypeError("batchSize must be a int.")
-        if not isinstance(throttle, float) and not isinstance(throttle, int):
-            raise TypeError("throttle must be a float or a int.")
-        if throttle <= DDB_EPSILON:
-            raise ValueError("throttle must be greater than 0.")
-        if filter is None:
-            filter = np.array([], dtype='int64')
-        if actionName is None:
-            actionName = ""
-        if userName is None:
-            userName = ""
-        if password is None:
-            password = ""
-        sd = None
-        if streamDeserializer is None:
-            sd = ddbcpp.streamDeserializer({})
-        else:
-            sd = streamDeserializer.cpp
-        if batchSize > 0:
-            self.cpp.subscribeBatch(
-                host, port, handler, tableName, actionName,
-                offset, resub, filter, msgAsTable, batchSize, throttle,
-                userName, password, sd
-            )
-        else:
-            if msgAsTable:
-                raise ValueError("msgAsTable must be False when batchSize is 0")
-            self.cpp.subscribe(
-                host, port, handler, tableName, actionName,
-                offset, resub, filter, userName, password, sd
-            )
-
-    def unsubscribe(self, host: str, port: str, tableName: str, actionName: str = None) -> None:
-        """Unsubscribe.
-
-        Args:
-            host : server address. It can be IP address, domain, or LAN hostname, etc.
-            port : port name.
-            tableName : name of the published table.
-            actionName : name of the subscription task. Defaults to None.
-        """
-        if actionName is None:
-            actionName = ""
-        self.cpp.unsubscribe(host, port, tableName, actionName)
-
-    def getSubscriptionTopics(self) -> List[str]:
-        """Get all subscription topics.
-
-        Returns:
-            a list of all subscription topics in the format of "host/port/tableName/actionName".
-        """
-        return self.cpp.getSubscriptionTopics()
-
-    def getInitScript(self) -> str:
-        """Get the init script of the Session.
-
-        Returns:
-            string of the init script.
-        """
-        return self.cpp.getInitScript()
-
-    def setInitScript(self, script: str) -> None:
-        """Set up init script of the Session.
-
-        Args:
-            string of the init script.
-        """
-        self.cpp.setInitScript(script)
-
-    def saveTable(self, tbl: Table, dbPath: str) -> bool:
-        """Save the table.
-
-        Args:
-            tbl : DolphinDB Table object of the in-memory table to be saved.
-            dbPath : DolphinDB database path.
-
-        Returns:
-            True.
-        """
-        tblName = tbl.tableName()
-        dbName =  _generate_dbname()
-        s1 = dbName+"=database('"+dbPath+"')"
-        self.run(s1)
-        s2 = "saveTable(%s, %s)" % (dbName, tblName)
-        self.run(s2)
-        return True
-
-    def loadText(self,  remoteFilePath: str, delimiter: str = ",") -> "Table":
-        """Import text files into DolphinDB as an in-memory table.
-
-        Args:
-            remoteFilePath : the remote file path on the server. Defaults to None.
-            delimiter : delimiter, Defaults to ",".
-
-        Returns:
-            a DolphinDB in-memory Table object.
-
-        Note:
-            The amount of data loaded into the in-memory table must be less than the available memory.
-        """
-        tableName = _generate_tablename()
-        runstr = tableName + '=loadText("' + remoteFilePath + '","' + delimiter + '")'
-        self.run(runstr)
-        return Table(data=tableName, s=self, isMaterialized=True)
-
-    def loadTextEx(
-        self, dbPath: str, tableName: str, partitionColumns: Optional[List[str]] = None,
-        remoteFilePath: str = None, delimiter: str = ",", sortColumns: Optional[List[str]] = None,
-    ) -> "Table":
-        """Import a partitioned in-memory table.
-
-        Args:
-            dbPath : database path.
-            tableName : table name.
-            partitionColumns : list of strings indicating the partitioning columns. Defaults to None.
-            remoteFilePath : remote file path. Defaults to None.
-            delimiter : delimiter of each column. Defaults to ",".
-            sortColumns : list of strings indicating the sort columns. Defaults to None.
-
-        Returns:
-            a DolphinDB Table object.
-        """
-        if partitionColumns is None:
-            partitionColumns = []
-        if sortColumns is None:
-            sortColumns = []
-        isDBPath = True
-        if "/" in dbPath or "\\" in dbPath or "dfs://" in dbPath:
-            dbstr = 'db=database("' + dbPath + '")'
-            self.run(dbstr)
-            tbl_str = '{tableNameNEW} = loadTextEx(db, "{tableName}", {partitionColumns}, "{remoteFilePath}", {delimiter} {extraParams})'
-        else:
-            isDBPath = False
-            tbl_str = '{tableNameNEW} = loadTextEx("{dbPath}", "{tableName}", {partitionColumns}, "{remoteFilePath}", {delimiter} {extraParams})'
-        fmtDict = dict()
-        fmtDict['tableNameNEW'] = _generate_tablename()
-        fmtDict['dbPath'] = dbPath
-        fmtDict['tableName'] = tableName
-        fmtDict['partitionColumns'] = '[' + ','.join([f'"{_}"' for _ in partitionColumns]) + ']'
-        fmtDict['remoteFilePath'] = remoteFilePath if remoteFilePath is not None else ""
-        fmtDict['delimiter'] = delimiter
-        if sortColumns:
-            extraParams = ", sortColumns=" + '[' + ','.join([f'"{_}"' for _ in sortColumns]) + ']'
-        else:
-            extraParams = ""
-        fmtDict['extraParams'] = extraParams
-        tbl_str = re.sub(' +', ' ', tbl_str.format(**fmtDict).strip())
-        self.run(tbl_str)
-        if isDBPath:
-            return Table(data=fmtDict['tableName'], dbPath=dbPath, s=self)
-        else:
-            return Table(data=fmtDict['tableNameNEW'], s=self)
-
-    def ploadText(self, remoteFilePath: str, delimiter: str = ",") -> "Table":
-        """Import text files in parallel into DolphinDB as a partitioned in-memory table, which is faster than method loadText.
-
-        Args:
-            remoteFilePath : the remote file path on the server. Defaults to None.
-            delimiter : delimiter, Defaults to ",".
-
-        Returns:
-            a DolphinDB in-memory Table object.
-        """
-        tableName = _generate_tablename()
-        runstr = tableName + '= ploadText("' + remoteFilePath + '","' + delimiter + '")'
-        self.run(runstr)
-        return Table(data=tableName, s=self, isMaterialized=True)
-
-    def table(
-        self, dbPath: str = None, data=None,  tableAliasName: str = None,
-        inMem: bool = False, partitions: Optional[List[str]] = None
-    ) -> "Table":
-        """Create a DolphinDB table object and upload it to the server.
-
-        Deprecated:
-            inMem will be deprecated in a future version.
-
-        Args:
-            dbPath : database path. Defaults to None.
-            data : data of the table. Defaults to None.
-            tableAliasName : alias of the table. Defaults to None.
-            inMem : whether to load the table into memory. True: to load the table into memory. Defaults to False.
-            partitions : the partitions to be loaded into memory. Defaults to None, which means to load all partitions.
-
-        Returns:
-            a DolphinDB table object.
-        """
-        if partitions is None:
-            partitions = []
-        return Table(dbPath=dbPath, data=data,  tableAliasName=tableAliasName, inMem=inMem, partitions=partitions, s=self, isMaterialized=True)
-
-    def loadTable(self, tableName: str,  dbPath: Optional[str] = None, partitions=None, memoryMode: bool = False) -> "Table":
-        """Load a DolphinDB table.
-
-        Args:
-            tableName : the DolphinDB table name.
-            dbPath : path to the DolphinDB database. Defaults to None.
-            partitions : the partitioning columns of the partitioned table. Defaults to None.
-            memoryMode : whether to load the table into memory or just load its column names. True: to load the table into memory. Defaults to False.
-
-        Deprecated:
-            memoryMode will be deprecated in a future version.
-
-        Returns:
-            a DolphinDB table object.
-        """
-        def isDate(s):
-            try:
-                datetime.strptime(s, '%Y.%m.%d')
-                return True
-            except ValueError:
-                return False
-
-        def isMonth(s):
-            try:
-                datetime.strptime(s, '%Y.%mM')
-                return True
-            except ValueError:
-                return False
-
-        def isDatehour(s):
-            try:
-                datetime.strptime(s, '%Y.%m.%dT%H')
-                return True
-            except ValueError:
-                return False
-
-        def isTime(s):
-            return isDate(s) or isMonth(s) or isDatehour(s)
-
-        def myStr(x):
-            if type(x) is str and not isTime(x):
-                return "'" + x + "'"
-            else:
-                return str(x)
-
-        if partitions is None:
-            partitions = []
-        if dbPath:
-            runstr = '{tableName} = loadTable("{dbPath}", "{data}",{partitions},{inMem})'
-            fmtDict = dict()
-            tbName = _generate_tablename(tableName)
-            fmtDict['tableName'] = tbName
-            fmtDict['dbPath'] = dbPath
-            fmtDict['data'] = tableName
-            if type(partitions) is list:
-                fmtDict['partitions'] = ('[' + ','.join(myStr(x) for x in partitions) + ']') if len(partitions) else ""
-            else:
-                fmtDict['partitions'] = myStr(partitions)
-
-            fmtDict['inMem'] = str(memoryMode).lower()
-            runstr = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
-            self.run(runstr)
-            return Table(data=tbName, s=self, isMaterialized=True)
-        else:
-            return Table(data=tableName, s=self, needGC=False, isMaterialized=True)
-
-    def loadTableBySQL(self, tableName: str, dbPath: str, sql: str) -> "Table":
-        """Load records that satisfy the filtering conditions in a SQL query as a partitioned in-memory table.
-
-        Args:
-            tableName : the DolphinDB table name.
-            dbPath : the DolphinDB database where the table is stored.
-            sql : SQL statement.
-
-        Returns:
-            a Table object.
-        """
-        # loadTableBySQL
-        tmpTableName = _generate_tablename()
-        self.run(f"""
-            {tableName}=loadTable("{dbPath}", "{tableName}");
-            {tmpTableName}=loadTableBySQL(<{sql}>);
-        """)
-        return Table(data=tmpTableName, s=self, isMaterialized=True)
-
-    def database(
-        self, dbName: str = None, partitionType: int = None, partitions=None,
-        dbPath: str = None, engine: str = None, atomic: str = None, chunkGranularity: str = None
-    ) -> "Database":
-        """Create database.
-
-        Args:
-            dbName : database name. Defaults to None.
-            partitionType : partition type. Defaults to None.
-            partitions : describes how the partitions are created. Partitions is usually a list or np.array, with type char/int/np.datetime64. Defaults to None.
-            dbPath : database path. Defaults to None.
-            engine: storage engine, can be 'OLAP' or 'TSDB'. Defaults to None, meaning to "OLAP".
-            atomic : indicates at which level the atomicity is guaranteed for a write transaction. It can be 'TRANS' or 'CHUNK'. Defaults to None, meaning to "TRANS".
-            chunkGranularity : the chunk granularity, can be 'TABLE' or 'DATABASE'. Defaults to None.
-
-        Note:
-            The parameter chunkGranularity only takes effect when enableChunkGranularityConfig = true.
-
-        Returns:
-            a DolphinDB database object.
-        """
-        if partitions is not None:
-            partition_type = type(partitions[0])
-        else:
-            partition_type = None
-
-        if partition_type == np.datetime64:
-            partition_str = self.convertDatetime64(partitions)
-
-        elif partition_type == Database:
-            partition_str = self.convertDatabase(partitions)
-
-        elif type(partitions) == np.ndarray and (partition_type == np.ndarray or partition_type == list):
-            dataType = type(partitions[0][0])
-            partition_str = '['
-            for partition in partitions:
-                if dataType == date or dataType == month:
-                    partition_str += self.convertDateAndMonth(partition) + ','
-                elif dataType == datetime:
-                    partition_str += self.convertDatetime(partition) + ','
-                elif dataType == Database:
-                    partition_str += self.convertDatabase(partition) + ','
-                else:
-                    partition_str += str(partition) + ','
-                    partition_str = partition_str.replace('list', ' ')
-                    partition_str = partition_str.replace('(', '')
-                    partition_str = partition_str.replace(')', '')
-            partition_str = partition_str.rstrip(',')
-            partition_str += ']'
-
-        else:
-            if partition_type is not None:
-                partition_str = str(partitions)
-            else:
-                partition_str = ""
-
-        if dbName is None:
-            dbName = _generate_dbname()
-
-        if partitionType:
-            if dbPath:
-                dbstr = dbName + '=database("'+dbPath+'",' + str(partitionType) + "," + partition_str
-            else:
-                dbstr = dbName + '=database("",' + str(partitionType) + "," + partition_str
-        else:
-            if dbPath:
-                dbstr = dbName + '=database("' + dbPath + '"'
-            else:
-                dbstr = dbName + '=database(""'
-
-        if engine is not None:
-            dbstr += ",engine='" + engine + "'"
-        if atomic is not None:
-            dbstr += ",atomic='" + atomic + "'"
-        if self.enableChunkGranularityConfig and chunkGranularity is not None:
-            dbstr += ",chunkGranularity='" + chunkGranularity + "'"
-
-        dbstr += ")"
-
-        self.run(dbstr)
-        return Database(dbName=dbName, s=self)
-
-    def existsDatabase(self, dbUrl: str) -> bool:
-        """Check if the database exists.
-
-        Args:
-            dbUrl : database path.
-
-        Returns:
-            True if the database exists, otherwise False.
-        """
-        return self.run("existsDatabase('%s')" % dbUrl)
-
-    def existsTable(self, dbUrl: str, tableName: str) -> bool:
-        """Check if the table exists.
-
-        Args:
-            dbUrl : database path.
-            tableName : table name.
-
-        Returns:
-            True if the table exists, otherwise False.
-        """
-        return self.run("existsTable('%s','%s')" % (dbUrl, tableName))
-
-    def dropDatabase(self, dbPath: str) -> None:
-        """Delete a database.
-
-        Args:
-            dbPath : database path.
-        """
-        self.run("dropDatabase('" + dbPath + "')")
-
-    def dropPartition(self, dbPath: str, partitionPaths: Union[str, List[str]], tableName: str = None) -> None:
-        """Delete one or more partitions of the database.
-
-        Args:
-            dbPath : database path.
-            partitionPaths : a string or list of partition paths.
-
-        Note:
-            The directory of a partition under the database folder or a list of directories of multiple partitions must start with '/'.
-
-        Args:
-            tableName : table name. Defaults to None, indicating all tables under the partitions are deleted.
-        """
-        db = _generate_dbname()
-        self.run(f"""{db} = database("{dbPath}")""")
-        if isinstance(partitionPaths, list):
-            pths = ','.join(partitionPaths)
-        else:
-            pths = partitionPaths
-
-        if tableName:
-            self.run(f"""dropPartition({db}, [{pths}], "{tableName}")""")
-        else:
-            self.run(f"""dropPartition({db}, [{pths}])""")
-        self.run(f"""undef("{db}")""")
-
-    def dropTable(self, dbPath: str, tableName: str) -> None:
-        """Delete a table.
-
-        Args:
-            dbPath : database path.
-            tableName : table name.
-        """
-        db = _generate_dbname()
-        self.run(db + '=database("' + dbPath + '")')
-        self.run(f'dropTable({db}, "{tableName}")')
-
-    def undef(self, varName: str, varType: str) -> None:
-        """Release the specified object in the Session.
-
-        Args:
-            varName : variable name in DolphinDB.
-            varType : variable type in DolphinDB,including "VAR" (variable), "SHARED" (shared variable), "DEF" (function definition).
-        """
-        undef_str = 'undef("{varName}", {varType})'
-        fmtDict = dict()
-        fmtDict['varName'] = varName
-        fmtDict['varType'] = varType
-        self.run(undef_str.format(**fmtDict).strip())
-
-    def undefAll(self) -> None:
-        """Release all objects in the Session."""
-        self.run("undef all")
-
-    def clearAllCache(self, dfs: bool = False) -> None:
-        """Clear all cache.
-
-        Args:
-            dfs : True: clear cache of all nodes; False (default): only clear the cache of the connected node. Defaults to False.
-        """
-        if dfs:
-            self.run("pnodeRun(clearAllCache)")
-        else:
-            self.run("clearAllCache()")
-
-    @classmethod
-    def enableJobCancellation(cls) -> None:
-        """Enable cancellation of running jobs.
-
-        When this method is enabled, all running jobs (executed with Session.run()) in the process will be canceled immediately. This method can only be executed once for each Session.
-        This method is not supported in high availability secenarios.
-        This method is not recommended in multithreaded mode. In multithreaded mode, make sure the main process of signal is imported before you call this method.
-
-        """
-        if platform.system() == "Linux":
-            ddbcpp.sessionimpl.enableJobCancellation()
-        else:
-            raise RuntimeError("This method is only supported on Linux.")
-
-    @classmethod
-    def setTimeout(cls, timeout: float) -> None:
-        """Set the TCP timeout.
-
-        Args:
-            timeout : corresponds to the TCP_USER_TIMEOUT option. Specify the value in units of seconds. 
-        """
-        ddbcpp.sessionimpl.setTimeout(timeout)
-
-    def nullValueToZero(self) -> None:
-        """Convert all NULL values to 0.
-
-        Deprecated:
-            this method will be deleted in a future version.
-        """
-        self.cpp.nullValueToZero()
-
-    def nullValueToNan(self) -> None:
-        """Convert all NULL values to NumPy NaN.
-
-        Deprecated:
-            this method will be delete in a future version.
-        """
-        self.cpp.nullValueToNan()
-
-    def hashBucket(self, obj, nBucket: int):
-        """Hash map, which maps DolphinDB objects into hash buckets of size nBucket.
-
-        Args:
-            obj : the DolphinDB object to be hashed.
-            nBucket : hash bucket size.
-
-        Returns:
-            hash of the DolphinDB object.
-        """
-        if not isinstance(nBucket, int) or nBucket <= 0:
-            raise ValueError("nBucket must be a positive integer")
-        return self.cpp.hashBucket(obj, nBucket)
-
-    def convertDatetime64(self, datetime64List):
-        length = len(str(datetime64List[0]))
-        # date and month
-        if length == 10 or length == 7:
-            listStr = '['
-            for dt64 in datetime64List:
-                s = str(dt64).replace('-', '.')
-                if len(str(dt64)) == 7:
-                    s += 'M'
-                listStr += s + ','
-            listStr = listStr.rstrip(',')
-            listStr += ']'
-        else:
-            listStr = 'datehour(['
-            for dt64 in datetime64List:
-                s = str(dt64).replace('-', '.').replace('T', ' ')
-                ldt = len(str(dt64))
-                if ldt == 13:
-                    s += ':00:00'
-                elif ldt == 16:
-                    s += ':00'
-                listStr += s + ','
-            listStr = listStr.rstrip(',')
-            listStr += '])'
-        return listStr
-
-    def convertDatabase(self, databaseList):
-        listStr = '['
-        for db in databaseList:
-            listStr += db._getDbName()
-            listStr += ','
-        listStr = listStr.rstrip(',')
-        listStr += ']'
-        return listStr
-
-    def _loadPickleFile(self, filePath):
-        return self.cpp.loadPickleFile(filePath)
-
-    def _printPerformance(self):
-        self.cpp.printPerformance()
-
-
-class BlockReader(object):
-    """Read in blocks.
-
-    Specify the paramter fetchSize for method Session.run and it returns a BlockReader object to read in blocks.
-
-    Args:
-        blockReader : dolphindbcpp object.
-    """
-    def __init__(self, blockReader):
-        """Constructor of BlockReader."""
-        self.block = blockReader
-
-    def read(self):
-        """Read a piece of data.
-
-        Returns:
-            execution result of a script.
-        """
-        return self.block.read()
-
-    def hasNext(self) -> bool:
-        """Check if there is data to be read.
-
-        Returns:
-            True if there is still data not read, otherwise False.
-        """
-        return self.block.hasNext()
-
-    def skipAll(self):
-        """Skip subsequent data.
-
-        Note:
-            When reading data in blocks, if not all blocks are read, please call the skipAll method to abort the reading before executing the subsequent code.
-            Otherwise, data will be stuck in the socket buffer and the deserialization of the subsequent data will fail.
-        """
-        self.block.skipAll()
-
-
-class PartitionedTableAppender(object):
-    """Class for writes to DolphinDB DFS tables.
-
-    Args:
-        dbPath : DFS database path. Defaults to None.
-        tableName : name of a DFS table. Defaults to None.
-        partitionColName : partitioning column. Defaults to None.
-        dbConnectionPool : connection pool. Defaults to None.
-
-    Note:
-        DolphinDB does not allow multiple writers to write data to the same partition at the same time, so when the client writes data in parallel with multiple threads, please ensure that each thread writes to a different partition.
-        The python API provides PartitionedTableAppender, an easy way to automatically split data writes by partition.
-    """
-    def __init__(
-        self, dbPath: str = None, tableName: str = None,
-        partitionColName: str = None, dbConnectionPool: DBConnectionPool = None
-    ):
-        """Constructor of PartitionedTableAppender."""
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        if partitionColName is None:
-            partitionColName = ""
-        if not isinstance(dbConnectionPool, DBConnectionPool):
-            raise Exception("dbConnectionPool must be a dolphindb DBConnectionPool!")
-        self.appender = ddbcpp.partitionedTableAppender(dbPath, tableName, partitionColName, dbConnectionPool.pool)
-        self.pool = dbConnectionPool
-
-    def append(self, table: DataFrame) -> int:
-        """Append data.
-
-        Args:
-            table : data to be written.
-
-        Returns:
-            number of rows written.
-        """
-        if self.pool.is_shutdown():
-            raise RuntimeError("DBConnectionPool has been shut down.")
-        return self.appender.append(table)
-
-
-class TableAppender(object):
-    """Class of table appender.
-
-    As the only temporal data type in Python pandas is datetime64, all temporal columns of a DataFrame are converted into nanotimestamp type after uploaded to DolphinDB.
-    Each time we use tableInsert or insert into to append a DataFrame with a temporal column to an in-memory table or DFS table, we need to conduct a data type conversion for the time column.
-    For automatic data type conversion, Python API offers tableAppender object.
-
-    Args:
-        dbPath : the path of a DFS database. Leave it unspecified for in-memory tables. Defaults to None.
-        tableName : table name. Defaults to None.
-        ddbSession : a Session connected to DolphinDB server. Defaults to None.
-        action : the action when appending. Now only supports "fitColumnType", indicating to convert the data type of temporal column. Defaults to "fitColumnType".
-    """
-    def __init__(self, dbPath: str = None, tableName: str = None, ddbSession: Session = None, action: str = "fitColumnType"):
-        """Constructor of tableAppender"""
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        if not isinstance(ddbSession, Session):
-            raise Exception("ddbSession must be a dolphindb Session!")
-        if action == "fitColumnType":
-            self.tableappender = ddbcpp.autoFitTableAppender(dbPath, tableName, ddbSession.cpp)
-            self.sess = ddbSession
-        else:
-            raise Exception("other action not supported yet!")
-
-    def append(self, table: DataFrame) -> int:
-        """Append data.
-
-        Args:
-            table : data to be written.
-
-        Returns:
-            number of rows written.
-        """
-        if self.sess.isClosed():
-            raise RuntimeError("Session has been closed.")
-        return self.tableappender.append(table)
-
-
-class TableUpserter(object):
-    """Class of table upserter.
-
-    Args:
-        dbPath : the path of a DFS database. Leave it unspecified for in-memory tables. Defaults to None.
-        tableName : table name. Defaults to None.
-        ddbSession : a Session connected to DolphinDB server. Defaults to None.
-        ignoreNull : if set to true, for the NULL values in the new data, the correponding elements in the table are not updated. Defaults to False.
-        keyColNames : key column names. For a DFS table, the columns specified by this parameter are considrd as key columns. Defaults to [].
-        sortColumns : sort column names. All data in the updated partition will be sorted according to the specified column. Defaults to [].
-    """
-    def __init__(
-        self, dbPath: str = None, tableName: str = None,
-        ddbSession: Session = None, ignoreNull: bool = False,
-        keyColNames: List[str] = [], sortColumns: List[str] = []
-    ):
-        """Constructor of tableUpsert."""
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        if not isinstance(ddbSession, Session):
-            raise Exception("ddbSession must be a dolphindb Session!")
-        self.tableupserter = ddbcpp.autoFitTableUpsert(dbPath, tableName, ddbSession.cpp, ignoreNull, keyColNames, sortColumns)
-        self.sess = ddbSession
-
-    def __del__(self):
-        self.tableupserter = None
-
-    def upsert(self, table: DataFrame):
-        """upsert data.
-
-        Args:
-            table : data to be written.
-        """
-        if self.sess.isClosed():
-            raise RuntimeError("Session has been closed.")
-        self.tableupserter.upsert(table)
-
-
-class BatchTableWriter(object):
-    """Class of batch writer for asynchronous batched writes.
-
-    Support batched writes to in-memory table and distributed table.
-
-    Args:
-        host : server address.
-        port : port name.
-        userid : username. Defaults to None.
-        password : password. Defaults to None.
-        acquireLock : whether to acquire a lock in the Python API, True (default) means to acquire a lock. Defaults to True.
-
-    Note:
-        It's required to acquire the lock for concurrent API calls
-    """
-    def __init__(
-        self, host: str, port: int,
-        userid: str = None, password: str = None,
-        acquireLock: bool = True
-    ):
-        """Constructor of BatchTableWriter"""
-        if userid is None:
-            userid = ""
-        if password is None:
-            password = ""
-        self.writer = ddbcpp.batchTableWriter(host, port, userid, password, acquireLock)
-
-    def addTable(
-        self, dbPath: str = None, tableName: str = None,
-        partitioned: bool = True
-    ) -> None:
-        """Add a table to be written to.
-
-        Args:
-            dbPath : the database path for a disk table; leave it empty for an in-memory table. Defaults to None.
-            tableName : table name. Defaults to None.
-            partitioned : whether is a partitioned table. True indicates a partitioned table. Defaults to True.
-
-        Note:
-            If the table is a non-partitioned table on disk, it's required to set partitioned=False.
-        """
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        self.writer.addTable(dbPath, tableName, partitioned)
-
-    def getStatus(self, dbPath: str = None, tableName: str = None) -> Tuple[int, bool, bool]:
-        """Get the current write status.
-
-        Args:
-            dbPath : database name. Defaults to None.
-            tableName : table name. Defaults to None.
-
-        Returns:
-            Tuple[int, bool, bool]: indicating the depth of the current writing queue, whether the current table is being removed (True if being removed), and whether the background thread exits due to an error (True if exits due to an error).
-        """
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        return self.writer.getStatus(dbPath, tableName)
-
-    def getAllStatus(self) -> DataFrame:
-        """Get the status of all tables except for the removed ones.
-
-        Returns:
-        | DatabaseName | TableName | WriteQueueDepth | sentRows | Removing | Finished |
-        | :----------- | :-------- | :-------------- | :------- | :------- | :------- |
-        | 0            | tglobal   | 0               | 5        | False    | False    |
-        """
-        return self.writer.getAllStatus()
-
-    def getUnwrittenData(self, dbPath: str = None, tableName: str = None) -> DataFrame:
-        """Obtain unwritten data. The method is mainly used to obtain the remaining unwritten data if an error occurs when writing.
-
-        Args:
-            dbPath : database name. Defaults to None.
-            tableName : table name. Defaults to None.
-
-        Returns:
-            DataFrame of unwritten data.
-        """
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        return self.writer.getUnwrittenData(dbPath, tableName)
-
-    def removeTable(self, dbPath: str = None, tableName: str = None) -> None:
-        """Release the resources occupied by the table added by the addTable method. The first time the method is called, it returns if the thread has exited.
-
-        Args:
-            dbPath : database name. Defaults to None.
-            tableName : table name. Defaults to None.
-        """
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        self.writer.removeTable(dbPath, tableName)
-
-    def insert(self, dbPath: str = None, tableName: str = None, *args):
-        """Insert a single row of data
-
-        Args:
-            dbPath : database name. Defaults to None.
-            tableName : table name. Defaults to None.
-            args : variable-length argument, indicating a row of data to be inserted.
-        """
-        if dbPath is None:
-            dbPath = ""
-        if tableName is None:
-            tableName = ""
-        self.writer.insert(dbPath, tableName, *args)
-
-
-class ErrorCodeInfo(object):
-    """MTW error codes and messages.
-
-    Args:
-        errorCode : error code. Defaults to None.
-        errorInfo : error information. Defaults to None.
-    """
-    def __init__(self, errorCode=None, errorInfo=None):
-        """Constructor of ErrorCodeInfo."""
-        self.errorCode = errorCode
-        self.errorInfo = errorInfo
-
-    def __repr__(self):
-        errorCodeText = ""
-        if self.hasError():
-            errorCodeText = self.errorCode
-        else:
-            errorCodeText = None
-        outStr = "errorCode: %s\n" % errorCodeText
-        outStr += " errorInfo: %s\n" % self.errorInfo
-        outStr += object.__repr__(self)
-        return outStr
-
-    def hasError(self) -> bool:
-        """Check if an error has occurred.
-
-        Returns:
-            True if an error occurred, otherwise False.
-        """
-        return self.errorCode is not None and len(self.errorCode) > 0
-
-    def succeed(self) -> bool:
-        """Check if data has been written successfully.
-
-        Returns:
-            True if the write is successful, otherwise False.
-        """
-        return self.errorCode is None or len(self.errorCode) < 1
-
-
-class MultithreadedTableWriterThreadStatus(object):
-    """Get the status of MTW.
-
-    Args:
-        threadId: thread ID.
-
-    Attribute:
-        threadId : thread ID.
-        sentRows : number of sent rows.
-        unsentRows : number of rows to be sent.
-        sendFailedRows : number of rows failed to be sent.
-
-    """
-    def __init__(self, threadId: int = None):
-        """Constructor of MultithreadedTableWriterThreadStatus."""
-        self.threadId = threadId
-        self.sentRows = None
-        self.unsentRows = None
-        self.sendFailedRows = None
-
-
-class MultithreadedTableWriterStatus(ErrorCodeInfo):
-    """The status information of MTW.
-
-    Attribute:
-        isExiting : whether the threads are exiting.
-        sentRows : number of sent rows.
-        unsentRows : number of rows to be sent.
-        sendFailedRows : number of rows failed to be sent.
-        threadStatus : a list of the thread status.
-    """
-    def __init__(self):
-        """Constructor of MultithreadedTableWriterStatus."""
-        self.isExiting = None
-        self.sentRows = None
-        self.unsentRows = None
-        self.sendFailedRows = None
-        self.threadStatus = []
-
-    def update(self, statusDict):
-        threadStatusDict = statusDict["threadStatus"]
-        del statusDict["threadStatus"]
-        self.__dict__.update(statusDict)
-        for oneThreadStatusDict in threadStatusDict:
-            oneThreadStatus = MultithreadedTableWriterThreadStatus()
-            oneThreadStatus.__dict__.update(oneThreadStatusDict)
-            self.threadStatus.append(oneThreadStatus)
-
-    def __repr__(self):
-        errorCodeText = ""
-        if self.hasError():
-            errorCodeText = self.errorCode
-        else:
-            errorCodeText = None
-        outStr = "%-14s: %s\n" % ("errorCode", errorCodeText)
-        if self.errorInfo is not None:
-            outStr += " %-14s: %s\n" % ("errorInfo", self.errorInfo)
-        if self.isExiting is not None:
-            outStr += " %-14s: %s\n" % ("isExiting", self.isExiting)
-        if self.sentRows is not None:
-            outStr += " %-14s: %s\n" % ("sentRows", self.sentRows)
-        if self.unsentRows is not None:
-            outStr += " %-14s: %s\n" % ("unsentRows", self.unsentRows)
-        if self.sendFailedRows is not None:
-            outStr += " %-14s: %s\n" % ("sendFailedRows", self.sendFailedRows)
-        if self.threadStatus is not None:
-            outStr += " %-14s: \n" % "threadStatus"
-            outStr += " \tthreadId\tsentRows\tunsentRows\tsendFailedRows\n"
-            for thread in self.threadStatus:
-                outStr += "\t"
-                if thread.threadId is not None:
-                    outStr += "%8d" % thread.threadId
-                outStr += "\t"
-                if thread.sentRows is not None:
-                    outStr += "%8d" % thread.sentRows
-                outStr += "\t"
-                if thread.unsentRows is not None:
-                    outStr += "%10d" % thread.unsentRows
-                outStr += "\t"
-                if thread.sendFailedRows is not None:
-                    outStr += "%14d" % thread.sendFailedRows
-                outStr += "\n"
-        outStr += object.__repr__(self)
-        return outStr
-
-
-class MultithreadedTableWriter(object):
-    """A multi-threaded writer is an ungrade of BatchTableWriter with support for multi-threaded concurrent writes.
-
-    Args:
-        host : host name.
-        port : port number.
-        userId : username.
-        password : password.
-        dbPath : the DFS database path or in-memory table name.
-        tableName : the DFS table name. Leave it unspecified for an in-memory table.
-        useSSL : whether to enable SSL. Defaults to False.
-        enableHighAvailability : whether to enable high availability. Defaults to False.
-        highAvailabilitySites : a list of "ip:port" of all available nodes. Defaults to [].
-        batchSize : the number of messages in batch processing. Defaults to 1.
-        throttle : the waiting time (in seconds) before the server processes the incoming data if the number of data written from the client does not reach batchSize. Defaults to 1.
-        threadCount : the number of working threads to be created. Defaults to 1.
-        partitionCol : a string indicating the partitioning column, the default is an empty string. The parameter only takes effect when threadCount>1. Defaults to "".
-                        For a partitioned table, it must be the partitioning column; for a stream table, it must be a column name; for a dimension table, the parameter does not work.
-        compressMethods : a list of the compression methods used for each column. If unspecified, the columns are not compressed. Defaults to []. 
-                            The compression methods include: "LZ4": LZ4 algorithm; "DELTA": Delta-of-delta encoding.
-        mode : The write mode. It can be Append (default) or Upsert. Defaults to "".
-        modeOption : The parameters of function upsert!. It only takes effect when mode is Upsert. Defaults to [].
-    """
-    def __init__(
-        self, host: str, port: int, userId: str, password: str,
-        dbPath: str, tableName: str, useSSL: bool = False,
-        enableHighAvailability: bool = False, highAvailabilitySites: List[str] = [],
-        batchSize: int = 1, throttle: float = 1.0, threadCount: int = 1,
-        partitionCol: str = "", compressMethods: List[str] = [],
-        mode: str = "", modeOption: List[str] = []
-    ):
-        """Constructor of MultithreadedTableWriter"""
-        self.writer = ddbcpp.multithreadedTableWriter(
-            host, port, userId, password, dbPath, tableName, useSSL,
-            enableHighAvailability, highAvailabilitySites, batchSize, throttle, threadCount,
-            partitionCol, compressMethods, mode, modeOption
-        )
-
-    def getStatus(self) -> MultithreadedTableWriterStatus:
-        """Get the current writer status and return a MultithreadedTableWriterStatus object.
-
-        Returns:
-            MultithreadedTableWriterStatus object.
-        """
-        status = MultithreadedTableWriterStatus()
-        status.update(self.writer.getStatus())
-        return status
-
-    def getUnwrittenData(self) -> List[List[Any]]:
-        """Get unwritten data.
-
-        The obtained data can be passed as an argument to method insertUnwrittenData.
-
-        Returns:
-            a nested list where each element is a record.
-        """
-        return self.writer.getUnwrittenData()
-
-    def insert(self, *args) -> ErrorCodeInfo:
-        """Insert a single row of data.
-
-        Args:
-            args : variable-length argument, indicating a row of data to be inserted.
-
-        Returns:
-            a ErrorCodeInfo object.
-        """
-        errorCodeInfo = ErrorCodeInfo()
-        errorCodeInfo.__dict__.update(self.writer.insert(*args))
-        return errorCodeInfo
-
-    def insertUnwrittenData(self, unwrittenData) -> ErrorCodeInfo:
-        """Insert unwritten data.
-
-        The result is in the same format as insert.
-        The difference is that insertUnwrittenData can insert multiple records at a time.
-
-        Args:
-            unwrittenData : the data that has not been written to the server. You can obtain the object with method getUnwrittenData.
-
-        Returns:
-            ErrorCodeInfo object
-        """
-        errorCodeInfo = ErrorCodeInfo()
-        errorCodeInfo.__dict__.update(self.writer.insertUnwrittenData(unwrittenData))
-        return errorCodeInfo
-
-    def waitForThreadCompletion(self) -> None:
-        """Wait until all working threads complete their tasks.
-
-        After calling the method, MultithreadedTableWriter will wait until all working threads complete their tasks.
-
-        """
-        self.writer.waitForThreadCompletion()
+"""Session
+Package: session package.
+        including classes Session, DBConnectionPool, BatchTableWriter, MultithreadedTableWriter
+"""
+
+
+import asyncio
+import platform
+import re
+import warnings
+from concurrent.futures import Future
+from datetime import date, datetime
+from threading import Lock, Thread
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+
+import numpy as np
+from dolphindb._core import DolphinDBRuntime
+from dolphindb.database import Database
+from dolphindb.settings import (DDB_EPSILON, PROTOCOL_ARROW, PROTOCOL_DDB,
+                                PROTOCOL_DEFAULT, PROTOCOL_PICKLE)
+from dolphindb.table import Table
+from dolphindb.utils import _generate_dbname, _generate_tablename, month
+from pandas import DataFrame
+
+ddbcpp = DolphinDBRuntime()._ddbcpp
+
+
+class DBConnectionPool(object):
+    """DBConnectionPool is the connection pool object where multiple threads can be created to execute scripts in parallel and improve task efficiency.
+
+    Note:
+        To improve efficiency, methods such as run of class DBConnectionPool are packaged into coroutine functions in python.
+
+    Args:
+        host : server address. It can be IP address, domain, or LAN hostname, etc.
+        port : port name.
+        threadNum : number of threads. Defaults to 10.
+        userid : username. Defaults to None.
+        password : password. Defaults to None.
+        loadBalance : whether to enable load balancing. True means enabled (the connections will be distributed evenly across the cluster), otherwise False. Defaults to False.
+        highAvailability : whether to enable high availability. True means enabled, otherwise False. Defaults to False.
+        compress : whether to enable compression. True means enabled, otherwise False. Defaults to False.
+        reConnect : whether to enable reconnection. True means enabled, otherwise False. Defaults to False.
+        enablePickle : whether to enable the Pickle protocol. Defaults to False.
+        python : whether to enable the Python parser. True means enabled, otherwise False. Defaults to False.
+        protocol : the data transmission protocol. Defaults to PROTOCOL_DEFAULT, which is equivalant to PROTOCOL_PICKLE.
+
+    Kwargs:
+        show_output : whether to display the output of print statements in the script after execution. Defaults to True.
+
+    Note:
+        If the parameter python is True, the script is parsed in Python rather than DolphinDB language.
+    """
+    def __init__(
+        self, host: str, port: int, threadNum: int = 10, userid: str = None, password: str = None,
+        loadBalance: bool = False, highAvailability: bool = False, compress: bool = False,
+        reConnect: bool = False, python: bool = False, protocol: int = PROTOCOL_DEFAULT,
+        *, show_output: bool = True
+    ):
+        """Constructor of DBConnectionPool, including the number of threads, load balancing, high availability, reconnection, compression and Pickle protocol."""
+        userid = userid if userid is not None else ""
+        password = password if password is not None else ""
+        if protocol == PROTOCOL_DEFAULT:
+            protocol = PROTOCOL_PICKLE
+        if protocol not in [PROTOCOL_DEFAULT, PROTOCOL_DDB, PROTOCOL_PICKLE, PROTOCOL_ARROW]:
+            raise RuntimeError(f"Protocol {protocol} is not supported. ")
+
+        if protocol == PROTOCOL_ARROW and compress:
+            raise RuntimeError("The Arrow protocol does not support compression.")
+
+        if protocol == PROTOCOL_ARROW:
+            __import__("pyarrow")
+
+        self.mutex = Lock()
+        self.pool = ddbcpp.dbConnectionPoolImpl(host, port, threadNum, userid, password, loadBalance, highAvailability, compress, reConnect, python, protocol, show_output)
+        self.host = host
+        self.port = port
+        self.userid = userid
+        self.password = password
+        self.taskId = 0
+        self.loop = None
+        self.thread = None
+        self.protocol = protocol
+        self.shutdown_flag = False
+
+    def __del__(self):
+        if hasattr(self, "pool") and self.pool is not None:
+            self.shutDown()
+
+    async def run(self, script: str, *args, **kwargs):
+        """Coroutine function.
+
+        Pass the script to the connection pool to call the thread execution with the run method.
+
+        Args:
+            script : DolphinDB script to be executed.
+            args : arguments to be passed to the function.
+
+        Note:
+            args is only required when script is the function name.
+
+        Kwargs:
+            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
+            pickleTableToList : whether to convert table to list or DataFrame. True: to list, False: to DataFrame. Defaults to False.
+            priority : a job priority system with 10 priority levels (0 to 9), allocating thread resources to high-priority jobs and using round-robin allocation for jobs of the same priority. Defaults to 4.
+            parallelism : parallelism determines the maximum number of threads to execute a job's tasks simultaneously on a data node; the system optimizes resource utilization by allocating all available threads to a job if there's only one job running and multiple local executors are available. Defaults to 2.
+
+        Returns:
+            execution result.
+
+        Note:
+            When setting pickleTableToList=True and enablePickle=True, if the table contains array vectors, it will be converted to a NumPy 2d array.
+            If the length of each row is different, the execution fails.
+        """
+        priority = kwargs.get('priority', 4)
+        parallelism = kwargs.get('parallelism', 2)
+        if type(priority) is not int or priority > 9 or priority < 0:
+            raise RuntimeError("priority must be an integer from 0 to 9")
+        if type(parallelism) is not int or parallelism <= 0:
+            raise RuntimeError("parallelism must be an integer greater than 0")
+
+        self.mutex.acquire()
+        self.taskId = self.taskId + 1
+        tid = self.taskId
+        self.mutex.release()
+        if "clearMemory" not in kwargs.keys():
+            kwargs["clearMemory"] = True
+        self.pool.run(script, tid, *args, **kwargs)
+        while True:
+            isFinished = self.pool.isFinished(tid)
+            if isFinished == 0:
+                await asyncio.sleep(0.01)
+            else:
+                return self.pool.getData(tid)
+
+    def addTask(self, script: str, taskId: int, *args, **kwargs):
+        """Add a task and specify the task ID to execute the script.
+
+        Args:
+            script : script to be executed.
+            taskId : the task ID.
+            args : arguments to be passed to the function.
+
+        Note:
+            args is only required when script is the function name.
+
+        Kwargs:
+            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
+
+        Returns:
+            execution result.
+        """
+        if "clearMemory" not in kwargs.keys():
+            kwargs["clearMemory"] = True
+        return self.pool.run(script, taskId, *args, **kwargs)
+
+    def isFinished(self, taskId: int) -> bool:
+        """Get the completion status of the specified task.
+
+        Args:
+            taskId : the task ID.
+
+        Returns:
+            True if the task is finished, otherwise False.
+        """
+        return self.pool.isFinished(taskId)
+
+    def getData(self, taskId: int):
+        """Get data of the specified task.
+
+        Args:
+            taskId : the task ID.
+
+        Returns:
+            data of the task.
+
+        Note:
+            For each task, the data can only be obtained once and will be cleared immediately after the data is obtained.
+        """
+        return self.pool.getData(taskId)
+
+    def __start_thread_loop(self, loop):
+        asyncio.set_event_loop(loop)
+        loop.run_forever()
+
+    def startLoop(self):
+        """Create and start an event loop.
+
+        Raises:
+            the event loop has been created.
+        """
+        if self.loop is not None:
+            raise RuntimeError("Event loop is already started!")
+        self.loop = asyncio.new_event_loop()
+        self.thread = Thread(target=self.__start_thread_loop, args=(self.loop,))
+        self.thread.setDaemon(True)
+        self.thread.start()
+
+    async def stopLoop(self):
+        """Stop the event loop."""
+        await asyncio.sleep(0.01)
+        self.loop.stop()
+
+    def runTaskAsync(self, script: str, *args, **kwargs) -> Future:
+        """Execute script tasks asynchronously.
+
+        Args:
+            script : script to be executed.
+            args : arguments to be passed to the function.
+
+        Kwargs:
+            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
+
+        Returns:
+            concurrent.futures.Future object for receiving data.
+        """
+        if self.loop is None:
+            self.startLoop()
+        if "clearMemory" not in kwargs.keys():
+            kwargs["clearMemory"] = True
+        task = asyncio.run_coroutine_threadsafe(self.run(script, *args, **kwargs), self.loop)
+        return task
+
+    def runTaskAsyn(self, script: str, *args, **kwargs) -> Future:
+        """Execute script tasks asynchronously.
+
+        Deprecated:
+            Please use runTaskAsync instead of runTaskAsyn.
+
+        Args:
+            script : script to be executed.
+            args : arguments to be passed to the function.
+
+        Kwargs:
+            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to True.
+
+        Returns:
+            concurrent.futures.Future object for receiving data.
+        """
+        if "clearMemory" not in kwargs.keys():
+            kwargs["clearMemory"] = True
+        warnings.warn("Please use runTaskAsync instead of runTaskAsyn.", DeprecationWarning, stacklevel=2)
+        return self.runTaskAsync(script, *args, **kwargs)
+
+    def shutDown(self):
+        """Close the DBConnectionPool, stop the event loop and terminate all asynchronous tasks."""
+        with self.mutex:
+            if self.shutdown_flag:
+                return
+            self.shutdown_flag = True
+        self.host = None
+        self.port = None
+        if self.loop is not None:
+            asyncio.run_coroutine_threadsafe(self.stopLoop(), self.loop)
+            self.thread.join()
+            if self.loop.is_running():
+                self.loop.stop()
+            else:
+                self.loop.close()
+        if self.pool is not None:
+            self.pool.shutDown()
+            self.pool = None
+        self.loop = None
+        self.thread = None
+
+    def getSessionId(self) -> List[str]:
+        """Obtain Session ID of all sessions.
+
+        Returns:
+            list of thread ID.
+        """
+        return self.pool.getSessionId()
+
+    def is_shutdown(self) -> bool:
+        with self.mutex:
+            return self.shutdown_flag
+
+
+class streamDeserializer(object):
+    """Deserializer stream blob in multistreamingtable reply.
+
+    Args:
+        sym2table : a dict object indicating the corresponding relationship between the unique identifiers of the tables and the table objects.
+        session : a Session object. Defaults to None.
+    """
+    def __init__(self, sym2table: Dict[str, Union[List[str], str]], session=None):
+        """Constructor of streamDeserializer."""
+        self.cpp = ddbcpp.streamDeserializer(sym2table)
+        if session is not None:
+            self.cpp.setSession(session.cpp)
+
+
+class Session(object):
+    """Session is the connection object to execute scripts.
+
+    Args:
+        host : server address. It can be IP address, domain, or LAN hostname, etc. Defaults to None.
+        port : port name. Defaults to None.
+
+    Note:
+        If neither host nor port is set to None, a connection will be established.
+
+    Args:
+        userid : username. Defaults to "", meaning not to log in.
+        password : password. Defaults to "", meaning not to log in.
+        enableSSL : whether to enable SSL. True means to enable SSL. Defaults to False.
+        enableASYNC(enableASYN) : whether to enable asynchronous communication. Defaults to False.
+
+    Deprecated:
+        Please use enableASYNC instead of enableASYN.
+
+    Args:
+        keepAliveTime : the duration between two keepalive transmissions to detect the TCP connection status. Defaults to 30 (seconds). Set the parameter to release half-open TCP connections timely when the network is unstable.
+        enableChunkGranularityConfig : whether to enable chunk granularity configuration. Defaults to False.
+        compress : whether to enable compressed communication. Defaults to False.
+        enablePickle : whether to enable the Pickle protocol. Defaults to True.
+        protocol: the data transmission protocol. Defaults to PROTOCOL_DEFAULT, which is equivalant to PROTOCOL_PICKLE.
+        python : whether to enable python parser. Defaults to False.
+
+    Kwargs:
+        show_output : whether to display the output of print statements in the script after execution. Defaults to True.
+
+    Note:
+        set enableSSL =True to enable encrypted communication. It's also required to configure enableHTTPS =true in the server.
+
+    Note:
+        set enableASYNC =True to enable asynchronous mode and the communication with the server can only be done through the session.run method. As there is no return value, it is suitable for asynchronous writes.
+    """
+    def __init__(
+        self, host: Optional[str] = None, port: Optional[int] = None,
+        userid: Optional[str] = "", password: Optional[str] = "", enableSSL: bool = False,
+        enableASYNC: bool = False, keepAliveTime: int = 30, enableChunkGranularityConfig: bool = False,
+        compress: bool = False, enablePickle: bool = None, protocol: int = PROTOCOL_DEFAULT,
+        python: bool = False, *, show_output: bool = True, **kwargs
+    ):
+        """Constructor of Session, inluding OpenSSL encryption, asynchronous mode, TCP detection, block granularity matching, compression, Pickle protocol."""
+        if 'enableASYN' in kwargs.keys():
+            enableASYNC = kwargs['enableASYN']
+            warnings.warn("Please use enableASYNC instead of enableASYN.", DeprecationWarning, stacklevel=2)
+
+        default_protocol = PROTOCOL_PICKLE
+        if protocol == PROTOCOL_DEFAULT:
+            protocol = PROTOCOL_PICKLE if enablePickle else PROTOCOL_DDB
+            if enablePickle is None:
+                protocol = default_protocol
+        elif enablePickle:
+            raise RuntimeError("When enablePickle=true, the parameter protocol must not be specified. ")
+
+        if protocol not in [PROTOCOL_DEFAULT, PROTOCOL_DDB, PROTOCOL_PICKLE, PROTOCOL_ARROW]:
+            raise RuntimeError(f"Protocol {protocol} is not supported. ")
+
+        if protocol == PROTOCOL_ARROW and compress:
+            raise RuntimeError("The Arrow protocol does not support compression.")
+
+        if protocol == PROTOCOL_ARROW:
+            __import__("pyarrow")
+
+        self.cpp = ddbcpp.sessionimpl(enableSSL, enableASYNC, keepAliveTime, compress, python, protocol, show_output)
+        self.host = host
+        self.port = port
+        self.userid = userid
+        self.password = password
+        self.mutex = Lock()
+        self.enableEncryption = True
+        self.enableChunkGranularityConfig = enableChunkGranularityConfig
+        self.enablePickle = enablePickle
+        self.protocol = protocol
+        if self.host is not None and self.port is not None:
+            self.connect(host, port, userid, password, keepAliveTime=keepAliveTime)
+
+    def __del__(self):
+        if hasattr(self, "cpp"):
+            self.cpp.close()
+
+    def connect(
+        self, host: str, port: int, userid: str = None, password: str = None, startup: str = None,
+        highAvailability: bool = False, highAvailabilitySites: Optional[List[str]] = None,
+        keepAliveTime: Optional[int] = None, reconnect: bool = False
+    ) -> bool:
+        """Establish connection, including initialization script, high availability, TCP detection.
+
+        Args:
+            host : server address. It can be IP address, domain, or LAN hostname, etc.
+            port : port name.
+            userid : username. Defaults to None, indicating no login.
+            password : password. Defaults to None, indicating no login..
+            startup : the startup script to execute the preloaded tasks immediately after the connection is established. Defaults to None.
+            highAvailability : whether to enable high availability. True means enabled, otherwise False. Defaults to False.
+            highAvailabilitySites : a list of high-availability nodes. Defaults to None.
+            keepAliveTime : the duration between two keepalive transmissions to detect the TCP connection status. Defaults to None, meaning keepAliveTime = 30 (seconds). Set the parameter to release half-open TCP connections timely when the network is unstable.
+            reconnect : whether to enable reconnection. True means enabled, otherwise False. Defaults to False.
+
+        Returns:
+            whether the connection is established. True if established, otherwise False.
+        """
+        if highAvailabilitySites is None:
+            highAvailabilitySites = []
+        if keepAliveTime is None:
+            keepAliveTime = -1
+        if userid is None:
+            userid = ""
+        if password is None:
+            password = ""
+        if startup is None:
+            startup = ""
+        if self.cpp.connect(host, port, userid, password, startup, highAvailability, highAvailabilitySites, keepAliveTime, reconnect):
+            self.host = host
+            self.port = port
+            self.userid = userid
+            self.password = password
+            return True
+        else:
+            return False
+
+    def login(self, userid: str, password: str, enableEncryption: bool = True):
+        """Manually log in to the server.
+
+        Args:
+            userid : username.
+            password : password.
+            enableEncryption : whether to enable encrypted transmission for username and password. Defaults to True.
+
+        Note:
+            Specify the userid and password in the connect() method to log in automatically.
+        """
+        self.mutex.acquire()
+        try:
+            self.userid = userid
+            self.password = password
+            self.enableEncryption = enableEncryption
+            self.cpp.login(userid, password, enableEncryption)
+        finally:
+            self.mutex.release()
+
+    def close(self):
+        """Close Session connection."""
+        self.host = None
+        self.port = None
+        self.cpp.close()
+
+    def isClosed(self) -> bool:
+        """Check if the current Session has been closed.
+
+        Returns:
+            bool: True if closed, otherwise False.
+        """
+        return self.host is None
+
+    def upload(self, nameObjectDict):
+        """Upload Python objects to DolphinDB server.
+
+        Args:
+            nameObjectDict : Python dictionary object. The keys of the dictionary are the variable names in DolphinDB and the values are Python objects, which can be numbers, strings, lists, DataFrame, etc.
+
+        Returns:
+            the server address of the uploaded object.
+
+        Note:
+            A pandas DataFrame corresponds to DolphinDB table.
+        """
+        return self.cpp.upload(nameObjectDict)
+
+    def run(self, script: str, *args, **kwargs):
+        """Execute script.
+
+        Args:
+            script : DolphinDB script to be executed.
+            args : arguments to be passed to the function.
+
+        Note:
+            args is only required when script is the function name.
+
+        Kwargs:
+            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to False.
+            pickleTableToList : whether to convert table to list or DataFrame. True: to list, False: to DataFrame.  Defaults to False.
+            priority : a job priority system with 10 priority levels (0 to 9), allocating thread resources to high-priority jobs and using round-robin allocation for jobs of the same priority. Defaults to 4.
+            parallelism : parallelism determines the maximum number of threads to execute a job's tasks simultaneously on a data node; the system optimizes resource utilization by allocating all available threads to a job if there's only one job running and multiple local executors are available. Defaults to 2.
+            fetchSize : the size of a block.
+
+        Note:
+            fetchSize cannot be less than 8192 Bytes.
+
+        Returns:
+            execution result. If fetchSize is specified, a BlockReader object will be returned. Each block can be read with the read() method.
+
+        Note:
+            When setting pickleTableToList=True and enablePickle=True, if the table contains array vectors, it will be converted to a NumPy 2d array. If the length of each row is different, the execution fails.
+        """
+        priority = kwargs.get('priority', 4)
+        parallelism = kwargs.get('parallelism', 2)
+        if type(priority) is not int or priority > 9 or priority < 0:
+            raise RuntimeError("priority must be an integer from 0 to 9")
+        if type(parallelism) is not int or parallelism <= 0:
+            raise RuntimeError("parallelism must be an integer greater than 0")
+
+        if kwargs:
+            if "fetchSize" in kwargs.keys():
+                return BlockReader(self.cpp.runBlock(script, **kwargs))
+        return self.cpp.run(script, *args, **kwargs)
+
+    def runFile(self, filepath: str, *args, **kwargs):
+        """Execute script.
+
+        Args:
+            filepath : the path of the file on the server to be executed.
+            args : arguments to be passed to the function.
+
+        Note:
+            args is only required when script is the function name.
+
+        Kwargs:
+            clearMemory : whether to release variables after queries. True means to release, otherwise False. Defaults to False.
+            pickleTableToList : whether to convert table to list or DataFrame. True: to list, False: to DataFrame.  Defaults to False.
+
+        Returns:
+            execution result.
+
+        Note:
+            When setting pickleTableToList=True and enablePickle=True, if the table contains array vectors, it will be converted to a NumPy 2d array. If the length of each row is different, the execution fails.
+        """
+        with open(filepath, "r") as fp:
+            script = fp.read()
+            return self.run(script, *args, **kwargs)
+
+    def getSessionId(self) -> str:
+        """Get the Session ID of the current Session.
+
+        Returns:
+            Session ID.
+        """
+        return self.cpp.getSessionId()
+
+    def enableStreaming(self, port: int = 0, threadCount: int = 1) -> None:
+        """Enable streaming.
+
+        Args:
+            port : the subscription port for incoming data. The server will connect to the port automatically.
+            threadCount : the number of threads. Defaults to 1.
+
+        Note:
+            If the server you're connecting to supports transferring subscribed data using the connection initiated by the subsriber, 
+            do not specify this port. Otherwise, the port must be specified.
+
+        """
+        self.cpp.enableStreaming(port, threadCount)
+
+    def subscribe(
+        self, host: str, port: int, handler: Callable, tableName: str, actionName: str = None,
+        offset: int = -1, resub: bool = False, filter=None,
+        msgAsTable: bool = False, batchSize: int = 0, throttle: float = 1.0,
+        userName: str = None, password: str = None, streamDeserializer: Optional["streamDeserializer"] = None,
+        backupSites: List[str] = None,
+        resubTimeout: int = 100,
+        subOnce: bool = False,
+    ) -> None:
+        """Subscribe to stream tables in DolphinDB.
+
+        Args:
+            host : server address. It can be IP address, domain, or LAN hostname, etc.
+            port : port name.
+            handler : user-defined callback function for processing incoming data.
+            tableName : name of the published table.
+            actionName : name of the subscription task. Defaults to "".
+            offset : an integer indicating the position of the first message where the subscription begins. Defaults to -1.
+
+        Note:
+            If offset is -1 or exceeding the number of rows in the stream table, the subscription starts with the next new message. It cannot be other negative values.
+
+        Args:
+            resub : True means to keep trying to subscribe to table after the subscription attempt fails. Defaults to False.
+            filter : a vector indicating the filtering columns. Only the rows with values of the filtering column in the vector are published to the subscriber. Defaults to None.
+            msgAsTable : whether to convert the subscribed data to dataframe. If msgAsTable = True, the subscribed data is ingested into handler as a DataFrame. Defaults to False, which means the subscribed data is ingested into handler as a List of nparrays. This optional parameter has no effect if batchSize is not specified.
+            batchSize : an integer indicating the number of unprocessed messages to trigger the handler. If it is positive, the handler does not process messages until the number of unprocessed messages reaches batchSize. If it is unspecified or non-positive, the handler processes incoming messages as soon as they come in. Defaults to 0.
+            throttle : a float indicating the maximum waiting time (in seconds) before the handler processes the incoming messages. Defaults to 1. This optional parameter has no effect if batchSize is not specified.
+            userName : username. Defaults to None, indicating no login.
+            password : password. Defaults to None, indicating no login.
+            streamDeserializer : a deserializer of heterogeneous stream table. Defaults to None.
+            backupSites : a list of strings indicating the host:port for each backup node, e.g. ["192.168.0.1:8848", "192.168.0.2:8849"]. If specified, the failover mechanism is automatically activated. Defaults to None.
+            resubTimeout : an integer representing the timeout for resubscribing (in milliseconds). Defaults to 100.
+            subOnce : a boolean, indicating whether to attempt reconnecting to disconnected nodes after each node switch occurs. Defaults to False.
+        """
+        if not isinstance(msgAsTable, bool):
+            raise TypeError("msgAsTable must be a bool.")
+        if not isinstance(batchSize, int):
+            raise TypeError("batchSize must be a int.")
+        if not isinstance(throttle, float) and not isinstance(throttle, int):
+            raise TypeError("throttle must be a float or a int.")
+        if throttle <= DDB_EPSILON:
+            raise ValueError("throttle must be greater than 0.")
+        if filter is None:
+            filter = np.array([], dtype='int64')
+        if actionName is None:
+            actionName = ""
+        if userName is None:
+            userName = ""
+        if password is None:
+            password = ""
+        sd = None
+        if streamDeserializer is None:
+            sd = ddbcpp.streamDeserializer({})
+        else:
+            sd = streamDeserializer.cpp
+        if backupSites is None:
+            backupSites = []
+        if not isinstance(backupSites, list):
+            raise TypeError("backupSites must be a list of str.")
+        for site in backupSites:
+            if not isinstance(site, str):
+                raise TypeError("backupSites must be a list of str.")
+        if not isinstance(resubTimeout, int):
+            raise TypeError("resubTimeout must be an int.")
+        if not isinstance(subOnce, bool):
+            raise TypeError("subOnce must be a bool.")
+        if batchSize > 0:
+            self.cpp.subscribeBatch(
+                host, port, handler, tableName, actionName,
+                offset, resub, filter, msgAsTable, batchSize, throttle,
+                userName, password, sd, backupSites, resubTimeout, subOnce
+            )
+        else:
+            if msgAsTable:
+                raise ValueError("msgAsTable must be False when batchSize is 0")
+            self.cpp.subscribe(
+                host, port, handler, tableName, actionName,
+                offset, resub, filter, userName, password, sd, backupSites, resubTimeout, subOnce
+            )
+
+    def unsubscribe(self, host: str, port: int, tableName: str, actionName: str = None) -> None:
+        """Unsubscribe.
+
+        Args:
+            host : server address. It can be IP address, domain, or LAN hostname, etc.
+            port : port name.
+            tableName : name of the published table.
+            actionName : name of the subscription task. Defaults to None.
+        """
+        if actionName is None:
+            actionName = ""
+        self.cpp.unsubscribe(host, port, tableName, actionName)
+
+    def getSubscriptionTopics(self) -> List[str]:
+        """Get all subscription topics.
+
+        Returns:
+            a list of all subscription topics in the format of "host/port/tableName/actionName".
+        """
+        return self.cpp.getSubscriptionTopics()
+
+    def getInitScript(self) -> str:
+        """Get the init script of the Session.
+
+        Returns:
+            string of the init script.
+        """
+        return self.cpp.getInitScript()
+
+    def setInitScript(self, script: str) -> None:
+        """Set up init script of the Session.
+
+        Args:
+            string of the init script.
+        """
+        self.cpp.setInitScript(script)
+
+    def saveTable(self, tbl: Table, dbPath: str) -> bool:
+        """Save the table.
+
+        Args:
+            tbl : DolphinDB Table object of the in-memory table to be saved.
+            dbPath : DolphinDB database path.
+
+        Returns:
+            True.
+        """
+        tblName = tbl.tableName()
+        dbName =  _generate_dbname()
+        s1 = dbName+"=database('"+dbPath+"')"
+        self.run(s1)
+        s2 = "saveTable(%s, %s)" % (dbName, tblName)
+        self.run(s2)
+        return True
+
+    def loadText(self,  remoteFilePath: str, delimiter: str = ",") -> "Table":
+        """Import text files into DolphinDB as an in-memory table.
+
+        Args:
+            remoteFilePath : the remote file path on the server. Defaults to None.
+            delimiter : delimiter, Defaults to ",".
+
+        Returns:
+            a DolphinDB in-memory Table object.
+
+        Note:
+            The amount of data loaded into the in-memory table must be less than the available memory.
+        """
+        tableName = _generate_tablename()
+        runstr = tableName + '=loadText("' + remoteFilePath + '","' + delimiter + '")'
+        self.run(runstr)
+        return Table(data=tableName, s=self, isMaterialized=True)
+
+    def loadTextEx(
+        self, dbPath: str, tableName: str, partitionColumns: Optional[List[str]] = None,
+        remoteFilePath: str = None, delimiter: str = ",", sortColumns: Optional[List[str]] = None,
+    ) -> "Table":
+        """Import a partitioned in-memory table.
+
+        Args:
+            dbPath : database path.
+            tableName : table name.
+            partitionColumns : list of strings indicating the partitioning columns. Defaults to None.
+            remoteFilePath : remote file path. Defaults to None.
+            delimiter : delimiter of each column. Defaults to ",".
+            sortColumns : list of strings indicating the sort columns. Defaults to None.
+
+        Returns:
+            a DolphinDB Table object.
+        """
+        if partitionColumns is None:
+            partitionColumns = []
+        if sortColumns is None:
+            sortColumns = []
+        isDBPath = True
+        if "/" in dbPath or "\\" in dbPath or "dfs://" in dbPath:
+            dbstr = 'db=database("' + dbPath + '")'
+            self.run(dbstr)
+            tbl_str = '{tableNameNEW} = loadTextEx(db, "{tableName}", {partitionColumns}, "{remoteFilePath}", {delimiter} {extraParams})'
+        else:
+            isDBPath = False
+            tbl_str = '{tableNameNEW} = loadTextEx("{dbPath}", "{tableName}", {partitionColumns}, "{remoteFilePath}", {delimiter} {extraParams})'
+        fmtDict = dict()
+        fmtDict['tableNameNEW'] = _generate_tablename()
+        fmtDict['dbPath'] = dbPath
+        fmtDict['tableName'] = tableName
+        fmtDict['partitionColumns'] = '[' + ','.join([f'"{_}"' for _ in partitionColumns]) + ']'
+        fmtDict['remoteFilePath'] = remoteFilePath if remoteFilePath is not None else ""
+        fmtDict['delimiter'] = delimiter
+        if sortColumns:
+            extraParams = ", sortColumns=" + '[' + ','.join([f'"{_}"' for _ in sortColumns]) + ']'
+        else:
+            extraParams = ""
+        fmtDict['extraParams'] = extraParams
+        tbl_str = re.sub(' +', ' ', tbl_str.format(**fmtDict).strip())
+        self.run(tbl_str)
+        if isDBPath:
+            return Table(data=fmtDict['tableName'], dbPath=dbPath, s=self)
+        else:
+            return Table(data=fmtDict['tableNameNEW'], s=self)
+
+    def ploadText(self, remoteFilePath: str, delimiter: str = ",") -> "Table":
+        """Import text files in parallel into DolphinDB as a partitioned in-memory table, which is faster than method loadText.
+
+        Args:
+            remoteFilePath : the remote file path on the server. Defaults to None.
+            delimiter : delimiter, Defaults to ",".
+
+        Returns:
+            a DolphinDB in-memory Table object.
+        """
+        tableName = _generate_tablename()
+        runstr = tableName + '= ploadText("' + remoteFilePath + '","' + delimiter + '")'
+        self.run(runstr)
+        return Table(data=tableName, s=self, isMaterialized=True)
+
+    def table(
+        self, dbPath: str = None, data=None,  tableAliasName: str = None,
+        inMem: bool = False, partitions: Optional[List[str]] = None
+    ) -> "Table":
+        """Create a DolphinDB table object and upload it to the server.
+
+        Deprecated:
+            inMem will be deprecated in a future version.
+
+        Args:
+            dbPath : database path. Defaults to None.
+            data : data of the table. Defaults to None.
+            tableAliasName : alias of the table. Defaults to None.
+            inMem : whether to load the table into memory. True: to load the table into memory. Defaults to False.
+            partitions : the partitions to be loaded into memory. Defaults to None, which means to load all partitions.
+
+        Returns:
+            a DolphinDB table object.
+        """
+        if partitions is None:
+            partitions = []
+        return Table(dbPath=dbPath, data=data,  tableAliasName=tableAliasName, inMem=inMem, partitions=partitions, s=self, isMaterialized=True)
+
+    def loadTable(self, tableName: str,  dbPath: Optional[str] = None, partitions=None, memoryMode: bool = False) -> "Table":
+        """Load a DolphinDB table.
+
+        Args:
+            tableName : the DolphinDB table name.
+            dbPath : path to the DolphinDB database. Defaults to None.
+            partitions : the partitioning columns of the partitioned table. Defaults to None.
+            memoryMode : whether to load the table into memory or just load its column names. True: to load the table into memory. Defaults to False.
+
+        Deprecated:
+            memoryMode will be deprecated in a future version.
+
+        Returns:
+            a DolphinDB table object.
+        """
+        def isDate(s):
+            try:
+                datetime.strptime(s, '%Y.%m.%d')
+                return True
+            except ValueError:
+                return False
+
+        def isMonth(s):
+            try:
+                datetime.strptime(s, '%Y.%mM')
+                return True
+            except ValueError:
+                return False
+
+        def isDatehour(s):
+            try:
+                datetime.strptime(s, '%Y.%m.%dT%H')
+                return True
+            except ValueError:
+                return False
+
+        def isTime(s):
+            return isDate(s) or isMonth(s) or isDatehour(s)
+
+        def myStr(x):
+            if type(x) is str and not isTime(x):
+                return "'" + x + "'"
+            else:
+                return str(x)
+
+        if partitions is None:
+            partitions = []
+        if dbPath:
+            runstr = '{tableName} = loadTable("{dbPath}", "{data}",{partitions},{inMem})'
+            fmtDict = dict()
+            tbName = _generate_tablename(tableName)
+            fmtDict['tableName'] = tbName
+            fmtDict['dbPath'] = dbPath
+            fmtDict['data'] = tableName
+            if type(partitions) is list:
+                fmtDict['partitions'] = ('[' + ','.join(myStr(x) for x in partitions) + ']') if len(partitions) else ""
+            else:
+                fmtDict['partitions'] = myStr(partitions)
+
+            fmtDict['inMem'] = str(memoryMode).lower()
+            runstr = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
+            self.run(runstr)
+            return Table(data=tbName, s=self, isMaterialized=True)
+        else:
+            return Table(data=tableName, s=self, needGC=False, isMaterialized=True)
+
+    def loadTableBySQL(self, tableName: str, dbPath: str, sql: str) -> "Table":
+        """Load records that satisfy the filtering conditions in a SQL query as a partitioned in-memory table.
+
+        Args:
+            tableName : the DolphinDB table name.
+            dbPath : the DolphinDB database where the table is stored.
+            sql : SQL statement.
+
+        Returns:
+            a Table object.
+        """
+        # loadTableBySQL
+        tmpTableName = _generate_tablename()
+        self.run(f"""
+            {tableName}=loadTable("{dbPath}", "{tableName}");
+            {tmpTableName}=loadTableBySQL(<{sql}>);
+        """)
+        return Table(data=tmpTableName, s=self, isMaterialized=True)
+
+    def database(
+        self, dbName: str = None, partitionType: int = None, partitions=None,
+        dbPath: str = None, engine: str = None, atomic: str = None, chunkGranularity: str = None
+    ) -> "Database":
+        """Create database.
+
+        Args:
+            dbName : database name. Defaults to None.
+            partitionType : partition type. Defaults to None.
+            partitions : describes how the partitions are created. Partitions is usually a list or np.array, with type char/int/np.datetime64. Defaults to None.
+            dbPath : database path. Defaults to None.
+            engine: storage engine, can be 'OLAP' or 'TSDB'. Defaults to None, meaning to "OLAP".
+            atomic : indicates at which level the atomicity is guaranteed for a write transaction. It can be 'TRANS' or 'CHUNK'. Defaults to None, meaning to "TRANS".
+            chunkGranularity : the chunk granularity, can be 'TABLE' or 'DATABASE'. Defaults to None.
+
+        Note:
+            The parameter chunkGranularity only takes effect when enableChunkGranularityConfig = true.
+
+        Returns:
+            a DolphinDB database object.
+        """
+        if partitions is not None:
+            partition_type = type(partitions[0])
+        else:
+            partition_type = None
+
+        if partition_type == np.datetime64:
+            partition_str = self.convertDatetime64(partitions)
+
+        elif partition_type == Database:
+            partition_str = self.convertDatabase(partitions)
+
+        elif type(partitions) == np.ndarray and (partition_type == np.ndarray or partition_type == list):
+            dataType = type(partitions[0][0])
+            partition_str = '['
+            for partition in partitions:
+                if dataType == date or dataType == month:
+                    partition_str += self.convertDateAndMonth(partition) + ','
+                elif dataType == datetime:
+                    partition_str += self.convertDatetime(partition) + ','
+                elif dataType == Database:
+                    partition_str += self.convertDatabase(partition) + ','
+                else:
+                    partition_str += str(partition) + ','
+                    partition_str = partition_str.replace('list', ' ')
+                    partition_str = partition_str.replace('(', '')
+                    partition_str = partition_str.replace(')', '')
+            partition_str = partition_str.rstrip(',')
+            partition_str += ']'
+
+        else:
+            if partition_type is not None:
+                partition_str = str(partitions)
+            else:
+                partition_str = ""
+
+        if dbName is None:
+            dbName = _generate_dbname()
+
+        if partitionType:
+            if dbPath:
+                dbstr = dbName + '=database("'+dbPath+'",' + str(partitionType) + "," + partition_str
+            else:
+                dbstr = dbName + '=database("",' + str(partitionType) + "," + partition_str
+        else:
+            if dbPath:
+                dbstr = dbName + '=database("' + dbPath + '"'
+            else:
+                dbstr = dbName + '=database(""'
+
+        if engine is not None:
+            dbstr += ",engine='" + engine + "'"
+        if atomic is not None:
+            dbstr += ",atomic='" + atomic + "'"
+        if self.enableChunkGranularityConfig and chunkGranularity is not None:
+            dbstr += ",chunkGranularity='" + chunkGranularity + "'"
+
+        dbstr += ")"
+
+        self.run(dbstr)
+        return Database(dbName=dbName, s=self)
+
+    def existsDatabase(self, dbUrl: str) -> bool:
+        """Check if the database exists.
+
+        Args:
+            dbUrl : database path.
+
+        Returns:
+            True if the database exists, otherwise False.
+        """
+        return self.run("existsDatabase('%s')" % dbUrl)
+
+    def existsTable(self, dbUrl: str, tableName: str) -> bool:
+        """Check if the table exists.
+
+        Args:
+            dbUrl : database path.
+            tableName : table name.
+
+        Returns:
+            True if the table exists, otherwise False.
+        """
+        return self.run("existsTable('%s','%s')" % (dbUrl, tableName))
+
+    def dropDatabase(self, dbPath: str) -> None:
+        """Delete a database.
+
+        Args:
+            dbPath : database path.
+        """
+        self.run("dropDatabase('" + dbPath + "')")
+
+    def dropPartition(self, dbPath: str, partitionPaths: Union[str, List[str]], tableName: str = None) -> None:
+        """Delete one or more partitions of the database.
+
+        Args:
+            dbPath : database path.
+            partitionPaths : a string or list of partition paths.
+
+        Note:
+            The directory of a partition under the database folder or a list of directories of multiple partitions must start with '/'.
+
+        Args:
+            tableName : table name. Defaults to None, indicating all tables under the partitions are deleted.
+        """
+        db = _generate_dbname()
+        self.run(f"""{db} = database("{dbPath}")""")
+        if isinstance(partitionPaths, list):
+            pths = ','.join(partitionPaths)
+        else:
+            pths = partitionPaths
+
+        if tableName:
+            self.run(f"""dropPartition({db}, [{pths}], "{tableName}")""")
+        else:
+            self.run(f"""dropPartition({db}, [{pths}])""")
+        self.run(f"""undef("{db}")""")
+
+    def dropTable(self, dbPath: str, tableName: str) -> None:
+        """Delete a table.
+
+        Args:
+            dbPath : database path.
+            tableName : table name.
+        """
+        db = _generate_dbname()
+        self.run(db + '=database("' + dbPath + '")')
+        self.run(f'dropTable({db}, "{tableName}")')
+
+    def undef(self, varName: str, varType: str) -> None:
+        """Release the specified object in the Session.
+
+        Args:
+            varName : variable name in DolphinDB.
+            varType : variable type in DolphinDB,including "VAR" (variable), "SHARED" (shared variable), "DEF" (function definition).
+        """
+        undef_str = 'undef("{varName}", {varType})'
+        fmtDict = dict()
+        fmtDict['varName'] = varName
+        fmtDict['varType'] = varType
+        self.run(undef_str.format(**fmtDict).strip())
+
+    def undefAll(self) -> None:
+        """Release all objects in the Session."""
+        self.run("undef all")
+
+    def clearAllCache(self, dfs: bool = False) -> None:
+        """Clear all cache.
+
+        Args:
+            dfs : True: clear cache of all nodes; False (default): only clear the cache of the connected node. Defaults to False.
+        """
+        if dfs:
+            self.run("pnodeRun(clearAllCache)")
+        else:
+            self.run("clearAllCache()")
+
+    @classmethod
+    def enableJobCancellation(cls) -> None:
+        """Enable cancellation of running jobs.
+
+        When this method is enabled, all running jobs (executed with Session.run()) in the process will be canceled immediately. This method can only be executed once for each Session.
+        This method is not supported in high availability secenarios.
+        This method is not recommended in multithreaded mode. In multithreaded mode, make sure the main process of signal is imported before you call this method.
+
+        """
+        if platform.system() == "Linux":
+            ddbcpp.sessionimpl.enableJobCancellation()
+        else:
+            raise RuntimeError("This method is only supported on Linux.")
+
+    @classmethod
+    def setTimeout(cls, timeout: float) -> None:
+        """Set the TCP timeout.
+
+        Args:
+            timeout : corresponds to the TCP_USER_TIMEOUT option. Specify the value in units of seconds. 
+        """
+        ddbcpp.sessionimpl.setTimeout(timeout)
+
+    def nullValueToZero(self) -> None:
+        """Convert all NULL values to 0.
+
+        Deprecated:
+            this method will be deleted in a future version.
+        """
+        self.cpp.nullValueToZero()
+
+    def nullValueToNan(self) -> None:
+        """Convert all NULL values to NumPy NaN.
+
+        Deprecated:
+            this method will be delete in a future version.
+        """
+        self.cpp.nullValueToNan()
+
+    def hashBucket(self, obj, nBucket: int):
+        """Hash map, which maps DolphinDB objects into hash buckets of size nBucket.
+
+        Args:
+            obj : the DolphinDB object to be hashed.
+            nBucket : hash bucket size.
+
+        Returns:
+            hash of the DolphinDB object.
+        """
+        if not isinstance(nBucket, int) or nBucket <= 0:
+            raise ValueError("nBucket must be a positive integer")
+        return self.cpp.hashBucket(obj, nBucket)
+
+    def convertDatetime64(self, datetime64List):
+        length = len(str(datetime64List[0]))
+        # date and month
+        if length == 10 or length == 7:
+            listStr = '['
+            for dt64 in datetime64List:
+                s = str(dt64).replace('-', '.')
+                if len(str(dt64)) == 7:
+                    s += 'M'
+                listStr += s + ','
+            listStr = listStr.rstrip(',')
+            listStr += ']'
+        else:
+            listStr = 'datehour(['
+            for dt64 in datetime64List:
+                s = str(dt64).replace('-', '.').replace('T', ' ')
+                ldt = len(str(dt64))
+                if ldt == 13:
+                    s += ':00:00'
+                elif ldt == 16:
+                    s += ':00'
+                listStr += s + ','
+            listStr = listStr.rstrip(',')
+            listStr += '])'
+        return listStr
+
+    def convertDatabase(self, databaseList):
+        listStr = '['
+        for db in databaseList:
+            listStr += db._getDbName()
+            listStr += ','
+        listStr = listStr.rstrip(',')
+        listStr += ']'
+        return listStr
+
+    def _loadPickleFile(self, filePath):
+        return self.cpp.loadPickleFile(filePath)
+
+    def _printPerformance(self):
+        self.cpp.printPerformance()
+
+
+class BlockReader(object):
+    """Read in blocks.
+
+    Specify the paramter fetchSize for method Session.run and it returns a BlockReader object to read in blocks.
+
+    Args:
+        blockReader : dolphindbcpp object.
+    """
+    def __init__(self, blockReader):
+        """Constructor of BlockReader."""
+        self.block = blockReader
+
+    def read(self):
+        """Read a piece of data.
+
+        Returns:
+            execution result of a script.
+        """
+        return self.block.read()
+
+    def hasNext(self) -> bool:
+        """Check if there is data to be read.
+
+        Returns:
+            True if there is still data not read, otherwise False.
+        """
+        return self.block.hasNext()
+
+    def skipAll(self):
+        """Skip subsequent data.
+
+        Note:
+            When reading data in blocks, if not all blocks are read, please call the skipAll method to abort the reading before executing the subsequent code.
+            Otherwise, data will be stuck in the socket buffer and the deserialization of the subsequent data will fail.
+        """
+        self.block.skipAll()
+
+
+class PartitionedTableAppender(object):
+    """Class for writes to DolphinDB DFS tables.
+
+    Args:
+        dbPath : DFS database path. Defaults to None.
+        tableName : name of a DFS table. Defaults to None.
+        partitionColName : partitioning column. Defaults to None.
+        dbConnectionPool : connection pool. Defaults to None.
+
+    Note:
+        DolphinDB does not allow multiple writers to write data to the same partition at the same time, so when the client writes data in parallel with multiple threads, please ensure that each thread writes to a different partition.
+        The python API provides PartitionedTableAppender, an easy way to automatically split data writes by partition.
+    """
+    def __init__(
+        self, dbPath: str = None, tableName: str = None,
+        partitionColName: str = None, dbConnectionPool: DBConnectionPool = None
+    ):
+        """Constructor of PartitionedTableAppender."""
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        if partitionColName is None:
+            partitionColName = ""
+        if not isinstance(dbConnectionPool, DBConnectionPool):
+            raise Exception("dbConnectionPool must be a dolphindb DBConnectionPool!")
+        self.appender = ddbcpp.partitionedTableAppender(dbPath, tableName, partitionColName, dbConnectionPool.pool)
+        self.pool = dbConnectionPool
+
+    def append(self, table: DataFrame) -> int:
+        """Append data.
+
+        Args:
+            table : data to be written.
+
+        Returns:
+            number of rows written.
+        """
+        if self.pool.is_shutdown():
+            raise RuntimeError("DBConnectionPool has been shut down.")
+        return self.appender.append(table)
+
+
+class TableAppender(object):
+    """Class of table appender.
+
+    As the only temporal data type in Python pandas is datetime64, all temporal columns of a DataFrame are converted into nanotimestamp type after uploaded to DolphinDB.
+    Each time we use tableInsert or insert into to append a DataFrame with a temporal column to an in-memory table or DFS table, we need to conduct a data type conversion for the time column.
+    For automatic data type conversion, Python API offers tableAppender object.
+
+    Args:
+        dbPath : the path of a DFS database. Leave it unspecified for in-memory tables. Defaults to None.
+        tableName : table name. Defaults to None.
+        ddbSession : a Session connected to DolphinDB server. Defaults to None.
+        action : the action when appending. Now only supports "fitColumnType", indicating to convert the data type of temporal column. Defaults to "fitColumnType".
+    """
+    def __init__(self, dbPath: str = None, tableName: str = None, ddbSession: Session = None, action: str = "fitColumnType"):
+        """Constructor of tableAppender"""
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        if not isinstance(ddbSession, Session):
+            raise Exception("ddbSession must be a dolphindb Session!")
+        if action == "fitColumnType":
+            self.tableappender = ddbcpp.autoFitTableAppender(dbPath, tableName, ddbSession.cpp)
+            self.sess = ddbSession
+        else:
+            raise Exception("other action not supported yet!")
+
+    def append(self, table: DataFrame) -> int:
+        """Append data.
+
+        Args:
+            table : data to be written.
+
+        Returns:
+            number of rows written.
+        """
+        if self.sess.isClosed():
+            raise RuntimeError("Session has been closed.")
+        return self.tableappender.append(table)
+
+
+class TableUpserter(object):
+    """Class of table upserter.
+
+    Args:
+        dbPath : the path of a DFS database. Leave it unspecified for in-memory tables. Defaults to None.
+        tableName : table name. Defaults to None.
+        ddbSession : a Session connected to DolphinDB server. Defaults to None.
+        ignoreNull : if set to true, for the NULL values in the new data, the correponding elements in the table are not updated. Defaults to False.
+        keyColNames : key column names. For a DFS table, the columns specified by this parameter are considrd as key columns. Defaults to [].
+        sortColumns : sort column names. All data in the updated partition will be sorted according to the specified column. Defaults to [].
+    """
+    def __init__(
+        self, dbPath: str = None, tableName: str = None,
+        ddbSession: Session = None, ignoreNull: bool = False,
+        keyColNames: List[str] = [], sortColumns: List[str] = []
+    ):
+        """Constructor of tableUpsert."""
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        if not isinstance(ddbSession, Session):
+            raise Exception("ddbSession must be a dolphindb Session!")
+        self.tableupserter = ddbcpp.autoFitTableUpsert(dbPath, tableName, ddbSession.cpp, ignoreNull, keyColNames, sortColumns)
+        self.sess = ddbSession
+
+    def __del__(self):
+        self.tableupserter = None
+
+    def upsert(self, table: DataFrame):
+        """upsert data.
+
+        Args:
+            table : data to be written.
+        """
+        if self.sess.isClosed():
+            raise RuntimeError("Session has been closed.")
+        self.tableupserter.upsert(table)
+
+
+class BatchTableWriter(object):
+    """Class of batch writer for asynchronous batched writes.
+
+    Support batched writes to in-memory table and distributed table.
+
+    Args:
+        host : server address.
+        port : port name.
+        userid : username. Defaults to None.
+        password : password. Defaults to None.
+        acquireLock : whether to acquire a lock in the Python API, True (default) means to acquire a lock. Defaults to True.
+
+    Note:
+        It's required to acquire the lock for concurrent API calls
+    """
+    def __init__(
+        self, host: str, port: int,
+        userid: str = None, password: str = None,
+        acquireLock: bool = True
+    ):
+        """Constructor of BatchTableWriter"""
+        if userid is None:
+            userid = ""
+        if password is None:
+            password = ""
+        self.writer = ddbcpp.batchTableWriter(host, port, userid, password, acquireLock)
+
+    def addTable(
+        self, dbPath: str = None, tableName: str = None,
+        partitioned: bool = True
+    ) -> None:
+        """Add a table to be written to.
+
+        Args:
+            dbPath : the database path for a disk table; leave it empty for an in-memory table. Defaults to None.
+            tableName : table name. Defaults to None.
+            partitioned : whether is a partitioned table. True indicates a partitioned table. Defaults to True.
+
+        Note:
+            If the table is a non-partitioned table on disk, it's required to set partitioned=False.
+        """
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        self.writer.addTable(dbPath, tableName, partitioned)
+
+    def getStatus(self, dbPath: str = None, tableName: str = None) -> Tuple[int, bool, bool]:
+        """Get the current write status.
+
+        Args:
+            dbPath : database name. Defaults to None.
+            tableName : table name. Defaults to None.
+
+        Returns:
+            Tuple[int, bool, bool]: indicating the depth of the current writing queue, whether the current table is being removed (True if being removed), and whether the background thread exits due to an error (True if exits due to an error).
+        """
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        return self.writer.getStatus(dbPath, tableName)
+
+    def getAllStatus(self) -> DataFrame:
+        """Get the status of all tables except for the removed ones.
+
+        Returns:
+        | DatabaseName | TableName | WriteQueueDepth | sentRows | Removing | Finished |
+        | :----------- | :-------- | :-------------- | :------- | :------- | :------- |
+        | 0            | tglobal   | 0               | 5        | False    | False    |
+        """
+        return self.writer.getAllStatus()
+
+    def getUnwrittenData(self, dbPath: str = None, tableName: str = None) -> DataFrame:
+        """Obtain unwritten data. The method is mainly used to obtain the remaining unwritten data if an error occurs when writing.
+
+        Args:
+            dbPath : database name. Defaults to None.
+            tableName : table name. Defaults to None.
+
+        Returns:
+            DataFrame of unwritten data.
+        """
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        return self.writer.getUnwrittenData(dbPath, tableName)
+
+    def removeTable(self, dbPath: str = None, tableName: str = None) -> None:
+        """Release the resources occupied by the table added by the addTable method. The first time the method is called, it returns if the thread has exited.
+
+        Args:
+            dbPath : database name. Defaults to None.
+            tableName : table name. Defaults to None.
+        """
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        self.writer.removeTable(dbPath, tableName)
+
+    def insert(self, dbPath: str = None, tableName: str = None, *args):
+        """Insert a single row of data
+
+        Args:
+            dbPath : database name. Defaults to None.
+            tableName : table name. Defaults to None.
+            args : variable-length argument, indicating a row of data to be inserted.
+        """
+        if dbPath is None:
+            dbPath = ""
+        if tableName is None:
+            tableName = ""
+        self.writer.insert(dbPath, tableName, *args)
+
+
+class ErrorCodeInfo(object):
+    """MTW error codes and messages.
+
+    Args:
+        errorCode : error code. Defaults to None.
+        errorInfo : error information. Defaults to None.
+    """
+    def __init__(self, errorCode=None, errorInfo=None):
+        """Constructor of ErrorCodeInfo."""
+        self.errorCode = errorCode
+        self.errorInfo = errorInfo
+
+    def __repr__(self):
+        errorCodeText = ""
+        if self.hasError():
+            errorCodeText = self.errorCode
+        else:
+            errorCodeText = None
+        outStr = "errorCode: %s\n" % errorCodeText
+        outStr += " errorInfo: %s\n" % self.errorInfo
+        outStr += object.__repr__(self)
+        return outStr
+
+    def hasError(self) -> bool:
+        """Check if an error has occurred.
+
+        Returns:
+            True if an error occurred, otherwise False.
+        """
+        return self.errorCode is not None and len(self.errorCode) > 0
+
+    def succeed(self) -> bool:
+        """Check if data has been written successfully.
+
+        Returns:
+            True if the write is successful, otherwise False.
+        """
+        return self.errorCode is None or len(self.errorCode) < 1
+
+
+class MultithreadedTableWriterThreadStatus(object):
+    """Get the status of MTW.
+
+    Args:
+        threadId: thread ID.
+
+    Attribute:
+        threadId : thread ID.
+        sentRows : number of sent rows.
+        unsentRows : number of rows to be sent.
+        sendFailedRows : number of rows failed to be sent.
+
+    """
+    def __init__(self, threadId: int = None):
+        """Constructor of MultithreadedTableWriterThreadStatus."""
+        self.threadId = threadId
+        self.sentRows = None
+        self.unsentRows = None
+        self.sendFailedRows = None
+
+
+class MultithreadedTableWriterStatus(ErrorCodeInfo):
+    """The status information of MTW.
+
+    Attribute:
+        isExiting : whether the threads are exiting.
+        sentRows : number of sent rows.
+        unsentRows : number of rows to be sent.
+        sendFailedRows : number of rows failed to be sent.
+        threadStatus : a list of the thread status.
+    """
+    def __init__(self):
+        """Constructor of MultithreadedTableWriterStatus."""
+        self.isExiting = None
+        self.sentRows = None
+        self.unsentRows = None
+        self.sendFailedRows = None
+        self.threadStatus = []
+
+    def update(self, statusDict):
+        threadStatusDict = statusDict["threadStatus"]
+        del statusDict["threadStatus"]
+        self.__dict__.update(statusDict)
+        for oneThreadStatusDict in threadStatusDict:
+            oneThreadStatus = MultithreadedTableWriterThreadStatus()
+            oneThreadStatus.__dict__.update(oneThreadStatusDict)
+            self.threadStatus.append(oneThreadStatus)
+
+    def __repr__(self):
+        errorCodeText = ""
+        if self.hasError():
+            errorCodeText = self.errorCode
+        else:
+            errorCodeText = None
+        outStr = "%-14s: %s\n" % ("errorCode", errorCodeText)
+        if self.errorInfo is not None:
+            outStr += " %-14s: %s\n" % ("errorInfo", self.errorInfo)
+        if self.isExiting is not None:
+            outStr += " %-14s: %s\n" % ("isExiting", self.isExiting)
+        if self.sentRows is not None:
+            outStr += " %-14s: %s\n" % ("sentRows", self.sentRows)
+        if self.unsentRows is not None:
+            outStr += " %-14s: %s\n" % ("unsentRows", self.unsentRows)
+        if self.sendFailedRows is not None:
+            outStr += " %-14s: %s\n" % ("sendFailedRows", self.sendFailedRows)
+        if self.threadStatus is not None:
+            outStr += " %-14s: \n" % "threadStatus"
+            outStr += " \tthreadId\tsentRows\tunsentRows\tsendFailedRows\n"
+            for thread in self.threadStatus:
+                outStr += "\t"
+                if thread.threadId is not None:
+                    outStr += "%8d" % thread.threadId
+                outStr += "\t"
+                if thread.sentRows is not None:
+                    outStr += "%8d" % thread.sentRows
+                outStr += "\t"
+                if thread.unsentRows is not None:
+                    outStr += "%10d" % thread.unsentRows
+                outStr += "\t"
+                if thread.sendFailedRows is not None:
+                    outStr += "%14d" % thread.sendFailedRows
+                outStr += "\n"
+        outStr += object.__repr__(self)
+        return outStr
+
+
+class MultithreadedTableWriter(object):
+    """A multi-threaded writer is an ungrade of BatchTableWriter with support for multi-threaded concurrent writes.
+
+    Args:
+        host : host name.
+        port : port number.
+        userId : username.
+        password : password.
+        dbPath : the DFS database path or in-memory table name.
+        tableName : the DFS table name. Leave it unspecified for an in-memory table.
+        useSSL : whether to enable SSL. Defaults to False.
+        enableHighAvailability : whether to enable high availability. Defaults to False.
+        highAvailabilitySites : a list of "ip:port" of all available nodes. Defaults to [].
+        batchSize : the number of messages in batch processing. Defaults to 1.
+        throttle : the waiting time (in seconds) before the server processes the incoming data if the number of data written from the client does not reach batchSize. Defaults to 1.
+        threadCount : the number of working threads to be created. Defaults to 1.
+        partitionCol : a string indicating the partitioning column, the default is an empty string. The parameter only takes effect when threadCount>1. Defaults to "".
+                        For a partitioned table, it must be the partitioning column; for a stream table, it must be a column name; for a dimension table, the parameter does not work.
+        compressMethods : a list of the compression methods used for each column. If unspecified, the columns are not compressed. Defaults to []. 
+                            The compression methods include: "LZ4": LZ4 algorithm; "DELTA": Delta-of-delta encoding.
+        mode : The write mode. It can be Append (default) or Upsert. Defaults to "".
+        modeOption : The parameters of function upsert!. It only takes effect when mode is Upsert. Defaults to [].
+    """
+    def __init__(
+        self, host: str, port: int, userId: str, password: str,
+        dbPath: str, tableName: str, useSSL: bool = False,
+        enableHighAvailability: bool = False, highAvailabilitySites: List[str] = [],
+        batchSize: int = 1, throttle: float = 1.0, threadCount: int = 1,
+        partitionCol: str = "", compressMethods: List[str] = [],
+        mode: str = "", modeOption: List[str] = []
+    ):
+        """Constructor of MultithreadedTableWriter"""
+        self.writer = ddbcpp.multithreadedTableWriter(
+            host, port, userId, password, dbPath, tableName, useSSL,
+            enableHighAvailability, highAvailabilitySites, batchSize, throttle, threadCount,
+            partitionCol, compressMethods, mode, modeOption
+        )
+
+    def getStatus(self) -> MultithreadedTableWriterStatus:
+        """Get the current writer status and return a MultithreadedTableWriterStatus object.
+
+        Returns:
+            MultithreadedTableWriterStatus object.
+        """
+        status = MultithreadedTableWriterStatus()
+        status.update(self.writer.getStatus())
+        return status
+
+    def getUnwrittenData(self) -> List[List[Any]]:
+        """Get unwritten data.
+
+        The obtained data can be passed as an argument to method insertUnwrittenData.
+
+        Returns:
+            a nested list where each element is a record.
+        """
+        return self.writer.getUnwrittenData()
+
+    def insert(self, *args) -> ErrorCodeInfo:
+        """Insert a single row of data.
+
+        Args:
+            args : variable-length argument, indicating a row of data to be inserted.
+
+        Returns:
+            a ErrorCodeInfo object.
+        """
+        errorCodeInfo = ErrorCodeInfo()
+        errorCodeInfo.__dict__.update(self.writer.insert(*args))
+        return errorCodeInfo
+
+    def insertUnwrittenData(self, unwrittenData) -> ErrorCodeInfo:
+        """Insert unwritten data.
+
+        The result is in the same format as insert.
+        The difference is that insertUnwrittenData can insert multiple records at a time.
+
+        Args:
+            unwrittenData : the data that has not been written to the server. You can obtain the object with method getUnwrittenData.
+
+        Returns:
+            ErrorCodeInfo object
+        """
+        errorCodeInfo = ErrorCodeInfo()
+        errorCodeInfo.__dict__.update(self.writer.insertUnwrittenData(unwrittenData))
+        return errorCodeInfo
+
+    def waitForThreadCompletion(self) -> None:
+        """Wait until all working threads complete their tasks.
+
+        After calling the method, MultithreadedTableWriter will wait until all working threads complete their tasks.
+
+        """
+        self.writer.waitForThreadCompletion()
```

## dolphindb/settings.py

```diff
@@ -1,223 +1,223 @@
-from enum import Enum
-
-FORM_NUM = 9
-# DATA FORM
-DF_SCALAR = 0
-DF_VECTOR = 1
-DF_PAIR = 2
-DF_MATRIX = 3
-DF_SET = 4
-DF_DICTIONARY = 5
-DF_TABLE = 6
-DF_CHART = 7
-DF_CHUNK = 8
-
-# DATA_TYPE
-TYPE_NUM = 71
-DT_VOID = 0
-DT_BOOL = 1
-DT_BYTE = 2
-DT_CHAR = 2
-DT_SHORT = 3
-DT_INT = 4
-DT_LONG = 5
-DT_DATE = 6
-DT_MONTH = 7
-DT_TIME = 8
-DT_MINUTE = 9
-DT_SECOND = 10
-DT_DATETIME = 11
-DT_TIMESTAMP = 12
-DT_NANOTIME = 13
-DT_NANOTIMESTAMP = 14
-DT_FLOAT = 15
-DT_DOUBLE = 16
-DT_SYMBOL = 17
-DT_STRING = 18
-DT_UUID = 19
-DT_FUNCTIONDEF = 20
-DT_HANDLE = 21
-DT_CODE = 22
-DT_DATASOURCE = 23
-DT_RESOURCE = 24
-DT_ANY = 25
-DT_COMPRESS = 26
-DT_DICTIONARY = 27
-DT_DATEHOUR = 28
-DT_DATEMINUTE = 29
-DT_IPPADDR = 30
-DT_IPADDR = 30
-DT_INT128 = 31
-DT_BLOB = 32
-DT_DECIMAL = 33
-DT_DECIMAL32 = 37
-DT_DECIMAL64 = 38
-DT_DECIMAL128 = 39
-DT_OBJECT = 40
-
-DT_VOID_ARRAY = 64
-ARRAY_TYPE_BASE = 64
-DT_BOOL_ARRAY = 65
-DT_BYTE_ARRAY = 66
-DT_CHAR_ARRAY = 66
-DT_SHORT_ARRAY = 67
-DT_INT_ARRAY = 68
-DT_LONG_ARRAY = 69
-DT_DATE_ARRAY = 70
-DT_MONTH_ARRAY = 71
-DT_TIME_ARRAY = 72
-DT_MINUTE_ARRAY = 73
-DT_SECOND_ARRAY = 74
-DT_DATETIME_ARRAY = 75
-DT_TIMESTAMP_ARRAY = 76
-DT_NANOTIME_ARRAY = 77
-DT_NANOTIMESTAMP_ARRAY = 78
-DT_FLOAT_ARRAY = 79
-DT_DOUBLE_ARRAY = 80
-DT_SYMBOL_ARRAY = 81
-DT_STRING_ARRAY = 82
-DT_UUID_ARRAY = 83
-DT_FUNCTIONDEF_ARRAY = 84
-DT_HANDLE_ARRAY = 85
-DT_CODE_ARRAY = 86
-DT_DATASOURCE_ARRAY = 87
-DT_RESOURCE_ARRAY = 88
-DT_ANY_ARRAY = 89
-DT_COMPRESS_ARRAY = 90
-DT_DICTIONARY_ARRAY = 91
-DT_DATEHOUR_ARRAY = 92
-DT_DATEMINUTE_ARRAY = 93
-DT_IPPADDR_ARRAY = 94
-DT_IPADDR_ARRAY = 94
-DT_INT128_ARRAY = 95
-DT_BLOB_ARRAY = 96
-DT_DECIMAL32_ARRAY = 101
-DT_DECIMAL64_ARRAY = 102
-DT_DECIMAL128_ARRAY = 103
-
-# Data type size
-DATA_SIZE = dict()
-DATA_SIZE[DT_VOID] = 0
-DATA_SIZE[DT_BOOL] = 1
-DATA_SIZE[DT_BYTE] = 1
-DATA_SIZE[DT_SHORT] = 2
-DATA_SIZE[DT_INT] = 4
-DATA_SIZE[DT_LONG] = 8
-DATA_SIZE[DT_DATE] = 4
-DATA_SIZE[DT_MONTH] = 4
-DATA_SIZE[DT_TIME] = 4
-DATA_SIZE[DT_MINUTE] = 4
-DATA_SIZE[DT_SECOND] = 4
-DATA_SIZE[DT_DATETIME] = 4
-DATA_SIZE[DT_TIMESTAMP] = 8
-DATA_SIZE[DT_NANOTIME] = 8
-DATA_SIZE[DT_NANOTIMESTAMP] = 8
-DATA_SIZE[DT_FLOAT] = 4
-DATA_SIZE[DT_DOUBLE] = 8
-DATA_SIZE[DT_SYMBOL] = 4
-DATA_SIZE[DT_STRING] = 0
-DATA_SIZE[DT_UUID] = 16
-DATA_SIZE[DT_ANY] = 0
-DATA_SIZE[DT_DICTIONARY] = 0
-DATA_SIZE[DT_OBJECT] = 0
-DATA_SIZE[DT_IPADDR] = 16
-DATA_SIZE[DT_INT128] = 16
-DATA_SIZE[DT_BLOB] = 0
-
-DBNAN = dict()
-DBNAN[DT_BYTE] = -128
-DBNAN[DT_BOOL] = -128
-DBNAN[DT_SHORT] = -32768
-DBNAN[DT_INT] = -2147483648
-DBNAN[DT_LONG] = -9223372036854775808
-DBNAN[DT_FLOAT] = -3.4028234663852886e+38
-DBNAN[DT_DOUBLE] = -1.7976931348623157e+308
-DBNAN[DT_SYMBOL] = ''
-DBNAN[DT_STRING] = ''
-DBNAN[DT_DATE] = -2147483648
-DBNAN[DT_MONTH] = -2147483648
-DBNAN[DT_TIME] = -2147483648
-DBNAN[DT_MINUTE] = -2147483648
-DBNAN[DT_SECOND] = -2147483648
-DBNAN[DT_DATETIME] = -2147483648
-DBNAN[DT_TIMESTAMP] = -9223372036854775808
-DBNAN[DT_NANOTIME] = -9223372036854775808
-DBNAN[DT_NANOTIMESTAMP] = -9223372036854775808
-DBNAN[DT_UUID]=0
-DBNAN[DT_INT128]=0
-DBNAN[DT_IPADDR]=0
-
-
-# partition Schema
-SEQ = 0
-VALUE = 1
-RANGE = 2
-LIST = 3
-COMPO = 4
-HASH = 5
-
-# VERBOSE
-VERBOSE = False
-
-
-def set_verbose(verbose=False):
-    global VERBOSE
-    VERBOSE = verbose
-
-
-def get_verbose():
-    return VERBOSE
-
-
-# Protocol
-PROTOCOL_DEFAULT = 0
-PROTOCOL_DDB = 1
-PROTOCOL_PICKLE = 2
-PROTOCOL_ARROW = 3
-
-# OTHER Settings
-DDB_EPSILON = 1e-5
-
-
-class DATA_CATEGORY(Enum):
-    NOTHING = 0
-    LOGICAL = 1
-    INTEGRAL = 2
-    FLOATING = 3
-    TEMPORAL = 4
-    LITERAL = 5
-    SYSTEM = 6
-    MIXED = 7
-    BINARY = 8
-    COMPLEX = 9
-    ARRAY = 10
-    DENARY = 11
-
-
-def getCategory(data_type):
-    if data_type in [
-        DT_TIME, DT_SECOND, DT_MINUTE, DT_DATE,
-        DT_DATEHOUR, DT_DATEMINUTE, DT_DATETIME, DT_MONTH,
-        DT_NANOTIME, DT_NANOTIMESTAMP, DT_TIMESTAMP,
-    ]:
-        return DATA_CATEGORY.TEMPORAL
-    elif data_type in [DT_INT, DT_LONG, DT_SHORT, DT_CHAR]:
-        return DATA_CATEGORY.INTEGRAL
-    elif data_type in [DT_BOOL]:
-        return DATA_CATEGORY.LOGICAL
-    elif data_type in [DT_DOUBLE, DT_FLOAT]:
-        return DATA_CATEGORY.FLOATING
-    elif data_type in [DT_STRING, DT_SYMBOL]:
-        return DATA_CATEGORY.LITERAL
-    elif data_type in [DT_INT128, DT_UUID, DT_IPADDR, DT_BLOB]:
-        return DATA_CATEGORY.BINARY
-    elif data_type in [DT_ANY]:
-        return DATA_CATEGORY.MIXED
-    elif data_type in [DT_VOID]:
-        return DATA_CATEGORY.NOTHING
-    elif data_type in [DT_DECIMAL32, DT_DECIMAL64, DT_DECIMAL128]:
-        return DATA_CATEGORY.DENARY
-    elif data_type >= ARRAY_TYPE_BASE:
-        return DATA_CATEGORY.ARRAY
-    else:
-        return DATA_CATEGORY.SYSTEM
+from enum import Enum
+
+FORM_NUM = 9
+# DATA FORM
+DF_SCALAR = 0
+DF_VECTOR = 1
+DF_PAIR = 2
+DF_MATRIX = 3
+DF_SET = 4
+DF_DICTIONARY = 5
+DF_TABLE = 6
+DF_CHART = 7
+DF_CHUNK = 8
+
+# DATA_TYPE
+TYPE_NUM = 71
+DT_VOID = 0
+DT_BOOL = 1
+DT_BYTE = 2
+DT_CHAR = 2
+DT_SHORT = 3
+DT_INT = 4
+DT_LONG = 5
+DT_DATE = 6
+DT_MONTH = 7
+DT_TIME = 8
+DT_MINUTE = 9
+DT_SECOND = 10
+DT_DATETIME = 11
+DT_TIMESTAMP = 12
+DT_NANOTIME = 13
+DT_NANOTIMESTAMP = 14
+DT_FLOAT = 15
+DT_DOUBLE = 16
+DT_SYMBOL = 17
+DT_STRING = 18
+DT_UUID = 19
+DT_FUNCTIONDEF = 20
+DT_HANDLE = 21
+DT_CODE = 22
+DT_DATASOURCE = 23
+DT_RESOURCE = 24
+DT_ANY = 25
+DT_COMPRESS = 26
+DT_DICTIONARY = 27
+DT_DATEHOUR = 28
+DT_DATEMINUTE = 29
+DT_IPPADDR = 30
+DT_IPADDR = 30
+DT_INT128 = 31
+DT_BLOB = 32
+DT_DECIMAL = 33
+DT_DECIMAL32 = 37
+DT_DECIMAL64 = 38
+DT_DECIMAL128 = 39
+DT_OBJECT = 40
+
+DT_VOID_ARRAY = 64
+ARRAY_TYPE_BASE = 64
+DT_BOOL_ARRAY = 65
+DT_BYTE_ARRAY = 66
+DT_CHAR_ARRAY = 66
+DT_SHORT_ARRAY = 67
+DT_INT_ARRAY = 68
+DT_LONG_ARRAY = 69
+DT_DATE_ARRAY = 70
+DT_MONTH_ARRAY = 71
+DT_TIME_ARRAY = 72
+DT_MINUTE_ARRAY = 73
+DT_SECOND_ARRAY = 74
+DT_DATETIME_ARRAY = 75
+DT_TIMESTAMP_ARRAY = 76
+DT_NANOTIME_ARRAY = 77
+DT_NANOTIMESTAMP_ARRAY = 78
+DT_FLOAT_ARRAY = 79
+DT_DOUBLE_ARRAY = 80
+DT_SYMBOL_ARRAY = 81
+DT_STRING_ARRAY = 82
+DT_UUID_ARRAY = 83
+DT_FUNCTIONDEF_ARRAY = 84
+DT_HANDLE_ARRAY = 85
+DT_CODE_ARRAY = 86
+DT_DATASOURCE_ARRAY = 87
+DT_RESOURCE_ARRAY = 88
+DT_ANY_ARRAY = 89
+DT_COMPRESS_ARRAY = 90
+DT_DICTIONARY_ARRAY = 91
+DT_DATEHOUR_ARRAY = 92
+DT_DATEMINUTE_ARRAY = 93
+DT_IPPADDR_ARRAY = 94
+DT_IPADDR_ARRAY = 94
+DT_INT128_ARRAY = 95
+DT_BLOB_ARRAY = 96
+DT_DECIMAL32_ARRAY = 101
+DT_DECIMAL64_ARRAY = 102
+DT_DECIMAL128_ARRAY = 103
+
+# Data type size
+DATA_SIZE = dict()
+DATA_SIZE[DT_VOID] = 0
+DATA_SIZE[DT_BOOL] = 1
+DATA_SIZE[DT_BYTE] = 1
+DATA_SIZE[DT_SHORT] = 2
+DATA_SIZE[DT_INT] = 4
+DATA_SIZE[DT_LONG] = 8
+DATA_SIZE[DT_DATE] = 4
+DATA_SIZE[DT_MONTH] = 4
+DATA_SIZE[DT_TIME] = 4
+DATA_SIZE[DT_MINUTE] = 4
+DATA_SIZE[DT_SECOND] = 4
+DATA_SIZE[DT_DATETIME] = 4
+DATA_SIZE[DT_TIMESTAMP] = 8
+DATA_SIZE[DT_NANOTIME] = 8
+DATA_SIZE[DT_NANOTIMESTAMP] = 8
+DATA_SIZE[DT_FLOAT] = 4
+DATA_SIZE[DT_DOUBLE] = 8
+DATA_SIZE[DT_SYMBOL] = 4
+DATA_SIZE[DT_STRING] = 0
+DATA_SIZE[DT_UUID] = 16
+DATA_SIZE[DT_ANY] = 0
+DATA_SIZE[DT_DICTIONARY] = 0
+DATA_SIZE[DT_OBJECT] = 0
+DATA_SIZE[DT_IPADDR] = 16
+DATA_SIZE[DT_INT128] = 16
+DATA_SIZE[DT_BLOB] = 0
+
+DBNAN = dict()
+DBNAN[DT_BYTE] = -128
+DBNAN[DT_BOOL] = -128
+DBNAN[DT_SHORT] = -32768
+DBNAN[DT_INT] = -2147483648
+DBNAN[DT_LONG] = -9223372036854775808
+DBNAN[DT_FLOAT] = -3.4028234663852886e+38
+DBNAN[DT_DOUBLE] = -1.7976931348623157e+308
+DBNAN[DT_SYMBOL] = ''
+DBNAN[DT_STRING] = ''
+DBNAN[DT_DATE] = -2147483648
+DBNAN[DT_MONTH] = -2147483648
+DBNAN[DT_TIME] = -2147483648
+DBNAN[DT_MINUTE] = -2147483648
+DBNAN[DT_SECOND] = -2147483648
+DBNAN[DT_DATETIME] = -2147483648
+DBNAN[DT_TIMESTAMP] = -9223372036854775808
+DBNAN[DT_NANOTIME] = -9223372036854775808
+DBNAN[DT_NANOTIMESTAMP] = -9223372036854775808
+DBNAN[DT_UUID]=0
+DBNAN[DT_INT128]=0
+DBNAN[DT_IPADDR]=0
+
+
+# partition Schema
+SEQ = 0
+VALUE = 1
+RANGE = 2
+LIST = 3
+COMPO = 4
+HASH = 5
+
+# VERBOSE
+VERBOSE = False
+
+
+def set_verbose(verbose=False):
+    global VERBOSE
+    VERBOSE = verbose
+
+
+def get_verbose():
+    return VERBOSE
+
+
+# Protocol
+PROTOCOL_DEFAULT = 0
+PROTOCOL_DDB = 1
+PROTOCOL_PICKLE = 2
+PROTOCOL_ARROW = 3
+
+# OTHER Settings
+DDB_EPSILON = 1e-5
+
+
+class DATA_CATEGORY(Enum):
+    NOTHING = 0
+    LOGICAL = 1
+    INTEGRAL = 2
+    FLOATING = 3
+    TEMPORAL = 4
+    LITERAL = 5
+    SYSTEM = 6
+    MIXED = 7
+    BINARY = 8
+    COMPLEX = 9
+    ARRAY = 10
+    DENARY = 11
+
+
+def getCategory(data_type):
+    if data_type in [
+        DT_TIME, DT_SECOND, DT_MINUTE, DT_DATE,
+        DT_DATEHOUR, DT_DATEMINUTE, DT_DATETIME, DT_MONTH,
+        DT_NANOTIME, DT_NANOTIMESTAMP, DT_TIMESTAMP,
+    ]:
+        return DATA_CATEGORY.TEMPORAL
+    elif data_type in [DT_INT, DT_LONG, DT_SHORT, DT_CHAR]:
+        return DATA_CATEGORY.INTEGRAL
+    elif data_type in [DT_BOOL]:
+        return DATA_CATEGORY.LOGICAL
+    elif data_type in [DT_DOUBLE, DT_FLOAT]:
+        return DATA_CATEGORY.FLOATING
+    elif data_type in [DT_STRING, DT_SYMBOL, DT_BLOB]:
+        return DATA_CATEGORY.LITERAL
+    elif data_type in [DT_INT128, DT_UUID, DT_IPADDR]:
+        return DATA_CATEGORY.BINARY
+    elif data_type in [DT_ANY]:
+        return DATA_CATEGORY.MIXED
+    elif data_type in [DT_VOID]:
+        return DATA_CATEGORY.NOTHING
+    elif data_type in [DT_DECIMAL32, DT_DECIMAL64, DT_DECIMAL128]:
+        return DATA_CATEGORY.DENARY
+    elif data_type >= ARRAY_TYPE_BASE:
+        return DATA_CATEGORY.ARRAY
+    else:
+        return DATA_CATEGORY.SYSTEM
```

## dolphindb/table.py

 * *Ordering differences only*

```diff
@@ -1,2382 +1,2382 @@
-import copy
-import inspect
-import re
-import threading
-from typing import Any, List, Optional, Tuple, Type, Union
-
-import numpy as np
-from dolphindb.settings import get_verbose
-from dolphindb.utils import _generate_tablename, _getFuncName, _isVariableCandidate
-from dolphindb.vector import FilterCond, Vector
-from pandas import DataFrame
-
-
-class Counter(object):
-    """Reference counter for internal use when caching table."""
-    def __init__(self):
-        """Constructor of Counter."""
-        self.__lock = threading.Lock()
-        self.__value = 1
-
-    def inc(self) -> int:
-        """Increment the reference count.
-
-        Returns:
-            current reference count.
-        """
-        with self.__lock:
-            self.__value += 1
-            return self.__value
-
-    def dec(self) -> int:
-        """Decrease the reference count.
-
-        Returns:
-            current reference count.
-        """
-        with self.__lock:
-            self.__value -= 1
-            return self.__value
-
-    def val(self) -> int:
-        """Get the current reference count.
-
-        Returns:
-            current reference count.
-        """
-        with self.__lock:
-            return self.__value
-
-
-class Table(object):
-    """DolphinDB Table object.
-
-    Args:
-        dbPath : database name. Defaults to None.
-        data : data of the table. Defaults to None.
-        tableAliasName : table alias. Defaults to None.
-        partitions : the partitions to be loaded into memory. Defaults to None, which means to load all partitions.
-        inMem : (deprecated) whether to load the table into memory. True: to load the table into memory. Defaults to False.
-        schemaInited : whether the table structure has been initialized. True: the table structure has been initialized. Defaults to False.
-        s : the connected Session object. Defaults to None.
-        needGC : whether to enable garbage collection. True: enable garbage collection. Defaults to True.
-        isMaterialized : whether table is materialized True: table has been materialized. Defaults to False.
-    """
-    def __init__(
-        self,
-        dbPath: str = None,
-        data=None,
-        tableAliasName: str = None,
-        partitions: Optional[List[str]] = None,
-        inMem: bool = False,
-        schemaInited: bool = False,
-        s=None,
-        needGC: bool = True,
-        isMaterialized: bool = False
-    ):
-        """Constructor of Table."""
-        if partitions is None:
-            partitions = []
-        self.__having = None
-        self.__top = None
-        self.__exec = False
-        self.__limit = None
-        self.__leftTable = None
-        self.__rightTable = None
-        self.__merge_for_update = False
-        self.__objAddr = None
-        self.__columns = None
-        self.isMaterialized = isMaterialized
-        if tableAliasName is not None:
-            self.isMaterialized = True
-        if s is None:
-            raise RuntimeError("Session must be provided")
-        self.__tableName = _generate_tablename() if not isinstance(data, str) else data
-        self.__session = s  # type : Session
-        self.__schemaInited = schemaInited
-        self.__need_gc = needGC
-        if self.__need_gc:
-            self.__ref = Counter()
-        if not isinstance(partitions, list):
-            raise RuntimeError(
-                'Column names must be passed in as a list')
-        if isinstance(data, dict) or isinstance(data, DataFrame):
-            df = data if isinstance(data, DataFrame) else DataFrame(data)
-            # if  not self.__tableName.startswith("TMP_TBL_"):
-            #    self._setTableName(_generate_tablename())
-            if tableAliasName is None:
-                self._setTableName(_generate_tablename())
-            else:
-                self._setTableName(tableAliasName)
-            self.__objAddr = self.__session.upload({self.__tableName: df})
-            self.vecs = {}
-
-            for colName in df.keys():
-                self.vecs[colName] = Vector(
-                    name=colName, tableName=self.__tableName, s=self.__session
-                )
-            select_list = list(self.vecs.keys())
-            select_list = [colName if _isVariableCandidate(colName) else f'_"{colName}"' for colName in select_list]
-            self._setSelect(select_list)
-        elif isinstance(data, str):
-            if dbPath:
-                if tableAliasName:
-                    self.__tableName = tableAliasName
-                else:
-                    self.__tableName = _generate_tablename(data)
-                runstr = '{tableName} = loadTable("{dbPath}", "{data}", {partitions}, {inMem})'
-                fmtDict = dict()
-                fmtDict['tableName'] = self.__tableName
-                fmtDict['dbPath'] = dbPath
-                fmtDict['data'] = data
-                if len(partitions) and type(partitions[0]) is not str:
-                    fmtDict['partitions'] = ('[' + ','.join(str(x) for x in partitions) + ']') if len(partitions) else ""
-                else:
-                    fmtDict['partitions'] = ('["' + '","'.join(partitions) + '"]') if len(partitions) else ""
-                fmtDict['inMem'] = str(inMem).lower()
-                runstr = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
-                self.__session.run(runstr)
-                # runstr = '%s = select * from %s' %(self.__tableName, self.__tableName)
-                # self.__session.run(runstr)
-            else:
-                pass
-        elif "orca.core.frame.DataFrame" in str(data.__class__):
-            df = s.run(data._var_name)
-            self.__init__(data=df, s=self.__session)
-        else:
-            raise RuntimeError("data must be a remote dolphindb table name or dict or DataFrame")
-        self._init_schema()
-
-    def __deepcopy__(self, memodict=None):
-        if memodict is None:
-            memodict = {}
-        newTable = Table(data=self.__tableName, schemaInited=True, s=self.__session, needGC=self.__need_gc)
-        newTable._setExec(self.isExec)
-        newTable.isMaterialized = self.isMaterialized
-        try:
-            newTable.vecs = copy.deepcopy(self.vecs, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__schemaInited = copy.deepcopy(self.__schemaInited, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__select = copy.deepcopy(self.__select, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__where = copy.deepcopy(self.__where, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__groupby = copy.deepcopy(self.__groupby, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__contextby = copy.deepcopy(self.__contextby, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__having = copy.deepcopy(self.__having, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__sort = copy.deepcopy(self.__sort, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__top = copy.deepcopy(self.__top, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__limit = copy.deepcopy(self.__limit, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__csort = copy.deepcopy(self.__csort, memodict)
-        except AttributeError:
-            pass
-
-        try:
-            if self.__need_gc:
-                newTable.__ref = self.__ref
-                self.__ref.inc()
-        except AttributeError:
-            pass
-
-        return newTable
-
-    def __copy__(self):
-        newTable = Table(data=self.__tableName, schemaInited=True, s=self.__session, needGC=self.__need_gc)
-        newTable._setExec(self.isExec)
-        newTable.isMaterialized = self.isMaterialized
-        try:
-            newTable.vecs = copy.copy(self.vecs)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__schemaInited = copy.copy(self.__schemaInited)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__select = copy.copy(self.__select)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__where = copy.copy(self.__where)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__groupby = copy.copy(self.__groupby)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__contextby = copy.copy(self.__contextby)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__having = copy.copy(self.__having)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__sort = copy.copy(self.__sort)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__top = copy.copy(self.__top)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__limit = copy.copy(self.__limit)
-        except AttributeError:
-            pass
-
-        try:
-            newTable.__csort = copy.copy(self.__csort)
-        except AttributeError:
-            pass
-
-        try:
-            if self.__need_gc:
-                newTable.__ref = self.__ref
-                self.__ref.inc()
-                # print("in copy ", self.__tableName, self.__ref.val())
-        except AttributeError:
-            pass
-
-        return newTable
-
-    def __del__(self):
-        # print("try to del ", self.__tableName, self.__ref.val())
-        if self.__need_gc:
-            if self.__ref.dec() == 0:
-                # print('do __del__', self.__tableName)
-                try:
-                    # this is not a real table name such as join table, no need to undef.
-                    if '(' in self.__tableName or ')' in self.__tableName:
-                        return
-                    # if self.__objAddr is None or self.__objAddr < 0:
-                    #     self.__session.run("undef('{}')".format(self.__tableName))
-                    # else:
-                    #     self.__session.run("undef('{}', VAR, {})".format(self.__tableName, self.__objAddr))
-                    if not self.__session.isClosed():
-                        if self.__tableName.find("TMP_TBL_") != -1:
-                            # print("undef ", self.__tableName)
-                            # tmp table, need to undef
-                            if self.__objAddr is None or self.__objAddr < 0:
-                                self.__session.run("undef('{}')".format(self.__tableName))
-                            else:
-                                self.__session.run("undef('{}', VAR)".format(self.__tableName))
-                except Exception as e:
-                    if get_verbose():
-                        print("undef table '{}' got an exception: ".format(self.__tableName))
-                        print(e)
-            # else:
-            #     print('__del__', self.__ref.val())
-
-    def _setSelect(self, cols):
-        self.__schemaInited = True
-        if isinstance(cols, tuple):
-            cols = list(cols)
-        if isinstance(cols, list) is False:
-            cols = [cols]
-
-        self.__select = cols
-
-    def _init_schema(self):
-        if self.__schemaInited is True:
-            return
-        self._init_columns()
-        self.vecs = {}
-        if self.__columns is not None:
-            if isinstance(self.__columns, list):
-                for colName in self.__columns:
-                    self.vecs[colName] = Vector(name=colName, tableName=self.__tableName, s=self.__session)
-                self._setSelect(self.__columns)
-            else:
-                self._setSelect(self.__columns)
-
-    def __getattr__(self, item):
-        vecs = object.__getattribute__(self, "vecs")
-        if item not in vecs:
-            return object.__getattribute__(self, item)
-        else:
-            return vecs[item]
-
-    def __getitem__(self, colOrCond):
-        if isinstance(colOrCond, FilterCond):
-            return self.where(colOrCond)
-        else:
-            return self.select(colOrCond)
-
-    def tableName(self) -> str:
-        """Get table name.
-
-        Returns:
-            name of the table in DolphinDB.
-        """
-        return self.__tableName
-
-    def _setTableName(self, tableName):
-        self.__tableName = tableName
-
-    def _getTableName(self):
-        return self.__tableName
-
-    def _setLeftTable(self, tableName):
-        self.__leftTable = tableName
-
-    def _setRightTable(self, tableName):
-        self.__rightTable = tableName
-
-    def getLeftTable(self) -> "Table":
-        """Get the left table of the join.
-
-        Returns:
-            the left table of the join.
-        """
-        return self.__leftTable
-
-    def getRightTable(self) -> "Table":
-        """Get the right table of the join.
-
-        Returns:
-            the right table of the join.
-        """
-        return self.__rightTable
-
-    def session(self):
-        """Get the Session where the Table belongs to.
-
-        Returns:
-            a Session where this Table belongs to.
-        """
-        return self.__session
-
-    def _addWhereCond(self, conds):
-        try:
-            _ = self.__where
-        except AttributeError:
-            self.__where = []
-
-        if isinstance(conds, list) or isinstance(conds, tuple):
-            self.__where.extend([str(x) for x in conds])
-        else:
-            self.__where.append(str(conds))
-
-    def _setSort(self, bys, ascending=True):
-        if isinstance(bys, list) or isinstance(bys, tuple):
-            self.__sort = [str(x) for x in bys]
-        else:
-            self.__sort = [str(bys)]
-        if isinstance(ascending, bool):
-            if not ascending:
-                self.__sort = [x + " desc" for x in self.__sort]
-            return
-        if (isinstance(ascending, list) or isinstance(ascending, tuple)) and (len(self.__sort) != len(ascending)):
-            raise ValueError(f"Length of ascending ({len(ascending)}) != length of by ({len(self.__sort)})")
-        self.__sort = [by + " desc" if not asc else by for by, asc in zip(self.__sort, ascending)]
-
-    def _setTop(self, num):
-        self.__top = str(num)
-
-    def _setCsort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True):
-        if isinstance(bys, list) or isinstance(bys, tuple):
-            self.__csort = [str(x) for x in bys]
-        else:
-            self.__csort = [str(bys)]
-        if isinstance(ascending, bool):
-            if not ascending:
-                self.__csort = [x + " desc" for x in self.__csort]
-            return
-        if (isinstance(ascending, list) or isinstance(ascending, tuple)) and (len(self.__csort) != len(ascending)):
-            raise ValueError(f"Length of ascending ({len(ascending)}) != length of by ({len(self.__csort)})")
-        self.__csort = [by + " desc" if not asc else by for by, asc in zip(self.__csort, ascending)]
-
-    def _setLimit(self, num):
-        if isinstance(num, list) or isinstance(num, tuple):
-            self.__limit = [str(x) for x in num]
-        else:
-            self.__limit = [str(num)]
-
-    def _setWhere(self, where):
-        self.__where = where
-
-    def select(self, cols: Union[str, Tuple[str, ...], List[str]]) -> "Table":
-        """Extract the specified columns and return them in a table.
-
-        Args:
-            cols : specify the columns to be extracted from table. Can be a string, a tuple of strings or a list of strings.
-
-        Returns:
-            a new Table object with the specified columns.
-        """
-        selectTable = copy.copy(self)
-        # print("ref of newTable: ", selectTable.__ref.val(), " self.ref: ", self.__ref.val())
-        selectTable._setSelect(cols)
-        if not self.isMaterialized:
-            selectTable.__tableName = f"({self.showSQL()})"
-        selectTable.isMaterialized = False
-        return selectTable
-
-    def exec(self, cols: Union[str, Tuple[str, ...], List[str]]) -> "Table":
-        """Generate a Table object containing the specified columns. The execution result is a scalar or vector.
-
-        Args:
-            cols : specify the columns. Can be a string, a tuple of strings or a list of strings.
-
-        Returns:
-            a new Table object of the specified columns.
-        """
-        selectTable = copy.copy(self)
-        selectTable._setSelect(cols)
-        selectTable._setExec(True)
-        if not self.isMaterialized:
-            selectTable.__tableName = f"({self.showSQL()})"
-        selectTable.isMaterialized = False
-        return selectTable
-
-    def where(self, conds) -> "Table":
-        """Add query conditions.
-
-        Args:
-            conds : query conditions.
-
-        Returns:
-            a new Table object with query conditions
-        """
-        # print("where", self.__tableName, __name__, conds)
-        whereTable = copy.copy(self)
-        whereTable._addWhereCond(conds)
-        return whereTable
-
-    def _setGroupby(self, groupby):
-        try:
-            _ = self.__contextby
-            raise RuntimeError('multiple context/group-by are not allowed ')
-        except AttributeError:
-            self.__groupby = groupby
-
-    def _setContextby(self, contextby):
-        try:
-            _ = self.__groupby
-            raise RuntimeError('multiple context/group-by are not allowed ')
-        except AttributeError:
-            self.__contextby = contextby
-
-    def _setHaving(self, having):
-        self.__having = having
-
-    def groupby(self, cols: Union[str, Tuple[str, ...], List[str]]) -> "TableGroupby":
-        """Apply group by on Table with specified columns.
-
-        Args:
-            cols : name of the grouping columns.
-
-        Returns:
-            a new TableGroupby object after adding the groupby.
-        """
-        groupbyTable = copy.copy(self)
-        groupby = TableGroupby(groupbyTable, cols)
-        groupbyTable._setGroupby(groupby)
-        return groupby
-
-    def sort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending=True) -> "Table":
-        """Specify parameter for sorting.
-
-        Args:
-            bys : the column(s) to sort on.
-            ascending : the sorting order. True: ascending order. Defaults to True.
-
-        Returns:
-            a new Table object after adding sort clause.
-        """
-        sortTable = copy.copy(self)
-        sortTable._setSort(bys, ascending)
-        return sortTable
-
-    def top(self, num: int) -> "Table":
-        """Retrieve the top n records from table.
-
-        Args:
-            num : the number of records to return. Must be a positive number.
-
-        Returns:
-            a new Table object with the top clause.
-        """
-        topTable = copy.copy(self)
-        topTable._setTop(num)
-        return topTable
-
-    def csort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True) -> "Table":
-        """Specify sorting column(s) for contextby.
-
-        Args:
-            bys : the column(s) to sort on.
-            ascending : the sorting order. True: ascending order. Defaults to True.
-
-        Returns:
-            a new Table object after adding csort clause.
-        """
-        csortTable = copy.copy(self)
-        csortTable._setCsort(bys, ascending)
-        return csortTable
-
-    def limit(self, num: Union[int, Tuple[int, ...], List[int]]) -> "Table":
-        """Specify parameters for limit.
-
-        Args:
-            num : when used with the contextby clause, the limit clause can use a negative integer to select a limited number of records in the end of each group. 
-                  In all other cases the limit clause can only use positive integers.
-                  Can pass in [x, y] to select data from row x to row y.
-
-        Returns:
-            a new Table object after adding the limit clause
-        """
-        limitTable = copy.copy(self)
-        limitTable._setLimit(num)
-        return limitTable
-
-    def execute(self, expr: Union[str, Tuple[str, ...], List[str]]) -> Any:
-        """Execute the SQL query.
-
-        Args:
-            expr : columns to be executed. Can be a string, tuple, or list.
-
-        Returns:
-            SQL query result.
-        """
-        if expr:
-            self._setSelect(expr)
-        pattern = re.compile("select", re.IGNORECASE)
-        query = pattern.sub('exec', self.showSQL())
-        return self.__session.run(query)
-
-    @property
-    def rows(self) -> int:
-        """Read-only property.
-
-        Get the row count of the Table.
-
-        Returns:
-            number of rows in the Table.
-        """
-        # if 'update' in self.showSQL().lower() or 'insert' in  self.showSQL().lower():
-        #     return self.__session.run('exec count(*) from %s'% self.__tableName)
-        sql = self.showSQL()
-        idx = sql.lower().index("from")
-        sql_new = "select count(*) as ct " + sql[idx:]
-        df = self.__session.run(sql_new)
-        if df.shape[0] > 1:
-            return df.shape[0]
-        else:
-            return df['ct'].iloc[0]
-
-    def _init_columns(self) -> None:
-        if not self.__columns:
-            schema = self.__session.run("schema(%s)" % self.__tableName)  # type: dict
-            columns = schema["colDefs"]["name"].tolist()
-            columns = [colName if _isVariableCandidate(colName) else f'_"{colName}"' for colName in columns]
-            self.__columns = columns
-
-    @property
-    def cols(self) -> int:
-        """read-only property.
-
-        Get the number of columns in the Table.
-
-        Returns:
-            the number of columns in the Table.
-        """
-        self._init_columns()
-        return len(self.__columns)
-
-    @property
-    def colNames(self) -> List[str]:
-        """read-only property.
-
-        Get all column names of the Table.
-
-        Returns:
-            all column names of the Table.
-        """
-        self._init_columns()
-        return [
-            col[2:-1] if len(col) >= 3 and col[0:2] == '_"' and col[-1] == '"' else col
-            for col in self.__columns
-        ]
-
-    @property
-    def schema(self) -> DataFrame:
-        """read-only property.
-
-        Get summary information of the Table.
-
-        Returns:
-            a DataFrame about summary information of the Table.
-        """
-        schema = self.__session.run("schema(%s)" % self.__tableName)  # type: dict
-        colDefs = schema.get('colDefs')  # type: DataFrame
-        return colDefs
-
-    @property
-    def isMergeForUpdate(self) -> bool:
-        """read-only property.
-
-        Decide whether the Table is to be joined.
-
-        Returns:
-            True means Table is to be joined.
-        """
-        return self.__merge_for_update
-
-    def setMergeForUpdate(self, toUpdate: bool):
-        """Mark if a Table is to be joined.
-
-        Args:
-            toUpdate : True means to mark the table as to be joined.
-        """
-        self.__merge_for_update = toUpdate
-
-    @property
-    def isExec(self) -> bool:
-        """read-only property.
-
-        Whether the SQL statement has an exec clause.
-
-        Returns:
-            True means the SQL statement has added an exec clause.
-        """
-        return self.__exec
-
-    def _setExec(self, isExec):
-        self.__exec = isExec
-
-    def pivotby(self, index: str, column: str, value=None, aggFunc=None) -> "TablePivotBy":
-        """Add pivot by clause to rearrange a column (or multiple columns) of a table on two dimensions.
-
-        Args:
-            index : the result table has the same number of rows as unique values on this column.
-            column : the result table has the same number of columns as unique values on this column.
-            value : the parameters of the aggregate function. Defaults to None.
-            aggFunc : the specified aggregate function. Defaults to lambda x: x.
-
-        Returns:
-            a TablePivotBy object.
-        """
-        pivotByTable = copy.copy(self)
-        return TablePivotBy(pivotByTable, index, column, value, aggFunc)
-
-    def merge(
-            self, right, how: str = 'inner', on: Union[str, Tuple[str, ...], List[str]] = None,
-            left_on: Union[str, Tuple[str, ...], List[str]] = None,
-            right_on: Union[str, Tuple[str, ...], List[str]] = None,
-            sort: bool = False, merge_for_update: bool = False
-    ) -> "Table":
-        """Join two table objects with ANSI SQL.
-
-        Args:
-            right : the right table from local or remote server.
-            how : connection type. The options are {"left", "right", "outer", "inner"}. Defaults to 'inner'.
-        | How   | Link                                                                 |
-        | :---- | :------------------------------------------------------------------- |
-        | left  | https://dolphindb.com/help/SQLStatements/TableJoiners/leftjoin.html  |
-        | right | https://dolphindb.com/help/SQLStatements/TableJoiners/leftjoin.html  |
-        | outer | https://dolphindb.com/help/SQLStatements/TableJoiners/fulljoin.html  |
-        | ineer | https://dolphindb.com/help/SQLStatements/TableJoiners/equaljoin.html |   
-            on : the columns to join on. If the column names are different in two tables, use the left_on and right_on parameters. Defaults to None.
-            left_on : the column to join on from the left table. Defaults to None.
-            right_on : the column to join on from the right table. Defaults to None.
-            sort : True means to enable sorting. Defaults to False.
-            merge_for_update : True means marking tables as to be joined. Defaults to False.
-
-        Note:
-            A partitioned table can only outer join a another partitioned table. An in-memory table can only outer join another in-memory table.
-
-        Returns:
-            the joined Table object.
-        """
-        howMap = {
-            'inner': 'ej',
-            'left': 'lj',
-            'right': 'lj',
-            'outer': 'fj',
-            'left semi': 'lsj'
-        }
-        joinFunc = howMap[how]
-        joinFuncPrefix = '' if sort is False or joinFunc == 'fj' else 's'
-
-        if self.isMaterialized or merge_for_update:
-            leftTableName = self.tableName()
-        else:
-            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
-
-        if right.isMaterialized:
-            rightTableName = right.tableName() if isinstance(right, Table) else right
-        else:
-            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
-
-        if how == 'right':
-            leftTableName, rightTableName = rightTableName, leftTableName
-            left_on, right_on = right_on, left_on
-
-        if on is not None and not isinstance(on, list) and not isinstance(on, tuple):
-            on = [on]
-        if left_on is not None and not isinstance(left_on, list) and not isinstance(left_on, tuple):
-            left_on = [left_on]
-        if right_on is not None and not isinstance(right_on, list) and not isinstance(right_on, tuple):
-            right_on = [right_on]
-
-        if on is not None:
-            left_on, right_on = on, on
-        elif left_on is None and right_on is None:
-            raise Exception('at least one of {\'on\', \'left_on\', \'right_on\'} must be present')
-        elif left_on is not None and right_on is not None and len(left_on) != len(right_on):
-            raise Exception('\'left_on\' must have the same length as \'right_on\'')
-
-        if left_on is None and right_on is not None:
-            left_on = right_on
-        if right_on is None and left_on is not None:
-            right_on = left_on
-
-        leftColumnNames = ''.join(['`' + x for x in left_on])
-        rightColumnNames = ''.join(['`' + x for x in right_on])
-        finalTableName = '%s(%s,%s,%s,%s)' % (
-            joinFuncPrefix + joinFunc, leftTableName, rightTableName, leftColumnNames, rightColumnNames
-        )
-        # print(finalTableName)
-        self._init_schema()
-        right._init_schema()
-        joinTable = copy.copy(self)
-        # leftAliasPrefix = 'lhs_' if how != 'right' else 'rhs_'
-        # rightAliasPrefix = 'rhs_' if how != 'right' else 'lhs_'
-        # leftSelectCols = [leftTableName + '.' + col + ' as ' + leftTableName + "_" + col for col in self._getSelect()]
-        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in right._getSelect()]
-        # leftSelectCols = self._getSelect()
-        # print(leftSelectCols)
-        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in
-        #                    right._getSelect() if col in self._getSelect()]
-        # print(rightSelectCols)
-        joinTable._setLeftTable(self.tableName())
-        joinTable._setRightTable(right.tableName())
-        joinTable._setTableName(finalTableName)
-        # joinTable._setSelect(leftSelectCols + rightSelectCols)
-        joinTable._setSelect('*')
-        if merge_for_update:
-            joinTable.setMergeForUpdate(True)
-        joinTable.isMaterialized = False
-        return joinTable
-
-    def merge_asof(
-        self, right, on: Union[str, Tuple[str, ...], List[str]] = None,
-        left_on: Union[str, Tuple[str, ...], List[str]] = None,
-        right_on: Union[str, Tuple[str, ...], List[str]] = None
-    ) -> "Table":
-        """Use asof join to join two Table objects.
-
-        Refer to https://dolphindb.com/help/SQLStatements/TableJoiners/asofjoin.html.
-
-        Args:
-            right : The right table from local or remote server.
-            on : the columns to join on. If the column names are different in two tables, use the left_on and right_on parameters. Defaults to None.
-            left_on : the column to join on from the left table. Defaults to None.
-            right_on : the column to join on from the right table. Defaults to None.
-
-        Returns:
-            the joined Table object.
-        """
-        if self.isMaterialized:
-            leftTableName = self.tableName()
-        else:
-            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
-
-        if right.isMaterialized:
-            rightTableName = right.tableName() if isinstance(right, Table) else right
-        else:
-            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
-
-        if on is not None and not isinstance(on, list) and not isinstance(on, tuple):
-            on = [on]
-        if left_on is not None and not isinstance(left_on, list) and not isinstance(left_on, tuple):
-            left_on = [left_on]
-        if right_on is not None and not isinstance(right_on, list) and not isinstance(right_on, tuple):
-            right_on = [right_on]
-
-        if on is not None:
-            left_on, right_on = on, on
-        elif left_on is None and right_on is None:
-            raise Exception('at least one of {\'on\', \'left_on\', \'right_on\'} must be present')
-        elif left_on is not None and right_on is not None and len(left_on) != len(right_on):
-            raise Exception('\'left_on\' must have the same length as \'right_on\'')
-
-        if left_on is None and right_on is not None:
-            left_on = right_on
-        if right_on is None and left_on is not None:
-            right_on = left_on
-
-        leftColumnNames = ''.join(['`' + x for x in left_on])
-        rightColumnNames = ''.join(['`' + x for x in right_on])
-        finalTableName = 'aj(%s,%s,%s,%s)' % (
-            leftTableName, rightTableName, leftColumnNames, rightColumnNames
-        )
-        self._init_schema()
-        right._init_schema()
-        joinTable = copy.copy(self)
-        # leftAliasPrefix = 'lhs_'
-        # rightAliasPrefix = 'rhs_'
-        # leftSelectCols = [leftTableName + '.' + col + ' as ' + leftTableName +"_" + col for col in self._getSelect()]
-        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in right._getSelect()]
-        # leftSelectCols = self._getSelect()
-        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in
-        #                    right._getSelect() if col in self._getSelect()]
-        joinTable._setLeftTable(self.tableName())
-        joinTable._setRightTable(right.tableName())
-        joinTable._setTableName(finalTableName)
-        joinTable._setSelect('*')
-        # joinTable._setSelect(leftSelectCols + rightSelectCols)
-        joinTable.isMaterialized = False
-        return joinTable
-
-    def merge_window(
-        self, right, leftBound: int, rightBound: int,
-        aggFunctions: Union[str, List[str]], on: Union[str, Tuple[str, ...], List[str]] = None,
-        left_on: Union[str, Tuple[str, ...], List[str]] = None,
-        right_on: Union[str, Tuple[str, ...], List[str]] = None,
-        prevailing: bool = False
-    ) -> "Table":
-        """Use window join to join two Table objects.
-
-        Args:
-            right : the name of the right table from local or remote server.
-            leftBound : left boundary (inclusive) of the window. Defaults to None.
-            rightBound : right boundary (inclusive) of the window. Defaults to None.
-            aggFunctions : aggregate function. Defaults to None.
-            on : the columns to join on. If the column names are different in two tables, use the left_on and right_on parameters. Defaults to None.
-            left_on : the column to join on from the left table. Defaults to None.
-            right_on : the column to join on from the right table. Defaults to None.
-            prevailing : whether to use prevailing window join. True: use prevailing window join. Defaults to False.
-
-        Returns:
-            the joined Table object.
-        """
-
-        if self.isMaterialized:
-            leftTableName = self.tableName()
-        else:
-            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
-
-        if right.isMaterialized:
-            rightTableName = right.tableName() if isinstance(right, Table) else right
-        else:
-            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
-
-        ifPrevailing = False
-
-        if prevailing is not None:
-            ifPrevailing = prevailing
-
-        if on is not None and not isinstance(on, list) and not isinstance(on, tuple):
-            on = [on]
-        if left_on is not None and not isinstance(left_on, list) and not isinstance(left_on, tuple):
-            left_on = [left_on]
-        if right_on is not None and not isinstance(right_on, list) and not isinstance(right_on, tuple):
-            right_on = [right_on]
-
-        if on is not None:
-            left_on, right_on = on, on
-        elif left_on is None and right_on is None:
-            raise Exception('at least one of {\'on\', \'left_on\', \'right_on\'} must be present')
-        elif left_on is not None and right_on is not None and len(left_on) != len(right_on):
-            raise Exception('\'left_on\' must have the same length as \'right_on\'')
-
-        if left_on is None and right_on is not None:
-            left_on = right_on
-        if right_on is None and left_on is not None:
-            right_on = left_on
-
-        leftColumnNames = ''.join(['`' + x for x in left_on])
-        rightColumnNames = ''.join(['`' + x for x in right_on])
-        if isinstance(aggFunctions, list):
-            aggFunctions = '[' + ','.join(aggFunctions) + ']'
-        if ifPrevailing:
-            finalTableName = 'pwj(%s,%s,%d:%d,%s,%s,%s)' % (
-                leftTableName, rightTableName, leftBound, rightBound,
-                '<' + aggFunctions + '>', leftColumnNames, rightColumnNames
-            )
-        else:
-            finalTableName = 'wj(%s,%s,%d:%d,%s,%s,%s)' % (
-                leftTableName, rightTableName, leftBound, rightBound, '<' + aggFunctions + '>', leftColumnNames,
-                rightColumnNames)
-        # print(finalTableName)
-        self._init_schema()
-        right._init_schema()
-        joinTable = copy.copy(self)
-        joinTable._setLeftTable(self.tableName())
-        joinTable._setRightTable(right.tableName())
-        joinTable._setTableName(finalTableName)
-        joinTable._setSelect('*')
-        return joinTable
-
-    def merge_cross(self, right) -> "Table":
-        """Perform a cross join with another table and return their Cartesian product.
-
-        Args:
-            right : the name of the right table from local or remote server.
-
-        Returns:
-            the joined Table object.
-        """
-        if self.isMaterialized:
-            leftTableName = self.tableName()
-        else:
-            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
-
-        if right.isMaterialized:
-            rightTableName = right.tableName() if isinstance(right, Table) else right
-        else:
-            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
-
-        finalTableName = 'cj(%s,%s)' % (leftTableName, rightTableName)
-        self._init_schema()
-        right._init_schema()
-        joinTable = copy.copy(self)
-        joinTable._setLeftTable(self.tableName())
-        joinTable._setRightTable(right.tableName())
-        joinTable._setTableName(finalTableName)
-        joinTable._setSelect("*")
-        return joinTable
-
-    def _getSelect(self):
-        return self.__select
-
-    def _assembleSelect(self):
-        try:
-            if len(self.__select) and isinstance(self.__select, list):
-                return ','.join(self.__select)
-            else:
-                return '*'
-        except AttributeError:
-            return '*'
-        except ValueError:
-            return '*'
-
-    def _assembleWhere(self):
-        try:
-            if len(self.__where) == 1:
-                return 'where ' + self.__where[0]
-            else:
-                return 'where ' + ' and '.join(["(" + x + ")" for x in self.__where])
-        except AttributeError:
-            return ''
-
-    def _assembleGroupbyOrContextby(self):
-        try:
-            return 'group by ' + ','.join(self.__groupby)
-        except AttributeError:
-            try:
-                return 'context by ' + ','.join(self.__contextby)
-            except AttributeError:
-                return ''
-
-    def _assembleOrderby(self):
-        try:
-            return 'order by ' + ','.join(self.__sort)
-        except AttributeError:
-            return ''
-
-    def _assembleCsort(self):
-        try:
-            return 'csort ' + ','.join(self.__csort)
-        except AttributeError:
-            return ''
-
-    def _assembleLimit(self):
-        try:
-            if (self.__limit is None):
-                return ''
-            if len(self.__limit) and isinstance(self.__limit, list):
-                return 'limit ' + ','.join(self.__limit)
-            else:
-                return self.__limit
-        except AttributeError:
-            return ''
-
-    def showSQL(self) -> str:
-        """View SQL query.
-
-        Returns:
-            the SQL query for the current Table.
-        """
-        import re
-        selectOrExec = "exec" if self.isExec else "select"
-        queryFmt = selectOrExec + ' {top} {select} from {table} {where} {groupby} {csort} {having} {orderby} {limit}'
-        fmtDict = {}
-        fmtDict['top'] = ("top " + self.__top) if self.__top else ''
-        fmtDict['select'] = self._assembleSelect()
-        fmtDict['table'] = self.tableName()
-        fmtDict['where'] = self._assembleWhere()
-        fmtDict['groupby'] = self._assembleGroupbyOrContextby()
-        fmtDict['csort'] = self._assembleCsort()
-        fmtDict['having'] = ("having " + self.__having) if self.__having else ''
-        fmtDict['orderby'] = self._assembleOrderby()
-        fmtDict['limit'] = self._assembleLimit()
-        query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
-        # print(query)
-        # if(self.__tableName.startswith("wj") or self.__tableName.startswith("pwj")):
-        #     return self.__tableName
-
-        if get_verbose():
-            print(query)
-        return query
-
-    def append(self, table: "Table") -> "Table":
-        """Append data to Table and execute at once.
-
-        Args:
-            table : Table object to be appended.
-
-        Returns:
-            the appended Table object.
-
-        Note:
-            The data in the DolphinDB server will be modified immediately.
-        """
-        if not isinstance(table, Table):
-            raise RuntimeError("Only DolphinDB Table object is accepted")
-
-        runstr = "%s.append!(%s)" % (self.tableName(), table.tableName())
-        self.__session.run(runstr)
-        return self
-
-    def update(self, cols: List[str], vals: List[str]) -> "TableUpdate":
-        """Update in-memory table. Must be called to be executed.
-
-        Args:
-            cols : list of names of columns to be updated.
-            vals : a list of values to be updated.
-
-        Returns:
-            a TableUpdate object.
-        """
-        # print("update for ", self.__tableName)
-        tmp = copy.copy(self)
-        if self.isMergeForUpdate:
-            tmp._setLeftTable(self.getLeftTable())
-        contextby = self.__contextby if hasattr(self, '__contextby') else None
-        having = self.__having if hasattr(self, '__having') else None
-        updateTable = TableUpdate(t=tmp, cols=cols, vals=vals, contextby=contextby, having=having)
-        updateTable._setMergeForUpdate(self.isMergeForUpdate)
-        return updateTable
-
-    def rename(self, newName: str) -> None:
-        """Rename table.
-
-        Args:
-            newName : new table name.
-        """
-        self.__session.run(newName + '=' + self.tableName())
-        self.__tableName = newName
-
-    def delete(self) -> "TableDelete":
-        """Delete table.
-
-        Returns:
-            a TableDelete object.
-        """
-        tmp = copy.copy(self)
-        delTable = TableDelete(t=tmp)
-        return delTable
-
-    def drop(self, cols: Union[List[str], str]) -> "Table":
-        """Delete columns.
-
-        Args:
-            cols : list of columns to be deleted.
-
-        Returns:
-            a Table object.
-        """
-        if isinstance(cols, str):
-            cols = [cols]
-        if not isinstance(cols, list):
-            raise TypeError("cols must be a str or a list of str.")
-        cols = [
-            col[2:-1] if len(col) >= 3 and col[0:2] == '_"' and col[-1] == '"' else col
-            for col in cols
-        ]
-        if len(cols) == 1:
-            query = f'{self.tableName()}.drop!("{str(cols[0])}")'
-        if len(cols) > 1:
-            runstr = '{table}.drop!([{cols}])'
-            fmtDict = dict()
-            fmtDict['table'] = self.tableName()
-            fmtDict['cols'] = '"' + '","'.join(cols) + '"'
-            query = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
-        if cols:
-            remove_list = []
-            for col in cols:
-                for colName in self.__select:
-                    col_o = colName[2:-1] if len(colName) >= 3 and colName[0:2] == '_"' and colName[-1] == '"' else colName
-                    if col.lower() == col_o.lower():
-                        remove_list.append(colName)
-            for colName in remove_list:
-                self.__select.remove(colName)
-            self.__session.run(query)
-        return self
-
-    def executeAs(self, newTableName: str) -> "Table":
-        """Save execution result as an in-memory table with a specified name.
-
-        Args:
-            newTableName : new table name.
-
-        Returns:
-            a new Table object saved with the new table name.
-        """
-        st = newTableName + "=(" + self.showSQL() + ")"
-        # print(st)
-        self.__session.run(st)
-        return Table(data=newTableName, s=self.__session)
-
-    def contextby(self, cols: Union[str, List[str]]) -> "TableContextby":
-        """Group by specified columns.
-
-        Args:
-            cols : name of the columns to context by.
-
-        Returns:
-            a TableContextby object after adding context by clause.
-        """
-        contextbyTable = copy.copy(self) # Table
-        contextbyTable.__merge_for_update = self.__merge_for_update
-        contextby = TableContextby(contextbyTable, cols)
-        contextbyTable._setContextby(contextby)
-        contextbyTable._setTableName(self.tableName())
-        return contextby
-
-    def ols(self, Y:str, X:Union[str, List[str]], INTERCEPT: bool = True) -> dict:
-        """Calculate Least Squares Regression Coefficients.
-
-        Refer to https://dolphindb.com/help/FunctionsandCommands/FunctionReferences/o/ols.html.
-
-        Args:
-            Y : dependent variable, column name.
-            X : argument, list of column names.
-            INTERCEPT : whether to include the intercept in the regression. Defaults to True, meaning that the system automatically adds a column of "1" to X to generate the intercept.
-
-        Returns:
-            a dictionary with ANOVA, RegressionStat, Cofficient and Residual.
-        """
-        myY = ""
-        myX = []
-
-        if isinstance(Y, str):
-            myY = Y
-        else:
-            raise ValueError("Y must be a column name")
-        if isinstance(X, str):
-            myX = [X]
-        elif isinstance(X, list):
-            myX = X
-        else:
-            raise ValueError("X must be a column name or a list of column names")
-        if not len(myY) or not len(myX):
-            raise ValueError("Invalid Input data")
-        schema = self.__session.run("schema(%s)" % self.__tableName)
-        if 'partitionColumnName' in schema and schema['partitionColumnName']:
-            dsstr = "sqlDS(<SQLSQL>)".replace('SQLSQL', self.showSQL()).replace('select select', 'select')
-            runstr = "olsEx({ds},{Y},{X},{INTERCEPT},2)"
-            fmtDict = dict()
-            fmtDict['table'] = self.tableName()
-            fmtDict['Y'] = '"' + myY + '"'
-            fmtDict['X'] = str(myX)
-            fmtDict['ds'] = dsstr
-            fmtDict['INTERCEPT'] = str(INTERCEPT).lower()
-            query = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
-            # print(query)
-            return self.__session.run(query)
-        else:
-            runstr = "z=exec ols({Y},{X},{INTERCEPT},2) from {table}"
-            fmtDict = dict()
-            fmtDict['table'] = self.tableName()
-            fmtDict['Y'] = myY
-            fmtDict['X'] = str(myX)
-            fmtDict['INTERCEPT'] = str(INTERCEPT).lower()
-            query = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
-            # print(query)
-            return self.__session.run(query)
-
-    def toDF(self) -> DataFrame:
-        """Execute SQL statement and return a DataFrame object.
-
-        Returns:
-            data queried by SQL in DataFrame form.
-        """
-        self._init_schema()
-        query = self.showSQL()
-        df = self.__session.run(query)  # type: DataFrame
-        return df
-
-    def toList(self) -> list:
-        """Execute SQL statement and return a List object.
-
-        Returns:
-            list: the query result in the form of a list. The length of the list is same as the rows of the Table.
-
-        Note:
-            If the table contains columns of array vectors, the system will try to convert them to NumPy 2D arrays. 
-            The conversion will fail if the rows in the array vector are different.
-        """
-        self._init_schema()
-        query = self.showSQL()
-        list = self.__session.run(query, pickleTableToList=True)  # type: DataFrame
-        return list
-
-    toDataFrame = toDF
-
-
-class TableDelete(object):
-    """Table object to be deleted.
-
-    Args:
-        t : Table object to be deleted.
-    """
-    def __init__(self, t):
-        """Constructor of TableDelete."""
-        self.__t = t
-        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
-
-    def _assembleWhere(self):
-        try:
-            if len(self.__where) == 1:
-                return 'where ' + self.__where[0]
-            else:
-                return 'where ' + ' and '.join(["(" + x + ")" for x in self.__where])
-        except AttributeError:
-            return ''
-
-    def _addWhereCond(self, conds):
-        try:
-            _ = self.__where
-        except AttributeError:
-            self.__where = []
-
-        if isinstance(conds, list) or isinstance(conds, tuple):
-            self.__where.extend([str(x) for x in conds])
-        else:
-            self.__where.append(str(conds))
-
-    def where(self, conds) -> "TableDelete":
-        """Add query conditions.
-
-        Args:
-            conds : query conditions.
-
-        Returns:
-            a TableDelete object with query conditions.
-        """
-        # print("where", self.__t.__dict__["_Table__tableName"], __name__, conds)
-        self._addWhereCond(conds)
-        return self
-
-    def __executesql(self) -> str:
-        return self.showSQL()
-
-    def showSQL(self) -> str:
-        """View SQL query.
-
-        Returns:
-            the SQL statement for the current TableDelete object.
-        """
-        curframe = inspect.currentframe()
-        calframe = inspect.getouterframes(curframe, 2)
-        caller = calframe[1][3]
-        if caller != 'execute' and caller != 'print' and caller != "str" and caller != '<module>' and caller != '__executesql':
-            return self.__t.showSQL()
-        queryFmt = 'delete from {table} {where}'
-        fmtDict = {}
-        fmtDict['table'] = self.__t.tableName()
-        fmtDict['where'] = self._assembleWhere()
-        query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
-        return query
-
-    def execute(self) -> "Table":
-        """Execute the SQL query.
-
-        Returns:
-            Table: SQL query result as Table.
-        """
-        query = self.showSQL()
-        self.__t.session().run(query)
-        return self.__t
-
-    def toDF(self) -> DataFrame:
-        """Execute SQL statement and return a DataFrame object.
-
-        Returns:
-            data queried by SQL in DataFrame form.
-        """
-        query = self.showSQL()
-
-        df = self.__t.session().run(query)  # type: DataFrame
-
-        return df
-
-
-class TableUpdate(object):
-    """Table object to be updated.
-
-    Args:
-        t : Table object to be updated.
-        cols : list of names of columns to be updated.
-        vals : a list of values corresponding to the columns to be updated.
-        contextby : whether SQL query contains a contextby clause. True means there is. Defaults to None.
-        having : the content contained in a having clause. Defaults to None.
-    """
-    def __init__(self, t: "Table", cols: List[str], vals: List[str], contextby=None, having: str = None):
-        """Constructor of TableUpdate."""
-        self.__t = t
-        self.__cols = cols
-        self.__vals = vals
-        self.__contextby = contextby
-        self.__having = having
-        self.__merge_for_update = False
-        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
-
-    def _setMergeForUpdate(self, toMerge):
-        self.__merge_for_update = toMerge
-
-    def _assembleUpdate(self):
-        query = ""
-        for col, val in zip(self.__cols, self.__vals):
-            query += col + "=" + val + ","
-        return query[:-1]
-
-    def _assembleWhere(self):
-        try:
-            if len(self.__where) == 1:
-                return 'where ' + self.__where[0]
-            else:
-                return 'where ' + ' and '.join(["(" + x + ")" for x in self.__where])
-        except AttributeError:
-            return ''
-
-    def _addWhereCond(self, conds):
-        try:
-            _ = self.__where
-        except AttributeError:
-            self.__where = []
-
-        if isinstance(conds, list) or isinstance(conds, tuple):
-            self.__where.extend([str(x) for x in conds])
-        else:
-            self.__where.append(str(conds))
-
-    def where(self, conds) -> "TableUpdate":
-        """Add query conditions.
-
-        Args:
-            conds : query conditions.
-
-        Returns:
-            a TableUpdate object with query conditions.
-        """
-        # print("where", self.__t.__dict__["_Table__tableName"], __name__, conds)
-        self._addWhereCond(conds)
-        return self
-
-    def __executesql(self) -> str:
-        return self.showSQL()
-
-    def showSQL(self) -> str:
-        """View SQL query.
-
-        Returns:
-            the SQL statement for the current TableUpdate object.
-        """
-        curframe = inspect.currentframe()
-        calframe = inspect.getouterframes(curframe, 2)
-        caller = calframe[1][3]
-        if caller != 'execute' and caller != 'print' and caller != "str" and caller != '<module>' and caller != '__executesql':
-            return self.__t.showSQL()
-        if not self.__merge_for_update:
-            queryFmt = 'update {table} set {update} {where} {contextby} {having}'
-            fmtDict = {}
-            fmtDict['update'] = self._assembleUpdate()
-            fmtDict['table'] = self.__t.tableName()
-            fmtDict['where'] = self._assembleWhere()
-            if self.__contextby:
-                fmtDict['contextby'] = 'context by ' + ','.join(self.__contextby)
-            else:
-                fmtDict['contextby'] = ""
-            if self.__having:
-                fmtDict['having'] = ' having ' + self.__having
-            else:
-                fmtDict['having'] = ""
-            query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
-            if get_verbose():
-                print(query)
-            return query
-        else:
-            if self.__t.getLeftTable() is None:
-                raise Exception("Join for update missing left table!")
-            queryFmt = 'update {table} set {update} from {joinTable} {where} {contextby} {having}'
-            fmtDict = {}
-            fmtDict['update'] = self._assembleUpdate()
-            fmtDict['table'] = self.__t.getLeftTable()
-            fmtDict['joinTable'] = self.__t.tableName()
-            fmtDict['where'] = self.__t._assembleWhere()
-            if self.__contextby:
-                fmtDict['contextby'] = 'context by ' + ','.join(self.__t.__contextby)
-            else:
-                fmtDict['contextby'] = ""
-            if self.__having:
-                fmtDict['having'] = ' having ' + self.__having
-            else:
-                fmtDict['having'] = ""
-            query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
-            self.__t.setMergeForUpdate(False)
-            if get_verbose():
-                print(query)
-            return query
-
-    def execute(self) -> "Table":
-        """Execute the SQL query.
-
-        Returns:
-            SQL query result as Table.
-        """
-        query = self.showSQL()
-        # print(query)
-        self.__t.session().run(query)
-        t = Table(data=self.__t.tableName(), s=self.__t.session(), needGC=self.__t.__dict__["_Table__need_gc"])
-        if self.__t.__dict__["_Table__need_gc"]:
-            t.__dict__["_Table__ref"] = self.__t.__dict__["_Table__ref"]
-            t.__dict__["_Table__ref"].inc()
-        return t
-
-    def toDF(self) -> DataFrame:
-        """Execute SQL statement and return a DataFrame object.
-
-        Returns:
-            data queried by SQL in DataFrame form.
-        """
-        query = self.showSQL()
-        df = self.__t.session().run(query)  # type: DataFrame
-        return df
-
-
-class TablePivotBy(object):
-    """Add pivot by clause to rearrange a column (or multiple columns) of a table on two dimensions.
-
-    Args:
-        t : Table object
-        index : the result table has the same number of rows as unique values on this column.
-        column : the result table has the same number of columns as unique values on this column.
-        value : the parameters of the aggregate function. Defaults to None.
-        agg : the specified aggregate function. Defaults to lambda x: x.
-    """
-    def __init__(self, t: "Table", index: str, column: str, value=None, agg=None):
-        """Constructor of TablePivotBy."""
-        self.__row = index
-        self.__column = column
-        self.__val = value
-        self.__t = t
-        self.__agg = agg
-        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
-
-    def toDF(self) -> DataFrame:
-        """Execute SQL statement and return a DataFrame object.
-
-        Returns:
-            data queried by SQL in DataFrame form.
-        """
-        query = self.showSQL()
-        if get_verbose():
-            print(query)
-        df = self.__t.session().run(query)  # type: DataFrame
-
-        return df
-
-    toDataFrame = toDF
-
-    def _assembleSelect(self):
-        if self.__val is not None:
-            return self.__val if self.__agg is None else _getFuncName(self.__agg) + '(' + self.__val + ')'
-        return None
-
-    def _assembleTableSelect(self):
-        return self.__t._assembleSelect()
-
-    def _assembleWhere(self):
-        return self.__t._assembleWhere()
-
-    def _assemblePivotBy(self):
-        return 'pivot by ' + self.__row + ',' + self.__column
-
-    def executeAs(self, newTableName: str) -> "Table":
-        """Save execution result as an in-memory table with a specified name.
-
-        Args:
-            newTableName : new table name.
-
-        Returns:
-            a new Table object saved with the new table name.
-        """
-        self.__t.session().run(newTableName + "=" + self.showSQL())
-        return Table(data=newTableName, s=self.__t.session())
-
-    def showSQL(self) -> str:
-        """View SQL query.
-
-        Returns:
-            the SQL query for the current Table.
-        """
-        import re
-        selectOrExec = "exec" if self.__t.isExec else "select"
-        queryFmt = selectOrExec + ' {select} from {table} {where} {pivotby}'
-        fmtDict = {}
-        select = self._assembleSelect()
-        if select is not None:
-            fmtDict['select'] = select
-        else:
-            fmtDict['select'] = self._assembleTableSelect()
-        fmtDict['table'] = self.__t.tableName()
-        fmtDict['where'] = self._assembleWhere()
-        fmtDict['pivotby'] = self._assemblePivotBy()
-        query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
-        return query
-
-    def selectAsVector(self, colName: Union[str, Tuple[str, ...], List[str]]) -> np.array:
-        """Execute query and return the specified columns.
-
-        Args:
-            colName : a string indicating the column name.
-
-        Returns:
-            data queried by SQL in numpy.array form.
-        """
-        if colName:
-            self.__t._setSelect(colName)
-        pattern = re.compile("select", re.IGNORECASE)
-        query = pattern.sub('exec', self.showSQL())
-        return self.__t.session().run(query)
-
-
-class TableGroupby(object):
-    """The table object to which the group by clause is to be added.
-
-    Args:
-        t : Table object to be added the group by clause.
-        groupBys : grouping column(s).
-        having : the content contained in a having clause. Defaults to None.
-    """
-    def __init__(self, t: "Table", groupBys: Union[str, List[str]], having: str = None):
-        """Constructor of TableGroupby."""
-        if isinstance(groupBys, list):
-            self.__groupBys = groupBys
-        else:
-            self.__groupBys = [groupBys]
-        self.__having = having
-        self.__t = t  # type: Table
-        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
-
-    def sort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: bool = True) -> "TableGroupby":
-        """Specify parameter for sorting.
-
-        Args:
-            bys : the column(s) to sort on.
-            ascending : the sorting order. True: ascending order. Defaults to True.
-
-        Returns:
-            a TableGroupby object after adding sort clause.
-        """
-        sortTable = copy.copy(self.__t)
-        sortTable._setSort(bys, ascending)
-        return TableGroupby(sortTable, self.__groupBys, self.__having)
-
-    def csort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True) -> "TableGroupby":
-        """Specify sorting parameters for context by.
-
-        Args:
-            bys : the column to sort on.
-            ascending : the sorting order. True: ascending order. Defaults to True.
-
-        Returns:
-            a TableGroupby object after adding csort clause.
-        """
-        csortTable = copy.copy(self.__t)
-        csortTable._setCsort(bys, ascending)
-        return TableGroupby(csortTable, self.__groupBys, self.__having)
-
-    def executeAs(self, newTableName: str) -> "Table":
-        """Save execution result as an in-memory table with a specified name.
-
-        Args:
-            newTableName : new table name.
-
-        Returns:
-            a new Table object saved with the new table name.
-        """
-        st = newTableName + "=" + self.showSQL()
-        # print(st)
-        self.__t.session().run(st)
-        return Table(data=newTableName, s=self.__t.session())
-
-    def __getitem__(self, item):
-        selectTable = self.__t.select(item)
-        return TableGroupby(selectTable, groupBys=self.__groupBys, having=self.__having)
-
-    def __iter__(self):
-        self.__groupBysIdx = 0
-        return self
-
-    def next(self) -> str:
-        """Get the name of the next group by column.
-
-        Returns:
-            column name.
-        """
-        try:
-            result = self.__groupBys[self.__groupBysIdx]
-        except IndexError:
-            raise StopIteration
-        self.__groupBysIdx += 1
-        return result
-
-    def __next__(self):
-        return self.next()
-
-    def having(self, expr: str) -> "Table":
-        """Add having clause.
-
-        Args:
-            expr : expression for the having clause.
-
-        Returns:
-            a Table object after adding the having clause.
-        """
-        havingTable = copy.copy(self.__t)
-        self.__having = expr
-        havingTable._setHaving(self.__having)
-        return havingTable
-
-    def ols(self, Y: str, X: List[str], INTERCEPT: bool = True) -> dict:
-        """Calculate Least Squares Regression Coefficients.
-
-        Refer to https://dolphindb.com/help/FunctionsandCommands/FunctionReferences/o/ols.html.
-
-        Args:
-            Y : dependent variable, column name.
-            X : argument, list of column names.
-            INTERCEPT : whether to include the intercept in the regression. Defaults to True, meaning that the system automatically adds a column of "1" to X to generate the intercept.
-
-        Returns:
-            a dictionary with ANOVA, RegressionStat, Cofficient and Residual.
-        """
-        return self.__t.ols(Y=Y, X=X, INTERCEPT=INTERCEPT)
-
-    def selectAsVector(self, colName: str) -> np.array:
-        """Execute query and return the specified column.
-
-        Args:
-            colName : a string indicating the column name.
-
-        Returns:
-            data queried by SQL in numpy.array form.
-        """
-        if colName:
-            self.__t._setSelect(colName)
-        pattern = re.compile("select", re.IGNORECASE)
-        query = pattern.sub('exec', self.showSQL())
-        return self.__t.session().run(query)
-
-    def showSQL(self) -> str:
-        """View SQL query.
-
-        Returns:
-            return the SQL query for the current Table.
-        """
-        return self.__t.showSQL()
-
-    def agg(self, func) -> "Table":
-        """Apply group by on all columns.
-
-        Args:
-            func : can be an aggregate function, a list of aggregate functions, or a dict where each key indicates a column and the corresponding value indicates the aggregate function to be applied to this column.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        selectCols = self.__t._getSelect()
-        if isinstance(func, list):
-            selectCols = [_getFuncName(f) + '(' + x + ')' for x in selectCols for f in
-                          func]  # if x not in self.__groupBys
-        elif isinstance(func, dict):
-            funcDict = {}
-            for colName, f in func.items():
-                funcDict[colName] = f if isinstance(f, list) else [f]
-            selectCols = [_getFuncName(f) + '(' + x + ')' for x, funcs in funcDict.items() for f in
-                          funcs]  # if x not in self.__groupBys
-        elif isinstance(func, str):
-            selectCols = [_getFuncName(func) + '(' + x + ')' for x in selectCols]  # if x not in self.__groupBys
-        else:
-            raise RuntimeError(
-                'invalid func format, func: aggregate function name or a list of aggregate function names'
-                ' or a dict of column label/expression->func')
-        aggTable = copy.copy(self.__t)
-        aggTable._setSelect(selectCols)
-        aggTable.isMaterialized = False
-        return aggTable
-
-    def sum(self) -> "Table":
-        """Execute the aggregate function sum.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('sum')
-
-    def avg(self) -> "Table":
-        """Execute the aggregate function avg.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('avg')
-
-    def count(self) -> "Table":
-        """Execute the aggregate function count.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('count')
-
-    def max(self) -> "Table":
-        """Execute the aggregate function max.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('max')
-
-    def min(self) -> "Table":
-        """Execute the aggregate function min.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('min')
-
-    def first(self) -> "Table":
-        """Execute the aggregate function first.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('first')
-
-    def last(self) -> "Table":
-        """Execute the aggregate function last.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('last')
-
-    def size(self) -> "Table":
-        """Execute aggregate function size.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('size')
-
-    def sum2(self) -> "Table":
-        """Execute the aggregate function sum2.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('sum2')
-
-    def std(self) -> "Table":
-        """Execute aggregate function std.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('std')
-
-    def var(self) -> "Table":
-        """Execute aggregate function var.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('var')
-
-    def prod(self) -> "Table":
-        """Execute the aggregate function prod.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('prod')
-
-    def agg2(self, func, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Perform aggregate function(s) on specified column(s).
-
-        Args:
-            func : string or list of strings indicating the aggregate function(s).
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object.
-        """
-        if isinstance(cols, list) is False:
-            cols = [cols]
-        if isinstance(func, list) is False:
-            func = [func]
-        if np.sum([1 for x in cols if isinstance(x, tuple) is False or len(x) != 2]):
-            raise RuntimeError('agg2 only accepts (x,y) pair or a list of (x,y) pair as cols')
-        funcName = [_getFuncName(f) + '(' + x + ',' + y + ')' for f in func for x, y in cols]
-        selects = funcName if funcName else self.__t._getSelect()
-        agg2Table = copy.copy(self.__t)
-        agg2Table._setSelect(selects)
-        agg2Table.isMaterialized = False
-        return agg2Table
-
-    def wavg(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Perform aggregate function wavg on specified column(s).
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object.
-        """
-        return self.agg2('wavg', cols)
-
-    def wsum(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Perform aggregate function wsum on specified column(s).
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object.
-        """
-        return self.agg2('wsum', cols)
-
-    def covar(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Perform aggregate function covar on specified column(s).
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object.
-        """
-        return self.agg2('covar', cols)
-
-    def corr(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Perform aggregate function corr on specified column(s).
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object.
-        """
-        return self.agg2('corr', cols)
-
-    def toDF(self) -> DataFrame:
-        """Execute SQL statement and return a DataFrame object.
-
-        Returns:
-            data queried by SQL in DataFrame form.
-        """
-        query = self.showSQL()
-        # print(query)
-        df = self.__t.session().run(query)  # type: DataFrame
-        return df
-
-
-class TableContextby(object):
-    """The table object to add the context by clause.
-
-    Args:
-        t : Table object to add the context by clause.
-        contextBys : names of columns to be grouped for aggregation.
-        having : the content contained in a having clause. Defaults to None.
-    """
-    def __init__(self, t: "Table", contextBys: Union[str, List[str]], having: str = None):
-        """Constructor of TableContextby."""
-        if isinstance(contextBys, list):
-            self.__contextBys = contextBys
-        else:
-            self.__contextBys = [contextBys]
-        self.__t = t  # type: Table
-        self.__having = having
-        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
-
-    def sort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: bool = True) -> "TableContextby":
-        """Specify parameter for sorting.
-
-        Args:
-            bys : the column(s) to sort on.
-            ascending : the sorting order. True: ascending order. Defaults to True.
-
-        Returns:
-            a TableContextby object after adding sort clause.
-        """
-        sortTable = copy.copy(self.__t)
-        sortTable._setSort(bys, ascending)
-        return TableContextby(sortTable, self.__contextBys)
-
-    def csort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True) -> "TableContextby":
-        """Specify sorting column(s) for contextby.
-
-        Args:
-            bys : the column(s) to sort on.
-            ascending : the sorting order. True: ascending order. Defaults to True.
-
-        Returns:
-            a TableContextby object after adding csort clause.
-        """
-        csortTable = copy.copy(self.__t)
-        csortTable._setCsort(bys, ascending)
-        return TableContextby(csortTable, self.__contextBys)
-
-    def having(self, expr: str) -> "Table":
-        """Set having clause.
-
-        Args:
-            expr : expression for the having clause.
-
-        Returns:
-            a new Table object after adding the having clause.
-        """
-        havingTable = copy.copy(self.__t)
-        self.__having = expr
-        havingTable._setHaving(self.__having)
-        return havingTable
-
-    def __getitem__(self, item):
-        selectTable = self.__t.select(item)
-        return TableContextby(selectTable, contextBys=self.__contextBys)
-
-    def __iter__(self):
-        self.__contextBysIdx = 0
-        return self
-
-    def next(self) -> str:
-        """Get the name of the next grouping column for context by.
-
-        Returns:
-            column name.
-        """
-        try:
-            result = self.__contextBys[self.__contextBysIdx]
-        except IndexError:
-            raise StopIteration
-        self.__contextBysIdx += 1
-        return result
-
-    def __next__(self):
-        return self.next()
-
-    def selectAsVector(self, colName: str) -> np.array:
-        """Execute query and return the specified column.
-
-        Args:
-            colName : a string indicating the column name.
-
-        Returns:
-            data queried by SQL in numpy.array form.
-        """
-        if colName:
-            self.__t._setSelect(colName)
-        pattern = re.compile("select", re.IGNORECASE)
-        query = pattern.sub('exec', self.showSQL())
-        return self.__t.session().run(query)
-
-    def top(self, num: int) -> "Table":
-        """Set the top clause to retrieve the first n records from a Table.
-
-        Args:
-            num : the number of records to return. Must be a positive number.
-
-        Returns:
-            a Table object with the top clause.
-        """
-        return self.__t.top(num=num)
-
-    def limit(self, num: Union[int, Tuple[int, ...], List[int]]) -> "Table":
-        """Specify parameters for limit.
-
-        Args:
-            num : when used with the contextby clause, the limit clause can use a negative integer to select a limited number of records in the end of each group. 
-                  In all other cases the limit clause can only use positive integers.
-                  Can pass in [x, y] to select data from row x to row y.
-
-        Returns:
-            a Table object after adding the limit clause.
-        """
-        return self.__t.limit(num=num)
-
-    def executeAs(self, newTableName: str) -> "Table":
-        """Save execution result as an in-memory table with a specified name.
-
-        Args:
-            newTableName : new table name.
-
-        Returns:
-            a new Table object saved with the new table name.
-        """
-        st = newTableName + "=" + self.showSQL()
-        # print(st)
-        self.__t.session().run(st)
-        return Table(data=newTableName, s=self.__t.session())
-
-    def showSQL(self) -> str:
-        """View SQL query.
-
-        Returns:
-            the SQL query for the current Table.
-        """
-        return self.__t.showSQL()
-
-    def agg(self, func) -> "Table":
-        """Apply context by on all columns except the grouping columns.
-
-        Args:
-            func : string or list of strings indicating the aggregate function(s).
-
-        Returns:
-            a Table object after aggregation.
-        """
-        selectCols = self.__t._getSelect()
-        if isinstance(func, list):
-            selectCols = [_getFuncName(f) + '(' + x + ')' for x in selectCols for f in func if
-                          x not in self.__contextBys]
-        elif isinstance(func, dict):
-            funcDict = {}
-            for colName, f in func.items():
-                funcDict[colName] = f if isinstance(f, list) else [f]
-            selectCols = [_getFuncName(f) + '(' + x + ')' for x, funcs in funcDict.items() for f in funcs if
-                          x not in self.__contextBys]
-        elif isinstance(func, str):
-            selectCols = [_getFuncName(func) + '(' + x + ')' for x in selectCols if x not in self.__contextBys]
-        else:
-            raise RuntimeError(
-                'invalid func format, func: aggregate function name or a list of aggregate function names'
-                ' or a dict of column label/expression->func')
-        columns = self.__contextBys[:]
-        columns.extend(selectCols)
-        aggTable = copy.copy(self.__t)
-        aggTable._setSelect(columns)
-        aggTable.isMaterialized = False
-        return aggTable
-
-    def agg2(self, func, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Perform aggregate function(s) on specified column(s).
-
-        Args:
-            func : string or list of strings indicating the aggregate function(s).
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object.
-        """
-        if isinstance(cols, list) is False:
-            cols = [cols]
-        if isinstance(func, list) is False:
-            func = [func]
-        if np.sum([1 for x in cols if isinstance(x, tuple) is False or len(x) != 2]):
-            raise RuntimeError('agg2 only accepts (x,y) pair or a list of (x,y) pair as cols')
-        funcName = [_getFuncName(f) + '(' + x + ',' + y + ')' for f in func for x, y in cols]
-        selects = self.__t._getSelect()
-        if funcName:
-            selects.extend(funcName)
-        agg2Table = copy.copy(self.__t)
-        agg2Table._setSelect(selects)
-        agg2Table.isMaterialized = False
-        return agg2Table
-
-    def update(self, cols: List[str], vals: List[str]) -> "TableUpdate":
-        """Update in-memory table. Must be called to be executed.
-
-        Args:
-            cols : list of names of columns to be updated.
-            vals : a list of values to be updated.
-
-        Returns:
-            a TableUpdate object.
-        """
-        updateTable = TableUpdate(t=self.__t, cols=cols, vals=vals, contextby=self.__contextBys, having=self.__having)
-        return updateTable
-
-    def sum(self) -> "Table":
-        """Execute the aggregate function sum.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('sum')
-
-    def avg(self) -> "Table":
-        """Execute the aggregate function avg.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('avg')
-
-    def count(self) -> "Table":
-        """Execute the aggregate function count.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('count')
-
-    def max(self) -> "Table":
-        """Execute the aggregate function max.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('max')
-
-    def min(self) -> "Table":
-        """Execute the aggregate function min.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('min')
-
-    def first(self) -> "Table":
-        """Execute the aggregate function first.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('first')
-
-    def last(self) -> "Table":
-        """Execute the aggregate function last.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('last')
-
-    def size(self) -> "Table":
-        """Execute aggregate function size.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('size')
-
-    def sum2(self) -> "Table":
-        """Execute the aggregate function sum2.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('sum2')
-
-    def std(self) -> "Table":
-        """Execute aggregate function std.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('std')
-
-    def var(self) -> "Table":
-        """Execute aggregate function var.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('var')
-
-    def prod(self) -> "Table":
-        """Execute the aggregate function prod.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('prod')
-
-    def cumsum(self) -> "Table":
-        """Execute the aggregate function cumsum.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('cumsum')
-
-    def cummax(self) -> "Table":
-        """Execute the aggregate function cummax.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('cummax')
-
-    def cumprod(self) -> "Table":
-        """Execute the aggregate function cumprod.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('cumprod')
-
-    def cummin(self) -> "Table":
-        """Execute the aggregate function cummin.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg('cummin')
-
-    def wavg(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Execute aggregate function wavg.
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg2('wavg', cols)
-
-    def wsum(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Execute the aggregate function wsum.
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg2('wsum', cols)
-
-    def covar(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Execute the aggregate function covar.
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg2('covar', cols)
-
-    def corr(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Execute the aggregate function corr.
-
-        Args:
-            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg2('corr', cols)
-
-    def eachPre(self, args: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
-        """Execute the aggregate function eachPre.
-
-        Reference link: https://dolphindb.com/help/Functionalprogramming/TemplateFunctions/eachPre.html.
-
-        Args:
-            args : the function and parameters of eachPre.
-
-        Note:
-            args [0]: the function. args [1]: a vector, matrix or table. Apply args [0] over all pairs of consecutive elements of args [1].
-
-        Returns:
-            a Table object after aggregation.
-        """
-        return self.agg2('eachPre', args)
-
-    def toDF(self) -> DataFrame:
-        """Execute the SQL statement and return a DataFrame object.
-
-        Returns:
-            data queried by SQL in DataFrame form.
-        """
-        query = self.showSQL()
-        # print(query)
-        df = self.__t.session().run(query)  # type : DataFrame
-        return df
-
-
-wavg = TableGroupby.wavg
-wsum = TableGroupby.wsum
-covar = TableGroupby.covar
-corr = TableGroupby.corr
-count = TableGroupby.count
-max = TableGroupby.max
-min = TableGroupby.min
-sum = TableGroupby.sum
-sum2 = TableGroupby.sum2
-size = TableGroupby.size
-avg = TableGroupby.avg
-std = TableGroupby.std
-prod = TableGroupby.prod
-var = TableGroupby.var
-first = TableGroupby.first
-last = TableGroupby.last
-eachPre = TableContextby.eachPre
-cumsum = TableContextby.cumsum
-cumprod = TableContextby.cumprod
-cummax = TableContextby.cummax
-cummin = TableContextby.cummin
+import copy
+import inspect
+import re
+import threading
+from typing import Any, List, Optional, Tuple, Type, Union
+
+import numpy as np
+from dolphindb.settings import get_verbose
+from dolphindb.utils import _generate_tablename, _getFuncName, _isVariableCandidate
+from dolphindb.vector import FilterCond, Vector
+from pandas import DataFrame
+
+
+class Counter(object):
+    """Reference counter for internal use when caching table."""
+    def __init__(self):
+        """Constructor of Counter."""
+        self.__lock = threading.Lock()
+        self.__value = 1
+
+    def inc(self) -> int:
+        """Increment the reference count.
+
+        Returns:
+            current reference count.
+        """
+        with self.__lock:
+            self.__value += 1
+            return self.__value
+
+    def dec(self) -> int:
+        """Decrease the reference count.
+
+        Returns:
+            current reference count.
+        """
+        with self.__lock:
+            self.__value -= 1
+            return self.__value
+
+    def val(self) -> int:
+        """Get the current reference count.
+
+        Returns:
+            current reference count.
+        """
+        with self.__lock:
+            return self.__value
+
+
+class Table(object):
+    """DolphinDB Table object.
+
+    Args:
+        dbPath : database name. Defaults to None.
+        data : data of the table. Defaults to None.
+        tableAliasName : table alias. Defaults to None.
+        partitions : the partitions to be loaded into memory. Defaults to None, which means to load all partitions.
+        inMem : (deprecated) whether to load the table into memory. True: to load the table into memory. Defaults to False.
+        schemaInited : whether the table structure has been initialized. True: the table structure has been initialized. Defaults to False.
+        s : the connected Session object. Defaults to None.
+        needGC : whether to enable garbage collection. True: enable garbage collection. Defaults to True.
+        isMaterialized : whether table is materialized True: table has been materialized. Defaults to False.
+    """
+    def __init__(
+        self,
+        dbPath: str = None,
+        data=None,
+        tableAliasName: str = None,
+        partitions: Optional[List[str]] = None,
+        inMem: bool = False,
+        schemaInited: bool = False,
+        s=None,
+        needGC: bool = True,
+        isMaterialized: bool = False
+    ):
+        """Constructor of Table."""
+        if partitions is None:
+            partitions = []
+        self.__having = None
+        self.__top = None
+        self.__exec = False
+        self.__limit = None
+        self.__leftTable = None
+        self.__rightTable = None
+        self.__merge_for_update = False
+        self.__objAddr = None
+        self.__columns = None
+        self.isMaterialized = isMaterialized
+        if tableAliasName is not None:
+            self.isMaterialized = True
+        if s is None:
+            raise RuntimeError("Session must be provided")
+        self.__tableName = _generate_tablename() if not isinstance(data, str) else data
+        self.__session = s  # type : Session
+        self.__schemaInited = schemaInited
+        self.__need_gc = needGC
+        if self.__need_gc:
+            self.__ref = Counter()
+        if not isinstance(partitions, list):
+            raise RuntimeError(
+                'Column names must be passed in as a list')
+        if isinstance(data, dict) or isinstance(data, DataFrame):
+            df = data if isinstance(data, DataFrame) else DataFrame(data)
+            # if  not self.__tableName.startswith("TMP_TBL_"):
+            #    self._setTableName(_generate_tablename())
+            if tableAliasName is None:
+                self._setTableName(_generate_tablename())
+            else:
+                self._setTableName(tableAliasName)
+            self.__objAddr = self.__session.upload({self.__tableName: df})
+            self.vecs = {}
+
+            for colName in df.keys():
+                self.vecs[colName] = Vector(
+                    name=colName, tableName=self.__tableName, s=self.__session
+                )
+            select_list = list(self.vecs.keys())
+            select_list = [colName if _isVariableCandidate(colName) else f'_"{colName}"' for colName in select_list]
+            self._setSelect(select_list)
+        elif isinstance(data, str):
+            if dbPath:
+                if tableAliasName:
+                    self.__tableName = tableAliasName
+                else:
+                    self.__tableName = _generate_tablename(data)
+                runstr = '{tableName} = loadTable("{dbPath}", "{data}", {partitions}, {inMem})'
+                fmtDict = dict()
+                fmtDict['tableName'] = self.__tableName
+                fmtDict['dbPath'] = dbPath
+                fmtDict['data'] = data
+                if len(partitions) and type(partitions[0]) is not str:
+                    fmtDict['partitions'] = ('[' + ','.join(str(x) for x in partitions) + ']') if len(partitions) else ""
+                else:
+                    fmtDict['partitions'] = ('["' + '","'.join(partitions) + '"]') if len(partitions) else ""
+                fmtDict['inMem'] = str(inMem).lower()
+                runstr = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
+                self.__session.run(runstr)
+                # runstr = '%s = select * from %s' %(self.__tableName, self.__tableName)
+                # self.__session.run(runstr)
+            else:
+                pass
+        elif "orca.core.frame.DataFrame" in str(data.__class__):
+            df = s.run(data._var_name)
+            self.__init__(data=df, s=self.__session)
+        else:
+            raise RuntimeError("data must be a remote dolphindb table name or dict or DataFrame")
+        self._init_schema()
+
+    def __deepcopy__(self, memodict=None):
+        if memodict is None:
+            memodict = {}
+        newTable = Table(data=self.__tableName, schemaInited=True, s=self.__session, needGC=self.__need_gc)
+        newTable._setExec(self.isExec)
+        newTable.isMaterialized = self.isMaterialized
+        try:
+            newTable.vecs = copy.deepcopy(self.vecs, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__schemaInited = copy.deepcopy(self.__schemaInited, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__select = copy.deepcopy(self.__select, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__where = copy.deepcopy(self.__where, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__groupby = copy.deepcopy(self.__groupby, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__contextby = copy.deepcopy(self.__contextby, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__having = copy.deepcopy(self.__having, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__sort = copy.deepcopy(self.__sort, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__top = copy.deepcopy(self.__top, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__limit = copy.deepcopy(self.__limit, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__csort = copy.deepcopy(self.__csort, memodict)
+        except AttributeError:
+            pass
+
+        try:
+            if self.__need_gc:
+                newTable.__ref = self.__ref
+                self.__ref.inc()
+        except AttributeError:
+            pass
+
+        return newTable
+
+    def __copy__(self):
+        newTable = Table(data=self.__tableName, schemaInited=True, s=self.__session, needGC=self.__need_gc)
+        newTable._setExec(self.isExec)
+        newTable.isMaterialized = self.isMaterialized
+        try:
+            newTable.vecs = copy.copy(self.vecs)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__schemaInited = copy.copy(self.__schemaInited)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__select = copy.copy(self.__select)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__where = copy.copy(self.__where)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__groupby = copy.copy(self.__groupby)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__contextby = copy.copy(self.__contextby)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__having = copy.copy(self.__having)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__sort = copy.copy(self.__sort)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__top = copy.copy(self.__top)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__limit = copy.copy(self.__limit)
+        except AttributeError:
+            pass
+
+        try:
+            newTable.__csort = copy.copy(self.__csort)
+        except AttributeError:
+            pass
+
+        try:
+            if self.__need_gc:
+                newTable.__ref = self.__ref
+                self.__ref.inc()
+                # print("in copy ", self.__tableName, self.__ref.val())
+        except AttributeError:
+            pass
+
+        return newTable
+
+    def __del__(self):
+        # print("try to del ", self.__tableName, self.__ref.val())
+        if self.__need_gc:
+            if self.__ref.dec() == 0:
+                # print('do __del__', self.__tableName)
+                try:
+                    # this is not a real table name such as join table, no need to undef.
+                    if '(' in self.__tableName or ')' in self.__tableName:
+                        return
+                    # if self.__objAddr is None or self.__objAddr < 0:
+                    #     self.__session.run("undef('{}')".format(self.__tableName))
+                    # else:
+                    #     self.__session.run("undef('{}', VAR, {})".format(self.__tableName, self.__objAddr))
+                    if not self.__session.isClosed():
+                        if self.__tableName.find("TMP_TBL_") != -1:
+                            # print("undef ", self.__tableName)
+                            # tmp table, need to undef
+                            if self.__objAddr is None or self.__objAddr < 0:
+                                self.__session.run("undef('{}')".format(self.__tableName))
+                            else:
+                                self.__session.run("undef('{}', VAR)".format(self.__tableName))
+                except Exception as e:
+                    if get_verbose():
+                        print("undef table '{}' got an exception: ".format(self.__tableName))
+                        print(e)
+            # else:
+            #     print('__del__', self.__ref.val())
+
+    def _setSelect(self, cols):
+        self.__schemaInited = True
+        if isinstance(cols, tuple):
+            cols = list(cols)
+        if isinstance(cols, list) is False:
+            cols = [cols]
+
+        self.__select = cols
+
+    def _init_schema(self):
+        if self.__schemaInited is True:
+            return
+        self._init_columns()
+        self.vecs = {}
+        if self.__columns is not None:
+            if isinstance(self.__columns, list):
+                for colName in self.__columns:
+                    self.vecs[colName] = Vector(name=colName, tableName=self.__tableName, s=self.__session)
+                self._setSelect(self.__columns)
+            else:
+                self._setSelect(self.__columns)
+
+    def __getattr__(self, item):
+        vecs = object.__getattribute__(self, "vecs")
+        if item not in vecs:
+            return object.__getattribute__(self, item)
+        else:
+            return vecs[item]
+
+    def __getitem__(self, colOrCond):
+        if isinstance(colOrCond, FilterCond):
+            return self.where(colOrCond)
+        else:
+            return self.select(colOrCond)
+
+    def tableName(self) -> str:
+        """Get table name.
+
+        Returns:
+            name of the table in DolphinDB.
+        """
+        return self.__tableName
+
+    def _setTableName(self, tableName):
+        self.__tableName = tableName
+
+    def _getTableName(self):
+        return self.__tableName
+
+    def _setLeftTable(self, tableName):
+        self.__leftTable = tableName
+
+    def _setRightTable(self, tableName):
+        self.__rightTable = tableName
+
+    def getLeftTable(self) -> "Table":
+        """Get the left table of the join.
+
+        Returns:
+            the left table of the join.
+        """
+        return self.__leftTable
+
+    def getRightTable(self) -> "Table":
+        """Get the right table of the join.
+
+        Returns:
+            the right table of the join.
+        """
+        return self.__rightTable
+
+    def session(self):
+        """Get the Session where the Table belongs to.
+
+        Returns:
+            a Session where this Table belongs to.
+        """
+        return self.__session
+
+    def _addWhereCond(self, conds):
+        try:
+            _ = self.__where
+        except AttributeError:
+            self.__where = []
+
+        if isinstance(conds, list) or isinstance(conds, tuple):
+            self.__where.extend([str(x) for x in conds])
+        else:
+            self.__where.append(str(conds))
+
+    def _setSort(self, bys, ascending=True):
+        if isinstance(bys, list) or isinstance(bys, tuple):
+            self.__sort = [str(x) for x in bys]
+        else:
+            self.__sort = [str(bys)]
+        if isinstance(ascending, bool):
+            if not ascending:
+                self.__sort = [x + " desc" for x in self.__sort]
+            return
+        if (isinstance(ascending, list) or isinstance(ascending, tuple)) and (len(self.__sort) != len(ascending)):
+            raise ValueError(f"Length of ascending ({len(ascending)}) != length of by ({len(self.__sort)})")
+        self.__sort = [by + " desc" if not asc else by for by, asc in zip(self.__sort, ascending)]
+
+    def _setTop(self, num):
+        self.__top = str(num)
+
+    def _setCsort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True):
+        if isinstance(bys, list) or isinstance(bys, tuple):
+            self.__csort = [str(x) for x in bys]
+        else:
+            self.__csort = [str(bys)]
+        if isinstance(ascending, bool):
+            if not ascending:
+                self.__csort = [x + " desc" for x in self.__csort]
+            return
+        if (isinstance(ascending, list) or isinstance(ascending, tuple)) and (len(self.__csort) != len(ascending)):
+            raise ValueError(f"Length of ascending ({len(ascending)}) != length of by ({len(self.__csort)})")
+        self.__csort = [by + " desc" if not asc else by for by, asc in zip(self.__csort, ascending)]
+
+    def _setLimit(self, num):
+        if isinstance(num, list) or isinstance(num, tuple):
+            self.__limit = [str(x) for x in num]
+        else:
+            self.__limit = [str(num)]
+
+    def _setWhere(self, where):
+        self.__where = where
+
+    def select(self, cols: Union[str, Tuple[str, ...], List[str]]) -> "Table":
+        """Extract the specified columns and return them in a table.
+
+        Args:
+            cols : specify the columns to be extracted from table. Can be a string, a tuple of strings or a list of strings.
+
+        Returns:
+            a new Table object with the specified columns.
+        """
+        selectTable = copy.copy(self)
+        # print("ref of newTable: ", selectTable.__ref.val(), " self.ref: ", self.__ref.val())
+        selectTable._setSelect(cols)
+        if not self.isMaterialized:
+            selectTable.__tableName = f"({self.showSQL()})"
+        selectTable.isMaterialized = False
+        return selectTable
+
+    def exec(self, cols: Union[str, Tuple[str, ...], List[str]]) -> "Table":
+        """Generate a Table object containing the specified columns. The execution result is a scalar or vector.
+
+        Args:
+            cols : specify the columns. Can be a string, a tuple of strings or a list of strings.
+
+        Returns:
+            a new Table object of the specified columns.
+        """
+        selectTable = copy.copy(self)
+        selectTable._setSelect(cols)
+        selectTable._setExec(True)
+        if not self.isMaterialized:
+            selectTable.__tableName = f"({self.showSQL()})"
+        selectTable.isMaterialized = False
+        return selectTable
+
+    def where(self, conds) -> "Table":
+        """Add query conditions.
+
+        Args:
+            conds : query conditions.
+
+        Returns:
+            a new Table object with query conditions
+        """
+        # print("where", self.__tableName, __name__, conds)
+        whereTable = copy.copy(self)
+        whereTable._addWhereCond(conds)
+        return whereTable
+
+    def _setGroupby(self, groupby):
+        try:
+            _ = self.__contextby
+            raise RuntimeError('multiple context/group-by are not allowed ')
+        except AttributeError:
+            self.__groupby = groupby
+
+    def _setContextby(self, contextby):
+        try:
+            _ = self.__groupby
+            raise RuntimeError('multiple context/group-by are not allowed ')
+        except AttributeError:
+            self.__contextby = contextby
+
+    def _setHaving(self, having):
+        self.__having = having
+
+    def groupby(self, cols: Union[str, Tuple[str, ...], List[str]]) -> "TableGroupby":
+        """Apply group by on Table with specified columns.
+
+        Args:
+            cols : name of the grouping columns.
+
+        Returns:
+            a new TableGroupby object after adding the groupby.
+        """
+        groupbyTable = copy.copy(self)
+        groupby = TableGroupby(groupbyTable, cols)
+        groupbyTable._setGroupby(groupby)
+        return groupby
+
+    def sort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending=True) -> "Table":
+        """Specify parameter for sorting.
+
+        Args:
+            bys : the column(s) to sort on.
+            ascending : the sorting order. True: ascending order. Defaults to True.
+
+        Returns:
+            a new Table object after adding sort clause.
+        """
+        sortTable = copy.copy(self)
+        sortTable._setSort(bys, ascending)
+        return sortTable
+
+    def top(self, num: int) -> "Table":
+        """Retrieve the top n records from table.
+
+        Args:
+            num : the number of records to return. Must be a positive number.
+
+        Returns:
+            a new Table object with the top clause.
+        """
+        topTable = copy.copy(self)
+        topTable._setTop(num)
+        return topTable
+
+    def csort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True) -> "Table":
+        """Specify sorting column(s) for contextby.
+
+        Args:
+            bys : the column(s) to sort on.
+            ascending : the sorting order. True: ascending order. Defaults to True.
+
+        Returns:
+            a new Table object after adding csort clause.
+        """
+        csortTable = copy.copy(self)
+        csortTable._setCsort(bys, ascending)
+        return csortTable
+
+    def limit(self, num: Union[int, Tuple[int, ...], List[int]]) -> "Table":
+        """Specify parameters for limit.
+
+        Args:
+            num : when used with the contextby clause, the limit clause can use a negative integer to select a limited number of records in the end of each group. 
+                  In all other cases the limit clause can only use positive integers.
+                  Can pass in [x, y] to select data from row x to row y.
+
+        Returns:
+            a new Table object after adding the limit clause
+        """
+        limitTable = copy.copy(self)
+        limitTable._setLimit(num)
+        return limitTable
+
+    def execute(self, expr: Union[str, Tuple[str, ...], List[str]]) -> Any:
+        """Execute the SQL query.
+
+        Args:
+            expr : columns to be executed. Can be a string, tuple, or list.
+
+        Returns:
+            SQL query result.
+        """
+        if expr:
+            self._setSelect(expr)
+        pattern = re.compile("select", re.IGNORECASE)
+        query = pattern.sub('exec', self.showSQL())
+        return self.__session.run(query)
+
+    @property
+    def rows(self) -> int:
+        """Read-only property.
+
+        Get the row count of the Table.
+
+        Returns:
+            number of rows in the Table.
+        """
+        # if 'update' in self.showSQL().lower() or 'insert' in  self.showSQL().lower():
+        #     return self.__session.run('exec count(*) from %s'% self.__tableName)
+        sql = self.showSQL()
+        idx = sql.lower().index("from")
+        sql_new = "select count(*) as ct " + sql[idx:]
+        df = self.__session.run(sql_new)
+        if df.shape[0] > 1:
+            return df.shape[0]
+        else:
+            return df['ct'].iloc[0]
+
+    def _init_columns(self) -> None:
+        if not self.__columns:
+            schema = self.__session.run("schema(%s)" % self.__tableName)  # type: dict
+            columns = schema["colDefs"]["name"].tolist()
+            columns = [colName if _isVariableCandidate(colName) else f'_"{colName}"' for colName in columns]
+            self.__columns = columns
+
+    @property
+    def cols(self) -> int:
+        """read-only property.
+
+        Get the number of columns in the Table.
+
+        Returns:
+            the number of columns in the Table.
+        """
+        self._init_columns()
+        return len(self.__columns)
+
+    @property
+    def colNames(self) -> List[str]:
+        """read-only property.
+
+        Get all column names of the Table.
+
+        Returns:
+            all column names of the Table.
+        """
+        self._init_columns()
+        return [
+            col[2:-1] if len(col) >= 3 and col[0:2] == '_"' and col[-1] == '"' else col
+            for col in self.__columns
+        ]
+
+    @property
+    def schema(self) -> DataFrame:
+        """read-only property.
+
+        Get summary information of the Table.
+
+        Returns:
+            a DataFrame about summary information of the Table.
+        """
+        schema = self.__session.run("schema(%s)" % self.__tableName)  # type: dict
+        colDefs = schema.get('colDefs')  # type: DataFrame
+        return colDefs
+
+    @property
+    def isMergeForUpdate(self) -> bool:
+        """read-only property.
+
+        Decide whether the Table is to be joined.
+
+        Returns:
+            True means Table is to be joined.
+        """
+        return self.__merge_for_update
+
+    def setMergeForUpdate(self, toUpdate: bool):
+        """Mark if a Table is to be joined.
+
+        Args:
+            toUpdate : True means to mark the table as to be joined.
+        """
+        self.__merge_for_update = toUpdate
+
+    @property
+    def isExec(self) -> bool:
+        """read-only property.
+
+        Whether the SQL statement has an exec clause.
+
+        Returns:
+            True means the SQL statement has added an exec clause.
+        """
+        return self.__exec
+
+    def _setExec(self, isExec):
+        self.__exec = isExec
+
+    def pivotby(self, index: str, column: str, value=None, aggFunc=None) -> "TablePivotBy":
+        """Add pivot by clause to rearrange a column (or multiple columns) of a table on two dimensions.
+
+        Args:
+            index : the result table has the same number of rows as unique values on this column.
+            column : the result table has the same number of columns as unique values on this column.
+            value : the parameters of the aggregate function. Defaults to None.
+            aggFunc : the specified aggregate function. Defaults to lambda x: x.
+
+        Returns:
+            a TablePivotBy object.
+        """
+        pivotByTable = copy.copy(self)
+        return TablePivotBy(pivotByTable, index, column, value, aggFunc)
+
+    def merge(
+            self, right, how: str = 'inner', on: Union[str, Tuple[str, ...], List[str]] = None,
+            left_on: Union[str, Tuple[str, ...], List[str]] = None,
+            right_on: Union[str, Tuple[str, ...], List[str]] = None,
+            sort: bool = False, merge_for_update: bool = False
+    ) -> "Table":
+        """Join two table objects with ANSI SQL.
+
+        Args:
+            right : the right table from local or remote server.
+            how : connection type. The options are {"left", "right", "outer", "inner"}. Defaults to 'inner'.
+        | How   | Link                                                                 |
+        | :---- | :------------------------------------------------------------------- |
+        | left  | https://dolphindb.com/help/SQLStatements/TableJoiners/leftjoin.html  |
+        | right | https://dolphindb.com/help/SQLStatements/TableJoiners/leftjoin.html  |
+        | outer | https://dolphindb.com/help/SQLStatements/TableJoiners/fulljoin.html  |
+        | ineer | https://dolphindb.com/help/SQLStatements/TableJoiners/equaljoin.html |   
+            on : the columns to join on. If the column names are different in two tables, use the left_on and right_on parameters. Defaults to None.
+            left_on : the column to join on from the left table. Defaults to None.
+            right_on : the column to join on from the right table. Defaults to None.
+            sort : True means to enable sorting. Defaults to False.
+            merge_for_update : True means marking tables as to be joined. Defaults to False.
+
+        Note:
+            A partitioned table can only outer join a another partitioned table. An in-memory table can only outer join another in-memory table.
+
+        Returns:
+            the joined Table object.
+        """
+        howMap = {
+            'inner': 'ej',
+            'left': 'lj',
+            'right': 'lj',
+            'outer': 'fj',
+            'left semi': 'lsj'
+        }
+        joinFunc = howMap[how]
+        joinFuncPrefix = '' if sort is False or joinFunc == 'fj' else 's'
+
+        if self.isMaterialized or merge_for_update:
+            leftTableName = self.tableName()
+        else:
+            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
+
+        if right.isMaterialized:
+            rightTableName = right.tableName() if isinstance(right, Table) else right
+        else:
+            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
+
+        if how == 'right':
+            leftTableName, rightTableName = rightTableName, leftTableName
+            left_on, right_on = right_on, left_on
+
+        if on is not None and not isinstance(on, list) and not isinstance(on, tuple):
+            on = [on]
+        if left_on is not None and not isinstance(left_on, list) and not isinstance(left_on, tuple):
+            left_on = [left_on]
+        if right_on is not None and not isinstance(right_on, list) and not isinstance(right_on, tuple):
+            right_on = [right_on]
+
+        if on is not None:
+            left_on, right_on = on, on
+        elif left_on is None and right_on is None:
+            raise Exception('at least one of {\'on\', \'left_on\', \'right_on\'} must be present')
+        elif left_on is not None and right_on is not None and len(left_on) != len(right_on):
+            raise Exception('\'left_on\' must have the same length as \'right_on\'')
+
+        if left_on is None and right_on is not None:
+            left_on = right_on
+        if right_on is None and left_on is not None:
+            right_on = left_on
+
+        leftColumnNames = ''.join(['`' + x for x in left_on])
+        rightColumnNames = ''.join(['`' + x for x in right_on])
+        finalTableName = '%s(%s,%s,%s,%s)' % (
+            joinFuncPrefix + joinFunc, leftTableName, rightTableName, leftColumnNames, rightColumnNames
+        )
+        # print(finalTableName)
+        self._init_schema()
+        right._init_schema()
+        joinTable = copy.copy(self)
+        # leftAliasPrefix = 'lhs_' if how != 'right' else 'rhs_'
+        # rightAliasPrefix = 'rhs_' if how != 'right' else 'lhs_'
+        # leftSelectCols = [leftTableName + '.' + col + ' as ' + leftTableName + "_" + col for col in self._getSelect()]
+        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in right._getSelect()]
+        # leftSelectCols = self._getSelect()
+        # print(leftSelectCols)
+        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in
+        #                    right._getSelect() if col in self._getSelect()]
+        # print(rightSelectCols)
+        joinTable._setLeftTable(self.tableName())
+        joinTable._setRightTable(right.tableName())
+        joinTable._setTableName(finalTableName)
+        # joinTable._setSelect(leftSelectCols + rightSelectCols)
+        joinTable._setSelect('*')
+        if merge_for_update:
+            joinTable.setMergeForUpdate(True)
+        joinTable.isMaterialized = False
+        return joinTable
+
+    def merge_asof(
+        self, right, on: Union[str, Tuple[str, ...], List[str]] = None,
+        left_on: Union[str, Tuple[str, ...], List[str]] = None,
+        right_on: Union[str, Tuple[str, ...], List[str]] = None
+    ) -> "Table":
+        """Use asof join to join two Table objects.
+
+        Refer to https://dolphindb.com/help/SQLStatements/TableJoiners/asofjoin.html.
+
+        Args:
+            right : The right table from local or remote server.
+            on : the columns to join on. If the column names are different in two tables, use the left_on and right_on parameters. Defaults to None.
+            left_on : the column to join on from the left table. Defaults to None.
+            right_on : the column to join on from the right table. Defaults to None.
+
+        Returns:
+            the joined Table object.
+        """
+        if self.isMaterialized:
+            leftTableName = self.tableName()
+        else:
+            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
+
+        if right.isMaterialized:
+            rightTableName = right.tableName() if isinstance(right, Table) else right
+        else:
+            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
+
+        if on is not None and not isinstance(on, list) and not isinstance(on, tuple):
+            on = [on]
+        if left_on is not None and not isinstance(left_on, list) and not isinstance(left_on, tuple):
+            left_on = [left_on]
+        if right_on is not None and not isinstance(right_on, list) and not isinstance(right_on, tuple):
+            right_on = [right_on]
+
+        if on is not None:
+            left_on, right_on = on, on
+        elif left_on is None and right_on is None:
+            raise Exception('at least one of {\'on\', \'left_on\', \'right_on\'} must be present')
+        elif left_on is not None and right_on is not None and len(left_on) != len(right_on):
+            raise Exception('\'left_on\' must have the same length as \'right_on\'')
+
+        if left_on is None and right_on is not None:
+            left_on = right_on
+        if right_on is None and left_on is not None:
+            right_on = left_on
+
+        leftColumnNames = ''.join(['`' + x for x in left_on])
+        rightColumnNames = ''.join(['`' + x for x in right_on])
+        finalTableName = 'aj(%s,%s,%s,%s)' % (
+            leftTableName, rightTableName, leftColumnNames, rightColumnNames
+        )
+        self._init_schema()
+        right._init_schema()
+        joinTable = copy.copy(self)
+        # leftAliasPrefix = 'lhs_'
+        # rightAliasPrefix = 'rhs_'
+        # leftSelectCols = [leftTableName + '.' + col + ' as ' + leftTableName +"_" + col for col in self._getSelect()]
+        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in right._getSelect()]
+        # leftSelectCols = self._getSelect()
+        # rightSelectCols = [rightTableName + '.' + col + ' as ' + rightTableName + "_" + col for col in
+        #                    right._getSelect() if col in self._getSelect()]
+        joinTable._setLeftTable(self.tableName())
+        joinTable._setRightTable(right.tableName())
+        joinTable._setTableName(finalTableName)
+        joinTable._setSelect('*')
+        # joinTable._setSelect(leftSelectCols + rightSelectCols)
+        joinTable.isMaterialized = False
+        return joinTable
+
+    def merge_window(
+        self, right, leftBound: int, rightBound: int,
+        aggFunctions: Union[str, List[str]], on: Union[str, Tuple[str, ...], List[str]] = None,
+        left_on: Union[str, Tuple[str, ...], List[str]] = None,
+        right_on: Union[str, Tuple[str, ...], List[str]] = None,
+        prevailing: bool = False
+    ) -> "Table":
+        """Use window join to join two Table objects.
+
+        Args:
+            right : the name of the right table from local or remote server.
+            leftBound : left boundary (inclusive) of the window. Defaults to None.
+            rightBound : right boundary (inclusive) of the window. Defaults to None.
+            aggFunctions : aggregate function. Defaults to None.
+            on : the columns to join on. If the column names are different in two tables, use the left_on and right_on parameters. Defaults to None.
+            left_on : the column to join on from the left table. Defaults to None.
+            right_on : the column to join on from the right table. Defaults to None.
+            prevailing : whether to use prevailing window join. True: use prevailing window join. Defaults to False.
+
+        Returns:
+            the joined Table object.
+        """
+
+        if self.isMaterialized:
+            leftTableName = self.tableName()
+        else:
+            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
+
+        if right.isMaterialized:
+            rightTableName = right.tableName() if isinstance(right, Table) else right
+        else:
+            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
+
+        ifPrevailing = False
+
+        if prevailing is not None:
+            ifPrevailing = prevailing
+
+        if on is not None and not isinstance(on, list) and not isinstance(on, tuple):
+            on = [on]
+        if left_on is not None and not isinstance(left_on, list) and not isinstance(left_on, tuple):
+            left_on = [left_on]
+        if right_on is not None and not isinstance(right_on, list) and not isinstance(right_on, tuple):
+            right_on = [right_on]
+
+        if on is not None:
+            left_on, right_on = on, on
+        elif left_on is None and right_on is None:
+            raise Exception('at least one of {\'on\', \'left_on\', \'right_on\'} must be present')
+        elif left_on is not None and right_on is not None and len(left_on) != len(right_on):
+            raise Exception('\'left_on\' must have the same length as \'right_on\'')
+
+        if left_on is None and right_on is not None:
+            left_on = right_on
+        if right_on is None and left_on is not None:
+            right_on = left_on
+
+        leftColumnNames = ''.join(['`' + x for x in left_on])
+        rightColumnNames = ''.join(['`' + x for x in right_on])
+        if isinstance(aggFunctions, list):
+            aggFunctions = '[' + ','.join(aggFunctions) + ']'
+        if ifPrevailing:
+            finalTableName = 'pwj(%s,%s,%d:%d,%s,%s,%s)' % (
+                leftTableName, rightTableName, leftBound, rightBound,
+                '<' + aggFunctions + '>', leftColumnNames, rightColumnNames
+            )
+        else:
+            finalTableName = 'wj(%s,%s,%d:%d,%s,%s,%s)' % (
+                leftTableName, rightTableName, leftBound, rightBound, '<' + aggFunctions + '>', leftColumnNames,
+                rightColumnNames)
+        # print(finalTableName)
+        self._init_schema()
+        right._init_schema()
+        joinTable = copy.copy(self)
+        joinTable._setLeftTable(self.tableName())
+        joinTable._setRightTable(right.tableName())
+        joinTable._setTableName(finalTableName)
+        joinTable._setSelect('*')
+        return joinTable
+
+    def merge_cross(self, right) -> "Table":
+        """Perform a cross join with another table and return their Cartesian product.
+
+        Args:
+            right : the name of the right table from local or remote server.
+
+        Returns:
+            the joined Table object.
+        """
+        if self.isMaterialized:
+            leftTableName = self.tableName()
+        else:
+            leftTableName = f"({self.showSQL()}) as {_generate_tablename('TMP_L')}"
+
+        if right.isMaterialized:
+            rightTableName = right.tableName() if isinstance(right, Table) else right
+        else:
+            rightTableName = f"({right.showSQL()}) as {_generate_tablename('TMP_R')}"
+
+        finalTableName = 'cj(%s,%s)' % (leftTableName, rightTableName)
+        self._init_schema()
+        right._init_schema()
+        joinTable = copy.copy(self)
+        joinTable._setLeftTable(self.tableName())
+        joinTable._setRightTable(right.tableName())
+        joinTable._setTableName(finalTableName)
+        joinTable._setSelect("*")
+        return joinTable
+
+    def _getSelect(self):
+        return self.__select
+
+    def _assembleSelect(self):
+        try:
+            if len(self.__select) and isinstance(self.__select, list):
+                return ','.join(self.__select)
+            else:
+                return '*'
+        except AttributeError:
+            return '*'
+        except ValueError:
+            return '*'
+
+    def _assembleWhere(self):
+        try:
+            if len(self.__where) == 1:
+                return 'where ' + self.__where[0]
+            else:
+                return 'where ' + ' and '.join(["(" + x + ")" for x in self.__where])
+        except AttributeError:
+            return ''
+
+    def _assembleGroupbyOrContextby(self):
+        try:
+            return 'group by ' + ','.join(self.__groupby)
+        except AttributeError:
+            try:
+                return 'context by ' + ','.join(self.__contextby)
+            except AttributeError:
+                return ''
+
+    def _assembleOrderby(self):
+        try:
+            return 'order by ' + ','.join(self.__sort)
+        except AttributeError:
+            return ''
+
+    def _assembleCsort(self):
+        try:
+            return 'csort ' + ','.join(self.__csort)
+        except AttributeError:
+            return ''
+
+    def _assembleLimit(self):
+        try:
+            if (self.__limit is None):
+                return ''
+            if len(self.__limit) and isinstance(self.__limit, list):
+                return 'limit ' + ','.join(self.__limit)
+            else:
+                return self.__limit
+        except AttributeError:
+            return ''
+
+    def showSQL(self) -> str:
+        """View SQL query.
+
+        Returns:
+            the SQL query for the current Table.
+        """
+        import re
+        selectOrExec = "exec" if self.isExec else "select"
+        queryFmt = selectOrExec + ' {top} {select} from {table} {where} {groupby} {csort} {having} {orderby} {limit}'
+        fmtDict = {}
+        fmtDict['top'] = ("top " + self.__top) if self.__top else ''
+        fmtDict['select'] = self._assembleSelect()
+        fmtDict['table'] = self.tableName()
+        fmtDict['where'] = self._assembleWhere()
+        fmtDict['groupby'] = self._assembleGroupbyOrContextby()
+        fmtDict['csort'] = self._assembleCsort()
+        fmtDict['having'] = ("having " + self.__having) if self.__having else ''
+        fmtDict['orderby'] = self._assembleOrderby()
+        fmtDict['limit'] = self._assembleLimit()
+        query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
+        # print(query)
+        # if(self.__tableName.startswith("wj") or self.__tableName.startswith("pwj")):
+        #     return self.__tableName
+
+        if get_verbose():
+            print(query)
+        return query
+
+    def append(self, table: "Table") -> "Table":
+        """Append data to Table and execute at once.
+
+        Args:
+            table : Table object to be appended.
+
+        Returns:
+            the appended Table object.
+
+        Note:
+            The data in the DolphinDB server will be modified immediately.
+        """
+        if not isinstance(table, Table):
+            raise RuntimeError("Only DolphinDB Table object is accepted")
+
+        runstr = "%s.append!(%s)" % (self.tableName(), table.tableName())
+        self.__session.run(runstr)
+        return self
+
+    def update(self, cols: List[str], vals: List[str]) -> "TableUpdate":
+        """Update in-memory table. Must be called to be executed.
+
+        Args:
+            cols : list of names of columns to be updated.
+            vals : a list of values to be updated.
+
+        Returns:
+            a TableUpdate object.
+        """
+        # print("update for ", self.__tableName)
+        tmp = copy.copy(self)
+        if self.isMergeForUpdate:
+            tmp._setLeftTable(self.getLeftTable())
+        contextby = self.__contextby if hasattr(self, '__contextby') else None
+        having = self.__having if hasattr(self, '__having') else None
+        updateTable = TableUpdate(t=tmp, cols=cols, vals=vals, contextby=contextby, having=having)
+        updateTable._setMergeForUpdate(self.isMergeForUpdate)
+        return updateTable
+
+    def rename(self, newName: str) -> None:
+        """Rename table.
+
+        Args:
+            newName : new table name.
+        """
+        self.__session.run(newName + '=' + self.tableName())
+        self.__tableName = newName
+
+    def delete(self) -> "TableDelete":
+        """Delete table.
+
+        Returns:
+            a TableDelete object.
+        """
+        tmp = copy.copy(self)
+        delTable = TableDelete(t=tmp)
+        return delTable
+
+    def drop(self, cols: Union[List[str], str]) -> "Table":
+        """Delete columns.
+
+        Args:
+            cols : list of columns to be deleted.
+
+        Returns:
+            a Table object.
+        """
+        if isinstance(cols, str):
+            cols = [cols]
+        if not isinstance(cols, list):
+            raise TypeError("cols must be a str or a list of str.")
+        cols = [
+            col[2:-1] if len(col) >= 3 and col[0:2] == '_"' and col[-1] == '"' else col
+            for col in cols
+        ]
+        if len(cols) == 1:
+            query = f'{self.tableName()}.drop!("{str(cols[0])}")'
+        if len(cols) > 1:
+            runstr = '{table}.drop!([{cols}])'
+            fmtDict = dict()
+            fmtDict['table'] = self.tableName()
+            fmtDict['cols'] = '"' + '","'.join(cols) + '"'
+            query = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
+        if cols:
+            remove_list = []
+            for col in cols:
+                for colName in self.__select:
+                    col_o = colName[2:-1] if len(colName) >= 3 and colName[0:2] == '_"' and colName[-1] == '"' else colName
+                    if col.lower() == col_o.lower():
+                        remove_list.append(colName)
+            for colName in remove_list:
+                self.__select.remove(colName)
+            self.__session.run(query)
+        return self
+
+    def executeAs(self, newTableName: str) -> "Table":
+        """Save execution result as an in-memory table with a specified name.
+
+        Args:
+            newTableName : new table name.
+
+        Returns:
+            a new Table object saved with the new table name.
+        """
+        st = newTableName + "=(" + self.showSQL() + ")"
+        # print(st)
+        self.__session.run(st)
+        return Table(data=newTableName, s=self.__session)
+
+    def contextby(self, cols: Union[str, List[str]]) -> "TableContextby":
+        """Group by specified columns.
+
+        Args:
+            cols : name of the columns to context by.
+
+        Returns:
+            a TableContextby object after adding context by clause.
+        """
+        contextbyTable = copy.copy(self) # Table
+        contextbyTable.__merge_for_update = self.__merge_for_update
+        contextby = TableContextby(contextbyTable, cols)
+        contextbyTable._setContextby(contextby)
+        contextbyTable._setTableName(self.tableName())
+        return contextby
+
+    def ols(self, Y:str, X:Union[str, List[str]], INTERCEPT: bool = True) -> dict:
+        """Calculate Least Squares Regression Coefficients.
+
+        Refer to https://dolphindb.com/help/FunctionsandCommands/FunctionReferences/o/ols.html.
+
+        Args:
+            Y : dependent variable, column name.
+            X : argument, list of column names.
+            INTERCEPT : whether to include the intercept in the regression. Defaults to True, meaning that the system automatically adds a column of "1" to X to generate the intercept.
+
+        Returns:
+            a dictionary with ANOVA, RegressionStat, Cofficient and Residual.
+        """
+        myY = ""
+        myX = []
+
+        if isinstance(Y, str):
+            myY = Y
+        else:
+            raise ValueError("Y must be a column name")
+        if isinstance(X, str):
+            myX = [X]
+        elif isinstance(X, list):
+            myX = X
+        else:
+            raise ValueError("X must be a column name or a list of column names")
+        if not len(myY) or not len(myX):
+            raise ValueError("Invalid Input data")
+        schema = self.__session.run("schema(%s)" % self.__tableName)
+        if 'partitionColumnName' in schema and schema['partitionColumnName']:
+            dsstr = "sqlDS(<SQLSQL>)".replace('SQLSQL', self.showSQL()).replace('select select', 'select')
+            runstr = "olsEx({ds},{Y},{X},{INTERCEPT},2)"
+            fmtDict = dict()
+            fmtDict['table'] = self.tableName()
+            fmtDict['Y'] = '"' + myY + '"'
+            fmtDict['X'] = str(myX)
+            fmtDict['ds'] = dsstr
+            fmtDict['INTERCEPT'] = str(INTERCEPT).lower()
+            query = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
+            # print(query)
+            return self.__session.run(query)
+        else:
+            runstr = "z=exec ols({Y},{X},{INTERCEPT},2) from {table}"
+            fmtDict = dict()
+            fmtDict['table'] = self.tableName()
+            fmtDict['Y'] = myY
+            fmtDict['X'] = str(myX)
+            fmtDict['INTERCEPT'] = str(INTERCEPT).lower()
+            query = re.sub(' +', ' ', runstr.format(**fmtDict).strip())
+            # print(query)
+            return self.__session.run(query)
+
+    def toDF(self) -> DataFrame:
+        """Execute SQL statement and return a DataFrame object.
+
+        Returns:
+            data queried by SQL in DataFrame form.
+        """
+        self._init_schema()
+        query = self.showSQL()
+        df = self.__session.run(query)  # type: DataFrame
+        return df
+
+    def toList(self) -> list:
+        """Execute SQL statement and return a List object.
+
+        Returns:
+            list: the query result in the form of a list. The length of the list is same as the rows of the Table.
+
+        Note:
+            If the table contains columns of array vectors, the system will try to convert them to NumPy 2D arrays. 
+            The conversion will fail if the rows in the array vector are different.
+        """
+        self._init_schema()
+        query = self.showSQL()
+        list = self.__session.run(query, pickleTableToList=True)  # type: DataFrame
+        return list
+
+    toDataFrame = toDF
+
+
+class TableDelete(object):
+    """Table object to be deleted.
+
+    Args:
+        t : Table object to be deleted.
+    """
+    def __init__(self, t):
+        """Constructor of TableDelete."""
+        self.__t = t
+        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
+
+    def _assembleWhere(self):
+        try:
+            if len(self.__where) == 1:
+                return 'where ' + self.__where[0]
+            else:
+                return 'where ' + ' and '.join(["(" + x + ")" for x in self.__where])
+        except AttributeError:
+            return ''
+
+    def _addWhereCond(self, conds):
+        try:
+            _ = self.__where
+        except AttributeError:
+            self.__where = []
+
+        if isinstance(conds, list) or isinstance(conds, tuple):
+            self.__where.extend([str(x) for x in conds])
+        else:
+            self.__where.append(str(conds))
+
+    def where(self, conds) -> "TableDelete":
+        """Add query conditions.
+
+        Args:
+            conds : query conditions.
+
+        Returns:
+            a TableDelete object with query conditions.
+        """
+        # print("where", self.__t.__dict__["_Table__tableName"], __name__, conds)
+        self._addWhereCond(conds)
+        return self
+
+    def __executesql(self) -> str:
+        return self.showSQL()
+
+    def showSQL(self) -> str:
+        """View SQL query.
+
+        Returns:
+            the SQL statement for the current TableDelete object.
+        """
+        curframe = inspect.currentframe()
+        calframe = inspect.getouterframes(curframe, 2)
+        caller = calframe[1][3]
+        if caller != 'execute' and caller != 'print' and caller != "str" and caller != '<module>' and caller != '__executesql':
+            return self.__t.showSQL()
+        queryFmt = 'delete from {table} {where}'
+        fmtDict = {}
+        fmtDict['table'] = self.__t.tableName()
+        fmtDict['where'] = self._assembleWhere()
+        query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
+        return query
+
+    def execute(self) -> "Table":
+        """Execute the SQL query.
+
+        Returns:
+            Table: SQL query result as Table.
+        """
+        query = self.showSQL()
+        self.__t.session().run(query)
+        return self.__t
+
+    def toDF(self) -> DataFrame:
+        """Execute SQL statement and return a DataFrame object.
+
+        Returns:
+            data queried by SQL in DataFrame form.
+        """
+        query = self.showSQL()
+
+        df = self.__t.session().run(query)  # type: DataFrame
+
+        return df
+
+
+class TableUpdate(object):
+    """Table object to be updated.
+
+    Args:
+        t : Table object to be updated.
+        cols : list of names of columns to be updated.
+        vals : a list of values corresponding to the columns to be updated.
+        contextby : whether SQL query contains a contextby clause. True means there is. Defaults to None.
+        having : the content contained in a having clause. Defaults to None.
+    """
+    def __init__(self, t: "Table", cols: List[str], vals: List[str], contextby=None, having: str = None):
+        """Constructor of TableUpdate."""
+        self.__t = t
+        self.__cols = cols
+        self.__vals = vals
+        self.__contextby = contextby
+        self.__having = having
+        self.__merge_for_update = False
+        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
+
+    def _setMergeForUpdate(self, toMerge):
+        self.__merge_for_update = toMerge
+
+    def _assembleUpdate(self):
+        query = ""
+        for col, val in zip(self.__cols, self.__vals):
+            query += col + "=" + val + ","
+        return query[:-1]
+
+    def _assembleWhere(self):
+        try:
+            if len(self.__where) == 1:
+                return 'where ' + self.__where[0]
+            else:
+                return 'where ' + ' and '.join(["(" + x + ")" for x in self.__where])
+        except AttributeError:
+            return ''
+
+    def _addWhereCond(self, conds):
+        try:
+            _ = self.__where
+        except AttributeError:
+            self.__where = []
+
+        if isinstance(conds, list) or isinstance(conds, tuple):
+            self.__where.extend([str(x) for x in conds])
+        else:
+            self.__where.append(str(conds))
+
+    def where(self, conds) -> "TableUpdate":
+        """Add query conditions.
+
+        Args:
+            conds : query conditions.
+
+        Returns:
+            a TableUpdate object with query conditions.
+        """
+        # print("where", self.__t.__dict__["_Table__tableName"], __name__, conds)
+        self._addWhereCond(conds)
+        return self
+
+    def __executesql(self) -> str:
+        return self.showSQL()
+
+    def showSQL(self) -> str:
+        """View SQL query.
+
+        Returns:
+            the SQL statement for the current TableUpdate object.
+        """
+        curframe = inspect.currentframe()
+        calframe = inspect.getouterframes(curframe, 2)
+        caller = calframe[1][3]
+        if caller != 'execute' and caller != 'print' and caller != "str" and caller != '<module>' and caller != '__executesql':
+            return self.__t.showSQL()
+        if not self.__merge_for_update:
+            queryFmt = 'update {table} set {update} {where} {contextby} {having}'
+            fmtDict = {}
+            fmtDict['update'] = self._assembleUpdate()
+            fmtDict['table'] = self.__t.tableName()
+            fmtDict['where'] = self._assembleWhere()
+            if self.__contextby:
+                fmtDict['contextby'] = 'context by ' + ','.join(self.__contextby)
+            else:
+                fmtDict['contextby'] = ""
+            if self.__having:
+                fmtDict['having'] = ' having ' + self.__having
+            else:
+                fmtDict['having'] = ""
+            query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
+            if get_verbose():
+                print(query)
+            return query
+        else:
+            if self.__t.getLeftTable() is None:
+                raise Exception("Join for update missing left table!")
+            queryFmt = 'update {table} set {update} from {joinTable} {where} {contextby} {having}'
+            fmtDict = {}
+            fmtDict['update'] = self._assembleUpdate()
+            fmtDict['table'] = self.__t.getLeftTable()
+            fmtDict['joinTable'] = self.__t.tableName()
+            fmtDict['where'] = self.__t._assembleWhere()
+            if self.__contextby:
+                fmtDict['contextby'] = 'context by ' + ','.join(self.__t.__contextby)
+            else:
+                fmtDict['contextby'] = ""
+            if self.__having:
+                fmtDict['having'] = ' having ' + self.__having
+            else:
+                fmtDict['having'] = ""
+            query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
+            self.__t.setMergeForUpdate(False)
+            if get_verbose():
+                print(query)
+            return query
+
+    def execute(self) -> "Table":
+        """Execute the SQL query.
+
+        Returns:
+            SQL query result as Table.
+        """
+        query = self.showSQL()
+        # print(query)
+        self.__t.session().run(query)
+        t = Table(data=self.__t.tableName(), s=self.__t.session(), needGC=self.__t.__dict__["_Table__need_gc"])
+        if self.__t.__dict__["_Table__need_gc"]:
+            t.__dict__["_Table__ref"] = self.__t.__dict__["_Table__ref"]
+            t.__dict__["_Table__ref"].inc()
+        return t
+
+    def toDF(self) -> DataFrame:
+        """Execute SQL statement and return a DataFrame object.
+
+        Returns:
+            data queried by SQL in DataFrame form.
+        """
+        query = self.showSQL()
+        df = self.__t.session().run(query)  # type: DataFrame
+        return df
+
+
+class TablePivotBy(object):
+    """Add pivot by clause to rearrange a column (or multiple columns) of a table on two dimensions.
+
+    Args:
+        t : Table object
+        index : the result table has the same number of rows as unique values on this column.
+        column : the result table has the same number of columns as unique values on this column.
+        value : the parameters of the aggregate function. Defaults to None.
+        agg : the specified aggregate function. Defaults to lambda x: x.
+    """
+    def __init__(self, t: "Table", index: str, column: str, value=None, agg=None):
+        """Constructor of TablePivotBy."""
+        self.__row = index
+        self.__column = column
+        self.__val = value
+        self.__t = t
+        self.__agg = agg
+        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
+
+    def toDF(self) -> DataFrame:
+        """Execute SQL statement and return a DataFrame object.
+
+        Returns:
+            data queried by SQL in DataFrame form.
+        """
+        query = self.showSQL()
+        if get_verbose():
+            print(query)
+        df = self.__t.session().run(query)  # type: DataFrame
+
+        return df
+
+    toDataFrame = toDF
+
+    def _assembleSelect(self):
+        if self.__val is not None:
+            return self.__val if self.__agg is None else _getFuncName(self.__agg) + '(' + self.__val + ')'
+        return None
+
+    def _assembleTableSelect(self):
+        return self.__t._assembleSelect()
+
+    def _assembleWhere(self):
+        return self.__t._assembleWhere()
+
+    def _assemblePivotBy(self):
+        return 'pivot by ' + self.__row + ',' + self.__column
+
+    def executeAs(self, newTableName: str) -> "Table":
+        """Save execution result as an in-memory table with a specified name.
+
+        Args:
+            newTableName : new table name.
+
+        Returns:
+            a new Table object saved with the new table name.
+        """
+        self.__t.session().run(newTableName + "=" + self.showSQL())
+        return Table(data=newTableName, s=self.__t.session())
+
+    def showSQL(self) -> str:
+        """View SQL query.
+
+        Returns:
+            the SQL query for the current Table.
+        """
+        import re
+        selectOrExec = "exec" if self.__t.isExec else "select"
+        queryFmt = selectOrExec + ' {select} from {table} {where} {pivotby}'
+        fmtDict = {}
+        select = self._assembleSelect()
+        if select is not None:
+            fmtDict['select'] = select
+        else:
+            fmtDict['select'] = self._assembleTableSelect()
+        fmtDict['table'] = self.__t.tableName()
+        fmtDict['where'] = self._assembleWhere()
+        fmtDict['pivotby'] = self._assemblePivotBy()
+        query = re.sub(' +', ' ', queryFmt.format(**fmtDict).strip())
+        return query
+
+    def selectAsVector(self, colName: Union[str, Tuple[str, ...], List[str]]) -> np.array:
+        """Execute query and return the specified columns.
+
+        Args:
+            colName : a string indicating the column name.
+
+        Returns:
+            data queried by SQL in numpy.array form.
+        """
+        if colName:
+            self.__t._setSelect(colName)
+        pattern = re.compile("select", re.IGNORECASE)
+        query = pattern.sub('exec', self.showSQL())
+        return self.__t.session().run(query)
+
+
+class TableGroupby(object):
+    """The table object to which the group by clause is to be added.
+
+    Args:
+        t : Table object to be added the group by clause.
+        groupBys : grouping column(s).
+        having : the content contained in a having clause. Defaults to None.
+    """
+    def __init__(self, t: "Table", groupBys: Union[str, List[str]], having: str = None):
+        """Constructor of TableGroupby."""
+        if isinstance(groupBys, list):
+            self.__groupBys = groupBys
+        else:
+            self.__groupBys = [groupBys]
+        self.__having = having
+        self.__t = t  # type: Table
+        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
+
+    def sort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: bool = True) -> "TableGroupby":
+        """Specify parameter for sorting.
+
+        Args:
+            bys : the column(s) to sort on.
+            ascending : the sorting order. True: ascending order. Defaults to True.
+
+        Returns:
+            a TableGroupby object after adding sort clause.
+        """
+        sortTable = copy.copy(self.__t)
+        sortTable._setSort(bys, ascending)
+        return TableGroupby(sortTable, self.__groupBys, self.__having)
+
+    def csort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True) -> "TableGroupby":
+        """Specify sorting parameters for context by.
+
+        Args:
+            bys : the column to sort on.
+            ascending : the sorting order. True: ascending order. Defaults to True.
+
+        Returns:
+            a TableGroupby object after adding csort clause.
+        """
+        csortTable = copy.copy(self.__t)
+        csortTable._setCsort(bys, ascending)
+        return TableGroupby(csortTable, self.__groupBys, self.__having)
+
+    def executeAs(self, newTableName: str) -> "Table":
+        """Save execution result as an in-memory table with a specified name.
+
+        Args:
+            newTableName : new table name.
+
+        Returns:
+            a new Table object saved with the new table name.
+        """
+        st = newTableName + "=" + self.showSQL()
+        # print(st)
+        self.__t.session().run(st)
+        return Table(data=newTableName, s=self.__t.session())
+
+    def __getitem__(self, item):
+        selectTable = self.__t.select(item)
+        return TableGroupby(selectTable, groupBys=self.__groupBys, having=self.__having)
+
+    def __iter__(self):
+        self.__groupBysIdx = 0
+        return self
+
+    def next(self) -> str:
+        """Get the name of the next group by column.
+
+        Returns:
+            column name.
+        """
+        try:
+            result = self.__groupBys[self.__groupBysIdx]
+        except IndexError:
+            raise StopIteration
+        self.__groupBysIdx += 1
+        return result
+
+    def __next__(self):
+        return self.next()
+
+    def having(self, expr: str) -> "Table":
+        """Add having clause.
+
+        Args:
+            expr : expression for the having clause.
+
+        Returns:
+            a Table object after adding the having clause.
+        """
+        havingTable = copy.copy(self.__t)
+        self.__having = expr
+        havingTable._setHaving(self.__having)
+        return havingTable
+
+    def ols(self, Y: str, X: List[str], INTERCEPT: bool = True) -> dict:
+        """Calculate Least Squares Regression Coefficients.
+
+        Refer to https://dolphindb.com/help/FunctionsandCommands/FunctionReferences/o/ols.html.
+
+        Args:
+            Y : dependent variable, column name.
+            X : argument, list of column names.
+            INTERCEPT : whether to include the intercept in the regression. Defaults to True, meaning that the system automatically adds a column of "1" to X to generate the intercept.
+
+        Returns:
+            a dictionary with ANOVA, RegressionStat, Cofficient and Residual.
+        """
+        return self.__t.ols(Y=Y, X=X, INTERCEPT=INTERCEPT)
+
+    def selectAsVector(self, colName: str) -> np.array:
+        """Execute query and return the specified column.
+
+        Args:
+            colName : a string indicating the column name.
+
+        Returns:
+            data queried by SQL in numpy.array form.
+        """
+        if colName:
+            self.__t._setSelect(colName)
+        pattern = re.compile("select", re.IGNORECASE)
+        query = pattern.sub('exec', self.showSQL())
+        return self.__t.session().run(query)
+
+    def showSQL(self) -> str:
+        """View SQL query.
+
+        Returns:
+            return the SQL query for the current Table.
+        """
+        return self.__t.showSQL()
+
+    def agg(self, func) -> "Table":
+        """Apply group by on all columns.
+
+        Args:
+            func : can be an aggregate function, a list of aggregate functions, or a dict where each key indicates a column and the corresponding value indicates the aggregate function to be applied to this column.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        selectCols = self.__t._getSelect()
+        if isinstance(func, list):
+            selectCols = [_getFuncName(f) + '(' + x + ')' for x in selectCols for f in
+                          func]  # if x not in self.__groupBys
+        elif isinstance(func, dict):
+            funcDict = {}
+            for colName, f in func.items():
+                funcDict[colName] = f if isinstance(f, list) else [f]
+            selectCols = [_getFuncName(f) + '(' + x + ')' for x, funcs in funcDict.items() for f in
+                          funcs]  # if x not in self.__groupBys
+        elif isinstance(func, str):
+            selectCols = [_getFuncName(func) + '(' + x + ')' for x in selectCols]  # if x not in self.__groupBys
+        else:
+            raise RuntimeError(
+                'invalid func format, func: aggregate function name or a list of aggregate function names'
+                ' or a dict of column label/expression->func')
+        aggTable = copy.copy(self.__t)
+        aggTable._setSelect(selectCols)
+        aggTable.isMaterialized = False
+        return aggTable
+
+    def sum(self) -> "Table":
+        """Execute the aggregate function sum.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('sum')
+
+    def avg(self) -> "Table":
+        """Execute the aggregate function avg.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('avg')
+
+    def count(self) -> "Table":
+        """Execute the aggregate function count.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('count')
+
+    def max(self) -> "Table":
+        """Execute the aggregate function max.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('max')
+
+    def min(self) -> "Table":
+        """Execute the aggregate function min.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('min')
+
+    def first(self) -> "Table":
+        """Execute the aggregate function first.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('first')
+
+    def last(self) -> "Table":
+        """Execute the aggregate function last.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('last')
+
+    def size(self) -> "Table":
+        """Execute aggregate function size.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('size')
+
+    def sum2(self) -> "Table":
+        """Execute the aggregate function sum2.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('sum2')
+
+    def std(self) -> "Table":
+        """Execute aggregate function std.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('std')
+
+    def var(self) -> "Table":
+        """Execute aggregate function var.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('var')
+
+    def prod(self) -> "Table":
+        """Execute the aggregate function prod.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('prod')
+
+    def agg2(self, func, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Perform aggregate function(s) on specified column(s).
+
+        Args:
+            func : string or list of strings indicating the aggregate function(s).
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object.
+        """
+        if isinstance(cols, list) is False:
+            cols = [cols]
+        if isinstance(func, list) is False:
+            func = [func]
+        if np.sum([1 for x in cols if isinstance(x, tuple) is False or len(x) != 2]):
+            raise RuntimeError('agg2 only accepts (x,y) pair or a list of (x,y) pair as cols')
+        funcName = [_getFuncName(f) + '(' + x + ',' + y + ')' for f in func for x, y in cols]
+        selects = funcName if funcName else self.__t._getSelect()
+        agg2Table = copy.copy(self.__t)
+        agg2Table._setSelect(selects)
+        agg2Table.isMaterialized = False
+        return agg2Table
+
+    def wavg(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Perform aggregate function wavg on specified column(s).
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object.
+        """
+        return self.agg2('wavg', cols)
+
+    def wsum(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Perform aggregate function wsum on specified column(s).
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object.
+        """
+        return self.agg2('wsum', cols)
+
+    def covar(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Perform aggregate function covar on specified column(s).
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object.
+        """
+        return self.agg2('covar', cols)
+
+    def corr(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Perform aggregate function corr on specified column(s).
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object.
+        """
+        return self.agg2('corr', cols)
+
+    def toDF(self) -> DataFrame:
+        """Execute SQL statement and return a DataFrame object.
+
+        Returns:
+            data queried by SQL in DataFrame form.
+        """
+        query = self.showSQL()
+        # print(query)
+        df = self.__t.session().run(query)  # type: DataFrame
+        return df
+
+
+class TableContextby(object):
+    """The table object to add the context by clause.
+
+    Args:
+        t : Table object to add the context by clause.
+        contextBys : names of columns to be grouped for aggregation.
+        having : the content contained in a having clause. Defaults to None.
+    """
+    def __init__(self, t: "Table", contextBys: Union[str, List[str]], having: str = None):
+        """Constructor of TableContextby."""
+        if isinstance(contextBys, list):
+            self.__contextBys = contextBys
+        else:
+            self.__contextBys = [contextBys]
+        self.__t = t  # type: Table
+        self.__having = having
+        # print("constructor of ", __class__, self.__t.__dict__["_Table__tableName"])
+
+    def sort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: bool = True) -> "TableContextby":
+        """Specify parameter for sorting.
+
+        Args:
+            bys : the column(s) to sort on.
+            ascending : the sorting order. True: ascending order. Defaults to True.
+
+        Returns:
+            a TableContextby object after adding sort clause.
+        """
+        sortTable = copy.copy(self.__t)
+        sortTable._setSort(bys, ascending)
+        return TableContextby(sortTable, self.__contextBys)
+
+    def csort(self, bys: Union[str, Tuple[str, ...], List[str]], ascending: Union[bool, Tuple[bool, ...], List[bool]] = True) -> "TableContextby":
+        """Specify sorting column(s) for contextby.
+
+        Args:
+            bys : the column(s) to sort on.
+            ascending : the sorting order. True: ascending order. Defaults to True.
+
+        Returns:
+            a TableContextby object after adding csort clause.
+        """
+        csortTable = copy.copy(self.__t)
+        csortTable._setCsort(bys, ascending)
+        return TableContextby(csortTable, self.__contextBys)
+
+    def having(self, expr: str) -> "Table":
+        """Set having clause.
+
+        Args:
+            expr : expression for the having clause.
+
+        Returns:
+            a new Table object after adding the having clause.
+        """
+        havingTable = copy.copy(self.__t)
+        self.__having = expr
+        havingTable._setHaving(self.__having)
+        return havingTable
+
+    def __getitem__(self, item):
+        selectTable = self.__t.select(item)
+        return TableContextby(selectTable, contextBys=self.__contextBys)
+
+    def __iter__(self):
+        self.__contextBysIdx = 0
+        return self
+
+    def next(self) -> str:
+        """Get the name of the next grouping column for context by.
+
+        Returns:
+            column name.
+        """
+        try:
+            result = self.__contextBys[self.__contextBysIdx]
+        except IndexError:
+            raise StopIteration
+        self.__contextBysIdx += 1
+        return result
+
+    def __next__(self):
+        return self.next()
+
+    def selectAsVector(self, colName: str) -> np.array:
+        """Execute query and return the specified column.
+
+        Args:
+            colName : a string indicating the column name.
+
+        Returns:
+            data queried by SQL in numpy.array form.
+        """
+        if colName:
+            self.__t._setSelect(colName)
+        pattern = re.compile("select", re.IGNORECASE)
+        query = pattern.sub('exec', self.showSQL())
+        return self.__t.session().run(query)
+
+    def top(self, num: int) -> "Table":
+        """Set the top clause to retrieve the first n records from a Table.
+
+        Args:
+            num : the number of records to return. Must be a positive number.
+
+        Returns:
+            a Table object with the top clause.
+        """
+        return self.__t.top(num=num)
+
+    def limit(self, num: Union[int, Tuple[int, ...], List[int]]) -> "Table":
+        """Specify parameters for limit.
+
+        Args:
+            num : when used with the contextby clause, the limit clause can use a negative integer to select a limited number of records in the end of each group. 
+                  In all other cases the limit clause can only use positive integers.
+                  Can pass in [x, y] to select data from row x to row y.
+
+        Returns:
+            a Table object after adding the limit clause.
+        """
+        return self.__t.limit(num=num)
+
+    def executeAs(self, newTableName: str) -> "Table":
+        """Save execution result as an in-memory table with a specified name.
+
+        Args:
+            newTableName : new table name.
+
+        Returns:
+            a new Table object saved with the new table name.
+        """
+        st = newTableName + "=" + self.showSQL()
+        # print(st)
+        self.__t.session().run(st)
+        return Table(data=newTableName, s=self.__t.session())
+
+    def showSQL(self) -> str:
+        """View SQL query.
+
+        Returns:
+            the SQL query for the current Table.
+        """
+        return self.__t.showSQL()
+
+    def agg(self, func) -> "Table":
+        """Apply context by on all columns except the grouping columns.
+
+        Args:
+            func : string or list of strings indicating the aggregate function(s).
+
+        Returns:
+            a Table object after aggregation.
+        """
+        selectCols = self.__t._getSelect()
+        if isinstance(func, list):
+            selectCols = [_getFuncName(f) + '(' + x + ')' for x in selectCols for f in func if
+                          x not in self.__contextBys]
+        elif isinstance(func, dict):
+            funcDict = {}
+            for colName, f in func.items():
+                funcDict[colName] = f if isinstance(f, list) else [f]
+            selectCols = [_getFuncName(f) + '(' + x + ')' for x, funcs in funcDict.items() for f in funcs if
+                          x not in self.__contextBys]
+        elif isinstance(func, str):
+            selectCols = [_getFuncName(func) + '(' + x + ')' for x in selectCols if x not in self.__contextBys]
+        else:
+            raise RuntimeError(
+                'invalid func format, func: aggregate function name or a list of aggregate function names'
+                ' or a dict of column label/expression->func')
+        columns = self.__contextBys[:]
+        columns.extend(selectCols)
+        aggTable = copy.copy(self.__t)
+        aggTable._setSelect(columns)
+        aggTable.isMaterialized = False
+        return aggTable
+
+    def agg2(self, func, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Perform aggregate function(s) on specified column(s).
+
+        Args:
+            func : string or list of strings indicating the aggregate function(s).
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object.
+        """
+        if isinstance(cols, list) is False:
+            cols = [cols]
+        if isinstance(func, list) is False:
+            func = [func]
+        if np.sum([1 for x in cols if isinstance(x, tuple) is False or len(x) != 2]):
+            raise RuntimeError('agg2 only accepts (x,y) pair or a list of (x,y) pair as cols')
+        funcName = [_getFuncName(f) + '(' + x + ',' + y + ')' for f in func for x, y in cols]
+        selects = self.__t._getSelect()
+        if funcName:
+            selects.extend(funcName)
+        agg2Table = copy.copy(self.__t)
+        agg2Table._setSelect(selects)
+        agg2Table.isMaterialized = False
+        return agg2Table
+
+    def update(self, cols: List[str], vals: List[str]) -> "TableUpdate":
+        """Update in-memory table. Must be called to be executed.
+
+        Args:
+            cols : list of names of columns to be updated.
+            vals : a list of values to be updated.
+
+        Returns:
+            a TableUpdate object.
+        """
+        updateTable = TableUpdate(t=self.__t, cols=cols, vals=vals, contextby=self.__contextBys, having=self.__having)
+        return updateTable
+
+    def sum(self) -> "Table":
+        """Execute the aggregate function sum.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('sum')
+
+    def avg(self) -> "Table":
+        """Execute the aggregate function avg.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('avg')
+
+    def count(self) -> "Table":
+        """Execute the aggregate function count.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('count')
+
+    def max(self) -> "Table":
+        """Execute the aggregate function max.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('max')
+
+    def min(self) -> "Table":
+        """Execute the aggregate function min.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('min')
+
+    def first(self) -> "Table":
+        """Execute the aggregate function first.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('first')
+
+    def last(self) -> "Table":
+        """Execute the aggregate function last.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('last')
+
+    def size(self) -> "Table":
+        """Execute aggregate function size.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('size')
+
+    def sum2(self) -> "Table":
+        """Execute the aggregate function sum2.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('sum2')
+
+    def std(self) -> "Table":
+        """Execute aggregate function std.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('std')
+
+    def var(self) -> "Table":
+        """Execute aggregate function var.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('var')
+
+    def prod(self) -> "Table":
+        """Execute the aggregate function prod.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('prod')
+
+    def cumsum(self) -> "Table":
+        """Execute the aggregate function cumsum.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('cumsum')
+
+    def cummax(self) -> "Table":
+        """Execute the aggregate function cummax.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('cummax')
+
+    def cumprod(self) -> "Table":
+        """Execute the aggregate function cumprod.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('cumprod')
+
+    def cummin(self) -> "Table":
+        """Execute the aggregate function cummin.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg('cummin')
+
+    def wavg(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Execute aggregate function wavg.
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg2('wavg', cols)
+
+    def wsum(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Execute the aggregate function wsum.
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg2('wsum', cols)
+
+    def covar(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Execute the aggregate function covar.
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg2('covar', cols)
+
+    def corr(self, cols: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Execute the aggregate function corr.
+
+        Args:
+            cols : ( x, y ) tuple or list of ( x, y ) tuples, where x and y are column labels or column expressions.
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg2('corr', cols)
+
+    def eachPre(self, args: Union[Tuple[str, str], List[Tuple[str, str]]]) -> "Table":
+        """Execute the aggregate function eachPre.
+
+        Reference link: https://dolphindb.com/help/Functionalprogramming/TemplateFunctions/eachPre.html.
+
+        Args:
+            args : the function and parameters of eachPre.
+
+        Note:
+            args [0]: the function. args [1]: a vector, matrix or table. Apply args [0] over all pairs of consecutive elements of args [1].
+
+        Returns:
+            a Table object after aggregation.
+        """
+        return self.agg2('eachPre', args)
+
+    def toDF(self) -> DataFrame:
+        """Execute the SQL statement and return a DataFrame object.
+
+        Returns:
+            data queried by SQL in DataFrame form.
+        """
+        query = self.showSQL()
+        # print(query)
+        df = self.__t.session().run(query)  # type : DataFrame
+        return df
+
+
+wavg = TableGroupby.wavg
+wsum = TableGroupby.wsum
+covar = TableGroupby.covar
+corr = TableGroupby.corr
+count = TableGroupby.count
+max = TableGroupby.max
+min = TableGroupby.min
+sum = TableGroupby.sum
+sum2 = TableGroupby.sum2
+size = TableGroupby.size
+avg = TableGroupby.avg
+std = TableGroupby.std
+prod = TableGroupby.prod
+var = TableGroupby.var
+first = TableGroupby.first
+last = TableGroupby.last
+eachPre = TableContextby.eachPre
+cumsum = TableContextby.cumsum
+cumprod = TableContextby.cumprod
+cummax = TableContextby.cummax
+cummin = TableContextby.cummin
```

## dolphindb/utils.py

 * *Ordering differences only*

```diff
@@ -1,49 +1,49 @@
-import uuid
-
-
-def _generate_tablename(tableName=None):
-    if tableName is None:
-        return "TMP_TBL_" + uuid.uuid4().hex[:8]
-    else:
-        return tableName + "_TMP_TBL_" + uuid.uuid4().hex[:8]
-
-
-def _generate_dbname():
-    return "TMP_DB_" + uuid.uuid4().hex[:8]+"DB"
-
-
-def _getFuncName(f):
-    if isinstance(f, str):
-        return f
-    else:
-        return f.__name__
-
-
-def _isVariableCandidate(word: str) -> bool:
-    if len(word) < 1:
-        raise RuntimeError("The column name cannot be empty.")
-    cur = word[0]
-    if not cur.isalpha():
-        return False
-    for cur in word:
-        cur: str
-        if not cur.isalpha() and not cur.isdigit() and cur != '_':
-            return False
-    return True
-
-
-class month(object):
-    """Temporal type - Month
-
-    Args:
-        year : Year number of type month
-        month : Month number of type month
-    """
-    def __init__(self, year: int, month: int):
-        self.__year = year
-        self.__month = month
-
-    def __str__(self):
-        if self.__month > 9:
-            return str(self.__year) + '-' + str(self.__month) + 'M'
-        return str(self.__year) + '-0' + str(self.__month) + 'M'
+import uuid
+
+
+def _generate_tablename(tableName=None):
+    if tableName is None:
+        return "TMP_TBL_" + uuid.uuid4().hex[:8]
+    else:
+        return tableName + "_TMP_TBL_" + uuid.uuid4().hex[:8]
+
+
+def _generate_dbname():
+    return "TMP_DB_" + uuid.uuid4().hex[:8]+"DB"
+
+
+def _getFuncName(f):
+    if isinstance(f, str):
+        return f
+    else:
+        return f.__name__
+
+
+def _isVariableCandidate(word: str) -> bool:
+    if len(word) < 1:
+        raise RuntimeError("The column name cannot be empty.")
+    cur = word[0]
+    if not cur.isalpha():
+        return False
+    for cur in word:
+        cur: str
+        if not cur.isalpha() and not cur.isdigit() and cur != '_':
+            return False
+    return True
+
+
+class month(object):
+    """Temporal type - Month
+
+    Args:
+        year : Year number of type month
+        month : Month number of type month
+    """
+    def __init__(self, year: int, month: int):
+        self.__year = year
+        self.__month = month
+
+    def __str__(self):
+        if self.__month > 9:
+            return str(self.__year) + '-' + str(self.__month) + 'M'
+        return str(self.__year) + '-0' + str(self.__month) + 'M'
```

## dolphindb/vector.py

 * *Ordering differences only*

```diff
@@ -1,234 +1,234 @@
-from typing import Union, Type
-from pandas import Series
-from numpy import ndarray
-
-
-
-class Vector(object):
-    """Columns of a DolphinDB table.
-
-    Args:
-        name : specifies the name of the Vector. Defaults to None.
-        data : data (list or series). Defaults to None.
-        s : connected Session object. Defaults to None.
-        tableName : the table name. Defaults to None.
-    """
-    def __init__(self, name: str = None, data: Union[list, Series] = None, s=None, tableName: str = None):
-        """Constructor of Vector."""
-        self.__name = name
-        self.__tableName = tableName
-        self.__session = s  # type : Session
-        if isinstance(data, Series):
-            self.__vec = data
-        elif isinstance(data, list):
-            self.__vec = Series(data)
-        elif isinstance(data, ndarray):
-            self.__vec = Series(data)
-        else:
-            self.__vec = None
-
-    def name(self):
-        return self.__name
-
-    def tableName(self):
-        return self.__tableName
-
-    def as_series(self, useCache=False):
-        if useCache is True and self.__vec is not None:
-            return self.__vec
-        self.__vec = Series(self.__session.run('.'.join((self.__tableName, self.__name))))
-        return self.__vec
-
-    def __str__(self):
-        return self.__name
-
-    def __lt__(self, other):
-        return FilterCond(self.__name, '<', str(other))
-
-    def __rlt__(self, other):
-        return FilterCond(other, '<', str(self.__name))
-
-    def __le__(self, other):
-        return FilterCond(self.__name, '<=', str(other))
-
-    def __rle__(self, other):
-        return FilterCond(other, '<=', str(self.__name))
-
-    def __gt__(self, other):
-        return FilterCond(self.__name, '>', str(other))
-
-    def __rgt__(self, other):
-        return FilterCond(other, '>', str(self.__name))
-
-    def __ge__(self, other):
-        return FilterCond(self.__name, '>=', str(other))
-
-    def __rge__(self, other):
-        return FilterCond(other, '>=', str(self.__name))
-
-    def __eq__(self, other):
-        return FilterCond(self.__name, '==', str(other))
-
-    def __req__(self, other):
-        return FilterCond(other, '==', str(self.__name))
-
-    def __ne__(self, other):
-        return FilterCond(self.__name, '!=', str(other))
-
-    def __rne__(self, other):
-        return FilterCond(other, '!=', str(self.__name))
-
-    def __add__(self, other):
-        return FilterCond(self.__name, '+', str(other))
-
-    def __radd__(self, other):
-        return FilterCond(other, '+', str(self.__name))
-
-    def __sub__(self, other):
-        return FilterCond(self.__name, '-', str(other))
-
-    def __rsub__(self, other):
-        return FilterCond(other, '-', str(self.__name))
-
-    def __mul__(self, other):
-        return FilterCond(self.__name, '*', str(other))
-
-    def __rmul__(self, other):
-        return FilterCond(other, '*', str(self.__name))
-
-    def __truediv__(self, other):
-        return FilterCond(self.__name, '/', str(other))
-
-    def __rtruediv__(self, other):
-        return FilterCond(other, '/', str(self.__name))
-
-    def __mod__(self, other):
-        return FilterCond(self.__name, '%', str(other))
-
-    def __rmod__(self, other):
-        return FilterCond(other, '%', str(self.__name))
-
-    def __lshift__(self, other):
-        return FilterCond(self.__name, '<<', str(other))
-
-    def __rlshift__(self, other):
-        return FilterCond(other, '<<', str(self.__name))
-
-    def __rshift__(self, other):
-        return FilterCond(self.__name, '>>', str(other))
-
-    def __rrshift__(self, other):
-        return FilterCond(other, '>>', str(self.__name))
-
-    def __floordiv__(self, other):
-        return FilterCond(self.__name, '//', str(other))
-
-    def __rfloordiv__(self, other):
-        return FilterCond(other, '//', str(self.__name))
-
-
-class FilterCond(object):
-    """Filtering conditions."""
-    def __init__(self, lhs: Union[str, "FilterCond"], op: str, rhs: Union[str, "FilterCond"]):
-        self.__lhs = lhs
-        self.__op = op
-        self.__rhs = rhs
-
-    def __str__(self):
-        return '(' + str(self.__lhs) + ' ' + str(self.__op) + ' ' + str(self.__rhs) + ')'
-
-    def __or__(self, other):
-        return FilterCond(str(self), 'or', str(other))
-
-    def __ror__(self, other):
-        return FilterCond(str(other), 'or', str(self))
-
-    def __and__(self, other):
-        return FilterCond(str(self), 'and', str(other))
-
-    def __rand__(self, other):
-        return FilterCond(str(other), 'and', str(self))
-
-    def __lt__(self, other):
-        return FilterCond(str(self), '<', str(other))
-
-    def __rlt__(self, other):
-        return FilterCond(str(other), '<', str(self))
-
-    def __le__(self, other):
-        return FilterCond(str(self), '<=', str(other))
-
-    def __rle__(self, other):
-        return FilterCond(str(other), '<=', str(self))
-
-    def __gt__(self, other):
-        return FilterCond(str(self), '>', str(other))
-
-    def __rgt__(self, other):
-        return FilterCond(str(other), '>', str(self))
-
-    def __ge__(self, other):
-        return FilterCond(str(self), '>=', str(other))
-
-    def __rge__(self, other):
-        return FilterCond(str(other), '>=', str(self))
-
-    def __eq__(self, other):
-        return FilterCond(str(self), '==', str(other))
-
-    def __req__(self, other):
-        return FilterCond(str(other), '==', str(self))
-
-    def __ne__(self, other):
-        return FilterCond(str(self), '!=', str(other))
-
-    def __rne__(self, other):
-        return FilterCond(str(self), '!=', str(other))
-
-    def __add__(self, other):
-        return FilterCond(str(self), '+', str(other))
-
-    def __radd__(self, other):
-        return FilterCond(str(other), '+', str(self))
-
-    def __sub__(self, other):
-        return FilterCond(str(self), '-', str(other))
-
-    def __rsub__(self, other):
-        return FilterCond(str(other), '-', str(self))
-
-    def __mul__(self, other):
-        return FilterCond(str(self), '*', str(other))
-
-    def __rmul__(self, other):
-        return FilterCond(str(other), '*', str(self))
-
-    def __truediv__(self, other):
-        return FilterCond(str(self), '/', str(other))
-
-    def __rtruediv__(self, other):
-        return FilterCond(str(other), '/', str(self))
-
-    def __mod__(self, other):
-        return FilterCond(str(self), '%', str(other))
-
-    def __rmod__(self, other):
-        return FilterCond(str(other), '%', str(self))
-
-    def __lshift__(self, other):
-        return FilterCond(str(self), '<<', str(other))
-
-    def __rlshift__(self, other):
-        return FilterCond(str(other), '<<', str(self))
-
-    def __rshift__(self, other):
-        return FilterCond(str(self), '>>', str(other))
-
-    def __rrshift__(self, other):
-        return FilterCond(str(other), '>>', str(self))
-
-    def __floordiv__(self, other):
-        return FilterCond(str(self), '//', str(other))
-
-    def __rfloordiv__(self, other):
-        return FilterCond(str(other), '//', str(self))
+from typing import Union, Type
+from pandas import Series
+from numpy import ndarray
+
+
+
+class Vector(object):
+    """Columns of a DolphinDB table.
+
+    Args:
+        name : specifies the name of the Vector. Defaults to None.
+        data : data (list or series). Defaults to None.
+        s : connected Session object. Defaults to None.
+        tableName : the table name. Defaults to None.
+    """
+    def __init__(self, name: str = None, data: Union[list, Series] = None, s=None, tableName: str = None):
+        """Constructor of Vector."""
+        self.__name = name
+        self.__tableName = tableName
+        self.__session = s  # type : Session
+        if isinstance(data, Series):
+            self.__vec = data
+        elif isinstance(data, list):
+            self.__vec = Series(data)
+        elif isinstance(data, ndarray):
+            self.__vec = Series(data)
+        else:
+            self.__vec = None
+
+    def name(self):
+        return self.__name
+
+    def tableName(self):
+        return self.__tableName
+
+    def as_series(self, useCache=False):
+        if useCache is True and self.__vec is not None:
+            return self.__vec
+        self.__vec = Series(self.__session.run('.'.join((self.__tableName, self.__name))))
+        return self.__vec
+
+    def __str__(self):
+        return self.__name
+
+    def __lt__(self, other):
+        return FilterCond(self.__name, '<', str(other))
+
+    def __rlt__(self, other):
+        return FilterCond(other, '<', str(self.__name))
+
+    def __le__(self, other):
+        return FilterCond(self.__name, '<=', str(other))
+
+    def __rle__(self, other):
+        return FilterCond(other, '<=', str(self.__name))
+
+    def __gt__(self, other):
+        return FilterCond(self.__name, '>', str(other))
+
+    def __rgt__(self, other):
+        return FilterCond(other, '>', str(self.__name))
+
+    def __ge__(self, other):
+        return FilterCond(self.__name, '>=', str(other))
+
+    def __rge__(self, other):
+        return FilterCond(other, '>=', str(self.__name))
+
+    def __eq__(self, other):
+        return FilterCond(self.__name, '==', str(other))
+
+    def __req__(self, other):
+        return FilterCond(other, '==', str(self.__name))
+
+    def __ne__(self, other):
+        return FilterCond(self.__name, '!=', str(other))
+
+    def __rne__(self, other):
+        return FilterCond(other, '!=', str(self.__name))
+
+    def __add__(self, other):
+        return FilterCond(self.__name, '+', str(other))
+
+    def __radd__(self, other):
+        return FilterCond(other, '+', str(self.__name))
+
+    def __sub__(self, other):
+        return FilterCond(self.__name, '-', str(other))
+
+    def __rsub__(self, other):
+        return FilterCond(other, '-', str(self.__name))
+
+    def __mul__(self, other):
+        return FilterCond(self.__name, '*', str(other))
+
+    def __rmul__(self, other):
+        return FilterCond(other, '*', str(self.__name))
+
+    def __truediv__(self, other):
+        return FilterCond(self.__name, '/', str(other))
+
+    def __rtruediv__(self, other):
+        return FilterCond(other, '/', str(self.__name))
+
+    def __mod__(self, other):
+        return FilterCond(self.__name, '%', str(other))
+
+    def __rmod__(self, other):
+        return FilterCond(other, '%', str(self.__name))
+
+    def __lshift__(self, other):
+        return FilterCond(self.__name, '<<', str(other))
+
+    def __rlshift__(self, other):
+        return FilterCond(other, '<<', str(self.__name))
+
+    def __rshift__(self, other):
+        return FilterCond(self.__name, '>>', str(other))
+
+    def __rrshift__(self, other):
+        return FilterCond(other, '>>', str(self.__name))
+
+    def __floordiv__(self, other):
+        return FilterCond(self.__name, '//', str(other))
+
+    def __rfloordiv__(self, other):
+        return FilterCond(other, '//', str(self.__name))
+
+
+class FilterCond(object):
+    """Filtering conditions."""
+    def __init__(self, lhs: Union[str, "FilterCond"], op: str, rhs: Union[str, "FilterCond"]):
+        self.__lhs = lhs
+        self.__op = op
+        self.__rhs = rhs
+
+    def __str__(self):
+        return '(' + str(self.__lhs) + ' ' + str(self.__op) + ' ' + str(self.__rhs) + ')'
+
+    def __or__(self, other):
+        return FilterCond(str(self), 'or', str(other))
+
+    def __ror__(self, other):
+        return FilterCond(str(other), 'or', str(self))
+
+    def __and__(self, other):
+        return FilterCond(str(self), 'and', str(other))
+
+    def __rand__(self, other):
+        return FilterCond(str(other), 'and', str(self))
+
+    def __lt__(self, other):
+        return FilterCond(str(self), '<', str(other))
+
+    def __rlt__(self, other):
+        return FilterCond(str(other), '<', str(self))
+
+    def __le__(self, other):
+        return FilterCond(str(self), '<=', str(other))
+
+    def __rle__(self, other):
+        return FilterCond(str(other), '<=', str(self))
+
+    def __gt__(self, other):
+        return FilterCond(str(self), '>', str(other))
+
+    def __rgt__(self, other):
+        return FilterCond(str(other), '>', str(self))
+
+    def __ge__(self, other):
+        return FilterCond(str(self), '>=', str(other))
+
+    def __rge__(self, other):
+        return FilterCond(str(other), '>=', str(self))
+
+    def __eq__(self, other):
+        return FilterCond(str(self), '==', str(other))
+
+    def __req__(self, other):
+        return FilterCond(str(other), '==', str(self))
+
+    def __ne__(self, other):
+        return FilterCond(str(self), '!=', str(other))
+
+    def __rne__(self, other):
+        return FilterCond(str(self), '!=', str(other))
+
+    def __add__(self, other):
+        return FilterCond(str(self), '+', str(other))
+
+    def __radd__(self, other):
+        return FilterCond(str(other), '+', str(self))
+
+    def __sub__(self, other):
+        return FilterCond(str(self), '-', str(other))
+
+    def __rsub__(self, other):
+        return FilterCond(str(other), '-', str(self))
+
+    def __mul__(self, other):
+        return FilterCond(str(self), '*', str(other))
+
+    def __rmul__(self, other):
+        return FilterCond(str(other), '*', str(self))
+
+    def __truediv__(self, other):
+        return FilterCond(str(self), '/', str(other))
+
+    def __rtruediv__(self, other):
+        return FilterCond(str(other), '/', str(self))
+
+    def __mod__(self, other):
+        return FilterCond(str(self), '%', str(other))
+
+    def __rmod__(self, other):
+        return FilterCond(str(other), '%', str(self))
+
+    def __lshift__(self, other):
+        return FilterCond(str(self), '<<', str(other))
+
+    def __rlshift__(self, other):
+        return FilterCond(str(other), '<<', str(self))
+
+    def __rshift__(self, other):
+        return FilterCond(str(self), '>>', str(other))
+
+    def __rrshift__(self, other):
+        return FilterCond(str(other), '>>', str(self))
+
+    def __floordiv__(self, other):
+        return FilterCond(str(self), '//', str(other))
+
+    def __rfloordiv__(self, other):
+        return FilterCond(str(other), '//', str(self))
```

## Comparing `dolphindb-2.0.11.0.dist-info/LICENSE` & `dolphindb-3.0.0.0.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-Copyright 2016-2023 DolphinDB, Inc.
-    
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2016-2023 DolphinDB, Inc.
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Copyright 2016-2023 DolphinDB, Inc.
+    
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2016-2023 DolphinDB, Inc.
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

## Comparing `dolphindb-2.0.11.0.dist-info/METADATA` & `dolphindb-3.0.0.0.dist-info/METADATA`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: dolphindb
-Version: 2.0.11.0
-Summary: A C++ boosted DolphinDB Python API based on Pybind11
-Home-page: https://www.dolphindb.com
-Author: DolphinDB, Inc.
-Author-email: support@dolphindb.com
-License: DolphinDB
-Platform: Windows
-Platform: MacOS
-Platform: Linux
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy >=1.18.0
-Requires-Dist: pandas !=1.3.0,>=1.0.0
-Requires-Dist: future
-
-# DolphinDB Python SDK
-
-A C++ boosted API for Python, built on Pybind11.
-
-## Requirements
-
-To use DolphinDB Python SDK, you'll need:
-
-- Python:
-  - CPython: version 3.6 and newer
-- DolphinDB Server
-- Packages:
-  - NumPy: version 1.18 and newer
-  - pandas: version 1.0.0 and newer, but not version 1.3.0
-  - future
-- Extension Packages:
-  - PyArrow: version 9.0.0 and newer
-
-## Installation
-
-To install the DolphinDB package, use the following command:
-
-```sh
-pip install dolphindb
-```
-
-## Example Code
-
-Here's an example of using DolphinDB Python SDK:
-
-```python
-import dolphindb as ddb
-
-conn = ddb.Session()
-conn.connect("localhost", 8848, "admin", "123456")
-
-conn.run("1+1;")
------------------------
-2
-```
+Metadata-Version: 2.1
+Name: dolphindb
+Version: 3.0.0.0
+Summary: A C++ boosted DolphinDB Python API based on Pybind11
+Home-page: https://www.dolphindb.com
+Author: DolphinDB, Inc.
+Author-email: support@dolphindb.com
+License: DolphinDB
+Platform: Windows
+Platform: MacOS
+Platform: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy >=1.18.0
+Requires-Dist: pandas !=1.3.0,>=1.0.0
+Requires-Dist: future
+
+# DolphinDB Python SDK
+
+A C++ boosted API for Python, built on Pybind11.
+
+## Requirements
+
+To use DolphinDB Python SDK, you'll need:
+
+- Python:
+  - CPython: version 3.6 and newer
+- DolphinDB Server
+- Packages:
+  - NumPy: version 1.18 and newer
+  - pandas: version 1.0.0 and newer, but not version 1.3.0
+  - future
+- Extension Packages:
+  - PyArrow: version 9.0.0 and newer
+
+## Installation
+
+To install the DolphinDB package, use the following command:
+
+```sh
+pip install dolphindb
+```
+
+## Example Code
+
+Here's an example of using DolphinDB Python SDK:
+
+```python
+import dolphindb as ddb
+
+conn = ddb.Session()
+conn.connect("localhost", 8848, "admin", "123456")
+
+conn.run("1+1;")
+-----------------------
+2
+```
```

