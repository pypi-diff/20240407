# Comparing `tmp/slinn-2.2.2.tar.gz` & `tmp/slinn-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slinn-2.2.2.tar", last modified: Sun Apr  7 11:02:22 2024, max compression
+gzip compressed data, was "slinn-2.2.3.tar", last modified: Sun Apr  7 15:42:07 2024, max compression
```

## Comparing `slinn-2.2.2.tar` & `slinn-2.2.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5330 2024-04-07 11:02:22.941159 slinn-2.2.2/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5090 2024-03-28 21:08:58.000000 slinn-2.2.2/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-07 11:02:22.941159 slinn-2.2.2/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      761 2024-04-07 11:00:29.000000 slinn-2.2.2/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-03-28 21:03:17.000000 slinn-2.2.2/slinn/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-03-28 20:47:57.000000 slinn-2.2.2/slinn/__main__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      328 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/address.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-03-28 20:49:08.000000 slinn-2.2.2/slinn/any_filter.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/default/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/default/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12930 2024-04-07 10:56:18.000000 slinn-2.2.2/slinn/default/manage.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      279 2024-03-28 20:39:01.000000 slinn-2.2.2/slinn/default/project.json
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      297 2024-03-28 21:04:44.000000 slinn-2.2.2/slinn/dispatcher.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.2/slinn/file.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-03-28 21:05:29.000000 slinn-2.2.2/slinn/filter.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/guides/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/guides/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      580 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/guides/migration1xx2xx.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-03-28 21:01:29.000000 slinn-2.2.2/slinn/http_api_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-03-28 20:50:47.000000 slinn-2.2.2/slinn/http_json_api_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-03-28 20:50:58.000000 slinn-2.2.2/slinn/http_json_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/http_redirect.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-03-28 21:01:34.000000 slinn-2.2.2/slinn/http_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-03-28 20:47:53.000000 slinn-2.2.2/slinn/link_filter.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-03-28 20:46:48.000000 slinn-2.2.2/slinn/request.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5028 2024-03-28 21:03:10.000000 slinn-2.2.2/slinn/server.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/templates/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/__init__.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn/templates/example/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/example/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/example/app.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/example/config.json
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn/templates/firstrun/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      567 2024-03-28 20:39:01.000000 slinn-2.2.2/slinn/templates/firstrun/app.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/config.json
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn/templates/firstrun/data/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/data/slinn.html
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/data/styles.css
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1093 2024-03-28 20:55:25.000000 slinn-2.2.2/slinn/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5330 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      936 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/top_level.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/zip-safe
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5365 2024-04-07 15:42:07.357757 slinn-2.2.3/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5123 2024-04-07 15:24:37.000000 slinn-2.2.3/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-07 15:42:07.357757 slinn-2.2.3/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      763 2024-04-07 15:32:00.000000 slinn-2.2.3/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-04-07 14:40:45.000000 slinn-2.2.3/slinn/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/__main__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      328 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/address.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/any_filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/default/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/default/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12930 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/default/manage.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      279 2024-03-28 20:39:01.000000 slinn-2.2.3/slinn/default/project.json
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      297 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/dispatcher.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.3/slinn/file.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/guides/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/guides/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      580 2024-04-07 11:25:26.000000 slinn-2.2.3/slinn/guides/migration1xx2xx.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/http_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/http_json_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/http_json_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/http_redirect.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-04-07 14:32:49.000000 slinn-2.2.3/slinn/http_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/link_filter.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-04-07 14:32:49.000000 slinn-2.2.3/slinn/request.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5178 2024-04-07 15:05:28.000000 slinn-2.2.3/slinn/server.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/__init__.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/example/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/example/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/example/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/example/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/firstrun/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      567 2024-03-28 20:39:01.000000 slinn-2.2.3/slinn/templates/firstrun/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/firstrun/data/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/data/slinn.html
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/data/styles.css
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1191 2024-04-07 15:10:25.000000 slinn-2.2.3/slinn/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5365 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      936 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.3/slinn.egg-info/zip-safe
```

### Comparing `slinn-2.2.2/PKG-INFO` & `slinn-2.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: slinn
-Version: 2.2.2
-Summary: HTTPS and HTTP server framework
+Version: 2.2.3
+Summary: A HTTPS and HTTP server framework
 Home-page: https://slinn.miotp.ru/
 Author: Mark Radin
 Author-email: mrybs2@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Slinn is a HTTPS and HTTP server framework
