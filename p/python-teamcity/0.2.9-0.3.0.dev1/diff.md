# Comparing `tmp/python-teamcity-0.2.9.tar.gz` & `tmp/python-teamcity-0.3.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-teamcity-0.2.9.tar", last modified: Wed Apr  3 11:54:30 2024, max compression
+gzip compressed data, was "python-teamcity-0.3.0.dev1.tar", last modified: Sun Apr  7 16:21:26 2024, max compression
```

## Comparing `python-teamcity-0.2.9.tar` & `python-teamcity-0.3.0.dev1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.889756 python-teamcity-0.2.9/
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.878920 python-teamcity-0.2.9/.github/
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.882324 python-teamcity-0.2.9/.github/workflows/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     2778 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/.github/workflows/codeql.yml
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      104 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/AUTHORS
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1617 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/ChangeLog
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1072 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/LICENSE
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1091 2024-04-03 11:54:30.889580 python-teamcity-0.2.9/PKG-INFO
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       65 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/README.md
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.884129 python-teamcity-0.2.9/examples/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/examples/__init__.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_auth.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_build.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1034 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_const.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     3194 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/examples/example_test.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.889126 python-teamcity-0.2.9/python_teamcity.egg-info/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1091 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/PKG-INFO
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      576 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/SOURCES.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/dependency_links.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-03-14 09:27:40.000000 python-teamcity-0.2.9/python_teamcity.egg-info/not-zip-safe
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       47 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/pbr.json
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/requires.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-03 11:54:30.000000 python-teamcity-0.2.9/python_teamcity.egg-info/top_level.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        8 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/requirements.txt
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      900 2024-04-03 11:54:30.890151 python-teamcity-0.2.9/setup.cfg
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      128 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/setup.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.888247 python-teamcity-0.2.9/teamcity/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       31 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/teamcity/__init__.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)    22108 2024-04-03 11:54:17.000000 python-teamcity-0.2.9/teamcity/teamcity.py
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      225 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/teamcity/teamcity_const.py
-drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:30.888717 python-teamcity-0.2.9/tests/
--rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.2.9/tests/__init__.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.737389 python-teamcity-0.3.0.dev1/
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.726424 python-teamcity-0.3.0.dev1/.github/
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.729466 python-teamcity-0.3.0.dev1/.github/workflows/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     2778 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/.github/workflows/codeql.yml
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      104 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/AUTHORS
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1693 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/ChangeLog
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1072 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/LICENSE
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1096 2024-04-07 16:21:26.737206 python-teamcity-0.3.0.dev1/PKG-INFO
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       65 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/README.md
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.731741 python-teamcity-0.3.0.dev1/examples/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/examples/__init__.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_auth.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_build.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      479 2024-04-07 16:13:56.000000 python-teamcity-0.3.0.dev1/examples/example_change.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1034 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_const.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     3194 2024-04-03 11:54:17.000000 python-teamcity-0.3.0.dev1/examples/example_test.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.736752 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)     1096 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/PKG-INFO
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      603 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/SOURCES.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/dependency_links.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        1 2024-03-14 09:27:40.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/not-zip-safe
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       47 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/pbr.json
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/requires.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        9 2024-04-07 16:21:26.000000 python-teamcity-0.3.0.dev1/python_teamcity.egg-info/top_level.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        8 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/requirements.txt
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      900 2024-04-07 16:21:26.737750 python-teamcity-0.3.0.dev1/setup.cfg
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      128 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/setup.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.735818 python-teamcity-0.3.0.dev1/teamcity/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)       31 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/teamcity/__init__.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)    27124 2024-04-07 16:17:59.000000 python-teamcity-0.3.0.dev1/teamcity/teamcity.py
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)      449 2024-04-04 09:43:54.000000 python-teamcity-0.3.0.dev1/teamcity/teamcity_const.py
+drwxr-xr-x   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-04-07 16:21:26.736414 python-teamcity-0.3.0.dev1/tests/
+-rw-r--r--   0 yunlin.tan (2073411975) MIHOYO\Domain Users (623285134)        0 2024-03-09 11:42:19.000000 python-teamcity-0.3.0.dev1/tests/__init__.py
```

### Comparing `python-teamcity-0.2.9/.github/workflows/codeql.yml` & `python-teamcity-0.3.0.dev1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.2.9/ChangeLog` & `python-teamcity-0.3.0.dev1/ChangeLog`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 CHANGES
 =======
 
+* Add support for fetching build queue changes and refactor authentication
+
 v0.2.9
 ------
 
 * Support to get latest build detail by build type id
 
 v0.2.8
 ------
```

