# Comparing `tmp/cc-feishu-0.1.3.tar.gz` & `tmp/cc-feishu-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc-feishu-0.1.3.tar", last modified: Sat Jan 13 08:51:54 2024, max compression
+gzip compressed data, was "cc-feishu-0.1.4.tar", last modified: Sun Apr  7 03:21:05 2024, max compression
```

## Comparing `cc-feishu-0.1.3.tar` & `cc-feishu-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 08:51:54.066319 cc-feishu-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-13 08:51:54.066319 cc-feishu-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 08:51:54.062319 cc-feishu-0.1.3/cc_feishu/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/cc_feishu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/cc_feishu/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/cc_feishu/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/cc_feishu/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/cc_feishu/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/cc_feishu/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 08:51:54.066319 cc-feishu-0.1.3/cc_feishu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-13 08:51:54.000000 cc-feishu-0.1.3/cc_feishu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-13 08:51:54.000000 cc-feishu-0.1.3/cc_feishu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 08:51:54.000000 cc-feishu-0.1.3/cc_feishu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 08:51:54.000000 cc-feishu-0.1.3/cc_feishu.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-13 08:51:54.000000 cc-feishu-0.1.3/cc_feishu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-13 08:51:54.066319 cc-feishu-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 08:51:54.066319 cc-feishu-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-13 08:51:47.000000 cc-feishu-0.1.3/tests/test_login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:21:05.661531 cc-feishu-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-07 03:21:05.661531 cc-feishu-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:21:05.661531 cc-feishu-0.1.4/cc_feishu/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/cc_feishu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/cc_feishu/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/cc_feishu/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/cc_feishu/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/cc_feishu/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/cc_feishu/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:21:05.661531 cc-feishu-0.1.4/cc_feishu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-07 03:21:05.000000 cc-feishu-0.1.4/cc_feishu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-07 03:21:05.000000 cc-feishu-0.1.4/cc_feishu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:21:05.000000 cc-feishu-0.1.4/cc_feishu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:21:05.000000 cc-feishu-0.1.4/cc_feishu.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 03:21:05.000000 cc-feishu-0.1.4/cc_feishu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:21:05.661531 cc-feishu-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:21:05.661531 cc-feishu-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-07 03:20:55.000000 cc-feishu-0.1.4/tests/test_login.py
```

### Comparing `cc-feishu-0.1.3/LICENSE` & `cc-feishu-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cc-feishu-0.1.3/PKG-INFO` & `cc-feishu-0.1.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc-feishu
-Version: 0.1.3
+Version: 0.1.4
 Summary: my feishu package
 Home-page: https://github.com/houm01/cc-feishu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## 概览
