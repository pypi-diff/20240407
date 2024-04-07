# Comparing `tmp/tuneapi-0.2.4.tar.gz` & `tmp/tuneapi-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.2.4.tar", max compression
+gzip compressed data, was "tuneapi-0.2.5.tar", max compression
```

## Comparing `tuneapi-0.2.4.tar` & `tuneapi-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.4/README.md
--rw-r--r--   0        0        0      696 2024-04-07 05:45:13.368509 tuneapi-0.2.4/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-07 05:45:09.458842 tuneapi-0.2.4/tuneapi/__init__.py
--rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.4/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6703 2024-04-05 08:55:18.981956 tuneapi-0.2.4/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.4/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.4/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0      309 2024-03-30 16:59:19.448589 tuneapi-0.2.4/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.4/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.4/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1449 2024-04-05 08:59:10.582515 tuneapi-0.2.4/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.4/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.4/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.4/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.4/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.4/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.4/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.4/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.4/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     5501 2024-04-07 05:42:46.978656 tuneapi-0.2.4/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.4/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.4/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.5/README.md
+-rw-r--r--   0        0        0      696 2024-04-07 05:56:39.783021 tuneapi-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-07 05:56:39.782698 tuneapi-0.2.5/tuneapi/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.5/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6703 2024-04-05 08:55:18.981956 tuneapi-0.2.5/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.5/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.5/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0      309 2024-03-30 16:59:19.448589 tuneapi-0.2.5/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.5/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.5/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1032 2024-04-07 05:56:12.541307 tuneapi-0.2.5/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.5/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.5/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.5/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.5/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.5/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.5/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.5/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.5/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     2430 2024-04-07 05:56:29.001597 tuneapi-0.2.5/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.5/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.5/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.5/PKG-INFO
```

### Comparing `tuneapi-0.2.4/pyproject.toml` & `tuneapi-0.2.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.2.4"
+version = "0.2.5"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.2.4/tuneapi/apis/model_anthropic.py` & `tuneapi-0.2.5/tuneapi/apis/model_anthropic.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/apis/model_openai.py` & `tuneapi-0.2.5/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/apis/model_tune.py` & `tuneapi-0.2.5/tuneapi/apis/model_tune.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/types/chats.py` & `tuneapi-0.2.5/tuneapi/types/chats.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/__init__.py` & `tuneapi-0.2.5/tuneapi/utils/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -51,15 +51,7 @@
 from tuneapi.utils.subway import (
     SubwayClientError,
     SubwayServerError,
     Subway,
     get_session,
     get_subway,
 )
-
-# sometimes services would need to not have tune dir, in which case anyone using this package can just
-# turn it off.
-if not ENV.TUNE_DISABLE_HOME_DIR("0") == "1":
-    # create the default folder for all the things that this library needs
-    os.makedirs(ENV.DEFAULT_FOLDER(os.path.expanduser("~/.tuneapi")), exist_ok=True)
-    if ENV.BLOB_ENGINE() == "local":
-        os.makedirs(ENV.BLOB_STORAGE(), exist_ok=True)
```

### Comparing `tuneapi-0.2.4/tuneapi/utils/fs.py` & `tuneapi-0.2.5/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/logger.py` & `tuneapi-0.2.5/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/mime.py` & `tuneapi-0.2.5/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/misc.py` & `tuneapi-0.2.5/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/networking.py` & `tuneapi-0.2.5/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/parallel.py` & `tuneapi-0.2.5/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/subway.py` & `tuneapi-0.2.5/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/tuneapi/utils/terminal.py` & `tuneapi-0.2.5/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.4/PKG-INFO` & `tuneapi-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.2.4
+Version: 0.2.5
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: Apache 2.0
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