### Comparing `python-teamcity-0.2.9/LICENSE` & `python-teamcity-0.3.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.2.9/PKG-INFO` & `python-teamcity-0.3.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.2.9
+Version: 0.3.0.dev1
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `python-teamcity-0.2.9/examples/example_const.py` & `python-teamcity-0.3.0.dev1/examples/example_const.py`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.2.9/examples/example_test.py` & `python-teamcity-0.3.0.dev1/examples/example_test.py`

 * *Files identical despite different names*

### Comparing `python-teamcity-0.2.9/python_teamcity.egg-info/PKG-INFO` & `python-teamcity-0.3.0.dev1/python_teamcity.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-teamcity
-Version: 0.2.9
+Version: 0.3.0.dev1
 Summary: Python library for triggering TeamCity by REST API
 Home-page: https://github.com/norbread2003/python-teamcity
 Author: Yunlin Tan
 Author-email: tanyunlin2003@norbread.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `python-teamcity-0.2.9/python_teamcity.egg-info/SOURCES.txt` & `python-teamcity-0.3.0.dev1/python_teamcity.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/codeql.yml
 examples/__init__.py
 examples/example_auth.py
 examples/example_build.py
+examples/example_change.py
 examples/example_const.py
 examples/example_test.py
 python_teamcity.egg-info/PKG-INFO
 python_teamcity.egg-info/SOURCES.txt
 python_teamcity.egg-info/dependency_links.txt
 python_teamcity.egg-info/not-zip-safe
 python_teamcity.egg-info/pbr.json
```

### Comparing `python-teamcity-0.2.9/setup.cfg` & `python-teamcity-0.3.0.dev1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python-teamcity
-version = 0.2.9
+version = 0.3.0
 author = Yunlin Tan
 author_email = tanyunlin2003@norbread.com
 summary = Python library for triggering TeamCity by REST API
 description_file = README.md
 license = MIT
 home_page = https://github.com/norbread2003/python-teamcity
 classifier =
```

### Comparing `python-teamcity-0.2.9/teamcity/teamcity.py` & `python-teamcity-0.3.0.dev1/teamcity/teamcity.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 @brief Python API for triggering TeamCity by REST API.
 
 @author Yunlin Tan
 
 @date 11/22/2022
 
 **Related Page**: https://github.com/norbread2003/python-teamcity
+**Reference Page**: https://www.jetbrains.com/help/teamcity/rest/teamcity-rest-api-documentation.html
 
 Arguments
 ---------
     - None
 
 Example Usage
 -------------
@@ -35,29 +36,30 @@
 0.2.0        11/13/2023   Yunlin Tan([None])            Change packing method.
 0.2.1        1/23/2024    Yunlin Tan([None])            Add agent-related functions.
 0.2.1        1/23/2024    Yunlin Tan([None])            Support to get agent details.
 0.2.3        2/1/2024     Yunlin Tan([None])            Support to get all agents (including unauthorized).
 0.2.4        3/4/2024     Yunlin Tan([None])            Support to get actual build parameters by resulting-properties.
 0.2.5        3/13/2024    Yunlin Tan([None])            Add more functions to get builds.
 0.2.9        4/3/2024     Yunlin Tan([None])            Support to get latest build detail by build type id.
