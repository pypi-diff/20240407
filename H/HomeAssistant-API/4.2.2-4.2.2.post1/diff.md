# Comparing `tmp/homeassistant_api-4.2.2.tar.gz` & `tmp/homeassistant_api-4.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeassistant_api-4.2.2.tar", max compression
+gzip compressed data, was "homeassistant_api-4.2.2.post1.tar", max compression
```

## Comparing `homeassistant_api-4.2.2.tar` & `homeassistant_api-4.2.2.post1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    32473 2024-03-14 19:12:39.525463 homeassistant_api-4.2.2/LICENSE
--rw-r--r--   0        0        0     2147 2024-03-14 19:12:39.525463 homeassistant_api-4.2.2/README.md
--rw-r--r--   0        0        0     1027 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/__init__.py
--rw-r--r--   0        0        0     1313 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/client.py
--rw-r--r--   0        0        0     2841 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/errors.py
--rw-r--r--   0        0        0      474 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/__init__.py
--rw-r--r--   0        0        0      534 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/base.py
--rw-r--r--   0        0        0     4241 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/domains.py
--rw-r--r--   0        0        0     4293 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/entity.py
--rw-r--r--   0        0        0     1387 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/events.py
--rw-r--r--   0        0        0      720 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/history.py
--rw-r--r--   0        0        0      979 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/logbook.py
--rw-r--r--   0        0        0     1361 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/models/states.py
--rw-r--r--   0        0        0     5458 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/processing.py
--rw-r--r--   0        0        0        0 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/py.typed
--rw-r--r--   0        0        0    13663 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/rawasyncclient.py
--rw-r--r--   0        0        0     5570 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/rawbaseclient.py
--rw-r--r--   0        0        0    13008 2024-03-14 19:12:39.529463 homeassistant_api-4.2.2/homeassistant_api/rawclient.py
--rw-r--r--   0        0        0     2260 2024-03-14 19:12:39.533463 homeassistant_api-4.2.2/pyproject.toml
--rw-r--r--   0        0        0     3271 1970-01-01 00:00:00.000000 homeassistant_api-4.2.2/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-04-07 04:20:53.364350 homeassistant_api-4.2.2.post1/LICENSE
+-rw-r--r--   0        0        0     2147 2024-04-07 04:20:53.364350 homeassistant_api-4.2.2.post1/README.md
+-rw-r--r--   0        0        0     1027 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/__init__.py
+-rw-r--r--   0        0        0     1313 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/client.py
+-rw-r--r--   0        0        0     2841 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/errors.py
+-rw-r--r--   0        0        0      474 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/__init__.py
+-rw-r--r--   0        0        0      534 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/base.py
+-rw-r--r--   0        0        0     4241 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/domains.py
+-rw-r--r--   0        0        0     4293 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/entity.py
+-rw-r--r--   0        0        0     1387 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/events.py
+-rw-r--r--   0        0        0      720 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/history.py
+-rw-r--r--   0        0        0      979 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/logbook.py
+-rw-r--r--   0        0        0     1361 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/models/states.py
+-rw-r--r--   0        0        0     5458 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/processing.py
+-rw-r--r--   0        0        0        0 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/py.typed
+-rw-r--r--   0        0        0    13663 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/rawasyncclient.py
+-rw-r--r--   0        0        0     5570 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/rawbaseclient.py
+-rw-r--r--   0        0        0    13008 2024-04-07 04:20:53.368351 homeassistant_api-4.2.2.post1/homeassistant_api/rawclient.py
+-rw-r--r--   0        0        0     2267 2024-04-07 04:20:53.372351 homeassistant_api-4.2.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     3270 1970-01-01 00:00:00.000000 homeassistant_api-4.2.2.post1/PKG-INFO
```

### Comparing `homeassistant_api-4.2.2/LICENSE` & `homeassistant_api-4.2.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/README.md` & `homeassistant_api-4.2.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/__init__.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/__init__.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/client.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/client.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/errors.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/errors.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/models/base.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/models/base.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/models/domains.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/models/domains.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/models/entity.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/models/entity.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/models/events.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/models/events.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/models/history.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/models/history.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/models/logbook.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/models/logbook.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/models/states.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/models/states.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/processing.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/processing.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/rawasyncclient.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/rawasyncclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/rawbaseclient.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/rawbaseclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/homeassistant_api/rawclient.py` & `homeassistant_api-4.2.2.post1/homeassistant_api/rawclient.py`

 * *Files identical despite different names*

### Comparing `homeassistant_api-4.2.2/pyproject.toml` & `homeassistant_api-4.2.2.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 documentation = "https://homeassistantapi.readthedocs.io"
 homepage = "https://github.com/GrandMoff100/HomeAssistantAPI"
 license = "GPL-3.0-or-later"
 name = "HomeAssistant-API"
 readme = "README.md"
 include = ["homeassistant_api/py.typed"]
 repository = "https://github.com/GrandMoff100/HomeAssistantAPI"
