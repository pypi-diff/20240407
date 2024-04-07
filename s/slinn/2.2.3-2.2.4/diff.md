# Comparing `tmp/slinn-2.2.3.tar.gz` & `tmp/slinn-2.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slinn-2.2.3.tar", last modified: Sun Apr  7 15:42:07 2024, max compression
+gzip compressed data, was "slinn-2.2.4.tar", last modified: Sun Apr  7 20:31:51 2024, max compression
```

## Comparing `slinn-2.2.3.tar` & `slinn-2.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5365 2024-04-07 15:42:07.357757 slinn-2.2.3/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5123 2024-04-07 15:24:37.000000 slinn-2.2.3/README.md
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-07 15:42:07.357757 slinn-2.2.3/setup.cfg
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      763 2024-04-07 15:32:00.000000 slinn-2.2.3/setup.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-04-07 14:40:45.000000 slinn-2.2.3/slinn/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/__main__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      328 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/address.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/any_filter.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/default/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/default/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12930 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/default/manage.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      279 2024-03-28 20:39:01.000000 slinn-2.2.3/slinn/default/project.json
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      297 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/dispatcher.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.3/slinn/file.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/filter.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/guides/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/guides/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      580 2024-04-07 11:25:26.000000 slinn-2.2.3/slinn/guides/migration1xx2xx.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/http_api_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/http_json_api_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/http_json_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/http_redirect.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-04-07 14:32:49.000000 slinn-2.2.3/slinn/http_response.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-04-07 11:26:11.000000 slinn-2.2.3/slinn/link_filter.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-04-07 14:32:49.000000 slinn-2.2.3/slinn/request.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5178 2024-04-07 15:05:28.000000 slinn-2.2.3/slinn/server.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/__init__.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/example/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/example/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/example/app.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/example/config.json
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/firstrun/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/__init__.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      567 2024-03-28 20:39:01.000000 slinn-2.2.3/slinn/templates/firstrun/app.py
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/config.json
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn/templates/firstrun/data/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/data/slinn.html
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.3/slinn/templates/firstrun/data/styles.css
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1191 2024-04-07 15:10:25.000000 slinn-2.2.3/slinn/utils.py
-drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 15:42:07.357757 slinn-2.2.3/slinn.egg-info/
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5365 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/PKG-INFO
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)      936 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/SOURCES.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/dependency_links.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-07 15:42:07.000000 slinn-2.2.3/slinn.egg-info/top_level.txt
--rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.3/slinn.egg-info/zip-safe
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.831788 slinn-2.2.4/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5430 2024-04-07 20:31:51.831788 slinn-2.2.4/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5188 2024-04-07 20:28:24.000000 slinn-2.2.4/README.md
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       38 2024-04-07 20:31:51.831788 slinn-2.2.4/setup.cfg
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      763 2024-04-07 17:15:37.000000 slinn-2.2.4/setup.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.828454 slinn-2.2.4/slinn/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      579 2024-04-07 17:15:09.000000 slinn-2.2.4/slinn/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4383 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/__main__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      328 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/address.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       58 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/any_filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.828454 slinn-2.2.4/slinn/default/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       35 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/default/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)    12973 2024-04-07 20:29:08.000000 slinn-2.2.4/slinn/default/manage.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      261 2024-04-07 20:24:45.000000 slinn-2.2.4/slinn/default/project.json
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      297 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/dispatcher.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      156 2024-03-28 20:39:01.000000 slinn-2.2.4/slinn/file.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      667 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/filter.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.828454 slinn-2.2.4/slinn/guides/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       56 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/guides/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      586 2024-04-07 20:25:23.000000 slinn-2.2.4/slinn/guides/migration1xx2xx.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      612 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/http_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      363 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/http_json_api_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      466 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/http_json_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      183 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/http_redirect.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      752 2024-04-07 14:32:49.000000 slinn-2.2.4/slinn/http_response.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      251 2024-04-07 11:26:11.000000 slinn-2.2.4/slinn/link_filter.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     3096 2024-04-07 14:32:49.000000 slinn-2.2.4/slinn/request.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     4581 2024-04-07 20:20:15.000000 slinn-2.2.4/slinn/server.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.828454 slinn-2.2.4/slinn/templates/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       23 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/__init__.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.828454 slinn-2.2.4/slinn/templates/example/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      159 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/example/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      277 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/example/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       22 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/example/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.831788 slinn-2.2.4/slinn/templates/firstrun/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      162 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/firstrun/__init__.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      567 2024-04-07 20:28:05.000000 slinn-2.2.4/slinn/templates/firstrun/app.py
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)       21 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/firstrun/config.json
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.831788 slinn-2.2.4/slinn/templates/firstrun/data/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     2199 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/firstrun/data/slinn.html
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      543 2024-03-28 20:36:39.000000 slinn-2.2.4/slinn/templates/firstrun/data/styles.css
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     1191 2024-04-07 15:10:25.000000 slinn-2.2.4/slinn/utils.py
+drwxr-xr-x   0 mrybs     (1000) mrybs     (1000)        0 2024-04-07 20:31:51.831788 slinn-2.2.4/slinn.egg-info/
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)     5430 2024-04-07 20:31:51.000000 slinn-2.2.4/slinn.egg-info/PKG-INFO
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)      936 2024-04-07 20:31:51.000000 slinn-2.2.4/slinn.egg-info/SOURCES.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 20:31:51.000000 slinn-2.2.4/slinn.egg-info/dependency_links.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        6 2024-04-07 20:31:51.000000 slinn-2.2.4/slinn.egg-info/top_level.txt
+-rw-r--r--   0 mrybs     (1000) mrybs     (1000)        1 2024-04-07 11:02:22.000000 slinn-2.2.4/slinn.egg-info/zip-safe
```

### Comparing `slinn-2.2.3/PKG-INFO` & `slinn-2.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slinn
-Version: 2.2.3
+Version: 2.2.4
 Summary: A HTTPS and HTTP server framework
 Home-page: https://slinn.miotp.ru/
 Author: Mark Radin
 Author-email: mrybs2@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
