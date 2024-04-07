# Comparing `tmp/django-learngual-0.33.tar.gz` & `tmp/django-learngual-0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-learngual-0.33.tar", last modified: Wed Mar  6 00:18:31 2024, max compression
+gzip compressed data, was "django-learngual-0.34.tar", last modified: Sun Apr  7 01:33:46 2024, max compression
```

## Comparing `django-learngual-0.33.tar` & `django-learngual-0.34.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:31.641458 django-learngual-0.33/
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-06 00:17:39.000000 django-learngual-0.33/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-06 00:17:39.000000 django-learngual-0.33/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-06 00:18:31.641458 django-learngual-0.33/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-06 00:17:39.000000 django-learngual-0.33/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:31.641458 django-learngual-0.33/django_learngual.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-06 00:18:31.000000 django-learngual-0.33/django_learngual.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-06 00:18:31.000000 django-learngual-0.33/django_learngual.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 00:18:31.000000 django-learngual-0.33/django_learngual.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-06 00:18:31.000000 django-learngual-0.33/django_learngual.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:31.641458 django-learngual-0.33/learngual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:31.641458 django-learngual-0.33/learngual/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9882 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:31.641458 django-learngual-0.33/learngual/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/service_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:31.641458 django-learngual-0.33/learngual/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/tests/test_drf_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)    19895 2024-03-06 00:18:28.000000 django-learngual-0.33/learngual/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-06 00:18:31.645458 django-learngual-0.33/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 00:17:39.000000 django-learngual-0.33/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.216587 django-learngual-0.34/
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-04-07 01:32:59.000000 django-learngual-0.34/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-07 01:32:59.000000 django-learngual-0.34/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 01:33:46.216587 django-learngual-0.34/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-07 01:32:59.000000 django-learngual-0.34/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.216587 django-learngual-0.34/django_learngual.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 01:33:46.000000 django-learngual-0.34/django_learngual.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.212587 django-learngual-0.34/learngual/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.212587 django-learngual-0.34/learngual/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.212587 django-learngual-0.34/learngual/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/service_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:46.216587 django-learngual-0.34/learngual/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/test_drf_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6542 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20829 2024-04-07 01:33:43.000000 django-learngual-0.34/learngual/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 01:33:46.216587 django-learngual-0.34/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:32:59.000000 django-learngual-0.34/setup.py
```

### Comparing `django-learngual-0.33/LICENSE` & `django-learngual-0.34/LICENSE`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/PKG-INFO` & `django-learngual-0.34/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.33
+Version: 0.34
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.33/README.rst` & `django-learngual-0.34/README.rst`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/django_learngual.egg-info/PKG-INFO` & `django-learngual-0.34/django_learngual.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-learngual
-Version: 0.33
+Version: 0.34
 Summary: Learngual helper package
 Home-page: https://learngual.com
 Author: learngual
 Author-email: developer@leanrgual.com
 Maintainer: Aniekutmfon
 Maintainer-email: aniekutmfonekere@gmail.com
 License: Proprietary Software License Agreement
```

### Comparing `django-learngual-0.33/django_learngual.egg-info/SOURCES.txt` & `django-learngual-0.34/django_learngual.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 django_learngual.egg-info/top_level.txt
 learngual/__init__.py
 learngual/admin.py
 learngual/apps.py
 learngual/authentication.py
 learngual/enums.py
 learngual/manager.py
+learngual/middleware.py
 learngual/models.py
 learngual/permissions.py
 learngual/schema.py
 learngual/service_requests.py
 learngual/signals.py
 learngual/urls.py
 learngual/utils.py
```

### Comparing `django-learngual-0.33/learngual/apps.py` & `django-learngual-0.34/learngual/apps.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/authentication.py` & `django-learngual-0.34/learngual/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,20 +118,15 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.user_model = get_user_model()
 
     @classmethod
     def get_http_headers(cls, request: Request):
