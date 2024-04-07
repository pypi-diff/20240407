# Comparing `tmp/cefi-4.4.5.tar.gz` & `tmp/cefi-4.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.4.5.tar", max compression
+gzip compressed data, was "cefi-4.4.6.tar", max compression
```

## Comparing `cefi-4.4.5.tar` & `cefi-4.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-06 07:33:06.424594 cefi-4.4.5/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-06 07:33:06.424594 cefi-4.4.5/README.md
--rw-r--r--   0        0        0       87 2024-04-06 07:33:38.712517 cefi-4.4.5/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/handler/__init__.py
--rw-r--r--   0        0        0     9083 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     4838 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     6972 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8055 2024-04-06 07:33:06.424594 cefi-4.4.5/cefi/main.py
--rw-r--r--   0        0        0     3726 2024-04-06 07:33:38.712517 cefi-4.4.5/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 07:13:31.092395 cefi-4.4.6/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-07 07:13:31.092395 cefi-4.4.6/README.md
+-rw-r--r--   0        0        0       87 2024-04-07 07:14:05.168242 cefi-4.4.6/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/handler/__init__.py
+-rw-r--r--   0        0        0     9536 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     4838 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     6972 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8055 2024-04-07 07:13:31.092395 cefi-4.4.6/cefi/main.py
+-rw-r--r--   0        0        0     3728 2024-04-07 07:14:05.168242 cefi-4.4.6/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.6/PKG-INFO
```

### Comparing `cefi-4.4.5/LICENSE` & `cefi-4.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/README.md` & `cefi-4.4.6/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/cefi/default_settings.toml` & `cefi-4.4.6/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/cefi/handler/capitalcom.py` & `cefi-4.4.6/cefi/handler/capitalcom.py`

 * *Files 4% similar despite different names*

```diff
@@ -255,29 +255,35 @@
                 )
                 if action_str == "BUY"
                 else (
                     await self.get_quote(instrument)
                     + (order_params.get("stop_loss", 0) / (10**decimals))
                 )
             )
-
+            logger.debug("stop price {}", stop_price)
+            logger.debug("profit price {}", profit_price)
             try:
                 order = self.client.place_the_position(
                     direction=action,
                     epic=instrument,
                     size=amount,
                     gsl=False,
                     tsl=False,
                     stop_level=stop_price,
                     stop_distance=None,
                     stop_amount=None,
                     profit_level=profit_price,
                     profit_distance=None,
                     profit_amount=None,
                 )
+                # Check if the order response contains an errorCode
+                if "errorCode" in order:
+                    # Handle the error, e.g., log it or return a specific message
+                    logger.error(f"Error placing order: {order['errorCode']}")
+                    return f"Error placing order: {order['errorCode']}"
             except Exception as e:
                 return str(e)
 
             logger.debug("Order: {}", order)
             deal_reference = order["dealReference"]
             order_check = self.client.position_order_confirmation(
                 deal_reference=deal_reference
```

### Comparing `cefi-4.4.5/cefi/handler/ccxt.py` & `cefi-4.4.6/cefi/handler/ccxt.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/cefi/handler/client.py` & `cefi-4.4.6/cefi/handler/client.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/cefi/handler/ctrader.py` & `cefi-4.4.6/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/cefi/handler/ib_sync.py` & `cefi-4.4.6/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/cefi/main.py` & `cefi-4.4.6/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.5/pyproject.toml` & `cefi-4.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.4.5"
+version = "4.4.6"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -142,27 +142,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.4.5/PKG-INFO` & `cefi-4.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.4.5
+Version: 4.4.6
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
-Metadata-Version: 2.1 Name: cefi Version: 4.4.5 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.4.6 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

