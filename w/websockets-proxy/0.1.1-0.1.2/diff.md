# Comparing `tmp/websockets_proxy-0.1.1.tar.gz` & `tmp/websockets_proxy-0.1.2.tar.gz`

## Comparing `websockets_proxy-0.1.1.tar` & `websockets_proxy-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/requirements.txt
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/websockets_proxy/__init__.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/websockets_proxy/websockets_proxy.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/LICENSE
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/README.md
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5723 2020-02-02 00:00:00.000000 websockets_proxy-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/requirements.txt
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/websockets_proxy/__init__.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/websockets_proxy/websockets_proxy.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/README.md
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5924 2020-02-02 00:00:00.000000 websockets_proxy-0.1.2/PKG-INFO
```

### Comparing `websockets_proxy-0.1.1/websockets_proxy/websockets_proxy.py` & `websockets_proxy-0.1.2/websockets_proxy/websockets_proxy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional, Union
 from urllib.parse import urlparse
 
-import websockets
 from websockets.legacy.client import connect
 from python_socks.async_.asyncio import Proxy
 
 
 class ProxyConnect(connect):
     def __init__(  # noqa
             self,
@@ -41,26 +40,29 @@
         # pass it to the super().__init__ call
         self.__kwargs = kwargs
         # We deliberately don't call the super().__init__ constructor method YET!
 
     def set_proxy(self, proxy: Proxy) -> None:
         self.__proxy = proxy
 
-    async def __aenter__(self) -> websockets.WebSocketClientProtocol:
+    async def __await_impl_proxy__(self):
         # creating patched socket
         sock = await self.__proxy.connect(
             dest_host=self.__host,
             dest_port=self.__port,
             timeout=self.__proxy_conn_timeout
         )
         self.__kwargs["sock"] = sock
         # HACK: THE super().__init__ IS DELIBERATELY CALLED HERE!
         # It is because we need an already connected socket object inside the constructor,
         # but we've only just got it inside of this method
         super().__init__(self.uri, **self.__kwargs)  # noqa
-        proto = await super().__aenter__()
+        proto = await super().__await_impl_timeout__()
         return proto
 
+    def __await__(self):
+        return self.__await_impl_proxy__().__await__()
+
 
 proxy_connect = ProxyConnect
 
 __all__ = ["proxy_connect", "Proxy"]
```

### Comparing `websockets_proxy-0.1.1/LICENSE` & `websockets_proxy-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `websockets_proxy-0.1.1/README.md` & `websockets_proxy-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 ```python
 import asyncio
 
 from aiohttp import web, WSMsgType, WSMessage
 
 
 HOST = '0.0.0.0'
-PORT = 54321
+PORT = 9999
 
 app = web.Application()
 
 
 async def websocket_handler(request: web.Request) -> web.StreamResponse:
     ws = web.WebSocketResponse()
     await ws.prepare(request)
@@ -93,19 +93,27 @@
 
 async def main():
     async with connect(CHECKER_URL) as ws:
         async for msg in ws:
             ip_no_proxy = msg
             print("Your IP:", ip_no_proxy)
     print('.')
-    # be sure to create your "Proxy" objects inside an async function 
-    proxy = Proxy.from_url("socks5://username:password@address:port")
+    # be sure to create your "Proxy" objects inside an async function
+    proxy = Proxy.from_url("http://login:password@address:port")
     async with proxy_connect(CHECKER_URL, proxy=proxy) as ws:
         async for msg in ws:
             ip_with_proxy = msg
-            print("Proxy IP", ip_with_proxy)
+            print("(async with) Proxy IP", ip_with_proxy)
+    print('.')
+
+    ws = await proxy_connect(CHECKER_URL, proxy=proxy)
+    async for msg in ws:
+        ip_with_proxy = msg
+        print("(await) Proxy IP", ip_with_proxy)
+    await ws.close()
     print('.')
 
 
 if __name__ == "__main__":
     asyncio.run(main())
+
 ```
```

### Comparing `websockets_proxy-0.1.1/pyproject.toml` & `websockets_proxy-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "websockets_proxy"
-version = "0.1.1"
+version = "0.1.2"
 requires-python = ">= 3.8"
 authors = [
     {name = "Andrei Karavatski", email = "verolomnyy@gmail.com"}
 ]
 maintainers = [
     {name = "Andrei Karavatski", email = "verolomnyy@gmail.com"}
 ]
```

### Comparing `websockets_proxy-0.1.1/PKG-INFO` & `websockets_proxy-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: websockets_proxy
-Version: 0.1.1
+Version: 0.1.2
 Summary: Connect to websockets through a proxy server.
 Project-URL: Homepage, https://github.com/racinette/websockets_proxy
 Project-URL: Issues, https://github.com/racinette/websockets_proxy/issues
 Author-email: Andrei Karavatski <verolomnyy@gmail.com>
 Maintainer-email: Andrei Karavatski <verolomnyy@gmail.com>
 License: MIT License
         
@@ -95,15 +95,15 @@
 ```python
 import asyncio
 
 from aiohttp import web, WSMsgType, WSMessage
 
 
 HOST = '0.0.0.0'
-PORT = 54321
+PORT = 9999
 
 app = web.Application()
 
 
 async def websocket_handler(request: web.Request) -> web.StreamResponse:
     ws = web.WebSocketResponse()
     await ws.prepare(request)
@@ -148,19 +148,27 @@
 
 async def main():
     async with connect(CHECKER_URL) as ws:
         async for msg in ws:
             ip_no_proxy = msg
             print("Your IP:", ip_no_proxy)
     print('.')
-    # be sure to create your "Proxy" objects inside an async function 
-    proxy = Proxy.from_url("socks5://username:password@address:port")
+    # be sure to create your "Proxy" objects inside an async function
+    proxy = Proxy.from_url("http://login:password@address:port")
     async with proxy_connect(CHECKER_URL, proxy=proxy) as ws:
         async for msg in ws:
             ip_with_proxy = msg
-            print("Proxy IP", ip_with_proxy)
+            print("(async with) Proxy IP", ip_with_proxy)
+    print('.')
+
+    ws = await proxy_connect(CHECKER_URL, proxy=proxy)
+    async for msg in ws:
+        ip_with_proxy = msg
+        print("(await) Proxy IP", ip_with_proxy)
+    await ws.close()
     print('.')
 
 
 if __name__ == "__main__":
     asyncio.run(main())
+
 ```
```

