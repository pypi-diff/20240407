# Comparing `tmp/http_injector-1.0.4.tar.gz` & `tmp/http_injector-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "http_injector-1.0.4.tar", max compression
+gzip compressed data, was "http_injector-1.0.5.tar", max compression
```

## Comparing `http_injector-1.0.4.tar` & `http_injector-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      170 2024-03-28 14:22:26.271497 http_injector-1.0.4/http_injector/__init__.py
--rw-r--r--   0        0        0      344 2024-03-28 12:54:13.763832 http_injector-1.0.4/http_injector/_adapter/__init__.py
--rw-r--r--   0        0        0     1097 2024-03-28 12:52:04.015953 http_injector-1.0.4/http_injector/_adapter/_Requests.py
--rw-r--r--   0        0        0      284 2024-03-28 12:49:02.327773 http_injector-1.0.4/http_injector/_context/__init__.py
--rw-r--r--   0        0        0     1811 2024-03-18 20:21:43.971226 http_injector-1.0.4/http_injector/_context/CIPHERS.py
--rw-r--r--   0        0        0      282 2024-03-18 20:21:43.972229 http_injector-1.0.4/http_injector/_context/SSLContext.py
--rw-r--r--   0        0        0     1256 2024-03-30 02:02:11.396465 http_injector-1.0.4/http_injector/_Httpx.py
--rw-r--r--   0        0        0     1500 2024-04-05 16:36:15.171274 http_injector-1.0.4/http_injector/_Injector.py
--rw-r--r--   0        0        0      682 2024-03-30 01:37:14.713457 http_injector-1.0.4/http_injector/_Requests.py
--rw-r--r--   0        0        0      214 2024-03-28 12:58:15.575396 http_injector-1.0.4/http_injector/_utils/__init__.py
--rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 http_injector-1.0.4/http_injector/_utils/_certificate/__init__.py
--rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 http_injector-1.0.4/http_injector/_utils/_certificate/cacert.pem
--rw-r--r--   0        0        0      439 2024-04-05 16:36:31.496417 http_injector-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       25 2024-03-28 13:19:27.878232 http_injector-1.0.4/README.md
--rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 http_injector-1.0.4/setup.py
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 http_injector-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      170 2024-03-28 14:22:26.271497 http_injector-1.0.5/http_injector/__init__.py
+-rw-r--r--   0        0        0      344 2024-03-28 12:54:13.763832 http_injector-1.0.5/http_injector/_adapter/__init__.py
+-rw-r--r--   0        0        0     1097 2024-03-28 12:52:04.015953 http_injector-1.0.5/http_injector/_adapter/_Requests.py
+-rw-r--r--   0        0        0      284 2024-03-28 12:49:02.327773 http_injector-1.0.5/http_injector/_context/__init__.py
+-rw-r--r--   0        0        0     1811 2024-03-18 20:21:43.971226 http_injector-1.0.5/http_injector/_context/CIPHERS.py
+-rw-r--r--   0        0        0      282 2024-03-18 20:21:43.972229 http_injector-1.0.5/http_injector/_context/SSLContext.py
+-rw-r--r--   0        0        0     1256 2024-03-30 02:02:11.396465 http_injector-1.0.5/http_injector/_Httpx.py
+-rw-r--r--   0        0        0     1520 2024-04-07 16:25:43.869818 http_injector-1.0.5/http_injector/_Injector.py
+-rw-r--r--   0        0        0      682 2024-03-30 01:37:14.713457 http_injector-1.0.5/http_injector/_Requests.py
+-rw-r--r--   0        0        0      214 2024-03-28 12:58:15.575396 http_injector-1.0.5/http_injector/_utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-18 20:21:44.103798 http_injector-1.0.5/http_injector/_utils/_certificate/__init__.py
+-rw-r--r--   0        0        0   286252 2024-03-18 20:21:44.105798 http_injector-1.0.5/http_injector/_utils/_certificate/cacert.pem
+-rw-r--r--   0        0        0      439 2024-04-07 16:26:00.478974 http_injector-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       25 2024-03-28 13:19:27.878232 http_injector-1.0.5/README.md
+-rw-r--r--   0        0        0      819 1970-01-01 00:00:00.000000 http_injector-1.0.5/setup.py
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 http_injector-1.0.5/PKG-INFO
```

### Comparing `http_injector-1.0.4/http_injector/_adapter/_Requests.py` & `http_injector-1.0.5/http_injector/_adapter/_Requests.py`

 * *Files identical despite different names*

### Comparing `http_injector-1.0.4/http_injector/_context/CIPHERS.py` & `http_injector-1.0.5/http_injector/_context/CIPHERS.py`

 * *Files identical despite different names*

### Comparing `http_injector-1.0.4/http_injector/_Httpx.py` & `http_injector-1.0.5/http_injector/_Httpx.py`

 * *Files identical despite different names*

### Comparing `http_injector-1.0.4/http_injector/_Injector.py` & `http_injector-1.0.5/http_injector/_Injector.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
             build = f'{USERNAME}:{PASSWORD}@{IP}:{PORT}'
         else:
             build = f'{IP}:{PORT}'
         if type == ProxyType.http:
             setattr(ProxyParams, 'URL', f'http://{build}')
         elif type == ProxyType.socks5:
             setattr(ProxyParams, 'URL', f'socks5://{build}')
+        return cls
 
 class HTTPInjector(_HAdapter, _RAdapter):
 
     def __new__(cls, typeInjector: TypeInjector, timeout: int = 30, headers: Dict[str, str] = dict(), proxyParams: Optional[ProxyParams] = None) -> Union[Client, Session]:
         if not proxyParams:
             proxy_url = None
         else:
```

### Comparing `http_injector-1.0.4/http_injector/_Requests.py` & `http_injector-1.0.5/http_injector/_Requests.py`

 * *Files identical despite different names*

### Comparing `http_injector-1.0.4/http_injector/_utils/_certificate/cacert.pem` & `http_injector-1.0.5/http_injector/_utils/_certificate/cacert.pem`

 * *Files identical despite different names*

### Comparing `http_injector-1.0.4/setup.py` & `http_injector-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 install_requires = \
 ['chardet>=5.2.0,<6.0.0',
  'httpx[http2,socks]>=0.27.0,<0.28.0',
  'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'http-injector',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': '',
     'long_description': 'pip install http_injector',
     'author': 'DesKaOne',
     'author_email': 'DesKaOne@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `http_injector-1.0.4/PKG-INFO` & `http_injector-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: http-injector
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 Author: DesKaOne
 Author-email: DesKaOne@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

