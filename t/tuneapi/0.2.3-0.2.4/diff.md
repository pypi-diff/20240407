# Comparing `tmp/tuneapi-0.2.3.tar.gz` & `tmp/tuneapi-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.2.3.tar", max compression
+gzip compressed data, was "tuneapi-0.2.4.tar", max compression
```

## Comparing `tuneapi-0.2.3.tar` & `tuneapi-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.3/README.md
--rw-r--r--   0        0        0      754 2024-04-07 05:39:45.015594 tuneapi-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-07 05:39:41.728370 tuneapi-0.2.3/tuneapi/__init__.py
--rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.3/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6703 2024-04-05 08:55:18.981956 tuneapi-0.2.3/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.3/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.3/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0      309 2024-03-30 16:59:19.448589 tuneapi-0.2.3/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.3/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.3/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1449 2024-04-05 08:59:10.582515 tuneapi-0.2.3/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.3/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.3/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.3/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.3/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.3/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.3/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.3/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.3/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     5501 2024-04-07 05:42:46.978656 tuneapi-0.2.3/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.3/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.3/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.4/README.md
+-rw-r--r--   0        0        0      696 2024-04-07 05:45:13.368509 tuneapi-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-07 05:45:09.458842 tuneapi-0.2.4/tuneapi/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.4/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6703 2024-04-05 08:55:18.981956 tuneapi-0.2.4/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.4/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.4/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0      309 2024-03-30 16:59:19.448589 tuneapi-0.2.4/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.4/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.4/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1449 2024-04-05 08:59:10.582515 tuneapi-0.2.4/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.4/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.4/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.4/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.4/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.4/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.4/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.4/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.4/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     5501 2024-04-07 05:42:46.978656 tuneapi-0.2.4/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.4/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.4/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.4/PKG-INFO
```

### Comparing `tuneapi-0.2.3/pyproject.toml` & `tuneapi-0.2.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.2.3"
+version = "0.2.4"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
 fire = "0.5.0"
 requests = "^2.31.0"
 cloudpickle = "3.0.0"
 protobuf = "^4.25.3"
-cryptography = "42.0.1"
+cryptography = ">=42.0.5"
 tqdm = "^4.66.1"
 boto3 = { version = "1.29.6", optional = true }
 
 [tool.poetry.extras]
 boto3 = ["boto3"]
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "7.2.5"
 sphinx_rtd_theme = "1.3.0"
 poetry = "1.6.1"
 
-# [tool.poetry.scripts]
-# chainfury = "chainfury.cli:main"
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tuneapi-0.2.3/tuneapi/apis/model_anthropic.py` & `tuneapi-0.2.4/tuneapi/apis/model_anthropic.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/apis/model_openai.py` & `tuneapi-0.2.4/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/apis/model_tune.py` & `tuneapi-0.2.4/tuneapi/apis/model_tune.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/types/chats.py` & `tuneapi-0.2.4/tuneapi/types/chats.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/__init__.py` & `tuneapi-0.2.4/tuneapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/fs.py` & `tuneapi-0.2.4/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/logger.py` & `tuneapi-0.2.4/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/mime.py` & `tuneapi-0.2.4/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/misc.py` & `tuneapi-0.2.4/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/networking.py` & `tuneapi-0.2.4/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/parallel.py` & `tuneapi-0.2.4/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/serdeser.py` & `tuneapi-0.2.4/tuneapi/utils/serdeser.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/subway.py` & `tuneapi-0.2.4/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/tuneapi/utils/terminal.py` & `tuneapi-0.2.4/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.3/PKG-INFO` & `tuneapi-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.2.3
+Version: 0.2.4
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: Apache 2.0
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: boto3
 Requires-Dist: boto3 (==1.29.6) ; extra == "boto3"
 Requires-Dist: cloudpickle (==3.0.0)
-Requires-Dist: cryptography (==42.0.1)
+Requires-Dist: cryptography (>=42.0.5)
 Requires-Dist: fire (==0.5.0)
 Requires-Dist: protobuf (>=4.25.3,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Project-URL: Repository, https://github.com/NimbleBoxAI/tuneapi
 Description-Content-Type: text/markdown
```

