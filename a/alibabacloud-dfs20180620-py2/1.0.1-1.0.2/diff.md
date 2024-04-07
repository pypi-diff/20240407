# Comparing `tmp/alibabacloud_dfs20180620_py2-1.0.1.tar.gz` & `tmp/alibabacloud_dfs20180620_py2-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dfs20180620_py2-1.0.1.tar", last modified: Fri Mar 29 02:31:58 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dfs20180620_py2-1.0.2.tar", last modified: Sun Apr  7 08:43:47 2024, max compression
```

## Comparing `alibabacloud_dfs20180620_py2-1.0.1.tar` & `alibabacloud_dfs20180620_py2-1.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/
--rw-r--r--   0 root         (0) root         (0)       46 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46343 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620/client.py
--rw-r--r--   0 root         (0) root         (0)   165388 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2024-03-29 02:31:58.000000 alibabacloud_dfs20180620_py2-1.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46343 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620/client.py
+-rw-r--r--   0 root         (0) root         (0)   165373 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2024-04-07 08:43:47.000000 alibabacloud_dfs20180620_py2-1.0.2/setup.py
```

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/LICENSE` & `alibabacloud_dfs20180620_py2-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/PKG-INFO` & `alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620_py2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud_dfs20180620_py2
-Version: 1.0.1
+Name: alibabacloud-dfs20180620-py2
+Version: 1.0.2
 Summary: Alibaba Cloud DFS (20180620) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/README-CN.md` & `alibabacloud_dfs20180620_py2-1.0.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/README.md` & `alibabacloud_dfs20180620_py2-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620/client.py` & `alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620/models.py` & `alibabacloud_dfs20180620_py2-1.0.2/alibabacloud_dfs20180620/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class AttachVscMountPointRequest(TeaModel):
     def __init__(self, description=None, file_system_id=None, input_region_id=None, instance_ids=None,
                  mount_point_id=None, vsc_ids=None, vsc_type=None):
         self.description = description  # type: str
         self.file_system_id = file_system_id  # type: str
         self.input_region_id = input_region_id  # type: str
-        self.instance_ids = instance_ids  # type: dict[str, any]
+        self.instance_ids = instance_ids  # type: list[str]
         self.mount_point_id = mount_point_id  # type: str
         self.vsc_ids = vsc_ids  # type: list[str]
         self.vsc_type = vsc_type  # type: str
 
     def validate(self):
         pass
 
@@ -901,15 +901,15 @@
 
 
 class CreateVscMountPointRequest(TeaModel):
     def __init__(self, description=None, file_system_id=None, input_region_id=None, instance_ids=None):
         self.description = description  # type: str
         self.file_system_id = file_system_id  # type: str
         self.input_region_id = input_region_id  # type: str
-        self.instance_ids = instance_ids  # type: dict[str, any]
+        self.instance_ids = instance_ids  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(CreateVscMountPointRequest, self).to_map()
         if _map is not None:
@@ -2062,15 +2062,15 @@
 
 class DetachVscMountPointRequest(TeaModel):
     def __init__(self, description=None, file_system_id=None, input_region_id=None, instance_ids=None,
                  mount_point_id=None, vsc_ids=None):
         self.description = description  # type: str
         self.file_system_id = file_system_id  # type: str
         self.input_region_id = input_region_id  # type: str
-        self.instance_ids = instance_ids  # type: dict[str, any]
+        self.instance_ids = instance_ids  # type: list[str]
         self.mount_point_id = mount_point_id  # type: str
         self.vsc_ids = vsc_ids  # type: list[str]
 
     def validate(self):
         pass
 
     def to_map(self):
```

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/alibabacloud_dfs20180620_py2.egg-info/PKG-INFO` & `alibabacloud_dfs20180620_py2-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alibabacloud-dfs20180620-py2
-Version: 1.0.1
+Name: alibabacloud_dfs20180620_py2
+Version: 1.0.2
 Summary: Alibaba Cloud DFS (20180620) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dfs20180620_py2-1.0.1/setup.py` & `alibabacloud_dfs20180620_py2-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dfs20180620_py2.
 
-Created on 29/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dfs20180620"
 NAME = "alibabacloud_dfs20180620_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud DFS (20180620) SDK Library for Python2"
```

