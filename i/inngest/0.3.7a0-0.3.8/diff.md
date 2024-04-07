# Comparing `tmp/inngest-0.3.7a0.tar.gz` & `tmp/inngest-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inngest-0.3.7a0.tar", last modified: Wed Mar 20 23:26:49 2024, max compression
+gzip compressed data, was "inngest-0.3.8.tar", last modified: Sun Apr  7 14:47:09 2024, max compression
```

## Comparing `inngest-0.3.7a0.tar` & `inngest-0.3.8.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:49.197114 inngest-0.3.7a0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 23:26:27.000000 inngest-0.3.7a0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-03-20 23:26:49.197114 inngest-0.3.7a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-03-20 23:26:27.000000 inngest-0.3.7a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:49.189113 inngest-0.3.7a0/inngest/
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:49.193113 inngest-0.3.7a0/inngest/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/client_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/client_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18081 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/comm_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/const_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/event_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/event_lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/function_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/function_config_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:49.193113 inngest-0.3.7a0/inngest/_internal/middleware_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/middleware_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/middleware_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/middleware_lib/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/middleware_lib/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/net.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/net_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:49.193113 inngest-0.3.7a0/inngest/_internal/step_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/step_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/step_lib/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/step_lib/step_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/step_lib/step_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/transforms_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/django.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/experimental.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-20 23:26:27.000000 inngest-0.3.7a0/inngest/tornado.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:49.197114 inngest-0.3.7a0/inngest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-03-20 23:26:49.000000 inngest-0.3.7a0/inngest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-03-20 23:26:49.000000 inngest-0.3.7a0/inngest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 23:26:49.000000 inngest-0.3.7a0/inngest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-20 23:26:49.000000 inngest-0.3.7a0/inngest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-20 23:26:49.000000 inngest-0.3.7a0/inngest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2528 2024-03-20 23:26:27.000000 inngest-0.3.7a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 23:26:49.197114 inngest-0.3.7a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 23:26:49.193113 inngest-0.3.7a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-20 23:26:27.000000 inngest-0.3.7a0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-20 23:26:27.000000 inngest-0.3.7a0/tests/test_django.py
--rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-03-20 23:26:27.000000 inngest-0.3.7a0/tests/test_fast_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-03-20 23:26:27.000000 inngest-0.3.7a0/tests/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-20 23:26:27.000000 inngest-0.3.7a0/tests/test_tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-03-20 23:26:27.000000 inngest-0.3.7a0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.904055 inngest-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 14:46:48.000000 inngest-0.3.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-07 14:47:09.904055 inngest-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-04-07 14:46:48.000000 inngest-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.892055 inngest-0.3.8/inngest/
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14077 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/client_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/client_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18680 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/comm_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/const_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/env_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/event_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/event_lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17117 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/function_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/function_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest/_internal/middleware_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6134 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/middleware_lib/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/net_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest/_internal/step_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12228 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/step_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11811 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/step_lib/step_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/transforms_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-07 14:46:48.000000 inngest-0.3.8/inngest/tornado.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/inngest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7247 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-07 14:47:09.000000 inngest-0.3.8/inngest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2526 2024-04-07 14:46:48.000000 inngest-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:47:09.904055 inngest-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:47:09.900055 inngest-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5858 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_fast_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-04-07 14:46:48.000000 inngest-0.3.8/tests/test_types.py
```

### Comparing `inngest-0.3.7a0/LICENSE.md` & `inngest-0.3.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/PKG-INFO` & `inngest-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inngest
-Version: 0.3.7a0
+Version: 0.3.8
 Summary: Python SDK for Inngest
 Project-URL: Homepage, https://github.com/inngest/inngest-py
 Project-URL: Bug Tracker, https://github.com/inngest/inngest-py/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inngest Version: 0.3.7a0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: inngest Version: 0.3.8 Summary: Python SDK for
 Inngest Project-URL: Homepage, https://github.com/inngest/inngest-py Project-
 URL: Bug Tracker, https://github.com/inngest/inngest-py/issues Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: Django Classifier:
 Framework :: FastAPI Classifier: Framework :: Flask Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `inngest-0.3.7a0/README.md` & `inngest-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/__init__.py` & `inngest-0.3.8/inngest/__init__.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/client_lib.py` & `inngest-0.3.8/inngest/_internal/client_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import typing
 import urllib.parse
 
 import httpx
 
 from . import (
     const,
-    env,
+    env_lib,
     errors,
     event_lib,
     function,
     function_config,
     net,
     types,
 )
@@ -103,20 +103,16 @@
 
         self.middleware = middleware or []
         self._event_key = event_key or os.getenv(const.EnvKey.EVENT_KEY.value)
 
         self._signing_key = signing_key or os.getenv(
             const.EnvKey.SIGNING_KEY.value
         )
-        if self._signing_key is None and self._mode == const.ServerKind.CLOUD:
-            raise errors.SigningKeyMissingError(
-                f"Signing key must be set when Cloud mode is enabled. If you don't want to use Cloud mode, set the {const.EnvKey.DEV.value} env var."
-            )
 
-        self._env = env or os.getenv(const.EnvKey.ENV.value)
+        self._env = env or env_lib.get_environment_name()
         if (
             self._env is None
             and self._signing_key is not None
             and "branch" in self._signing_key
         ):
             self.logger.warning(
                 "Signing key is for a branch environment but no branch environment is specified. This may cause unexpected behavior"
@@ -452,15 +448,15 @@
         if is_production:
             logger.debug("Cloud mode enabled by client argument")
             return const.ServerKind.CLOUD
 
         logger.debug("Dev Server mode enabled by client argument")
         return const.ServerKind.DEV_SERVER
 
-    if env.is_true(const.EnvKey.DEV):
+    if env_lib.is_true(const.EnvKey.DEV):
         logger.debug(
             f"Dev Server mode enabled by {const.EnvKey.DEV.value} env var"
         )
         return const.ServerKind.DEV_SERVER
 
     logger.debug(
         f"Cloud mode enabled. Set {const.EnvKey.DEV.value} to enable development mode"
```

