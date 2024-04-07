# Comparing `tmp/piwebx-0.0.4.tar.gz` & `tmp/piwebx-0.1.0.tar.gz`

## Comparing `piwebx-0.0.4.tar` & `piwebx-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 piwebx-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 piwebx-0.0.4/README.md
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/__init__.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/__version__.py
--rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/af.py
--rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/exceptions.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/points.py
--rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/servers.py
--rw-r--r--   0        0        0    15414 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/streams.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/types.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/util/__init__.py
--rw-r--r--   0        0        0     6088 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/util/data.py
--rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/util/response.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 piwebx-0.0.4/piwebx/util/time.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 piwebx-0.0.4/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 piwebx-0.0.4/LICENSE
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 piwebx-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 piwebx-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 piwebx-0.1.0/README.md
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/__init__.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/__version__.py
+-rw-r--r--   0        0        0     8462 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/af.py
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/exceptions.py
+-rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/points.py
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/servers.py
+-rw-r--r--   0        0        0    15461 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/streams.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/types.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/util/__init__.py
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/util/data.py
+-rw-r--r--   0        0        0     3261 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/util/response.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 piwebx-0.1.0/piwebx/util/time.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 piwebx-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 piwebx-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 piwebx-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     7040 2020-02-02 00:00:00.000000 piwebx-0.1.0/PKG-INFO
```

### Comparing `piwebx-0.0.4/piwebx/af.py` & `piwebx-0.1.0/piwebx/af.py`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/piwebx/exceptions.py` & `piwebx-0.1.0/piwebx/exceptions.py`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/piwebx/points.py` & `piwebx-0.1.0/piwebx/points.py`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/piwebx/servers.py` & `piwebx-0.1.0/piwebx/servers.py`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/piwebx/streams.py` & `piwebx-0.1.0/piwebx/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,14 +311,15 @@
 
     results = cast("list[dict[str, JSONPrimitive] | None]", [])
     requests = [
         client.get(
             f"streams/{web_id}/recordedattime",
             params={
                 "time": to_zulu_format(time),
+                "retrievalMode": "AtOrBefore",
                 "selectedFields": "Timestamp;Value;Good",
             },
         )
         for web_id in web_ids
     ]
 
     max_concurrency = max_concurrency or len(web_ids)
```

### Comparing `piwebx-0.0.4/piwebx/util/response.py` & `piwebx-0.1.0/piwebx/util/response.py`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/piwebx/util/time.py` & `piwebx-0.1.0/piwebx/util/time.py`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/.gitignore` & `piwebx-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/LICENSE` & `piwebx-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `piwebx-0.0.4/pyproject.toml` & `piwebx-0.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -7,62 +7,51 @@
 description = "Async data client for the AVEVA PI Web API"
 license = "MIT"
 requires-python = ">=3.8,<4.0"
 authors = [
     { name = "Chris Newville", email = "christopher.newville@hyprxa.io" },
 ]
 classifiers = [
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12"
 ]
 dependencies = [
-    "dateparser",
-    "httpx",
+    "dateparser>=1.0.0,<2.0.0",
+    "httpx>=0.25.0,<1.0.0",
     "orjson",
-    "pendulum",
-    "python-dateutil",
+    "pendulum>=2.1.0,<4.0.0",
+    "python-dateutil>=2.7.0,<3.0.0",
     "typing-extensions",
 ]
 dynamic = ["readme", "version"]
 
 [project.optional-dependencies]
-kerberos = ["httpx-kerberos"]
+kerberos = ["httpx-kerberos>=0.1.0,<1.0.0"]
 
 
 [project.urls]
-Changelog = "https://github.com/hyprxa/piwebx/blob/master/CHANGELOG.md"
 Homepage = "https://github.com/hyprxa/piwebx"
 Source = "https://github.com/hyprxa/piwebx"
 
 [tool.hatch.version]
 path = "./piwebx/__version__.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/piwebx",
-    "/CHANGELOG.md",
     "/README.md",
 ]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
 path = "README.md"
-
-[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
-text = "\n## Release Information\n\n"
-
-[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
-path = "CHANGELOG.md"
-
-[[tool.hatch.metadata.hooks.fancy-pypi-readme.fragments]]
-text = "\n---\n\n[Full changelog](https://github.com/hyprxa/piwebx/blob/master/CHANGELOG.md)\n"
```

