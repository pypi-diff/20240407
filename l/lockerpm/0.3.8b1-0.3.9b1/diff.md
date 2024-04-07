# Comparing `tmp/lockerpm-0.3.8b1.tar.gz` & `tmp/lockerpm-0.3.9b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lockerpm-0.3.8b1.tar", last modified: Mon Feb 19 05:00:15 2024, max compression
+gzip compressed data, was "lockerpm-0.3.9b1.tar", last modified: Tue Feb 27 07:15:17 2024, max compression
```

## Comparing `lockerpm-0.3.8b1.tar` & `lockerpm-0.3.9b1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 05:00:15.860779 lockerpm-0.3.8b1/
--rw-rw-r--   0 root         (0) root         (0)      288 2023-11-21 08:47:01.000000 lockerpm-0.3.8b1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10888 2024-02-19 05:00:15.860779 lockerpm-0.3.8b1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     9914 2024-02-19 04:59:40.000000 lockerpm-0.3.8b1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 05:00:15.852779 lockerpm-0.3.8b1/docs/
--rw-rw-r--   0 root         (0) root         (0)     1578 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/docs/standard.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 05:00:15.856778 lockerpm-0.3.8b1/locker/
--rw-rw-r--   0 root         (0) root         (0)      162 2024-02-19 04:59:40.000000 lockerpm-0.3.8b1/locker/__about__.json
--rw-rw-r--   0 root         (0) root         (0)      228 2024-02-19 04:59:40.000000 lockerpm-0.3.8b1/locker/__about__.py
--rw-rw-r--   0 root         (0) root         (0)     2425 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/locker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10311 2024-02-15 10:58:31.000000 lockerpm-0.3.8b1/locker/binary_adapter.py
--rw-rw-r--   0 root         (0) root         (0)     6291 2024-02-15 10:26:50.000000 lockerpm-0.3.8b1/locker/client.py
--rw-rw-r--   0 root         (0) root         (0)     4313 2024-02-19 04:59:40.000000 lockerpm-0.3.8b1/locker/error.py
--rw-rw-r--   0 root         (0) root         (0)     1931 2023-12-06 07:39:00.000000 lockerpm-0.3.8b1/locker/logger.py
--rw-rw-r--   0 root         (0) root         (0)    13121 2024-02-08 15:53:14.000000 lockerpm-0.3.8b1/locker/ls_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 05:00:15.856778 lockerpm-0.3.8b1/locker/ls_resources/
--rw-rw-r--   0 root         (0) root         (0)      251 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/locker/ls_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 05:00:15.856778 lockerpm-0.3.8b1/locker/ls_resources/abstract/
--rw-rw-r--   0 root         (0) root         (0)      701 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5130 2024-02-08 15:53:14.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      543 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/createable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      644 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/deletable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      354 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/detailable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      690 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/listable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      826 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/singleton_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)      456 2023-12-05 08:56:19.000000 lockerpm-0.3.8b1/locker/ls_resources/abstract/updateable_api_resource.py
--rw-rw-r--   0 root         (0) root         (0)     2548 2024-02-15 10:26:50.000000 lockerpm-0.3.8b1/locker/ls_resources/environment.py
--rw-rw-r--   0 root         (0) root         (0)     1274 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/locker/ls_resources/error_object.py
--rw-rw-r--   0 root         (0) root         (0)     3023 2024-02-15 10:26:50.000000 lockerpm-0.3.8b1/locker/ls_resources/secret.py
--rw-rw-r--   0 root         (0) root         (0)      909 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/locker/ls_response.py
--rw-rw-r--   0 root         (0) root         (0)      422 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/locker/object_classes.py
--rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/locker/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 05:00:15.856778 lockerpm-0.3.8b1/lockerpm.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10888 2024-02-19 05:00:15.000000 lockerpm-0.3.8b1/lockerpm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1176 2024-02-19 05:00:15.000000 lockerpm-0.3.8b1/lockerpm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-19 05:00:15.000000 lockerpm-0.3.8b1/lockerpm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-19 05:00:15.000000 lockerpm-0.3.8b1/lockerpm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-02-19 05:00:15.000000 lockerpm-0.3.8b1/lockerpm.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      108 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)       38 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/requirements-dev.txt
--rw-rw-r--   0 root         (0) root         (0)       39 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/requirements-test.txt
--rw-rw-r--   0 root         (0) root         (0)       28 2023-11-28 06:52:28.000000 lockerpm-0.3.8b1/requirements.txt
--rw-rw-r--   0 root         (0) root         (0)       61 2024-02-19 05:00:15.860779 lockerpm-0.3.8b1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-23 08:02:16.000000 lockerpm-0.3.8b1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-19 05:00:15.860779 lockerpm-0.3.8b1/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/tests/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1377 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/tests/test_binary_adapter.py
--rw-rw-r--   0 root         (0) root         (0)     2636 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/tests/test_client.py
--rw-rw-r--   0 root         (0) root         (0)      547 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/tests/test_logger.py
--rw-rw-r--   0 root         (0) root         (0)     2788 2024-01-22 10:32:54.000000 lockerpm-0.3.8b1/tests/test_util.py
--rw-rw-r--   0 root         (0) root         (0)     1219 2023-09-20 11:33:43.000000 lockerpm-0.3.8b1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/
+-rw-rw-r--   0 root         (0) root         (0)      288 2023-11-21 08:47:01.000000 lockerpm-0.3.9b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10888 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     9914 2024-02-19 04:59:40.000000 lockerpm-0.3.9b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.357288 lockerpm-0.3.9b1/docs/
+-rw-rw-r--   0 root         (0) root         (0)     1578 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/docs/standard.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/locker/
+-rw-rw-r--   0 root         (0) root         (0)      162 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/__about__.json
+-rw-rw-r--   0 root         (0) root         (0)      228 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/__about__.py
+-rw-rw-r--   0 root         (0) root         (0)     2425 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10317 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/binary_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     6291 2024-02-15 10:26:50.000000 lockerpm-0.3.9b1/locker/client.py
+-rw-rw-r--   0 root         (0) root         (0)     4313 2024-02-19 04:59:40.000000 lockerpm-0.3.9b1/locker/error.py
+-rw-rw-r--   0 root         (0) root         (0)     1931 2023-12-06 07:39:00.000000 lockerpm-0.3.9b1/locker/logger.py
+-rw-rw-r--   0 root         (0) root         (0)    13121 2024-02-08 15:53:14.000000 lockerpm-0.3.9b1/locker/ls_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/locker/ls_resources/
+-rw-rw-r--   0 root         (0) root         (0)      251 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/locker/ls_resources/abstract/
+-rw-rw-r--   0 root         (0) root         (0)      701 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5130 2024-02-08 15:53:14.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      543 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/createable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      644 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/deletable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      354 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/detailable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      690 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/listable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      826 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/singleton_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)      456 2023-12-05 08:56:19.000000 lockerpm-0.3.9b1/locker/ls_resources/abstract/updateable_api_resource.py
+-rw-rw-r--   0 root         (0) root         (0)     2548 2024-02-15 10:26:50.000000 lockerpm-0.3.9b1/locker/ls_resources/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     1274 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/ls_resources/error_object.py
+-rw-rw-r--   0 root         (0) root         (0)     2965 2024-02-27 07:14:42.000000 lockerpm-0.3.9b1/locker/ls_resources/secret.py
+-rw-rw-r--   0 root         (0) root         (0)      909 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/ls_response.py
+-rw-rw-r--   0 root         (0) root         (0)      422 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/locker/object_classes.py
+-rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/locker/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.361288 lockerpm-0.3.9b1/lockerpm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10888 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1176 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-02-27 07:15:17.000000 lockerpm-0.3.9b1/lockerpm.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      108 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/requirements-dev.txt
+-rw-rw-r--   0 root         (0) root         (0)       39 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/requirements-test.txt
+-rw-rw-r--   0 root         (0) root         (0)       28 2023-11-28 06:52:28.000000 lockerpm-0.3.9b1/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       61 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     4166 2024-01-23 08:02:16.000000 lockerpm-0.3.9b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 07:15:17.365288 lockerpm-0.3.9b1/tests/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/tests/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1377 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/tests/test_binary_adapter.py
+-rw-rw-r--   0 root         (0) root         (0)     2636 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/tests/test_client.py
+-rw-rw-r--   0 root         (0) root         (0)      547 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/tests/test_logger.py
+-rw-rw-r--   0 root         (0) root         (0)     2788 2024-01-22 10:32:54.000000 lockerpm-0.3.9b1/tests/test_util.py
+-rw-rw-r--   0 root         (0) root         (0)     1219 2023-09-20 11:33:43.000000 lockerpm-0.3.9b1/tox.ini
```

### Comparing `lockerpm-0.3.8b1/PKG-INFO` & `lockerpm-0.3.9b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockerpm
-Version: 0.3.8b1
+Version: 0.3.9b1
 Summary: Locker Secret Python SDK
 Home-page: https://locker.io
 Download-URL: 
 Author: CyStack
 Author-email: contact@locker.io
 Keywords: django,vault management,security
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lockerpm-0.3.8b1/README.md` & `lockerpm-0.3.9b1/README.md`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/docs/standard.md` & `lockerpm-0.3.9b1/docs/standard.md`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/__init__.py` & `lockerpm-0.3.9b1/locker/__init__.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/binary_adapter.py` & `lockerpm-0.3.9b1/locker/binary_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -192,18 +192,18 @@
             return res_body.get("object") == "error" or res_body.get("success") is False or\
                 res_body.get("success") == "false"
         except AttributeError:
             return False
 
     def handle_error_response(self, res_body):
         exc = self.specific_cli_error(error_data=res_body)
