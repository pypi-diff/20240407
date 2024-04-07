# Comparing `tmp/lesscode_database-0.0.8.tar.gz` & `tmp/lesscode_database-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lesscode_database-0.0.8.tar", last modified: Sun Dec  3 15:09:57 2023, max compression
+gzip compressed data, was "dist/lesscode_database-0.0.9.tar", last modified: Sun Apr  7 02:31:44 2024, max compression
```

## Comparing `lesscode_database-0.0.8.tar` & `lesscode_database-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/
--rw-r--r--   0 navy      (1000) navy      (1000)    11357 2023-06-01 13:04:22.000000 lesscode_database-0.0.8/LICENSE
--rw-r--r--   0 navy      (1000) navy      (1000)    11692 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)    11326 2023-12-03 15:03:15.000000 lesscode_database-0.0.8/README.md
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/lesscode_database/
--rw-r--r--   0 navy      (1000) navy      (1000)        0 2023-06-01 13:04:45.000000 lesscode_database-0.0.8/lesscode_database/__init__.py
--rw-r--r--   0 navy      (1000) navy      (1000)    41144 2023-12-03 14:45:34.000000 lesscode_database-0.0.8/lesscode_database/connect_pool.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1307 2023-12-03 09:06:15.000000 lesscode_database-0.0.8/lesscode_database/connection_info.py
--rw-r--r--   0 navy      (1000) navy      (1000)     1928 2023-12-03 12:45:01.000000 lesscode_database-0.0.8/lesscode_database/db_options.py
--rw-r--r--   0 navy      (1000) navy      (1000)     4832 2023-12-03 14:57:31.000000 lesscode_database-0.0.8/lesscode_database/db_request.py
--rw-r--r--   0 navy      (1000) navy      (1000)     4845 2023-12-03 14:33:59.000000 lesscode_database-0.0.8/lesscode_database/ds_helper.py
--rw-r--r--   0 navy      (1000) navy      (1000)      164 2023-12-03 09:06:15.000000 lesscode_database-0.0.8/lesscode_database/dynamic_import_package.py
--rw-r--r--   0 navy      (1000) navy      (1000)     6406 2023-12-03 15:09:52.000000 lesscode_database-0.0.8/lesscode_database/mongo_base_model.py
--rw-r--r--   0 navy      (1000) navy      (1000)       22 2023-12-03 15:09:53.000000 lesscode_database-0.0.8/lesscode_database/version.py
-drwxr-xr-x   0 navy      (1000) navy      (1000)        0 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/lesscode_database.egg-info/
--rw-r--r--   0 navy      (1000) navy      (1000)    11692 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/lesscode_database.egg-info/PKG-INFO
--rw-r--r--   0 navy      (1000) navy      (1000)      497 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/lesscode_database.egg-info/SOURCES.txt
--rw-r--r--   0 navy      (1000) navy      (1000)        1 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/lesscode_database.egg-info/dependency_links.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       18 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/lesscode_database.egg-info/top_level.txt
--rw-r--r--   0 navy      (1000) navy      (1000)       38 2023-12-03 15:09:57.000000 lesscode_database-0.0.8/setup.cfg
--rw-r--r--   0 navy      (1000) navy      (1000)     1198 2023-06-03 08:00:48.000000 lesscode_database-0.0.8/setup.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2024-04-07 02:31:44.000000 lesscode_database-0.0.9/
+-rw-r--r--   0 baai       (501) staff       (20)    11357 2024-04-03 03:48:35.000000 lesscode_database-0.0.9/LICENSE
+-rw-r--r--   0 baai       (501) staff       (20)    11692 2024-04-07 02:31:44.000000 lesscode_database-0.0.9/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)    11326 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/README.md
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2024-04-07 02:31:44.000000 lesscode_database-0.0.9/lesscode_database/
+-rw-r--r--   0 baai       (501) staff       (20)        0 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/lesscode_database/__init__.py
+-rw-r--r--   0 baai       (501) staff       (20)    44572 2024-04-07 02:30:09.000000 lesscode_database-0.0.9/lesscode_database/connect_pool.py
+-rw-r--r--   0 baai       (501) staff       (20)     1307 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/lesscode_database/connection_info.py
+-rw-r--r--   0 baai       (501) staff       (20)     1928 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/lesscode_database/db_options.py
+-rw-r--r--   0 baai       (501) staff       (20)     4832 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/lesscode_database/db_request.py
+-rw-r--r--   0 baai       (501) staff       (20)     4845 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/lesscode_database/ds_helper.py
+-rw-r--r--   0 baai       (501) staff       (20)      164 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/lesscode_database/dynamic_import_package.py
+-rw-r--r--   0 baai       (501) staff       (20)     6406 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/lesscode_database/mongo_base_model.py
+-rw-r--r--   0 baai       (501) staff       (20)       22 2024-04-07 02:30:09.000000 lesscode_database-0.0.9/lesscode_database/version.py
+drwxr-xr-x   0 baai       (501) staff       (20)        0 2024-04-07 02:31:44.000000 lesscode_database-0.0.9/lesscode_database.egg-info/
+-rw-r--r--   0 baai       (501) staff       (20)    11692 2024-04-07 02:31:43.000000 lesscode_database-0.0.9/lesscode_database.egg-info/PKG-INFO
+-rw-r--r--   0 baai       (501) staff       (20)      497 2024-04-07 02:31:44.000000 lesscode_database-0.0.9/lesscode_database.egg-info/SOURCES.txt
+-rw-r--r--   0 baai       (501) staff       (20)        1 2024-04-07 02:31:43.000000 lesscode_database-0.0.9/lesscode_database.egg-info/dependency_links.txt
+-rw-r--r--   0 baai       (501) staff       (20)       18 2024-04-07 02:31:43.000000 lesscode_database-0.0.9/lesscode_database.egg-info/top_level.txt
+-rw-r--r--   0 baai       (501) staff       (20)       38 2024-04-07 02:31:44.000000 lesscode_database-0.0.9/setup.cfg
+-rw-r--r--   0 baai       (501) staff       (20)     1198 2024-04-03 05:51:55.000000 lesscode_database-0.0.9/setup.py
```

### Comparing `lesscode_database-0.0.8/LICENSE` & `lesscode_database-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.8/PKG-INFO` & `lesscode_database-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesscode_database
-Version: 0.0.8
+Version: 0.0.9
 Summary: lesscode_database是数据库连接工具包
 Author: navysummer
 Author-email: navysummer@yeah.net
 Platform: python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lesscode_database-0.0.8/README.md` & `lesscode_database-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.8/lesscode_database/connect_pool.py` & `lesscode_database-0.0.9/lesscode_database/connect_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -653,21 +653,30 @@
                                         user=conn_info.user, password=conn_info.password,
                                         port=conn_info.port, database=conn_info.db_name)
         return pool
 
     @staticmethod
     def sync_create_clickhouse_pool(conn_info: ConnectionInfo):
         try:
