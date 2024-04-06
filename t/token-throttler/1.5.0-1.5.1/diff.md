# Comparing `tmp/token_throttler-1.5.0.tar.gz` & `tmp/token_throttler-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "token_throttler-1.5.0.tar", max compression
+gzip compressed data, was "token_throttler-1.5.1.tar", max compression
```

## Comparing `token_throttler-1.5.0.tar` & `token_throttler-1.5.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1058 2024-03-20 23:38:24.204175 token_throttler-1.5.0/LICENSE
--rw-r--r--   0        0        0     8424 2024-03-20 23:23:08.715079 token_throttler-1.5.0/README.md
--rw-r--r--   0        0        0     2665 2024-03-20 23:38:47.300971 token_throttler-1.5.0/pyproject.toml
--rw-r--r--   0        0        0      269 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/__init__.py
--rw-r--r--   0        0        0      238 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/exception.py
--rw-r--r--   0        0        0        0 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/ext/__init__.py
--rw-r--r--   0        0        0      799 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/ext/fastapi.py
--rw-r--r--   0        0        0        0 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/py.typed
--rw-r--r--   0        0        0      139 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/storage/__init__.py
--rw-r--r--   0        0        0     1107 2024-03-20 23:39:41.111265 token_throttler-1.5.0/src/token_throttler/storage/bucket_storage.py
--rw-r--r--   0        0        0     1168 2024-03-20 23:39:32.551219 token_throttler-1.5.0/src/token_throttler/storage/bucket_storage_async.py
--rw-r--r--   0        0        0       91 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/storage/redis/__init__.py
--rw-r--r--   0        0        0     3806 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/storage/redis/redis_storage.py
--rw-r--r--   0        0        0     4001 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/storage/redis/redis_storage_async.py
--rw-r--r--   0        0        0     1728 2024-03-20 23:23:08.718412 token_throttler-1.5.0/src/token_throttler/storage/runtime_storage.py
--rw-r--r--   0        0        0     2033 2024-03-20 23:39:15.481126 token_throttler-1.5.0/src/token_throttler/throttler_config.py
--rw-r--r--   0        0        0      753 2024-03-20 23:23:08.721746 token_throttler-1.5.0/src/token_throttler/token_bucket.py
--rw-r--r--   0        0        0     4165 2024-03-20 23:23:08.721746 token_throttler-1.5.0/src/token_throttler/token_throttler.py
--rw-r--r--   0        0        0     3955 2024-03-20 23:23:08.721746 token_throttler-1.5.0/src/token_throttler/token_throttler_async.py
--rw-r--r--   0        0        0     1945 2024-03-20 23:23:08.721746 token_throttler-1.5.0/src/token_throttler/validate.py
--rw-r--r--   0        0        0     9985 1970-01-01 00:00:00.000000 token_throttler-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-03-20 23:38:24.204175 token_throttler-1.5.1/LICENSE
+-rw-r--r--   0        0        0     8427 2024-04-06 22:23:38.931991 token_throttler-1.5.1/README.md
+-rw-r--r--   0        0        0     2665 2024-04-06 22:23:38.925324 token_throttler-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0      269 2024-03-20 23:23:08.718412 token_throttler-1.5.1/src/token_throttler/__init__.py
+-rw-r--r--   0        0        0      238 2024-03-20 23:23:08.718412 token_throttler-1.5.1/src/token_throttler/exception.py
+-rw-r--r--   0        0        0        0 2024-03-20 23:23:08.718412 token_throttler-1.5.1/src/token_throttler/ext/__init__.py
+-rw-r--r--   0        0        0      799 2024-03-20 23:23:08.718412 token_throttler-1.5.1/src/token_throttler/ext/fastapi.py
+-rw-r--r--   0        0        0        0 2024-03-20 23:23:08.718412 token_throttler-1.5.1/src/token_throttler/py.typed
+-rw-r--r--   0        0        0      139 2024-03-20 23:23:08.718412 token_throttler-1.5.1/src/token_throttler/storage/__init__.py
+-rw-r--r--   0        0        0     1107 2024-03-20 23:39:41.111265 token_throttler-1.5.1/src/token_throttler/storage/bucket_storage.py
+-rw-r--r--   0        0        0     1168 2024-03-20 23:39:32.551219 token_throttler-1.5.1/src/token_throttler/storage/bucket_storage_async.py
+-rw-r--r--   0        0        0       91 2024-03-20 23:23:08.718412 token_throttler-1.5.1/src/token_throttler/storage/redis/__init__.py
+-rw-r--r--   0        0        0     3819 2024-04-06 21:31:38.106576 token_throttler-1.5.1/src/token_throttler/storage/redis/redis_storage.py
+-rw-r--r--   0        0        0     4014 2024-04-06 21:31:38.099910 token_throttler-1.5.1/src/token_throttler/storage/redis/redis_storage_async.py
+-rw-r--r--   0        0        0     1666 2024-04-06 22:44:10.313697 token_throttler-1.5.1/src/token_throttler/storage/runtime_storage.py
+-rw-r--r--   0        0        0     2037 2024-04-06 22:49:02.350442 token_throttler-1.5.1/src/token_throttler/throttler_config.py
+-rw-r--r--   0        0        0     1169 2024-04-06 21:51:15.802737 token_throttler-1.5.1/src/token_throttler/token_bucket.py
+-rw-r--r--   0        0        0     4486 2024-04-06 22:44:31.266696 token_throttler-1.5.1/src/token_throttler/token_throttler.py
+-rw-r--r--   0        0        0     4255 2024-04-06 22:44:53.236365 token_throttler-1.5.1/src/token_throttler/token_throttler_async.py
+-rw-r--r--   0        0        0     1945 2024-03-20 23:23:08.721746 token_throttler-1.5.1/src/token_throttler/validate.py
+-rw-r--r--   0        0        0     9988 1970-01-01 00:00:00.000000 token_throttler-1.5.1/PKG-INFO
```

### Comparing `token_throttler-1.5.0/LICENSE` & `token_throttler-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `token_throttler-1.5.0/README.md` & `token_throttler-1.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 <a name="installation"></a>
 ## 1. Installation
 
 Token throttler is available on PyPI:
 ```console 
 $ python -m pip install token-throttler
 ```
-Token throttler officially supports Python >= 3.7.
+Token throttler officially supports Python >= 3.8.
 
 *NOTE*: Depending on the storage engine you pick, you can install token throttler with extras:
 ```console 
 $ python -m pip install token-throttler[redis]
 ```
 
 <a name="features"></a>
@@ -58,31 +58,33 @@
 <a name="usage-manual"></a>
 ### 1) Manual usage example:
 
 ```python
 from token_throttler import TokenBucket, TokenThrottler
 from token_throttler.storage import RuntimeStorage
 