@@ -16,35 +16,40 @@
 python3 -m slinn create helloworld
 cd helloworld
 venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
 venv/bin/python manage.py run 
 ```
 
 ##### Windows:
-```bat
+```batch
 py -m slinn create helloworld
 cd helloworld
 venv\Scripts\activate
 py manage.py create localhost host=localhost host=127.0.0.1
 py manage.py run 
 ```
 
 #### Simple example
 ```python
 # localhost/app.py
 
-from slinn import Dispatcher, AnyFilter, LinkFilter, HttpResponse, HttpAPIResponse
+from slinn import *
 
 
 dp = Dispatcher('localhost', '127.0.0.1')
 
 
 @dp(LinkFilter('api'))
 def api(request):
-    return HttpAPIResponse('{"status": "ok"}')
+    return HttpJSONAPIResponse(status='ok')
+
+@dp(LinkFilter(''))
+@dp(LinkFilter('index'))
+def index(request):
+    return HttpRedirect('/helloworld')
 
 
 @dp(AnyFilter)
 def helloworld(request):
      return HttpResponse('Hello world!')
 
 ```
@@ -72,15 +77,15 @@
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv/bin/activate
 ```
 
 ##### Windows:
-```bat
+```batch
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv\Scripts\activate
 ```
 
 You should add this code to example `example.py`
@@ -89,28 +94,28 @@
 ```
 then write `python example.py`
 
 #### Functions:
 ```python
 from slinn import Server
 
-server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run server
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
 server.address() -> str  # Returns info str
 server.reload(*dispatchers: tuple)  # Reloads server
 server.listen(address: Address)  # Start listening address
 
 Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
 ```
 
 ```python
 from slinn import Address
 
 address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
 
-Address(443, 'google.com')
+Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
 ```
 
 ```python
 from slinn import Dispatcher
 
 dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
 
@@ -125,30 +130,29 @@
 ```
 
 ```python
 from slinn import Filter, LinkFilter, AnyFilter
 
 _filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
 _filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-_filter.size(text: str, method: str) -> int  # Special method for Smart Navigation
 
 Filter('/user/.+/profile.*')
 
 # LinkFilter inherits from Filter
 LinkFilter('user/.+/profile')
 
 # AnyFilter as same as Filter('.*')
 ```
 
 ```python
 from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
 
 http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value: any)
-http_response.make(type: str='HTTP/2.0') -> str
+http_response.set_cookie(key: str, value: any)  # Sets cookie
+http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
 
 HttpResponse('<h1>Hello world</h1>', content_type='text/html')
 
 # HttpAPIResponse inherits from HttpResponse
 # HttpAPIResponse sets Access-Control-Allow-Origin to '*'
 
 HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
@@ -159,15 +163,15 @@
 HttpRedirect('slinn.miotp.ru')
 
 # HttpJSONResponse for responding JSON 
 HttpJSONResponse(**payload: dict)
 
 HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
 
-# HttpJSONAPIResponse is like HttpJSONResponse, but it sets Access-Control-Allow-Origin to '*'
+# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
 
 HttpJSONAPIResponse(code=43657, until=1719931149)
 ```
 
 ```python
 from slinn import Request
```

### Comparing `slinn-2.2.2/README.md` & `slinn-2.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 python3 -m slinn create helloworld
 cd helloworld
 venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
 venv/bin/python manage.py run 
 ```
 
 ##### Windows:
-```bat
+```batch
 py -m slinn create helloworld
 cd helloworld
 venv\Scripts\activate
 py manage.py create localhost host=localhost host=127.0.0.1
 py manage.py run 
 ```
 
 #### Simple example
 ```python
 # localhost/app.py
 
-from slinn import Dispatcher, AnyFilter, LinkFilter, HttpResponse, HttpAPIResponse
+from slinn import *
 
 
 dp = Dispatcher('localhost', '127.0.0.1')
 
 
 @dp(LinkFilter('api'))
 def api(request):
-    return HttpAPIResponse('{"status": "ok"}')
+    return HttpJSONAPIResponse(status='ok')
+
+@dp(LinkFilter(''))
+@dp(LinkFilter('index'))
+def index(request):
+    return HttpRedirect('/helloworld')
 
 
 @dp(AnyFilter)
 def helloworld(request):
      return HttpResponse('Hello world!')
 
 ```
