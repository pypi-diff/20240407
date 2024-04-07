# Comparing `tmp/alibabacloud_r-kvstore20150101-3.0.0.tar.gz` & `tmp/alibabacloud_r-kvstore20150101-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_r-kvstore20150101-3.0.0.tar", last modified: Sat Mar 30 01:14:51 2024, max compression
+gzip compressed data, was "dist/alibabacloud_r-kvstore20150101-3.0.1.tar", last modified: Sun Apr  7 07:15:06 2024, max compression
```

## Comparing `alibabacloud_r-kvstore20150101-3.0.0.tar` & `alibabacloud_r-kvstore20150101-3.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     2204 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2443 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1204 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   709714 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101/client.py
--rw-r--r--   0 root         (0) root         (0)  1076196 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2443 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2643 2024-03-30 01:14:51.000000 alibabacloud_r-kvstore20150101-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)     2572 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   709714 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1076616 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 07:15:06.000000 alibabacloud_r-kvstore20150101-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2643 2024-04-07 07:15:05.000000 alibabacloud_r-kvstore20150101-3.0.1/setup.py
```

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/ChangeLog.md` & `alibabacloud_r-kvstore20150101-3.0.1/ChangeLog.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2024-03-30 Version: 3.0.0
+- Update API DescribeBackupTasks: update response param.
+- Update API DescribeBackups: update param BackupId.
+- Update API DescribeBackups: update param BackupJobId.
+- Update API DescribeClusterBackupList: update param ClusterBackupId.
+- Update API DescribePrice: update response param.
+- Update API ModifyInstanceSpec: add param NodeType.
+
+
 2024-02-28 Version: 2.25.6
 - Update API DescribeClusterBackupList: update param ClusterBackupId.
 - Update API DescribePrice: update response param.
 
 
 2024-01-30 Version: 2.25.5
 - Update API ModifyBackupPolicyadd BackupRetentionPeriod param.
```

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/LICENSE` & `alibabacloud_r-kvstore20150101-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/PKG-INFO` & `alibabacloud_r-kvstore20150101-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_r-kvstore20150101
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud R-kvstore (20150101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/README-CN.md` & `alibabacloud_r-kvstore20150101-3.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/README.md` & `alibabacloud_r-kvstore20150101-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101/client.py` & `alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101/models.py` & `alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -16622,24 +16622,26 @@
         contract_activity: DescribePriceResponseBodySubOrdersSubOrderDepreciateInfoContractActivity = None,
         differential: int = None,
         differential_name: str = None,
         is_contract_activity: bool = None,
         list_price: int = None,
         month_price: int = None,
         original_stand_amount: int = None,
+        start_time: str = None,
     ):
         self.cheap_rate = cheap_rate
         self.cheap_stand_amount = cheap_stand_amount
         self.contract_activity = contract_activity
         self.differential = differential
         self.differential_name = differential_name
         self.is_contract_activity = is_contract_activity
         self.list_price = list_price
         self.month_price = month_price
         self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
 
     def validate(self):
         if self.contract_activity:
             self.contract_activity.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -16661,14 +16663,16 @@
             result['IsContractActivity'] = self.is_contract_activity
         if self.list_price is not None:
             result['ListPrice'] = self.list_price
         if self.month_price is not None:
             result['MonthPrice'] = self.month_price
         if self.original_stand_amount is not None:
             result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('CheapRate') is not None:
             self.cheap_rate = m.get('CheapRate')
         if m.get('CheapStandAmount') is not None:
@@ -16684,14 +16688,16 @@
             self.is_contract_activity = m.get('IsContractActivity')
         if m.get('ListPrice') is not None:
             self.list_price = m.get('ListPrice')
         if m.get('MonthPrice') is not None:
             self.month_price = m.get('MonthPrice')
         if m.get('OriginalStandAmount') is not None:
             self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
         return self
 
 
 class DescribePriceResponseBodySubOrdersSubOrderModuleInstanceModuleInstanceModuleAttrsModuleAttr(TeaModel):
     def __init__(
         self,
         code: str = None,
@@ -21104,14 +21110,16 @@
     ):
         # The ID of the ApsaraDB for Redis instance.
         self.dbinstance_id = dbinstance_id
         # Specifies the time when the database is switched after data is migrated. Valid values:
         # 
         # *   **Immediately**: immediately switched after the data is migrated.
         # *   **MaintainTime**: switched within the maintenance window.
+        # *   **0**: immediately switched after the data is migrated.
+        # *   **1**: switched within the maintenance window.
         # 
         # >  Default value: **Immediately**.
         self.effective_time = effective_time
         self.owner_account = owner_account
         self.owner_id = owner_id
         self.resource_owner_account = resource_owner_account
         self.resource_owner_id = resource_owner_id
@@ -26797,15 +26805,15 @@
         # 
         # *   **True**: retains the classic network endpoint.
         # *   **False**: does not retain the classic network endpoint.
         # 
         # > This parameter is available only when the network type of the instance is classic network.
         self.retain_classic = retain_classic
         self.security_token = security_token
-        # The network type to which you want to switch. Set the value to **VPC**.
+        # The network type to which you want to switch. If you want to switch to VPC network, Set the value to **VPC**.
         self.target_network_type = target_network_type
         # The ID of the vSwitch that belongs to the VPC to which you want to switch. You can call the [DescribeVpcs](~~35739~~) operation to query the VPC ID.
         # 
         # > The vSwitch and the ApsaraDB for Redis instance must be deployed in the same zone.
         self.v_switch_id = v_switch_id
         # The ID of the VPC to which you want to switch. You can call the [DescribeVpcs](~~35739~~) operation to query the VPC ID.
         #
```

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/alibabacloud_r_kvstore20150101.egg-info/PKG-INFO` & `alibabacloud_r-kvstore20150101-3.0.1/alibabacloud_r_kvstore20150101.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-r-kvstore20150101
-Version: 3.0.0
+Version: 3.0.1
 Summary: Alibaba Cloud R-kvstore (20150101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_r-kvstore20150101-3.0.0/setup.py` & `alibabacloud_r-kvstore20150101-3.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_r-kvstore20150101.
 
-Created on 30/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_r_kvstore20150101"
 NAME = "alibabacloud_r-kvstore20150101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud R-kvstore (20150101) SDK Library for Python"
```