-
-        headers = dict()
-        if request:
-            for key, value in request.META.items():
-                if key.lower().startswith("http_"):
-                    headers[key.lower().lstrip("http_")] = value
+        headers = {key.lower(): value for key, value in request.headers.items()}
         return headers
 
     @classmethod
     def get_query_str(cls, request: Request):
         return "?{query}".format(query=request.META.get("QUERY_STRING", ""))
 
     def authenticate(self, request):
@@ -247,21 +242,19 @@
     @classmethod
     def get_query_str(cls, request: Request):
         return "?{query}".format(query=request.META.get("QUERY_STRING", ""))
 
     def authenticate(self, request):
         logger.info("authenticate() starting")
         header = self.get_header(request)
-        logger.info("header: %s", header)
 
         headers = self.get_http_headers(request)
-        logger.info("headers: %s", headers)
 
         account_or_user_id = headers.get("account")
-        logger.info("account_or_user_id: %s", account_or_user_id)
+        # logger.info("account_or_user_id: %s", account_or_user_id)
         account = None
         user = None
         if self.account_model:
             account = self.account_model.objects.filter(id=account_or_user_id).first()
             if account:
                 logger.info("account exist: %s", account)
                 user = getattr(account, "owner", None) or getattr(account, "user", None)
```

### Comparing `django-learngual-0.33/learngual/enums.py` & `django-learngual-0.34/learngual/enums.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/permissions.py` & `django-learngual-0.34/learngual/permissions.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/schema.py` & `django-learngual-0.34/learngual/schema.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/service_requests.py` & `django-learngual-0.34/learngual/service_requests.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/tests/request_mock.py` & `django-learngual-0.34/learngual/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/tests/test_authentication.py` & `django-learngual-0.34/learngual/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/tests/test_utils.py` & `django-learngual-0.34/learngual/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `django-learngual-0.33/learngual/utils.py` & `django-learngual-0.34/learngual/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import urllib.parse
 from collections import OrderedDict
 from logging import getLogger
 from typing import Any, Literal
 from urllib.parse import urlparse
 
+import pytz
 import requests
 from django.conf import settings
 from django.core.cache import cache
 from django.utils import timezone
 from faker import Faker
 
 faker = Faker()
@@ -26,14 +27,33 @@
     "learn": "http://host.docker.internal:8001",
     "payment": "http://host.docker.internal:8002",
     "notify": "http://host.docker.internal:8003",
     "media": "http://host.docker.internal:8004",
 }
 
 
+def transform_local_base_url(
+    base_url: str,
+    service: Literal["payment", "iam", "learn", "notify", "media"] = "iam",
+) -> str:
+    """check if baser_url is local url return the approprate url
+
+    Args:
+        base_url (str): _description_
+        service
+              _description_. Defaults to "iam".
+
+    Returns:
+        str: _description_
+    """
+    if not base_url.startswith("https://"):
+        return LOCAL_URLS.get(service, "iam")
+    return base_url
+
+
 def get_service_request_headers(**kwargs) -> dict:
     """function add headers needed for request made from a service
 
     Returns:
         dict: _description_
     """
     if LEARNGUAL_SERVICE_API_KEY:
@@ -621,7 +641,19 @@
 
     def has_response_status(self, response, status_code: int) -> bool:
         return response.status_code == status_code
 
     def add_query_params_to_url(self, url: str, params: dict[str, Any]) -> str:
         query_string = urllib.parse.urlencode(params)
         return f"{url}?{query_string}"
+
+
+def get_timezone_from_country(country_code) -> str:
+    try:
+        country_timezones = pytz.country_timezones.get(country_code.upper())
+        if country_timezones:
+            # Assuming the first timezone for simplicity
+            return pytz.timezone(country_timezones[0])
+        else:
+            return None  # Country code not found or no timezone information available
+    except KeyError:
+        return None  # Invalid country code
```

### Comparing `django-learngual-0.33/setup.cfg` & `django-learngual-0.34/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-learngual
-version = 0.33
+version = 0.34
 author = learngual
 author_email = developer@leanrgual.com
 maintainer = Aniekutmfon
 maintainer_email = aniekutmfonekere@gmail.com
 description = Learngual helper package
 long_description = file:README.rst
 long_description_content_type = text/x-rst
```

