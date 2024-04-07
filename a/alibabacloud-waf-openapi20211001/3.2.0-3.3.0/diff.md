# Comparing `tmp/alibabacloud_waf-openapi20211001-3.2.0.tar.gz` & `tmp/alibabacloud_waf-openapi20211001-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_waf-openapi20211001-3.2.0.tar", last modified: Thu Mar 28 17:18:13 2024, max compression
+gzip compressed data, was "dist/alibabacloud_waf-openapi20211001-3.3.0.tar", last modified: Sun Apr  7 03:49:29 2024, max compression
```

## Comparing `alibabacloud_waf-openapi20211001-3.2.0.tar` & `alibabacloud_waf-openapi20211001-3.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/
--rw-r--r--   0 root         (0) root         (0)     1367 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001/__init__.py
--rw-r--r--   0 root         (0) root         (0)   278542 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001/client.py
--rw-r--r--   0 root         (0) root         (0)   554625 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2653 2024-03-28 17:18:13.000000 alibabacloud_waf-openapi20211001-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   294088 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/client.py
+-rw-r--r--   0 root         (0) root         (0)   585958 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 03:49:29.000000 alibabacloud_waf-openapi20211001-3.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2653 2024-04-07 03:49:28.000000 alibabacloud_waf-openapi20211001-3.3.0/setup.py
```

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/ChangeLog.md` & `alibabacloud_waf-openapi20211001-3.3.0/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+2024-03-28 Version: 3.2.0
+- Support API DescribeCerts.
+- Support API DescribeDomainDNSRecord.
+- Support API DescribeResourceRegionId.
+- Support API DescribeResourceSupportRegions.
+- Support API ModifyDefenseResourceXff.
+- Support API ModifyDefenseRuleCache.
+
+
 2024-03-26 Version: 3.1.0
 - Support API CreateMemberAccounts.
 - Support API DeleteMemberAccount.
 - Support API DescribeAccountDelegatedStatus.
 - Support API DescribeDefenseResourceTemplates.
 - Support API DescribeDefenseTemplates.
 - Support API DescribeMemberAccounts.
```

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/LICENSE` & `alibabacloud_waf-openapi20211001-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/PKG-INFO` & `alibabacloud_waf-openapi20211001-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_waf-openapi20211001
-Version: 3.2.0
+Version: 3.3.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/README-CN.md` & `alibabacloud_waf-openapi20211001-3.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/README.md` & `alibabacloud_waf-openapi20211001-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001/client.py` & `alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1431,14 +1431,132 @@
     async def describe_certs_async(
         self,
         request: waf_openapi_20211001_models.DescribeCertsRequest,
     ) -> waf_openapi_20211001_models.DescribeCertsResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_certs_with_options_async(request, runtime)
 
+    def describe_cloud_resources_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeCloudResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeCloudResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.owner_user_id):
+            query['OwnerUserId'] = request.owner_user_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_domain):
+            query['ResourceDomain'] = request.resource_domain
+        if not UtilClient.is_unset(request.resource_function):
+            query['ResourceFunction'] = request.resource_function
+        if not UtilClient.is_unset(request.resource_instance_id):
+            query['ResourceInstanceId'] = request.resource_instance_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.resource_name):
+            query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.resource_product):
+            query['ResourceProduct'] = request.resource_product
+        if not UtilClient.is_unset(request.resource_region_id):
+            query['ResourceRegionId'] = request.resource_region_id
+        if not UtilClient.is_unset(request.resource_route_name):
+            query['ResourceRouteName'] = request.resource_route_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeCloudResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeCloudResourcesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_cloud_resources_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeCloudResourcesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeCloudResourcesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.owner_user_id):
+            query['OwnerUserId'] = request.owner_user_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_domain):
+            query['ResourceDomain'] = request.resource_domain
+        if not UtilClient.is_unset(request.resource_function):
+            query['ResourceFunction'] = request.resource_function
+        if not UtilClient.is_unset(request.resource_instance_id):
+            query['ResourceInstanceId'] = request.resource_instance_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.resource_name):
+            query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.resource_product):
+            query['ResourceProduct'] = request.resource_product
+        if not UtilClient.is_unset(request.resource_region_id):
+            query['ResourceRegionId'] = request.resource_region_id
+        if not UtilClient.is_unset(request.resource_route_name):
+            query['ResourceRouteName'] = request.resource_route_name
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeCloudResources',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeCloudResourcesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_cloud_resources(
+        self,
+        request: waf_openapi_20211001_models.DescribeCloudResourcesRequest,
+    ) -> waf_openapi_20211001_models.DescribeCloudResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cloud_resources_with_options(request, runtime)
+
+    async def describe_cloud_resources_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeCloudResourcesRequest,
+    ) -> waf_openapi_20211001_models.DescribeCloudResourcesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_cloud_resources_with_options_async(request, runtime)
+
     def describe_defense_resource_group_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeDefenseResourceGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeDefenseResourceGroupResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -3235,14 +3353,124 @@
     async def describe_peak_trend_async(
         self,
         request: waf_openapi_20211001_models.DescribePeakTrendRequest,
     ) -> waf_openapi_20211001_models.DescribePeakTrendResponse:
         runtime = util_models.RuntimeOptions()
         return await self.describe_peak_trend_with_options_async(request, runtime)
 