-version = "4.2.2"
+version = "4.2.2.post1"
 packages = [{ include = "homeassistant_api" }]
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.1"
-aiohttp-client-cache = "^0.6.1"
+aiohttp-client-cache = ">=0.6.1"
 pydantic = ">=2.0"
 python = "^3.8,<4.0.0"
 requests = "^2.27.1"
 requests-cache = "^0.9.2"
 simplejson = "^3.17.6"
 
 [tool.poetry.group.docs]
```

### Comparing `homeassistant_api-4.2.2/PKG-INFO` & `homeassistant_api-4.2.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: HomeAssistant-API
-Version: 4.2.2
+Version: 4.2.2.post1
 Summary: Python Wrapper for Homeassistant's REST API
 Home-page: https://github.com/GrandMoff100/HomeAssistantAPI
 License: GPL-3.0-or-later
 Author: GrandMoff100
 Author-email: minecraftcrusher100@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
-Requires-Dist: aiohttp-client-cache (>=0.6.1,<0.7.0)
+Requires-Dist: aiohttp-client-cache (>=0.6.1)
 Requires-Dist: pydantic (>=2.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: requests-cache (>=0.9.2,<0.10.0)
 Requires-Dist: simplejson (>=3.17.6,<4.0.0)
 Project-URL: Documentation, https://homeassistantapi.readthedocs.io
 Project-URL: Repository, https://github.com/GrandMoff100/HomeAssistantAPI
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: HomeAssistant-API Version: 4.2.2 Summary: Python
-Wrapper for Homeassistant's REST API Home-page: https://github.com/
+Metadata-Version: 2.1 Name: HomeAssistant-API Version: 4.2.2.post1 Summary:
+Python Wrapper for Homeassistant's REST API Home-page: https://github.com/
 GrandMoff100/HomeAssistantAPI License: GPL-3.0-or-later Author: GrandMoff100
 Author-email: minecraftcrusher100@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: aiohttp (>=3.8.1,<4.0.0) Requires-Dist: aiohttp-
-client-cache (>=0.6.1,<0.7.0) Requires-Dist: pydantic (>=2.0) Requires-Dist:
-requests (>=2.27.1,<3.0.0) Requires-Dist: requests-cache (>=0.9.2,<0.10.0)
-Requires-Dist: simplejson (>=3.17.6,<4.0.0) Project-URL: Documentation, https:/
-/homeassistantapi.readthedocs.io Project-URL: Repository, https://github.com/
+client-cache (>=0.6.1) Requires-Dist: pydantic (>=2.0) Requires-Dist: requests
+(>=2.27.1,<3.0.0) Requires-Dist: requests-cache (>=0.9.2,<0.10.0) Requires-
+Dist: simplejson (>=3.17.6,<4.0.0) Project-URL: Documentation, https://
+homeassistantapi.readthedocs.io Project-URL: Repository, https://github.com/
 GrandMoff100/HomeAssistantAPI Description-Content-Type: text/markdown #
 HomeassistantAPI [![Code Coverage](https://img.shields.io/codecov/c/github/
 GrandMoff100/HomeAssistantAPI/dev?style=for-the-badge&token=SJFC3HX5R1)](https:
 //codecov.io/gh/GrandMoff100/HomeAssistantAPI) [![PyPI - Downloads](https://
 img.shields.io/pypi/dm/HomeAssistant-API?style=for-the-badge)](https://
 pypi.org/project/homeassistant_api) ![GitHub commits since latest release (by
 date including pre-releases)](https://img.shields.io/github/commits-since/
```

