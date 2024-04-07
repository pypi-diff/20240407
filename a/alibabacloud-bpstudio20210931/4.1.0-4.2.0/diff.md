# Comparing `tmp/alibabacloud_bpstudio20210931-4.1.0.tar.gz` & `tmp/alibabacloud_bpstudio20210931-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931-4.1.0.tar", last modified: Tue Feb 27 17:22:15 2024, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931-4.2.0.tar", last modified: Sun Apr  7 17:09:58 2024, max compression
```

## Comparing `alibabacloud_bpstudio20210931-4.1.0.tar` & `alibabacloud_bpstudio20210931-4.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/
--rw-r--r--   0 root         (0) root         (0)      939 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81956 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)   155183 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-02-27 17:22:15.000000 alibabacloud_bpstudio20210931-4.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1286 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81956 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)   155731 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-07 17:09:58.000000 alibabacloud_bpstudio20210931-4.2.0/setup.py
```

### Comparing `alibabacloud_bpstudio20210931-4.1.0/LICENSE` & `alibabacloud_bpstudio20210931-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-4.1.0/PKG-INFO` & `alibabacloud_bpstudio20210931-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bpstudio20210931
-Version: 4.1.0
+Version: 4.2.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-4.1.0/README-CN.md` & `alibabacloud_bpstudio20210931-4.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-4.1.0/README.md` & `alibabacloud_bpstudio20210931-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931/models.py` & `alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -791,14 +791,15 @@
         self,
         application_id: str = None,
         client_token: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the application.
         self.application_id = application_id
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
@@ -947,14 +948,15 @@
         # 
         #     <!-- -->
         # 
         #     { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
         # 
         #     <!-- -->
         self.attributes = attributes
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # This operation type is the operation type of modifying the product, some operation types are generic, and some are used alone. The following is an example of ECS deployment:
         # - The name of the ECS: rename
         # - Specificationof ecs: modifyInstanceType
         # - Startup of ecs: modifyInstanceType
         # - Stop of ecs: modifyInstanceType
         # - Restart of ecs: modifyInstanceType
@@ -1037,14 +1039,15 @@
         # 
         #     <!-- -->
         # 
         #     { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
         # 
         #     <!-- -->
         self.attributes_shrink = attributes_shrink
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # This operation type is the operation type of modifying the product, some operation types are generic, and some are used alone. The following is an example of ECS deployment:
         # - The name of the ECS: rename
         # - Specificationof ecs: modifyInstanceType
         # - Startup of ecs: modifyInstanceType
         # - Stop of ecs: modifyInstanceType
         # - Restart of ecs: modifyInstanceType
@@ -3793,14 +3796,15 @@
         self,
         application_id: str = None,
         client_token: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the application.
         self.application_id = application_id
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # The ID of the resource.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
@@ -3924,14 +3928,15 @@
         self,
         application_id: str = None,
         client_token: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the application.
         self.application_id = application_id
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
@@ -4053,18 +4058,19 @@
 class ValuateApplicationRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         client_token: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the application.
+        # The operation that you want to perform. Set the value to ValuateApplication.
         self.application_id = application_id
+        # The ID of the resource group to which the application you want to query belongs.
         self.client_token = client_token
-        # The ID of the resource group.
+        # The ID of the application.
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4095,21 +4101,21 @@
     def __init__(
         self,
         code: int = None,
         data: int = None,
         message: str = None,
         request_id: str = None,
     ):
-        # The HTTP status code.
+        # The code of the query task.
         self.code = code
-        # The data of the application.
+        # The ID of the request.
         self.data = data
-        # The error message.
+        # Idempotent notation
         self.message = message
-        # The ID of the request.
+        # The returned message.
         self.request_id = request_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
```

### Comparing `alibabacloud_bpstudio20210931-4.1.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931-4.2.0/alibabacloud_bpstudio20210931.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bpstudio20210931
-Version: 4.1.0
+Version: 4.2.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931-4.1.0/setup.py` & `alibabacloud_bpstudio20210931-4.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931.
 
-Created on 27/02/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python"
```