+    def describe_product_instances_with_options(
+        self,
+        request: waf_openapi_20211001_models.DescribeProductInstancesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeProductInstancesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.owner_user_id):
+            query['OwnerUserId'] = request.owner_user_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_instance_id):
+            query['ResourceInstanceId'] = request.resource_instance_id
+        if not UtilClient.is_unset(request.resource_ip):
+            query['ResourceIp'] = request.resource_ip
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.resource_name):
+            query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.resource_product):
+            query['ResourceProduct'] = request.resource_product
+        if not UtilClient.is_unset(request.resource_region_id):
+            query['ResourceRegionId'] = request.resource_region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeProductInstances',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeProductInstancesResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def describe_product_instances_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeProductInstancesRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.DescribeProductInstancesResponse:
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.owner_user_id):
+            query['OwnerUserId'] = request.owner_user_id
+        if not UtilClient.is_unset(request.page_number):
+            query['PageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['PageSize'] = request.page_size
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_instance_id):
+            query['ResourceInstanceId'] = request.resource_instance_id
+        if not UtilClient.is_unset(request.resource_ip):
+            query['ResourceIp'] = request.resource_ip
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        if not UtilClient.is_unset(request.resource_name):
+            query['ResourceName'] = request.resource_name
+        if not UtilClient.is_unset(request.resource_product):
+            query['ResourceProduct'] = request.resource_product
+        if not UtilClient.is_unset(request.resource_region_id):
+            query['ResourceRegionId'] = request.resource_region_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='DescribeProductInstances',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.DescribeProductInstancesResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def describe_product_instances(
+        self,
+        request: waf_openapi_20211001_models.DescribeProductInstancesRequest,
+    ) -> waf_openapi_20211001_models.DescribeProductInstancesResponse:
+        runtime = util_models.RuntimeOptions()
+        return self.describe_product_instances_with_options(request, runtime)
+
+    async def describe_product_instances_async(
+        self,
+        request: waf_openapi_20211001_models.DescribeProductInstancesRequest,
+    ) -> waf_openapi_20211001_models.DescribeProductInstancesResponse:
+        runtime = util_models.RuntimeOptions()
+        return await self.describe_product_instances_with_options_async(request, runtime)
+
     def describe_resource_instance_certs_with_options(
         self,
         request: waf_openapi_20211001_models.DescribeResourceInstanceCertsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> waf_openapi_20211001_models.DescribeResourceInstanceCertsResponse:
         UtilClient.validate_model(request)
         query = {}
@@ -6308,7 +6536,111 @@
 
     async def modify_template_resources_async(
         self,
         request: waf_openapi_20211001_models.ModifyTemplateResourcesRequest,
     ) -> waf_openapi_20211001_models.ModifyTemplateResourcesResponse:
         runtime = util_models.RuntimeOptions()
         return await self.modify_template_resources_with_options_async(request, runtime)
+
+    def sync_product_instance_with_options(
+        self,
+        request: waf_openapi_20211001_models.SyncProductInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.SyncProductInstanceResponse:
+        """
+        SyncProductInstance is an asynchronous operation. You can call the [DescribeProductInstances](~~2743168~~) operation to query the status of the task.
+        
+        @param request: SyncProductInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SyncProductInstanceResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SyncProductInstance',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.SyncProductInstanceResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def sync_product_instance_with_options_async(
+        self,
+        request: waf_openapi_20211001_models.SyncProductInstanceRequest,
+        runtime: util_models.RuntimeOptions,
+    ) -> waf_openapi_20211001_models.SyncProductInstanceResponse:
+        """
+        SyncProductInstance is an asynchronous operation. You can call the [DescribeProductInstances](~~2743168~~) operation to query the status of the task.
+        
+        @param request: SyncProductInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SyncProductInstanceResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.instance_id):
+            query['InstanceId'] = request.instance_id
+        if not UtilClient.is_unset(request.region_id):
+            query['RegionId'] = request.region_id
+        if not UtilClient.is_unset(request.resource_manager_resource_group_id):
+            query['ResourceManagerResourceGroupId'] = request.resource_manager_resource_group_id
+        req = open_api_models.OpenApiRequest(
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='SyncProductInstance',
+            version='2021-10-01',
+            protocol='HTTPS',
+            pathname='/',
+            method='POST',
+            auth_type='AK',
+            style='RPC',
+            req_body_type='formData',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            waf_openapi_20211001_models.SyncProductInstanceResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def sync_product_instance(
+        self,
+        request: waf_openapi_20211001_models.SyncProductInstanceRequest,
+    ) -> waf_openapi_20211001_models.SyncProductInstanceResponse:
+        """
+        SyncProductInstance is an asynchronous operation. You can call the [DescribeProductInstances](~~2743168~~) operation to query the status of the task.
+        
+        @param request: SyncProductInstanceRequest
+        @return: SyncProductInstanceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.sync_product_instance_with_options(request, runtime)
+
+    async def sync_product_instance_async(
+        self,
+        request: waf_openapi_20211001_models.SyncProductInstanceRequest,
+    ) -> waf_openapi_20211001_models.SyncProductInstanceResponse:
+        """
+        SyncProductInstance is an asynchronous operation. You can call the [DescribeProductInstances](~~2743168~~) operation to query the status of the task.
+        
+        @param request: SyncProductInstanceRequest
+        @return: SyncProductInstanceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return await self.sync_product_instance_with_options_async(request, runtime)
```

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001/models.py` & `alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2647,14 +2647,320 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCertsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCloudResourcesRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        owner_user_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        resource_domain: str = None,
+        resource_function: str = None,
+        resource_instance_id: str = None,
+        resource_manager_resource_group_id: str = None,
+        resource_name: str = None,
+        resource_product: str = None,
+        resource_region_id: str = None,
+        resource_route_name: str = None,
+    ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The ID of the Alibaba Cloud account to which the resource belongs.
+        self.owner_user_id = owner_user_id
+        # The page number. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries per page. Default value: **10**.
+        self.page_size = page_size
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The domain name. You can use this parameter if you set ResourceProduct to fc or sae.
+        self.resource_domain = resource_domain
+        # The function name. You can use this parameter if you set ResourceProduct to fc.
+        self.resource_function = resource_function
+        # The ID of the resource.
+        self.resource_instance_id = resource_instance_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The name of the resource.
+        self.resource_name = resource_name
+        # The cloud service to which the resource belongs. Valid values:
+        # 
+        # *   **alb**: Application Load Balancer (ALB).
+        # *   **mse**: Microservices Engine (MSE).
+        # *   **fc**: Function Compute.
+        # *   **sae**: Serverless App Engine (SAE).
+        # 
+        # >  Different cloud services are available in different regions. The specified cloud service must be available in the specified region.
+        self.resource_product = resource_product
+        # The region ID of the resource. For information about region IDs, see the following table.
+        # 
+        # >  Different cloud services are available in different regions. The specified cloud service must be available in the specified region.
+        self.resource_region_id = resource_region_id
+        # The route name. You can use this parameter if you set ResourceProduct to mse.
+        self.resource_route_name = resource_route_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.owner_user_id is not None:
+            result['OwnerUserId'] = self.owner_user_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_domain is not None:
+            result['ResourceDomain'] = self.resource_domain
+        if self.resource_function is not None:
+            result['ResourceFunction'] = self.resource_function
+        if self.resource_instance_id is not None:
+            result['ResourceInstanceId'] = self.resource_instance_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.resource_product is not None:
+            result['ResourceProduct'] = self.resource_product
+        if self.resource_region_id is not None:
+            result['ResourceRegionId'] = self.resource_region_id
+        if self.resource_route_name is not None:
+            result['ResourceRouteName'] = self.resource_route_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('OwnerUserId') is not None:
+            self.owner_user_id = m.get('OwnerUserId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceDomain') is not None:
+            self.resource_domain = m.get('ResourceDomain')
+        if m.get('ResourceFunction') is not None:
+            self.resource_function = m.get('ResourceFunction')
+        if m.get('ResourceInstanceId') is not None:
+            self.resource_instance_id = m.get('ResourceInstanceId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('ResourceProduct') is not None:
+            self.resource_product = m.get('ResourceProduct')
+        if m.get('ResourceRegionId') is not None:
+            self.resource_region_id = m.get('ResourceRegionId')
+        if m.get('ResourceRouteName') is not None:
+            self.resource_route_name = m.get('ResourceRouteName')
+        return self
+
+
+class DescribeCloudResourcesResponseBodyCloudResources(TeaModel):
+    def __init__(
+        self,
+        owner_user_id: str = None,
+        resource_domain: str = None,
+        resource_function: str = None,
+        resource_instance: str = None,
+        resource_name: str = None,
+        resource_product: str = None,
+        resource_region_id: str = None,
+        resource_route_name: str = None,
+        resource_service: str = None,
+    ):
+        # The ID of the Alibaba Cloud account to which the resource belongs.
+        self.owner_user_id = owner_user_id
+        # The domain name. This parameter has a value only if the value of ResourceProduct is fc or sae.
+        self.resource_domain = resource_domain
+        # The function name. This parameter has a value only if the value of ResourceProduct is fc.
+        self.resource_function = resource_function
+        # The ID of the resource.
+        self.resource_instance = resource_instance
+        # The name of the resource.
+        self.resource_name = resource_name
+        # The cloud service to which the resource belongs. Valid values:
+        # 
+        # *   **alb**: ALB.
+        # *   **mse**: MSE.
+        # *   **fc**: Function Compute.
+        # *   **sae**: SAE.
+        self.resource_product = resource_product
+        # The region ID of the resource.
+        self.resource_region_id = resource_region_id
+        # The route name. This parameter has a value only if the value of ResourceProduct is mse.
+        self.resource_route_name = resource_route_name
+        # The service name. This parameter has a value only if the value of ResourceProduct is fc.
+        self.resource_service = resource_service
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.owner_user_id is not None:
+            result['OwnerUserId'] = self.owner_user_id
+        if self.resource_domain is not None:
+            result['ResourceDomain'] = self.resource_domain
+        if self.resource_function is not None:
+            result['ResourceFunction'] = self.resource_function
+        if self.resource_instance is not None:
+            result['ResourceInstance'] = self.resource_instance
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.resource_product is not None:
+            result['ResourceProduct'] = self.resource_product
+        if self.resource_region_id is not None:
+            result['ResourceRegionId'] = self.resource_region_id
+        if self.resource_route_name is not None:
+            result['ResourceRouteName'] = self.resource_route_name
+        if self.resource_service is not None:
+            result['ResourceService'] = self.resource_service
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OwnerUserId') is not None:
+            self.owner_user_id = m.get('OwnerUserId')
+        if m.get('ResourceDomain') is not None:
+            self.resource_domain = m.get('ResourceDomain')
+        if m.get('ResourceFunction') is not None:
+            self.resource_function = m.get('ResourceFunction')
+        if m.get('ResourceInstance') is not None:
+            self.resource_instance = m.get('ResourceInstance')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('ResourceProduct') is not None:
+            self.resource_product = m.get('ResourceProduct')
+        if m.get('ResourceRegionId') is not None:
+            self.resource_region_id = m.get('ResourceRegionId')
+        if m.get('ResourceRouteName') is not None:
+            self.resource_route_name = m.get('ResourceRouteName')
+        if m.get('ResourceService') is not None:
+            self.resource_service = m.get('ResourceService')
+        return self
+
+
+class DescribeCloudResourcesResponseBody(TeaModel):
+    def __init__(
+        self,
+        cloud_resources: List[DescribeCloudResourcesResponseBodyCloudResources] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # The cloud service resources that are added to WAF.
+        self.cloud_resources = cloud_resources
+        # The request ID.
+        self.request_id = request_id
+        # The total number of cloud service resources returned.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.cloud_resources:
+            for k in self.cloud_resources:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['CloudResources'] = []
+        if self.cloud_resources is not None:
+            for k in self.cloud_resources:
+                result['CloudResources'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.cloud_resources = []
+        if m.get('CloudResources') is not None:
+            for k in m.get('CloudResources'):
+                temp_model = DescribeCloudResourcesResponseBodyCloudResources()
+                self.cloud_resources.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeCloudResourcesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeCloudResourcesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeCloudResourcesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeDefenseResourceGroupRequest(TeaModel):
     def __init__(
         self,
         group_name: str = None,
         instance_id: str = None,
         region_id: str = None,
         resource_manager_resource_group_id: str = None,
@@ -3270,14 +3576,15 @@
         self.description = description
         # The details of the protected object. Different key-value pairs indicate different attributes of the protected object.
         self.detail = detail
         # The time when the protected object was created. Unit: milliseconds.
         self.gmt_create = gmt_create
         # The time when the protected object was modified. Unit: milliseconds.
         self.gmt_modified = gmt_modified
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.owner_user_id = owner_user_id
         # The pattern in which the protected object is protected.
         self.pattern = pattern
         # The name of the cloud service.
         self.product = product
         # The name of the protected object.
         self.resource = resource
@@ -4499,15 +4806,15 @@
         self.domain = domain
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id
         # The region in which the WAF instance is deployed. Valid values:
         # 
-        # *   **cn-hangzhou**: Chinese mainland
+        # *   **cn-hangzhou**: Chinese mainland.
         # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id
         # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id
 
     def validate(self):
         pass
@@ -8822,14 +9129,403 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribePeakTrendResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeProductInstancesRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        owner_user_id: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        region_id: str = None,
+        resource_instance_id: str = None,
+        resource_ip: str = None,
+        resource_manager_resource_group_id: str = None,
+        resource_name: str = None,
+        resource_product: str = None,
+        resource_region_id: str = None,
+    ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        self.owner_user_id = owner_user_id
+        # The page number. Default value: **1**.
+        self.page_number = page_number
+        # The number of entries per page. Default value: **10**.
+        self.page_size = page_size
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the instance.
+        self.resource_instance_id = resource_instance_id
+        # The public IP address of the instance.
+        self.resource_ip = resource_ip
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
+        # The name of the instance.
+        self.resource_name = resource_name
+        # The cloud service to which the instance belongs. Valid values:
+        # 
+        # *   **clb4**: Layer 4 Classic Load Balancer (CLB).
+        # *   **clb7**: Layer 7 CLB.
+        # *   **ecs**: Elastic Compute Service (ECS).
+        self.resource_product = resource_product
+        # The region ID of the instance. Valid values:
+        # 
+        # *   **cn-chengdu**: China (Chengdu).
+        # *   **cn-beijing**: China (Beijing).
+        # *   **cn-zhangjiakou**: China (Zhangjiakou).
+        # *   **cn-hangzhou**: China (Hangzhou).
+        # *   **cn-shanghai**: China (Shanghai).
+        # *   **cn-shenzhen**: China (Shenzhen).
+        # *   **cn-qingdao**: China (Qingdao).
+        # *   **cn-hongkong**: China (Hong Kong).
+        # *   **ap-southeast-3**: Malaysia (Kuala Lumpur).
+        # *   **ap-southeast-5**: Indonesia (Jakarta).
+        self.resource_region_id = resource_region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.owner_user_id is not None:
+            result['OwnerUserId'] = self.owner_user_id
+        if self.page_number is not None:
+            result['PageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['PageSize'] = self.page_size
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_instance_id is not None:
+            result['ResourceInstanceId'] = self.resource_instance_id
+        if self.resource_ip is not None:
+            result['ResourceIp'] = self.resource_ip
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        if self.resource_product is not None:
+            result['ResourceProduct'] = self.resource_product
+        if self.resource_region_id is not None:
+            result['ResourceRegionId'] = self.resource_region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('OwnerUserId') is not None:
+            self.owner_user_id = m.get('OwnerUserId')
+        if m.get('PageNumber') is not None:
+            self.page_number = m.get('PageNumber')
+        if m.get('PageSize') is not None:
+            self.page_size = m.get('PageSize')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceInstanceId') is not None:
+            self.resource_instance_id = m.get('ResourceInstanceId')
+        if m.get('ResourceIp') is not None:
+            self.resource_ip = m.get('ResourceIp')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        if m.get('ResourceProduct') is not None:
+            self.resource_product = m.get('ResourceProduct')
+        if m.get('ResourceRegionId') is not None:
+            self.resource_region_id = m.get('ResourceRegionId')
+        return self
+
+
+class DescribeProductInstancesResponseBodyProductInstancesResourcePortsCertificates(TeaModel):
+    def __init__(
+        self,
+        certificate_id: str = None,
+        certificate_name: str = None,
+    ):
+        # The ID of the certificate.
+        self.certificate_id = certificate_id
+        # The name of the certificate.
+        self.certificate_name = certificate_name
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.certificate_id is not None:
+            result['CertificateId'] = self.certificate_id
+        if self.certificate_name is not None:
+            result['CertificateName'] = self.certificate_name
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CertificateId') is not None:
+            self.certificate_id = m.get('CertificateId')
+        if m.get('CertificateName') is not None:
+            self.certificate_name = m.get('CertificateName')
+        return self
+
+
+class DescribeProductInstancesResponseBodyProductInstancesResourcePorts(TeaModel):
+    def __init__(
+        self,
+        certificates: List[DescribeProductInstancesResponseBodyProductInstancesResourcePortsCertificates] = None,
+        port: int = None,
+        protocol: str = None,
+    ):
+        # The information about the certificates.
+        self.certificates = certificates
+        # The port number.
+        self.port = port
+        # The protocol type. Valid values:
+        # 
+        # *   **http**\
+        # *   **https**\
+        self.protocol = protocol
+
+    def validate(self):
+        if self.certificates:
+            for k in self.certificates:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['Certificates'] = []
+        if self.certificates is not None:
+            for k in self.certificates:
+                result['Certificates'].append(k.to_map() if k else None)
+        if self.port is not None:
+            result['Port'] = self.port
+        if self.protocol is not None:
+            result['Protocol'] = self.protocol
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.certificates = []
+        if m.get('Certificates') is not None:
+            for k in m.get('Certificates'):
+                temp_model = DescribeProductInstancesResponseBodyProductInstancesResourcePortsCertificates()
+                self.certificates.append(temp_model.from_map(k))
+        if m.get('Port') is not None:
+            self.port = m.get('Port')
+        if m.get('Protocol') is not None:
+            self.protocol = m.get('Protocol')
+        return self
+
+
+class DescribeProductInstancesResponseBodyProductInstances(TeaModel):
+    def __init__(
+        self,
+        owner_user_id: str = None,
+        resource_instance_id: str = None,
+        resource_ip: str = None,
+        resource_name: str = None,
+        resource_ports: List[DescribeProductInstancesResponseBodyProductInstancesResourcePorts] = None,
+        resource_product: str = None,
+        resource_region_id: str = None,
+    ):
+        # The ID of the Alibaba Cloud account to which the resource belongs.
+        self.owner_user_id = owner_user_id
+        # The ID of the instance.
+        self.resource_instance_id = resource_instance_id
+        # The public IP address of the instance.
+        self.resource_ip = resource_ip
+        # The name of the instance.
+        self.resource_name = resource_name
+        # The information about the ports.
+        self.resource_ports = resource_ports
+        # The cloud service to which the instance belongs. Valid values:
+        # 
+        # *   **clb4**: Layer 4 CLB.
+        # *   **clb7**: Layer 7 CLB.
+        # *   **ecs**: ECS.
+        self.resource_product = resource_product
+        # The region ID of the instance. Valid values:
+        # 
+        # *   **cn-chengdu**: China (Chengdu).
+        # *   **cn-beijing**: China (Beijing).
+        # *   **cn-zhangjiakou**: China (Zhangjiakou).
+        # *   **cn-hangzhou**: China (Hangzhou).
+        # *   **cn-shanghai**: China (Shanghai).
+        # *   **cn-shenzhen**: China (Shenzhen).
+        # *   **cn-qingdao**: China (Qingdao).
+        # *   **cn-hongkong**: China (Hong Kong).
+        # *   **ap-southeast-3**: Malaysia (Kuala Lumpur).
+        # *   **ap-southeast-5**: Indonesia (Jakarta).
+        self.resource_region_id = resource_region_id
+
+    def validate(self):
+        if self.resource_ports:
+            for k in self.resource_ports:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.owner_user_id is not None:
+            result['OwnerUserId'] = self.owner_user_id
+        if self.resource_instance_id is not None:
+            result['ResourceInstanceId'] = self.resource_instance_id
+        if self.resource_ip is not None:
+            result['ResourceIp'] = self.resource_ip
+        if self.resource_name is not None:
+            result['ResourceName'] = self.resource_name
+        result['ResourcePorts'] = []
+        if self.resource_ports is not None:
+            for k in self.resource_ports:
+                result['ResourcePorts'].append(k.to_map() if k else None)
+        if self.resource_product is not None:
+            result['ResourceProduct'] = self.resource_product
+        if self.resource_region_id is not None:
+            result['ResourceRegionId'] = self.resource_region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('OwnerUserId') is not None:
+            self.owner_user_id = m.get('OwnerUserId')
+        if m.get('ResourceInstanceId') is not None:
+            self.resource_instance_id = m.get('ResourceInstanceId')
+        if m.get('ResourceIp') is not None:
+            self.resource_ip = m.get('ResourceIp')
+        if m.get('ResourceName') is not None:
+            self.resource_name = m.get('ResourceName')
+        self.resource_ports = []
+        if m.get('ResourcePorts') is not None:
+            for k in m.get('ResourcePorts'):
+                temp_model = DescribeProductInstancesResponseBodyProductInstancesResourcePorts()
+                self.resource_ports.append(temp_model.from_map(k))
+        if m.get('ResourceProduct') is not None:
+            self.resource_product = m.get('ResourceProduct')
+        if m.get('ResourceRegionId') is not None:
+            self.resource_region_id = m.get('ResourceRegionId')
+        return self
+
+
+class DescribeProductInstancesResponseBody(TeaModel):
+    def __init__(
+        self,
+        product_instances: List[DescribeProductInstancesResponseBodyProductInstances] = None,
+        request_id: str = None,
+        total_count: int = None,
+    ):
+        # The information about the instances.
+        self.product_instances = product_instances
+        # The ID of the request.
+        self.request_id = request_id
+        # The total number of entries returned.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.product_instances:
+            for k in self.product_instances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        result['ProductInstances'] = []
+        if self.product_instances is not None:
+            for k in self.product_instances:
+                result['ProductInstances'].append(k.to_map() if k else None)
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        if self.total_count is not None:
+            result['TotalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        self.product_instances = []
+        if m.get('ProductInstances') is not None:
+            for k in m.get('ProductInstances'):
+                temp_model = DescribeProductInstancesResponseBodyProductInstances()
+                self.product_instances.append(temp_model.from_map(k))
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        if m.get('TotalCount') is not None:
+            self.total_count = m.get('TotalCount')
+        return self
+
+
+class DescribeProductInstancesResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: DescribeProductInstancesResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = DescribeProductInstancesResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class DescribeResourceInstanceCertsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         region_id: str = None,
@@ -14948,7 +15644,123 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyTemplateResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SyncProductInstanceRequest(TeaModel):
+    def __init__(
+        self,
+        instance_id: str = None,
+        region_id: str = None,
+        resource_manager_resource_group_id: str = None,
+    ):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.instance_id is not None:
+            result['InstanceId'] = self.instance_id
+        if self.region_id is not None:
+            result['RegionId'] = self.region_id
+        if self.resource_manager_resource_group_id is not None:
+            result['ResourceManagerResourceGroupId'] = self.resource_manager_resource_group_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('InstanceId') is not None:
+            self.instance_id = m.get('InstanceId')
+        if m.get('RegionId') is not None:
+            self.region_id = m.get('RegionId')
+        if m.get('ResourceManagerResourceGroupId') is not None:
+            self.resource_manager_resource_group_id = m.get('ResourceManagerResourceGroupId')
+        return self
+
+
+class SyncProductInstanceResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        # The request ID.
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SyncProductInstanceResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: SyncProductInstanceResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = SyncProductInstanceResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO` & `alibabacloud_waf-openapi20211001-3.3.0/alibabacloud_waf_openapi20211001.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-waf-openapi20211001
-Version: 3.2.0
+Version: 3.3.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001-3.2.0/setup.py` & `alibabacloud_waf-openapi20211001-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_waf-openapi20211001.
 
-Created on 28/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_waf_openapi20211001"
 NAME = "alibabacloud_waf-openapi20211001" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud waf-openapi (20211001) SDK Library for Python"
```