```

### Comparing `cc-feishu-0.1.3/cc_feishu/client.py` & `cc-feishu-0.1.4/cc_feishu/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
-import os
 from typing import Optional, Union, Any, Dict, Type, List
 from dataclasses import dataclass
 from .endpoints import (
     AuthEndpoint,
     MessageEndpoint,
-    ExtensionsEndpoint
+    ExtensionsEndpoint,
+    BitableEndpoint
 )
 
 from .errors import (
     RequestTimeoutError,
     is_api_error_code,
     APIResponseError,
     HTTPResponseError
@@ -55,14 +55,15 @@
         self.options = ClientOptions()
 
         self._clients: List[Union[httpx.Client, httpx.AsyncClient]] = []
         self.client = client
 
         self.auth = AuthEndpoint(self)
         self.message = MessageEndpoint(self)
+        self.bitable = BitableEndpoint(self)
         self.extensions = ExtensionsEndpoint(self)
     
     @property
     def client(self) -> Union[httpx.Client, httpx.AsyncClient]:
         return self._clients[-1]
     
     @client.setter
@@ -78,21 +79,22 @@
 
 
     def _build_request(self,
                        method: str,
                        path: str,
                        query: Optional[Dict[Any, Any]] = None,
                        body: Optional[Dict[Any, Any]] = None,
+                       files: Optional[Dict[Any, Any]] = None,
                        token: Optional[str] = None) -> Request:
         
         headers = httpx.Headers()
         headers['Authorization'] = f'Bearer {token}'
 
         return self.client.build_request(
-            method=method, url=path, params=query, json=body, headers=headers
+            method=method, url=path, params=query, json=body, headers=headers, files=files
         )
 
     def _parse_response(self, response) -> Any:
         response = response.json()
         return FeishuResponse(code=response.get('code'),
                               data=response.get('data'),
                               chat_id=response.get('chat_id'),
@@ -150,25 +152,26 @@
             return self.auth.fetch_token_from_file()
 
     def request(self,
                 path: str,
                 method: str,
                 query: Optional[Dict[Any, Any]] = None,
                 body: Optional[Dict[Any, Any]] = None,
+                files: Optional[Dict[Any, Any]] = None,
                 token: Optional[str] = None,
                 ) -> Any:
 
-        request = self._build_request(method, path, query, body, token=self._get_token())
+        request = self._build_request(method, path, query, body, files=files, token=self._get_token())
         
         try:
             response = self._parse_response(self.client.send(request))
 
             if 'Invalid access token for authorization' in response.msg:
                 self.auth.save_token_to_file()
-                request = self._build_request(method, path, query, body, token=self._get_token())
+                request = self._build_request(method, path, query, body, files=files, token=self._get_token())
                 return self._parse_response(self.client.send(request))
             else:
                 return response
         except httpx.TimeoutException:
             raise RequestTimeoutError()
```

### Comparing `cc-feishu-0.1.3/cc_feishu/endpoints.py` & `cc-feishu-0.1.4/cc_feishu/endpoints.py`

 * *Files 16% similar despite different names*

```diff
@@ -159,26 +159,72 @@
         content = json.dumps(content, ensure_ascii=False)
         
         payload = {
            	"content": content,
             "msg_type": "interactive",
             "receive_id": receive_id
         }
-        
+
         return self.parent.request(path=f'/im/v1/messages?receive_id_type={receive_id_type}', 
                                    method='POST',
                                    body=payload)
 
+    def send_file(self, file_name, file_path, receive_id):
+        receive_id_type = self.parent.extensions.parse_receive_id_type(receive_id=receive_id)
+        content = {
+            "file_key": self.parent.extensions.upload_file(file_name=file_name, file_path=file_path)
+        }
+        content = json.dumps(content, ensure_ascii=False)
+        payload = {
+            "content": content,
+            "msg_type": "file",
+            "receive_id": receive_id
+        }
+
+        return self.parent.request(path=f'/im/v1/messages?receive_id_type={receive_id_type}', 
+                            method='POST',
+                            body=payload)
+
+class BitableEndpoint(Endpoint):
+    def list_records(self, app_token, table_id):
+        return self.parent.request(path=f'/bitable/v1/apps/{app_token}/tables/{table_id}/records',
+                                   method='GET')
+    
+    def add_record(self, app_token, table_id ,fields):
+        payload = {
+            "fields": fields
+        }
+        return self.parent.request(path=f'/bitable/v1/apps/{app_token}/tables/{table_id}/records',
+                                   method='POST',
+                                   body=payload)
+
+    def query_record(self, app_token, table_id, view_id, payload):
+
+        return self.parent.request(path=f'/bitable/v1/apps/{app_token}/tables/{table_id}/records/search',
+                                   method='POST',
+                                   body=payload)
+
+
 
 class ExtensionsEndpoint(Endpoint):
     def parse_receive_id_type(self, receive_id):
         if receive_id.startswith('ou'):
             receive_id_type = 'open_id'
         elif receive_id.startswith('oc'):
             receive_id_type = 'chat_id'
         else:
             raise 'No such named receive_id'
 
         return receive_id_type
 
+    def upload_file(self, file_name, file_path):
 
+        files = {
+            'file_type': ('', 'stream'),
+            'file_name': ('', file_name),
+            'file': open(file_path, 'rb')
+        }
+
+        return self.parent.request(path=f'/im/v1/files',
+                                   method='POST',
+                                   files=files).data['file_key']
```

### Comparing `cc-feishu-0.1.3/cc_feishu/errors.py` & `cc-feishu-0.1.4/cc_feishu/errors.py`

 * *Files identical despite different names*

### Comparing `cc-feishu-0.1.3/cc_feishu.egg-info/PKG-INFO` & `cc-feishu-0.1.4/cc_feishu.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cc-feishu
-Version: 0.1.3
+Version: 0.1.4
 Summary: my feishu package
 Home-page: https://github.com/houm01/cc-feishu
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## 概览
```

### Comparing `cc-feishu-0.1.3/setup.py` & `cc-feishu-0.1.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding: utf-8
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
-VERSION = '0.1.3'
+VERSION = '0.1.4'
 
 setup(
     name='cc-feishu',  # package name
     version=VERSION,  # package version
     description='my feishu package',  # package description
     packages=find_packages(),
     url="https://github.com/houm01/cc-feishu",
```