@@ -62,15 +67,15 @@
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv/bin/activate
 ```
 
 ##### Windows:
-```bat
+```batch
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv\Scripts\activate
 ```
 
 You should add this code to example `example.py`
@@ -79,28 +84,28 @@
 ```
 then write `python example.py`
 
 #### Functions:
 ```python
 from slinn import Server
 
-server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run server
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
 server.address() -> str  # Returns info str
 server.reload(*dispatchers: tuple)  # Reloads server
 server.listen(address: Address)  # Start listening address
 
 Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
 ```
 
 ```python
 from slinn import Address
 
 address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
 
-Address(443, 'google.com')
+Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
 ```
 
 ```python
 from slinn import Dispatcher
 
 dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
 
@@ -115,30 +120,29 @@
 ```
 
 ```python
 from slinn import Filter, LinkFilter, AnyFilter
 
 _filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
 _filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-_filter.size(text: str, method: str) -> int  # Special method for Smart Navigation
 
 Filter('/user/.+/profile.*')
 
 # LinkFilter inherits from Filter
 LinkFilter('user/.+/profile')
 
 # AnyFilter as same as Filter('.*')
 ```
 
 ```python
 from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
 
 http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value: any)
-http_response.make(type: str='HTTP/2.0') -> str
+http_response.set_cookie(key: str, value: any)  # Sets cookie
+http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
 
 HttpResponse('<h1>Hello world</h1>', content_type='text/html')
 
 # HttpAPIResponse inherits from HttpResponse
 # HttpAPIResponse sets Access-Control-Allow-Origin to '*'
 
 HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
@@ -149,15 +153,15 @@
 HttpRedirect('slinn.miotp.ru')
 
 # HttpJSONResponse for responding JSON 
 HttpJSONResponse(**payload: dict)
 
 HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
 
-# HttpJSONAPIResponse is like HttpJSONResponse, but it sets Access-Control-Allow-Origin to '*'
+# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
 
 HttpJSONAPIResponse(code=43657, until=1719931149)
 ```
 
 ```python
 from slinn import Request
