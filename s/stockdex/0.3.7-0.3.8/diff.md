# Comparing `tmp/stockdex-0.3.7.tar.gz` & `tmp/stockdex-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockdex-0.3.7.tar", last modified: Sun Apr  7 10:05:58 2024, max compression
+gzip compressed data, was "stockdex-0.3.8.tar", last modified: Sun Apr  7 10:34:36 2024, max compression
```

## Comparing `stockdex-0.3.7.tar` & `stockdex-0.3.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.093271 stockdex-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:05:58.093271 stockdex-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-07 10:05:50.000000 stockdex-0.3.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:05:58.093271 stockdex-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-07 10:05:50.000000 stockdex-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.089271 stockdex-0.3.7/stockdex/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/selenium_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:50.000000 stockdex-0.3.7/stockdex/ticker_etf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.093271 stockdex-0.3.7/stockdex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 10:05:58.000000 stockdex-0.3.7/stockdex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:58.093271 stockdex-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_justetf.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_nasdaq_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_ticker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-07 10:05:50.000000 stockdex-0.3.7/tests/test_ticker_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:34:36.577845 stockdex-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-07 10:34:28.000000 stockdex-0.3.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:34:36.577845 stockdex-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-07 10:34:28.000000 stockdex-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/stockdex/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14539 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8463 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/justetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/selenium_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15771 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:28.000000 stockdex-0.3.8/stockdex/ticker_etf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/stockdex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 10:34:36.000000 stockdex-0.3.8/stockdex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:36.577845 stockdex-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4053 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_justetf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_nasdaq_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_ticker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-04-07 10:34:28.000000 stockdex-0.3.8/tests/test_ticker_api.py
```

### Comparing `stockdex-0.3.7/PKG-INFO` & `stockdex-0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.3.7
+Version: 0.3.8
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `stockdex-0.3.7/README.md` & `stockdex-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/config.py` & `stockdex-0.3.8/stockdex/config.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/justetf.py` & `stockdex-0.3.8/stockdex/justetf.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/lib.py` & `stockdex-0.3.8/stockdex/lib.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/nasdaq_interface.py` & `stockdex-0.3.8/stockdex/nasdaq_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/selenium_interface.py` & `stockdex-0.3.8/stockdex/selenium_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/ticker.py` & `stockdex-0.3.8/stockdex/ticker.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/ticker_api.py` & `stockdex-0.3.8/stockdex/ticker_api.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex/ticker_base.py` & `stockdex-0.3.8/stockdex/ticker_base.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/stockdex.egg-info/PKG-INFO` & `stockdex-0.3.8/stockdex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stockdex
-Version: 0.3.7
+Version: 0.3.8
 Summary: A package to get stock data from Yahoo Finance
 Home-page: https://github.com/ahnazary/stockdex
 Author: Amir Nazary
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `stockdex-0.3.7/stockdex.egg-info/SOURCES.txt` & `stockdex-0.3.8/stockdex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/tests/test_justetf.py` & `stockdex-0.3.8/tests/test_justetf.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/tests/test_nasdaq_interface.py` & `stockdex-0.3.8/tests/test_nasdaq_interface.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/tests/test_ticker.py` & `stockdex-0.3.8/tests/test_ticker.py`

 * *Files identical despite different names*

### Comparing `stockdex-0.3.7/tests/test_ticker_api.py` & `stockdex-0.3.8/tests/test_ticker_api.py`

 * *Files identical despite different names*

