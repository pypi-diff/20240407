# Comparing `tmp/cefi-4.4.8.tar.gz` & `tmp/cefi-4.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.4.8.tar", max compression
+gzip compressed data, was "cefi-4.4.9.tar", max compression
```

## Comparing `cefi-4.4.8.tar` & `cefi-4.4.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-07 14:35:05.528879 cefi-4.4.8/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-07 14:35:05.528879 cefi-4.4.8/README.md
--rw-r--r--   0        0        0       87 2024-04-07 14:35:40.232661 cefi-4.4.8/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/__init__.py
--rw-r--r--   0        0        0    10615 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     5517 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     7383 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8055 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/main.py
--rw-r--r--   0        0        0     3732 2024-04-07 14:35:40.232661 cefi-4.4.8/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 14:56:21.924445 cefi-4.4.9/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-07 14:56:21.924445 cefi-4.4.9/README.md
+-rw-r--r--   0        0        0       87 2024-04-07 14:56:56.448538 cefi-4.4.9/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    10668 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     7383 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8055 2024-04-07 14:56:21.924445 cefi-4.4.9/cefi/main.py
+-rw-r--r--   0        0        0     3734 2024-04-07 14:56:56.448538 cefi-4.4.9/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.9/PKG-INFO
```

### Comparing `cefi-4.4.8/LICENSE` & `cefi-4.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/README.md` & `cefi-4.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/cefi/default_settings.toml` & `cefi-4.4.9/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/cefi/handler/capitalcom.py` & `cefi-4.4.9/cefi/handler/capitalcom.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,16 @@
                 )
             else:
                 self.client = Client(
                     log=self.user_id,
                     pas=self.password,
                     api_key=self.api_key,
                 )
+
+            logger.debug("Client: {}", self.client)
             self.accounts_data = self.client.all_accounts()
             logger.debug("Account data: {}", self.accounts_data)
             self.account_number = self.accounts_data["accounts"][0]["accountId"]
             logger.debug("Account number: {}", self.account_number)
 
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
```

### Comparing `cefi-4.4.8/cefi/handler/ccxt.py` & `cefi-4.4.9/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/cefi/handler/client.py` & `cefi-4.4.9/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/cefi/handler/ctrader.py` & `cefi-4.4.9/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/cefi/handler/ib_sync.py` & `cefi-4.4.9/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/cefi/main.py` & `cefi-4.4.9/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.8/pyproject.toml` & `cefi-4.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.4.8"
+version = "4.4.9"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -145,27 +145,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.4.8/PKG-INFO` & `cefi-4.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.4.8
+Version: 4.4.9
 Summary: A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT
 Keywords: cex, cefi, crypto, exchange, broker
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cefi Version: 4.4.8 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.4.9 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

