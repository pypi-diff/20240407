# Comparing `tmp/alibabacloud_mse20190531-6.3.0.tar.gz` & `tmp/alibabacloud_mse20190531-6.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_mse20190531-6.3.0.tar", last modified: Thu Mar 14 17:24:31 2024, max compression
+gzip compressed data, was "dist/alibabacloud_mse20190531-6.3.1.tar", last modified: Sun Apr  7 03:15:21 2024, max compression
```

## Comparing `alibabacloud_mse20190531-6.3.0.tar` & `alibabacloud_mse20190531-6.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/
--rw-r--r--   0 root         (0) root         (0)     7746 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2417 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531/__init__.py
--rw-r--r--   0 root         (0) root         (0)   837632 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531/client.py
--rw-r--r--   0 root         (0) root         (0)  2187446 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2417 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2627 2024-03-14 17:24:31.000000 alibabacloud_mse20190531-6.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/
+-rw-r--r--   0 root         (0) root         (0)     8506 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   837632 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531/client.py
+-rw-r--r--   0 root         (0) root         (0)  2187446 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2417 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2627 2024-04-07 03:15:21.000000 alibabacloud_mse20190531-6.3.1/setup.py
```

### Comparing `alibabacloud_mse20190531-6.3.0/LICENSE` & `alibabacloud_mse20190531-6.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-6.3.0/PKG-INFO` & `alibabacloud_mse20190531-6.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_mse20190531
-Version: 6.3.0
+Version: 6.3.1
 Summary: Alibaba Cloud Microservice Engine (20190531) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mse20190531-6.3.0/README-CN.md` & `alibabacloud_mse20190531-6.3.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-6.3.0/README.md` & `alibabacloud_mse20190531-6.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531/client.py` & `alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531/models.py` & `alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_mse20190531-6.3.0/alibabacloud_mse20190531.egg-info/PKG-INFO` & `alibabacloud_mse20190531-6.3.1/alibabacloud_mse20190531.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-mse20190531
-Version: 6.3.0
+Version: 6.3.1
 Summary: Alibaba Cloud Microservice Engine (20190531) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_mse20190531-6.3.0/setup.py` & `alibabacloud_mse20190531-6.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_mse20190531.
 
-Created on 14/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_mse20190531"
 NAME = "alibabacloud_mse20190531" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Microservice Engine (20190531) SDK Library for Python"
```