-throttler: TokenThrottler = TokenThrottler(cost=1, storage=RuntimeStorage())
-throttler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=10, max_tokens=10))
-throttler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=30, max_tokens=20))
+throttler: TokenThrottler = TokenThrottler(1, RuntimeStorage())
+throttler.add_bucket("hello_world", TokenBucket(10, 10))
+throttler.add_bucket("hello_world", TokenBucket(30, 20))
 
 
 def hello_world() -> None:
     print("Hello World")
 
 
 for i in range(10):
-    throttler.consume(identifier="hello_world")
+    throttler.consume("hello_world")
     hello_world()
 
-if throttler.consume(identifier="hello_world"):
+if throttler.consume("hello_world"):
     hello_world()
 else:
-    print("bucket_one ran out of tokens")
+    print(
+        f"bucket_one ran out of tokens, retry in: {throttler.wait_time('hello_world')}"
+    )
 ```
 
 <a name="usage-decorator"></a>
 ### 2) Decorator usage example:
 
 ```python
 from token_throttler import TokenBucket, TokenThrottler, TokenThrottlerException
@@ -100,15 +102,17 @@
 
 for i in range(10):
     hello_world()
 
 try:
     hello_world()
 except TokenThrottlerException:
-    print("bucket_one ran out of tokens")
+    print(
+        f"bucket_one ran out of tokens, retry in: {throttler.wait_time('hello_world')}"
+    )
 ```
 
 <a name="usage-fastapi"></a>
 ### 3) FastAPI usage example:
 
 ```python
 from fastapi import Depends, FastAPI, Request