```

### Comparing `slinn-2.2.2/setup.py` & `slinn-2.2.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     with open('README.md', 'r') as f:
         return f.read()
     
 templates = ['firstrun', 'example']
 
 
 setup(name='slinn',
-      version='2.2.2',
-      description='HTTPS and HTTP server framework',
+      version='2.2.3',
+      description='A HTTPS and HTTP server framework',
       packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
       package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
       author='Mark Radin',
       author_email='mrybs2@gmail.com',
       url='https://slinn.miotp.ru/',
       long_description=readme(),
       long_description_content_type='text/markdown',
```

### Comparing `slinn-2.2.2/slinn/__init__.py` & `slinn-2.2.3/slinn/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from slinn.http_api_response import HttpAPIResponse
 from slinn.http_json_response import HttpJSONResponse
 from slinn.http_json_api_response import HttpJSONAPIResponse
 from slinn.server import Server
 from slinn.dispatcher import Dispatcher
 
 
-version = 'Slinn Murega v2.2.1 290324a'
+version = 'Slinn Murega v2.2.3 070424C'
```

### Comparing `slinn-2.2.2/slinn/__main__.py` & `slinn-2.2.3/slinn/__main__.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/default/manage.py` & `slinn-2.2.3/slinn/default/manage.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/filter.py` & `slinn-2.2.3/slinn/filter.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/guides/migration1xx2xx.py` & `slinn-2.2.3/slinn/guides/migration1xx2xx.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/http_api_response.py` & `slinn-2.2.3/slinn/http_api_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/http_response.py` & `slinn-2.2.3/slinn/http_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/request.py` & `slinn-2.2.3/slinn/request.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/server.py` & `slinn-2.2.3/slinn/server.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from slinn import Request, Address, Filter, utils
-import socket, ssl, threading, time, traceback, os
+import socket, ssl, time, os, traceback
 
 
 class Server:
 	class Handle:
 		def __init__(self, filter: Filter, function):
 			self.filter = filter
 			self.function = function
@@ -12,15 +12,14 @@
 		self.dispatchers = dispatchers
 		self.smart_navigation = smart_navigation
 		self.server_socket = None
 		self.ssl = ssl_fullchain is not None and ssl_key is not None
 		self.ssl_cert, self.ssl_key = ssl_fullchain, ssl_key
 		self.ssl_context = None
 		self.waiting = False
-		self.running = True
 		self.thread = None
 		self.delay = delay
 		self.timeout = timeout
 		self.max_bytes_per_recieve = max_bytes_per_recieve
 		self.max_bytes = max_bytes
 		self.__address = None
 
@@ -29,20 +28,18 @@
 		if self.thread is not None:
 			self.thread.stop()
 			try:
 				self.thread.join()
 			except RuntimeError:
 				pass
 		self.dispatchers = dispatchers
-		if self.running:
+		if utils.check_socket(self.server_socket):
 			self.server_socket.close()
-			self.running = False
 		if self.__address is not None:
 			self.listen(self.__address)
-		self.waiting = False
 
 	def address(self):
 		return f'HTTP{"S" if self.ssl else ""} server is available on http{"s" if self.ssl else ""}://{"" if "." in self.host else "["}{self.host}{"" if "." in self.host else "]"}{(":"+str(self.port) if self.port != 443 else "") if self.ssl else (":"+str(self.port )if self.port != 80 else "")}/'
 		
 	def listen(self, address: Address):		
 		self.__address = address
 		self.host, self.port = address.host, address.port
@@ -52,34 +49,31 @@
 			self.server_socket = socket.create_server((self.host, self.port), family=socket.AF_INET6)
 		else:
 			self.server_socket = socket.create_server((self.host, self.port), family=(socket.AF_INET if '.' in self.host else socket.AF_INET6))
 		self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 		if self.ssl:
 			self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
 			self.ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
-		self.running = True
 		self.server_socket.listen()
 		print(self.address())
+		self.waiting = False
 		try:
-			while self.running:
+			while utils.check_socket(self.server_socket):
 				if not self.waiting:
 					self.thread = utils.StoppableThread(target=self.handle_request)
 					self.thread.start()
 				time.sleep(self.delay)
 		except KeyboardInterrupt:
 			print('Got KeyboardInterrupt, halting the application...')
-			if self.running:
+			if utils.check_socket(self.server_socket):
 				self.server_socket.close()
-				self.running = False
 			os._exit(0)
 						
 	def handle_request(self):
 		try:
-			if not self.running:
-				return
 			self.waiting = True
 			client_socket, client_address = self.server_socket.accept()
 			if self.ssl:
 				client_socket = self.ssl_context.wrap_socket(client_socket, server_side=True)
 			self.waiting = False
 			try:
 				client_socket.settimeout(self.timeout)
@@ -97,40 +91,45 @@
 				
 				if header == '':
 					return
 
 				request = Request(header, content, client_address)
 				print(request)
 			except KeyError:
+				if utils.check_socket(client_socket):
+					client_socket.close()
 				return print('Got KeyError, probably invalid request. Ignore')
 			except UnicodeDecodeError:
+				if utils.check_socket(client_socket):
+					client_socket.close()
 				return print('Got UnocodeDecodeError, probably invalid request. Ignore')
 			except ConnectionResetError:
 				return print('Connection reset by client')
 			except OSError:
 				return print('Connection closed')
 			for dispatcher in self.dispatchers:
 				if True in [utils.restartswith(request.host, host) for host in dispatcher.hosts]:
 					if self.smart_navigation:
 						sizes = [handle.filter.size(request.link, request.method) for handle in dispatcher.handles]
 						if sizes != []:
 							handle = dispatcher.handles[sizes.index(max(sizes))]
 							if handle.filter.check(request.link, request.method):
-								client_socket.sendall(handle.function(request).make(request.version))
-								client_socket.close()
+								if utils.check_socket(client_socket):
+									client_socket.sendall(handle.function(request).make(request.version))
+									client_socket.close()
 								return
 					else:
 						for handle in dispatcher.handles:
 							if handle.filter.check(request.link, request.method):
-								client_socket.sendall(handle.function(request).make(request.version))
-								client_socket.close()
+								if utils.check_socket(client_socket):
+									client_socket.sendall(handle.function(request).make(request.version))
+									client_socket.close()
 								return
 		except ssl.SSLError:
 			print('During handling request, an exception has occured:')
 			traceback.print_exc()
-			self.waiting = False
 			print('Got ssl.SSLError, reloading...')
-			self.reload(self.dispatchers)
+			self.reload(*self.dispatchers)
 		except Exception:
 			print('During handling request, an exception has occured:')
 			traceback.print_exc()
 			self.waiting = False
```

### Comparing `slinn-2.2.2/slinn/templates/firstrun/app.py` & `slinn-2.2.3/slinn/templates/firstrun/app.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/templates/firstrun/data/slinn.html` & `slinn-2.2.3/slinn/templates/firstrun/data/slinn.html`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn/templates/firstrun/data/styles.css` & `slinn-2.2.3/slinn/templates/firstrun/data/styles.css`

 * *Files identical despite different names*

### Comparing `slinn-2.2.2/slinn.egg-info/PKG-INFO` & `slinn-2.2.3/slinn.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: slinn
-Version: 2.2.2
-Summary: HTTPS and HTTP server framework
+Version: 2.2.3
+Summary: A HTTPS and HTTP server framework
 Home-page: https://slinn.miotp.ru/
 Author: Mark Radin
 Author-email: mrybs2@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Slinn is a HTTPS and HTTP server framework
@@ -16,35 +16,40 @@
 python3 -m slinn create helloworld
 cd helloworld
 venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
 venv/bin/python manage.py run 
 ```
 
 ##### Windows:
-```bat
+```batch
 py -m slinn create helloworld
 cd helloworld
 venv\Scripts\activate
 py manage.py create localhost host=localhost host=127.0.0.1
 py manage.py run 
 ```
 
 #### Simple example
 ```python
 # localhost/app.py
 
-from slinn import Dispatcher, AnyFilter, LinkFilter, HttpResponse, HttpAPIResponse
+from slinn import *
 
 
 dp = Dispatcher('localhost', '127.0.0.1')
 
 
 @dp(LinkFilter('api'))
 def api(request):
-    return HttpAPIResponse('{"status": "ok"}')
+    return HttpJSONAPIResponse(status='ok')
+
+@dp(LinkFilter(''))
+@dp(LinkFilter('index'))
+def index(request):
+    return HttpRedirect('/helloworld')
 
 
 @dp(AnyFilter)
 def helloworld(request):
      return HttpResponse('Hello world!')
 
 ```
@@ -72,15 +77,15 @@
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv/bin/activate
 ```
 
 ##### Windows:
-```bat
+```batch
 mkdir helloworld 
 cd helloworld
 python3 -m venv venv
 venv\Scripts\activate
 ```
 
 You should add this code to example `example.py`
@@ -89,28 +94,28 @@
 ```
 then write `python example.py`
 
 #### Functions:
 ```python
 from slinn import Server
 
-server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run server
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
 server.address() -> str  # Returns info str
 server.reload(*dispatchers: tuple)  # Reloads server
 server.listen(address: Address)  # Start listening address
 
 Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
 ```
 
 ```python
 from slinn import Address
 
 address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
 
-Address(443, 'google.com')
+Address(443, 'google.com') <-> Address(443, '2a00:1450:4010:c02::71')
 ```
 
 ```python
 from slinn import Dispatcher
 
 dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
 
@@ -125,30 +130,29 @@
 ```
 
 ```python
 from slinn import Filter, LinkFilter, AnyFilter
 
 _filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
 _filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-_filter.size(text: str, method: str) -> int  # Special method for Smart Navigation
 
 Filter('/user/.+/profile.*')
 
 # LinkFilter inherits from Filter
 LinkFilter('user/.+/profile')
 
 # AnyFilter as same as Filter('.*')
 ```
 
 ```python
 from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
 
 http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value: any)
-http_response.make(type: str='HTTP/2.0') -> str
+http_response.set_cookie(key: str, value: any)  # Sets cookie
+http_response.make(type: str='HTTP/2.0') -> str  # Makes HTTP code
 
 HttpResponse('<h1>Hello world</h1>', content_type='text/html')
 
 # HttpAPIResponse inherits from HttpResponse
 # HttpAPIResponse sets Access-Control-Allow-Origin to '*'
 
 HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
@@ -159,15 +163,15 @@
 HttpRedirect('slinn.miotp.ru')
 
 # HttpJSONResponse for responding JSON 
 HttpJSONResponse(**payload: dict)
 
 HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
 
-# HttpJSONAPIResponse is like HttpJSONResponse, but it sets Access-Control-Allow-Origin to '*'
+# HttpJSONAPIResponse for responding JSON and it sets Access-Control-Allow-Origin to '*'
 
 HttpJSONAPIResponse(code=43657, until=1719931149)
 ```
 
 ```python
 from slinn import Request
```

### Comparing `slinn-2.2.2/slinn.egg-info/SOURCES.txt` & `slinn-2.2.3/slinn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

