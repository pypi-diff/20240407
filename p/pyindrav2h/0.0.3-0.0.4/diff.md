# Comparing `tmp/pyindrav2h-0.0.3.tar.gz` & `tmp/pyindrav2h-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyindrav2h-0.0.3.tar", last modified: Sat Apr  6 16:07:50 2024, max compression
+gzip compressed data, was "pyindrav2h-0.0.4.tar", last modified: Sun Apr  7 18:30:35 2024, max compression
```

## Comparing `pyindrav2h-0.0.3.tar` & `pyindrav2h-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.409372 pyindrav2h-0.0.3/
--rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/LICENSE
--rw-r--r--   0 paulmorris   (501) staff       (20)     4183 2024-04-06 16:07:50.408610 pyindrav2h-0.0.3/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)     2387 2024-04-04 19:59:48.000000 pyindrav2h-0.0.3/README.md
--rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-06 16:02:23.000000 pyindrav2h-0.0.3/pyproject.toml
--rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-06 16:07:50.409509 pyindrav2h-0.0.3/setup.cfg
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.396456 pyindrav2h-0.0.3/src/
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.401147 pyindrav2h-0.0.3/src/pyindrav2h/
--rw-r--r--   0 paulmorris   (501) staff       (20)      114 2024-04-06 16:02:37.000000 pyindrav2h-0.0.3/src/pyindrav2h/__init__.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     2451 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/cli.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     4634 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/connection.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      746 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/exceptions.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      551 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/v2hclient.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     4170 2024-04-06 15:54:41.000000 pyindrav2h-0.0.3/src/pyindrav2h/v2hdevice.py
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.407607 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/
--rw-r--r--   0 paulmorris   (501) staff       (20)     4183 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/SOURCES.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/dependency_links.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/entry_points.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/requires.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/top_level.txt
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.836485 pyindrav2h-0.0.4/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.4/LICENSE
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4371 2024-04-07 18:30:35.835671 pyindrav2h-0.0.4/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)     2575 2024-04-07 18:19:36.000000 pyindrav2h-0.0.4/README.md
+-rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-07 18:20:14.000000 pyindrav2h-0.0.4/pyproject.toml
+-rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-07 18:30:35.836703 pyindrav2h-0.0.4/setup.cfg
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.823136 pyindrav2h-0.0.4/src/
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.828579 pyindrav2h-0.0.4/src/pyindrav2h/
+-rw-r--r--   0 paulmorris   (501) staff       (20)      202 2024-04-07 18:20:26.000000 pyindrav2h-0.0.4/src/pyindrav2h/__init__.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     2742 2024-04-07 18:14:52.000000 pyindrav2h-0.0.4/src/pyindrav2h/cli.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     5079 2024-04-07 16:17:53.000000 pyindrav2h-0.0.4/src/pyindrav2h/connection.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      736 2024-04-07 15:13:50.000000 pyindrav2h-0.0.4/src/pyindrav2h/exceptions.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      551 2024-04-04 19:31:06.000000 pyindrav2h-0.0.4/src/pyindrav2h/v2hclient.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4374 2024-04-07 17:58:54.000000 pyindrav2h-0.0.4/src/pyindrav2h/v2hdevice.py
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-07 18:30:35.834760 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4371 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/SOURCES.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/dependency_links.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/entry_points.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/requires.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-07 18:30:35.000000 pyindrav2h-0.0.4/src/pyindrav2h.egg-info/top_level.txt
```

### Comparing `pyindrav2h-0.0.3/LICENSE` & `pyindrav2h-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.3/PKG-INFO` & `pyindrav2h-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.3
+Version: 0.0.4
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,26 +60,28 @@
 ```
 On installation a CLI will become available: ```indracli```
 ## Usage/Examples
 
 ### CLI
 
 ```bash
-usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d]
-           {statistics,device,all,loadmatch,idle,schedule} ...
+usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
 
 Indra V2H CLI
 
 positional arguments:
-  {statistics,device,all,loadmatch,idle,schedule}
+  {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
     statistics          show device statistics
     device              show device info
     all                 show all info
     loadmatch           set mode to load matching
     idle                set mode to IDLE
+    exportmatch         set mode to export matching
+    charge              set mode to CHARGE
+    discharge           set mode to discharge
     schedule            return to scheuduled mode
 
 options:
   -h, --help            show this help message and exit
   -u EMAIL, --email EMAIL
   -p PASSWORD, --password PASSWORD
   -d, --debug
```

### Comparing `pyindrav2h-0.0.3/README.md` & `pyindrav2h-0.0.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 ```
 On installation a CLI will become available: ```indracli```
 ## Usage/Examples
 
 ### CLI
 
 ```bash
-usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d]
-           {statistics,device,all,loadmatch,idle,schedule} ...
+usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
 
 Indra V2H CLI
 
 positional arguments:
