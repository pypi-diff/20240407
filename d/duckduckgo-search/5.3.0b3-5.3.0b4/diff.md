# Comparing `tmp/duckduckgo_search-5.3.0b3.tar.gz` & `tmp/duckduckgo_search-5.3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-5.3.0b3.tar", last modified: Sat Apr  6 13:15:41 2024, max compression
+gzip compressed data, was "duckduckgo_search-5.3.0b4.tar", last modified: Sun Apr  7 10:22:23 2024, max compression
```

## Comparing `duckduckgo_search-5.3.0b3.tar` & `duckduckgo_search-5.3.0b4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.747339 duckduckgo_search-5.3.0b3/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    40930 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 13:15:41.000000 duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 13:15:41.751339 duckduckgo_search-5.3.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-04-06 13:15:27.000000 duckduckgo_search-5.3.0b3/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:22:23.369237 duckduckgo_search-5.3.0b4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-07 10:22:23.369237 duckduckgo_search-5.3.0b4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16745 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:22:23.365237 duckduckgo_search-5.3.0b4/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      765 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42757 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       24 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:22:23.369237 duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-04-07 10:22:23.000000 duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-07 10:22:23.000000 duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:22:23.000000 duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-07 10:22:23.000000 duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-07 10:22:23.000000 duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 10:22:23.000000 duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:22:23.369237 duckduckgo_search-5.3.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:22:23.369237 duckduckgo_search-5.3.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1859 2024-04-07 10:22:12.000000 duckduckgo_search-5.3.0b4/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-5.3.0b3/LICENSE.md` & `duckduckgo_search-5.3.0b4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/PKG-INFO` & `duckduckgo_search-5.3.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.0b3
+Version: 5.3.0b4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-5.3.0b3/README.md` & `duckduckgo_search-5.3.0b4/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/duckduckgo_search/cli.py` & `duckduckgo_search-5.3.0b4/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-5.3.0b4/duckduckgo_search/duckduckgo_search.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-5.3.0b4/duckduckgo_search/duckduckgo_search_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         exc_val: Optional[BaseException] = None,
         exc_tb: Optional[TracebackType] = None,
     ) -> None:
         await self._aclient.__aexit__(exc_type, exc_val, exc_tb)
 
     def __del__(self) -> None:
         if hasattr(self, "_aclient") and self._aclient.is_closed is False:
-            with suppress(RuntimeError):
+            with suppress(RuntimeError, RuntimeWarning):
                 asyncio.create_task(self._aclient.aclose())
 
     @cached_property
     def parser(self) -> "LHTMLParser":
         """Get HTML parser."""
         return LHTMLParser(remove_blank_text=True, remove_comments=True, remove_pis=True, collect_ids=False)
 
@@ -243,19 +243,27 @@
                         result = {
                             "title": _normalize(row["t"]),
                             "href": _normalize_url(href),
                             "body": body,
                         }
                         results[priority] = result
 