+0.3.0        4/8/2024     Yunlin Tan([None])            Support to get build queue changes.
 
 Depends On
 ----------
 **Python Dependencies:**
     - requests
 
 **Other Dependencies:**
     - None
 """
 import logging
 import os
 
 import requests
 
-from teamcity.teamcity_const import AUTH_METHOD
+from teamcity.teamcity_const import AuthMethod, RequestMethod, RequestReturnType
 
 
 class TeamCity:
     def __init__(self, server=None, tokens=None, user=None, password=None, guest=False):
         self.server = self.process_server_address(server or os.environ.get('TEAMCITY_SERVER', None))
         self.tokens = tokens or os.environ.get('TEAMCITY_TOKENS', None)
         self.user = user or os.environ.get('TEAMCITY_USER', None)
@@ -77,82 +79,89 @@
 
     def check_auth_method(self):
         """Check authentication method and return related info."""
 
         header = {'Accept': 'application/json'}
         if self.tokens:
             logging.info(f'Logging in TeamCity with tokens.')
-            authentication_method = AUTH_METHOD.TOKENS
+            authentication_method = AuthMethod.TOKENS
             base_url = f'{self.server}/app/rest'
             header.update({'Authorization': f'Bearer {self.tokens}'})
         elif self.user and self.password:
             logging.info(f'Logging TeamCity with user: {self.user}')
-            authentication_method = AUTH_METHOD.USER
+            authentication_method = AuthMethod.USER
             base_url = f'{self.server}/httpAuth/app/rest'
         elif self.guest:  # Guest login
             logging.info(f'Logging TeamCity as guest.')
-            authentication_method = AUTH_METHOD.GUEST
+            authentication_method = AuthMethod.GUEST
             base_url = f'{self.server}/guestAuth/app/rest'
         else:  # No authentication
             logging.warning('No authentication method provided, assume you are logged in to TeamCity in the browser.')
             logging.warning('If you are not logged in, you will get 401 Unauthorized error.')
-            authentication_method = AUTH_METHOD.LOGGED_IN
+            authentication_method = AuthMethod.LOGGED_IN
             base_url = f'{self.server}/app/rest'
         return authentication_method, base_url, header
 
-    def request_base(self, url, method, extra_headers={}, data=None, json=None, timeout=None, retries=3):
+    def request_base(self, url, method, extra_headers=None, data=None, json=None, timeout=None, retries=3):
         url, headers = f'{self.base_url}/{url}', self.header
+        extra_headers = {} if extra_headers is None else extra_headers
         headers.update(extra_headers)
         session = requests.Session()
         logging.info(f'Calling TeamCity API: {url}')
 
+        response = None
         while retries > 0:
             try:
-                if self.authentication_method in [AUTH_METHOD.TOKENS, AUTH_METHOD.GUEST]:
+                if self.authentication_method in [AuthMethod.TOKENS, AuthMethod.GUEST]:
                     response = session.request(method, url, headers=headers, data=data, json=json, timeout=timeout)
-                elif self.authentication_method == AUTH_METHOD.USER:
+                elif self.authentication_method == AuthMethod.USER:
                     response = session.request(method, url, auth=(self.user, self.password), headers=headers,
                                                data=data, json=json, timeout=timeout)
-                elif self.authentication_method == AUTH_METHOD.LOGGED_IN:
+                elif self.authentication_method == AuthMethod.LOGGED_IN:
                     logging.error('You are not logged in to TeamCity, POST method is not supported.')
                     raise ValueError('You are not logged in to TeamCity, POST method is not supported.')
                 else:
                     logging.error('Unknown authentication method.')
                     raise ValueError('Unknown authentication method.')
 
             except Exception as e:
                 logging.error(f'Failed to {method.lower()} request to TeamCity: {e}, retries left: {retries}')
 
             if response is None or response.status_code != 200:
-                logging.error(
-                    f'Failed to {method.lower()} request to TeamCity: {response.status_code}, retries left: {retries}')
+                return_code = response.status_code if response is not None else 'NA'
+                logging.error(f'Failed to {method.lower()} request to TeamCity: {return_code}, retries left: {retries}')
             else:
                 return response
 
             retries -= 1
         else:
-            logging.error(f'No retries left, failed to {method.lower()} request to TeamCity: {response.status_code}')
-            raise ValueError(f'No retries left, failed to {method.lower()} request to TeamCity: {response.status_code}')
+            return_code = response.status_code if response is not None else 'NA'
+            logging.error(f'No retries left, failed to {method.lower()} request to TeamCity: {return_code}')
+            raise ValueError(f'No retries left, failed to {method.lower()} request to TeamCity: {return_code}')
 
-    def post_request(self, url, extra_headers={}, data=None, json=None, timeout=None, retries=3):
+    def post_request(self, url, extra_headers=None, data=None, json=None, timeout=None, retries=3):
+        extra_headers = {} if extra_headers is None else extra_headers
         extra_headers.update({'Content-Type': 'application/json'})
         return self.request_base(url=url, method='POST', extra_headers=extra_headers, data=data, json=json,
                                  timeout=timeout, retries=retries)
 
-    def get_request(self, url, extra_headers={}, data=None, json=None, timeout=None, retries=3):
+    def get_request(self, url, extra_headers=None, data=None, json=None, timeout=None, retries=3):
+        extra_headers = {} if extra_headers is None else extra_headers
         extra_headers.update({'Accept': 'application/json'})
         return self.request_base(url=url, method='GET', extra_headers=extra_headers, data=data, json=json,
                                  timeout=timeout, retries=retries).json()
 
-    def get_string_request(self, url, extra_headers={}, data=None, json=None, timeout=None, retries=3):
+    def get_string_request(self, url, extra_headers=None, data=None, json=None, timeout=None, retries=3):
+        extra_headers = {} if extra_headers is None else extra_headers
         extra_headers.update({'Accept': 'text/plain'})
         return self.request_base(url=url, method='GET', extra_headers=extra_headers, data=data, json=json,
                                  timeout=timeout, retries=retries).text
 
-    def get_file_request(self, url, extra_headers={}, data=None, json=None, timeout=None, retries=3):
+    def get_file_request(self, url, extra_headers=None, data=None, json=None, timeout=None, retries=3):
+        extra_headers = {} if extra_headers is None else extra_headers
         extra_headers.update({'Accept': 'application/json'})
         return self.request_base(url=url, method='GET', extra_headers=extra_headers, data=data, json=json,
                                  timeout=timeout, retries=retries).text
 
     def get_all_builds(self, build_type_id='', details=False, count=10000):
         """Get builds from TeamCity.
 
