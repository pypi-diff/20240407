# Comparing `tmp/rockai_cli_app-0.1.8.tar.gz` & `tmp/rockai_cli_app-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rockai_cli_app-0.1.8.tar", max compression
+gzip compressed data, was "rockai_cli_app-0.1.9.tar", max compression
```

## Comparing `rockai_cli_app-0.1.8.tar` & `rockai_cli_app-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       72 2024-03-05 09:01:49.763544 rockai_cli_app-0.1.8/README.md
--rw-r--r--   0        0        0      619 2024-04-03 07:46:48.396859 rockai_cli_app-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-07 03:29:24.441443 rockai_cli_app-0.1.8/rockai_cli_app/__init__.py
--rw-r--r--   0        0        0     2346 2024-04-03 07:24:35.496357 rockai_cli_app-0.1.8/rockai_cli_app/data_class.py
--rw-r--r--   0        0        0        0 2024-03-01 08:25:13.083771 rockai_cli_app-0.1.8/rockai_cli_app/docker/__init__.py
--rw-r--r--   0        0        0    11652 2024-04-02 08:30:02.204871 rockai_cli_app-0.1.8/rockai_cli_app/docker/docker_util.py
--rw-r--r--   0        0        0     2819 2024-03-01 08:15:55.566855 rockai_cli_app-0.1.8/rockai_cli_app/docker/tf_compat.json
--rw-r--r--   0        0        0      604 2024-03-26 06:45:43.007156 rockai_cli_app-0.1.8/rockai_cli_app/docker/torch_compat.json
--rw-r--r--   0        0        0     1406 2024-03-08 06:28:07.738273 rockai_cli_app-0.1.8/rockai_cli_app/main.py
--rw-r--r--   0        0        0        0 2024-02-28 08:04:20.239254 rockai_cli_app-0.1.8/rockai_cli_app/parser/__init__.py
--rw-r--r--   0        0        0      799 2024-02-28 09:29:39.709568 rockai_cli_app-0.1.8/rockai_cli_app/parser/config_util.py
--rw-r--r--   0        0        0      290 2024-02-07 03:35:01.202042 rockai_cli_app-0.1.8/rockai_cli_app/predictor.py
--rw-r--r--   0        0        0        0 2024-02-07 03:35:44.528854 rockai_cli_app-0.1.8/rockai_cli_app/server/__init__.py
--rw-r--r--   0        0        0     2569 2024-04-03 07:46:25.050529 rockai_cli_app-0.1.8/rockai_cli_app/server/http.py
--rw-r--r--   0        0        0       77 2024-02-07 06:52:07.739336 rockai_cli_app-0.1.8/rockai_cli_app/server/runner.py
--rw-r--r--   0        0        0        0 2024-02-20 09:20:10.188788 rockai_cli_app-0.1.8/rockai_cli_app/server/test/__init__.py
--rw-r--r--   0        0        0      783 2024-02-28 07:05:00.986936 rockai_cli_app-0.1.8/rockai_cli_app/server/test/predict.py
--rw-r--r--   0        0        0      149 2024-02-20 06:38:03.569237 rockai_cli_app-0.1.8/rockai_cli_app/server/test/test_config.yaml
--rw-r--r--   0        0        0     8582 2024-02-23 06:25:29.351387 rockai_cli_app-0.1.8/rockai_cli_app/server/types.py
--rw-r--r--   0        0        0     8639 2024-02-28 09:23:42.650045 rockai_cli_app-0.1.8/rockai_cli_app/server/utils.py
--rw-r--r--   0        0        0        0 2024-02-07 05:25:34.434644 rockai_cli_app-0.1.8/rockai_cli_app/server/worker.py
--rw-r--r--   0        0        0      703 2024-02-22 08:32:41.013574 rockai_cli_app-0.1.8/rockai_cli_app/test.py
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 rockai_cli_app-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       72 2024-03-05 09:01:49.763544 rockai_cli_app-0.1.9/README.md
+-rw-r--r--   0        0        0      619 2024-04-07 03:06:56.162738 rockai_cli_app-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-07 03:29:24.441443 rockai_cli_app-0.1.9/rockai_cli_app/__init__.py
+-rw-r--r--   0        0        0     2346 2024-04-03 07:24:35.496357 rockai_cli_app-0.1.9/rockai_cli_app/data_class.py
+-rw-r--r--   0        0        0        0 2024-03-01 08:25:13.083771 rockai_cli_app-0.1.9/rockai_cli_app/docker/__init__.py
+-rw-r--r--   0        0        0    11652 2024-04-02 08:30:02.204871 rockai_cli_app-0.1.9/rockai_cli_app/docker/docker_util.py
+-rw-r--r--   0        0        0     2819 2024-03-01 08:15:55.566855 rockai_cli_app-0.1.9/rockai_cli_app/docker/tf_compat.json
+-rw-r--r--   0        0        0      604 2024-03-26 06:45:43.007156 rockai_cli_app-0.1.9/rockai_cli_app/docker/torch_compat.json
+-rw-r--r--   0        0        0     1406 2024-03-08 06:28:07.738273 rockai_cli_app-0.1.9/rockai_cli_app/main.py
+-rw-r--r--   0        0        0        0 2024-02-28 08:04:20.239254 rockai_cli_app-0.1.9/rockai_cli_app/parser/__init__.py
+-rw-r--r--   0        0        0      799 2024-02-28 09:29:39.709568 rockai_cli_app-0.1.9/rockai_cli_app/parser/config_util.py
+-rw-r--r--   0        0        0      290 2024-02-07 03:35:01.202042 rockai_cli_app-0.1.9/rockai_cli_app/predictor.py
+-rw-r--r--   0        0        0        0 2024-02-07 03:35:44.528854 rockai_cli_app-0.1.9/rockai_cli_app/server/__init__.py
+-rw-r--r--   0        0        0     2569 2024-04-03 07:46:25.050529 rockai_cli_app-0.1.9/rockai_cli_app/server/http.py
+-rw-r--r--   0        0        0       77 2024-02-07 06:52:07.739336 rockai_cli_app-0.1.9/rockai_cli_app/server/runner.py
+-rw-r--r--   0        0        0        0 2024-02-20 09:20:10.188788 rockai_cli_app-0.1.9/rockai_cli_app/server/test/__init__.py
+-rw-r--r--   0        0        0      783 2024-02-28 07:05:00.986936 rockai_cli_app-0.1.9/rockai_cli_app/server/test/predict.py
+-rw-r--r--   0        0        0      149 2024-02-20 06:38:03.569237 rockai_cli_app-0.1.9/rockai_cli_app/server/test/test_config.yaml
+-rw-r--r--   0        0        0     8582 2024-02-23 06:25:29.351387 rockai_cli_app-0.1.9/rockai_cli_app/server/types.py
+-rw-r--r--   0        0        0     8643 2024-04-07 03:06:47.237759 rockai_cli_app-0.1.9/rockai_cli_app/server/utils.py
+-rw-r--r--   0        0        0        0 2024-02-07 05:25:34.434644 rockai_cli_app-0.1.9/rockai_cli_app/server/worker.py
+-rw-r--r--   0        0        0      703 2024-02-22 08:32:41.013574 rockai_cli_app-0.1.9/rockai_cli_app/test.py
+-rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 rockai_cli_app-0.1.9/PKG-INFO
```

### Comparing `rockai_cli_app-0.1.8/pyproject.toml` & `rockai_cli_app-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rockai-cli-app"
-version = "0.1.8"
+version = "0.1.9"
 description = "For inference and training"
 authors = ["Rocky <some_developer@example.com>"]
 readme = "README.md"
 include = ["./rockai_cli_app/docker/tf_compat.json","./rockai_cli_app/docker/torch_compat.json"]
 
 [tool.poetry.scripts]
 rock = "rockai_cli_app.main:app"
