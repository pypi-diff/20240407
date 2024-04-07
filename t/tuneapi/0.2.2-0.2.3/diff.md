# Comparing `tmp/tuneapi-0.2.2.tar.gz` & `tmp/tuneapi-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneapi-0.2.2.tar", max compression
+gzip compressed data, was "tuneapi-0.2.3.tar", max compression
```

## Comparing `tuneapi-0.2.2.tar` & `tuneapi-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.2/README.md
--rw-r--r--   0        0        0      754 2024-04-04 13:48:41.808466 tuneapi-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       78 2024-04-04 13:48:41.818332 tuneapi-0.2.2/tuneapi/__init__.py
--rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.2/tuneapi/apis/__init__.py
--rw-r--r--   0        0        0     6602 2024-03-31 13:35:11.551633 tuneapi-0.2.2/tuneapi/apis/model_anthropic.py
--rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.2/tuneapi/apis/model_openai.py
--rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.2/tuneapi/apis/model_tune.py
--rw-r--r--   0        0        0      309 2024-03-30 16:59:19.448589 tuneapi-0.2.2/tuneapi/apis/threads.py
--rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.2/tuneapi/types/__init__.py
--rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.2/tuneapi/types/chats.py
--rw-r--r--   0        0        0     1423 2024-03-11 17:27:02.931939 tuneapi-0.2.2/tuneapi/utils/__init__.py
--rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.2/tuneapi/utils/env.py
--rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.2/tuneapi/utils/fs.py
--rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.2/tuneapi/utils/logger.py
--rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.2/tuneapi/utils/mime.py
--rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.2/tuneapi/utils/misc.py
--rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.2/tuneapi/utils/networking.py
--rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.2/tuneapi/utils/parallel.py
--rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.2/tuneapi/utils/randomness.py
--rw-r--r--   0        0        0     5547 2024-03-15 08:31:20.357021 tuneapi-0.2.2/tuneapi/utils/serdeser.py
--rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.2/tuneapi/utils/subway.py
--rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.2/tuneapi/utils/terminal.py
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0       30 2024-03-02 10:46:47.727709 tuneapi-0.2.3/README.md
+-rw-r--r--   0        0        0      754 2024-04-07 05:39:45.015594 tuneapi-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       78 2024-04-07 05:39:41.728370 tuneapi-0.2.3/tuneapi/__init__.py
+-rw-r--r--   0        0        0      142 2024-03-30 16:57:38.522684 tuneapi-0.2.3/tuneapi/apis/__init__.py
+-rw-r--r--   0        0        0     6703 2024-04-05 08:55:18.981956 tuneapi-0.2.3/tuneapi/apis/model_anthropic.py
+-rw-r--r--   0        0        0     8309 2024-03-30 16:56:55.006134 tuneapi-0.2.3/tuneapi/apis/model_openai.py
+-rw-r--r--   0        0        0     5521 2024-03-30 16:56:38.330332 tuneapi-0.2.3/tuneapi/apis/model_tune.py
+-rw-r--r--   0        0        0      309 2024-03-30 16:59:19.448589 tuneapi-0.2.3/tuneapi/apis/threads.py
+-rw-r--r--   0        0        0      183 2024-03-30 04:57:08.088526 tuneapi-0.2.3/tuneapi/types/__init__.py
+-rw-r--r--   0        0        0    14666 2024-04-03 06:38:04.010933 tuneapi-0.2.3/tuneapi/types/chats.py
+-rw-r--r--   0        0        0     1449 2024-04-05 08:59:10.582515 tuneapi-0.2.3/tuneapi/utils/__init__.py
+-rw-r--r--   0        0        0      279 2024-02-29 16:50:59.822352 tuneapi-0.2.3/tuneapi/utils/env.py
+-rw-r--r--   0        0        0     2389 2024-03-17 09:04:09.851851 tuneapi-0.2.3/tuneapi/utils/fs.py
+-rw-r--r--   0        0        0      958 2024-02-29 04:52:05.321819 tuneapi-0.2.3/tuneapi/utils/logger.py
+-rw-r--r--   0        0        0    33461 2024-02-28 18:58:17.252019 tuneapi-0.2.3/tuneapi/utils/mime.py
+-rw-r--r--   0        0        0     3537 2024-03-11 17:26:50.020305 tuneapi-0.2.3/tuneapi/utils/misc.py
+-rw-r--r--   0        0        0     2065 2024-02-28 18:58:23.839022 tuneapi-0.2.3/tuneapi/utils/networking.py
+-rw-r--r--   0        0        0     4653 2024-04-02 03:55:14.556441 tuneapi-0.2.3/tuneapi/utils/parallel.py
+-rw-r--r--   0        0        0      400 2024-03-08 09:25:58.748478 tuneapi-0.2.3/tuneapi/utils/randomness.py
+-rw-r--r--   0        0        0     5501 2024-04-07 05:42:46.978656 tuneapi-0.2.3/tuneapi/utils/serdeser.py
+-rw-r--r--   0        0        0     5297 2024-03-28 07:17:07.821045 tuneapi-0.2.3/tuneapi/utils/subway.py
+-rw-r--r--   0        0        0      535 2024-03-15 08:31:32.392327 tuneapi-0.2.3/tuneapi/utils/terminal.py
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 tuneapi-0.2.3/PKG-INFO
```

### Comparing `tuneapi-0.2.2/pyproject.toml` & `tuneapi-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tuneapi"
-version = "0.2.2"
+version = "0.2.3"
 description = "Tune AI APIs."
 authors = ["Frello Technology Private Limited <engineering@nimblebox.ai>"]
 license = "Apache 2.0"
 readme = "README.md"
 repository = "https://github.com/NimbleBoxAI/tuneapi"
 
 [tool.poetry.dependencies]
