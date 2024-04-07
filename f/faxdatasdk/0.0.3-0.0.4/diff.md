# Comparing `tmp/faxdatasdk-0.0.3.tar.gz` & `tmp/faxdatasdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faxdatasdk-0.0.3.tar", last modified: Fri Jan 19 07:30:10 2024, max compression
+gzip compressed data, was "faxdatasdk-0.0.4.tar", last modified: Sun Apr  7 14:32:02 2024, max compression
```

## Comparing `faxdatasdk-0.0.3.tar` & `faxdatasdk-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-01-19 07:30:10.017221 faxdatasdk-0.0.3/
--rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 faxdatasdk-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     3484 2024-01-19 07:30:10.017221 faxdatasdk-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2770 2024-01-06 09:53:52.000000 faxdatasdk-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-01-19 07:30:10.006220 faxdatasdk-0.0.3/faxdatasdk/
--rw-rw-rw-   0        0        0     1247 2023-12-30 10:47:04.000000 faxdatasdk-0.0.3/faxdatasdk/__init__.py
--rw-rw-rw-   0        0        0    10579 2024-01-19 07:28:47.000000 faxdatasdk-0.0.3/faxdatasdk/api.py
--rw-rw-rw-   0        0        0     9351 2023-12-30 04:43:59.000000 faxdatasdk-0.0.3/faxdatasdk/client.py
-drwxrwxrwx   0        0        0        0 2024-01-19 07:30:10.016220 faxdatasdk-0.0.3/faxdatasdk/compat/
--rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 faxdatasdk-0.0.3/faxdatasdk/compat/__init__.py
--rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 faxdatasdk-0.0.3/faxdatasdk/compat/pickle_compat.py
--rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 faxdatasdk-0.0.3/faxdatasdk/exceptions.py
--rw-rw-rw-   0        0        0     3417 2023-12-29 07:30:25.000000 faxdatasdk-0.0.3/faxdatasdk/logger.py
--rw-rw-rw-   0        0        0     2216 2023-12-30 10:25:49.000000 faxdatasdk-0.0.3/faxdatasdk/request.py
--rw-rw-rw-   0        0        0      793 2023-07-09 16:17:28.000000 faxdatasdk-0.0.3/faxdatasdk/thrift_client.py
--rw-rw-rw-   0        0        0      590 2023-12-30 02:20:26.000000 faxdatasdk-0.0.3/faxdatasdk/utils.py
--rw-rw-rw-   0        0        0      438 2024-01-19 07:30:06.000000 faxdatasdk-0.0.3/faxdatasdk/version.py
-drwxrwxrwx   0        0        0        0 2024-01-19 07:30:10.015221 faxdatasdk-0.0.3/faxdatasdk.egg-info/
--rw-rw-rw-   0        0        0     3484 2024-01-19 07:30:09.000000 faxdatasdk-0.0.3/faxdatasdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2024-01-19 07:30:09.000000 faxdatasdk-0.0.3/faxdatasdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-19 07:30:09.000000 faxdatasdk-0.0.3/faxdatasdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-29 08:32:19.000000 faxdatasdk-0.0.3/faxdatasdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      151 2024-01-19 07:30:09.000000 faxdatasdk-0.0.3/faxdatasdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-01-19 07:30:09.000000 faxdatasdk-0.0.3/faxdatasdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-19 07:30:10.018220 faxdatasdk-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1976 2023-12-29 08:29:21.000000 faxdatasdk-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-19 07:30:10.017221 faxdatasdk-0.0.3/tests/
--rw-rw-rw-   0        0        0     2161 2023-12-30 04:54:05.000000 faxdatasdk-0.0.3/tests/test_faxdatasdk.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:32:02.116410 faxdatasdk-0.0.4/
+-rw-rw-rw-   0        0        0    11558 2023-07-09 16:17:28.000000 faxdatasdk-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     3484 2024-04-07 14:32:02.115409 faxdatasdk-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2770 2024-01-06 09:53:52.000000 faxdatasdk-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 14:32:02.102410 faxdatasdk-0.0.4/faxdatasdk/
+-rw-rw-rw-   0        0        0     1294 2024-04-07 13:47:56.000000 faxdatasdk-0.0.4/faxdatasdk/__init__.py
+-rw-rw-rw-   0        0        0    10579 2024-01-19 07:28:47.000000 faxdatasdk-0.0.4/faxdatasdk/api.py
+-rw-rw-rw-   0        0        0     9605 2024-04-07 14:10:47.000000 faxdatasdk-0.0.4/faxdatasdk/client.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:32:02.114410 faxdatasdk-0.0.4/faxdatasdk/compat/
+-rw-rw-rw-   0        0        0        0 2023-07-09 16:17:28.000000 faxdatasdk-0.0.4/faxdatasdk/compat/__init__.py
+-rw-rw-rw-   0        0        0     2187 2023-07-09 16:17:28.000000 faxdatasdk-0.0.4/faxdatasdk/compat/pickle_compat.py
+-rw-rw-rw-   0        0        0      175 2023-07-09 16:17:28.000000 faxdatasdk-0.0.4/faxdatasdk/exceptions.py
+-rw-rw-rw-   0        0        0     3417 2023-12-29 07:30:25.000000 faxdatasdk-0.0.4/faxdatasdk/logger.py
+-rw-rw-rw-   0        0        0     2216 2023-12-30 10:25:49.000000 faxdatasdk-0.0.4/faxdatasdk/request.py
+-rw-rw-rw-   0        0        0      811 2024-04-07 14:11:07.000000 faxdatasdk-0.0.4/faxdatasdk/thrift_client.py
+-rw-rw-rw-   0        0        0      590 2023-12-30 02:20:26.000000 faxdatasdk-0.0.4/faxdatasdk/utils.py
+-rw-rw-rw-   0        0        0      438 2024-04-07 14:15:47.000000 faxdatasdk-0.0.4/faxdatasdk/version.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:32:02.113411 faxdatasdk-0.0.4/faxdatasdk.egg-info/
+-rw-rw-rw-   0        0        0     3484 2024-04-07 14:32:02.000000 faxdatasdk-0.0.4/faxdatasdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      493 2024-04-07 14:32:02.000000 faxdatasdk-0.0.4/faxdatasdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 14:32:02.000000 faxdatasdk-0.0.4/faxdatasdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 14:32:02.000000 faxdatasdk-0.0.4/faxdatasdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      151 2024-04-07 14:32:02.000000 faxdatasdk-0.0.4/faxdatasdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 14:32:02.000000 faxdatasdk-0.0.4/faxdatasdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 14:32:02.116410 faxdatasdk-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1966 2024-04-07 14:26:19.000000 faxdatasdk-0.0.4/setup.py
```

### Comparing `faxdatasdk-0.0.3/LICENSE` & `faxdatasdk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.3/PKG-INFO` & `faxdatasdk-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faxdatasdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data SDK for stock analysis.
 Home-page: https://www.faxframework.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