-        tasks = [_text_api_page(0, 0)]
+        tasks = [asyncio.create_task(_text_api_page(0, 0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_text_api_page(s, i) for i, s in enumerate(range(23, max_results, 50), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_text_api_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
@@ -329,19 +337,27 @@
                     result = {
                         "title": _normalize(title[0]),
                         "href": _normalize_url(href),
                         "body": _normalize("".join(body)),
                     }
                     results[priority] = result
 
-        tasks = [_text_html_page(0, 0)]
+        tasks = [asyncio.create_task(_text_html_page(0, 0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_text_html_page(s, i) for i, s in enumerate(range(23, max_results, 50), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_text_html_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def _text_lite(
         self,
         keywords: str,
         region: str = "wt-wt",
@@ -412,19 +428,27 @@
                     result = {
                         "title": _normalize(title),
                         "href": _normalize_url(href),
                         "body": _normalize(body),
                     }
                     results[priority] = result
 
-        tasks = [_text_lite_page(0, 0)]
+        tasks = [asyncio.create_task(_text_lite_page(0, 0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_text_lite_page(s, i) for i, s in enumerate(range(23, max_results, 50), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_text_lite_page(s, i)) for i, s in enumerate(range(23, max_results, 50), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def images(
         self,
         keywords: str,
         region: str = "wt-wt",
@@ -507,19 +531,27 @@
                         "url": _normalize_url(row["url"]),
                         "height": row["height"],
                         "width": row["width"],
                         "source": row["source"],
                     }
                     results[priority] = result
 
-        tasks = [_images_page(0, page=0)]
+        tasks = [asyncio.create_task(_images_page(0, page=0))]
         if max_results:
             max_results = min(max_results, 500)
-            tasks.extend(_images_page(s, i) for i, s in enumerate(range(100, max_results, 100), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_images_page(s, i)) for i, s in enumerate(range(100, max_results, 100), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def videos(
         self,
         keywords: str,
         region: str = "wt-wt",
@@ -581,19 +613,27 @@
 
             for row in page_data:
                 if row["content"] not in cache:
                     cache.add(row["content"])
                     priority += 1
                     results[priority] = row
 
-        tasks = [_videos_page(0, 0)]
+        tasks = [asyncio.create_task(_videos_page(0, 0))]
         if max_results:
             max_results = min(max_results, 400)
-            tasks.extend(_videos_page(s, i) for i, s in enumerate(range(59, max_results, 59), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_videos_page(s, i)) for i, s in enumerate(range(59, max_results, 59), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def news(
         self,
         keywords: str,
         region: str = "wt-wt",
@@ -655,19 +695,27 @@
                         "body": _normalize(row["excerpt"]),
                         "url": _normalize_url(row["url"]),
                         "image": _normalize_url(image_url),
                         "source": row["source"],
                     }
                     results[priority] = result
 
-        tasks = [_news_page(0, 0)]
+        tasks = [asyncio.create_task(_news_page(0, 0))]
         if max_results:
             max_results = min(max_results, 200)
-            tasks.extend(_news_page(s, i) for i, s in enumerate(range(29, max_results, 29), start=1))
-        await asyncio.gather(*tasks)
+            tasks.extend(
+                asyncio.create_task(_news_page(s, i)) for i, s in enumerate(range(29, max_results, 29), start=1)
+            )
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return list(islice(filter(None, results), max_results))
 
     async def answers(self, keywords: str) -> List[Dict[str, str]]:
         """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params.
 
         Args:
@@ -989,11 +1037,17 @@
             )
             page_data = json_loads(resp_content)
             page_data["original"] = keyword
             results.append(page_data)
 
         if isinstance(keywords, str):
             keywords = [keywords]
-        tasks = [_translate_keyword(keyword) for keyword in keywords]
-        await asyncio.gather(*tasks)
+        tasks = [asyncio.create_task(_translate_keyword(keyword)) for keyword in keywords]
+        try:
+            await asyncio.gather(*tasks)
+        except Exception as e:
+            for task in tasks:
+                task.cancel()
+            await asyncio.gather(*tasks, return_exceptions=True)
+            raise e
 
         return results
```

### Comparing `duckduckgo_search-5.3.0b3/duckduckgo_search/utils.py` & `duckduckgo_search-5.3.0b4/duckduckgo_search/utils.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 5.3.0b3
+Version: 5.3.0b4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-5.3.0b3/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-5.3.0b4/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/pyproject.toml` & `duckduckgo_search-5.3.0b4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/tests/test_cli.py` & `duckduckgo_search-5.3.0b4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-5.3.0b3/tests/test_duckduckgo_search.py` & `duckduckgo_search-5.3.0b4/tests/test_duckduckgo_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def test_text_lite():
     results = DDGS().text("dog", backend="lite", max_results=30)
     assert 27 <= len(results) <= 30
 
 
 def test_images():
     results = DDGS().images("flower", max_results=200)
-    assert 100 <= len(results) <= 200
+    assert 95 <= len(results) <= 200
 
 
 def test_videos():
     results = DDGS().videos("sea", max_results=40)
     assert 37 <= len(results) <= 40
```