-  {statistics,device,all,loadmatch,idle,schedule}
+  {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
     statistics          show device statistics
     device              show device info
     all                 show all info
     loadmatch           set mode to load matching
     idle                set mode to IDLE
+    exportmatch         set mode to export matching
+    charge              set mode to CHARGE
+    discharge           set mode to discharge
     schedule            return to scheuduled mode
 
 options:
   -h, --help            show this help message and exit
   -u EMAIL, --email EMAIL
   -p PASSWORD, --password PASSWORD
   -d, --debug
```

### Comparing `pyindrav2h-0.0.3/pyproject.toml` & `pyindrav2h-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyindrav2h"
-version = "0.0.3"
+version = "0.0.4"
 description = "API client and example CLI to interact with Indra V2H Chargers"
 readme = "README.md"
 authors = [{ name = "Paul Morris", email = "paul@creatingwake.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyindrav2h-0.0.3/src/pyindrav2h/cli.py` & `pyindrav2h-0.0.4/src/pyindrav2h/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import logging
 from getpass import getpass
 import argparse
 import configparser
 import asyncio
 import os
-from pyindrav2h.connection import Connection
-from pyindrav2h.v2hclient import v2hClient
+from .connection import Connection
+from .v2hclient import v2hClient
+from . import V2H_MODES
 
 logging.basicConfig()
 logging.root.setLevel(logging.WARNING)
 
 _LOGGER = logging.getLogger(__name__)
 
 async def main(args):
@@ -25,27 +26,27 @@
     conn = Connection(userEmail, userPass)
     await conn.checkAPICreds()
 
     client = v2hClient(conn)
 
     # refresh device/stats data
     await client.refresh()
-    
+
+    if args.command == "schedule":
+        args.command = "clear" # translate displayed mode commmand to endpoint command
     if (args.command == "device"):
         print(client.device.showDevice())
     elif (args.command == "statistics"):
         print(client.device.showStats())
     elif (args.command == "all"):
         print(client.device.showAll())
-    elif (args.command == "loadmatch"):
-        print(await client.device.load_match())
-    elif (args.command == "idle"):
-        print(await client.device.idle())
-    elif (args.command == "schedule"):
-        print(await client.device.schedule())
+    elif (args.command in list(V2H_MODES.values())):
+        for mode, command in V2H_MODES.items():
+            if command == args.command:
+                print(await client.device.select_charger_mode(mode))
 
 def cli():
     config = configparser.ConfigParser()
     config["indra-account"] = {"email": "", "password": ""}
     config.read([".indra.cfg", os.path.expanduser("~/.indra.cfg")])
     parser = argparse.ArgumentParser(prog="indracli", description="Indra V2H CLI")
     parser.add_argument(
@@ -63,13 +64,16 @@
     parser.add_argument("-d", "--debug", dest="debug", action="store_true")
     subparsers = parser.add_subparsers(dest="command", required=True)
     subparsers.add_parser("statistics", help="show device statistics")
     subparsers.add_parser("device", help="show device info")
     subparsers.add_parser("all", help="show all info")
     subparsers.add_parser("loadmatch", help="set mode to load matching")
     subparsers.add_parser("idle", help="set mode to IDLE")
+    subparsers.add_parser("exportmatch", help="set mode to export matching")
+    subparsers.add_parser("charge", help="set mode to CHARGE")
+    subparsers.add_parser("discharge", help="set mode to discharge")
     subparsers.add_parser("schedule", help="return to scheuduled mode")
 
     args = parser.parse_args()
 
     loop = asyncio.get_event_loop()
     loop.run_until_complete(main(args))
```

### Comparing `pyindrav2h-0.0.3/src/pyindrav2h/connection.py` & `pyindrav2h-0.0.4/src/pyindrav2h/connection.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,45 +20,56 @@
         self.timeout = timeout
         self.email = userEmail
         self.password = userPass
         self._headers = {"User-Agent": "Wget/1.14 (linux-gnu)"}
         self._xsrfToken = None
         self._bearerToken = None
         self._cookies = None
+        self._authRetries = 2
         _LOGGER.debug("New connection created")
 
-    async def checkAPICreds(self):
+    async def updateBearerAuth(self):
+        _LOGGER.debug(f"Updating BearerToken")
         self._xsrfToken = await self.getXsrf(loginUrl)
         _LOGGER.debug(f"XSRF token: {self._xsrfToken}")
         self._bearerToken = await self.getAuth("POST", "/login")
         self._headers["Authorization"] = self._bearerToken
-        succ = {'success': 'True'}
-        if succ['success'] == False:
+
+    async def checkAPICreds(self):
+        await self.updateBearerAuth()
+        if self._bearerToken is None:
             raise WrongCredentialsException()
     
     async def send(self, method, url, json=None):
-        # params = {'api_key': self.email, 'api_secret': self.password}
+        if self._bearerToken is None:
+            _LOGGER.error("Missing BearerToken - calling updateBearerAuth()")
+            await self.updateBearerAuth()
+
         async with httpx.AsyncClient(
             headers=self._headers, timeout=self.timeout
         ) as httpclient:
-            # theUrl = apiBaseUrl + url
-            theUrl = url
-            try:
-                _LOGGER.debug(f"{method} {url} {theUrl}")
-                response = await httpclient.request(method, theUrl, json=json)
-            except httpx.ReadTimeout:
-                raise TimeoutException()
-            else:
-                if response.status_code == 200:
-                    return response.json()
-                elif response.status_code == 202:
-                    return True
-                elif response.status_code == 401:
-                    raise WrongCredentialsException()
-                raise V2HException(response.status_code)
+            for i in range(self._authRetries): # allow retries to obtain a new Bearer Auth token
+                try:
+                    _LOGGER.debug(f"{method} {url} Attempt: {i}")
+                    response = await httpclient.request(method, url, json=json)
+                except httpx.ReadTimeout:
+                    raise TimeoutException()
+                else:
+                    if response.status_code == 200:
+                        return response.json()
+                    elif response.status_code == 202:
+                        return True
+                    elif response.status_code == 401:
+                        if i < self._authRetries - 1:  # i is zero indexed
+                            await self.updateBearerAuth()
+                            httpclient.headers=self._headers
+                            continue
+                        else:
+                            raise WrongCredentialsException()
+                    raise V2HException(response.status_code)
     
     async def get(self, url, data=None):
         url = apiBaseUrl + url
         return await self.send("GET", url, data)
     
     async def post(self, url, data=None):
         url = apiBaseUrl + url
@@ -103,13 +114,10 @@
                     self._cookies = response.cookies
                     soup = bs(htmlBody, "lxml")
                     jwtToken = soup.find('input', {"name": "JWTToken"})
                     if jwtToken:
                         return jwtToken['value']
                     else:
                         raise WrongCredentialsException()
-
-                    # _LOGGER.debug(f"RESPONSE: {response.text}")
-                    # return response.json()
                 elif response.status_code == 401:
                     raise WrongCredentialsException()
                 raise V2HException(response.status_code)
```

### Comparing `pyindrav2h-0.0.3/src/pyindrav2h/exceptions.py` & `pyindrav2h-0.0.4/src/pyindrav2h/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,9 +19,9 @@
 
 class WrongCredentialsException(V2HException):
     """Class of exceptions for incomplete credentials."""
     pass
 
 
 class TimeoutException(V2HException):
-    """Class of exceptions for incomplete credentials."""
+    """Class of exceptions for http timeout."""
     pass
```

### Comparing `pyindrav2h-0.0.3/src/pyindrav2h/v2hclient.py` & `pyindrav2h-0.0.4/src/pyindrav2h/v2hclient.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.3/src/pyindrav2h/v2hdevice.py` & `pyindrav2h-0.0.4/src/pyindrav2h/v2hdevice.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,33 @@
         self.stats = {}
         self.active = {}
 
     async def refresh_device_info(self):
         d = await self.connection.get("/authorize/validate")
         self.data = d
     
-    async def __set_mode(self, mode):
+    async def __set_mode(self, mode, payload=None):
         s = await self.connection.post("/transactions/" + self.id + 
-                                        "/interrupt/" + mode)
+                                        "/interrupt/" + mode,
+                                        payload)
         return s
-    
+
     async def load_match(self):
         return await self.__set_mode(V2H_MODES['LOAD_MATCH'])
 
     async def idle(self):
         return await self.__set_mode(V2H_MODES['IDLE'])       
 
     async def schedule(self):
         return await self.__set_mode(V2H_MODES['SCHEDULE'])
     
-    async def select_charger_mode(self, mode):
-        return await self.__set_mode(V2H_MODES[mode])
+    async def select_charger_mode(self, mode, rate=None):
+        if mode in {'CHARGE', 'DISCHARGE'}:
+            rate = {"limitAmps": 25} # charge / discharge fixed at max rate for now
+        return await self.__set_mode(V2H_MODES[mode], rate)
 
     async def refresh_stats(self):
         s = await self.connection.get("/telemetry/devices/" + self.serial + 
                                       "/latest")
         self.stats = s
         _LOGGER.debug(f"Stats: {s}")
         a = await self.connection.get("/transactions/" + self.serial +
```

### Comparing `pyindrav2h-0.0.3/src/pyindrav2h.egg-info/PKG-INFO` & `pyindrav2h-0.0.4/src/pyindrav2h.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.3
+Version: 0.0.4
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -60,26 +60,28 @@
 ```
 On installation a CLI will become available: ```indracli```
 ## Usage/Examples
 
 ### CLI
 
 ```bash
-usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d]
-           {statistics,device,all,loadmatch,idle,schedule} ...
+usage: indracli [-h] [-u EMAIL] [-p PASSWORD] [-d] {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule} ...
 
 Indra V2H CLI
 
 positional arguments:
-  {statistics,device,all,loadmatch,idle,schedule}
+  {statistics,device,all,loadmatch,idle,exportmatch,charge,discharge,schedule}
     statistics          show device statistics
     device              show device info
     all                 show all info
     loadmatch           set mode to load matching
     idle                set mode to IDLE
+    exportmatch         set mode to export matching
+    charge              set mode to CHARGE
+    discharge           set mode to discharge
     schedule            return to scheuduled mode
 
 options:
   -h, --help            show this help message and exit
   -u EMAIL, --email EMAIL
   -p PASSWORD, --password PASSWORD
   -d, --debug
```

