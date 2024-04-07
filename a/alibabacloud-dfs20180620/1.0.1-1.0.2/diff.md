# Comparing `tmp/alibabacloud_dfs20180620-1.0.1.tar.gz` & `tmp/alibabacloud_dfs20180620-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dfs20180620-1.0.1.tar", last modified: Fri Mar 29 02:32:57 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dfs20180620-1.0.2.tar", last modified: Sun Apr  7 08:43:12 2024, max compression
```

## Comparing `alibabacloud_dfs20180620-1.0.1.tar` & `alibabacloud_dfs20180620-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       46 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620/__init__.py
--rw-r--r--   0 root         (0) root         (0)   109474 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620/client.py
--rw-r--r--   0 root         (0) root         (0)   164482 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2401 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 02:32:57.000000 alibabacloud_dfs20180620-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2611 2024-03-29 02:32:56.000000 alibabacloud_dfs20180620-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   109474 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620/client.py
+-rw-r--r--   0 root         (0) root         (0)   164467 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2401 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2611 2024-04-07 08:43:12.000000 alibabacloud_dfs20180620-1.0.2/setup.py
```

### Comparing `alibabacloud_dfs20180620-1.0.1/LICENSE` & `alibabacloud_dfs20180620-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620-1.0.1/PKG-INFO` & `alibabacloud_dfs20180620-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dfs20180620
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud DFS (20180620) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dfs20180620-1.0.1/README-CN.md` & `alibabacloud_dfs20180620-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620-1.0.1/README.md` & `alibabacloud_dfs20180620-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620/client.py` & `alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620/models.py` & `alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # -*- coding: utf-8 -*-
 # This file is auto-generated, don't edit it. Thanks.
 from Tea.model import TeaModel
-from typing import Dict, Any, List
+from typing import List, Dict, Any
 
 
 class AttachVscMountPointRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         file_system_id: str = None,
         input_region_id: str = None,
-        instance_ids: Dict[str, Any] = None,
+        instance_ids: List[str] = None,
         mount_point_id: str = None,
         vsc_ids: List[str] = None,
         vsc_type: str = None,
     ):
         self.description = description
         self.file_system_id = file_system_id
         self.input_region_id = input_region_id
@@ -1031,15 +1031,15 @@
 
 class CreateVscMountPointRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         file_system_id: str = None,
         input_region_id: str = None,
-        instance_ids: Dict[str, Any] = None,
+        instance_ids: List[str] = None,
     ):
         self.description = description
         self.file_system_id = file_system_id
         self.input_region_id = input_region_id
         self.instance_ids = instance_ids
 
     def validate(self):
@@ -2349,15 +2349,15 @@
 
 class DetachVscMountPointRequest(TeaModel):
     def __init__(
         self,
         description: str = None,
         file_system_id: str = None,
         input_region_id: str = None,
-        instance_ids: Dict[str, Any] = None,
+        instance_ids: List[str] = None,
         mount_point_id: str = None,
         vsc_ids: List[str] = None,
     ):
         self.description = description
         self.file_system_id = file_system_id
         self.input_region_id = input_region_id
         self.instance_ids = instance_ids
```

### Comparing `alibabacloud_dfs20180620-1.0.1/alibabacloud_dfs20180620.egg-info/PKG-INFO` & `alibabacloud_dfs20180620-1.0.2/alibabacloud_dfs20180620.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dfs20180620
-Version: 1.0.1
+Version: 1.0.2
 Summary: Alibaba Cloud DFS (20180620) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dfs20180620-1.0.1/setup.py` & `alibabacloud_dfs20180620-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dfs20180620.
 
-Created on 29/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dfs20180620"
 NAME = "alibabacloud_dfs20180620" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud DFS (20180620) SDK Library for Python"
```

