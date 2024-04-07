# Comparing `tmp/slinn-2.2.0.tar.gz` & `tmp/slinn-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slinn-2.2.0.tar", last modified: Sat Mar 23 11:54:15 2024, max compression
+gzip compressed data, was "slinn-2.2.2.tar", last modified: Sun Apr  7 11:02:22 2024, max compression
```

## Comparing `slinn-2.2.0.tar` & `slinn-2.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:15.004765 slinn-2.2.0/
--rw-rw-rw-   0        0        0     5285 2024-03-23 11:54:15.003765 slinn-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     5035 2024-03-23 11:53:16.000000 slinn-2.2.0/README.md
--rw-rw-rw-   0        0        0       42 2024-03-23 11:54:15.005765 slinn-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0      782 2024-03-23 11:53:16.000000 slinn-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:14.944928 slinn-2.2.0/slinn/
--rw-rw-rw-   0        0        0      593 2024-03-23 11:53:16.000000 slinn-2.2.0/slinn/__init__.py
--rw-rw-rw-   0        0        0     4484 2024-03-23 11:53:16.000000 slinn-2.2.0/slinn/__main__.py
--rw-rw-rw-   0        0        0      338 2024-02-09 18:54:22.000000 slinn-2.2.0/slinn/address.py
--rw-rw-rw-   0        0        0       59 2024-02-09 19:48:36.000000 slinn-2.2.0/slinn/any_filter.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:14.961488 slinn-2.2.0/slinn/default/
--rw-rw-rw-   0        0        0       36 2024-02-10 11:37:15.000000 slinn-2.2.0/slinn/default/__init__.py
--rw-rw-rw-   0        0        0    13291 2024-03-23 11:53:16.000000 slinn-2.2.0/slinn/default/manage.py
--rw-rw-rw-   0        0        0      295 2024-03-23 11:53:16.000000 slinn-2.2.0/slinn/default/project.json
--rw-rw-rw-   0        0        0      307 2024-02-09 19:04:46.000000 slinn-2.2.0/slinn/dispatcher.py
--rw-rw-rw-   0        0        0      161 2024-03-22 21:18:07.000000 slinn-2.2.0/slinn/file.py
--rw-rw-rw-   0        0        0      690 2024-02-11 11:30:11.000000 slinn-2.2.0/slinn/filter.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:14.968486 slinn-2.2.0/slinn/guides/
--rw-rw-rw-   0        0        0       56 2024-02-11 13:06:29.000000 slinn-2.2.0/slinn/guides/__init__.py
--rw-rw-rw-   0        0        0      589 2024-02-11 13:27:24.000000 slinn-2.2.0/slinn/guides/migration1xx2xx.py
--rw-rw-rw-   0        0        0      614 2024-02-09 20:08:21.000000 slinn-2.2.0/slinn/http_api_response.py
--rw-rw-rw-   0        0        0      363 2024-03-07 15:19:54.000000 slinn-2.2.0/slinn/http_json_api_response.py
--rw-rw-rw-   0        0        0      467 2024-03-07 15:19:54.000000 slinn-2.2.0/slinn/http_json_response.py
--rw-rw-rw-   0        0        0      188 2024-02-09 18:54:22.000000 slinn-2.2.0/slinn/http_redirect.py
--rw-rw-rw-   0        0        0      752 2024-02-09 18:54:22.000000 slinn-2.2.0/slinn/http_response.py
--rw-rw-rw-   0        0        0      283 2024-02-10 17:56:59.000000 slinn-2.2.0/slinn/link_filter.py
--rw-rw-rw-   0        0        0     3174 2024-03-23 11:53:16.000000 slinn-2.2.0/slinn/request.py
--rw-rw-rw-   0        0        0     5110 2024-03-23 11:53:16.000000 slinn-2.2.0/slinn/server.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:14.971486 slinn-2.2.0/slinn/templates/
--rw-rw-rw-   0        0        0       23 2024-02-09 18:54:22.000000 slinn-2.2.0/slinn/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:14.981492 slinn-2.2.0/slinn/templates/example/
--rw-rw-rw-   0        0        0      163 2024-02-10 16:27:17.000000 slinn-2.2.0/slinn/templates/example/__init__.py
--rw-rw-rw-   0        0        0      291 2024-02-10 16:22:53.000000 slinn-2.2.0/slinn/templates/example/app.py
--rw-rw-rw-   0        0        0       24 2024-02-10 14:08:22.000000 slinn-2.2.0/slinn/templates/example/config.json
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:14.987951 slinn-2.2.0/slinn/templates/firstrun/
--rw-rw-rw-   0        0        0      166 2024-02-10 16:27:25.000000 slinn-2.2.0/slinn/templates/firstrun/__init__.py
--rw-rw-rw-   0        0        0      586 2024-03-23 11:53:16.000000 slinn-2.2.0/slinn/templates/firstrun/app.py
--rw-rw-rw-   0        0        0       23 2024-02-10 13:32:52.000000 slinn-2.2.0/slinn/templates/firstrun/config.json
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:15.002765 slinn-2.2.0/slinn/templates/firstrun/data/
--rw-rw-rw-   0        0        0     2241 2024-03-07 15:19:54.000000 slinn-2.2.0/slinn/templates/firstrun/data/slinn.html
--rw-rw-rw-   0        0        0      578 2024-02-09 18:54:22.000000 slinn-2.2.0/slinn/templates/firstrun/data/styles.css
--rw-rw-rw-   0        0        0     1083 2024-03-14 18:10:00.000000 slinn-2.2.0/slinn/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-23 11:54:15.003765 slinn-2.2.0/slinn.egg-info/
--rw-rw-rw-   0        0        0     5285 2024-03-23 11:54:14.000000 slinn-2.2.0/slinn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      946 2024-03-23 11:54:14.000000 slinn-2.2.0/slinn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-23 11:54:14.000000 slinn-2.2.0/slinn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-03-23 11:54:14.000000 slinn-2.2.0/slinn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-02-11 13:47:21.000000 slinn-2.2.0/slinn.egg-info/zip-safe
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5330 2024-04-07 11:02:22.941159 slinn-2.2.2/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5090 2024-03-28 21:08:58.000000 slinn-2.2.2/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-07 11:02:22.941159 slinn-2.2.2/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      761 2024-04-07 11:00:29.000000 slinn-2.2.2/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-03-28 21:03:17.000000 slinn-2.2.2/slinn/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-03-28 20:47:57.000000 slinn-2.2.2/slinn/__main__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      328 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/address.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-03-28 20:49:08.000000 slinn-2.2.2/slinn/any_filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/default/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/default/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12930 2024-04-07 10:56:18.000000 slinn-2.2.2/slinn/default/manage.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      279 2024-03-28 20:39:01.000000 slinn-2.2.2/slinn/default/project.json
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      297 2024-03-28 21:04:44.000000 slinn-2.2.2/slinn/dispatcher.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.2/slinn/file.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-03-28 21:05:29.000000 slinn-2.2.2/slinn/filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/guides/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/guides/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      580 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/guides/migration1xx2xx.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-03-28 21:01:29.000000 slinn-2.2.2/slinn/http_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-03-28 20:50:47.000000 slinn-2.2.2/slinn/http_json_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-03-28 20:50:58.000000 slinn-2.2.2/slinn/http_json_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/http_redirect.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-03-28 21:01:34.000000 slinn-2.2.2/slinn/http_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-03-28 20:47:53.000000 slinn-2.2.2/slinn/link_filter.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-03-28 20:46:48.000000 slinn-2.2.2/slinn/request.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5028 2024-03-28 21:03:10.000000 slinn-2.2.2/slinn/server.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.937825 slinn-2.2.2/slinn/templates/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/__init__.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn/templates/example/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/example/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/example/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/example/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn/templates/firstrun/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      567 2024-03-28 20:39:01.000000 slinn-2.2.2/slinn/templates/firstrun/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn/templates/firstrun/data/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/data/slinn.html
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.2/slinn/templates/firstrun/data/styles.css
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1093 2024-03-28 20:55:25.000000 slinn-2.2.2/slinn/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 11:02:22.941159 slinn-2.2.2/slinn.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5330 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      936 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.2/slinn.egg-info/zip-safe
```

### Comparing `slinn-2.2.0/PKG-INFO` & `slinn-2.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,200 +1,194 @@
-Metadata-Version: 2.1
-Name: slinn
-Version: 2.2.0
-Summary: HTTPS and HTTP server framework
-Home-page: https://slinn.miotp.ru/
-Author: Mark Radin
-Author-email: mrybs2@gmail.com
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
-# Slinn is a HTTPS and HTTP server framework
-
-### Create project
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash
-python3 -m slinn create helloworld
-cd helloworld
-venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
-venv/bin/python manage.py run 
-```
-
-##### Windows:
-```bat
-py -m slinn create helloworld
-cd helloworld
-venv\Scripts\activate
-py manage.py create localhost host=localhost host=127.0.0.1
-py manage.py run 
-```
-
-#### Simple example
-```python
-# localhost/app.py
-
-from slinn import Dispatcher, AnyFilter, LinkFilter, HttpResponse, HttpAPIResponse
-
-
-dp = Dispatcher('localhost', '127.0.0.1')
-
-
-@dp(LinkFilter('api'))
-def api(request):
-    return HttpAPIResponse('{"status": "ok"}')
-
-
-@dp(AnyFilter)
-def helloworld(request):
-     return HttpResponse('Hello world!')
-
-```
-
-Excepted output
-```
-$ venv/bin/python manage.py run
-Loading config...
-Apps: firstrun
-Debug mode enabled
-Smart navigation enabled
-
-Starting server...
-HTTP server is available on http://[::1]:8080/
-```
-
-To config project you should edit `./project.json`
-
-To config app you should edit `./%app%/config.json`
-
-### Create classic project
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash 
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv/bin/activate
-```
-
-##### Windows:
-```bat
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv\Scripts\activate
-```
-
-You should add this code to example `example.py`
-```
-Server(dp).listen(Address(8080))
-```
-then write `python example.py`
-
-#### Functions:
-```python
-from slinn import Server
-
-server = Server(*dispatchers: list[Dispatcher], ssl_cert: str=None, ssl_key: str=None, delay=0.05, timeout=0.03, max_bytes_per_recieve=4096, max_bytes=4294967296)  # Main class to run server
-server.address() -> str  # Returns info str
-server.reload(*dispatchers: list[Dispatcher])  # Reloads server
-server.listen(address: Address)  # Start listening address
-
-Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
-```
-
-```python
-from slinn import Address
-
-address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
-
-Address(443, 'google.com')
-```
-
-```python
-from slinn import Dispatcher
-
-dispatcher = Dispatcher(hosts: list=None)  # A class that contain many handlers
-
-Dispatcher('localhost', '127.0.0.1', '::1')
-
-# To add handler into dispatcher
-@dispatcher(filter: Filter)
-def handler(request: Request):
-    ...
-
-# handler should return HttpResponse-based object
-```
-
-```python
-from slinn import Filter, LinkFilter, AnyFilter
-
-_filter = Filter(filter: str, methods: list[str]=None)  # This class is used to choose match handler by link; uses regexp
-_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-_filter.size(text: str, method: str) -> int  # Special method for Smart Navigation
-
-Filter('/user/.+/profile.*')
-
-# LinkFilter inherits from Filter
-LinkFilter('user/.+/profile')
-
-# AnyFilter as same as Filter('.*')
-```
-
-```python
-from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
-
-http_response = HttpResponse(payload, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value)
-http_response.make(type: str='HTTP/2.0') -> str
-
-HttpResponse('<h1>Hello world</h1>', content_type='text/html')
-
-# HttpAPIResponse inherits from HttpResponse
-# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
-
-HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
-
-# HttpRedirect inherits from HttpResponse
-HttpRedirect(location: str)
-
-HttpRedirect('slinn.miotp.ru')
-
-# HttpJSONResponse for responding JSON 
-HttpJSONResponse(**payload)
-
-HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
-
-# HttpJSONAPIResponse is like HttpJSONResponse, but it sets Access-Control-Allow-Origin to '*'
-
-HttpJSONAPIResponse(code=43657, until=1719931149)
-```
-
-```python
-from slinn import Request
-
-request = Request(http_data: str, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
-
-# Attributes
-request.ip, request.port  # Client`s IP and port
-request.method  # HTTP method
-request.version  # HTTP version
-request.full_link  # Full link(path and params)
-request.host  # Requested host
-request.user_agent  # Client`s user agent
-request.accept  # maybe supported technologies
-request.encoding  # Supported encodings
-request.language  # Client`s language
-request.link  # Link(only path)
-request.args  # GET args
-request.cookies  # All saved cookies
-request.files # Uploaded files
-```
-
-```python
-from slinn import File
-
-file = File(id: str=None, data: bytes|bytearray=bytearray())
-
-# Attributes
-file.id  # File`s id 
-file.data  # Binary data
-file.headers  # Headers such as Content-Disposition
-```
+# Slinn is a HTTPS and HTTP server framework
+
+### Create project
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash
+python3 -m slinn create helloworld
+cd helloworld
+venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
+venv/bin/python manage.py run 
+```
+
+##### Windows:
+```bat
+py -m slinn create helloworld
+cd helloworld
+venv\Scripts\activate
+py manage.py create localhost host=localhost host=127.0.0.1
+py manage.py run 
+```
+
+#### Simple example
+```python
+# localhost/app.py
+
+from slinn import Dispatcher, AnyFilter, LinkFilter, HttpResponse, HttpAPIResponse
+
+
+dp = Dispatcher('localhost', '127.0.0.1')
+
+
+@dp(LinkFilter('api'))
+def api(request):
+    return HttpAPIResponse('{"status": "ok"}')
+
+
+@dp(AnyFilter)
+def helloworld(request):
+     return HttpResponse('Hello world!')
+
+```
+
+Excepted output
+```
+$ venv/bin/python manage.py run
+Loading config...
+Apps: firstrun
+Debug mode enabled
+Smart navigation enabled
+Delay: 50.0ms
+
+Starting server...
+HTTP server is available on http://[::1]:8080/
+```
+
+To config project you should edit `./project.json`
+
+To config app you should edit `./%app%/config.json`
+
+### Create classic project
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash 
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv/bin/activate
+```
+
+##### Windows:
+```bat
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv\Scripts\activate
+```
+
+You should add this code to example `example.py`
+```
+Server(dp).listen(Address(8080))
+```
+then write `python example.py`
+
+#### Functions:
+```python
+from slinn import Server
+
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run server
+server.address() -> str  # Returns info str
+server.reload(*dispatchers: tuple)  # Reloads server
+server.listen(address: Address)  # Start listening address
+
+Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
+```
+
+```python
+from slinn import Address
+
+address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
+
+Address(443, 'google.com')
+```
+
+```python
+from slinn import Dispatcher
+
+dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
+
+Dispatcher('localhost', '127.0.0.1', '::1')
+
+# To add handler into dispatcher
+@dispatcher(filter: Filter)
+def handler(request: Request):
+    ...
+
+# handler should return HttpResponse-based object
+```
+
+```python
+from slinn import Filter, LinkFilter, AnyFilter
+
+_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
+_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
+_filter.size(text: str, method: str) -> int  # Special method for Smart Navigation
+
+Filter('/user/.+/profile.*')
+
+# LinkFilter inherits from Filter
+LinkFilter('user/.+/profile')
+
+# AnyFilter as same as Filter('.*')
+```
+
+```python
+from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
+
+http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
+http_response.set_cookie(key: str, value: any)
+http_response.make(type: str='HTTP/2.0') -> str
+
+HttpResponse('<h1>Hello world</h1>', content_type='text/html')
+
+# HttpAPIResponse inherits from HttpResponse
+# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
+
+HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
+
+# HttpRedirect inherits from HttpResponse
+HttpRedirect(location: str)
+
+HttpRedirect('slinn.miotp.ru')
+
+# HttpJSONResponse for responding JSON 
+HttpJSONResponse(**payload: dict)
+
+HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
+
+# HttpJSONAPIResponse is like HttpJSONResponse, but it sets Access-Control-Allow-Origin to '*'
+
+HttpJSONAPIResponse(code=43657, until=1719931149)
+```
+
+```python
+from slinn import Request
+
+request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
+request.parse_http_header(http_header: str)  # Parse HTTP request`s header
+request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
+str(request)  # Convert slinn.Request to info text
+
+# Attributes
+request.ip, request.port  # Client`s IP and port
+request.method  # HTTP method
+request.version  # HTTP version
+request.full_link  # Full link(path and params)
+request.host  # Requested host
+request.user_agent  # Client`s user agent
+request.accept  # maybe supported technologies
+request.encoding  # Supported encodings
+request.language  # Client`s language
+request.link  # Link(only path)
+request.args  # GET args
+request.cookies  # All saved cookies
+request.files # Uploaded files
+```
+
+```python
+from slinn import File
+
+file = File(id: str=None, data: bytes|bytearray=bytearray())
+
+# Attributes
+file.id  # File`s id 
+file.data  # Binary data
+file.headers  # Headers such as Content-Disposition
+```
```

