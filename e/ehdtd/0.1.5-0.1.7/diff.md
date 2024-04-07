# Comparing `tmp/ehdtd-0.1.5.tar.gz` & `tmp/ehdtd-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd-0.1.5.tar", max compression
+gzip compressed data, was "ehdtd-0.1.7.tar", max compression
```

## Comparing `ehdtd-0.1.5.tar` & `ehdtd-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.5/LICENSE
--rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.5/README.md
--rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.5/ehdtd/__init__.py
--rw-r--r--   0        0        0    23627 2024-04-07 10:15:34.286547 ehdtd-0.1.5/ehdtd/binance.py
--rw-r--r--   0        0        0   105876 2024-04-07 04:00:06.936458 ehdtd-0.1.5/ehdtd/ehdtd.py
--rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.1.5/ehdtd/ehdtd_common_functions.py
--rw-r--r--   0        0        0      683 2024-04-07 10:18:28.832548 ehdtd-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.7/README.md
+-rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.7/ehdtd/__init__.py
+-rw-r--r--   0        0        0    23616 2024-04-07 11:09:25.919645 ehdtd-0.1.7/ehdtd/binance.py
+-rw-r--r--   0        0        0   105876 2024-04-07 04:00:06.936458 ehdtd-0.1.7/ehdtd/ehdtd.py
+-rw-r--r--   0        0        0     6539 2024-04-07 09:34:20.505668 ehdtd-0.1.7/ehdtd/ehdtd_common_functions.py
+-rw-r--r--   0        0        0      683 2024-04-07 11:12:35.028850 ehdtd-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.7/PKG-INFO
```

### Comparing `ehdtd-0.1.5/LICENSE` & `ehdtd-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.5/README.md` & `ehdtd-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.5/ehdtd/__init__.py` & `ehdtd-0.1.7/ehdtd/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.5/ehdtd/binance.py` & `ehdtd-0.1.7/ehdtd/binance.py`

 * *Files 1% similar despite different names*

```diff
@@ -371,15 +371,15 @@
                 result['headers'] = None
                 result['headers_str'] = None
                 result['final_url'] = None
                 result['res_code'] = None
                 result['res_msg'] = None
 
                 if hasattr(exc, 'code'):
-                    result['code'] = response.status
+                    result['code'] = exc.code
                 if hasattr(exc, 'read'):
                     result['data'] = exc.read().decode('utf-8')
                 if hasattr(exc, 'headers'):
                     result['headers'] = exc.headers
                     header_str = ''
                     for header in exc.headers:
                         header_str += f'{header}: {exc.headers[header]}'
@@ -397,15 +397,15 @@
                 if ecf.is_json(result['data']):
                     result['data'] = json.loads(result['data'])
 
                     if result['data'] is not None and isinstance(result['data'], dict):
                         if 'code' in result['data']:
                             result['res_code'] = result['data']['code']
                         if 'msg' in result['data']:
-                            result['res_msg'] = result['data']['res_msg']
+                            result['res_msg'] = result['data']['msg']
 
                 if result['code'] is not None\
                     and isinstance(result['code'], int)\
                     and 200 <= result['code'] < 300\
                     and result['res_code'] is None:
                     result['result'] = True
                 else:
```

### Comparing `ehdtd-0.1.5/ehdtd/ehdtd.py` & `ehdtd-0.1.7/ehdtd/ehdtd.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.5/ehdtd/ehdtd_common_functions.py` & `ehdtd-0.1.7/ehdtd/ehdtd_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.5/pyproject.toml` & `ehdtd-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd"
-version = "0.1.5"
+version = "0.1.7"
 description = "Ehdtd - cryptoCurrency Exchange history data to database"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/rmalvarezkai/ehdtd"
 
 [tool.poetry.dependencies]
```

### Comparing `ehdtd-0.1.5/PKG-INFO` & `ehdtd-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd
-Version: 0.1.5
+Version: 0.1.7
 Summary: Ehdtd - cryptoCurrency Exchange history data to database
 Home-page: https://github.com/rmalvarezkai/ehdtd
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