@@ -57,15 +57,14 @@
 Excepted output
 ```
 $ venv/bin/python manage.py run
 Loading config...
 Apps: firstrun
 Debug mode enabled
 Smart navigation enabled
-Delay: 50.0ms
 
 Starting server...
 HTTP server is available on http://[::1]:8080/
 ```
 
 To config project you should edit `./project.json`
 
@@ -95,15 +94,15 @@
 then write `python example.py`
 
 #### Functions:
 ```python
 from slinn import Server
 
 server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
-server.address() -> str  # Returns info str
+server.address(port: int, host: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
 server.reload(*dispatchers: tuple)  # Reloads server
 server.listen(address: Address)  # Start listening address
 
 Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
 ```
 
 ```python
```

### Comparing `slinn-2.2.3/README.md` & `slinn-2.2.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 Excepted output
 ```
 $ venv/bin/python manage.py run
 Loading config...
 Apps: firstrun
 Debug mode enabled
 Smart navigation enabled
-Delay: 50.0ms
 
 Starting server...
 HTTP server is available on http://[::1]:8080/
 ```
 
 To config project you should edit `./project.json`
 
@@ -85,15 +84,15 @@
 then write `python example.py`
 
 #### Functions:
 ```python
 from slinn import Server
 
 server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
-server.address() -> str  # Returns info str
+server.address(port: int, host: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
 server.reload(*dispatchers: tuple)  # Reloads server
 server.listen(address: Address)  # Start listening address
 
 Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
 ```
 
 ```python
```

