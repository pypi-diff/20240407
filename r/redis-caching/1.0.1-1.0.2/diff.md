# Comparing `tmp/redis_caching-1.0.1.tar.gz` & `tmp/redis_caching-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_caching-1.0.1.tar", last modified: Mon Mar 11 14:05:48 2024, max compression
+gzip compressed data, was "redis_caching-1.0.2.tar", last modified: Sun Apr  7 01:02:54 2024, max compression
```

## Comparing `redis_caching-1.0.1.tar` & `redis_caching-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 14:05:48.262084 redis_caching-1.0.1/
--rw-rw-rw-   0        0        0      271 2024-03-11 14:05:48.262084 redis_caching-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-11 14:05:48.247657 redis_caching-1.0.1/redis_caching/
--rw-rw-rw-   0        0        0       35 2024-03-11 14:04:12.000000 redis_caching-1.0.1/redis_caching/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-03-10 20:58:53.000000 redis_caching-1.0.1/redis_caching/caching.py
-drwxrwxrwx   0        0        0        0 2024-03-11 14:05:48.260086 redis_caching-1.0.1/redis_caching.egg-info/
--rw-rw-rw-   0        0        0      271 2024-03-11 14:05:48.000000 redis_caching-1.0.1/redis_caching.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2024-03-11 14:05:48.000000 redis_caching-1.0.1/redis_caching.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 14:05:48.000000 redis_caching-1.0.1/redis_caching.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-11 14:05:48.000000 redis_caching-1.0.1/redis_caching.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-11 14:05:48.262084 redis_caching-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      479 2024-03-11 14:05:35.000000 redis_caching-1.0.1/setup.py
--rw-rw-rw-   0        0        0      384 2024-03-11 14:05:38.000000 redis_caching-1.0.1/setup_redis_caching.py
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:54.361230 redis_caching-1.0.2/
+-rw-rw-rw-   0        0        0      271 2024-04-07 01:02:54.360222 redis_caching-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:54.342951 redis_caching-1.0.2/flask_redis_caching/
+-rw-rw-rw-   0        0        0       35 2024-03-11 14:07:03.000000 redis_caching-1.0.2/flask_redis_caching/__init__.py
+-rw-rw-rw-   0        0        0     4366 2024-04-07 01:01:21.000000 redis_caching-1.0.2/flask_redis_caching/caching.py
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:54.344922 redis_caching-1.0.2/redis_caching/
+-rw-rw-rw-   0        0        0       35 2024-03-11 14:04:12.000000 redis_caching-1.0.2/redis_caching/__init__.py
+-rw-rw-rw-   0        0        0     4062 2024-04-07 01:00:21.000000 redis_caching-1.0.2/redis_caching/caching.py
+drwxrwxrwx   0        0        0        0 2024-04-07 01:02:54.358717 redis_caching-1.0.2/redis_caching.egg-info/
+-rw-rw-rw-   0        0        0      271 2024-04-07 01:02:54.000000 redis_caching-1.0.2/redis_caching.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2024-04-07 01:02:54.000000 redis_caching-1.0.2/redis_caching.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 01:02:54.000000 redis_caching-1.0.2/redis_caching.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-04-07 01:02:54.000000 redis_caching-1.0.2/redis_caching.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 01:02:54.361230 redis_caching-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      479 2024-04-07 01:01:35.000000 redis_caching-1.0.2/setup.py
+-rw-rw-rw-   0        0        0      384 2024-04-07 01:01:37.000000 redis_caching-1.0.2/setup_redis_caching.py
```

### Comparing `redis_caching-1.0.1/redis_caching/caching.py` & `redis_caching-1.0.2/redis_caching/caching.py`

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

