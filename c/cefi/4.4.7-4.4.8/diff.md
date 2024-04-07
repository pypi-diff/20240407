# Comparing `tmp/cefi-4.4.7.tar.gz` & `tmp/cefi-4.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cefi-4.4.7.tar", max compression
+gzip compressed data, was "cefi-4.4.8.tar", max compression
```

## Comparing `cefi-4.4.7.tar` & `cefi-4.4.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1064 2024-04-07 12:45:07.754900 cefi-4.4.7/LICENSE
--rw-r--r--   0        0        0     2661 2024-04-07 12:45:07.754900 cefi-4.4.7/README.md
--rw-r--r--   0        0        0       87 2024-04-07 12:45:42.711196 cefi-4.4.7/cefi/__init__.py
--rw-r--r--   0        0        0      439 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/config.py
--rw-r--r--   0        0        0     3617 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/default_settings.toml
--rw-r--r--   0        0        0      158 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/handler/__init__.py
--rw-r--r--   0        0        0    10502 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/handler/capitalcom.py
--rw-r--r--   0        0        0     4838 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/handler/ccxt.py
--rw-r--r--   0        0        0     6972 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/handler/client.py
--rw-r--r--   0        0        0     1938 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/handler/ctrader.py
--rw-r--r--   0        0        0     7006 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/handler/ib_sync.py
--rw-r--r--   0        0        0     8055 2024-04-07 12:45:07.754900 cefi-4.4.7/cefi/main.py
--rw-r--r--   0        0        0     3730 2024-04-07 12:45:42.711196 cefi-4.4.7/pyproject.toml
--rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 14:35:05.528879 cefi-4.4.8/LICENSE
+-rw-r--r--   0        0        0     2661 2024-04-07 14:35:05.528879 cefi-4.4.8/README.md
+-rw-r--r--   0        0        0       87 2024-04-07 14:35:40.232661 cefi-4.4.8/cefi/__init__.py
+-rw-r--r--   0        0        0      439 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/config.py
+-rw-r--r--   0        0        0     3617 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/default_settings.toml
+-rw-r--r--   0        0        0      158 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/__init__.py
+-rw-r--r--   0        0        0    10615 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/capitalcom.py
+-rw-r--r--   0        0        0     5517 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/ccxt.py
+-rw-r--r--   0        0        0     7383 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/client.py
+-rw-r--r--   0        0        0     1938 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/ctrader.py
+-rw-r--r--   0        0        0     7006 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/handler/ib_sync.py
+-rw-r--r--   0        0        0     8055 2024-04-07 14:35:05.528879 cefi-4.4.8/cefi/main.py
+-rw-r--r--   0        0        0     3732 2024-04-07 14:35:40.232661 cefi-4.4.8/pyproject.toml
+-rw-r--r--   0        0        0     3657 1970-01-01 00:00:00.000000 cefi-4.4.8/PKG-INFO
```

### Comparing `cefi-4.4.7/LICENSE` & `cefi-4.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cefi-4.4.7/README.md` & `cefi-4.4.8/README.md`

 * *Files identical despite different names*

### Comparing `cefi-4.4.7/cefi/default_settings.toml` & `cefi-4.4.8/cefi/default_settings.toml`

 * *Files identical despite different names*

### Comparing `cefi-4.4.7/cefi/handler/capitalcom.py` & `cefi-4.4.8/cefi/handler/capitalcom.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,24 +67,19 @@
             logger.debug("Account number: {}", self.account_number)
 
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
 
     async def get_quote(self, instrument):
         """
-        Return a quote for a instrument
-        of a given exchange ccxt object
+        Asynchronously fetches a ask/offer quote
+        for the specified instrument.
 
-
-        Args:
-            cex
-            instrument
-
-        Returns:
-            quote
+        :param instrument: The instrument for which the quote is to be fetched.
+        :return: The fetched quote.
         """
         try:
             logger.debug("Instrument: {}", instrument)
             instrument = await self.replace_instrument(instrument)
             logger.debug("Changed Instrument: {}", instrument)
             search_markets = self.client.searching_market(searchTerm=instrument)
             logger.debug("Instrument verification: {}", search_markets)