```

### Comparing `token_throttler-1.5.0/pyproject.toml` & `token_throttler-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "token-throttler"
-version = "1.5.0"
+version = "1.5.1"
 description = "Token throttler is an extendable rate-limiting library somewhat based on a token bucket algorithm"
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = [
         "Vojko Pribudić <dmanthing@gmail.com>",
         "Rino Dugonjić <dugonjic.rino@gmail.com>",
 ]
 repository = "https://gitlab.com/vojko.pribudic/token-throttler"
```

### Comparing `token_throttler-1.5.0/src/token_throttler/ext/fastapi.py` & `token_throttler-1.5.1/src/token_throttler/ext/fastapi.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.5.0/src/token_throttler/storage/bucket_storage.py` & `token_throttler-1.5.1/src/token_throttler/storage/bucket_storage.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.5.0/src/token_throttler/storage/bucket_storage_async.py` & `token_throttler-1.5.1/src/token_throttler/storage/bucket_storage_async.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.5.0/src/token_throttler/storage/redis/redis_storage.py` & `token_throttler-1.5.1/src/token_throttler/storage/redis/redis_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         bucket: Union[bytes, None] = self.redis.get(cache_key)
         if not bucket:
             return None
         return pickle.loads(bucket)
 
     def get_all_buckets(self, identifier: str) -> Union[Dict[str, TokenBucket], None]:
         buckets: Dict[str, TokenBucket] = {}
-        stored_buckets: Dict[str, str] = self.buckets.get(identifier, None)
+        stored_buckets: Union[Dict[str, str], None] = self.buckets.get(identifier, None)
         if not stored_buckets:
             return None
         for bucket_key in stored_buckets:
             bucket: Union[TokenBucket, None] = self.get_bucket(identifier, bucket_key)
             if not bucket:  # pragma: no cover
                 continue
             buckets[bucket_key] = bucket
```

### Comparing `token_throttler-1.5.0/src/token_throttler/storage/redis/redis_storage_async.py` & `token_throttler-1.5.1/src/token_throttler/storage/redis/redis_storage_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             return None
         return pickle.loads(bucket)
 
     async def get_all_buckets(
         self, identifier: str
     ) -> Union[Dict[str, TokenBucket], None]:
         buckets: Dict[str, TokenBucket] = {}
-        stored_buckets: Dict[str, str] = self.buckets.get(identifier, None)
+        stored_buckets: Union[Dict[str, str], None] = self.buckets.get(identifier, None)
         if not stored_buckets:
             return None
         for bucket_key in stored_buckets:
             bucket: Union[TokenBucket, None] = await self.get_bucket(
                 identifier, bucket_key
             )
             if not bucket:  # pragma: no cover
```

### Comparing `token_throttler-1.5.0/src/token_throttler/storage/runtime_storage.py` & `token_throttler-1.5.1/src/token_throttler/storage/runtime_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,14 +33,13 @@
         current_time: float = datetime.now(timezone.utc).timestamp()
 
         if (current_time < bucket.last_replenished) or (
             current_time - bucket.last_replenished < bucket.replenish_time
         ):
             return
 
-        bucket.last_replenished = current_time
-        bucket.tokens = bucket.max_tokens
+        bucket.replenish()
 
     def consume(self, identifier: str, bucket_key: str) -> bool:
         bucket: TokenBucket = self.buckets[identifier][str(bucket_key)]
         self.replenish(bucket)
         return bucket.consume()
```

### Comparing `token_throttler-1.5.0/src/token_throttler/throttler_config.py` & `token_throttler-1.5.1/src/token_throttler/throttler_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             self.set(config)
 
     def _configure(self, config: Dict) -> None:
         for key, value in config.items():
             if not hasattr(self, key):
                 return
             attr: Any = getattr(self, key)
