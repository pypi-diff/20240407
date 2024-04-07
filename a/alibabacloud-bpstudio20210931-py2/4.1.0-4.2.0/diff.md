# Comparing `tmp/alibabacloud_bpstudio20210931_py2-4.1.0.tar.gz` & `tmp/alibabacloud_bpstudio20210931_py2-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-4.1.0.tar", last modified: Tue Feb 27 17:14:31 2024, max compression
+gzip compressed data, was "dist/alibabacloud_bpstudio20210931_py2-4.2.0.tar", last modified: Sun Apr  7 17:09:56 2024, max compression
```

## Comparing `alibabacloud_bpstudio20210931_py2-4.1.0.tar` & `alibabacloud_bpstudio20210931_py2-4.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/
--rw-r--r--   0 root         (0) root         (0)      672 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34566 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931/client.py
--rw-r--r--   0 root         (0) root         (0)   155721 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2024-02-27 17:14:31.000000 alibabacloud_bpstudio20210931_py2-4.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/
+-rw-r--r--   0 root         (0) root         (0)     1019 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34566 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931/client.py
+-rw-r--r--   0 root         (0) root         (0)   156269 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-04-07 17:09:56.000000 alibabacloud_bpstudio20210931_py2-4.2.0/setup.py
```

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/LICENSE` & `alibabacloud_bpstudio20210931_py2-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_bpstudio20210931_py2
-Version: 4.1.0
+Version: 4.2.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/README-CN.md` & `alibabacloud_bpstudio20210931_py2-4.2.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/README.md` & `alibabacloud_bpstudio20210931_py2-4.2.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931/client.py` & `alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931/models.py` & `alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,14 +692,15 @@
         return self
 
 
 class DeployApplicationRequest(TeaModel):
     def __init__(self, application_id=None, client_token=None, resource_group_id=None):
         # The ID of the application.
         self.application_id = application_id  # type: str
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
@@ -830,14 +831,15 @@
         # 
         #     <!-- -->
         # 
         #     { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
         # 
         #     <!-- -->
         self.attributes = attributes  # type: dict[str, any]
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
         # This operation type is the operation type of modifying the product, some operation types are generic, and some are used alone. The following is an example of ECS deployment:
         # - The name of the ECS: rename
         # - Specificationof ecs: modifyInstanceType
         # - Startup of ecs: modifyInstanceType
         # - Stop of ecs: modifyInstanceType
         # - Restart of ecs: modifyInstanceType
@@ -913,14 +915,15 @@
         # 
         #     <!-- -->
         # 
         #     { "ServiceType": "ecs", "Operation": "modifyInstanceType", "Attributes": "{\\"change_type\\":\\"modify_instance_type\\",\\"instance_type\\":\\"ecs.hfr7.2xlarge\\",\\"instanceId\\":\\"i-xxxxxxxxx\\",\\"regionId\\":\\"cn-beijing\\",\\"appId\\":\\"xxxxxxxxxxxxx\\"}" }
         # 
         #     <!-- -->
         self.attributes_shrink = attributes_shrink  # type: str
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
         # This operation type is the operation type of modifying the product, some operation types are generic, and some are used alone. The following is an example of ECS deployment:
         # - The name of the ECS: rename
         # - Specificationof ecs: modifyInstanceType
         # - Startup of ecs: modifyInstanceType
         # - Stop of ecs: modifyInstanceType
         # - Restart of ecs: modifyInstanceType
@@ -3351,14 +3354,15 @@
         return self
 
 
 class ReleaseApplicationRequest(TeaModel):
     def __init__(self, application_id=None, client_token=None, resource_group_id=None):
         # The ID of the application.
         self.application_id = application_id  # type: str
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
         # The ID of the resource.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
@@ -3466,14 +3470,15 @@
         return self
 
 
 class ValidateApplicationRequest(TeaModel):
     def __init__(self, application_id=None, client_token=None, resource_group_id=None):
         # The ID of the application.
         self.application_id = application_id  # type: str
+        # The client token that is used to ensure the idempotence of the request.
         self.client_token = client_token  # type: str
         # The ID of the resource group.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
@@ -3579,18 +3584,19 @@
             temp_model = ValidateApplicationResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class ValuateApplicationRequest(TeaModel):
     def __init__(self, application_id=None, client_token=None, resource_group_id=None):
-        # The ID of the application.
+        # The operation that you want to perform. Set the value to ValuateApplication.
         self.application_id = application_id  # type: str
+        # The ID of the resource group to which the application you want to query belongs.
         self.client_token = client_token  # type: str
-        # The ID of the resource group.
+        # The ID of the application.
         self.resource_group_id = resource_group_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ValuateApplicationRequest, self).to_map()
@@ -3615,21 +3621,21 @@
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class ValuateApplicationResponseBody(TeaModel):
     def __init__(self, code=None, data=None, message=None, request_id=None):
-        # The HTTP status code.
+        # The code of the query task.
         self.code = code  # type: int
-        # The data of the application.
+        # The ID of the request.
         self.data = data  # type: long
-        # The error message.
+        # Idempotent notation
         self.message = message  # type: str
-        # The ID of the request.
+        # The returned message.
         self.request_id = request_id  # type: str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(ValuateApplicationResponseBody, self).to_map()
```

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO` & `alibabacloud_bpstudio20210931_py2-4.2.0/alibabacloud_bpstudio20210931_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-bpstudio20210931-py2
-Version: 4.1.0
+Version: 4.2.0
 Summary: Alibaba Cloud BPStudio (20210931) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_bpstudio20210931_py2-4.1.0/setup.py` & `alibabacloud_bpstudio20210931_py2-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_bpstudio20210931_py2.
 
-Created on 27/02/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_bpstudio20210931"
 NAME = "alibabacloud_bpstudio20210931_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud BPStudio (20210931) SDK Library for Python2"
```