```

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/data_class.py` & `rockai_cli_app-0.1.9/rockai_cli_app/data_class.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/docker/docker_util.py` & `rockai_cli_app-0.1.9/rockai_cli_app/docker/docker_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/docker/tf_compat.json` & `rockai_cli_app-0.1.9/rockai_cli_app/docker/tf_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/docker/torch_compat.json` & `rockai_cli_app-0.1.9/rockai_cli_app/docker/torch_compat.json`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/main.py` & `rockai_cli_app-0.1.9/rockai_cli_app/main.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/parser/config_util.py` & `rockai_cli_app-0.1.9/rockai_cli_app/parser/config_util.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/server/http.py` & `rockai_cli_app-0.1.9/rockai_cli_app/server/http.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/server/test/predict.py` & `rockai_cli_app-0.1.9/rockai_cli_app/server/test/predict.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/server/types.py` & `rockai_cli_app-0.1.9/rockai_cli_app/server/types.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/server/utils.py` & `rockai_cli_app-0.1.9/rockai_cli_app/server/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,16 +120,16 @@
             # If user hasn't used `Input`, then wrap it in that
             if not isinstance(default, FieldInfo):
                 default = Input(default=default)
 
         # Fields aren't ordered, so use this pattern to ensure defined order
         # https://github.com/go-openapi/spec/pull/116
         
-        default.json_schema_extra["x-order"] = order
-        order += 1
+        # default.json_schema_extra["x-order"] = order
+        # order += 1
 
         # Choices!
         if default.json_schema_extra.get("choices"):
             choices = default.json_schema_extra["choices"]
             # It will be passed automatically as 'enum' in the schema, so remove it as an extra field.
             del default.json_schema_extra["choices"]
             if InputType == str:
```

### Comparing `rockai_cli_app-0.1.8/rockai_cli_app/test.py` & `rockai_cli_app-0.1.9/rockai_cli_app/test.py`

 * *Files identical despite different names*

### Comparing `rockai_cli_app-0.1.8/PKG-INFO` & `rockai_cli_app-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rockai-cli-app
-Version: 0.1.8
+Version: 0.1.9
 Summary: For inference and training
 Author: Rocky
 Author-email: some_developer@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

