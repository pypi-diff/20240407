# Comparing `tmp/esrt-1.27.0.tar.gz` & `tmp/esrt-1.28.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esrt-1.27.0.tar", last modified: Wed Apr  3 06:03:21 2024, max compression
+gzip compressed data, was "esrt-1.28.0.tar", last modified: Sun Apr  7 14:25:47 2024, max compression
```

## Comparing `esrt-1.27.0.tar` & `esrt-1.28.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:03:21.874947 esrt-1.27.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-03 06:03:21.874947 esrt-1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10129 2024-04-03 06:02:58.000000 esrt-1.27.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-03 06:02:58.000000 esrt-1.27.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:03:21.874947 esrt-1.27.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:03:21.870947 esrt-1.27.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:03:21.874947 esrt-1.27.0/src/esrt/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 06:02:58.000000 esrt-1.27.0/src/esrt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11474 2024-04-03 06:02:58.000000 esrt-1.27.0/src/esrt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 06:02:58.000000 esrt-1.27.0/src/esrt/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 06:02:58.000000 esrt-1.27.0/src/esrt/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-03 06:02:58.000000 esrt-1.27.0/src/esrt/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-03 06:02:58.000000 esrt-1.27.0/src/esrt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:03:21.874947 esrt-1.27.0/src/esrt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10353 2024-04-03 06:03:21.000000 esrt-1.27.0/src/esrt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 06:03:21.000000 esrt-1.27.0/src/esrt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:03:21.000000 esrt-1.27.0/src/esrt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 06:03:21.000000 esrt-1.27.0/src/esrt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 06:03:21.000000 esrt-1.27.0/src/esrt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 06:03:21.000000 esrt-1.27.0/src/esrt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:25:47.855399 esrt-1.28.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-07 14:25:47.855399 esrt-1.28.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-07 14:25:31.000000 esrt-1.28.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-07 14:25:31.000000 esrt-1.28.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:25:47.855399 esrt-1.28.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:25:47.851399 esrt-1.28.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:25:47.851399 esrt-1.28.0/src/esrt/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-07 14:25:31.000000 esrt-1.28.0/src/esrt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11512 2024-04-07 14:25:31.000000 esrt-1.28.0/src/esrt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-07 14:25:31.000000 esrt-1.28.0/src/esrt/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 14:25:31.000000 esrt-1.28.0/src/esrt/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-07 14:25:31.000000 esrt-1.28.0/src/esrt/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-07 14:25:31.000000 esrt-1.28.0/src/esrt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:25:47.855399 esrt-1.28.0/src/esrt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-04-07 14:25:47.000000 esrt-1.28.0/src/esrt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 14:25:47.000000 esrt-1.28.0/src/esrt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:25:47.000000 esrt-1.28.0/src/esrt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 14:25:47.000000 esrt-1.28.0/src/esrt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 14:25:47.000000 esrt-1.28.0/src/esrt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 14:25:47.000000 esrt-1.28.0/src/esrt.egg-info/top_level.txt
```

### Comparing `esrt-1.27.0/PKG-INFO` & `esrt-1.28.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrt
-Version: 1.27.0
+Version: 1.28.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==6.8.2
 Requires-Dist: typer-slim[standard]>=0.12.0
 Requires-Dist: uvicorn>=0.2.14
 
 # esrt - Elasticsearch Request Tool
@@ -154,14 +154,15 @@
     for action in actions:
         obj = json.loads(action)
         prefix = 'new-'
         if not t.cast(str, obj['_index']).startswith(prefix):
             obj['_index'] = prefix + obj['_index']
         yield obj
 
+
 # class style
 class MyHandler(DocHandler):
     def handle(self, actions: t.Iterable[str]):
         for action in actions:
             yield self.handle_one(action)
 
     def handle_one(self, action: str):
```

### Comparing `esrt-1.27.0/README.md` & `esrt-1.28.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -145,14 +145,15 @@
     for action in actions:
         obj = json.loads(action)
         prefix = 'new-'
         if not t.cast(str, obj['_index']).startswith(prefix):
             obj['_index'] = prefix + obj['_index']
         yield obj
 
+
 # class style
 class MyHandler(DocHandler):
     def handle(self, actions: t.Iterable[str]):
         for action in actions:
             yield self.handle_one(action)
 
     def handle_one(self, action: str):
```

### Comparing `esrt-1.27.0/pyproject.toml` & `esrt-1.28.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "esrt"
-version = "1.27.0"
+version = "1.28.0"
 requires-python = ">=3.9"
 readme = "README.md"
 dependencies = [
     "elasticsearch==6.8.2",
     "typer-slim[standard]>=0.12.0",
     # uvicorn.importer.import_from_string
     "uvicorn>=0.2.14",
```

### Comparing `esrt-1.27.0/src/esrt/__main__.py` & `esrt-1.28.0/src/esrt/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from contextlib import nullcontext
 from contextlib import redirect_stdout
 import json
 from pathlib import Path
 import sys
 import time
 import typing as t
+from urllib.parse import quote
 
 from elasticsearch.helpers import scan
 from elasticsearch.helpers import streaming_bulk
 import typer
 from uvicorn.importer import import_from_string
 
 from . import es
@@ -197,15 +198,15 @@
     #
 ):
     client = es.Client(host=host)
     if not url.startswith('/'):
         url = '/' + url
     response = client.transport.perform_request(
         method=method,
-        url=url,
+        url=quote(url),
         headers=merge_dicts(headers),
         params=merge_dicts(params),
         body=finput_body and finput_body.read(),
     )
     foutput.write(json_obj_to_line(response))
```

### Comparing `esrt-1.27.0/src/esrt/handlers.py` & `esrt-1.28.0/src/esrt/handlers.py`

 * *Files identical despite different names*

### Comparing `esrt-1.27.0/src/esrt/utils.py` & `esrt-1.28.0/src/esrt/utils.py`

 * *Files identical despite different names*

### Comparing `esrt-1.27.0/src/esrt.egg-info/PKG-INFO` & `esrt-1.28.0/src/esrt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esrt
-Version: 1.27.0
+Version: 1.28.0
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: elasticsearch==6.8.2
 Requires-Dist: typer-slim[standard]>=0.12.0
 Requires-Dist: uvicorn>=0.2.14
 
 # esrt - Elasticsearch Request Tool
@@ -154,14 +154,15 @@
     for action in actions:
         obj = json.loads(action)
         prefix = 'new-'
         if not t.cast(str, obj['_index']).startswith(prefix):
             obj['_index'] = prefix + obj['_index']
         yield obj
 
+
 # class style
 class MyHandler(DocHandler):
     def handle(self, actions: t.Iterable[str]):
         for action in actions:
             yield self.handle_one(action)
 
     def handle_one(self, action: str):
```

