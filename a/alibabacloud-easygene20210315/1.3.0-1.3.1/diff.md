# Comparing `tmp/alibabacloud_easygene20210315-1.3.0.tar.gz` & `tmp/alibabacloud_easygene20210315-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_easygene20210315-1.3.0.tar", last modified: Tue Jan 30 17:18:03 2024, max compression
+gzip compressed data, was "dist/alibabacloud_easygene20210315-1.3.1.tar", last modified: Sun Apr  7 17:11:07 2024, max compression
```

## Comparing `alibabacloud_easygene20210315-1.3.0.tar` & `alibabacloud_easygene20210315-1.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      305 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315/__init__.py
--rw-r--r--   0 root         (0) root         (0)   167395 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315/client.py
--rw-r--r--   0 root         (0) root         (0)   362357 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-01-30 17:18:03.000000 alibabacloud_easygene20210315-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)      361 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   167755 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315/client.py
+-rw-r--r--   0 root         (0) root         (0)   362701 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-04-07 17:11:07.000000 alibabacloud_easygene20210315-1.3.1/setup.py
```

### Comparing `alibabacloud_easygene20210315-1.3.0/LICENSE` & `alibabacloud_easygene20210315-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_easygene20210315-1.3.0/PKG-INFO` & `alibabacloud_easygene20210315-1.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_easygene20210315
-Version: 1.3.0
+Version: 1.3.1
 Summary: Alibaba Cloud EasyGene (20210315) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_easygene20210315-1.3.0/README-CN.md` & `alibabacloud_easygene20210315-1.3.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_easygene20210315-1.3.0/README.md` & `alibabacloud_easygene20210315-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315/client.py` & `alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3699,15 +3699,15 @@
 
     def update_entity_with_options(
         self,
         tmp_req: easy_gene_20210315_models.UpdateEntityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> easy_gene_20210315_models.UpdateEntityResponse:
         """
-        @deprecated
+        @deprecated : UpdateEntity is deprecated, please use EasyGene::2021-03-15::UpdateEntityItems instead.
         
         @param tmp_req: UpdateEntityRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateEntityResponse
         Deprecated
         """
         UtilClient.validate_model(tmp_req)
@@ -3745,15 +3745,15 @@
 
     async def update_entity_with_options_async(
         self,
         tmp_req: easy_gene_20210315_models.UpdateEntityRequest,
         runtime: util_models.RuntimeOptions,
     ) -> easy_gene_20210315_models.UpdateEntityResponse:
         """
-        @deprecated
+        @deprecated : UpdateEntity is deprecated, please use EasyGene::2021-03-15::UpdateEntityItems instead.
         
         @param tmp_req: UpdateEntityRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpdateEntityResponse
         Deprecated
         """
         UtilClient.validate_model(tmp_req)
@@ -3790,29 +3790,29 @@
         )
 
     def update_entity(
         self,
         request: easy_gene_20210315_models.UpdateEntityRequest,
     ) -> easy_gene_20210315_models.UpdateEntityResponse:
         """
-        @deprecated
+        @deprecated : UpdateEntity is deprecated, please use EasyGene::2021-03-15::UpdateEntityItems instead.
         
         @param request: UpdateEntityRequest
         @return: UpdateEntityResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         return self.update_entity_with_options(request, runtime)
 
     async def update_entity_async(
         self,
         request: easy_gene_20210315_models.UpdateEntityRequest,
     ) -> easy_gene_20210315_models.UpdateEntityResponse:
         """
-        @deprecated
+        @deprecated : UpdateEntity is deprecated, please use EasyGene::2021-03-15::UpdateEntityItems instead.
         
         @param request: UpdateEntityRequest
         @return: UpdateEntityResponse
         Deprecated
         """
         runtime = util_models.RuntimeOptions()
         return await self.update_entity_with_options_async(request, runtime)
```

### Comparing `alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315/models.py` & `alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4582,14 +4582,15 @@
 
 
 class GetRunResponseBody(TeaModel):
     def __init__(
         self,
         app_name: str = None,
         app_revision: str = None,
+        billing_instance_ids: List[str] = None,
         calls: str = None,
         create_time: str = None,
         default_runtime: str = None,
         description: str = None,
         end_time: str = None,
         entity_name: str = None,
         entity_type: str = None,
@@ -4610,14 +4611,15 @@
         submission_id: str = None,
         timing: str = None,
         user: str = None,
         workspace: str = None,
     ):
         self.app_name = app_name
         self.app_revision = app_revision
+        self.billing_instance_ids = billing_instance_ids
         self.calls = calls
         self.create_time = create_time
         self.default_runtime = default_runtime
         self.description = description
         self.end_time = end_time
         self.entity_name = entity_name
         self.entity_type = entity_type
@@ -4650,14 +4652,16 @@
             return _map
 
         result = dict()
         if self.app_name is not None:
             result['AppName'] = self.app_name
         if self.app_revision is not None:
             result['AppRevision'] = self.app_revision
+        if self.billing_instance_ids is not None:
+            result['BillingInstanceIds'] = self.billing_instance_ids
         if self.calls is not None:
             result['Calls'] = self.calls
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.default_runtime is not None:
             result['DefaultRuntime'] = self.default_runtime
         if self.description is not None:
@@ -4708,14 +4712,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('AppName') is not None:
             self.app_name = m.get('AppName')
         if m.get('AppRevision') is not None:
             self.app_revision = m.get('AppRevision')
+        if m.get('BillingInstanceIds') is not None:
+            self.billing_instance_ids = m.get('BillingInstanceIds')
         if m.get('Calls') is not None:
             self.calls = m.get('Calls')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('DefaultRuntime') is not None:
             self.default_runtime = m.get('DefaultRuntime')
         if m.get('Description') is not None:
```

### Comparing `alibabacloud_easygene20210315-1.3.0/alibabacloud_easygene20210315.egg-info/PKG-INFO` & `alibabacloud_easygene20210315-1.3.1/alibabacloud_easygene20210315.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-easygene20210315
-Version: 1.3.0
+Version: 1.3.1
 Summary: Alibaba Cloud EasyGene (20210315) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_easygene20210315-1.3.0/setup.py` & `alibabacloud_easygene20210315-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_easygene20210315.
 
-Created on 30/01/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_easygene20210315"
 NAME = "alibabacloud_easygene20210315" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud EasyGene (20210315) SDK Library for Python"
```

