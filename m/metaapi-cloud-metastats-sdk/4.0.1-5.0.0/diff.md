# Comparing `tmp/metaapi_cloud_metastats_sdk-4.0.1.tar.gz` & `tmp/metaapi_cloud_metastats_sdk-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaapi_cloud_metastats_sdk-4.0.1.tar", last modified: Sat Jan  6 06:37:37 2024, max compression
+gzip compressed data, was "metaapi_cloud_metastats_sdk-5.0.0.tar", last modified: Sun Apr  7 08:56:10 2024, max compression
```

## Comparing `metaapi_cloud_metastats_sdk-4.0.1.tar` & `metaapi_cloud_metastats_sdk-5.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:37:37.715759 metaapi_cloud_metastats_sdk-4.0.1/
--rw-r--r--   0 roman      (501) staff       (20)      781 2023-02-22 08:53:30.000000 metaapi_cloud_metastats_sdk-4.0.1/LICENSE
--rw-r--r--   0 roman      (501) staff       (20)      161 2024-01-06 06:37:18.000000 metaapi_cloud_metastats_sdk-4.0.1/MANIFEST.in
--rw-r--r--   0 roman      (501) staff       (20)     5624 2024-01-06 06:37:37.715585 metaapi_cloud_metastats_sdk-4.0.1/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     4805 2023-11-08 11:17:43.000000 metaapi_cloud_metastats_sdk-4.0.1/README.rst
--rw-r--r--   0 roman      (501) staff       (20)     1025 2024-01-06 06:37:18.000000 metaapi_cloud_metastats_sdk-4.0.1/changelog.md
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:37:37.710123 metaapi_cloud_metastats_sdk-4.0.1/examples/
--rw-r--r--   0 roman      (501) staff       (20)      204 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/examples/README.md
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:37:37.710627 metaapi_cloud_metastats_sdk-4.0.1/examples/exampleGenerator/
--rw-r--r--   0 roman      (501) staff       (20)     1573 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-4.0.1/examples/exampleGenerator/metastats.py
--rw-r--r--   0 roman      (501) staff       (20)       24 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-4.0.1/examples/exampleGenerator/requirements.txt
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:37:37.711258 metaapi_cloud_metastats_sdk-4.0.1/lib/
--rw-r--r--   0 roman      (501) staff       (20)       33 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:37:37.714004 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/
--rw-r--r--   0 roman      (501) staff       (20)        0 2021-06-05 13:27:46.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)     4675 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/domain_client.py
--rw-r--r--   0 roman      (501) staff       (20)     9528 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/domain_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     4575 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/error_handler.py
--rw-r--r--   0 roman      (501) staff       (20)     7963 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/http_client.py
--rw-r--r--   0 roman      (501) staff       (20)    11843 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/http_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     3811 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/metastats_client.py
--rw-r--r--   0 roman      (501) staff       (20)     3871 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/metastats_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)    20730 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/metastats_models.py
--rw-r--r--   0 roman      (501) staff       (20)      364 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/clients/timeout_exception.py
--rw-r--r--   0 roman      (501) staff       (20)     2737 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/metastats.py
--rw-r--r--   0 roman      (501) staff       (20)     1386 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-4.0.1/lib/models.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:37:37.715340 metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)     5624 2024-01-06 06:37:37.000000 metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)      763 2024-01-06 06:37:37.000000 metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2024-01-06 06:37:37.000000 metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)       52 2024-01-06 06:37:37.000000 metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)       28 2024-01-06 06:37:37.000000 metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/top_level.txt
--rw-r--r--   0 roman      (501) staff       (20)       38 2024-01-06 06:37:37.715814 metaapi_cloud_metastats_sdk-4.0.1/setup.cfg
--rw-r--r--   0 roman      (501) staff       (20)     1554 2024-01-06 06:37:18.000000 metaapi_cloud_metastats_sdk-4.0.1/setup.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-07 08:56:10.368853 metaapi_cloud_metastats_sdk-5.0.0/
+-rw-r--r--   0 roman      (501) staff       (20)      781 2023-02-22 08:53:30.000000 metaapi_cloud_metastats_sdk-5.0.0/LICENSE
+-rw-r--r--   0 roman      (501) staff       (20)      161 2024-01-06 06:37:18.000000 metaapi_cloud_metastats_sdk-5.0.0/MANIFEST.in
+-rw-r--r--   0 roman      (501) staff       (20)     5624 2024-04-07 08:56:10.368703 metaapi_cloud_metastats_sdk-5.0.0/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     4805 2023-11-08 11:17:43.000000 metaapi_cloud_metastats_sdk-5.0.0/README.rst
+-rw-r--r--   0 roman      (501) staff       (20)     1087 2024-04-07 08:56:09.000000 metaapi_cloud_metastats_sdk-5.0.0/changelog.md
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-07 08:56:10.364549 metaapi_cloud_metastats_sdk-5.0.0/examples/
+-rw-r--r--   0 roman      (501) staff       (20)      204 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/examples/README.md
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-07 08:56:10.365246 metaapi_cloud_metastats_sdk-5.0.0/examples/exampleGenerator/
+-rw-r--r--   0 roman      (501) staff       (20)     1573 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-5.0.0/examples/exampleGenerator/metastats.py
+-rw-r--r--   0 roman      (501) staff       (20)       24 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-5.0.0/examples/exampleGenerator/requirements.txt
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-07 08:56:10.365906 metaapi_cloud_metastats_sdk-5.0.0/lib/
+-rw-r--r--   0 roman      (501) staff       (20)       33 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-07 08:56:10.367721 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2021-06-05 13:27:46.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)     4675 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/domain_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     9528 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/domain_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     4575 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/error_handler.py
+-rw-r--r--   0 roman      (501) staff       (20)     7963 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/http_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    11843 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/http_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     3811 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/metastats_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     3871 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/metastats_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    20730 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/metastats_models.py
+-rw-r--r--   0 roman      (501) staff       (20)      364 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/clients/timeout_exception.py
+-rw-r--r--   0 roman      (501) staff       (20)     2737 2024-01-05 05:35:59.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/metastats.py
+-rw-r--r--   0 roman      (501) staff       (20)     1386 2024-01-04 14:03:06.000000 metaapi_cloud_metastats_sdk-5.0.0/lib/models.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-04-07 08:56:10.368496 metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/
+-rw-r--r--   0 roman      (501) staff       (20)     5624 2024-04-07 08:56:10.000000 metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)      763 2024-04-07 08:56:10.000000 metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (501) staff       (20)        1 2024-04-07 08:56:10.000000 metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (501) staff       (20)       52 2024-04-07 08:56:10.000000 metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/requires.txt
+-rw-r--r--   0 roman      (501) staff       (20)       28 2024-04-07 08:56:10.000000 metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/top_level.txt
+-rw-r--r--   0 roman      (501) staff       (20)       38 2024-04-07 08:56:10.368899 metaapi_cloud_metastats_sdk-5.0.0/setup.cfg
+-rw-r--r--   0 roman      (501) staff       (20)     1554 2024-04-07 08:56:09.000000 metaapi_cloud_metastats_sdk-5.0.0/setup.py
```

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/LICENSE` & `metaapi_cloud_metastats_sdk-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/PKG-INFO` & `metaapi_cloud_metastats_sdk-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaapi_cloud_metastats_sdk
-Version: 4.0.1
+Version: 5.0.0
 Summary: Python SDK for MetaStats forex trading statistics API. Can calculate metrics for MetaTrader accounts added to MetaApi. Supports both MetaTrader 5 (MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)
 Home-page: https://github.com/metaapi/metaapi-metastats-python-sdk
 Author: MetaApi DMCC
 Author-email: support@metaapi.cloud
 License: SEE LICENSE IN LICENSE
 Keywords: metaapi.cloud,MetaTrader,MetaTrader 5,MetaTrader 4,MetaTrader5,MetaTrader4,MT,MT4,MT5,forex,API,REST,client,sdk,cloud,metrics,MetaStats,metastats
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/README.rst` & `metaapi_cloud_metastats_sdk-5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/changelog.md` & `metaapi_cloud_metastats_sdk-5.0.0/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+5.0.0
+  - breaking change: update httpx dependency to 0.27.0
+
 4.0.1
   - fix broken release
 
 4.0.0
   - breaking change: change modules naming method
   - breaking change: migrate to Python 3.8
   - synchronized with JavaScript SDK 3.5.3
```

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/examples/exampleGenerator/metastats.py` & `metaapi_cloud_metastats_sdk-5.0.0/examples/exampleGenerator/metastats.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/domain_client.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/domain_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/domain_client_test.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/domain_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/error_handler.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/error_handler.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/http_client.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/http_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/http_client_test.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/http_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/metastats_client.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/metastats_client.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/metastats_client_test.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/metastats_client_test.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/clients/metastats_models.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/clients/metastats_models.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/metastats.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/metastats.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/lib/models.py` & `metaapi_cloud_metastats_sdk-5.0.0/lib/models.py`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/PKG-INFO` & `metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaapi-cloud-metastats-sdk
-Version: 4.0.1
+Version: 5.0.0
 Summary: Python SDK for MetaStats forex trading statistics API. Can calculate metrics for MetaTrader accounts added to MetaApi. Supports both MetaTrader 5 (MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)
 Home-page: https://github.com/metaapi/metaapi-metastats-python-sdk
 Author: MetaApi DMCC
 Author-email: support@metaapi.cloud
 License: SEE LICENSE IN LICENSE
 Keywords: metaapi.cloud,MetaTrader,MetaTrader 5,MetaTrader 4,MetaTrader5,MetaTrader4,MT,MT4,MT5,forex,API,REST,client,sdk,cloud,metrics,MetaStats,metastats
 Classifier: Programming Language :: Python :: 3
```

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/metaapi_cloud_metastats_sdk.egg-info/SOURCES.txt` & `metaapi_cloud_metastats_sdk-5.0.0/metaapi_cloud_metastats_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_metastats_sdk-4.0.1/setup.py` & `metaapi_cloud_metastats_sdk-5.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
-install_requires = ['typing-extensions>=4.0.0', 'iso8601', 'pytz', 'httpx==0.23.0']
+install_requires = ['typing-extensions>=4.0.0', 'iso8601', 'pytz', 'httpx==0.27.0']
 
-tests_require = ['pytest==6.2.5', 'pytest-mock==3.8.2', 'pytest-asyncio==0.16.0', 'mock==4.0.3', 'respx==0.19.2',
+tests_require = ['pytest==6.2.5', 'pytest-mock==3.8.2', 'pytest-asyncio==0.16.0', 'mock==4.0.3', 'respx==0.21.1',
                  'freezegun==1.0.0']
 
 setuptools.setup(
     name="metaapi_cloud_metastats_sdk",
-    version="4.0.1",
+    version="5.0.0",
     author="MetaApi DMCC",
     author_email="support@metaapi.cloud",
     description="Python SDK for MetaStats forex trading statistics API. Can calculate metrics for MetaTrader "
                 "accounts added to MetaApi. Supports both MetaTrader 5 (MT5) and MetaTrader 4 (MT4). "
                 "(https://metaapi.cloud)",
     long_description=long_description,
     long_description_content_type="text/x-rst",
```

