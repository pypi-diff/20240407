# Comparing `tmp/flask_redis_caching-1.0.3.tar.gz` & `tmp/flask_redis_caching-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_redis_caching-1.0.3.tar", last modified: Mon Mar 11 14:05:41 2024, max compression
+gzip compressed data, was "flask_redis_caching-1.0.4.tar", last modified: Sun Apr  7 01:02:27 2024, max compression
```

## Comparing `flask_redis_caching-1.0.3.tar` & `flask_redis_caching-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 14:05:41.715339 flask_redis_caching-1.0.3/
--rw-rw-rw-   0        0        0      311 2024-03-11 14:05:41.714183 flask_redis_caching-1.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-11 14:05:41.712187 flask_redis_caching-1.0.3/flask_redis_caching.egg-info/
--rw-rw-rw-   0        0        0      311 2024-03-11 14:05:41.000000 flask_redis_caching-1.0.3/flask_redis_caching.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-03-11 14:05:41.000000 flask_redis_caching-1.0.3/flask_redis_caching.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 14:05:41.000000 flask_redis_caching-1.0.3/flask_redis_caching.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-11 14:05:41.000000 flask_redis_caching-1.0.3/flask_redis_caching.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-11 14:05:41.000000 flask_redis_caching-1.0.3/flask_redis_caching.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-11 14:05:41.714183 flask_redis_caching-1.0.3/redis_caching/
--rw-rw-rw-   0        0        0       35 2024-03-11 14:04:12.000000 flask_redis_caching-1.0.3/redis_caching/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-03-10 20:58:53.000000 flask_redis_caching-1.0.3/redis_caching/caching.py
--rw-rw-rw-   0        0        0       42 2024-03-11 14:05:41.715339 flask_redis_caching-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      479 2024-03-11 14:05:35.000000 flask_redis_caching-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:27.599523 flask_redis_caching-1.0.4/
+-rw-rw-rw-   0        0        0      311 2024-04-07 01:02:27.598493 flask_redis_caching-1.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:27.568019 flask_redis_caching-1.0.4/flask_redis_caching/
+-rw-rw-rw-   0        0        0       35 2024-03-11 14:07:03.000000 flask_redis_caching-1.0.4/flask_redis_caching/__init__.py
+-rw-rw-rw-   0        0        0     4366 2024-04-07 01:01:21.000000 flask_redis_caching-1.0.4/flask_redis_caching/caching.py
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:27.587619 flask_redis_caching-1.0.4/flask_redis_caching.egg-info/
+-rw-rw-rw-   0        0        0      311 2024-04-07 01:02:27.000000 flask_redis_caching-1.0.4/flask_redis_caching.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2024-04-07 01:02:27.000000 flask_redis_caching-1.0.4/flask_redis_caching.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 01:02:27.000000 flask_redis_caching-1.0.4/flask_redis_caching.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 01:02:27.000000 flask_redis_caching-1.0.4/flask_redis_caching.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2024-04-07 01:02:27.000000 flask_redis_caching-1.0.4/flask_redis_caching.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:27.597486 flask_redis_caching-1.0.4/redis_caching/
+-rw-rw-rw-   0        0        0       35 2024-03-11 14:04:12.000000 flask_redis_caching-1.0.4/redis_caching/__init__.py
+-rw-rw-rw-   0        0        0     4062 2024-04-07 01:00:21.000000 flask_redis_caching-1.0.4/redis_caching/caching.py
+-rw-rw-rw-   0        0        0       42 2024-04-07 01:02:27.599523 flask_redis_caching-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      479 2024-04-07 01:01:35.000000 flask_redis_caching-1.0.4/setup.py
```

### Comparing `flask_redis_caching-1.0.3/redis_caching/caching.py` & `flask_redis_caching-1.0.4/redis_caching/caching.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,24 +6,27 @@
 
 
 class RedisCaching:
     """
     RedisCaching provides caching functionalities using Redis for storing and retrieving cached values.
     """
     
-    def __init__(self, log: bool = True, **kwargs):
+    def __init__(self, log: bool = True, pre_ping: bool = False, **kwargs):
         self.log = log
 
         self._redis_client = redis.Redis(**kwargs)
 
         self._log("The logging is currently on. If you wish to turn it off, simply include log=False as an argument in the __init__ function.")
 
-        self._pre_ping()
+        if pre_ping is True:
+            self._pre_ping()
 
     def _pre_ping(self) -> None:
+        self._log("The pre ping is currently on. If you wish to turn it off, simply include pre_ping=False as an argument in the __init__ function.")
+
         self._log("A ping was sent to the Redis server.")
 
         self._redis_client.ping()
 
         self._log("The Redis server received a ping.")
 
     def _log(self, message: str) -> None:
```