```

### Comparing `faxdatasdk-0.0.3/README.md` & `faxdatasdk-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.3/faxdatasdk/__init__.py` & `faxdatasdk-0.0.4/faxdatasdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 
 def auth(username, password, host=None, port=None):
     """账号认证"""
     FaxDataClient.set_auth_params(host=host, port=port, username=username, password=password)
 
 
-def auth_by_token(token, host=None, port=None):
+def auth_by_token(token, host=None, port=None, audience="resource-client"):
     """使用 token 认证账号"""
-    FaxDataClient.set_auth_params(host=host, port=port, token=token)
+    FaxDataClient.set_auth_params(host=host, port=port, token=token, audience=audience)
 
 
 @assert_auth
 def request(method, url, params=None, data=None, json=None, **kwargs):
     return FaxDataClient.instance().request(method=method, url=url, params=params, data=data, json=json, **kwargs)
```

### Comparing `faxdatasdk-0.0.3/faxdatasdk/api.py` & `faxdatasdk-0.0.4/faxdatasdk/api.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.3/faxdatasdk/client.py` & `faxdatasdk-0.0.4/faxdatasdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,20 +34,28 @@
 
     _default_host = "47.101.192.116"
     _default_port = 7000
 
     request_timeout = 300
     request_attempt_count = 3
 
