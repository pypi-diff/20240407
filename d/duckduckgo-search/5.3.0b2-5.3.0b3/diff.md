# Comparing `tmp/duckduckgo_search-5.3.0b2.tar.gz` & `tmp/duckduckgo_search-5.3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-5.3.0b2.tar", last modified: Fri Apr  5 18:41:04 2024, max compression
+gzip compressed data, was "duckduckgo_search-5.3.0b3.tar", last modified: Sat Apr  6 13:15:41 2024, max compression
```

## Comparing `duckduckgo_search-5.3.0b2.tar` & `duckduckgo_search-5.3.0b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.773678 duckduckgo_search-5.3.0b2/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    40880 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 18:41:04.000000 duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 18:41:04.777678 duckduckgo_search-5.3.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-05 18:40:45.000000 duckduckgo_search-5.3.0b2/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.747339 duckduckgo_search-5.3.0b3/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40930 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-5.3.0b2/LICENSE.md` & `duckduckgo_search-5.3.0b3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/PKG-INFO` & `duckduckgo_search-5.3.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.0b2
+Version: 5.3.0b3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-5.3.0b2/README.md` & `duckduckgo_search-5.3.0b3/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/duckduckgo_search/__init__.py` & `duckduckgo_search-5.3.0b3/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/duckduckgo_search/cli.py` & `duckduckgo_search-5.3.0b3/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,20 +36,20 @@
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         self._close_session()
 
     def __del__(self) -> None:
-        if self._asession.is_closed is False:
-            self._close_session()
+        self._close_session()
 
     def _close_session(self) -> None:
         """Close the curl-cffi async session."""
-        self._run_async_in_thread(self._asession.aclose())
+        if hasattr(self, "_aclient") and self._aclient.is_closed is False:
+            self._run_async_in_thread(self._aclient.aclose())
 
     def _run_async_in_thread(self, coro: Awaitable[Any]) -> Any:
         """Runs an async coroutine in a separate thread."""
         future: Future[Any] = asyncio.run_coroutine_threadsafe(coro, self._loop)
         result = future.result()
         return result
```

### Comparing `duckduckgo_search-5.3.0b2/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search_async.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,40 +56,40 @@
             timeout (int, optional): Timeout value for the HTTP client. Defaults to 10.
         """
         self.proxy: Optional[str] = proxy
         assert self.proxy is None or isinstance(self.proxy, str), "proxy must be a str"
         if not proxy and proxies:
             warnings.warn("'proxies' is deprecated, use 'proxy' instead.", stacklevel=1)
             self.proxy = proxies.get("http") or proxies.get("https") if isinstance(proxies, dict) else proxies
-        self._asession = httpx.AsyncClient(
+        self._aclient = httpx.AsyncClient(
             headers=_get_headers() if headers is None else headers,
             proxy=self.proxy,
             timeout=timeout,
             follow_redirects=False,
             http2=True,
             verify=_get_ssl_context(),
         )
-        self._asession.headers["Referer"] = "https://duckduckgo.com/"
+        self._aclient.headers["Referer"] = "https://duckduckgo.com/"
         self._exception_event = asyncio.Event()
 
     async def __aenter__(self) -> "AsyncDDGS":
         return self
 
     async def __aexit__(
         self,
         exc_type: Optional[Type[BaseException]] = None,
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
-        await self._asession.aclose()
+        await self._aclient.__aexit__(exc_type, exc_val, exc_tb)
 
     def __del__(self) -> None:
-        if self._asession.is_closed is False:
+        if hasattr(self, "_aclient") and self._aclient.is_closed is False:
             with suppress(RuntimeError):
-                asyncio.create_task(self._asession.aclose())
+                asyncio.create_task(self._aclient.aclose())
 
     @cached_property
     def parser(self) -> "LHTMLParser":
         """Get HTML parser."""
         return LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
 
     @classmethod
@@ -110,15 +110,15 @@
         content: Optional[Union[str, bytes]] = None,
         data: Optional[Dict[str, Any]] = None,
         params: Optional[Dict[str, str]] = None,
     ) -> bytes:
         if self._exception_event.is_set():
             raise DuckDuckGoSearchException("Exception occurred in previous call.")
         try:
-            resp = await self._asession.request(method, url, content=content, data=data, params=params)
+            resp = await self._aclient.request(method, url, content=content, data=data, params=params)
         except httpx.TimeoutException as ex:
             self._exception_event.set()
             raise TimeoutException(f"{url} {type(ex).__name__}: {ex}") from ex
         except Exception as ex:
             self._exception_event.set()
             raise DuckDuckGoSearchException(f"{url} {type(ex).__name__}: {ex}") from ex
         if resp.status_code == 200:
@@ -278,15 +278,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._asession.headers["Referer"] = "https://html.duckduckgo.com/"
+        self._aclient.headers["Referer"] = "https://html.duckduckgo.com/"
         safesearch_base = {"on": "1", "moderate": "-1", "off": "-2"}
         payload = {
             "q": keywords,
             "kl": region,
             "p": safesearch_base[safesearch.lower()],
             "o": "json",
             "api": "d.js",
@@ -362,15 +362,15 @@
         Raises:
             DuckDuckGoSearchException: Base exception for duckduckgo_search errors.
             RatelimitException: Inherits from DuckDuckGoSearchException, raised for exceeding API request rate limits.
             TimeoutException: Inherits from DuckDuckGoSearchException, raised for API request timeouts.
         """
         assert keywords, "keywords is mandatory"
 
-        self._asession.headers["Referer"] = "https://lite.duckduckgo.com/"
+        self._aclient.headers["Referer"] = "https://lite.duckduckgo.com/"
         payload = {
             "q": keywords,
             "o": "json",
             "api": "d.js",
             "kl": region,
         }
         if timelimit:
```

### Comparing `duckduckgo_search-5.3.0b2/duckduckgo_search/utils.py` & `duckduckgo_search-5.3.0b3/duckduckgo_search/utils.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.0b2
+Version: 5.3.0b3
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-5.3.0b2/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/pyproject.toml` & `duckduckgo_search-5.3.0b3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/tests/test_cli.py` & `duckduckgo_search-5.3.0b3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b2/tests/test_duckduckgo_search.py` & `duckduckgo_search-5.3.0b3/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