@@ -267,37 +276,93 @@
         try:
             return self.get_request(url)
         except Exception as ex:
             logging.error(ex)
             logging.error(f'Failed to get build {build_id} canceled info.')
             return dict()
 
+    # def build_api_base(self, url, method, return_type=None, build_id='', locator=''):
+    #     return_type = RequestReturnType.NONE if method == RequestMethod.POST else return_type
+    #     try:
+    #         if type(method) is str and method.upper() not in [RequestMethod.GET, RequestMethod.POST]:
+    #             raise ValueError(f'Invalid method {method}. Only GET, POST are supported.')
+    #         if type(return_type) is str and method.lower() not in [RequestReturnType.JSON, RequestReturnType.TEXT,
+    #                                                                RequestReturnType.FILE]:
+    #             raise ValueError(f'Invalid return type {return_type}. Only JSON, TEXT, FILE are supported.')
+    #         if url == '':
+    #             raise ValueError('Please provide a valid url.')
+    #         if build_id != '' and locator == '':
+    #             raise ValueError('Please provide a valid build_id or locator.')
+    #
+    #         if build_id != '' and locator != '':  # TODO(yunlin): Need to fix this issue.
+    #             url = url.replace('{{buildLocator}}', locator)
+    #         elif build_id != '':
+    #             url = url.replace('{{buildLocator}}', f'id:{build_id}')
+    #         elif locator != '':
+    #             url = url.replace('{{buildLocator}}', locator)
+    #
+    #         if method.upper() == RequestMethod.GET:
+    #             if return_type == RequestReturnType.JSON:
+    #                 return self.get_request(url)
+    #             elif return_type == RequestReturnType.TEXT:
+    #                 return self.get_string_request(url)
+    #             elif return_type == RequestReturnType.FILE:
+    #                 return self.get_file_request(url)
+    #             else:
+    #                 return None
+    #         elif method.upper() == RequestMethod.POST:
+    #             return self.post_request(url)
+    #     except Exception as ex:
+    #         logging.error(ex)
+    #         if return_type == RequestReturnType.JSON:
+    #             return dict()
+    #         elif return_type == RequestReturnType.TEXT or return_type == RequestReturnType.FILE:
+    #             return ''
+    #         elif return_type == RequestReturnType.NONE:
+    #             return False
+    #         else:
+    #             return None
+    #
+    # def get_aggregated_build_status(self, build_id='', locator=''):
+    #     """Get the build status of aggregated matching builds.
+    #
+    #     :param build_id: TeamCity build id.
+    #     :param locator: TeamCity build locator, should be provided if build id is not available.
+    #                     If both parameters are provided, both will be used.
+    #
+    #     :return:
+    #     """
+    #     url = f'/app/rest/builds/aggregated/{{buildLocator}}/status'
+
     def get_build_actual_parameters(self, build_id, property_name=''):
         """Get actual build parameters of the matching build by resulting-properties from TeamCity.
 
+        Reference Page: https://www.jetbrains.com/help/teamcity/rest/buildapi.html#getBuildActualParameters
+
         :param build_id: TeamCity build id.
         :param property_name: A valid property name could be empty.
         :return: List format actual parameters or string format specific result attributes.
         """
         try:
