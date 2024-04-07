# Comparing `tmp/podpointclient-1.4.3.tar.gz` & `tmp/podpointclient-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podpointclient-1.4.3.tar", last modified: Sun Feb 11 09:58:09 2024, max compression
+gzip compressed data, was "podpointclient-1.5.0.tar", last modified: Sun Apr  7 21:06:21 2024, max compression
```

## Comparing `podpointclient-1.4.3.tar` & `podpointclient-1.5.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 09:58:09.467515 podpointclient-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-11 09:58:00.000000 podpointclient-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-02-11 09:58:09.467515 podpointclient-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-02-11 09:58:00.000000 podpointclient-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 09:58:09.463515 podpointclient-1.4.3/podpointclient/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/charge_mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/charge_override.py
--rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/factories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 09:58:09.467515 podpointclient-1.4.3/podpointclient/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/helpers/api_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/helpers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/helpers/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/helpers/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/user.py
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-11 09:58:00.000000 podpointclient-1.4.3/podpointclient/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 09:58:09.463515 podpointclient-1.4.3/podpointclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-02-11 09:58:09.000000 podpointclient-1.4.3/podpointclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-11 09:58:09.000000 podpointclient-1.4.3/podpointclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 09:58:09.000000 podpointclient-1.4.3/podpointclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-11 09:58:09.000000 podpointclient-1.4.3/podpointclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-11 09:58:09.000000 podpointclient-1.4.3/podpointclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-11 09:58:00.000000 podpointclient-1.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 09:58:09.467515 podpointclient-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-11 09:58:00.000000 podpointclient-1.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.381305 podpointclient-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 21:06:04.000000 podpointclient-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-07 21:06:21.381305 podpointclient-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4607 2024-04-07 21:06:04.000000 podpointclient-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.377304 podpointclient-1.5.0/podpointclient/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/charge_mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/charge_override.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13230 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/factories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.381305 podpointclient-1.5.0/podpointclient/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6155 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/api_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5788 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/helpers/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15369 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7680 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-07 21:06:04.000000 podpointclient-1.5.0/podpointclient/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:06:21.381305 podpointclient-1.5.0/podpointclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 21:06:21.000000 podpointclient-1.5.0/podpointclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 21:06:04.000000 podpointclient-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:06:21.381305 podpointclient-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 21:06:04.000000 podpointclient-1.5.0/setup.py
```

### Comparing `podpointclient-1.4.3/LICENSE` & `podpointclient-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/PKG-INFO` & `podpointclient-1.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.4.3
+Version: 1.5.0
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.4.3/README.md` & `podpointclient-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/charge.py` & `podpointclient-1.5.0/podpointclient/charge.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/charge_override.py` & `podpointclient-1.5.0/podpointclient/charge_override.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/client.py` & `podpointclient-1.5.0/podpointclient/client.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/endpoints.py` & `podpointclient-1.5.0/podpointclient/endpoints.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,10 +13,14 @@
 API_BASE = 'mobile-api.pod-point.com/api3/'
 API_VERSION = 'v5'
 API_BASE_URL = f"https://{API_BASE}{API_VERSION}"
 
 """Google endpoint, used for auth"""
 GOOGLE_KEY = '?key=AIzaSyCwhF8IOl_7qHXML0pOd5HmziYP46IZAGU'
 PASSWORD_VERIFY = f"/verifyPassword{GOOGLE_KEY}"
+TOKEN = f"/token{GOOGLE_KEY}"
 
 GOOGLE_BASE = 'www.googleapis.com/identitytoolkit/v3/relyingparty'
 GOOGLE_BASE_URL = f"https://{GOOGLE_BASE}"
+
+GOOGLE_TOKEN_BASE = 'securetoken.googleapis.com/v1'
+GOOGLE_TOKEN_BASE_URL = f"https://{GOOGLE_TOKEN_BASE}"
```

### Comparing `podpointclient-1.4.3/podpointclient/errors.py` & `podpointclient-1.5.0/podpointclient/errors.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/factories.py` & `podpointclient-1.5.0/podpointclient/factories.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/helpers/api_wrapper.py` & `podpointclient-1.5.0/podpointclient/helpers/api_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,20 +121,28 @@
                         url,
                         headers=headers,
                         params=params,
                         json=data
                     )
 
                 elif method == "post":
-                    response = await self._session.post(
-                        url,
-                        headers=headers,
-                        params=params,
-                        json=data
-                    )
+                    if isinstance(data, str):
+                        response = await self._session.post(
+                            url,
+                            headers=headers,
+                            params=params,
+                            data=data
+                        )
+                    else:
+                        response = await self._session.post(
+                            url,
+                            headers=headers,
+                            params=params,
+                            json=data
+                        )
 
                 elif method == "delete":
                     response = await self._session.delete(url, headers=headers, params=params)
 
                 else:
                     raise ValueError(f'Method \'{method}\' not supported')
