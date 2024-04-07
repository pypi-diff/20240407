# Comparing `tmp/vxutils-20240403.tar.gz` & `tmp/vxutils-20240406.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vxutils-20240403.tar", max compression
+gzip compressed data, was "vxutils-20240406.tar", max compression
```

## Comparing `vxutils-20240403.tar` & `vxutils-20240406.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1998 2024-04-03 01:53:54.415891 vxutils-20240403/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240403/README.md
--rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240403/src/vxsched/__init__.py
--rw-r--r--   0        0        0     1370 2024-03-31 05:45:50.712223 vxutils-20240403/src/vxsched/__main__.py
--rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240403/src/vxsched/core.py
--rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240403/src/vxsched/event.py
--rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240403/src/vxsched/py.typed
--rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240403/src/vxsched/subpubs.py
--rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240403/src/vxutils/__init__.py
--rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240403/src/vxutils/context.py
--rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240403/src/vxutils/convertors.py
--rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240403/src/vxutils/datamodel/__init__.py
--rw-r--r--   0        0        0     4214 2024-02-18 02:09:20.092983 vxutils-20240403/src/vxutils/datamodel/adapter.py
--rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240403/src/vxutils/datamodel/core.py
--rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240403/src/vxutils/datamodel/dborm.py
--rw-r--r--   0        0        0     8716 2024-04-03 01:52:41.512838 vxutils-20240403/src/vxutils/decorators.py
--rw-r--r--   0        0        0     9568 2024-04-03 04:14:10.732009 vxutils-20240403/src/vxutils/dtutils.py
--rw-r--r--   0        0        0     7344 2024-03-31 03:46:11.067709 vxutils-20240403/src/vxutils/logger.py
--rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240403/src/vxutils/networking/requests.py
--rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240403/src/vxutils/networking/wechat.py
--rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240403/src/vxutils/provider.py
--rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240403/src/vxutils/py.typed
--rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240403/src/vxutils/typehints.py
--rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240403/PKG-INFO
+-rw-r--r--   0        0        0     1998 2024-04-07 01:17:45.738343 vxutils-20240406/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-02-28 02:40:58.487414 vxutils-20240406/README.md
+-rw-r--r--   0        0        0      421 2024-04-02 02:11:16.355963 vxutils-20240406/src/vxsched/__init__.py
+-rw-r--r--   0        0        0     1370 2024-03-31 05:45:50.712223 vxutils-20240406/src/vxsched/__main__.py
+-rw-r--r--   0        0        0     7776 2024-03-15 02:21:02.576581 vxutils-20240406/src/vxsched/core.py
+-rw-r--r--   0        0        0    11734 2024-03-07 05:59:56.919198 vxutils-20240406/src/vxsched/event.py
+-rw-r--r--   0        0        0        0 2024-03-07 06:18:59.347092 vxutils-20240406/src/vxsched/py.typed
+-rw-r--r--   0        0        0     1202 2024-04-02 02:11:10.194079 vxutils-20240406/src/vxsched/subpubs.py
+-rw-r--r--   0        0        0     1375 2024-04-03 04:23:00.014767 vxutils-20240406/src/vxutils/__init__.py
+-rw-r--r--   0        0        0     3738 2024-03-31 05:45:39.670502 vxutils-20240406/src/vxutils/context.py
+-rw-r--r--   0        0        0     9225 2024-02-20 02:25:26.235753 vxutils-20240406/src/vxutils/convertors.py
+-rw-r--r--   0        0        0        0 2024-02-17 13:24:20.316286 vxutils-20240406/src/vxutils/datamodel/__init__.py
+-rw-r--r--   0        0        0     4214 2024-02-18 02:09:20.092983 vxutils-20240406/src/vxutils/datamodel/adapter.py
+-rw-r--r--   0        0        0     2369 2024-03-07 04:24:54.189680 vxutils-20240406/src/vxutils/datamodel/core.py
+-rw-r--r--   0        0        0    15247 2024-03-12 05:04:59.968100 vxutils-20240406/src/vxutils/datamodel/dborm.py
+-rw-r--r--   0        0        0     9071 2024-04-07 01:14:57.773870 vxutils-20240406/src/vxutils/decorators.py
+-rw-r--r--   0        0        0     9568 2024-04-07 01:16:17.431751 vxutils-20240406/src/vxutils/dtutils.py
+-rw-r--r--   0        0        0     7344 2024-03-31 03:46:11.067709 vxutils-20240406/src/vxutils/logger.py
+-rw-r--r--   0        0        0    14529 2024-02-20 08:56:31.979240 vxutils-20240406/src/vxutils/networking/requests.py
+-rw-r--r--   0        0        0     7987 2024-03-31 01:34:06.580192 vxutils-20240406/src/vxutils/networking/wechat.py
+-rw-r--r--   0        0        0     6173 2024-03-15 02:47:00.420052 vxutils-20240406/src/vxutils/provider.py
+-rw-r--r--   0        0        0        0 2024-02-15 15:46:34.000000 vxutils-20240406/src/vxutils/py.typed
+-rw-r--r--   0        0        0      446 2024-03-10 03:13:04.515372 vxutils-20240406/src/vxutils/typehints.py
+-rw-r--r--   0        0        0     1067 1970-01-01 00:00:00.000000 vxutils-20240406/PKG-INFO
```

### Comparing `vxutils-20240403/pyproject.toml` & `vxutils-20240406/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vxutils"
-version = "20240403"
+version = "20240406"
 description = "python 常用工具箱"
 license = "MIT"
 authors = ["vex1023 <vex1023@qq.com>"]
 homepage = "https://gitee.com/vxquant/vxutils"
 keywords = ["quant", "tools"]
 readme = "README.md"
