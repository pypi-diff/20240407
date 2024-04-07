# Comparing `tmp/ehdtd-0.1.4.tar.gz` & `tmp/ehdtd-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd-0.1.4.tar", max compression
+gzip compressed data, was "ehdtd-0.1.5.tar", max compression
```

## Comparing `ehdtd-0.1.4.tar` & `ehdtd-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.4/LICENSE
--rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.4/README.md
--rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.4/ehdtd/__init__.py
--rw-r--r--   0        0        0    21441 2024-04-07 03:50:53.982388 ehdtd-0.1.4/ehdtd/binance.py
--rw-r--r--   0        0        0   105876 2024-04-07 04:00:06.936458 ehdtd-0.1.4/ehdtd/ehdtd.py
--rw-r--r--   0        0        0     6540 2024-02-26 01:34:46.815409 ehdtd-0.1.4/ehdtd/ehdtd_common_functions.py
--rw-r--r--   0        0        0      683 2024-04-07 05:47:00.921192 ehdtd-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.5/README.md
+-rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.5/ehdtd/__init__.py
+-rw-r--r--   0        0        0    23627 2024-04-07 10:15:34.286547 ehdtd-0.1.5/ehdtd/binance.py
+-rw-r--r--   0        0        0   105876 2024-04-07 04:00:06.936458 ehdtd-0.1.5/ehdtd/ehdtd.py
+-rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.1.5/ehdtd/ehdtd_common_functions.py
+-rw-r--r--   0        0        0      683 2024-04-07 10:18:28.832548 ehdtd-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.5/PKG-INFO
```

### Comparing `ehdtd-0.1.4/LICENSE` & `ehdtd-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.4/README.md` & `ehdtd-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.4/ehdtd/__init__.py` & `ehdtd-0.1.5/ehdtd/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.4/ehdtd/binance.py` & `ehdtd-0.1.5/ehdtd/binance.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Author: Ricardo Marcelo Alvarez
 Date: 2023-10-31
 """
 
 import json
 import time
 import io
+import urllib.request
 import csv
 import random
 import hashlib
 import calendar
 
 import ehdtd.ehdtd_common_functions as ecf
 
@@ -337,32 +338,82 @@
                     result = {
                         'result': bool, # True if connectivity is working False in other case.
                         'code': int | None, # Error Code
                         'msg': str | None # Error message
                     }
         """
         result = None
+        headers = {}
+        timeout = 45
 
         __url_api = cls.get_api_url()
         __endpoint = '/ping'
         __url = f'{__url_api}{__endpoint}'
-        __data = ecf.file_get_contents_url(__url)
-        if ecf.is_json(__data):
-            __data = json.loads(__data)
-            if __data is not None and isinstance(__data, dict):
+
+        req = urllib.request.Request(__url, None, headers)
+        if req is not None:
+            try:
+                with urllib.request.urlopen(req, None, timeout=timeout) as response:
+                    result = {}
+                    result['result'] = None
+                    result['code'] = response.status
+                    result['data'] = response.read()
+                    result['headers'] = response.headers
+                    result['headers_str'] = response.headers.as_string()
+                    result['final_url'] = response.url
+                    result['res_code'] = None
+                    result['res_msg'] = None
+
+            except Exception as exc: # pylint: disable=broad-except
                 result = {}
-                result['result'] = True
+                result['result'] = None
                 result['code'] = None
-                result['msg'] = None
-
-                if 'code' in __data:
+                result['data'] = None
+                result['headers'] = None
+                result['headers_str'] = None
+                result['final_url'] = None
+                result['res_code'] = None
+                result['res_msg'] = None
+
+                if hasattr(exc, 'code'):
+                    result['code'] = response.status
+                if hasattr(exc, 'read'):
+                    result['data'] = exc.read().decode('utf-8')
+                if hasattr(exc, 'headers'):
+                    result['headers'] = exc.headers
+                    header_str = ''
+                    for header in exc.headers:
+                        header_str += f'{header}: {exc.headers[header]}'
+                    result['headers_str'] = header_str
+                if hasattr(exc, 'url'):
+                    result['final_url'] = exc.url
+
+            if result is not None\
+                and isinstance(result, dict)\
+                and 'data' in result:
+
+                if isinstance(result['data'], bytes):
+                    result['data'] = result['data'].decode()
+
+                if ecf.is_json(result['data']):
+                    result['data'] = json.loads(result['data'])
+
+                    if result['data'] is not None and isinstance(result['data'], dict):
+                        if 'code' in result['data']:
+                            result['res_code'] = result['data']['code']
+                        if 'msg' in result['data']:
+                            result['res_msg'] = result['data']['res_msg']
+
+                if result['code'] is not None\
+                    and isinstance(result['code'], int)\
+                    and 200 <= result['code'] < 300\
+                    and result['res_code'] is None:
+                    result['result'] = True
+                else:
                     result['result'] = False
-                    result['code'] = __data['code']
-                    if 'msg' in __data:
-                        result['msg'] = __data['msg']
 
         return result
 
     @classmethod
     def get_unified_symbol_from_symbol(cls, symbol):
         """
         get_unified_symbol_from_symbol
```

### Comparing `ehdtd-0.1.4/ehdtd/ehdtd.py` & `ehdtd-0.1.5/ehdtd/ehdtd.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.4/ehdtd/ehdtd_common_functions.py` & `ehdtd-0.1.5/ehdtd/ehdtd_common_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
             req = urllib.request.Request(url, None, headers)
 
         if req is not None:
             try:
                 with urllib.request.urlopen(req, None, timeout=timeout) as response:
                     result = response.read()
 
-
             except Exception: # pylint: disable=broad-except
                 result = None
 
         if mode != 'b' and result is not None and isinstance(result, bytes):
             result = result.decode()
 
     except Exception: # pylint: disable=broad-except
```

### Comparing `ehdtd-0.1.4/pyproject.toml` & `ehdtd-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd"
-version = "0.1.4"
+version = "0.1.5"
 description = "Ehdtd - cryptoCurrency Exchange history data to database"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/rmalvarezkai/ehdtd"
 
 [tool.poetry.dependencies]
```

### Comparing `ehdtd-0.1.4/PKG-INFO` & `ehdtd-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd
-Version: 0.1.4
+Version: 0.1.5
 Summary: Ehdtd - cryptoCurrency Exchange history data to database
 Home-page: https://github.com/rmalvarezkai/ehdtd
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

