# Comparing `tmp/alibabacloud_easygene20210315_py2-1.1.0.tar.gz` & `tmp/alibabacloud_easygene20210315_py2-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_easygene20210315_py2-1.1.0.tar", last modified: Tue Jan 30 17:19:17 2024, max compression
+gzip compressed data, was "dist/alibabacloud_easygene20210315_py2-1.1.1.tar", last modified: Sun Apr  7 17:10:38 2024, max compression
```

## Comparing `alibabacloud_easygene20210315_py2-1.1.0.tar` & `alibabacloud_easygene20210315_py2-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/
--rw-r--r--   0 root         (0) root         (0)       99 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2502 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1048 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1131 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315/
--rw-r--r--   0 root         (0) root         (0)       21 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315/__init__.py
--rw-r--r--   0 root         (0) root         (0)    68799 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315/client.py
--rw-r--r--   0 root         (0) root         (0)   363648 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2502 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-01-30 17:19:17.000000 alibabacloud_easygene20210315_py2-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2928 2024-01-30 17:19:16.000000 alibabacloud_easygene20210315_py2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)      155 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1048 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68979 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315/client.py
+-rw-r--r--   0 root         (0) root         (0)   363990 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2502 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      480 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 17:10:38.000000 alibabacloud_easygene20210315_py2-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2928 2024-04-07 17:10:37.000000 alibabacloud_easygene20210315_py2-1.1.1/setup.py
```

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/LICENSE` & `alibabacloud_easygene20210315_py2-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/PKG-INFO` & `alibabacloud_easygene20210315_py2-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_easygene20210315_py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud EasyGene (20210315) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/README-CN.md` & `alibabacloud_easygene20210315_py2-1.1.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/README.md` & `alibabacloud_easygene20210315_py2-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315/client.py` & `alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1538,15 +1538,15 @@
 
     def tag_app(self, request):
         runtime = util_models.RuntimeOptions()
         return self.tag_app_with_options(request, runtime)
 
     def update_entity_with_options(self, tmp_req, runtime):
         """
-        @deprecated
+        @deprecated : UpdateEntity is deprecated, please use EasyGene::2021-03-15::UpdateEntityItems instead.
         
 
         @param tmp_req: UpdateEntityRequest
 
         @param runtime: runtime options for this request RuntimeOptions
 
         @return: UpdateEntityResponse
@@ -1583,15 +1583,15 @@
         return TeaCore.from_map(
             easy_gene_20210315_models.UpdateEntityResponse(),
             self.call_api(params, req, runtime)
         )
 
     def update_entity(self, request):
         """
-        @deprecated
+        @deprecated : UpdateEntity is deprecated, please use EasyGene::2021-03-15::UpdateEntityItems instead.
         
 
         @param request: UpdateEntityRequest
 
         @return: UpdateEntityResponse
         Deprecated
         """
```

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315/models.py` & `alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4009,21 +4009,22 @@
             self.failure_mode = m.get('FailureMode')
         if m.get('UseRelativeOutputPaths') is not None:
             self.use_relative_output_paths = m.get('UseRelativeOutputPaths')
         return self
 
 
 class GetRunResponseBody(TeaModel):
-    def __init__(self, app_name=None, app_revision=None, calls=None, create_time=None, default_runtime=None,
-                 description=None, end_time=None, entity_name=None, entity_type=None, execute_directory=None,
+    def __init__(self, app_name=None, app_revision=None, billing_instance_ids=None, calls=None, create_time=None,
+                 default_runtime=None, description=None, end_time=None, entity_name=None, entity_type=None, execute_directory=None,
                  execute_options=None, failures=None, host_id=None, inputs=None, labels=None, output_folder=None, outputs=None,
                  request_id=None, run_id=None, run_name=None, source=None, start_time=None, status=None, submission_id=None,
                  timing=None, user=None, workspace=None):
         self.app_name = app_name  # type: str
         self.app_revision = app_revision  # type: str
+        self.billing_instance_ids = billing_instance_ids  # type: list[str]
         self.calls = calls  # type: str
         self.create_time = create_time  # type: str
         self.default_runtime = default_runtime  # type: str
         self.description = description  # type: str
         self.end_time = end_time  # type: str
         self.entity_name = entity_name  # type: str
         self.entity_type = entity_type  # type: str
@@ -4056,14 +4057,16 @@
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
@@ -4114,14 +4117,16 @@
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/alibabacloud_easygene20210315_py2.egg-info/PKG-INFO` & `alibabacloud_easygene20210315_py2-1.1.1/alibabacloud_easygene20210315_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-easygene20210315-py2
-Version: 1.1.0
+Version: 1.1.1
 Summary: Alibaba Cloud EasyGene (20210315) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_easygene20210315_py2-1.1.0/setup.py` & `alibabacloud_easygene20210315_py2-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_easygene20210315_py2.
 
-Created on 30/01/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_easygene20210315"
 NAME = "alibabacloud_easygene20210315_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud EasyGene (20210315) SDK Library for Python2"
```