### Comparing `inngest-0.3.7a0/inngest/_internal/client_lib_test.py` & `inngest-0.3.8/inngest/_internal/client_lib_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -87,21 +87,23 @@
     def test_signing_key_param(self) -> None:
         client = client_lib.Inngest(
             app_id="test",
             signing_key="foo1",
         )
         assert client.signing_key == "foo1"
 
-    def test_signing_key_missing(self) -> None:
+    def test_cloud_mode_without_signing_key(self) -> None:
         """
-        Error is raised when the signing key is not set in production.
+        When in Cloud mode but no signing key, no error is raised. This behavior
+        is necessary because some users may only use the Inngest client for
+        sending events. The signing key should only be required when serving
+        Inngest functions in Cloud mode
         """
 
-        with pytest.raises(errors.SigningKeyMissingError):
-            client_lib.Inngest(app_id="test")
+        client_lib.Inngest(app_id="test")
 
     def test_api_base_url_env_var(self) -> None:
         os.environ[const.EnvKey.API_BASE_URL.value] = "example.com"
         self.addCleanup(lambda: os.environ.pop(const.EnvKey.API_BASE_URL.value))
         client = client_lib.Inngest(
             app_id="test",
             signing_key="foo",
```

### Comparing `inngest-0.3.7a0/inngest/_internal/comm.py` & `inngest-0.3.8/inngest/_internal/comm.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,22 +217,24 @@
         headers = net.create_headers(
             env=self._client.env,
             framework=self._framework,
             server_kind=server_kind,
             signing_key=self._signing_key,
         )
 
+        params = {}
+        if sync_id is not None:
+            params[const.QueryParamKey.SYNC_ID.value] = sync_id
+
         return httpx.Client().build_request(
             "POST",
             registration_url,
             headers=headers,
             json=transforms.prep_body(body),
-            params={
-                const.QueryParamKey.SYNC_ID.value: sync_id,
-            },
+            params=params,
             timeout=30,
         )
 
     async def call_function(
         self,
         *,
         call: execution.Call,
@@ -401,25 +403,37 @@
             return errors.FunctionConfigInvalidError("no functions found")
         return configs
 
     def inspect(
         self, server_kind: typing.Optional[const.ServerKind]
     ) -> CommResponse:
         """Handle Dev Server's auto-discovery."""
-        if server_kind != self._mode:
+
+        if server_kind is not None and server_kind != self._mode:
             # Tell Dev Server to leave the app alone since it's in production
             # mode.
             return CommResponse(
                 body={},
                 headers={},
                 status_code=403,
             )
 
+        body = _Inspection(
+            function_count=len(self._fns),
+            has_event_key=self._client.event_key is not None,
+            has_signing_key=self._signing_key is not None,
+            mode=self._mode,
+        ).to_dict()
+        if isinstance(body, Exception):
+            body = {
+                "error": "failed to serialize inspection data",
+            }
+
         return CommResponse(
-            body={},
+            body=body,
             headers=net.create_headers(
                 env=self._client.env,
                 framework=self._framework,
                 server_kind=server_kind,
                 signing_key=None,
             ),
             status_code=200,
@@ -563,7 +577,14 @@
             return CommResponse.from_error_code(
                 const.ErrorCode.SERVER_KIND_MISMATCH,
                 msg,
                 http.HTTPStatus.BAD_REQUEST,
             )
 
         return None
+
+
+class _Inspection(types.BaseModel):
+    function_count: int
+    has_event_key: bool
+    has_signing_key: bool
+    mode: const.ServerKind
```

### Comparing `inngest-0.3.7a0/inngest/_internal/comm_test.py` & `inngest-0.3.8/inngest/_internal/comm_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/const.py` & `inngest-0.3.8/inngest/_internal/const.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,40 @@
 import typing
 
 DEFAULT_API_ORIGIN: typing.Final = "https://api.inngest.com/"
 DEFAULT_EVENT_ORIGIN: typing.Final = "https://inn.gs/"
 DEV_SERVER_ORIGIN: typing.Final = "http://127.0.0.1:8288/"
 LANGUAGE: typing.Final = "py"
 ROOT_STEP_ID: typing.Final = "step"
-VERSION: typing.Final = "0.3.7a0"
+VERSION: typing.Final = "0.3.8"
 
 
 class EnvKey(enum.Enum):
     API_BASE_URL = "INNGEST_API_BASE_URL"
     DEV = "INNGEST_DEV"
     EVENT_API_BASE_URL = "INNGEST_EVENT_API_BASE_URL"
     EVENT_KEY = "INNGEST_EVENT_KEY"
     ENV = "INNGEST_ENV"
+
+    # Railway deployment's git branch
+    # https://docs.railway.app/develop/variables#railway-provided-variables
+    RAILWAY_GIT_BRANCH = "RAILWAY_GIT_BRANCH"
+
+    # Render deployment's git branch
+    # https://render.com/docs/environment-variables#all-services
+    RENDER_GIT_BRANCH = "RENDER_GIT_BRANCH"
+
     SERVE_ORIGIN = "INNGEST_SERVE_ORIGIN"
     SERVE_PATH = "INNGEST_SERVE_PATH"
     SIGNING_KEY = "INNGEST_SIGNING_KEY"
 
+    # Vercel deployment's git branch
+    # https://vercel.com/docs/concepts/projects/environment-variables/system-environment-variables#system-environment-variables
+    VERCEL_GIT_BRANCH = "VERCEL_GIT_COMMIT_REF"
+
 
 class ErrorCode(enum.Enum):
     ASYNC_UNSUPPORTED = "async_unsupported"
     BODY_INVALID = "body_invalid"
     EVENT_KEY_UNSPECIFIED = "event_key_unspecified"
     FUNCTION_CONFIG_INVALID = "function_config_invalid"
     FUNCTION_NOT_FOUND = "function_not_found"
```

### Comparing `inngest-0.3.7a0/inngest/_internal/errors.py` & `inngest-0.3.8/inngest/_internal/errors.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/event_lib_test.py` & `inngest-0.3.8/inngest/_internal/event_lib_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/execution.py` & `inngest-0.3.8/inngest/_internal/execution.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/function.py` & `inngest-0.3.8/inngest/_internal/function.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/function_config.py` & `inngest-0.3.8/inngest/_internal/function_config.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/function_config_test.py` & `inngest-0.3.8/inngest/_internal/function_config_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/log.py` & `inngest-0.3.8/inngest/_internal/log.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/middleware_lib/log.py` & `inngest-0.3.8/inngest/_internal/middleware_lib/log.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/middleware_lib/manager.py` & `inngest-0.3.8/inngest/_internal/middleware_lib/manager.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/middleware_lib/middleware.py` & `inngest-0.3.8/inngest/_internal/middleware_lib/middleware.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/net.py` & `inngest-0.3.8/inngest/_internal/net.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/net_test.py` & `inngest-0.3.8/inngest/_internal/net_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/step_lib/base.py` & `inngest-0.3.8/inngest/_internal/step_lib/base.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/step_lib/step_async.py` & `inngest-0.3.8/inngest/_internal/step_lib/step_async.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/step_lib/step_sync.py` & `inngest-0.3.8/inngest/_internal/step_lib/step_sync.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/transforms.py` & `inngest-0.3.8/inngest/_internal/transforms.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/transforms_test.py` & `inngest-0.3.8/inngest/_internal/transforms_test.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/_internal/types.py` & `inngest-0.3.8/inngest/_internal/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,17 +42,18 @@
     # "possible cyclic definition"
     JSON = typing_extensions.TypeAliasType(
         "JSON",
         typing.Union[
             bool,
             int,
             float,
-            typing.Optional[str],
-            list["JSON"],
+            str,
             dict[str, "JSON"],
+            list["JSON"],
+            None,
         ],
     )
 
 
 JSONT = typing.TypeVar("JSONT", bound=JSON)
```

### Comparing `inngest-0.3.7a0/inngest/django.py` & `inngest-0.3.8/inngest/django.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/fast_api.py` & `inngest-0.3.8/inngest/fast_api.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/flask.py` & `inngest-0.3.8/inngest/flask.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest/tornado.py` & `inngest-0.3.8/inngest/tornado.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/inngest.egg-info/PKG-INFO` & `inngest-0.3.8/inngest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inngest
-Version: 0.3.7a0
+Version: 0.3.8
 Summary: Python SDK for Inngest
 Project-URL: Homepage, https://github.com/inngest/inngest-py
 Project-URL: Bug Tracker, https://github.com/inngest/inngest-py/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: FastAPI
 Classifier: Framework :: Flask
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: inngest Version: 0.3.7a0 Summary: Python SDK for
+Metadata-Version: 2.1 Name: inngest Version: 0.3.8 Summary: Python SDK for
 Inngest Project-URL: Homepage, https://github.com/inngest/inngest-py Project-
 URL: Bug Tracker, https://github.com/inngest/inngest-py/issues Classifier:
 Development Status :: 4 - Beta Classifier: Framework :: Django Classifier:
 Framework :: FastAPI Classifier: Framework :: Flask Classifier: Intended
 Audience :: Developers Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
```

### Comparing `inngest-0.3.7a0/inngest.egg-info/SOURCES.txt` & `inngest-0.3.8/inngest.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 inngest/_internal/__init__.py
 inngest/_internal/client_lib.py
 inngest/_internal/client_lib_test.py
 inngest/_internal/comm.py
 inngest/_internal/comm_test.py
 inngest/_internal/const.py
 inngest/_internal/const_test.py
-inngest/_internal/env.py
+inngest/_internal/env_lib.py
 inngest/_internal/errors.py
 inngest/_internal/event_lib.py
 inngest/_internal/event_lib_test.py
 inngest/_internal/execution.py
 inngest/_internal/function.py
 inngest/_internal/function_config.py
 inngest/_internal/function_config_test.py
```

### Comparing `inngest-0.3.7a0/pyproject.toml` & `inngest-0.3.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "inngest"
-version = "0.3.7a0"
+version = "0.3.8"
 description = "Python SDK for Inngest"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Framework :: Django",
     "Framework :: FastAPI",
     "Framework :: Flask",
```

### Comparing `inngest-0.3.7a0/tests/test_client.py` & `inngest-0.3.8/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/tests/test_django.py` & `inngest-0.3.8/tests/test_django.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/tests/test_fast_api.py` & `inngest-0.3.8/tests/test_fast_api.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/tests/test_flask.py` & `inngest-0.3.8/tests/test_flask.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import json
 import typing
 import unittest
 
 import flask
 import flask.logging
 import flask.testing
+import pytest
 
 import inngest
 import inngest.flask
-from inngest._internal import const
+from inngest._internal import const, errors
 
 from . import base, cases, dev_server, http_proxy, net
 
 _framework = "flask"
 _dev_server_origin = f"http://{net.HOST}:{dev_server.PORT}"
 
 _client = inngest.Inngest(
@@ -28,15 +29,15 @@
 for case in _cases:
     if isinstance(case.fn, list):
         _fns.extend(case.fn)
     else:
         _fns.append(case.fn)
 
 
-class TestFlask(unittest.TestCase):
+class TestFunctions(unittest.TestCase):
     app: flask.testing.FlaskClient
     client: inngest.Inngest
     dev_server_port: int
     proxy: http_proxy.Proxy
 
     @classmethod
     def setUpClass(cls) -> None:
@@ -79,15 +80,39 @@
             headers=dict(res.headers),
             status_code=res.status_code,
         )
 
 
 for case in _cases:
     test_name = f"test_{case.name}"
-    setattr(TestFlask, test_name, case.run_test)
+    setattr(TestFunctions, test_name, case.run_test)
+
+
+class TestServe(unittest.TestCase):
+    def test_cloud_mode_without_signing_key(self) -> None:
+        """
+        When in Cloud mode but no signing key, raise an error.
+
+        This test isn't needed for every framework since it's testing logic in
+        CommHandler
+        """
+
+        app = flask.Flask(__name__)
+        client = inngest.Inngest(app_id="client")
+
+        @client.create_function(
+            fn_id="fn",
+            trigger=inngest.TriggerEvent(event="event"),
+        )
+        def fn(ctx: inngest.Context, step: inngest.StepSync) -> None:
+            pass
+
+        with pytest.raises(Exception) as err:
+            inngest.flask.serve(app, client, [fn])
+        assert isinstance(err.value, errors.SigningKeyMissingError)
 
 
 class TestRegistration(unittest.TestCase):
     def test_sync_with_server_kind_mismatch(self) -> None:
         """Ensure that Dev Server cannot initiate a registration request when in
         production mode.
         """
```

### Comparing `inngest-0.3.7a0/tests/test_tornado.py` & `inngest-0.3.8/tests/test_tornado.py`

 * *Files identical despite different names*

### Comparing `inngest-0.3.7a0/tests/test_types.py` & `inngest-0.3.8/tests/test_types.py`

 * *Files identical despite different names*