```

### Comparing `podpointclient-1.4.3/podpointclient/helpers/auth.py` & `podpointclient-1.5.0/podpointclient/helpers/auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from datetime import datetime, timedelta
 
 import aiohttp
 
 from ..errors import APIError, AuthError, SessionError
 from .session import Session
-from ..endpoints import GOOGLE_BASE_URL, PASSWORD_VERIFY
+from ..endpoints import GOOGLE_BASE_URL, PASSWORD_VERIFY, GOOGLE_TOKEN_BASE_URL, TOKEN
 from .functions import HEADERS
 from .api_wrapper import APIWrapper
 
 _LOGGER: logging.Logger = logging.getLogger(__package__)
 
 class Auth():
     """Manages authentication lifecycle for a user"""
@@ -57,15 +57,17 @@
     async def async_update_access_token(self) -> bool:
         """Update access token, if needed."""
         if self.check_access_token():
             return True
 
         try:
             _LOGGER.debug('Updating access token')
-            access_token_updated: bool = await self.__update_access_token()
+            access_token_updated: bool = await self.__update_access_token(
+                refresh=self.access_token_expired()
+            )
 
             _LOGGER.debug(
                 "Updated access token. New expiration: %s",
                 self.access_token_expiry
             )
 
             self.session = Session(
@@ -86,31 +88,53 @@
             raise exception
         except SessionError as exception:
             _LOGGER.error("Error creating session. %s", exception)
             raise exception
 
     async def __update_access_token(self, refresh: bool = False) -> bool:
         return_value = False
+        id_token_response = 'idToken'
+        refresh_token_response = 'refreshToken'
+        expires_in_response = 'expiresIn'
 
         try:
             wrapper = APIWrapper(session=self._session)
+
+            if refresh:
+                _LOGGER.debug('Refreshing access token')
+                headers = HEADERS.copy()
+                headers["Content-type"] = 'application/x-www-form-urlencoded'
+
+                url = f"{GOOGLE_TOKEN_BASE_URL}{TOKEN}"
+                body = f"grant_type=refresh_token&refresh_token={self.refresh_token}"
+
+                id_token_response = 'id_token'
+                refresh_token_response = 'refresh_token'
+                expires_in_response = 'expires_in'
+            else:
+                _LOGGER.debug('Getting a new access token')
+
+                url = f"{GOOGLE_BASE_URL}{PASSWORD_VERIFY}"
+                body = {"email": self.email, "returnSecureToken": True, "password": self.password}
+                headers = HEADERS.copy()
+
             response = await wrapper.post(
-                url=f"{GOOGLE_BASE_URL}{PASSWORD_VERIFY}",
-                body={"email": self.email, "returnSecureToken": True, "password": self.password},
-                headers=HEADERS,
+                url=url,
+                body=body,
+                headers=headers,
                 exception_class=AuthError)
 
             if response.status != 200:
                 await self.__handle_response_error(response, AuthError)
 
             json = await response.json()
-            self.access_token = json["idToken"]
-            self.refresh_token = json["refreshToken"]
+            self.access_token = json[id_token_response]
+            self.refresh_token = json[refresh_token_response]
             self.access_token_expiry = datetime.now() + timedelta(
-                seconds=int(json["expiresIn"]) - 10
+                seconds=int(json[expires_in_response]) - 10
             )
             return_value = True
 
             if self._http_debug:
                 _LOGGER.debug(json)
         except AuthError as exception:
             raise exception
@@ -130,8 +154,11 @@
 
         return return_value
 
     async def __handle_response_error(self, response, error_class):
         status = response.status
         response = await response.text()
 
+        if self._http_debug:
+            _LOGGER.debug(response)
+
         raise error_class(status, response)
```

### Comparing `podpointclient-1.4.3/podpointclient/helpers/functions.py` & `podpointclient-1.5.0/podpointclient/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/helpers/session.py` & `podpointclient-1.5.0/podpointclient/helpers/session.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/pod.py` & `podpointclient-1.5.0/podpointclient/pod.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/schedule.py` & `podpointclient-1.5.0/podpointclient/schedule.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient/user.py` & `podpointclient-1.5.0/podpointclient/user.py`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/podpointclient.egg-info/PKG-INFO` & `podpointclient-1.5.0/podpointclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podpointclient
-Version: 1.4.3
+Version: 1.5.0
 Summary: A simple API client for Pod Point (https://pod-point.com) aimed at home users
 Home-page: https://github.com/mattrayner/podpointclient
 Author: Matthew Rayner
 Author-email: hello@rayner.io
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mattrayner/podpointclient/issues
 Keywords: Pod Point PodPoint
```

### Comparing `podpointclient-1.4.3/podpointclient.egg-info/SOURCES.txt` & `podpointclient-1.5.0/podpointclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `podpointclient-1.4.3/setup.py` & `podpointclient-1.5.0/setup.py`

 * *Files identical despite different names*

