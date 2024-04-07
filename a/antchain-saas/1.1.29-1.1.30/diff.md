# Comparing `tmp/antchain_saas-1.1.29.tar.gz` & `tmp/antchain_saas-1.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_saas-1.1.29.tar", last modified: Fri Feb  2 07:04:13 2024, max compression
+gzip compressed data, was "dist/antchain_saas-1.1.30.tar", last modified: Sun Apr  7 07:34:17 2024, max compression
```

## Comparing `antchain_saas-1.1.29.tar` & `antchain_saas-1.1.30.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 07:04:13.000000 antchain_saas-1.1.29/
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2169 2024-02-02 07:04:13.000000 antchain_saas-1.1.29/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 07:04:13.000000 antchain_saas-1.1.29/antchain_saas.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2169 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_saas.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_saas.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_saas.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_saas.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_saas.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-02 07:04:13.000000 antchain_saas-1.1.29/antchain_sdk_saas/
--rw-r--r--   0 root         (0) root         (0)       22 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_sdk_saas/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51399 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_sdk_saas/client.py
--rw-r--r--   0 root         (0) root         (0)    92729 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/antchain_sdk_saas/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-02 07:04:13.000000 antchain_saas-1.1.29/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2494 2024-02-02 07:04:12.000000 antchain_saas-1.1.29/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/antchain_saas.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2169 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/antchain_saas.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/antchain_saas.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/antchain_saas.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/antchain_saas.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/antchain_saas.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/antchain_sdk_saas/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/antchain_sdk_saas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51399 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/antchain_sdk_saas/client.py
+-rw-r--r--   0 root         (0) root         (0)    92729 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/antchain_sdk_saas/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 07:34:17.000000 antchain_saas-1.1.30/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2494 2024-04-07 07:34:16.000000 antchain_saas-1.1.30/setup.py
```

### Comparing `antchain_saas-1.1.29/LICENSE` & `antchain_saas-1.1.30/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_saas-1.1.29/PKG-INFO` & `antchain_saas-1.1.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_saas
-Version: 1.1.29
+Version: 1.1.30
 Summary: Ant Chain SAAS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_saas-1.1.29/README-CN.md` & `antchain_saas-1.1.30/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_saas-1.1.29/README.md` & `antchain_saas-1.1.30/README.md`

 * *Files identical despite different names*

### Comparing `antchain_saas-1.1.29/antchain_saas.egg-info/PKG-INFO` & `antchain_saas-1.1.30/antchain_saas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-saas
-Version: 1.1.29
+Version: 1.1.30
 Summary: Ant Chain SAAS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_saas-1.1.29/antchain_sdk_saas/client.py` & `antchain_saas-1.1.30/antchain_sdk_saas/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.29',
+                    'sdk_version': '1.1.30',
                     '_prod_code': 'SAAS',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.1.29',
+                    'sdk_version': '1.1.30',
                     '_prod_code': 'SAAS',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_saas-1.1.29/antchain_sdk_saas/models.py` & `antchain_saas-1.1.30/antchain_sdk_saas/models.py`

 * *Files identical despite different names*

### Comparing `antchain_saas-1.1.29/setup.py` & `antchain_saas-1.1.30/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_saas.
 
-Created on 02/02/2024
+Created on 07/04/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_saas"
 NAME = "antchain_saas" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain SAAS SDK Library for Python"
```

