# Comparing `tmp/WebexCompassSDK-44.3.4.tar.gz` & `tmp/WebexCompassSDK-44.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WebexCompassSDK-44.3.4.tar", last modified: Mon Feb  5 10:14:51 2024, max compression
+gzip compressed data, was "WebexCompassSDK-44.4.1.tar", last modified: Sun Apr  7 06:43:57 2024, max compression
```

## Comparing `WebexCompassSDK-44.3.4.tar` & `WebexCompassSDK-44.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-02-05 10:14:51.512687 WebexCompassSDK-44.3.4/
--rw-r--r--   0 wangyongzhou   (501) staff       (20)      159 2024-02-05 10:14:51.512436 WebexCompassSDK-44.3.4/PKG-INFO
--rw-r--r--   0 wangyongzhou   (501) staff       (20)     2544 2024-02-05 09:05:23.000000 WebexCompassSDK-44.3.4/README.md
--rw-r--r--   0 wangyongzhou   (501) staff       (20)       38 2024-02-05 10:14:51.512734 WebexCompassSDK-44.3.4/setup.cfg
--rw-r--r--   0 wangyongzhou   (501) staff       (20)      463 2024-02-05 10:14:28.000000 WebexCompassSDK-44.3.4/setup.py
-drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-02-05 10:14:51.510304 WebexCompassSDK-44.3.4/src/
-drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-02-05 10:14:51.511379 WebexCompassSDK-44.3.4/src/WebexCompassSDK/
--rw-r--r--   0 wangyongzhou   (501) staff       (20)     7206 2024-02-05 10:07:06.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK/WebexCompassClient.py
--rw-r--r--   0 wangyongzhou   (501) staff       (20)        0 2024-02-05 09:05:23.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK/__init__.py
--rw-r--r--   0 wangyongzhou   (501) staff       (20)       24 2024-02-05 10:14:41.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK/version.py
--rw-r--r--   0 wangyongzhou   (501) staff       (20)     3601 2024-02-05 09:05:23.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK/ws.py
-drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-02-05 10:14:51.512201 WebexCompassSDK-44.3.4/src/WebexCompassSDK.egg-info/
--rw-r--r--   0 wangyongzhou   (501) staff       (20)      159 2024-02-05 10:14:51.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK.egg-info/PKG-INFO
--rw-r--r--   0 wangyongzhou   (501) staff       (20)      321 2024-02-05 10:14:51.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK.egg-info/SOURCES.txt
--rw-r--r--   0 wangyongzhou   (501) staff       (20)        1 2024-02-05 10:14:51.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK.egg-info/dependency_links.txt
--rw-r--r--   0 wangyongzhou   (501) staff       (20)      103 2024-02-05 10:14:51.000000 WebexCompassSDK-44.3.4/src/WebexCompassSDK.egg-info/top_level.txt
+drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-04-07 06:43:57.002882 WebexCompassSDK-44.4.1/
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)      159 2024-04-07 06:43:57.002618 WebexCompassSDK-44.4.1/PKG-INFO
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)     2544 2024-02-06 07:31:40.000000 WebexCompassSDK-44.4.1/README.md
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)       38 2024-04-07 06:43:57.002935 WebexCompassSDK-44.4.1/setup.cfg
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)      463 2024-02-06 07:31:40.000000 WebexCompassSDK-44.4.1/setup.py
+drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-04-07 06:43:57.000176 WebexCompassSDK-44.4.1/src/
+drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-04-07 06:43:57.001171 WebexCompassSDK-44.4.1/src/WebexCompassSDK/
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)     8635 2024-04-07 06:32:22.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK/WebexCompassClient.py
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)        0 2024-02-06 07:31:40.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK/__init__.py
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)      119 2024-04-07 06:32:22.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK/version.py
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)     3876 2024-04-07 06:32:22.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK/ws.py
+drwxr-xr-x   0 wangyongzhou   (501) staff       (20)        0 2024-04-07 06:43:57.002340 WebexCompassSDK-44.4.1/src/WebexCompassSDK.egg-info/
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)      159 2024-04-07 06:43:56.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK.egg-info/PKG-INFO
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)      321 2024-04-07 06:43:56.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK.egg-info/SOURCES.txt
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)        1 2024-04-07 06:43:56.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK.egg-info/dependency_links.txt
+-rw-r--r--   0 wangyongzhou   (501) staff       (20)      103 2024-04-07 06:43:56.000000 WebexCompassSDK-44.4.1/src/WebexCompassSDK.egg-info/top_level.txt
```

### Comparing `WebexCompassSDK-44.3.4/README.md` & `WebexCompassSDK-44.4.1/README.md`

 * *Files identical despite different names*

### Comparing `WebexCompassSDK-44.3.4/src/WebexCompassSDK/ws.py` & `WebexCompassSDK-44.4.1/src/WebexCompassSDK/ws.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import asyncio
 import threading
 
 import websockets
+import ssl
 import logging
 
 class websocketWrapper:
     def __init__(self):
         self.websocket : websockets.WebSocketClientProtocol = None # type: ignore
         self.websocket_loop : asyncio.AbstractEventLoop = None # type: ignore
         self.websocket_thread : threading.Thread = None # type: ignore
@@ -67,15 +68,21 @@
         
         await self.websocket.send(message)
 
     async def _connect_websocket(self,uri,on_message = None ,on_connected=None, on_disconnected=None):
 
         logging.info(f"Connecting to {uri}")
         try:
-            async with websockets.connect(uri=uri) as websocket:
+            ssl_context = None
+            if uri.startswith("wss"):
+                ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+                ssl_context.check_hostname = False
+                ssl_context.verify_mode = ssl.CERT_NONE
+
+            async with websockets.connect(uri=uri, ssl=ssl_context) as websocket:
 
                 self.websocket = websocket
 
                 logging.info(f"Connected to {uri}")
                 if on_connected:
                     on_connected(websocket)
```

