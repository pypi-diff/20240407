# Comparing `tmp/django-learngual-0.34.tar.gz` & `tmp/django-learngual-0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.34.tar", last modified: Sun Apr  7 01:33:46 2024, max compression
+gzip compressed data, was "django-learngual-0.36.tar", last modified: Sun Apr  7 10:38:11 2024, max compression
```

## Comparing `django-learngual-0.34.tar` & `django-learngual-0.36.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.216587 django-learngual-0.34/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-07 01:32:59.000000 django-learngual-0.34/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-07 01:32:59.000000 django-learngual-0.34/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 01:33:46.216587 django-learngual-0.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-07 01:32:59.000000 django-learngual-0.34/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.216587 django-learngual-0.34/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.212587 django-learngual-0.34/learngual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.212587 django-learngual-0.34/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.212587 django-learngual-0.34/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/service_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.216587 django-learngual-0.34/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    20829 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 01:33:46.216587 django-learngual-0.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:32:59.000000 django-learngual-0.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:11.931309 django-learngual-0.36/
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-07 10:37:26.000000 django-learngual-0.36/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-07 10:37:26.000000 django-learngual-0.36/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 10:38:11.931309 django-learngual-0.36/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-07 10:37:26.000000 django-learngual-0.36/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:11.931309 django-learngual-0.36/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 10:38:11.000000 django-learngual-0.36/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-07 10:38:11.000000 django-learngual-0.36/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:38:11.000000 django-learngual-0.36/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 10:38:11.000000 django-learngual-0.36/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:11.931309 django-learngual-0.36/learngual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:11.931309 django-learngual-0.36/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9826 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:11.931309 django-learngual-0.36/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/service_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:11.931309 django-learngual-0.36/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20829 2024-04-07 10:38:09.000000 django-learngual-0.36/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 10:38:11.935309 django-learngual-0.36/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:37:26.000000 django-learngual-0.36/setup.py
```

### Comparing `django-learngual-0.34/LICENSE` & `django-learngual-0.36/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/PKG-INFO` & `django-learngual-0.36/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.34
+Version: 0.36
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.34/README.rst` & `django-learngual-0.36/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.36/django_learngual.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.34
+Version: 0.36
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.34/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.36/django_learngual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/apps.py` & `django-learngual-0.36/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/authentication.py` & `django-learngual-0.36/learngual/authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,19 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.user_model = get_user_model()
 
     @classmethod
     def get_http_headers(cls, request: Request):
-        headers = {key.lower(): value for key, value in request.headers.items()}
+        headers = {
+            key.lower(): value
+            for key, value in request.headers.items()
+            if isinstance(value, (int, str, float))
+        }
         return headers
 
     @classmethod
     def get_query_str(cls, request: Request):
         return "?{query}".format(query=request.META.get("QUERY_STRING", ""))
 
     def authenticate(self, request):
@@ -152,25 +156,26 @@
             "retrieve required authentication header during authentication -> %s",
             header,
         )
         if not header.get("authorization"):
             logger.warn("no authorization")
             return None
         headers = self.get_http_headers(request)
-        logger.info("get django request header for forwarding -> ", headers)
+        logger.info("get django request header for forwarding -> %s", headers)
 
         query_str = self.get_query_str(request)
         logger.info("query string for forwarding -> %s", query_str)
         logger.info(f"{LEARNGUAL_AUTH_RETRIEVE_URL =}")
         res = requests.get(LEARNGUAL_AUTH_RETRIEVE_URL + query_str, headers=headers)
         if not res.ok:
             logging.warn("request to IAM service did not go through")
             return None
+        logging.info("verify auth response data -> %s", res.content)
         res_data = res.json()
-        logging.info("verify auth response data -> %s", res_data)
+        logging.info("verify auth response json data -> %s", res_data)
         return (
             get_user(res_data),
             header.get("api_key") or header.get("authorization").split(" ")[-1],
         )
 
     def get_header(self, request):
         """
```

### Comparing `django-learngual-0.34/learngual/enums.py` & `django-learngual-0.36/learngual/enums.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/middleware.py` & `django-learngual-0.36/learngual/middleware.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/permissions.py` & `django-learngual-0.36/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/schema.py` & `django-learngual-0.36/learngual/schema.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/service_requests.py` & `django-learngual-0.36/learngual/service_requests.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/tests/request_mock.py` & `django-learngual-0.36/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/tests/test_authentication.py` & `django-learngual-0.36/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/tests/test_utils.py` & `django-learngual-0.36/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/learngual/utils.py` & `django-learngual-0.36/learngual/utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.34/setup.cfg` & `django-learngual-0.36/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.34
+version = 0.36
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

