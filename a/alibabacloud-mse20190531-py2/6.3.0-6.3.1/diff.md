# Comparing `tmp/alibabacloud_mse20190531_py2-6.3.0.tar.gz` & `tmp/alibabacloud_mse20190531_py2-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mse20190531_py2-6.3.0.tar", last modified: Thu Mar 14 17:20:19 2024, max compression
+gzip compressed data, was "dist/alibabacloud_mse20190531_py2-6.3.1.tar", last modified: Sun Apr  7 03:15:06 2024, max compression
```

## Comparing `alibabacloud_mse20190531_py2-6.3.0.tar` & `alibabacloud_mse20190531_py2-6.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/
--rw-r--r--   0 root         (0) root         (0)     6738 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2488 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531/__init__.py
--rw-r--r--   0 root         (0) root         (0)   357346 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531/client.py
--rw-r--r--   0 root         (0) root         (0)  2199466 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2488 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2919 2024-03-14 17:20:19.000000 alibabacloud_mse20190531_py2-6.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/
+-rw-r--r--   0 root         (0) root         (0)     7498 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   357346 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531/client.py
+-rw-r--r--   0 root         (0) root         (0)  2199466 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2488 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2919 2024-04-07 03:15:06.000000 alibabacloud_mse20190531_py2-6.3.1/setup.py
```

### Comparing `alibabacloud_mse20190531_py2-6.3.0/ChangeLog.md` & `alibabacloud_mse20190531_py2-6.3.1/ChangeLog.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+2024-03-14 Version: 6.3.0
+- Support API AddGatewayAuth.
+- Support API CreateIsolationRule.
+- Support API DeleteIsolationRules.
+- Support API GetGatewayAuthDetail.
+- Support API ListIsolationRules.
+- Support API UpdateIsolationRule.
+- Update API CreateOrUpdateSwimmingLane: update param GatewaySwimmingLaneRouteJson.
+- Update API CreateOrUpdateSwimmingLaneGroup: add param CanaryModel.
+- Update API CreateOrUpdateSwimmingLaneGroup: add param Paths.
+- Update API CreateOrUpdateSwimmingLaneGroup: add param RouteIds.
+- Update API CreateOrUpdateSwimmingLaneGroup: update response param.
+- Update API ListClusterTypes: update response param.
+- Update API QueryAllSwimmingLane: update response param.
+- Update API QueryAllSwimmingLaneGroup: update response param.
+
+
 2024-02-29 Version: 6.2.0
 - Support API AddGatewayAuth.
 - Support API CreateIsolationRule.
 - Support API DeleteIsolationRules.
 - Support API GetGatewayAuthDetail.
 - Support API ListIsolationRules.
 - Support API UpdateIsolationRule.
```

### Comparing `alibabacloud_mse20190531_py2-6.3.0/LICENSE` & `alibabacloud_mse20190531_py2-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531_py2-6.3.0/PKG-INFO` & `alibabacloud_mse20190531_py2-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mse20190531_py2
-Version: 6.3.0
+Version: 6.3.1
 Summary: Alibaba Cloud Microservice Engine (20190531) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mse20190531_py2-6.3.0/README-CN.md` & `alibabacloud_mse20190531_py2-6.3.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531_py2-6.3.0/README.md` & `alibabacloud_mse20190531_py2-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531/client.py` & `alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531/models.py` & `alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531_py2-6.3.0/alibabacloud_mse20190531_py2.egg-info/PKG-INFO` & `alibabacloud_mse20190531_py2-6.3.1/alibabacloud_mse20190531_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mse20190531-py2
-Version: 6.3.0
+Version: 6.3.1
 Summary: Alibaba Cloud Microservice Engine (20190531) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mse20190531_py2-6.3.0/setup.py` & `alibabacloud_mse20190531_py2-6.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mse20190531_py2.
 
-Created on 14/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mse20190531"
 NAME = "alibabacloud_mse20190531_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Microservice Engine (20190531) SDK Library for Python2"
```