-    def __init__(self, host=None, port=None, username="", password="", token="", token_type=""):
+    def __init__(self,
+                 host=None,
+                 port=None,
+                 username="",
+                 password="",
+                 token="",
+                 token_type="",
+                 audience="resource-client"):
         self.host = host or self._default_host
         self.port = int(port or self._default_port)
         self.username = username
         self.password = password
         self.token = token
+        self.audience = audience
         self.token_type = token_type
 
         assert self.host, "host is required"
         assert self.port, "port is required"
         assert self.username or self.token, "username is required"
         assert self.password or self.token, "password is required"
 
@@ -101,15 +109,15 @@
                     response = self.client.auth(self.username,
                                                 self.password,
                                                 self.compress,
                                                 get_mac_address(),
                                                 current_version, )
                 else:
                     # Token登录
-                    response = self.client.auth_by_token(self.token)
+                    response = self.client.auth_by_token(self.token, self.audience)
                     break
             except socket_error as ex:
                 error = ex
                 time.sleep(0.5)
                 if self.client:
                     self.client.close()
                     self.client = None
@@ -121,15 +129,16 @@
         auth_message = zlib.decompress(response.msg).decode('utf-8')
 
         if not response.status:
             self._threading_local._instance = None
             raise self.get_error(response)
         else:
             if self.not_auth:
-                log.debug("账号认证成功: %s" % auth_message)
+                # log.debug("账号认证成功: %s" % auth_message)
+                log.debug("账号认证成功")
                 self.not_auth = False
         # 保存token
         self.token = json.loads(auth_message)['token']
         self.token_type = json.loads(auth_message)['token_type']
         self.inited = True
 
     def get_error(self, response):
```

### Comparing `faxdatasdk-0.0.3/faxdatasdk/compat/pickle_compat.py` & `faxdatasdk-0.0.4/faxdatasdk/compat/pickle_compat.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.3/faxdatasdk/logger.py` & `faxdatasdk-0.0.4/faxdatasdk/logger.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.3/faxdatasdk/request.py` & `faxdatasdk-0.0.4/faxdatasdk/request.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.3/faxdatasdk/thrift_client.py` & `faxdatasdk-0.0.4/faxdatasdk/thrift_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,12 +19,12 @@
     3:required binary data,
 }
 
 service DataService {
     string ping(),
     Query_Response query(1:Query_Request req),
     Query_Response auth(1:string username, 2:string password, 5:bool compress, 8:string mac, 10:string version),
-    Query_Response auth_by_token(1: string token),
+    Query_Response auth_by_token(1:string token, 2:string audience),
     Query_Response submit(1:Submit_Request req)
 }
 """
 thrift = thriftpy.load_fp(six.StringIO(api_description), "api_thrift")
```

### Comparing `faxdatasdk-0.0.3/faxdatasdk/utils.py` & `faxdatasdk-0.0.4/faxdatasdk/utils.py`

 * *Files identical despite different names*

### Comparing `faxdatasdk-0.0.3/faxdatasdk.egg-info/PKG-INFO` & `faxdatasdk-0.0.4/faxdatasdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faxdatasdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: Data SDK for stock analysis.
 Home-page: https://www.faxframework.com
 Author: PinkQuant
 Author-email: tickertrading@163.com
 Maintainer: topbip
 Maintainer-email: pinkquant@163.com
 License: Apache License v2
```

### Comparing `faxdatasdk-0.0.3/setup.py` & `faxdatasdk-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     return _parse_requirement_file(requirement_file)
 
 
 setup(
     name="faxdatasdk",
     version=get_version(),
     description="Data SDK for stock analysis.",
-    packages=find_packages(exclude=("tests", "tests.*")),
+    packages=find_packages(exclude=("tests",)),
     author="PinkQuant",
     author_email="tickertrading@163.com",
     maintainer="topbip",
     maintainer_email="pinkquant@163.com",
     license='Apache License v2',
     package_data={'': ['*.*']},
     url="https://www.faxframework.com",
```

