# Comparing `tmp/ehdtd-0.1.3.tar.gz` & `tmp/ehdtd-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ehdtd-0.1.3.tar", max compression
+gzip compressed data, was "ehdtd-0.1.4.tar", max compression
```

## Comparing `ehdtd-0.1.3.tar` & `ehdtd-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.3/LICENSE
--rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.3/README.md
--rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.3/ehdtd/__init__.py
--rw-r--r--   0        0        0    20149 2024-02-26 01:49:11.663755 ehdtd-0.1.3/ehdtd/binance.py
--rw-r--r--   0        0        0   105082 2024-03-21 02:38:07.275171 ehdtd-0.1.3/ehdtd/ehdtd.py
--rw-r--r--   0        0        0     6540 2024-02-26 01:34:46.815409 ehdtd-0.1.3/ehdtd/ehdtd_common_functions.py
--rw-r--r--   0        0        0      683 2024-03-21 02:37:43.807937 ehdtd-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1105 2023-11-23 05:07:16.141066 ehdtd-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2530 2024-02-29 07:50:34.714293 ehdtd-0.1.4/README.md
+-rw-r--r--   0        0        0      921 2023-11-28 02:30:35.236883 ehdtd-0.1.4/ehdtd/__init__.py
+-rw-r--r--   0        0        0    21441 2024-04-07 03:50:53.982388 ehdtd-0.1.4/ehdtd/binance.py
+-rw-r--r--   0        0        0   105876 2024-04-07 04:00:06.936458 ehdtd-0.1.4/ehdtd/ehdtd.py
+-rw-r--r--   0        0        0     6540 2024-02-26 01:34:46.815409 ehdtd-0.1.4/ehdtd/ehdtd_common_functions.py
+-rw-r--r--   0        0        0      683 2024-04-07 05:47:00.921192 ehdtd-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3523 1970-01-01 00:00:00.000000 ehdtd-0.1.4/PKG-INFO
```

### Comparing `ehdtd-0.1.3/LICENSE` & `ehdtd-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.3/README.md` & `ehdtd-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.3/ehdtd/__init__.py` & `ehdtd-0.1.4/ehdtd/__init__.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.3/ehdtd/binance.py` & `ehdtd-0.1.4/ehdtd/binance.py`

 * *Files 3% similar despite different names*

```diff
@@ -323,14 +323,50 @@
             #__url_test = 'https://testnet.binance.vision/api/v3'
 
         result = __url_api
 
         return result
 
     @classmethod
+    def get_exchange_connectivity(cls):
+        """
+        get_exchange_connectivity
+        =========================
+            This function return a dict with connectivity information.
+                :param cls: BinanceEhdtdAuxClass Class.
+                :return dict: result.
+                    result = {
+                        'result': bool, # True if connectivity is working False in other case.
+                        'code': int | None, # Error Code
+                        'msg': str | None # Error message
+                    }
+        """
+        result = None
+
+        __url_api = cls.get_api_url()
+        __endpoint = '/ping'
+        __url = f'{__url_api}{__endpoint}'
+        __data = ecf.file_get_contents_url(__url)
+        if ecf.is_json(__data):
+            __data = json.loads(__data)
+            if __data is not None and isinstance(__data, dict):
+                result = {}
+                result['result'] = True
+                result['code'] = None
+                result['msg'] = None
+
+                if 'code' in __data:
+                    result['result'] = False
+                    result['code'] = __data['code']
+                    if 'msg' in __data:
+                        result['msg'] = __data['msg']
+
+        return result
+
+    @classmethod
     def get_unified_symbol_from_symbol(cls, symbol):
         """
         get_unified_symbol_from_symbol
         ==============================
             This function get unified symbol from symbol.
                 :param cls: BinanceEhdtdAuxClass Class.
                 :param symbol: str.
```

### Comparing `ehdtd-0.1.3/ehdtd/ehdtd.py` & `ehdtd-0.1.4/ehdtd/ehdtd.py`

 * *Files 1% similar despite different names*

```diff
@@ -2427,14 +2427,39 @@
                 :return: list of supported exchanges.
         """
         __suported_exchanges = ['binance']
 
         return __suported_exchanges
 
     @classmethod
+    def get_exchange_connectivity(cls, exchange='binance'):
+        """
+        get_exchange_connectivity.
+        =========================
+            This function return a dict with connectivity information.
+                :param cls: Ehdtd Class.
+                :param exchange: str.
+
+                :return dict: result.
+                    result = {
+                        'result': bool, # True if connectivity is working False in other case.
+                        'code': int | None, # Error Code
+                        'msg': str | None # Error message
+                    }
+
+        """
+        __result = None
+
+        __result = (
+            EhdtdExchangeConfig.exchange_classes[exchange]().get_exchange_connectivity()
+        )
+
+        return __result
+
+    @classmethod
     def get_supported_intervals(cls, exchange='binance'):
         """
         get_supported_intervals.
         ========================
             This method return a list of supported intervals.
                 :param cls: Ehdtd Class.
                 :param exchange: str.
```

### Comparing `ehdtd-0.1.3/ehdtd/ehdtd_common_functions.py` & `ehdtd-0.1.4/ehdtd/ehdtd_common_functions.py`

 * *Files identical despite different names*

### Comparing `ehdtd-0.1.3/pyproject.toml` & `ehdtd-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ehdtd"
-version = "0.1.3"
+version = "0.1.4"
 description = "Ehdtd - cryptoCurrency Exchange history data to database"
 authors = ["Ricardo Marcelo Alvarez <rmalvarezkai@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/rmalvarezkai/ehdtd"
 
 [tool.poetry.dependencies]
```

### Comparing `ehdtd-0.1.3/PKG-INFO` & `ehdtd-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ehdtd
-Version: 0.1.3
+Version: 0.1.4
 Summary: Ehdtd - cryptoCurrency Exchange history data to database
 Home-page: https://github.com/rmalvarezkai/ehdtd
 License: MIT
 Author: Ricardo Marcelo Alvarez
 Author-email: rmalvarezkai@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