```

### Comparing `tuneapi-0.2.2/tuneapi/apis/model_anthropic.py` & `tuneapi-0.2.3/tuneapi/apis/model_anthropic.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,18 +65,21 @@
         if messages[0]["role"] == Message.SYSTEM:
             system = messages[0]["content"]
         start_idx = 1 if system else 0
         for m in messages[start_idx:]:
             role = m["role"]
             if m["role"] == Message.HUMAN:
                 role = "user"
+            content = m["content"]
+            if type(content) == str:
+                content = [{"type": "text", "text": content.strip()}]
             claude_messages.append(
                 {
                     "role": role,
-                    "content": [{"type": "text", "text": m["content"].strip()}],
+                    "content": content,
                 }
             )
 
         if tools:
             tool_use_system_prompt = (
                 "In this environment you have access to a set of tools you can use to answer the user's question.\n"
                 "\n"
```

### Comparing `tuneapi-0.2.2/tuneapi/apis/model_openai.py` & `tuneapi-0.2.3/tuneapi/apis/model_openai.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/apis/model_tune.py` & `tuneapi-0.2.3/tuneapi/apis/model_tune.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/types/chats.py` & `tuneapi-0.2.3/tuneapi/types/chats.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/__init__.py` & `tuneapi-0.2.3/tuneapi/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     logger,
 )
 from tuneapi.utils.serdeser import (
     to_json,
     from_json,
     dict_to_structpb,
     structpb_to_dict,
+    to_b64,
+    from_b64,
 )
 from tuneapi.utils.networking import (
     UnAuthException,
     DoNotRetryException,
     exponential_backoff,
 )
 from tuneapi.utils.parallel import (
```

### Comparing `tuneapi-0.2.2/tuneapi/utils/fs.py` & `tuneapi-0.2.3/tuneapi/utils/fs.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/logger.py` & `tuneapi-0.2.3/tuneapi/utils/logger.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/mime.py` & `tuneapi-0.2.3/tuneapi/utils/mime.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/misc.py` & `tuneapi-0.2.3/tuneapi/utils/misc.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/networking.py` & `tuneapi-0.2.3/tuneapi/utils/networking.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/parallel.py` & `tuneapi-0.2.3/tuneapi/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/serdeser.py` & `tuneapi-0.2.3/tuneapi/utils/serdeser.py`

 * *Files 3% similar despite different names*

```diff
@@ -152,20 +152,20 @@
     Args:
       path: path to load from
     """
     with open(path, "rb") as f:
         return cloudpickle.load(f)
 
 
-def py_to_bs64(x: Any):
-    return b64encode(cloudpickle.dumps(x)).decode("utf-8")
+def to_b64(x: bytes):
+    return b64encode(x).decode("utf-8")
 
 
-def py_from_bs64(x: bytes):
-    return cloudpickle.loads(b64decode(x.encode("utf-8")))
+def from_b64(x: str):
+    return b64decode(x.encode("utf-8"))
 
 
 def dict_to_structpb(data: Dict) -> Struct:
     s = Struct()
     s.update(data)
     return s
```

### Comparing `tuneapi-0.2.2/tuneapi/utils/subway.py` & `tuneapi-0.2.3/tuneapi/utils/subway.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/tuneapi/utils/terminal.py` & `tuneapi-0.2.3/tuneapi/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `tuneapi-0.2.2/PKG-INFO` & `tuneapi-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneapi
-Version: 0.2.2
+Version: 0.2.3
 Summary: Tune AI APIs.
 Home-page: https://github.com/NimbleBoxAI/tuneapi
 License: Apache 2.0
 Author: Frello Technology Private Limited
 Author-email: engineering@nimblebox.ai
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