### Comparing `slinn-2.2.3/setup.py` & `slinn-2.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open('README.md', 'r') as f:
         return f.read()
     
 templates = ['firstrun', 'example']
 
 
 setup(name='slinn',
-      version='2.2.3',
+      version='2.2.4',
       description='A HTTPS and HTTP server framework',
       packages=['slinn', 'slinn.templates', 'slinn.guides'] + ['slinn.templates.' + template for template in templates],
       package_data={'slinn': ['default/*.*']} | {'slinn.templates.' + template: ['data/*.css', 'data/*.html', 'config.json'] for template in templates},
       author='Mark Radin',
       author_email='mrybs2@gmail.com',
       url='https://slinn.miotp.ru/',
       long_description=readme(),
```

### Comparing `slinn-2.2.3/slinn/__init__.py` & `slinn-2.2.4/slinn/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 from slinn.http_api_response import HttpAPIResponse
 from slinn.http_json_response import HttpJSONResponse
 from slinn.http_json_api_response import HttpJSONAPIResponse
 from slinn.server import Server
 from slinn.dispatcher import Dispatcher
 
 
-version = 'Slinn Murega v2.2.3 070424C'
+version = 'Slinn Murega v2.2.4 070424D'
```

### Comparing `slinn-2.2.3/slinn/__main__.py` & `slinn-2.2.4/slinn/__main__.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn/default/manage.py` & `slinn-2.2.4/slinn/default/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,14 @@
 			
 			print('Loading config...')
 			cfg = config()
 			debug = cfg["debug"] if "debug" in cfg.keys() else False
 			apps = cfg['apps'] if 'apps' in cfg.keys() else []
 			port = cfg['port'] if 'port' in cfg.keys() else 8080
 			host = cfg['host'] if 'host' in cfg.keys() else ''
-			delay = float(cfg['delay']) if 'delay' in cfg.keys() else 0.05
 			timeout = float(cfg['timeout']) if 'timeout' in cfg.keys() else 0.03
 			max_bytes_per_recieve = int(cfg['max_bytes_per_recieve']) if 'max_bytes_per_recieve' in cfg.keys() else 4096
 			max_bytes = int(cfg['max_bytes']) if 'max_bytes' in cfg.keys() else 4294967296
 			smart_navigation = cfg['smart_navigation'] if 'smart_navigation' in cfg.keys() else True
 			ssl_fullchain, ssl_key = None, None
 			if 'ssl' in cfg.keys() and 'fullchain' in cfg['ssl'].keys() and 'key' in cfg['ssl'].keys():
 				ssl_fullchain = '"'+cfg['ssl']['fullchain']+'"' if cfg['ssl']['fullchain'] else None    
@@ -179,47 +178,50 @@
 							checksums.append(path+md5(dir+'/'+path))
 					return checksums
 				return hashlib.md5(''.join([checksum for checksum in get_dir_checksums(dir)]).encode()).hexdigest()
 			global checksum
 			checksum = get_dir_checksum('.')
 			reloader = """
 def reloader(server, delay=0.3):
-	import time, importlib
+	import time, importlib, traceback
 	def runtime(delay, server):
 		global checksum
 		while True:
-			if checksum != get_dir_checksum('.'):
-				checksum = get_dir_checksum('.')
-				"""
+			try:
+				if checksum != get_dir_checksum('.'):
+					checksum = get_dir_checksum('.')
+					"""
 			for app in cfg['apps']:
 				if not app_config(app)['debug'] or debug:
 					reloader += app_reload(app)
 			reloader += """
-				print('\\n\\nServer updated')
-				print(server.address())
-				server.reload("""
+					print('\\n\\nServer updated')
+					print(server.address("""+f'{port}, "{host}"'+"""))
+					server.reload("""
 			reloader += ",".join(dps)
 			reloader += """)
-			time.sleep(delay)
+				time.sleep(delay)
+			except Exception:
+				print('During handling request, an exception has occured:')
+				traceback.print_exc()
 	import threading;threading.Thread(target=runtime, args=(delay, server)).start()
 """
 			apps_info = []
 			for app in cfg['apps']:
 				if not app_config(app)['debug'] or debug:
 					apps_info.append(app)
 				else:
 					apps_info.append('['+app+']')
 			print(f'{GRAY}Apps: ' + ', '.join(apps_info))
 			print('Debug mode ' + 'enabled' if debug else 'disabled')
 			print('Smart navigation ' + ('enabled' if smart_navigation else 'disabled'))
-			print(f'Delay: {str(delay*1000)}ms')
 			print(RESET)
 
 			print('Starting server...')
-			start = ';'.join(load_imports(apps, debug))+reloader+f'server=Server({",".join(dps)}, smart_navigation={smart_navigation}, ssl_fullchain={ssl_fullchain}, ssl_key={ssl_key}, delay={delay}, timeout={timeout}, max_bytes_per_recieve={max_bytes_per_recieve}, max_bytes={max_bytes});reloader(server=server);server.listen(Address({port}, "{host}"))'
+			start = ';'.join(load_imports(apps, debug))+reloader+f'server=Server({",".join(dps)}, smart_navigation={smart_navigation}, ssl_fullchain={ssl_fullchain}, ssl_key={ssl_key}, timeout={timeout}, max_bytes_per_recieve={max_bytes_per_recieve}, max_bytes={max_bytes});reloader(server=server);server.listen(Address({port}, "{host}"))'
 			exec(start)
 		elif sys.argv[1].lower() == 'create':
 			args = get_args(['name', 'host'], ' '.join(sys.argv[2:]))
 			if 'name' not in args.keys():
 				return print(f'{RED}The app`s name is not specified{RESET}')
 			ensure_appname = replace_all(args['name'], '-&$#!@%^().,', '_')
 			if os.path.isdir(ensure_appname):
```

### Comparing `slinn-2.2.3/slinn/filter.py` & `slinn-2.2.4/slinn/filter.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn/guides/migration1xx2xx.py` & `slinn-2.2.4/slinn/guides/migration1xx2xx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0)
+migration1xx2xx = """How to migrate from 1xx(1.2.1) to 2xx(2.0.0-2.2.4)
 
 Firstly, change all your @dp_xxx.route(...) to @dp_xxx(...)
 Then, you should change some filters from Filter to AnyFilter or LinkFilter where it is suit
 If you have troubles with Smart Navigation, then specify '{"smart_navigation": false}' in your project.json
 
 If you want support of autoreloading your app, follow these steps:
 - Change dp_xxx = Dispatcher(...) to dp = Dispatcher(...) and @dp_xxx.route(...) to @dp(...) OR dp = dp_xxx in the end of the file
```

### Comparing `slinn-2.2.3/slinn/http_api_response.py` & `slinn-2.2.4/slinn/http_api_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn/http_response.py` & `slinn-2.2.4/slinn/http_response.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn/request.py` & `slinn-2.2.4/slinn/request.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn/server.py` & `slinn-2.2.4/slinn/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,81 +4,68 @@
 
 class Server:
 	class Handle:
 		def __init__(self, filter: Filter, function):
 			self.filter = filter
 			self.function = function
 	
-	def __init__(self, *dispatchers: tuple, smart_navigation: bool=True, ssl_fullchain: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296):
+	def __init__(self, *dispatchers: tuple, smart_navigation: bool=True, ssl_fullchain: str=None, ssl_key: str=None, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296):
 		self.dispatchers = dispatchers
 		self.smart_navigation = smart_navigation
 		self.server_socket = None
 		self.ssl = ssl_fullchain is not None and ssl_key is not None
 		self.ssl_cert, self.ssl_key = ssl_fullchain, ssl_key
 		self.ssl_context = None
-		self.waiting = False
 		self.thread = None
-		self.delay = delay
 		self.timeout = timeout
 		self.max_bytes_per_recieve = max_bytes_per_recieve
 		self.max_bytes = max_bytes
 		self.__address = None
 
 	def reload(self, *dispatchers: tuple):
-		self.waiting = True
 		if self.thread is not None:
 			self.thread.stop()
 			try:
 				self.thread.join()
 			except RuntimeError:
 				pass
 		self.dispatchers = dispatchers
-		if utils.check_socket(self.server_socket):
-			self.server_socket.close()
-		if self.__address is not None:
-			self.listen(self.__address)
+			
 
-	def address(self):
-		return f'HTTP{"S" if self.ssl else ""} server is available on http{"s" if self.ssl else ""}://{"" if "." in self.host else "["}{self.host}{"" if "." in self.host else "]"}{(":"+str(self.port) if self.port != 443 else "") if self.ssl else (":"+str(self.port )if self.port != 80 else "")}/'
+	def address(self, port: int, host: str):
+		return f'HTTP{"S" if self.ssl else ""} server is available on http{"s" if self.ssl else ""}://{"" if "." in host else "["}{host}{"" if "." in host else "]"}{(":"+str(port) if port != 443 else "") if self.ssl else (":"+str(port )if port != 80 else "")}/'
 		
 	def listen(self, address: Address):		
-		self.__address = address
-		self.host, self.port = address.host, address.port
-		if socket.has_dualstack_ipv6() and '.' not in self.host and ':' not in self.host:
-			self.server_socket = socket.create_server((self.host, self.port), family=socket.AF_INET6, dualstack_ipv6=True)
-		elif ':' in self.host:
-			self.server_socket = socket.create_server((self.host, self.port), family=socket.AF_INET6)
+		self.server_socket = None
+		if socket.has_dualstack_ipv6() and '.' not in address.host and ':' not in address.host:
+			self.server_socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM, dualstack_ipv6=True)
+		elif ':' in address.host:
+			self.server_socket = socket.socket(socket.AF_INET6, socket.SOCK_STREAM)
 		else:
-			self.server_socket = socket.create_server((self.host, self.port), family=(socket.AF_INET if '.' in self.host else socket.AF_INET6))
+			self.server_socket = socket.socket(socket.AF_INET if '.' in self.host else socket.AF_INET6, socket.SOCK_STREAM)
 		self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+		self.server_socket.bind((address.host, address.port))
 		if self.ssl:
 			self.ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
 			self.ssl_context.load_cert_chain(certfile=self.ssl_cert, keyfile=self.ssl_key)
 		self.server_socket.listen()
-		print(self.address())
-		self.waiting = False
+		print(self.address(address.port, address.host))
 		try:
-			while utils.check_socket(self.server_socket):
-				if not self.waiting:
-					self.thread = utils.StoppableThread(target=self.handle_request)
-					self.thread.start()
-				time.sleep(self.delay)
+			while True:
+				utils.StoppableThread(target=self.handle_request, args=self.server_socket.accept()).start()
 		except KeyboardInterrupt:
 			print('Got KeyboardInterrupt, halting the application...')
 			if utils.check_socket(self.server_socket):
 				self.server_socket.close()
 			os._exit(0)
 						
-	def handle_request(self):
+	def handle_request(self, client_socket, client_address):
 		try:
-			self.waiting = True
-			client_socket, client_address = self.server_socket.accept()
 			if self.ssl:
 				client_socket = self.ssl_context.wrap_socket(client_socket, server_side=True)
-			self.waiting = False
 			try:
 				client_socket.settimeout(self.timeout)
 				data = bytearray()
 				while len(data) < self.max_bytes:
 					try:
 						b = client_socket.recv(self.max_bytes_per_recieve)
 						data += b
@@ -91,20 +78,16 @@
 				
 				if header == '':
 					return
 
 				request = Request(header, content, client_address)
 				print(request)
 			except KeyError:
-				if utils.check_socket(client_socket):
-					client_socket.close()
 				return print('Got KeyError, probably invalid request. Ignore')
 			except UnicodeDecodeError:
-				if utils.check_socket(client_socket):
-					client_socket.close()
 				return print('Got UnocodeDecodeError, probably invalid request. Ignore')
 			except ConnectionResetError:
 				return print('Connection reset by client')
 			except OSError:
 				return print('Connection closed')
 			for dispatcher in self.dispatchers:
 				if True in [utils.restartswith(request.host, host) for host in dispatcher.hosts]:
@@ -128,8 +111,7 @@
 			print('During handling request, an exception has occured:')
 			traceback.print_exc()
 			print('Got ssl.SSLError, reloading...')
 			self.reload(*self.dispatchers)
 		except Exception:
 			print('During handling request, an exception has occured:')
 			traceback.print_exc()
-			self.waiting = False
```

### Comparing `slinn-2.2.3/slinn/templates/firstrun/app.py` & `slinn-2.2.4/slinn/templates/firstrun/app.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # Write your code down here  
 @dp(Filter('/styles.css'))
 def colorscss(request):
     return HttpResponse(read('templates_data/firstrun/styles.css'))
                        
 @dp(Filter('.*'))
 def index(request):
-    return HttpResponse(read('templates_data/firstrun/slinn.html').replace('{% version %}', slinn.version.split()[1]), content_type='text/html')
+    return HttpResponse(read('templates_data/firstrun/slinn.html').replace('{% version %}', slinn.version.split()[2]), content_type='text/html')
```

### Comparing `slinn-2.2.3/slinn/templates/firstrun/data/slinn.html` & `slinn-2.2.4/slinn/templates/firstrun/data/slinn.html`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn/templates/firstrun/data/styles.css` & `slinn-2.2.4/slinn/templates/firstrun/data/styles.css`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn/utils.py` & `slinn-2.2.4/slinn/utils.py`

 * *Files identical despite different names*

### Comparing `slinn-2.2.3/slinn.egg-info/PKG-INFO` & `slinn-2.2.4/slinn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slinn
-Version: 2.2.3
+Version: 2.2.4
 Summary: A HTTPS and HTTP server framework
 Home-page: https://slinn.miotp.ru/
 Author: Mark Radin
 Author-email: mrybs2@gmail.com
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
@@ -57,15 +57,14 @@
 Excepted output
 ```
 $ venv/bin/python manage.py run
 Loading config...
 Apps: firstrun
 Debug mode enabled
 Smart navigation enabled
-Delay: 50.0ms
 
 Starting server...
 HTTP server is available on http://[::1]:8080/
 ```
 
 To config project you should edit `./project.json`
 
@@ -95,15 +94,15 @@
 then write `python example.py`
 
 #### Functions:
 ```python
 from slinn import Server
 
 server = Server(*dispatchers: tuple, ssl_cert: str=None, ssl_key: str=None, delay: float=0.05, timeout: float=0.03, max_bytes_per_recieve: int=4096, max_bytes: int=4294967296)  # Main class to run a server
-server.address() -> str  # Returns info str
+server.address(port: int, host: str) -> str  # Returns message like 'HTTPS server is available on https://localhost:8080/'
 server.reload(*dispatchers: tuple)  # Reloads server
 server.listen(address: Address)  # Start listening address
 
 Server(dp_api, dp_gui, ssl_cert='fullchain.pem', ssl_key='privkey.pem')
 ```
 
 ```python
```

### Comparing `slinn-2.2.3/slinn.egg-info/SOURCES.txt` & `slinn-2.2.4/slinn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