@@ -98,24 +93,23 @@
             return quote
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
             return e
 
     async def get_bid(self, instrument):
         """
-        Return a quote for a instrument
-        of a given exchange ccxt object
-
+        Asynchronously retrieves the bid
+        for the specified instrument.
 
         Args:
-            cex
-            instrument
+            instrument: The instrument for which
+            the bid is to be retrieved.
 
         Returns:
-            quote
+            The bid for the specified instrument.
         """
         try:
             logger.debug("Instrument: {}", instrument)
             instrument = await self.replace_instrument(instrument)
             logger.debug("Changed Instrument: {}", instrument)
             search_markets = self.client.searching_market(searchTerm=instrument)
             logger.debug("Instrument verification: {}", search_markets)
```

### Comparing `cefi-4.4.7/cefi/handler/ccxt.py` & `cefi-4.4.8/cefi/handler/ccxt.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,30 +51,49 @@
             self.client.set_sandbox_mode("enabled")
         self.account_number = self.client.uid
         self.name = self.client.id
 
 
     async def get_quote(self, instrument):
         """
-        Return a quote for a instrument
-        of a given exchange ccxt object
+        Asynchronously fetches a ask/offer quote
+        for the specified instrument.
 
+        :param instrument: The instrument for which the quote is to be fetched.
+        :return: The fetched quote.
+        """
+        try:
+            instrument = await self.replace_instrument(instrument)
+
+            ticker = self.client.fetch_ticker(instrument)
+            quote = ticker["ask"]
+            logger.debug("Quote: {}", quote)
+            return quote
+        except Exception as e:
+            logger.error("{} Error {}", self.name, e)
+
+
+
+    async def get_bid(self, instrument):
+        """
+        Asynchronously retrieves the bid
+        for the specified instrument.
 
         Args:
-            cex
-            instrument
+            instrument: The instrument for which
+            the bid is to be retrieved.
 
         Returns:
-            quote
+            The bid for the specified instrument.
         """
         try:
             instrument = await self.replace_instrument(instrument)
 
             ticker = self.client.fetch_ticker(instrument)
-            quote = ticker["last"]
+            quote = ticker["bid"]
             logger.debug("Quote: {}", quote)
             return quote
         except Exception as e:
             logger.error("{} Error {}", self.name, e)
 
     async def get_account_balance(self):
         """
```

### Comparing `cefi-4.4.7/cefi/handler/client.py` & `cefi-4.4.8/cefi/handler/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,24 +67,35 @@
             return None
         if not self.enabled:
             logger.debug("{} Not enabled", self.name)
             return
 
     async def get_quote(self, symbol):
         """
-        Return a quote for a symbol
-        of a given exchange ccxt object
+        Asynchronously fetches a ask/offer quote
+        for the specified instrument.
 
+        :param instrument: The instrument for which the quote is to be fetched.
+        :return: The fetched quote.
+        """
+
+    # Alias for get_quote
+    get_offer = get_quote
+
+    async def get_bid(self, instrument):
+        """
+        Asynchronously retrieves the bid
+        for the specified instrument.
 
         Args:
-            cex
-            symbol
+            instrument: The instrument for which
+            the bid is to be retrieved.
 
         Returns:
-            quote
+            The bid for the specified instrument.
         """
 
     async def get_account_balance(self):
         """
         return account balance of
         a given ccxt exchange
```

### Comparing `cefi-4.4.7/cefi/handler/ctrader.py` & `cefi-4.4.8/cefi/handler/ctrader.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.7/cefi/handler/ib_sync.py` & `cefi-4.4.8/cefi/handler/ib_sync.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.7/cefi/main.py` & `cefi-4.4.8/cefi/main.py`

 * *Files identical despite different names*

### Comparing `cefi-4.4.7/pyproject.toml` & `cefi-4.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "cefi"
-version = "4.4.7"
+version = "4.4.8"
 description = "A python library, to interact  with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)"
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["cex, cefi, crypto, exchange, broker"]
 packages = [
     {include = "cefi"}
@@ -144,27 +144,29 @@
 
 
 
 
 
 
 
+
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.23.0"
 pytest-mock = "^3.11.1"
 pytest-loguru = "^0.4.0"
 
 
 
 
 
 
 
+
```

### Comparing `cefi-4.4.7/PKG-INFO` & `cefi-4.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cefi
-Version: 4.4.7
+Version: 4.4.8
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
-Metadata-Version: 2.1 Name: cefi Version: 4.4.7 Summary: A python library, to
+Metadata-Version: 2.1 Name: cefi Version: 4.4.8 Summary: A python library, to
 interact with Crypto Exchanges (CCXT library) and brokers (IB & Capital.com)
 License: MIT Keywords: cex, cefi, crypto, exchange, broker Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: capitalcom-python
```

