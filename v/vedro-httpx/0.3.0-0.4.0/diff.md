# Comparing `tmp/vedro-httpx-0.3.0.tar.gz` & `tmp/vedro-httpx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vedro-httpx-0.3.0.tar", last modified: Fri Jul 28 16:46:53 2023, max compression
+gzip compressed data, was "vedro-httpx-0.4.0.tar", last modified: Sun Apr  7 14:34:57 2024, max compression
```

## Comparing `vedro-httpx-0.3.0.tar` & `vedro-httpx-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.755904 vedro-httpx-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_async_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_format_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_print_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/tests/test_sync_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.755904 vedro-httpx-0.3.0/vedro_httpx/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_async_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_render_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_sync_http_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/_vedro_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:42.000000 vedro-httpx-0.3.0/vedro_httpx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 16:46:53.759904 vedro-httpx-0.3.0/vedro_httpx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-28 16:46:53.000000 vedro-httpx-0.3.0/vedro_httpx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.985721 vedro-httpx-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_async_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3679 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_format_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_print_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/tests/test_sync_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.985721 vedro-httpx-0.4.0/vedro_httpx/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_async_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_render_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_sync_http_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_vedro_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/vedro_httpx/recorder/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_async_har_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_base_har_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_har_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_request_recorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/_sync_har_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/vedro_httpx/recorder/har/
+-rw-r--r--   0 runner    (1001) docker     (127)    10536 2024-04-07 14:34:50.000000 vedro-httpx-0.4.0/vedro_httpx/recorder/har/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:34:57.989721 vedro-httpx-0.4.0/vedro_httpx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 14:34:57.000000 vedro-httpx-0.4.0/vedro_httpx.egg-info/top_level.txt
```

### Comparing `vedro-httpx-0.3.0/LICENSE` & `vedro-httpx-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.3.0/PKG-INFO` & `vedro-httpx-0.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.3.0
+Version: 0.4.0
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx<1.0,>=0.23
+Requires-Dist: vedro<2.0,>=1.7
 
 # vedro-httpx
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-httpx/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-httpx)
 [![PyPI](https://img.shields.io/pypi/v/vedro-httpx.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-httpx?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-httpx.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
@@ -74,28 +77,28 @@
 ## Usage
 
 ### AsyncHTTPInterface
 
 ```python
 from vedro_httpx import Response, AsyncHTTPInterface
 
-class Api(AsyncHTTPInterface):
+class AuthAPI(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
 
 ### SyncHTTPInterface
 
 ```python
 from vedro_httpx import Response, AsyncHTTPInterface
 
-class Api(AsyncHTTPInterface):
+class AuthAPI(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
```

### Comparing `vedro-httpx-0.3.0/README.md` & `vedro-httpx-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -54,28 +54,28 @@
 ## Usage
 
 ### AsyncHTTPInterface
 
 ```python
 from vedro_httpx import Response, AsyncHTTPInterface
 
-class Api(AsyncHTTPInterface):
+class AuthAPI(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
 
 ### SyncHTTPInterface
 
 ```python
 from vedro_httpx import Response, AsyncHTTPInterface
 
-class Api(AsyncHTTPInterface):
+class AuthAPI(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
```

### Comparing `vedro-httpx-0.3.0/setup.cfg` & `vedro-httpx-0.4.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [bumpversion]
-current_version = 0.3.0
+current_version = 0.4.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
 
-[bumpversion:file:vedro_httpx/__init__.py]
+[bumpversion:file:vedro_httpx/_version.py]
 
 [aliases]
 test = pytest
 
 [flake8]
 exclude = __pycache__
 max_line_length = 99
```

### Comparing `vedro-httpx-0.3.0/setup.py` & `vedro-httpx-0.4.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="vedro-httpx",
-    version="0.3.0",
+    version="0.4.0",
     description="Vedro + HTTPX",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
     author_email="tsv1@fastmail.com",
     python_requires=">=3.8",
     url="https://github.com/vedro-universe/vedro-httpx",
@@ -32,10 +32,11 @@
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
     ],
 )
```

### Comparing `vedro-httpx-0.3.0/tests/test_format_response.py` & `vedro-httpx-0.4.0/tests/test_format_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.3.0/tests/test_print_response.py` & `vedro-httpx-0.4.0/tests/test_print_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.3.0/tests/test_response.py` & `vedro-httpx-0.4.0/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.3.0/vedro_httpx/_async_http_interface.py` & `vedro-httpx-0.4.0/vedro_httpx/_async_http_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,89 @@
+from datetime import datetime
 from typing import Any, Dict, Optional, Union, cast
 
 import vedro
 from httpx import URL
 from httpx import AsyncClient as _AsyncClient
 from httpx import Request
 from httpx._client import USE_CLIENT_DEFAULT, UseClientDefault
 from httpx._types import (
     AuthTypes,
-    CookieTypes,
     HeaderTypes,
     QueryParamTypes,
     RequestContent,
     RequestFiles,
     TimeoutTypes,
 )
 
 from ._response import Response
+from .recorder import RequestRecorder
+from .recorder import request_recorder as default_request_recorder
 
 __all__ = ("AsyncHTTPInterface", "AsyncClient",)
 
 
 RequestData = Dict[Any, Any]
 
 
 class AsyncClient(_AsyncClient):
     async def _send_single_request(self, request: Request) -> Response:
+        request.extensions["vedro_httpx_started_at"] = datetime.now()
+
         response = await super()._send_single_request(request)
+
         return Response(
             status_code=response.status_code,
             headers=response.headers,
             stream=response.stream,
             request=response.request,
             extensions=response.extensions,
             default_encoding=response.default_encoding,
             history=response.history,
         )
 
 
 class AsyncHTTPInterface(vedro.Interface):
-    def __init__(self, base_url: Union[URL, str] = "") -> None:
+    def __init__(self, base_url: Union[URL, str] = "", *,
+                 request_recorder: RequestRecorder = default_request_recorder) -> None:
         super().__init__()
         self._base_url = base_url
+        self._request_recorder = request_recorder
 
     # Docs https://www.python-httpx.org/api/#asyncclient
     def _client(self, **kwargs: Any) -> AsyncClient:
-        return AsyncClient(**kwargs)
+        base_url = kwargs.pop("base_url", self._base_url)
+        client = AsyncClient(base_url=base_url, **kwargs)
+        client.event_hooks["response"].append(self._request_recorder.async_record)
+        return client
 
     # Arguments are duplicated to provide auto-completion
     async def _request(self,
                        method: str,
                        url: Union[URL, str],
                        *,
                        content: Optional[RequestContent] = None,
                        data: Optional[RequestData] = None,
                        files: Optional[RequestFiles] = None,
                        json: Optional[Any] = None,
                        params: Optional[QueryParamTypes] = None,
                        headers: Optional[HeaderTypes] = None,
-                       cookies: Optional[CookieTypes] = None,
                        auth: Union[AuthTypes, UseClientDefault, None] = USE_CLIENT_DEFAULT,
                        follow_redirects: Union[bool, UseClientDefault] = USE_CLIENT_DEFAULT,
                        timeout: Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
                        **kwargs: Any
                        ) -> Response:
-        async with self._client(base_url=self._base_url, trust_env=False) as client:
+        async with self._client() as client:
             return cast(Response, await client.request(
                 method=method,
                 url=url,
                 content=content,
                 data=data,
                 files=files,
                 json=json,
                 params=params,
                 headers=headers,
-                cookies=cookies,
                 auth=auth,
                 follow_redirects=follow_redirects,
                 timeout=timeout,
                 **kwargs
             ))
```

### Comparing `vedro-httpx-0.3.0/vedro_httpx/_render_response.py` & `vedro-httpx-0.4.0/vedro_httpx/_render_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.3.0/vedro_httpx/_response.py` & `vedro-httpx-0.4.0/vedro_httpx/_response.py`

 * *Files identical despite different names*

### Comparing `vedro-httpx-0.3.0/vedro_httpx/_sync_http_interface.py` & `vedro-httpx-0.4.0/vedro_httpx/_sync_http_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,87 @@
+from datetime import datetime
 from typing import Any, Dict, Optional, Union, cast
 
 import vedro
 from httpx import URL
 from httpx import Client as _SyncClient
 from httpx import Request
 from httpx._client import USE_CLIENT_DEFAULT, UseClientDefault
 from httpx._types import (
     AuthTypes,
-    CookieTypes,
     HeaderTypes,
     QueryParamTypes,
     RequestContent,
     RequestFiles,
     TimeoutTypes,
 )
 
 from ._response import Response
+from .recorder import RequestRecorder
+from .recorder import request_recorder as default_request_recorder
 
 __all__ = ("SyncHTTPInterface", "SyncClient",)
 
 RequestData = Dict[Any, Any]
 
 
 class SyncClient(_SyncClient):
     def _send_single_request(self, request: Request) -> Response:
+        request.extensions["vedro_httpx_started_at"] = datetime.now()
+
         response = super()._send_single_request(request)
         return Response(
             status_code=response.status_code,
             headers=response.headers,
             stream=response.stream,
             request=response.request,
             extensions=response.extensions,
             default_encoding=response.default_encoding,
             history=response.history,
         )
 
 
 class SyncHTTPInterface(vedro.Interface):
-    def __init__(self, base_url: Union[URL, str] = "") -> None:
+    def __init__(self, base_url: Union[URL, str] = "", *,
+                 request_recorder: RequestRecorder = default_request_recorder) -> None:
         super().__init__()
         self._base_url = base_url
+        self._request_recorder = request_recorder
 
     # Docs https://www.python-httpx.org/api/#client
     def _client(self, **kwargs: Any) -> SyncClient:
-        return SyncClient(**kwargs)
+        base_url = kwargs.pop("base_url", self._base_url)
+        client = SyncClient(base_url=base_url, **kwargs)
+        client.event_hooks["response"].append(self._request_recorder.sync_record)
+        return client
 
     # Arguments are duplicated to provide auto-completion
     def _request(self,
                  method: str,
                  url: Union[URL, str],
                  *,
                  content: Optional[RequestContent] = None,
                  data: Optional[RequestData] = None,
                  files: Optional[RequestFiles] = None,
                  json: Optional[Any] = None,
                  params: Optional[QueryParamTypes] = None,
                  headers: Optional[HeaderTypes] = None,
-                 cookies: Optional[CookieTypes] = None,
                  auth: Union[AuthTypes, UseClientDefault, None] = USE_CLIENT_DEFAULT,
                  follow_redirects: Union[bool, UseClientDefault] = USE_CLIENT_DEFAULT,
                  timeout: Union[TimeoutTypes, UseClientDefault] = USE_CLIENT_DEFAULT,
                  **kwargs: Any
                  ) -> Response:
-        with self._client(base_url=self._base_url, trust_env=False) as client:
+        with self._client() as client:
             return cast(Response, client.request(
                 method=method,
                 url=url,
                 content=content,
                 data=data,
                 files=files,
                 json=json,
                 params=params,
                 headers=headers,
-                cookies=cookies,
                 auth=auth,
                 follow_redirects=follow_redirects,
                 timeout=timeout,
                 **kwargs
             ))
```

### Comparing `vedro-httpx-0.3.0/vedro_httpx.egg-info/PKG-INFO` & `vedro-httpx-0.4.0/vedro_httpx.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: vedro-httpx
-Version: 0.3.0
+Version: 0.4.0
 Summary: Vedro + HTTPX
 Home-page: https://github.com/vedro-universe/vedro-httpx
 Author: Nikita Tsvetkov
 Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Project-URL: Docs, https://vedro.io/docs/integrations/httpx-client
 Project-URL: GitHub, https://github.com/vedro-universe/vedro-httpx
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: httpx<1.0,>=0.23
+Requires-Dist: vedro<2.0,>=1.7
 
 # vedro-httpx
 
 [![Codecov](https://img.shields.io/codecov/c/github/vedro-universe/vedro-httpx/master.svg?style=flat-square)](https://codecov.io/gh/vedro-universe/vedro-httpx)
 [![PyPI](https://img.shields.io/pypi/v/vedro-httpx.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/vedro-httpx?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
 [![Python Version](https://img.shields.io/pypi/pyversions/vedro-httpx.svg?style=flat-square)](https://pypi.python.org/pypi/vedro-httpx/)
@@ -74,28 +77,28 @@
 ## Usage
 
 ### AsyncHTTPInterface
 
 ```python
 from vedro_httpx import Response, AsyncHTTPInterface
 
-class Api(AsyncHTTPInterface):
+class AuthAPI(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
 
 ### SyncHTTPInterface
 
 ```python
 from vedro_httpx import Response, AsyncHTTPInterface
 
-class Api(AsyncHTTPInterface):
+class AuthAPI(AsyncHTTPInterface):
     def __init__(self, base_url: str = "http://localhost:8080") -> None:
         super().__init__(base_url)
 
     async def register(self, creds: dict[str, str]) -> Response:
         return await self._request("POST", "/auth/register", json=creds)
 ```
```