+        self.logger.warning(f"[!] CLI return error object:::{exc.http_body}")
         raise exc
 
     def specific_cli_error(self, error_data):
-        self.logger.info(f"[!] CLI return error object:::{error_data}")
         status_code = error_data.get("status_code")
         error_code = error_data.get("error")
         if status_code == 429 or error_code == "rate_limit":
             return error.RateLimitError(
                 error_data.get("message"),
                 http_body=error_data,
                 http_status=429,
```

### Comparing `lockerpm-0.3.8b1/locker/client.py` & `lockerpm-0.3.9b1/locker/client.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/error.py` & `lockerpm-0.3.9b1/locker/error.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/logger.py` & `lockerpm-0.3.9b1/locker/logger.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_object.py` & `lockerpm-0.3.9b1/locker/ls_object.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/abstract/__init__.py` & `lockerpm-0.3.9b1/locker/ls_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/abstract/api_resource.py` & `lockerpm-0.3.9b1/locker/ls_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/abstract/createable_api_resource.py` & `lockerpm-0.3.9b1/locker/ls_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/abstract/deletable_api_resource.py` & `lockerpm-0.3.9b1/locker/ls_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/abstract/listable_api_resource.py` & `lockerpm-0.3.9b1/locker/ls_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/abstract/singleton_api_resource.py` & `lockerpm-0.3.9b1/locker/ls_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/environment.py` & `lockerpm-0.3.9b1/locker/ls_resources/environment.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/error_object.py` & `lockerpm-0.3.9b1/locker/ls_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/ls_resources/secret.py` & `lockerpm-0.3.9b1/locker/ls_resources/secret.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from __future__ import absolute_import, division, print_function
 
-import logging
-
-from six.moves.urllib.parse import quote_plus
 
 from locker.error import CliRunError
 from locker.ls_resources.abstract import ListableAPIResource, CreateableAPIResource, UpdateableAPIResource, \
     DeletableAPIResource
 
 
 class Secret(ListableAPIResource, CreateableAPIResource, UpdateableAPIResource, DeletableAPIResource):
@@ -22,19 +19,19 @@
         instance = cls(None, access_key_id, secret_access_key, **params)
         try:
             instance._call_and_refresh(
                 cli_, access_key_id=access_key_id, secret_access_key=secret_access_key,
                 api_base=api_base, api_version=api_version, params=params
             )
         except CliRunError as e:
-            logging.debug(f"[!] CliRunError when get_secret of {key}. So return default value is {default_value}\n"
-                          f"Traceback: {e} - {e.user_message} ")
+            # logging.warning(f"[!] CliRunError when get_secret of {key}. So return default value is {default_value}\n"
+            #                 f"Error: {e.code} - {e.user_message} ")
             return default_value
         try:
-            return instance.data.value
+            return instance.value
         except AttributeError:
             return default_value
 
     @classmethod
     def retrieve_secret(cls, key, environment_name=None,
                         access_key_id=None, secret_access_key=None, api_base=None, api_version=None, **params):
         base = cls.class_cli()
```

### Comparing `lockerpm-0.3.8b1/locker/ls_response.py` & `lockerpm-0.3.9b1/locker/ls_response.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/locker/util.py` & `lockerpm-0.3.9b1/locker/util.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/lockerpm.egg-info/PKG-INFO` & `lockerpm-0.3.9b1/lockerpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lockerpm
-Version: 0.3.8b1
+Version: 0.3.9b1
 Summary: Locker Secret Python SDK
 Home-page: https://locker.io
 Download-URL: 
 Author: CyStack
 Author-email: contact@locker.io
 Keywords: django,vault management,security
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lockerpm-0.3.8b1/lockerpm.egg-info/SOURCES.txt` & `lockerpm-0.3.9b1/lockerpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/setup.py` & `lockerpm-0.3.9b1/setup.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/tests/test_binary_adapter.py` & `lockerpm-0.3.9b1/tests/test_binary_adapter.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/tests/test_client.py` & `lockerpm-0.3.9b1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/tests/test_logger.py` & `lockerpm-0.3.9b1/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/tests/test_util.py` & `lockerpm-0.3.9b1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `lockerpm-0.3.8b1/tox.ini` & `lockerpm-0.3.9b1/tox.ini`

 * *Files identical despite different names*