-            if type(attr) != type(value):
+            if type(attr) is not type(value):
                 raise TypeError(f"Invalid type for configuration parameter `{key}`")
             setattr(self, key, value)
 
     def set(self, config: Dict) -> None:
         if config is None or not config:
             raise ValueError(f"Invalid configuration provided: {config}")
         if not isinstance(config, Dict):
```

### Comparing `token_throttler-1.5.0/src/token_throttler/token_bucket.py` & `token_throttler-1.5.1/src/token_throttler/token_bucket.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,13 +11,27 @@
         self.tokens: int = max_tokens
         self.last_replenished: float = datetime.now(timezone.utc).timestamp()
         self.identifier: Union[str, None] = None
         self.cost: int = 0
         validate_max_tokens(self.max_tokens)
         validate_replenish_time(self.replenish_time)
 
+    @property
+    def wait_time(self) -> int:
+        if self.tokens < self.cost:
+            return round(
+                self.last_replenished
+                + self.replenish_time
+                - datetime.now(timezone.utc).timestamp()
+            )
+        return 0
+
     def consume(self) -> bool:
         if self.tokens < self.cost:
             return False
 
         self.tokens -= self.cost
         return True
+
+    def replenish(self) -> None:
+        self.last_replenished = datetime.now(timezone.utc).timestamp()
+        self.tokens = self.max_tokens
```

### Comparing `token_throttler-1.5.0/src/token_throttler/token_throttler.py` & `token_throttler-1.5.1/src/token_throttler/token_throttler_async.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,128 +1,127 @@
-import asyncio
-from threading import Lock
+from asyncio import Lock
 from typing import Any, Callable, Dict, List, Union
 
 from . import (
     ThrottlerConfig,
     ThrottlerConfigGlobal,
     TokenBucket,
     TokenThrottlerException,
     default_config,
 )
-from .storage import BucketStorage
+from .storage import BucketStorageAsync
 from .validate import (
     validate_bucket,
     validate_bucket_config,
     validate_bucket_key,
     validate_cost,
     validate_identifier,
     validate_storage,
 )
 
 
-class TokenThrottler:
+class TokenThrottlerAsync:
     def __init__(
         self,
         cost: int,
-        storage: BucketStorage,
+        storage: BucketStorageAsync,
         config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = default_config,
     ) -> None:
         self._cost: int = cost
-        self._storage: BucketStorage = storage
+        self._storage: BucketStorageAsync = storage
         self._lock: Lock = Lock()
         self._config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = config
         validate_cost(self._cost)
-        validate_storage(self._storage, BucketStorage)
+        validate_storage(self._storage, BucketStorageAsync)
+
+    async def wait_time(self, identifier: str) -> int:
+        buckets: Union[Dict[str, TokenBucket], None] = await self.get_all_buckets(
+            identifier
+        )
+        if not buckets:
+            return 0
+        return max([b.wait_time for b in buckets.values() if b.wait_time > 0])
 
     def _add_identifier(self, identifier: str) -> None:
         validate_identifier(identifier)
         if identifier not in self._storage.buckets:
             self._storage.buckets[identifier] = {}
 
-    def get_bucket(self, identifier: str, bucket_key: str) -> Union[TokenBucket, None]:
+    async def get_bucket(
+        self, identifier: str, bucket_key: str
+    ) -> Union[TokenBucket, None]:
         validate_identifier(identifier)
         validate_bucket_key(bucket_key)
-        return self._storage.get_bucket(identifier, bucket_key)
+        return await self._storage.get_bucket(identifier, bucket_key)
 
-    def get_all_buckets(self, identifier: str) -> Union[Dict[str, TokenBucket], None]:
+    async def get_all_buckets(
+        self, identifier: str
+    ) -> Union[Dict[str, TokenBucket], None]:
         validate_identifier(identifier)
-        return self._storage.get_all_buckets(identifier)
+        return await self._storage.get_all_buckets(identifier)
 
-    def add_bucket(self, identifier: str, bucket: TokenBucket) -> None:
+    async def add_bucket(self, identifier: str, bucket: TokenBucket) -> None:
         validate_bucket(bucket, TokenBucket)
         self._add_identifier(identifier)
         bucket.identifier = identifier
         bucket.cost = self._cost