-            clickhouse_driver_dbapi = importlib.import_module("clickhouse_driver.dbapi")
+            pooled_db = importlib.import_module("dbutils.pooled_db")
         except ImportError:
-            raise ImportError(f"clickhouse-driver is not exist,run:pip install clickhouse-driver")
-        con = clickhouse_driver_dbapi.connect(dsn=conn_info.dsn, host=conn_info.host,
-                                              user=conn_info.user, password=conn_info.password,
-                                              port=conn_info.port, database=conn_info.db_name)
-        return con
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils==3.0.2")
+        try:
+            clickhouse_driver = importlib.import_module("clickhouse_driver")
+        except ImportError:
+            raise Exception(f"clickhouse_driver is not exist,run:pip install clickhouse_driver")
+        params = conn_info.params
+        if not isinstance(params, dict):
+            params = dict()
+
+        pool = pooled_db.PooledDB(creator=clickhouse_driver.connect, host=conn_info.host, port=conn_info.port,
+                                  user=conn_info.user,
+                                  password=conn_info.password, database=conn_info.db_name or "default",
+                                  **params)
+        return pool
 
     @staticmethod
     def create_sqlalchemy_pool(conn_info: ConnectionInfo):
         """
         创建sqlalchemy同步连接池
         :param conn_info: 连接信息
         :return:
@@ -777,14 +786,64 @@
                                                                             0) if conn_info.params else 0,
                                           pool_timeout=conn_info.params.get("pool_timeout",
                                                                             10) if conn_info.params else 10,
                                           pool_pre_ping=conn_info.params.get("pool_pre_ping",
                                                                              True) if conn_info.params else True)
         return engine
 
+    @staticmethod
+    def sync_create_dbutils_pool(conn_info: ConnectionInfo):
+        params = conn_info.params
+        if not isinstance(params, dict):
+            params = dict()
+        creator = params.pop("creator")
+        try:
+            generic = importlib.import_module(creator)
+        except ImportError:
+            raise Exception(f"{creator} is not exist,run:pip install {creator}")
+        try:
+            pooled_db = importlib.import_module("dbutils.pooled_db")
+            steady_db = importlib.import_module("dbutils.steady_db")
+            simple_pooled_db = importlib.import_module("dbutils.simple_pooled_db")
+            persistent_db = importlib.import_module("dbutils.persistent_db")
+        except ImportError:
+            raise Exception(f"DBUtils is not exist,run:pip install DBUtils==3.0.2")
+        pool_type = params.pop("pool_type", "PooledDB")
+        if pool_type not in ["SimplePooledDB", "SteadyDBConnection", "PersistentDB", "PooledDB"]:
+            pool_type = "PooledDB"
+
+        mincached = params.pop("mincached", conn_info.min_size)
+        maxusage = params.pop("maxusage", conn_info.min_size)
+        maxshared = params.pop("maxshared", conn_info.max_size)
+        maxcached = params.pop("maxcached", conn_info.max_size)
+        blocking = params.pop("blocking", True)
+        reset = params.pop("reset", True)
+        setsession = params.pop("setsession", None)
+        failures = params.pop("failures", None)
+        ping = params.pop("ping", 1)
+        threadlocal = params.pop("threadlocal", None)
+        closeable = params.pop("closeable", True)
+        maxconnections = params.pop("maxconnections", None)
+        if pool_type == "SimplePooledDB":
+            pool = simple_pooled_db.PooledDB(dbapi=creator, maxconnections=maxconnections, **params)
+        elif pool_type == "SteadyDBConnection":
+            pool = steady_db.SteadyDBConnection(creator=creator, maxusage=maxusage, setsession=setsession,
+                                                failures=failures,
+                                                ping=ping, closeable=closeable, **params)
+        elif pool_type == "PersistentDB":
+            pool = persistent_db.PersistentDB(creator=creator, maxusage=maxusage, setsession=setsession,
+                                              failures=failures, ping=ping,
+                                              closeable=closeable, threadlocal=threadlocal, **params)
+        else:
+            pool = pooled_db.PooledDB(creator=generic, mincached=mincached, maxcached=maxcached,
+                                      maxshared=maxshared, maxconnections=conn_info.max_size, blocking=blocking,
+                                      maxusage=maxusage, setsession=setsession, reset=reset,
+                                      failures=failures, ping=ping, **params)
+        return pool
+
 
 def run_sync(func_instance):
     if iscoroutine(func_instance):
         loop = asyncio.get_event_loop()
         future = asyncio.ensure_future(func_instance)
         loop.run_until_complete(future)
         return future.result()
@@ -882,9 +941,15 @@
 
     elif conn_info.dialect == "sqlalchemy":
         if conn_info.async_enable:
             return run_sync(Pool.create_sqlalchemy_pool(conn_info)), conn_info
         else:
             return run_sync(Pool.sync_create_sqlalchemy_pool(conn_info)), conn_info
 
+    elif conn_info.dialect == "dbutils":
+        if conn_info.async_enable:
+            return run_sync(Pool.sync_create_dbutils_pool(conn_info)), conn_info
+        else:
+            return run_sync(Pool.sync_create_dbutils_pool(conn_info)), conn_info
+
     else:
         raise Exception(f"conn_info.dialect={conn_info.dialect} is not supported")
```

### Comparing `lesscode_database-0.0.8/lesscode_database/connection_info.py` & `lesscode_database-0.0.9/lesscode_database/connection_info.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.8/lesscode_database/db_options.py` & `lesscode_database-0.0.9/lesscode_database/db_options.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.8/lesscode_database/db_request.py` & `lesscode_database-0.0.9/lesscode_database/db_request.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.8/lesscode_database/ds_helper.py` & `lesscode_database-0.0.9/lesscode_database/ds_helper.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.8/lesscode_database/mongo_base_model.py` & `lesscode_database-0.0.9/lesscode_database/mongo_base_model.py`

 * *Files identical despite different names*

### Comparing `lesscode_database-0.0.8/lesscode_database.egg-info/PKG-INFO` & `lesscode_database-0.0.9/lesscode_database.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lesscode-database
-Version: 0.0.8
+Version: 0.0.9
 Summary: lesscode_database是数据库连接工具包
 Author: navysummer
 Author-email: navysummer@yeah.net
 Platform: python
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `lesscode_database-0.0.8/setup.py` & `lesscode_database-0.0.9/setup.py`

 * *Files identical despite different names*

