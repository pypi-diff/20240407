# Comparing `tmp/alibabacloud_eflo-controller20221215_py2-1.2.1.tar.gz` & `tmp/alibabacloud_eflo-controller20221215_py2-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eflo-controller20221215_py2-1.2.1.tar", last modified: Fri Mar 29 17:16:05 2024, max compression
+gzip compressed data, was "dist/alibabacloud_eflo-controller20221215_py2-1.2.2.tar", last modified: Sun Apr  7 17:10:53 2024, max compression
```

## Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1.tar` & `alibabacloud_eflo-controller20221215_py2-1.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/
--rw-r--r--   0 root         (0) root         (0)     1337 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2544 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1069 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1152 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37136 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215/client.py
--rw-r--r--   0 root         (0) root         (0)   204203 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2544 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      536 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2965 2024-03-29 17:16:05.000000 alibabacloud_eflo-controller20221215_py2-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)     1416 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2544 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1069 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1152 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37136 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215/client.py
+-rw-r--r--   0 root         (0) root         (0)   204892 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2544 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      536 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2965 2024-04-07 17:10:53.000000 alibabacloud_eflo-controller20221215_py2-1.2.2/setup.py
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/ChangeLog.md` & `alibabacloud_eflo-controller20221215_py2-1.2.2/ChangeLog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-29 Version: 1.2.1
+- Update API CreateCluster: update param Networks.
+
+
 2024-03-12 Version: 1.2.0
 - Support API DescribeInvocations.
 - Support API DescribeSendFileResults.
 - Support API RunCommand.
 - Support API SendFile.
 - Support API StopInvocation.
 - Update API CreateCluster: update param NodeGroups.
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/LICENSE` & `alibabacloud_eflo-controller20221215_py2-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/PKG-INFO` & `alibabacloud_eflo-controller20221215_py2-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eflo-controller20221215_py2
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/README-CN.md` & `alibabacloud_eflo-controller20221215_py2-1.2.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/README.md` & `alibabacloud_eflo-controller20221215_py2-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215/client.py` & `alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215/models.py` & `alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1290,21 +1290,23 @@
         if m.get('VpdId') is not None:
             self.vpd_id = m.get('VpdId')
         return self
 
 
 class DescribeClusterResponseBody(TeaModel):
     def __init__(self, cluster_description=None, cluster_id=None, cluster_name=None, cluster_type=None,
-                 components=None, create_time=None, hpn_zone=None, networks=None, node_count=None, node_group_count=None,
-                 operating_state=None, request_id=None, resource_group_id=None, task_id=None, update_time=None, vpc_id=None):
+                 components=None, computing_ip_version=None, create_time=None, hpn_zone=None, networks=None, node_count=None,
+                 node_group_count=None, operating_state=None, request_id=None, resource_group_id=None, task_id=None,
+                 update_time=None, vpc_id=None):
         self.cluster_description = cluster_description  # type: str
         self.cluster_id = cluster_id  # type: str
         self.cluster_name = cluster_name  # type: str
         self.cluster_type = cluster_type  # type: str
         self.components = components  # type: list[DescribeClusterResponseBodyComponents]
+        self.computing_ip_version = computing_ip_version  # type: str
         self.create_time = create_time  # type: str
         self.hpn_zone = hpn_zone  # type: str
         self.networks = networks  # type: list[DescribeClusterResponseBodyNetworks]
         self.node_count = node_count  # type: long
         self.node_group_count = node_group_count  # type: long
         self.operating_state = operating_state  # type: str
         self.request_id = request_id  # type: str
@@ -1337,14 +1339,16 @@
             result['ClusterName'] = self.cluster_name
         if self.cluster_type is not None:
             result['ClusterType'] = self.cluster_type
         result['Components'] = []
         if self.components is not None:
             for k in self.components:
                 result['Components'].append(k.to_map() if k else None)
+        if self.computing_ip_version is not None:
+            result['ComputingIpVersion'] = self.computing_ip_version
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.hpn_zone is not None:
             result['HpnZone'] = self.hpn_zone
         result['Networks'] = []
         if self.networks is not None:
             for k in self.networks:
@@ -1378,14 +1382,16 @@
         if m.get('ClusterType') is not None:
             self.cluster_type = m.get('ClusterType')
         self.components = []
         if m.get('Components') is not None:
             for k in m.get('Components'):
                 temp_model = DescribeClusterResponseBodyComponents()
                 self.components.append(temp_model.from_map(k))
+        if m.get('ComputingIpVersion') is not None:
+            self.computing_ip_version = m.get('ComputingIpVersion')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('HpnZone') is not None:
             self.hpn_zone = m.get('HpnZone')
         self.networks = []
         if m.get('Networks') is not None:
             for k in m.get('Networks'):
@@ -3654,21 +3660,22 @@
         if m.get('ResourceGroupId') is not None:
             self.resource_group_id = m.get('ResourceGroupId')
         return self
 
 
 class ListClustersResponseBodyClusters(TeaModel):
     def __init__(self, cluster_description=None, cluster_id=None, cluster_name=None, cluster_type=None,
-                 components=None, create_time=None, hpn_zone=None, node_count=None, node_group_count=None,
-                 operating_state=None, resource_group_id=None, task_id=None, update_time=None, vpc_id=None):
+                 components=None, computing_ip_version=None, create_time=None, hpn_zone=None, node_count=None,
+                 node_group_count=None, operating_state=None, resource_group_id=None, task_id=None, update_time=None, vpc_id=None):
         self.cluster_description = cluster_description  # type: str
         self.cluster_id = cluster_id  # type: str
         self.cluster_name = cluster_name  # type: str
         self.cluster_type = cluster_type  # type: str
         self.components = components  # type: any
+        self.computing_ip_version = computing_ip_version  # type: str
         self.create_time = create_time  # type: str
         self.hpn_zone = hpn_zone  # type: str
         self.node_count = node_count  # type: long
         self.node_group_count = node_group_count  # type: long
         self.operating_state = operating_state  # type: str
         self.resource_group_id = resource_group_id  # type: str
         self.task_id = task_id  # type: str
@@ -3690,14 +3697,16 @@
             result['ClusterId'] = self.cluster_id
         if self.cluster_name is not None:
             result['ClusterName'] = self.cluster_name
         if self.cluster_type is not None:
             result['ClusterType'] = self.cluster_type
         if self.components is not None:
             result['Components'] = self.components
+        if self.computing_ip_version is not None:
+            result['ComputingIpVersion'] = self.computing_ip_version
         if self.create_time is not None:
             result['CreateTime'] = self.create_time
         if self.hpn_zone is not None:
             result['HpnZone'] = self.hpn_zone
         if self.node_count is not None:
             result['NodeCount'] = self.node_count
         if self.node_group_count is not None:
@@ -3722,14 +3731,16 @@
             self.cluster_id = m.get('ClusterId')
         if m.get('ClusterName') is not None:
             self.cluster_name = m.get('ClusterName')
         if m.get('ClusterType') is not None:
             self.cluster_type = m.get('ClusterType')
         if m.get('Components') is not None:
             self.components = m.get('Components')
+        if m.get('ComputingIpVersion') is not None:
+            self.computing_ip_version = m.get('ComputingIpVersion')
         if m.get('CreateTime') is not None:
             self.create_time = m.get('CreateTime')
         if m.get('HpnZone') is not None:
             self.hpn_zone = m.get('HpnZone')
         if m.get('NodeCount') is not None:
             self.node_count = m.get('NodeCount')
         if m.get('NodeGroupCount') is not None:
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO` & `alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eflo-controller20221215-py2
-Version: 1.2.1
+Version: 1.2.2
 Summary: Alibaba Cloud eflo-controller (20221215) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt` & `alibabacloud_eflo-controller20221215_py2-1.2.2/alibabacloud_eflo_controller20221215_py2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_eflo-controller20221215_py2-1.2.1/setup.py` & `alibabacloud_eflo-controller20221215_py2-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eflo-controller20221215_py2.
 
-Created on 29/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eflo_controller20221215"
 NAME = "alibabacloud_eflo-controller20221215_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud eflo-controller (20221215) SDK Library for Python2"
```