### Comparing `slinn-2.2.0/setup.py` & `slinn-2.2.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from setuptools import setup
-
-def readme():
-    with open('README.md', 'r') as f:
-        return f.read()
-    
-templates = ['firstrun', 'example']
-
-
-setup(name='slinn',
-      version='2.2.0',
-      description='HTTPS and HTTP server framework',
-      packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
-      package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
-      author='Mark Radin',
-      author_email='mrybs2@gmail.com',
-      url='https://slinn.miotp.ru/',
-      long_description=readme(),
-      long_description_content_type='text/markdown',
-      python_requires='>=3.11',
-      zip_safe=True)
+from setuptools import setup
+
+def readme():
+    with open('README.md', 'r') as f:
+        return f.read()
+    
+templates = ['firstrun', 'example']
+
+
+setup(name='slinn',
+      version='2.2.2',
+      description='HTTPS and HTTP server framework',
+      packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
+      package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
+      author='Mark Radin',
+      author_email='mrybs2@gmail.com',
+      url='https://slinn.miotp.ru/',
+      long_description=readme(),
+      long_description_content_type='text/markdown',
+      python_requires='>=3.11',
+      zip_safe=True)
```

### Comparing `slinn-2.2.0/slinn/__init__.py` & `slinn-2.2.2/slinn/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from slinn.address import Address
-from slinn.filter import Filter
-from slinn.link_filter import LinkFilter
-from slinn.any_filter import AnyFilter
-from slinn.file import File
-from slinn.request import Request
-from slinn.http_response import HttpResponse
-from slinn.http_redirect import HttpRedirect
-from slinn.http_api_response import HttpAPIResponse
-from slinn.http_json_response import HttpJSONResponse
-from slinn.http_json_api_response import HttpJSONAPIResponse
-from slinn.server import Server
-from slinn.dispatcher import Dispatcher
-
-version = 'Slinn Murega v2.2.0 230324b'
+from slinn.address import Address
+from slinn.filter import Filter
+from slinn.link_filter import LinkFilter
+from slinn.any_filter import AnyFilter
+from slinn.file import File
+from slinn.request import Request
+from slinn.http_response import HttpResponse
+from slinn.http_redirect import HttpRedirect
+from slinn.http_api_response import HttpAPIResponse
+from slinn.http_json_response import HttpJSONResponse
+from slinn.http_json_api_response import HttpJSONAPIResponse
+from slinn.server import Server
+from slinn.dispatcher import Dispatcher
+
+
+version = 'Slinn Murega v2.2.1 290324a'
```

### Comparing `slinn-2.2.0/slinn/__main__.py` & `slinn-2.2.2/slinn/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,103 +1,105 @@
-import sys, venv
-from slinn.default import *
-
-RED = '\u001b[31m'
-GREEN = '\u001b[32m'
-BLUE = '\u001b[34m'
-RESET = '\u001b[0m'
-BOLD = '\u001b[1m'
-GRAY = '\u001b[38;2;127;127;127m'
-
-if __name__ == '__main__':
-	if len(sys.argv) > 1:
-		if sys.argv[1].lower() == 'create':
-			args = get_args(['path'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			import os, slinn, shutil, platform
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			if not os.path.isdir(apppath):
-				os.mkdir(apppath)
-			else:
-				print(f'{BLUE}{apppath} has already existed{RESET}')
-			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
-			shutil.copyfile(modulepath+'default/project.json', f'{apppath}/project.json')
-			venv.create(f'{apppath}/venv')
-			packages_dir = ''
-			if platform.system() == 'Windows':
-				packages_dir = f'{apppath}/venv/Lib/site-packages'
-			else:
-				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
-			try:
-				os.makedirs(packages_dir)
-			except FileExistsError:
-				pass
-			try:
-				shutil.copytree(modulepath, packages_dir+'/slinn')
-			except FileNotFoundError:
-				print(f'{RED}Cannot install slinn to the new virtual environment{RESET}')
-				exit()
-			try:
-				import pip
-				shutil.copytree(os.path.abspath(pip.__file__).replace('__init__.py', ''), packages_dir+'/pip')
-			except FileNotFoundError:
-				print(f'{BLUE}pip was not installed{RESET}')
-			try:
-				import wheel
-				shutil.copytree(os.path.abspath(wheel.__file__).replace('__init__.py', ''), packages_dir+'/wheel')
-			except Exception:
-				print(f'{BLUE}wheel was not installed{RESET}')
-			try:
-				import setuptools
-				shutil.copytree(os.path.abspath(setuptools.__file__).replace('__init__.py', ''), packages_dir+'/setuptools')
-			except Exception:
-				print(f'{BLUE}setuptools was not installed{RESET}')
-			print(f'{GREEN}Project has created{RESET}')
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			try:
-				shutil.copytree(f'{modulepath}templates/firstrun/', f'{apppath}/firstrun')
-				shutil.copytree(f'{modulepath}templates/firstrun/data/', f'{apppath}/templates_data/firstrun')
-				print(f'{GREEN}Template firstrun successfully installed{RESET}') 
-			except FileExistsError:
-				print(f'{BLUE}Template firstrun has already existed installed{RESET}')
-			except FileNotFoundError:
-				print(f'{BLUE}Template firstrun not found{RESET}')
-		elif sys.argv[1].lower() == 'update':
-			args = get_args(['path'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			import os, slinn, shutil, platform
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			if not os.path.isdir(apppath):
-				print(f'{BLUE}`{apppath}` does not exist{RESET}')
-				exit()
-			packages_dir = ''
-			if platform.system() == 'Windows':
-				packages_dir = f'{apppath}/venv/Lib/site-packages'
-			else:
-				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
-			if not os.path.isdir(packages_dir+'/slinn'):
-				print(f'{RED}Virtual environment directory is corrupted. Reinstall the project{RESET}')
-				exit()
-			if not os.path.isfile(apppath+'/manage.py'):
-				print(f'{RED}manage.py file does not exist. Reinstall the project{RESET}')
-				exit()
-			shutil.rmtree(packages_dir+'/slinn')
-			os.remove(apppath+'/manage.py')
-			shutil.copytree(modulepath, packages_dir+'/slinn')
-			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
-			print(f'{GREEN}Project has updated{RESET}')
-		elif sys.argv[1].lower() == 'help':
-			print("""%BOLD%Slinn help page
-
-Commands%RESET%:
-	%cmd% create {project`s name}		%GRAY%# Creates a new project%RESET%
-	%cmd% update {project`s name}		%GRAY%# Updates the project%RESET%
-	%cmd% help                   		%GRAY%# Prints this help%RESET%
-	%cmd% version                		%GRAY%# Prints version of Slinn%RESET%
-""".replace('%cmd%', f'py -m slinn').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
-		elif sys.argv[1].lower() == 'version':
-			print(slinn_version)
-		else:
-			print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
-	else:
-		print(f'{RED}Command was not specified{RESET}')
-
+import sys, venv
+from slinn.default import *
+
+
+RED = '\u001b[31m'
+GREEN = '\u001b[32m'
+BLUE = '\u001b[34m'
+RESET = '\u001b[0m'
+BOLD = '\u001b[1m'
+GRAY = '\u001b[38;2;127;127;127m'
+
+
+if __name__ == '__main__':
+	if len(sys.argv) > 1:
+		if sys.argv[1].lower() == 'create':
+			args = get_args(['path'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			import os, slinn, shutil, platform
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			if not os.path.isdir(apppath):
+				os.mkdir(apppath)
+			else:
+				print(f'{BLUE}{apppath} has already existed{RESET}')
+			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
+			shutil.copyfile(modulepath+'default/project.json', f'{apppath}/project.json')
+			venv.create(f'{apppath}/venv')
+			packages_dir = ''
+			if platform.system() == 'Windows':
+				packages_dir = f'{apppath}/venv/Lib/site-packages'
+			else:
+				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
+			try:
+				os.makedirs(packages_dir)
+			except FileExistsError:
+				pass
+			try:
+				shutil.copytree(modulepath, packages_dir+'/slinn')
+			except FileNotFoundError:
+				print(f'{RED}Cannot install slinn to the new virtual environment{RESET}')
+				exit()
+			try:
+				import pip
+				shutil.copytree(os.path.abspath(pip.__file__).replace('__init__.py', ''), packages_dir+'/pip')
+			except FileNotFoundError:
+				print(f'{BLUE}pip was not installed{RESET}')
+			try:
+				import wheel
+				shutil.copytree(os.path.abspath(wheel.__file__).replace('__init__.py', ''), packages_dir+'/wheel')
+			except Exception:
+				print(f'{BLUE}wheel was not installed{RESET}')
+			try:
+				import setuptools
+				shutil.copytree(os.path.abspath(setuptools.__file__).replace('__init__.py', ''), packages_dir+'/setuptools')
+			except Exception:
+				print(f'{BLUE}setuptools was not installed{RESET}')
+			print(f'{GREEN}Project has created{RESET}')
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			try:
+				shutil.copytree(f'{modulepath}templates/firstrun/', f'{apppath}/firstrun')
+				shutil.copytree(f'{modulepath}templates/firstrun/data/', f'{apppath}/templates_data/firstrun')
+				print(f'{GREEN}Template firstrun successfully installed{RESET}') 
+			except FileExistsError:
+				print(f'{BLUE}Template firstrun has already existed installed{RESET}')
+			except FileNotFoundError:
+				print(f'{BLUE}Template firstrun not found{RESET}')
+		elif sys.argv[1].lower() == 'update':
+			args = get_args(['path'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			import os, slinn, shutil, platform
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			if not os.path.isdir(apppath):
+				print(f'{BLUE}`{apppath}` does not exist{RESET}')
+				exit()
+			packages_dir = ''
+			if platform.system() == 'Windows':
+				packages_dir = f'{apppath}/venv/Lib/site-packages'
+			else:
+				packages_dir = f'{apppath}/venv/lib/python{".".join(sys.version.split(" ")[0].split(".")[:-1])}/site-packages'
+			if not os.path.isdir(packages_dir+'/slinn'):
+				print(f'{RED}Virtual environment directory is corrupted. Reinstall the project{RESET}')
+				exit()
+			if not os.path.isfile(apppath+'/manage.py'):
+				print(f'{RED}manage.py file does not exist. Reinstall the project{RESET}')
+				exit()
+			shutil.rmtree(packages_dir+'/slinn')
+			os.remove(apppath+'/manage.py')
+			shutil.copytree(modulepath, packages_dir+'/slinn')
+			shutil.copyfile(modulepath+'default/manage.py', f'{apppath}/manage.py')
+			print(f'{GREEN}Project has updated{RESET}')
+		elif sys.argv[1].lower() == 'help':
+			print("""%BOLD%Slinn help page
+
+Commands%RESET%:
+	%cmd% create {project`s name}		%GRAY%# Creates a new project%RESET%
+	%cmd% update {project`s name}		%GRAY%# Updates the project%RESET%
+	%cmd% help                   		%GRAY%# Prints this help%RESET%
+	%cmd% version                		%GRAY%# Prints version of Slinn%RESET%
+""".replace('%cmd%', f'py -m slinn').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
+		elif sys.argv[1].lower() == 'version':
+			print(slinn_version)
+		else:
+			print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
+	else:
+		print(f'{RED}Command was not specified{RESET}')
+
```

### Comparing `slinn-2.2.0/slinn/default/manage.py` & `slinn-2.2.2/slinn/default/manage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,364 +1,364 @@
-import sys, os, shutil, json, base64
-from slinn import version as slinn_version
-import slinn
-
-RED = '\u001b[31m'
-GREEN = '\u001b[32m'
-BLUE = '\u001b[34m'
-RESET = '\u001b[0m'
-BOLD = '\u001b[1m'
-GRAY = '\u001b[38;2;127;127;127m'
-
-
-def arg_parse(arg: str):
-	return base64.urlsafe_b64decode(arg.removeprefix('b64@').encode()+b'==').decode() if arg.startswith('b64@') else arg
-
-def splits(string: str, delimeters: list[str]=[' ', '\n'], quotes: list[str]=[]):
-		result = ['']
-		current_quote = ''
-		for char in str(string):
-			if char in quotes:
-				if current_quote == '':
-					current_quote = char
-					continue
-				elif current_quote == char:
-					current_quote = ''
-					continue
-			if current_quote == '':
-				if char in delimeters:
-					result.append('')
-				else:
-					result[-1] += char
-			else:
-				result[-1] += char
-		return result
-
-def get_args(expecting, text):
-	text = text.strip()
-	if text == '':
-		return {}
-	args = {'not_used': []}
-	Ds = ['\n', ' ']
-	Qs = ['"', "'", '`']
-	spls  = splits(text, Ds, Qs)
-	i = 0
-	while i < len(spls):
-		arg = str(spls[i])
-		try:
-			if arg.strip().endswith('='):
-				W = arg.strip().removesuffix('=').strip()
-				expecting.pop(expecting.index(W))
-				args[W] = arg_parse(str(splits[i + 1]))
-				i += 2
-				continue
-			if len(splits(arg, ['='], Qs)) == 2:
-				spl = splits(arg, ['='])
-				W = str(spl[0])
-				if W not in args.keys():
-					args[W] = arg_parse(str(spl[1]))
-					expecting.pop(expecting.index(W))
-				else:
-					args[W] = [args[W]]
-					args[W].append(arg_parse(str(spl[1])))
-				i += 1
-				continue
-		except ValueError:
-			pass
-
-		if len(expecting) == 0:
-			args['not_used'].append(arg_parse(arg))
-			i += 1
-			continue
-
-		E = expecting.pop(0)
-		args[E] = arg_parse(arg)
-		i += 1
-	return args
-
-def replace_all(text: str, sss: list[str] | str, ss2: str) -> str:
-	for ss1 in sss:
-		text = text.replace(ss1, ss2)
-	return text
-
-def add_quotes_to_list(lst: list[str]):
-		for l in lst:
-			yield f'\'{l}\''
-
-def update():
-	project = open('project.json', 'r')
-	project_json = json.loads(project.read())
-	project.close()
-	if 'apps' not in project_json.keys():
-		return print(f'Updated project.json')
-	apps = []
-	for app in project_json['apps']:
-		if os.path.isdir(app):
-			apps.append(app)
-	project_json['apps'] = apps
-	project = open('project.json', 'w')
-	project.write(json.dumps(project_json, indent=4))
-	project.close()
-	return print(f'Updated project.json')
-
-def main():
-	if len(sys.argv) > 1:
-		if sys.argv[1].lower() == 'run':
-			from slinn import Server, Address
-
-			def config():
-				file = open('project.json')
-				cfg = json.loads(file.read())
-				file.close()
-				return cfg
-			
-			def app_config(app):
-				try:
-					cfg = {"debug": False}
-					file = open(f'{app}/config.json')
-					cfg.update(json.loads(file.read()))
-					file.close()
-					return cfg
-				except FileNotFoundError:
-					print(f'{RED}{app}/config.json file not found{RESET}')
-					exit()
-
-
-			def load_imports(apps, debug=False):
-				imports = []
-				for app in apps:
-					if not app_config(app)['debug'] or debug:
-						imports.append(f'import {app}')
-				return imports
-
-
-			def get_dispatchers(apps, debug=False):
-				dispachers = []
-				for app in apps:
-					if not app_config(app)['debug'] or debug:
-						dispachers.append(f'{app}.dp')
-				return dispachers
-			
-			def app_reload(app):
-				return f'global {app};{app} = importlib.reload({app});'
-			
-			print('Loading config...')
-			cfg = config()
-			debug = cfg["debug"] if "debug" in cfg.keys() else False
-			apps = cfg['apps'] if 'apps' in cfg.keys() else []
-			port = cfg['port'] if 'port' in cfg.keys() else 8080
-			host = cfg['host'] if 'host' in cfg.keys() else ''
-			delay = float(cfg['delay']) if 'delay' in cfg.keys() else 0.05
-			timeout = float(cfg['timeout']) if 'timeout' in cfg.keys() else 0.03
-			max_bytes_per_recieve = int(cfg['max_bytes_per_recieve']) if 'max_bytes_per_recieve' in cfg.keys() else 4096
-			max_bytes = int(cfg['max_bytes']) if 'max_bytes' in cfg.keys() else 4294967296
-			smart_navigation = cfg['smart_navigation'] if 'smart_navigation' in cfg.keys() else True
-			ssl_fullchain, ssl_key = None, None
-			if 'ssl' in cfg.keys() and 'fullchain' in cfg['ssl'].keys() and 'key' in cfg['ssl'].keys():
-				ssl_fullchain = '"'+cfg['ssl']['fullchain']+'"' if cfg['ssl']['fullchain'] else None    
-				ssl_key = '"'+cfg['ssl']['key']+'"' if cfg['ssl']['key'] else None
-			dps = get_dispatchers(apps, debug)
-			if dps == []:
-				print(f'{RED}Dispatchers not found. Check your apps and ./project.json{RESET}')
-				exit()
-			global get_dir_checksum
-			def get_dir_checksum(dir):
-				import hashlib
-				def get_dir_checksums(dir):
-					def md5(fname):
-						hash_md5 = hashlib.md5()
-						with open(fname, "rb") as f:
-							for chunk in iter(lambda: f.read(4096), b""):
-								hash_md5.update(chunk)
-						return hash_md5.hexdigest()
-					paths = os.listdir(dir)
-					checksums = []
-					for path in paths:
-						if os.path.isdir(path):
-							checksums += get_dir_checksums(dir+'/'+path)
-						elif path.endswith('.py'):
-							checksums.append(path+md5(dir+'/'+path))
-					return checksums
-				return hashlib.md5(''.join([checksum for checksum in get_dir_checksums(dir)]).encode()).hexdigest()
-			global checksum
-			checksum = get_dir_checksum('.')
-			reloader = """
-def reloader(server, delay=0.3):
-	import time, importlib
-	def runtime(delay, server):
-		global checksum
-		while True:
-			if checksum != get_dir_checksum('.'):
-				checksum = get_dir_checksum('.')
-				"""
-			for app in cfg['apps']:
-				if not app_config(app)['debug'] or debug:
-					reloader += app_reload(app)
-			reloader += """
-				print('\\n\\nServer updated')
-				print(server.address())
-				server.reload("""
-			reloader += ",".join(dps)
-			reloader += """)
-			time.sleep(delay)
-	import threading;threading.Thread(target=runtime, args=(delay, server)).start()
-"""
-			apps_info = []
-			for app in cfg['apps']:
-				if not app_config(app)['debug'] or debug:
-					apps_info.append(app)
-				else:
-					apps_info.append('['+app+']')
-			print(f'{GRAY}Apps: ' + ', '.join(apps_info))
-			print('Debug mode ' + 'enabled' if debug else 'disabled')
-			print('Smart navigation ' + ('enabled' if smart_navigation else 'disabled'))
-			print(f'Delay: {str(delay*1000)}ms')
-			print(RESET)
-
-			print('Starting server...')
-			start = ';'.join(load_imports(apps, debug))+reloader+f'server=Server({",".join(dps)}, smart_navigation={smart_navigation}, ssl_fullchain={ssl_fullchain}, ssl_key={ssl_key}, delay={delay}, timeout={timeout}, max_bytes_per_recieve={max_bytes_per_recieve}, max_bytes={max_bytes});reloader(server=server);server.listen(Address({port}, "{host}"))'
-			exec(start)
-		elif sys.argv[1].lower() == 'create':
-			args = get_args(['name', 'host'], ' '.join(sys.argv[2:]))
-			if 'name' not in args.keys():
-				return print(f'{RED}The app`s name is not specified{RESET}')
-			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
-			if os.path.isdir(ensure_appname):
-				return print(f'{BLUE}The app named {args["name"]} exists{RESET}')
-			if 'host' not in args.keys():
-				print(f'{BLUE}Hosts were not specified')
-			os.mkdir(ensure_appname)
-			with open(f'{ensure_appname}/__init__.py', 'w') as f:
-				data = """import sys, importlib
-if '%appname%.app' not in sys.modules.keys():
-    from %appname%.app import dp
-else:
-    dp = importlib.reload(sys.modules['%appname%.app']).dp
-""".replace('%appname%', ensure_appname)
-				f.write(data)
-			with open(f'{ensure_appname}/app.py', 'w') as f:
-				data = """from slinn import Dispatcher, Filter, HttpResponse
- 
-dp = Dispatcher(%hosts%)
-
-# Write your code down here                         
-""".replace('%appname%', ensure_appname).replace('%hosts%', '' if 'host' not in args.keys() else ', '.join(add_quotes_to_list(args['host'] if type(args['host']) == list else [args['host']])))
-				f.write(data)
-			with open(f'{ensure_appname}/config.json', 'w') as f:
-				data = """
-{
-	"debug": false
-}
-"""
-				f.write(data)
-			fr = open('project.json', 'r')
-			fj = json.loads(fr.read())
-			fr.close()
-			if 'apps' in fj.keys():
-				fj['apps'].insert(0, ensure_appname)
-			else:
-				fj['apps'] = []
-			fw = open('project.json', 'w')
-			fw.write(json.dumps(fj, indent=4))
-			fw.close()
-			update()
-			print(f'{GREEN}App successfully created{RESET}')
-		elif sys.argv[1].lower() == 'delete':
-			args = get_args(['name'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			if 'name' not in args.keys():
-				return print(f'{RED}The app`s name is not specified{RESET}')
-			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
-			if not os.path.isdir(ensure_appname):
-				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
-			if input(f'{RESET}Are you sure? (y/N) >>> ').lower() not in ['y', 'yes']:
-				return print(f'{RESET}Aborted')
-			shutil.rmtree(ensure_appname)
-			if os.path.isdir(f'{apppath}/templates_data/{ensure_appname}'):
-				shutil.rmtree(f'{apppath}/templates_data/{ensure_appname}')
-			if len(os.listdir('{apppath}/templates_data')) == 0:
-				shutil.rmtree(f'{apppath}/templates_data')
-			update()
-			return print(f'{GREEN}App successfully deleted{RESET}')
-		elif sys.argv[1].lower() == 'update':
-			return update()
-		elif sys.argv[1].lower() == 'help':
-			return print("""%BOLD%Slinn manager help page
-
-Commands%RESET%:
-	%cmd% run                                                              %GRAY%# Starts server%RESET%
-	%cmd% create {app`s name} host=(host1) host=(host2)...                 %GRAY%# Creates a new app
-		Example: %cmd% create localhost host=localhost host=127.0.0.1%RESET%
-	%cmd% delete {app`s name} (project`s path)                             %GRAY%# Deletes an app
-		Example: %cmd% delete localhost%RESET%
-	%cmd% template {template`s name} (projects`s path)                     %GRAY%# Installs a template
-		Example: %cmd% template firstrun%RESET%
-	%cmd% update                                                           %GRAY%# Updates project.py%RESET%
-	%cmd% migrate_app {app`s name}                                         %GRAY%# Migrates app(check slinn.guides.migration1xx2xx.migration1xx2xx)%RESET
-	%cmd% help                                                             %GRAY%# Prints this help%RESET%
-	%cmd% version                                                          %GRAY%# Prints version of Slinn%RESET%
-""".replace('%cmd%', f'py {sys.argv[0]}').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
-		elif sys.argv[1].lower() == 'version':
-			return print(slinn_version)
-		elif sys.argv[1].lower() == 'template':
-			args = get_args(['name', 'path'], ' '.join(sys.argv[2:]))
-			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
-			if 'name' not in args.keys():
-				return print(f'{RED}Template name is not specified{RESET}')
-			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
-			fr = open('project.json', 'r')
-			fj = json.loads(fr.read())
-			fr.close()
-			if 'apps' in fj.keys():
-				fj['apps'].insert(0, args['name'])
-			else:
-				fj['apps'] = []
-			fw = open('project.json', 'w')
-			fw.write(json.dumps(fj, indent=4))
-			fw.close()
-			update()
-			try:
-				shutil.copytree(f'{modulepath}templates/{args["name"]}/', f'{apppath}/{args["name"]}')
-				try:
-					if not os.isdir(f'{apppath}/templates_data'):
-						os.mkdir(f'{apppath}/templates_data')
-					shutil.copytree(f'{modulepath}templates/{args["name"]}/data/', f'{apppath}/templates_data/{args["name"]}')
-				except  FileExistsError:
-					pass
-				except FileNotFoundError:
-					pass
-				return print(f'{GREEN}Template {args["name"]} successfully installed{RESET}') 
-			except FileExistsError:
-				return print(f'{BLUE}Template {args["name"]} has already installed{RESET}')
-			except FileNotFoundError:
-				return print(f'{BLUE}Template {args["name"]} not found{RESET}')
-		elif sys.argv[1].lower() == 'migrate_app':
-			args = get_args(['name'], ' '.join(sys.argv[2:]))
-			if 'name' not in args.keys():
-				return print(f'{RED}The app`s name is not specified{RESET}')
-			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
-			if not os.path.isdir(ensure_appname):
-				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
-			with open(f'{ensure_appname}/__init__.py', 'w') as f:
-				data = """import sys, importlib
-if '%appname%.app' not in sys.modules.keys():
-    from %appname%.app import dp
-else:
-    dp = importlib.reload(sys.modules['%appname%.app']).dp
-""".replace('%appname%', ensure_appname)
-				f.write(data)
-			with open(f'{ensure_appname}/config.json', 'w') as f:
-				data = """
-{
-	"debug": false
-}
-"""
-				f.write(data)
-			print(f'{GREEN}App successfully migrated{RESET}')
-		else:
-			return print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
-	else:
-		return print(f'{RED}Command was not specified{RESET}')
-
-			
-if __name__ == '__main__':
+import sys, os, shutil, json, base64
+from slinn import version as slinn_version
+import slinn
+
+RED = '\u001b[31m'
+GREEN = '\u001b[32m'
+BLUE = '\u001b[34m'
+RESET = '\u001b[0m'
+BOLD = '\u001b[1m'
+GRAY = '\u001b[38;2;127;127;127m'
+
+
+def arg_parse(arg: str):
+	return base64.urlsafe_b64decode(arg.removeprefix('b64@').encode()+b'==').decode() if arg.startswith('b64@') else arg
+
+def splits(string: str, delimeters: list[str]=[' ', '\n'], quotes: list[str]=[]):
+		result = ['']
+		current_quote = ''
+		for char in str(string):
+			if char in quotes:
+				if current_quote == '':
+					current_quote = char
+					continue
+				elif current_quote == char:
+					current_quote = ''
+					continue
+			if current_quote == '':
+				if char in delimeters:
+					result.append('')
+				else:
+					result[-1] += char
+			else:
+				result[-1] += char
+		return result
+
+def get_args(expecting, text):
+	text = text.strip()
+	if text == '':
+		return {}
+	args = {'not_used': []}
+	Ds = ['\n', ' ']
+	Qs = ['"', "'", '`']
+	spls  = splits(text, Ds, Qs)
+	i = 0
+	while i < len(spls):
+		arg = str(spls[i])
+		try:
+			if arg.strip().endswith('='):
+				W = arg.strip().removesuffix('=').strip()
+				expecting.pop(expecting.index(W))
+				args[W] = arg_parse(str(splits[i + 1]))
+				i += 2
+				continue
+			if len(splits(arg, ['='], Qs)) == 2:
+				spl = splits(arg, ['='])
+				W = str(spl[0])
+				if W not in args.keys():
+					args[W] = arg_parse(str(spl[1]))
+					expecting.pop(expecting.index(W))
+				else:
+					args[W] = [args[W]]
+					args[W].append(arg_parse(str(spl[1])))
+				i += 1
+				continue
+		except ValueError:
+			pass
+
+		if len(expecting) == 0:
+			args['not_used'].append(arg_parse(arg))
+			i += 1
+			continue
+
+		E = expecting.pop(0)
+		args[E] = arg_parse(arg)
+		i += 1
+	return args
+
+def replace_all(text: str, sss: list[str] | str, ss2: str) -> str:
+	for ss1 in sss:
+		text = text.replace(ss1, ss2)
+	return text
+
+def add_quotes_to_list(lst: list[str]):
+		for l in lst:
+			yield f'\'{l}\''
+
+def update():
+	project = open('project.json', 'r')
+	project_json = json.loads(project.read())
+	project.close()
+	if 'apps' not in project_json.keys():
+		return print(f'Updated project.json')
+	apps = []
+	for app in project_json['apps']:
+		if os.path.isdir(app):
+			apps.append(app)
+	project_json['apps'] = apps
+	project = open('project.json', 'w')
+	project.write(json.dumps(project_json, indent=4))
+	project.close()
+	return print(f'Updated project.json')
+
+def main():
+	if len(sys.argv) > 1:
+		if sys.argv[1].lower() == 'run':
+			from slinn import Server, Address
+
+			def config():
+				file = open('project.json')
+				cfg = json.loads(file.read())
+				file.close()
+				return cfg
+			
+			def app_config(app):
+				try:
+					cfg = {"debug": False}
+					file = open(f'{app}/config.json')
+					cfg.update(json.loads(file.read()))
+					file.close()
+					return cfg
+				except FileNotFoundError:
+					print(f'{RED}{app}/config.json file not found{RESET}')
+					exit()
+
+
+			def load_imports(apps, debug=False):
+				imports = []
+				for app in apps:
+					if not app_config(app)['debug'] or debug:
+						imports.append(f'import {app}')
+				return imports
+
+
+			def get_dispatchers(apps, debug=False):
+				dispachers = []
+				for app in apps:
+					if not app_config(app)['debug'] or debug:
+						dispachers.append(f'{app}.dp')
+				return dispachers
+			
+			def app_reload(app):
+				return f'global {app};{app} = importlib.reload({app});'
+			
+			print('Loading config...')
+			cfg = config()
+			debug = cfg["debug"] if "debug" in cfg.keys() else False
+			apps = cfg['apps'] if 'apps' in cfg.keys() else []
+			port = cfg['port'] if 'port' in cfg.keys() else 8080
+			host = cfg['host'] if 'host' in cfg.keys() else ''
+			delay = float(cfg['delay']) if 'delay' in cfg.keys() else 0.05
+			timeout = float(cfg['timeout']) if 'timeout' in cfg.keys() else 0.03
+			max_bytes_per_recieve = int(cfg['max_bytes_per_recieve']) if 'max_bytes_per_recieve' in cfg.keys() else 4096
+			max_bytes = int(cfg['max_bytes']) if 'max_bytes' in cfg.keys() else 4294967296
+			smart_navigation = cfg['smart_navigation'] if 'smart_navigation' in cfg.keys() else True
+			ssl_fullchain, ssl_key = None, None
+			if 'ssl' in cfg.keys() and 'fullchain' in cfg['ssl'].keys() and 'key' in cfg['ssl'].keys():
+				ssl_fullchain = '"'+cfg['ssl']['fullchain']+'"' if cfg['ssl']['fullchain'] else None    
+				ssl_key = '"'+cfg['ssl']['key']+'"' if cfg['ssl']['key'] else None
+			dps = get_dispatchers(apps, debug)
+			if dps == []:
+				print(f'{RED}Dispatchers not found. Check your apps and ./project.json{RESET}')
+				exit()
+			global get_dir_checksum
+			def get_dir_checksum(dir):
+				import hashlib
+				def get_dir_checksums(dir):
+					def md5(fname):
+						hash_md5 = hashlib.md5()
+						with open(fname, "rb") as f:
+							for chunk in iter(lambda: f.read(4096), b""):
+								hash_md5.update(chunk)
+						return hash_md5.hexdigest()
+					paths = os.listdir(dir)
+					checksums = []
+					for path in paths:
+						if os.path.isdir(path):
+							checksums += get_dir_checksums(dir+'/'+path)
+						elif path.endswith('.py'):
+							checksums.append(path+md5(dir+'/'+path))
+					return checksums
+				return hashlib.md5(''.join([checksum for checksum in get_dir_checksums(dir)]).encode()).hexdigest()
+			global checksum
+			checksum = get_dir_checksum('.')
+			reloader = """
+def reloader(server, delay=0.3):
+	import time, importlib
+	def runtime(delay, server):
+		global checksum
+		while True:
+			if checksum != get_dir_checksum('.'):
+				checksum = get_dir_checksum('.')
+				"""
+			for app in cfg['apps']:
+				if not app_config(app)['debug'] or debug:
+					reloader += app_reload(app)
+			reloader += """
+				print('\\n\\nServer updated')
+				print(server.address())
+				server.reload("""
+			reloader += ",".join(dps)
+			reloader += """)
+			time.sleep(delay)
+	import threading;threading.Thread(target=runtime, args=(delay, server)).start()
+"""
+			apps_info = []
+			for app in cfg['apps']:
+				if not app_config(app)['debug'] or debug:
+					apps_info.append(app)
+				else:
+					apps_info.append('['+app+']')
+			print(f'{GRAY}Apps: ' + ', '.join(apps_info))
+			print('Debug mode ' + 'enabled' if debug else 'disabled')
+			print('Smart navigation ' + ('enabled' if smart_navigation else 'disabled'))
+			print(f'Delay: {str(delay*1000)}ms')
+			print(RESET)
+
+			print('Starting server...')
+			start = ';'.join(load_imports(apps, debug))+reloader+f'server=Server({",".join(dps)}, smart_navigation={smart_navigation}, ssl_fullchain={ssl_fullchain}, ssl_key={ssl_key}, delay={delay}, timeout={timeout}, max_bytes_per_recieve={max_bytes_per_recieve}, max_bytes={max_bytes});reloader(server=server);server.listen(Address({port}, "{host}"))'
+			exec(start)
+		elif sys.argv[1].lower() == 'create':
+			args = get_args(['name', 'host'], ' '.join(sys.argv[2:]))
+			if 'name' not in args.keys():
+				return print(f'{RED}The app`s name is not specified{RESET}')
+			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
+			if os.path.isdir(ensure_appname):
+				return print(f'{BLUE}The app named {args["name"]} exists{RESET}')
+			if 'host' not in args.keys():
+				print(f'{BLUE}Hosts were not specified')
+			os.mkdir(ensure_appname)
+			with open(f'{ensure_appname}/__init__.py', 'w') as f:
+				data = """import sys, importlib
+if '%appname%.app' not in sys.modules.keys():
+    from %appname%.app import dp
+else:
+    dp = importlib.reload(sys.modules['%appname%.app']).dp
+""".replace('%appname%', ensure_appname)
+				f.write(data)
+			with open(f'{ensure_appname}/app.py', 'w') as f:
+				data = """from slinn import Dispatcher, Filter, HttpResponse
+ 
+dp = Dispatcher(%hosts%)
+
+# Write your code down here                         
+""".replace('%appname%', ensure_appname).replace('%hosts%', '' if 'host' not in args.keys() else ', '.join(add_quotes_to_list(args['host'] if type(args['host']) == list else [args['host']])))
+				f.write(data)
+			with open(f'{ensure_appname}/config.json', 'w') as f:
+				data = """
+{
+	"debug": false
+}
+"""
+				f.write(data)
+			fr = open('project.json', 'r')
+			fj = json.loads(fr.read())
+			fr.close()
+			if 'apps' in fj.keys():
+				fj['apps'].insert(0, ensure_appname)
+			else:
+				fj['apps'] = []
+			fw = open('project.json', 'w')
+			fw.write(json.dumps(fj, indent=4))
+			fw.close()
+			update()
+			print(f'{GREEN}App successfully created{RESET}')
+		elif sys.argv[1].lower() == 'delete':
+			args = get_args(['name'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			if 'name' not in args.keys():
+				return print(f'{RED}The app`s name is not specified{RESET}')
+			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
+			if not os.path.isdir(ensure_appname):
+				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
+			if input(f'{RESET}Are you sure? (y/N) >>> ').lower() not in ['y', 'yes']:
+				return print(f'{RESET}Aborted')
+			shutil.rmtree(ensure_appname)
+			if os.path.isdir(f'{apppath}/templates_data/{ensure_appname}'):
+				shutil.rmtree(f'{apppath}/templates_data/{ensure_appname}')
+			if len(os.listdir(f'{apppath}/templates_data')) == 0:
+				shutil.rmtree(f'{apppath}/templates_data')
+			update()
+			return print(f'{GREEN}App successfully deleted{RESET}')
+		elif sys.argv[1].lower() == 'update':
+			return update()
+		elif sys.argv[1].lower() == 'help':
+			return print("""%BOLD%Slinn manager help page
+
+Commands%RESET%:
+	%cmd% run                                                              %GRAY%# Starts server%RESET%
+	%cmd% create {app`s name} host=(host1) host=(host2)...                 %GRAY%# Creates a new app
+		Example: %cmd% create localhost host=localhost host=127.0.0.1%RESET%
+	%cmd% delete {app`s name} (project`s path)                             %GRAY%# Deletes an app
+		Example: %cmd% delete localhost%RESET%
+	%cmd% template {template`s name} (projects`s path)                     %GRAY%# Installs a template
+		Example: %cmd% template firstrun%RESET%
+	%cmd% update                                                           %GRAY%# Updates project.py%RESET%
+	%cmd% migrate_app {app`s name}                                         %GRAY%# Migrates app(check slinn.guides.migration1xx2xx.migration1xx2xx)%RESET%
+	%cmd% help                                                             %GRAY%# Prints this help%RESET%
+	%cmd% version                                                          %GRAY%# Prints version of Slinn%RESET%
+""".replace('%cmd%', f'py {sys.argv[0]}').replace('%GRAY%', GRAY).replace('%RESET%', RESET).replace('%BOLD%', BOLD))
+		elif sys.argv[1].lower() == 'version':
+			return print(slinn_version)
+		elif sys.argv[1].lower() == 'template':
+			args = get_args(['name', 'path'], ' '.join(sys.argv[2:]))
+			apppath = (args['path']+'?').replace('/?', '').replace('?', '') if 'path' in args.keys() else '.'
+			if 'name' not in args.keys():
+				return print(f'{RED}Template name is not specified{RESET}')
+			modulepath = os.path.abspath(slinn.__file__).replace('__init__.py', '')
+			fr = open('project.json', 'r')
+			fj = json.loads(fr.read())
+			fr.close()
+			if 'apps' in fj.keys():
+				fj['apps'].insert(0, args['name'])
+			else:
+				fj['apps'] = []
+			fw = open('project.json', 'w')
+			fw.write(json.dumps(fj, indent=4))
+			fw.close()
+			update()
+			try:
+				shutil.copytree(f'{modulepath}templates/{args["name"]}/', f'{apppath}/{args["name"]}')
+				try:
+					if not os.isdir(f'{apppath}/templates_data'):
+						os.mkdir(f'{apppath}/templates_data')
+					shutil.copytree(f'{modulepath}templates/{args["name"]}/data/', f'{apppath}/templates_data/{args["name"]}')
+				except  FileExistsError:
+					pass
+				except FileNotFoundError:
+					pass
+				return print(f'{GREEN}Template {args["name"]} successfully installed{RESET}') 
+			except FileExistsError:
+				return print(f'{BLUE}Template {args["name"]} has already installed{RESET}')
+			except FileNotFoundError:
+				return print(f'{BLUE}Template {args["name"]} not found{RESET}')
+		elif sys.argv[1].lower() == 'migrate_app':
+			args = get_args(['name'], ' '.join(sys.argv[2:]))
+			if 'name' not in args.keys():
+				return print(f'{RED}The app`s name is not specified{RESET}')
+			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
+			if not os.path.isdir(ensure_appname):
+				return print(f'{BLUE}The app named {args["name"]} does not exist{RESET}')
+			with open(f'{ensure_appname}/__init__.py', 'w') as f:
+				data = """import sys, importlib
+if '%appname%.app' not in sys.modules.keys():
+    from %appname%.app import dp
+else:
+    dp = importlib.reload(sys.modules['%appname%.app']).dp
+""".replace('%appname%', ensure_appname)
+				f.write(data)
+			with open(f'{ensure_appname}/config.json', 'w') as f:
+				data = """
+{
+	"debug": false
+}
+"""
+				f.write(data)
+			print(f'{GREEN}App successfully migrated{RESET}')
+		else:
+			return print(f'{RED}Command {sys.argv[1].lower()} is not exists{RESET}')
+	else:
+		return print(f'{RED}Command was not specified{RESET}')
+
+			
+if __name__ == '__main__':
 	main()
```

### Comparing `slinn-2.2.0/slinn/guides/migration1xx2xx.py` & `slinn-2.2.2/slinn/guides/migration1xx2xx.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0)
-
-Firstly, change all your @dp_xxx.route(...) to @dp_xxx(...)
-Then, you should change some filters from Filter to AnyFilter or LinkFilter where it is suit
-If you have troubles with Smart Navigation, then specify '{"smart_navigation": false}' in your project.json
-
-If you want support of autoreloading your app, follow these steps:
-- Change dp_xxx = Dispatcher(...) to dp = Dispatcher(...) and @dp_xxx.route(...) to @dp(...) OR dp = dp_xxx in the end of the file
-- Execute `py manage.py migrate_app {app`s name}`
+migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0)
+
+Firstly, change all your @dp_xxx.route(...) to @dp_xxx(...)
+Then, you should change some filters from Filter to AnyFilter or LinkFilter where it is suit
+If you have troubles with Smart Navigation, then specify '{"smart_navigation": false}' in your project.json
+
+If you want support of autoreloading your app, follow these steps:
+- Change dp_xxx = Dispatcher(...) to dp = Dispatcher(...) and @dp_xxx.route(...) to @dp(...) OR dp = dp_xxx in the end of the file
+- Execute `py manage.py migrate_app {app`s name}`
 """
```

### Comparing `slinn-2.2.0/slinn/http_api_response.py` & `slinn-2.2.2/slinn/http_api_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from slinn.http_response import HttpResponse
-
-class HttpAPIResponse(HttpResponse):
-	def __init__(self, payload, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
-		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
-		default_data = [('Server', 'Slinn'), ('Content-Type', content_type), ('Access-Control-Allow-Origin', '*')]
-		self.data = default_data + data if data is not None else default_data + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
-		self.status = status
+from slinn.http_response import HttpResponse
+
+
+class HttpAPIResponse(HttpResponse):
+	def __init__(self, payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
+		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
+		default_data = [('Server', 'Slinn'), ('Content-Type', content_type), ('Access-Control-Allow-Origin', '*')]
+		self.data = default_data + data if data is not None else default_data + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
+		self.status = status
```

### Comparing `slinn-2.2.0/slinn/http_response.py` & `slinn-2.2.2/slinn/http_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-class HttpResponse:
-	def __init__(self, payload, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
-		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
-		self.data = data if data is not None else [('Content-Type', content_type), ('Server', 'Slinn')] + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
-		self.status = status
-	
-	def set_cookie(self, key: str, value):
-		self.data.append(('Set-Cookie', f'{key}={value}'))
-	
-	def make(self, type: str='HTTP/2.0') -> str:
+class HttpResponse:
+	def __init__(self, payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain'):
+		self.payload = str(payload).encode() if type(payload) in [str, int, float, bool, dict] else bytes(payload)
+		self.data = data if data is not None else [('Content-Type', content_type), ('Server', 'Slinn')] + ([] if type(payload) in [str, int, float, bool, dict] else [('Content-Length', len(self.payload))])
+		self.status = status
+	
+	def set_cookie(self, key: str, value: any):
+		self.data.append(('Set-Cookie', f'{key}={value}'))
+	
+	def make(self, type: str='HTTP/2.0') -> str:
 		return (f'{type} {self.status}'+'\r\n'+"\r\n".join([str(dat[0])+": "+str(dat[1]) for dat in self.data])+'\r\n\r\n').encode()+self.payload
```

### Comparing `slinn-2.2.0/slinn/request.py` & `slinn-2.2.2/slinn/request.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import urllib.parse
-from slinn import File
-
-class Request:	
-	RESET = '\u001b[0m'
-	GRAY = '\u001b[38;2;127;127;127m'
-
-	@staticmethod
-	def parse_http_header(http_header: str):
-		result = {}
-		for line in http_header.split('\r\n'):
-			key, value = line.split(':')[0], ':'.join(line.split(':')[1:])
-			result[key.strip()] = value.strip()
-		return result
-	
-	@staticmethod
-	def parse_http_body(http_body: bytes):
-		files = [File()]
-		BGNs = [b'-----------------------------', b'------WebKitFormBoundary']
-		END = b'--'
-		binary = 0
-		for line in http_body.split(b'\r\n'):
-			if binary != 2:
-				if line == b'':
-					binary += 1
-				elif b':' in line:
-					key, value = line.split(b':')[0].decode(), b':'.join(line.split(b':')[1:])
-					files[-1].header[key.strip()] = value.strip()
-				elif files[-1].id is None:
-					if line.startswith(BGNs[0]):
-						files[-1].id = line[len(BGNs[0]):]
-					elif line.startswith(BGNs[1]):
-						files[-1].id = line[len(BGNs[1]):]
-				continue
-			if files[-1].id is not None:
-				if line.startswith(BGNs[0]) and line.endswith(END) and line[len(BGNs[0]):-len(END)] == files[-1].id \
-				   or line.startswith(BGNs[1]) and line.endswith(END) and line[len(BGNs[1]):-len(END)] == files[-1].id:
-					files[-1].data = bytes(files[-1].data[:-2])
-					files.append(File())
-					binary = 0
-					continue
-			files[-1].data += line + b'\r\n'
-		return files[:-1]
-
-	def __init__(self, header: str, body: bytes, client_address: tuple[str, int]):
-		def get_args(text):
-				return {} if text == '' else {pair.split('=')[0]: '='.join(pair.split('=')[1:]) for pair in text.split('&')}
-		
-		self.type = header.split('\n')[0].strip().replace('\r','').split(' ')
-		self.header = {'method': self.type[0], 'link': ' '.join(self.type[1:-1]), 'ver': self.type[-1], 'data': {'user-agent': '', 'Accept': '', 'Accept-Encoding': '', 'Accept-Language': ''}}
-		header = self.parse_http_header(header)
-		self.files = self.parse_http_body(body)
-		self.header['data'].update(header)
-		self.ip, self.port = client_address[:2]
-		self.method = self.header['method']
-		self.version = self.header["ver"]
-		self.full_link = urllib.parse.unquote(self.header["link"].replace('+', ' '))
-		self.host = self.header["data"]["Host"]
-		self.user_agent = self.header["data"]["User-Agent"] if 'User-Agent' in self.header['data'].keys() else self.header['data']['user-agent']
-		self.accept = self.header["data"]["Accept"].split(',')
-		self.encoding = self.header["data"]["Accept-Encoding"].split(',')
-		self.language = self.header["data"]["Accept-Language"].split(',')
-		self.link = self.full_link[:(self.full_link.index('?') if '?' in self.full_link else None)]
-		self.args = get_args(self.full_link[(self.full_link.index('?')+1 if '?' in self.full_link else len(self.full_link)):])
-		self.cookies = {c.split('=')[0]:c.split('=')[1] for c in self.header["data"]["Cookie"].split(';')} if 'Cookie' in self.header['data'] else []
-
-	def __str__(self):
-		return f'{self.GRAY}[{self.method}]{self.RESET} request {self.full_link} from {"" if "." in self.ip else "["}{self.ip}{"" if "." in self.ip else "]"}:{self.port} on {self.host}'
+import urllib.parse
+from slinn import File
+
+class Request:	
+	RESET = '\u001b[0m'
+	GRAY = '\u001b[38;2;127;127;127m'
+
+	@staticmethod
+	def parse_http_header(http_header: str):
+		result = {}
+		for line in http_header.split('\r\n'):
+			key, value = line.split(':')[0], ':'.join(line.split(':')[1:])
+			result[key.strip()] = value.strip()
+		return result
+	
+	@staticmethod
+	def parse_http_body(http_body: bytes):
+		files = [File()]
+		BGNs = [b'-----------------------------', b'------WebKitFormBoundary']
+		END = b'--'
+		binary = 0
+		for line in http_body.split(b'\r\n'):
+			if binary != 2:
+				if line == b'':
+					binary += 1
+				elif b':' in line:
+					key, value = line.split(b':')[0].decode(), b':'.join(line.split(b':')[1:])
+					files[-1].header[key.strip()] = value.strip()
+				elif files[-1].id is None:
+					if line.startswith(BGNs[0]):
+						files[-1].id = line[len(BGNs[0]):]
+					elif line.startswith(BGNs[1]):
+						files[-1].id = line[len(BGNs[1]):]
+				continue
+			if files[-1].id is not None:
+				if line.startswith(BGNs[0]) and line.endswith(END) and line[len(BGNs[0]):-len(END)] == files[-1].id \
+				   or line.startswith(BGNs[1]) and line.endswith(END) and line[len(BGNs[1]):-len(END)] == files[-1].id:
+					files[-1].data = bytes(files[-1].data[:-2])
+					files.append(File())
+					binary = 0
+					continue
+			files[-1].data += line + b'\r\n'
+		return files[:-1]
+
+	def __init__(self, header: str, body: bytes, client_address: tuple[str, int]):
+		def get_args(text):
+				return {} if text == '' else {pair.split('=')[0]: '='.join(pair.split('=')[1:]) for pair in text.split('&')}
+		
+		self.type = header.split('\r\n')[0].strip().split(' ')
+		self.header = {'method': self.type[0], 'link': ' '.join(self.type[1:-1]), 'ver': self.type[-1], 'data': {'user-agent': '', 'Accept': '', 'Accept-Encoding': '', 'Accept-Language': ''}}
+		header = self.parse_http_header(header)
+		self.files = self.parse_http_body(body)
+		self.header['data'].update(header)
+		self.ip, self.port = client_address[:2]
+		self.method = self.header['method']
+		self.version = self.header["ver"]
+		self.full_link = urllib.parse.unquote_plus(self.header["link"].replace('+', ' '))
+		self.host = self.header["data"]["Host"]
+		self.user_agent = self.header["data"]["User-Agent"] if 'User-Agent' in self.header['data'].keys() else self.header['data']['user-agent']
+		self.accept = self.header["data"]["Accept"].split(',')
+		self.encoding = self.header["data"]["Accept-Encoding"].split(',')
+		self.language = self.header["data"]["Accept-Language"].split(',')
+		self.link = self.full_link[:(self.full_link.index('?') if '?' in self.full_link else None)]
+		self.args = get_args(self.full_link[(self.full_link.index('?')+1 if '?' in self.full_link else len(self.full_link)):])
+		self.cookies = {c.split('=')[0]:c.split('=')[1] for c in self.header["data"]["Cookie"].split(';')} if 'Cookie' in self.header['data'] else []
+
+	def __str__(self):
+		return f'{self.GRAY}[{self.method}]{self.RESET} request {self.full_link} from {"" if "." in self.ip else "["}{self.ip}{"" if "." in self.ip else "]"}:{self.port} on {self.host}'
```

### Comparing `slinn-2.2.0/slinn/server.py` & `slinn-2.2.2/slinn/server.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,136 @@
-from slinn import Request, Address, utils
-import socket, ssl, threading, time, traceback, os
-
-
-class Server:
-	class Handle:
-		def __init__(self, filter, function):
-			self.filter = filter
-			self.function = function
-	
-	def __init__(self, *dispatchers, smart_navigation=True, ssl_fullchain: str=None, ssl_key: str=None, delay=0.05, timeout=0.03, max_bytes_per_recieve=4096, max_bytes=4294967296):
-		self.dispatchers = dispatchers
-		self.smart_navigation = smart_navigation
-		self.server_socket = None
-		self.ssl = ssl_fullchain is not None and ssl_key is not None
-		self.ssl_cert, self.ssl_key = ssl_fullchain, ssl_key
-		self.ssl_context = None
-		self.waiting = False
-		self.running = True
-		self.thread = None
-		self.delay = delay
-		self.timeout = timeout
-		self.max_bytes_per_recieve = max_bytes_per_recieve
-		self.max_bytes = max_bytes
-		self.__address = None
-
-	def reload(self, *dispatchers):
-		self.waiting = True
-		if self.thread is not None:
-			self.thread.stop()
-			try:
-				self.thread.join()
-			except RuntimeError:
-				pass
-		self.dispatchers = dispatchers
-		if self.running:
-			self.server_socket.close()
-			self.running = False
-		if self.__address is not None:
-			self.listen(self.__address)
-		self.waiting = False
-
-	def address(self):
-		return f'HTTP{"S" if self.ssl else ""} server is available on http{"s" if self.ssl else ""}://{"" if "." in self.host else "["}{self.host}{"" if "." in self.host else "]"}{(":"+str(self.port) if self.port != 443 else "") if self.ssl else (":"+str(self.port )if self.port != 80 else "")}/'
-		
-	def listen(self, address: Address):		
-		self.__address = address
-		self.host, self.port = address.host, address.port
-		if socket.has_dualstack_ipv6() and '.' not in self.host and ':' not in self.host:
-			self.server_socket = socket.create_server((self.host, self.port), family=socket.AF_INET6, dualstack_ipv6=True)
-		elif ':' in self.host:
-			self.server_socket = socket.create_server((self.host, self.port), family=socket.AF_INET6)
-		else:
-			self.server_socket = socket.create_server((self.host, self.port), family=(socket.AF_INET if '.' in self.host else socket.AF_INET6))
-		self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-		if self.ssl:
-			self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
-			self.ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
-		self.running = True
-		self.server_socket.listen()
-		print(self.address())
-		try:
-			while self.running:
-				if not self.waiting:
-					self.thread = utils.StoppableThread(target=self.handle_request)
-					self.thread.start()
-				time.sleep(self.delay)
-		except KeyboardInterrupt:
-			print('Got KeyboardInterrupt, halting the application...')
-			if self.running:
-				self.server_socket.close()
-				self.running = False
-			os._exit(0)
-						
-	def handle_request(self):
-		try:
-			if not self.running:
-				return
-			self.waiting = True
-			client_socket, client_address = self.server_socket.accept()
-			if self.ssl:
-				client_socket = self.ssl_context.wrap_socket(client_socket, server_side=True)
-			self.waiting = False
-			try:
-				client_socket.settimeout(self.timeout)
-				data = bytearray()
-				while len(data) < self.max_bytes:
-					try:
-						b = client_socket.recv(self.max_bytes_per_recieve)
-						data += b
-					except TimeoutError:
-						break
-					
-				data = data.split(b'\r\n\r\n')
-				header = data[0].decode()
-				content = b'\r\n\r\n'.join(data[1:])
-				
-				if header == '':
-					return
-
-				request = Request(header, content, client_address)
-				print(request)
-			except KeyError:
-				return print('Got KeyError, probably invalid request. Ignore')
-			except UnicodeDecodeError:
-				return print('Got UnocodeDecodeError, probably invalid request. Ignore')
-			except ConnectionResetError:
-				return print('Got ConnectionResetError. Ignore')
-			except OSError:
-				return print('Connection closed')
-			for dispatcher in self.dispatchers:
-				if True in [utils.restartswith(request.host, host) for host in dispatcher.hosts]:
-					if self.smart_navigation:
-						sizes = [handle.filter.size(request.link, request.method) for handle in dispatcher.handles]
-						if sizes != []:
-							handle = dispatcher.handles[sizes.index(max(sizes))]
-							if handle.filter.check(request.link, request.method):
-								client_socket.sendall(handle.function(request).make(request.version))
-								client_socket.close()
-								return
-					else:
-						for handle in dispatcher.handles:
-							if handle.filter.check(request.link, request.method):
-								client_socket.sendall(handle.function(request).make(request.version))
-								client_socket.close()
-								return
-		except ssl.SSLError:
-			print('During handling request, an exception has occured:')
-			traceback.print_exc()
-			self.waiting = False
-			print('Got ssl.SSLError, reloading...')
-			self.reload(self.dispatchers)
-		except Exception:
-			print('During handling request, an exception has occured:')
-			traceback.print_exc()
-			self.waiting = False
+from slinn import Request, Address, Filter, utils
+import socket, ssl, threading, time, traceback, os
+
+
+class Server:
+	class Handle:
+		def __init__(self, filter: Filter, function):
+			self.filter = filter
+			self.function = function
+	
+	def __init__(self, *dispatchers: tuple, smart_navigation: bool=True, ssl_fullchain: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296):
+		self.dispatchers = dispatchers
+		self.smart_navigation = smart_navigation
+		self.server_socket = None
+		self.ssl = ssl_fullchain is not None and ssl_key is not None
+		self.ssl_cert, self.ssl_key = ssl_fullchain, ssl_key
+		self.ssl_context = None
+		self.waiting = False
+		self.running = True
+		self.thread = None
+		self.delay = delay
+		self.timeout = timeout
+		self.max_bytes_per_recieve = max_bytes_per_recieve
+		self.max_bytes = max_bytes
+		self.__address = None
+
+	def reload(self, *dispatchers: tuple):
+		self.waiting = True
+		if self.thread is not None:
+			self.thread.stop()
+			try:
+				self.thread.join()
+			except RuntimeError:
+				pass
+		self.dispatchers = dispatchers
+		if self.running:
+			self.server_socket.close()
+			self.running = False
+		if self.__address is not None:
+			self.listen(self.__address)
+		self.waiting = False
+
+	def address(self):
+		return f'HTTP{"S" if self.ssl else ""} server is available on http{"s" if self.ssl else ""}://{"" if "." in self.host else "["}{self.host}{"" if "." in self.host else "]"}{(":"+str(self.port) if self.port != 443 else "") if self.ssl else (":"+str(self.port )if self.port != 80 else "")}/'
+		
+	def listen(self, address: Address):		
+		self.__address = address
+		self.host, self.port = address.host, address.port
+		if socket.has_dualstack_ipv6() and '.' not in self.host and ':' not in self.host:
+			self.server_socket = socket.create_server((self.host, self.port), family=socket.AF_INET6, dualstack_ipv6=True)
+		elif ':' in self.host:
+			self.server_socket = socket.create_server((self.host, self.port), family=socket.AF_INET6)
+		else:
+			self.server_socket = socket.create_server((self.host, self.port), family=(socket.AF_INET if '.' in self.host else socket.AF_INET6))
+		self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+		if self.ssl:
+			self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
+			self.ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
+		self.running = True
+		self.server_socket.listen()
+		print(self.address())
+		try:
+			while self.running:
+				if not self.waiting:
+					self.thread = utils.StoppableThread(target=self.handle_request)
+					self.thread.start()
+				time.sleep(self.delay)
+		except KeyboardInterrupt:
+			print('Got KeyboardInterrupt, halting the application...')
+			if self.running:
+				self.server_socket.close()
+				self.running = False
+			os._exit(0)
+						
+	def handle_request(self):
+		try:
+			if not self.running:
+				return
+			self.waiting = True
+			client_socket, client_address = self.server_socket.accept()
+			if self.ssl:
+				client_socket = self.ssl_context.wrap_socket(client_socket, server_side=True)
+			self.waiting = False
+			try:
+				client_socket.settimeout(self.timeout)
+				data = bytearray()
+				while len(data) < self.max_bytes:
+					try:
+						b = client_socket.recv(self.max_bytes_per_recieve)
+						data += b
+					except TimeoutError:
+						break
+					
+				data = data.split(b'\r\n\r\n')
+				header = data[0].decode()
+				content = b'\r\n\r\n'.join(data[1:])
+				
+				if header == '':
+					return
+
+				request = Request(header, content, client_address)
+				print(request)
+			except KeyError:
+				return print('Got KeyError, probably invalid request. Ignore')
+			except UnicodeDecodeError:
+				return print('Got UnocodeDecodeError, probably invalid request. Ignore')
+			except ConnectionResetError:
+				return print('Connection reset by client')
+			except OSError:
+				return print('Connection closed')
+			for dispatcher in self.dispatchers:
+				if True in [utils.restartswith(request.host, host) for host in dispatcher.hosts]:
+					if self.smart_navigation:
+						sizes = [handle.filter.size(request.link, request.method) for handle in dispatcher.handles]
+						if sizes != []:
+							handle = dispatcher.handles[sizes.index(max(sizes))]
+							if handle.filter.check(request.link, request.method):
+								client_socket.sendall(handle.function(request).make(request.version))
+								client_socket.close()
+								return
+					else:
+						for handle in dispatcher.handles:
+							if handle.filter.check(request.link, request.method):
+								client_socket.sendall(handle.function(request).make(request.version))
+								client_socket.close()
+								return
+		except ssl.SSLError:
+			print('During handling request, an exception has occured:')
+			traceback.print_exc()
+			self.waiting = False
+			print('Got ssl.SSLError, reloading...')
+			self.reload(self.dispatchers)
+		except Exception:
+			print('During handling request, an exception has occured:')
+			traceback.print_exc()
+			self.waiting = False
```

### Comparing `slinn-2.2.0/slinn/templates/firstrun/app.py` & `slinn-2.2.2/slinn/templates/firstrun/app.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from slinn import Dispatcher, Filter, HttpResponse
-import slinn
- 
-dp = Dispatcher()
-
-def read(filename):
-    file = open(filename, 'r', encoding='utf-8')
-    data = file.read()
-    file.close()
-    return data
-
-# Write your code down here  
-@dp(Filter('/styles.css'))
-def colorscss(request):
-    return HttpResponse(read('templates_data/firstrun/styles.css'))
-                       
-@dp(Filter('.*'))
-def index(request):
-    return HttpResponse(read('templates_data/firstrun/slinn.html').replace('{% version %}', slinn.version.split()[1]), content_type='text/html')
+from slinn import Dispatcher, Filter, HttpResponse
+import slinn
+ 
+dp = Dispatcher()
+
+def read(filename):
+    file = open(filename, 'r', encoding='utf-8')
+    data = file.read()
+    file.close()
+    return data
+
+# Write your code down here  
+@dp(Filter('/styles.css'))
+def colorscss(request):
+    return HttpResponse(read('templates_data/firstrun/styles.css'))
+                       
+@dp(Filter('.*'))
+def index(request):
+    return HttpResponse(read('templates_data/firstrun/slinn.html').replace('{% version %}', slinn.version.split()[1]), content_type='text/html')
```

### Comparing `slinn-2.2.0/slinn/templates/firstrun/data/slinn.html` & `slinn-2.2.2/slinn/templates/firstrun/data/slinn.html`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-<html>
-<head>
-	<meta charset="utf-8" name="viewport" content="width=device-width, initial-scale=1">
-	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
-	<script src="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.js?content_type=text/javascript"></script>
-	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.css?content_type=text/css">
-	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/colors_min.css?content_type=text/css">
-	<link rel="stylesheet" href="styles.css">
-
-	<title>Slinn</title>
-
-</head>
-<body>
-	<script>
-		header = new UiHeaderContainer('header', document.querySelector('body'))
-		new UiLabel('slinn', header.elem, 'Slinn — Miot Project')
-		new UiHorizontalFlexSpacer('spacer1', header.elem)
-		new UiLinkLabel('pypi', header.elem, 'Slinn on PyPI', 'https://pypi.org/project/slinn/', 'violet')
-		new UiLinkLabel('homepage', header.elem, 'Slinn`s homepage', 'https://slinn.miotp.ru/', 'violet')
-		new UiLinkLabel('homepage', header.elem, 'Miot Project', 'https://miotp.ru/', 'violet')
-		body = new UiCenterContainer('body', document.querySelector('body'))
-		new UiLabel('title', body.elem, 'Your Slinn server started successfully!')
-		new UiLabel('subtitle', body.elem, 'Congratulations! 🎉')
-		text = new UiText('text', body.elem, '')
-		new UiText('text1', text.elem, 'You are seeing this page because')
-		new UiMonoText('debugtruechip', text.elem, '{"debug": true}', 'violet')
-		new UiText('text2', text.elem, 'is in your')
-		new UiMonoText('projectjson', text.elem, 'project.json', 'violet')
-		new UiText('text3', text.elem, 'file')
-		footer = new UiCenterContainer('footer', document.querySelector('body'))
-
-		new UiText('footertext1', footer.elem, 'Your version: {% version %}')
-		fetch('https://slinn.miotp.ru/check')
-			.then(response => response.text())
-			.then((result) => {
-				console.log(result)
-				latest = result.split('\n')[0].split(': ')[1]
-				nightly = result.split('\n')[1].split(': ')[1]
-				new UiText('footertext2', footer.elem, 'Latest stable version: '+latest+', latest nightly version: '+nightly)
-			})
-	</script>
-</body>
+<html>
+<head>
+	<meta charset="utf-8" name="viewport" content="width=device-width, initial-scale=1">
+	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
+	<script src="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.js?content_type=text/javascript"></script>
+	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/miotuikit_min.css?content_type=text/css">
+	<link rel="stylesheet" href="https://uikit.miotp.ru/cdn/miotuikit/130124a/colors_min.css?content_type=text/css">
+	<link rel="stylesheet" href="styles.css">
+
+	<title>Slinn</title>
+
+</head>
+<body>
+	<script>
+		header = new UiHeaderContainer('header', document.querySelector('body'))
+		new UiLabel('slinn', header.elem, 'Slinn — Miot Project')
+		new UiHorizontalFlexSpacer('spacer1', header.elem)
+		new UiLinkLabel('pypi', header.elem, 'Slinn on PyPI', 'https://pypi.org/project/slinn/', 'violet')
+		new UiLinkLabel('homepage', header.elem, 'Slinn`s homepage', 'https://slinn.miotp.ru/', 'violet')
+		new UiLinkLabel('homepage', header.elem, 'Miot Project', 'https://miotp.ru/', 'violet')
+		body = new UiCenterContainer('body', document.querySelector('body'))
+		new UiLabel('title', body.elem, 'Your Slinn server started successfully!')
+		new UiLabel('subtitle', body.elem, 'Congratulations! 🎉')
+		text = new UiText('text', body.elem, '')
+		new UiText('text1', text.elem, 'You are seeing this page because')
+		new UiMonoText('debugtruechip', text.elem, '{"debug": true}', 'violet')
+		new UiText('text2', text.elem, 'is in your')
+		new UiMonoText('projectjson', text.elem, 'project.json', 'violet')
+		new UiText('text3', text.elem, 'file')
+		footer = new UiCenterContainer('footer', document.querySelector('body'))
+
+		new UiText('footertext1', footer.elem, 'Your version: {% version %}')
+		fetch('https://slinn.miotp.ru/check')
+			.then(response => response.text())
+			.then((result) => {
+				console.log(result)
+				latest = result.split('\n')[0].split(': ')[1]
+				nightly = result.split('\n')[1].split(': ')[1]
+				new UiText('footertext2', footer.elem, 'Latest stable version: '+latest+', latest nightly version: '+nightly)
+			})
+	</script>
+</body>
 </html>
```

### Comparing `slinn-2.2.0/slinn/templates/firstrun/data/styles.css` & `slinn-2.2.2/slinn/templates/firstrun/data/styles.css`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-*[name='btngen']{
-	display: block;
-}
-
-@media screen and (max-width: 700px) {
-  *[name='slinn'], *[name='pypi'], *[name='miotproject'], *[name='homepage']{
-    min-width: 200px;
-    display: block;
-    text-align: center;
-  }
-
-  *[name='header']{
-    display: block;
-  }
-}
-
-@media screen and (min-width: 500px){
-  *[name='header']{
-    min-width: 450px;
-  }
-}
-
-@media screen and (max-width: 500px){
-  *[name='header']{
-    max-width: 450px;
-  }
-}
-
-*[name='body']{
-  max-width: 450px;
-  display: block;
-}
-
-*[name='footer'] *{
-  display: block;
+*[name='btngen']{
+	display: block;
+}
+
+@media screen and (max-width: 700px) {
+  *[name='slinn'], *[name='pypi'], *[name='miotproject'], *[name='homepage']{
+    min-width: 200px;
+    display: block;
+    text-align: center;
+  }
+
+  *[name='header']{
+    display: block;
+  }
+}
+
+@media screen and (min-width: 500px){
+  *[name='header']{
+    min-width: 450px;
+  }
+}
+
+@media screen and (max-width: 500px){
+  *[name='header']{
+    max-width: 450px;
+  }
+}
+
+*[name='body']{
+  max-width: 450px;
+  display: block;
+}
+
+*[name='footer'] *{
+  display: block;
 }
```

### Comparing `slinn-2.2.0/slinn.egg-info/PKG-INFO` & `slinn-2.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,200 +1,204 @@
-Metadata-Version: 2.1
-Name: slinn
-Version: 2.2.0
-Summary: HTTPS and HTTP server framework
-Home-page: https://slinn.miotp.ru/
-Author: Mark Radin
-Author-email: mrybs2@gmail.com
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-
-# Slinn is a HTTPS and HTTP server framework
-
-### Create project
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash
-python3 -m slinn create helloworld
-cd helloworld
-venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
-venv/bin/python manage.py run 
-```
-
-##### Windows:
-```bat
-py -m slinn create helloworld
-cd helloworld
-venv\Scripts\activate
-py manage.py create localhost host=localhost host=127.0.0.1
-py manage.py run 
-```
-
-#### Simple example
-```python
-# localhost/app.py
-
-from slinn import Dispatcher, AnyFilter, LinkFilter, HttpResponse, HttpAPIResponse
-
-
-dp = Dispatcher('localhost', '127.0.0.1')
-
-
-@dp(LinkFilter('api'))
-def api(request):
-    return HttpAPIResponse('{"status": "ok"}')
-
-
-@dp(AnyFilter)
-def helloworld(request):
-     return HttpResponse('Hello world!')
-
-```
-
-Excepted output
-```
-$ venv/bin/python manage.py run
-Loading config...
-Apps: firstrun
-Debug mode enabled
-Smart navigation enabled
-
-Starting server...
-HTTP server is available on http://[::1]:8080/
-```
-
-To config project you should edit `./project.json`
-
-To config app you should edit `./%app%/config.json`
-
-### Create classic project
-##### Unix-like (Linux, MacOS, FreeBSD...):
-```bash 
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv/bin/activate
-```
-
-##### Windows:
-```bat
-mkdir helloworld 
-cd helloworld
-python3 -m venv venv
-venv\Scripts\activate
-```
-
-You should add this code to example `example.py`
-```
-Server(dp).listen(Address(8080))
-```
-then write `python example.py`
-
-#### Functions:
-```python
-from slinn import Server
-
-server = Server(*dispatchers: list[Dispatcher], ssl_cert: str=None, ssl_key: str=None, delay=0.05, timeout=0.03, max_bytes_per_recieve=4096, max_bytes=4294967296)  # Main class to run server
-server.address() -> str  # Returns info str
-server.reload(*dispatchers: list[Dispatcher])  # Reloads server
-server.listen(address: Address)  # Start listening address
-
-Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
-```
-
-```python
-from slinn import Address
-
-address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
-
-Address(443, 'google.com')
-```
-
-```python
-from slinn import Dispatcher
-
-dispatcher = Dispatcher(hosts: list=None)  # A class that contain many handlers
-
-Dispatcher('localhost', '127.0.0.1', '::1')
-
-# To add handler into dispatcher
-@dispatcher(filter: Filter)
-def handler(request: Request):
-    ...
-
-# handler should return HttpResponse-based object
-```
-
-```python
-from slinn import Filter, LinkFilter, AnyFilter
-
-_filter = Filter(filter: str, methods: list[str]=None)  # This class is used to choose match handler by link; uses regexp
-_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
-_filter.size(text: str, method: str) -> int  # Special method for Smart Navigation
-
-Filter('/user/.+/profile.*')
-
-# LinkFilter inherits from Filter
-LinkFilter('user/.+/profile')
-
-# AnyFilter as same as Filter('.*')
-```
-
-```python
-from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
-
-http_response = HttpResponse(payload, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
-http_response.set_cookie(key: str, value)
-http_response.make(type: str='HTTP/2.0') -> str
-
-HttpResponse('<h1>Hello world</h1>', content_type='text/html')
-
-# HttpAPIResponse inherits from HttpResponse
-# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
-
-HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
-
-# HttpRedirect inherits from HttpResponse
-HttpRedirect(location: str)
-
-HttpRedirect('slinn.miotp.ru')
-
-# HttpJSONResponse for responding JSON 
-HttpJSONResponse(**payload)
-
-HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
-
-# HttpJSONAPIResponse is like HttpJSONResponse, but it sets Access-Control-Allow-Origin to '*'
-
-HttpJSONAPIResponse(code=43657, until=1719931149)
-```
-
-```python
-from slinn import Request
-
-request = Request(http_data: str, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
-
-# Attributes
-request.ip, request.port  # Client`s IP and port
-request.method  # HTTP method
-request.version  # HTTP version
-request.full_link  # Full link(path and params)
-request.host  # Requested host
-request.user_agent  # Client`s user agent
-request.accept  # maybe supported technologies
-request.encoding  # Supported encodings
-request.language  # Client`s language
-request.link  # Link(only path)
-request.args  # GET args
-request.cookies  # All saved cookies
-request.files # Uploaded files
-```
-
-```python
-from slinn import File
-
-file = File(id: str=None, data: bytes|bytearray=bytearray())
-
-# Attributes
-file.id  # File`s id 
-file.data  # Binary data
-file.headers  # Headers such as Content-Disposition
-```
+Metadata-Version: 2.1
+Name: slinn
+Version: 2.2.2
+Summary: HTTPS and HTTP server framework
+Home-page: https://slinn.miotp.ru/
+Author: Mark Radin
+Author-email: mrybs2@gmail.com
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+
+# Slinn is a HTTPS and HTTP server framework
+
+### Create project
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash
+python3 -m slinn create helloworld
+cd helloworld
+venv/bin/python manage.py create localhost host=localhost host=127.0.0.1
+venv/bin/python manage.py run 
+```
+
+##### Windows:
+```bat
+py -m slinn create helloworld
+cd helloworld
+venv\Scripts\activate
+py manage.py create localhost host=localhost host=127.0.0.1
+py manage.py run 
+```
+
+#### Simple example
+```python
+# localhost/app.py
+
+from slinn import Dispatcher, AnyFilter, LinkFilter, HttpResponse, HttpAPIResponse
+
+
+dp = Dispatcher('localhost', '127.0.0.1')
+
+
+@dp(LinkFilter('api'))
+def api(request):
+    return HttpAPIResponse('{"status": "ok"}')
+
+
+@dp(AnyFilter)
+def helloworld(request):
+     return HttpResponse('Hello world!')
+
+```
+
+Excepted output
+```
+$ venv/bin/python manage.py run
+Loading config...
+Apps: firstrun
+Debug mode enabled
+Smart navigation enabled
+Delay: 50.0ms
+
+Starting server...
+HTTP server is available on http://[::1]:8080/
+```
+
+To config project you should edit `./project.json`
+
+To config app you should edit `./%app%/config.json`
+
+### Create classic project
+##### Unix-like (Linux, MacOS, FreeBSD...):
+```bash 
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv/bin/activate
+```
+
+##### Windows:
+```bat
+mkdir helloworld 
+cd helloworld
+python3 -m venv venv
+venv\Scripts\activate
+```
+
+You should add this code to example `example.py`
+```
+Server(dp).listen(Address(8080))
+```
+then write `python example.py`
+
+#### Functions:
+```python
+from slinn import Server
+
+server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run server
+server.address() -> str  # Returns info str
+server.reload(*dispatchers: tuple)  # Reloads server
+server.listen(address: Address)  # Start listening address
+
+Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
+```
+
+```python
+from slinn import Address
+
+address = Address(port: int, host: str=None)  # A structure containing a port and a host; converts dns-address to ip-address
+
+Address(443, 'google.com')
+```
+
+```python
+from slinn import Dispatcher
+
+dispatcher = Dispatcher(hosts: tuple=None)  # A class that contain many handlers
+
+Dispatcher('localhost', '127.0.0.1', '::1')
+
+# To add handler into dispatcher
+@dispatcher(filter: Filter)
+def handler(request: Request):
+    ...
+
+# handler should return HttpResponse-based object
+```
+
+```python
+from slinn import Filter, LinkFilter, AnyFilter
+
+_filter = Filter(filter: str, methods: tuple=None)  # This class is used to choose match handler by link; uses regexp
+_filter.check(text: str, method: str) -> bool  # Checks for a match by filter
+_filter.size(text: str, method: str) -> int  # Special method for Smart Navigation
+
+Filter('/user/.+/profile.*')
+
+# LinkFilter inherits from Filter
+LinkFilter('user/.+/profile')
+
+# AnyFilter as same as Filter('.*')
+```
+
+```python
+from slinn import HttpResponse, HttpRedirect, HttpAPIResponse, HttpJSONResponse, HttpJSONAPIResponse
+
+http_response = HttpResponse(payload: any, data: list[tuple]=None, status: str='200 OK', content_type: str='text/plain')  # This class is used to convert some data to HTTP code
+http_response.set_cookie(key: str, value: any)
+http_response.make(type: str='HTTP/2.0') -> str
+
+HttpResponse('<h1>Hello world</h1>', content_type='text/html')
+
+# HttpAPIResponse inherits from HttpResponse
+# HttpAPIResponse sets Access-Control-Allow-Origin to '*'
+
+HttpAPIResponse('{"status": "ok", "username": "mrybs"}')
+
+# HttpRedirect inherits from HttpResponse
+HttpRedirect(location: str)
+
+HttpRedirect('slinn.miotp.ru')
+
+# HttpJSONResponse for responding JSON 
+HttpJSONResponse(**payload: dict)
+
+HttpJSONResponse(status='this action is forbidden', _status='403 Forbidden')
+
+# HttpJSONAPIResponse is like HttpJSONResponse, but it sets Access-Control-Allow-Origin to '*'
+
+HttpJSONAPIResponse(code=43657, until=1719931149)
+```
+
+```python
+from slinn import Request
+
+request = Request(header: str, body: bytes, client_address: tuple[str, int])  # This structure is used in the dispatcher`s handler
+request.parse_http_header(http_header: str)  # Parse HTTP request`s header
+request.parse_http_body(http_body: body)  # Parse HTTP request`s body if exists
+str(request)  # Convert slinn.Request to info text
+
+# Attributes
+request.ip, request.port  # Client`s IP and port
+request.method  # HTTP method
+request.version  # HTTP version
+request.full_link  # Full link(path and params)
+request.host  # Requested host
+request.user_agent  # Client`s user agent
+request.accept  # maybe supported technologies
+request.encoding  # Supported encodings
+request.language  # Client`s language
+request.link  # Link(only path)
+request.args  # GET args
+request.cookies  # All saved cookies
+request.files # Uploaded files
+```
+
+```python
+from slinn import File
+
+file = File(id: str=None, data: bytes|bytearray=bytearray())
+
+# Attributes
+file.id  # File`s id 
+file.data  # Binary data
+file.headers  # Headers such as Content-Disposition
+```
```

### Comparing `slinn-2.2.0/slinn.egg-info/SOURCES.txt` & `slinn-2.2.2/slinn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 README.md
-setup.cfg
 setup.py
 slinn/__init__.py
 slinn/__main__.py
 slinn/address.py
 slinn/any_filter.py
 slinn/dispatcher.py
 slinn/file.py
```