-
             if property_name == '':
                 url = f'builds/id:{build_id}/resulting-properties'
                 return self.get_request(url)['property']
             else:
                 url = f'builds/id:{build_id}/resulting-properties/{property_name}'
                 return self.get_string_request(url)
         except Exception as ex:
             logging.error(ex)
             logging.error(f'Failed to get build {build_id} actual parameters.')
             return list() if property_name == '' else None
 
     def get_build_resulting_properties(self, build_id, property_name):
         """Get the specific resulting properties of the matching build from TeamCity.
 
+        Reference Page: https://www.jetbrains.com/help/teamcity/rest/buildapi.html#getBuildResultingProperties
+
         :param build_id: TeamCity build id.
         :param property_name: A valid property name must be provided.
         :return: String format specific result attributes.
         """
         if property_name == '':
             logging.error('Property name is empty. '
                           'Please provide a valid property name or use get_build_actual_parameters instead.')
@@ -348,14 +413,46 @@
               f'startEstimate,finishEstimate,plannedAgent(name,id,environment(osType),typeId,pool(id,name)),' \
               f'delayedByBuild(id,number,status,state,failedToStart,personal,canceledInfo,buildType(id)),' \
               f'triggered(date,displayText,buildType(id,paused,internalId,projectId,name,type,links(' \
               f'link(type,relativeUrl)))))'
         data = self.get_request(url)['build']
         return data if data else []
 
+    def get_all_changes(self, build_type_id='', locator='', count=10000):
+        """Get all changes by build type id from TeamCity."""
+        url = f'changes?count:{count}'
+        if build_type_id != '':
+            url += f',buildType:(id:{build_type_id})'
+        if locator != '':
+            url += f',{locator}'
+        try:
+            data = self.get_request(url)['change']
+            return data
+        except Exception as ex:
+            logging.error(ex)
+            logging.error(f'Failed to get all changes from TeamCity.')
+            return list()
+
+    def get_pending_changes(self, build_type_id='', locator=''):
+        """Get pending changes by build type id from TeamCity."""
+        url = f'changes?locator=buildType:(id:{build_type_id}),pending:true'
+        if locator != '':
+            url += f',{locator}'
+        try:
+            data = self.get_request(url)
+            if len(data) > 0 and 'change' in data:
+                return data['change']
+            else:
+                logging.info(f'No pending changes found for build type {build_type_id}.')
+                return list()
+        except Exception as ex:
+            logging.error(ex)
+            logging.error(f'Failed to get pending changes from TeamCity.')
+            return list()
+
     def get_user(self, username='') -> dict:
         """Get user by username from TeamCity.
 
         :param username: username, if empty - get current user
         :return: user dict, for example:
 
         {'username': 'teamcity', 'name': 'Teamcity', 'id': 200, 'email': 'support@jetbrains.com',
```