-        self._storage.add_bucket(bucket)
+        await self._storage.add_bucket(bucket)
 
-    def remove_bucket(self, identifier: str, bucket_key: str) -> None:
+    async def remove_bucket(self, identifier: str, bucket_key: str) -> None:
         validate_identifier(identifier)
         validate_bucket_key(bucket_key)
-        self._storage.remove_bucket(identifier, bucket_key)
+        await self._storage.remove_bucket(identifier, bucket_key)
 
-    def remove_all_buckets(self, identifier: str) -> None:
+    async def remove_all_buckets(self, identifier: str) -> None:
         validate_identifier(identifier)
-        self._storage.remove_all_buckets(identifier)
+        await self._storage.remove_all_buckets(identifier)
 
-    def add_from_dict(
+    async def add_from_dict(
         self,
         identifier: str,
         bucket_config: List[Dict[str, Any]],
         remove_old_buckets: bool = False,
     ) -> None:
         validate_bucket_config(bucket_config, TokenBucket)
         self._add_identifier(identifier)
 
         if remove_old_buckets:
-            self.remove_all_buckets(identifier)
+            await self.remove_all_buckets(identifier)
 
         for bucket in bucket_config:
             token_bucket: TokenBucket = TokenBucket(
                 replenish_time=int(bucket["replenish_time"]),
                 max_tokens=int(bucket["max_tokens"]),
             )
-            self.add_bucket(identifier, token_bucket)
+            await self.add_bucket(identifier, token_bucket)
 
-    def consume(self, identifier: str) -> bool:
+    async def consume(self, identifier: str) -> bool:
         return_value: bool = True
         validate_identifier(identifier)
         if identifier not in self._storage.buckets.keys():
             if not self._config.IDENTIFIER_FAIL_SAFE:
                 raise KeyError(f"Invalid identifier: `{identifier}`")
             else:
                 return return_value
 
         if self._config.ENABLE_THREAD_LOCK:
-            self._lock.acquire()
+            await self._lock.acquire()
 
-        if not all(
-            self._storage.consume(identifier, str(bucket_key))
-            for bucket_key in self._storage.buckets[identifier].keys()
-        ):
-            return_value = False
+        for bucket_key in self._storage.buckets[identifier].keys():
+            if not await self._storage.consume(identifier, str(bucket_key)):
+                return_value = False
 
         if self._lock.locked():
             self._lock.release()
 
         return return_value
 
     def enable(self, identifier: str) -> Any:
         def wrapper(fn: Callable):
-            if not asyncio.iscoroutinefunction(fn):
-
-                def inner(*args, **kwargs):
-                    if not self.consume(identifier):
-                        raise TokenThrottlerException()
-                    return fn(*args, **kwargs)
-
-                return inner
-            else:
-
-                async def inner(*args, **kwargs):
-                    if not self.consume(identifier):
-                        raise TokenThrottlerException()
-                    return await fn(*args, **kwargs)
+            async def inner(*args, **kwargs):
+                if not await self.consume(identifier):
+                    raise TokenThrottlerException()
+                return await fn(*args, **kwargs)
 
-                return inner
+            return inner
 
         return wrapper
```

### Comparing `token_throttler-1.5.0/src/token_throttler/token_throttler_async.py` & `token_throttler-1.5.1/src/token_throttler/token_throttler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,119 +1,135 @@
+import asyncio
 from threading import Lock
 from typing import Any, Callable, Dict, List, Union
 
 from . import (
     ThrottlerConfig,
     ThrottlerConfigGlobal,
     TokenBucket,
     TokenThrottlerException,
     default_config,
 )
-from .storage import BucketStorageAsync
+from .storage import BucketStorage
 from .validate import (
     validate_bucket,
     validate_bucket_config,
     validate_bucket_key,
     validate_cost,
     validate_identifier,
     validate_storage,
 )
 
 
-class TokenThrottlerAsync:
+class TokenThrottler:
     def __init__(
         self,
         cost: int,
-        storage: BucketStorageAsync,
+        storage: BucketStorage,
         config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = default_config,
     ) -> None:
         self._cost: int = cost
-        self._storage: BucketStorageAsync = storage
+        self._storage: BucketStorage = storage
         self._lock: Lock = Lock()
         self._config: Union[ThrottlerConfig, ThrottlerConfigGlobal] = config
         validate_cost(self._cost)
-        validate_storage(self._storage, BucketStorageAsync)
+        validate_storage(self._storage, BucketStorage)
+
+    def wait_time(self, identifier: str) -> int:
+        buckets: Union[Dict[str, TokenBucket], None] = self.get_all_buckets(identifier)
+        if not buckets:
+            return 0
+        wait_times: list = [b.wait_time for b in buckets.values() if b.wait_time > 0]
+        return max(wait_times) if wait_times else 0
 
     def _add_identifier(self, identifier: str) -> None:
         validate_identifier(identifier)
         if identifier not in self._storage.buckets:
             self._storage.buckets[identifier] = {}
 
-    async def get_bucket(
-        self, identifier: str, bucket_key: str
-    ) -> Union[TokenBucket, None]:
+    def get_bucket(self, identifier: str, bucket_key: str) -> Union[TokenBucket, None]:
         validate_identifier(identifier)
         validate_bucket_key(bucket_key)
-        return await self._storage.get_bucket(identifier, bucket_key)
+        return self._storage.get_bucket(identifier, bucket_key)
 
-    async def get_all_buckets(
-        self, identifier: str
-    ) -> Union[Dict[str, TokenBucket], None]:
+    def get_all_buckets(self, identifier: str) -> Union[Dict[str, TokenBucket], None]:
         validate_identifier(identifier)
-        return await self._storage.get_all_buckets(identifier)
+        return self._storage.get_all_buckets(identifier)
 
-    async def add_bucket(self, identifier: str, bucket: TokenBucket) -> None:
+    def add_bucket(self, identifier: str, bucket: TokenBucket) -> None:
         validate_bucket(bucket, TokenBucket)
         self._add_identifier(identifier)
         bucket.identifier = identifier
         bucket.cost = self._cost
-        await self._storage.add_bucket(bucket)
+        self._storage.add_bucket(bucket)
 
-    async def remove_bucket(self, identifier: str, bucket_key: str) -> None:
+    def remove_bucket(self, identifier: str, bucket_key: str) -> None:
         validate_identifier(identifier)
         validate_bucket_key(bucket_key)
-        await self._storage.remove_bucket(identifier, bucket_key)
+        self._storage.remove_bucket(identifier, bucket_key)
 
-    async def remove_all_buckets(self, identifier: str) -> None:
+    def remove_all_buckets(self, identifier: str) -> None:
         validate_identifier(identifier)
-        await self._storage.remove_all_buckets(identifier)
+        self._storage.remove_all_buckets(identifier)
 
-    async def add_from_dict(
+    def add_from_dict(
         self,
         identifier: str,
         bucket_config: List[Dict[str, Any]],
         remove_old_buckets: bool = False,
     ) -> None:
         validate_bucket_config(bucket_config, TokenBucket)
         self._add_identifier(identifier)
 
         if remove_old_buckets:
-            await self.remove_all_buckets(identifier)
+            self.remove_all_buckets(identifier)
 
         for bucket in bucket_config:
             token_bucket: TokenBucket = TokenBucket(
                 replenish_time=int(bucket["replenish_time"]),
                 max_tokens=int(bucket["max_tokens"]),
             )
-            await self.add_bucket(identifier, token_bucket)
+            self.add_bucket(identifier, token_bucket)
 
-    async def consume(self, identifier: str) -> bool:
+    def consume(self, identifier: str) -> bool:
         return_value: bool = True
         validate_identifier(identifier)
         if identifier not in self._storage.buckets.keys():
             if not self._config.IDENTIFIER_FAIL_SAFE:
                 raise KeyError(f"Invalid identifier: `{identifier}`")
             else:
                 return return_value
 
         if self._config.ENABLE_THREAD_LOCK:
             self._lock.acquire()
 
-        for bucket_key in self._storage.buckets[identifier].keys():
-            if not await self._storage.consume(identifier, str(bucket_key)):
-                return_value = False
+        if not all(
+            self._storage.consume(identifier, str(bucket_key))
+            for bucket_key in self._storage.buckets[identifier].keys()
+        ):
+            return_value = False
 
         if self._lock.locked():
             self._lock.release()
 
         return return_value
 
     def enable(self, identifier: str) -> Any:
         def wrapper(fn: Callable):
-            async def inner(*args, **kwargs):
-                if not await self.consume(identifier):
-                    raise TokenThrottlerException()
-                return await fn(*args, **kwargs)
+            if not asyncio.iscoroutinefunction(fn):
+
+                def inner(*args, **kwargs):
+                    if not self.consume(identifier):
+                        raise TokenThrottlerException()
+                    return fn(*args, **kwargs)
+
+                return inner
+            else:
+
+                async def inner(*args, **kwargs):
+                    if not self.consume(identifier):
+                        raise TokenThrottlerException()
+                    return await fn(*args, **kwargs)
 
-            return inner
+                return inner
 
         return wrapper
```

### Comparing `token_throttler-1.5.0/src/token_throttler/validate.py` & `token_throttler-1.5.1/src/token_throttler/validate.py`

 * *Files identical despite different names*

### Comparing `token_throttler-1.5.0/PKG-INFO` & `token_throttler-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: token-throttler
-Version: 1.5.0
+Version: 1.5.1
 Summary: Token throttler is an extendable rate-limiting library somewhat based on a token bucket algorithm
 Home-page: https://gitlab.com/vojko.pribudic/token-throttler
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
@@ -59,15 +59,15 @@
 <a name="installation"></a>
 ## 1. Installation
 
 Token throttler is available on PyPI:
 ```console 
 $ python -m pip install token-throttler
 ```
-Token throttler officially supports Python >= 3.7.
+Token throttler officially supports Python >= 3.8.
 
 *NOTE*: Depending on the storage engine you pick, you can install token throttler with extras:
 ```console 
 $ python -m pip install token-throttler[redis]
 ```
 
 <a name="features"></a>
@@ -93,31 +93,33 @@
 <a name="usage-manual"></a>
 ### 1) Manual usage example:
 
 ```python
 from token_throttler import TokenBucket, TokenThrottler
 from token_throttler.storage import RuntimeStorage
 
-throttler: TokenThrottler = TokenThrottler(cost=1, storage=RuntimeStorage())
-throttler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=10, max_tokens=10))
-throttler.add_bucket(identifier="hello_world", bucket=TokenBucket(replenish_time=30, max_tokens=20))
+throttler: TokenThrottler = TokenThrottler(1, RuntimeStorage())
+throttler.add_bucket("hello_world", TokenBucket(10, 10))
+throttler.add_bucket("hello_world", TokenBucket(30, 20))
 
 
 def hello_world() -> None:
     print("Hello World")
 
 
 for i in range(10):
-    throttler.consume(identifier="hello_world")
+    throttler.consume("hello_world")
     hello_world()
 
-if throttler.consume(identifier="hello_world"):
+if throttler.consume("hello_world"):
     hello_world()
 else:
-    print("bucket_one ran out of tokens")
+    print(
+        f"bucket_one ran out of tokens, retry in: {throttler.wait_time('hello_world')}"
+    )
 ```
 
 <a name="usage-decorator"></a>
 ### 2) Decorator usage example:
 
 ```python
 from token_throttler import TokenBucket, TokenThrottler, TokenThrottlerException
@@ -135,15 +137,17 @@
 
 for i in range(10):
     hello_world()
 
 try:
     hello_world()
 except TokenThrottlerException:
-    print("bucket_one ran out of tokens")
+    print(
+        f"bucket_one ran out of tokens, retry in: {throttler.wait_time('hello_world')}"
+    )
 ```
 
 <a name="usage-fastapi"></a>
 ### 3) FastAPI usage example:
 
 ```python
 from fastapi import Depends, FastAPI, Request
```