```

### Comparing `vxutils-20240403/src/vxsched/__main__.py` & `vxutils-20240406/src/vxsched/__main__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxsched/core.py` & `vxutils-20240406/src/vxsched/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxsched/event.py` & `vxutils-20240406/src/vxsched/event.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxsched/subpubs.py` & `vxutils-20240406/src/vxsched/subpubs.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/__init__.py` & `vxutils-20240406/src/vxutils/__init__.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/context.py` & `vxutils-20240406/src/vxutils/context.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/convertors.py` & `vxutils-20240406/src/vxutils/convertors.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/datamodel/adapter.py` & `vxutils-20240406/src/vxutils/datamodel/adapter.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/datamodel/core.py` & `vxutils-20240406/src/vxutils/datamodel/core.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/datamodel/dborm.py` & `vxutils-20240406/src/vxutils/datamodel/dborm.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/decorators.py` & `vxutils-20240406/src/vxutils/decorators.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 各类型的decorator
 """
 
 import signal
 import time
 import logging
 
-from typing import Callable, Union, Tuple, Any, Type, Literal
+from typing import Callable, Union, Tuple, Any, Type, Literal, Optional
 from concurrent.futures import ThreadPoolExecutor, Future
 from multiprocessing import Lock, Semaphore
 from functools import wraps
 
 __all__ = [
     "retry",
     "timeit",
@@ -311,15 +311,32 @@
         try:
             cls.__executor__.shutdown()
             cls.__executor__ = executor
         except Exception as err:
             logging.error("set executor error: %s", err, exc_info=True)
 
 
-async_map = async_task.__executor__.map
+def async_map(
+    func: Callable[..., Any],
+    *iterables: Any,
+    timeout: Optional[float] = None,
+    chunsize: int = 1,
+) -> Any:
+    """异步map提交任务
+
+    Arguments:
+        func {Callable[..., Any]} -- 运行func
+
+    Returns:
+        Any -- 返回值
+    """
+    return async_task.__executor__.map(
+        func, *iterables, timeout=timeout, chunksize=chunsize
+    )
+
 
 if __name__ == "__main__":
 
     @async_task()
     def test(i: int) -> int:
         print("test", i, end="\n")
         time.sleep(1)
```

### Comparing `vxutils-20240403/src/vxutils/dtutils.py` & `vxutils-20240406/src/vxutils/dtutils.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/logger.py` & `vxutils-20240406/src/vxutils/logger.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/networking/requests.py` & `vxutils-20240406/src/vxutils/networking/requests.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/networking/wechat.py` & `vxutils-20240406/src/vxutils/networking/wechat.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/src/vxutils/provider.py` & `vxutils-20240406/src/vxutils/provider.py`

 * *Files identical despite different names*

### Comparing `vxutils-20240403/PKG-INFO` & `vxutils-20240406/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vxutils
-Version: 20240403
+Version: 20240406
 Summary: python 常用工具箱
 Home-page: https://gitee.com/vxquant/vxutils
 License: MIT
 Keywords: quant,tools
 Author: vex1023
 Author-email: vex1023@qq.com
 Requires-Python: >=3.8,<4.0
```

