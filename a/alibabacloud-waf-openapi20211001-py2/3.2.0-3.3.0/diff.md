# Comparing `tmp/alibabacloud_waf-openapi20211001_py2-3.2.0.tar.gz` & `tmp/alibabacloud_waf-openapi20211001_py2-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_waf-openapi20211001_py2-3.2.0.tar", last modified: Thu Mar 28 17:18:17 2024, max compression
+gzip compressed data, was "dist/alibabacloud_waf-openapi20211001_py2-3.3.0.tar", last modified: Sun Apr  7 03:49:23 2024, max compression
```

## Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0.tar` & `alibabacloud_waf-openapi20211001_py2-3.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/
--rw-r--r--   0 root         (0) root         (0)     1369 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001/__init__.py
--rw-r--r--   0 root         (0) root         (0)   116205 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001/client.py
--rw-r--r--   0 root         (0) root         (0)   558815 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2945 2024-03-28 17:18:17.000000 alibabacloud_waf-openapi20211001_py2-3.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1629 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   122943 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/client.py
+-rw-r--r--   0 root         (0) root         (0)   590442 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2945 2024-04-07 03:49:23.000000 alibabacloud_waf-openapi20211001_py2-3.3.0/setup.py
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/ChangeLog.md` & `alibabacloud_waf-openapi20211001_py2-3.3.0/ChangeLog.md`

 * *Files 5% similar despite different names*

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

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/LICENSE` & `alibabacloud_waf-openapi20211001_py2-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/PKG-INFO` & `alibabacloud_waf-openapi20211001_py2-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_waf-openapi20211001_py2
-Version: 3.2.0
+Version: 3.3.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/README-CN.md` & `alibabacloud_waf-openapi20211001_py2-3.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/README.md` & `alibabacloud_waf-openapi20211001_py2-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001/client.py` & `alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -636,14 +636,66 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_certs(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_certs_with_options(request, runtime)
 
+    def describe_cloud_resources_with_options(self, request, runtime):
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
+    def describe_cloud_resources(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_cloud_resources_with_options(request, runtime)
+
     def describe_defense_resource_group_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.group_name):
             query['GroupName'] = request.group_name
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
@@ -1398,14 +1450,62 @@
             self.call_api(params, req, runtime)
         )
 
     def describe_peak_trend(self, request):
         runtime = util_models.RuntimeOptions()
         return self.describe_peak_trend_with_options(request, runtime)
 
+    def describe_product_instances_with_options(self, request, runtime):
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
+    def describe_product_instances(self, request):
+        runtime = util_models.RuntimeOptions()
+        return self.describe_product_instances_with_options(request, runtime)
+
     def describe_resource_instance_certs_with_options(self, request, runtime):
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
@@ -2689,7 +2789,57 @@
             waf_openapi_20211001_models.ModifyTemplateResourcesResponse(),
             self.call_api(params, req, runtime)
         )
 
     def modify_template_resources(self, request):
         runtime = util_models.RuntimeOptions()
         return self.modify_template_resources_with_options(request, runtime)
+
+    def sync_product_instance_with_options(self, request, runtime):
+        """
+        SyncProductInstance is an asynchronous operation. You can call the [DescribeProductInstances](~~2743168~~) operation to query the status of the task.
+        
+
+        @param request: SyncProductInstanceRequest
+
+        @param runtime: runtime options for this request RuntimeOptions
+
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
+    def sync_product_instance(self, request):
+        """
+        SyncProductInstance is an asynchronous operation. You can call the [DescribeProductInstances](~~2743168~~) operation to query the status of the task.
+        
+
+        @param request: SyncProductInstanceRequest
+
+        @return: SyncProductInstanceResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        return self.sync_product_instance_with_options(request, runtime)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001/models.py` & `alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2360,14 +2360,288 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribeCertsResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeCloudResourcesRequest(TeaModel):
+    def __init__(self, instance_id=None, owner_user_id=None, page_number=None, page_size=None, region_id=None,
+                 resource_domain=None, resource_function=None, resource_instance_id=None, resource_manager_resource_group_id=None,
+                 resource_name=None, resource_product=None, resource_region_id=None, resource_route_name=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The ID of the Alibaba Cloud account to which the resource belongs.
+        self.owner_user_id = owner_user_id  # type: str
+        # The page number. Default value: **1**.
+        self.page_number = page_number  # type: long
+        # The number of entries per page. Default value: **10**.
+        self.page_size = page_size  # type: long
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The domain name. You can use this parameter if you set ResourceProduct to fc or sae.
+        self.resource_domain = resource_domain  # type: str
+        # The function name. You can use this parameter if you set ResourceProduct to fc.
+        self.resource_function = resource_function  # type: str
+        # The ID of the resource.
+        self.resource_instance_id = resource_instance_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The name of the resource.
+        self.resource_name = resource_name  # type: str
+        # The cloud service to which the resource belongs. Valid values:
+        # 
+        # *   **alb**: Application Load Balancer (ALB).
+        # *   **mse**: Microservices Engine (MSE).
+        # *   **fc**: Function Compute.
+        # *   **sae**: Serverless App Engine (SAE).
+        # 
+        # >  Different cloud services are available in different regions. The specified cloud service must be available in the specified region.
+        self.resource_product = resource_product  # type: str
+        # The region ID of the resource. For information about region IDs, see the following table.
+        # 
+        # >  Different cloud services are available in different regions. The specified cloud service must be available in the specified region.
+        self.resource_region_id = resource_region_id  # type: str
+        # The route name. You can use this parameter if you set ResourceProduct to mse.
+        self.resource_route_name = resource_route_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCloudResourcesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, owner_user_id=None, resource_domain=None, resource_function=None, resource_instance=None,
+                 resource_name=None, resource_product=None, resource_region_id=None, resource_route_name=None,
+                 resource_service=None):
+        # The ID of the Alibaba Cloud account to which the resource belongs.
+        self.owner_user_id = owner_user_id  # type: str
+        # The domain name. This parameter has a value only if the value of ResourceProduct is fc or sae.
+        self.resource_domain = resource_domain  # type: str
+        # The function name. This parameter has a value only if the value of ResourceProduct is fc.
+        self.resource_function = resource_function  # type: str
+        # The ID of the resource.
+        self.resource_instance = resource_instance  # type: str
+        # The name of the resource.
+        self.resource_name = resource_name  # type: str
+        # The cloud service to which the resource belongs. Valid values:
+        # 
+        # *   **alb**: ALB.
+        # *   **mse**: MSE.
+        # *   **fc**: Function Compute.
+        # *   **sae**: SAE.
+        self.resource_product = resource_product  # type: str
+        # The region ID of the resource.
+        self.resource_region_id = resource_region_id  # type: str
+        # The route name. This parameter has a value only if the value of ResourceProduct is mse.
+        self.resource_route_name = resource_route_name  # type: str
+        # The service name. This parameter has a value only if the value of ResourceProduct is fc.
+        self.resource_service = resource_service  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeCloudResourcesResponseBodyCloudResources, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, cloud_resources=None, request_id=None, total_count=None):
+        # The cloud service resources that are added to WAF.
+        self.cloud_resources = cloud_resources  # type: list[DescribeCloudResourcesResponseBodyCloudResources]
+        # The request ID.
+        self.request_id = request_id  # type: str
+        # The total number of cloud service resources returned.
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.cloud_resources:
+            for k in self.cloud_resources:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeCloudResourcesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeCloudResourcesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeCloudResourcesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, group_name=None, instance_id=None, region_id=None, resource_manager_resource_group_id=None):
         # The name of the protected object group whose information you want to query.
         self.group_name = group_name  # type: str
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to obtain the ID of the WAF instance.
@@ -2907,14 +3181,15 @@
         self.description = description  # type: str
         # The details of the protected object. Different key-value pairs indicate different attributes of the protected object.
         self.detail = detail  # type: dict[str, any]
         # The time when the protected object was created. Unit: milliseconds.
         self.gmt_create = gmt_create  # type: long
         # The time when the protected object was modified. Unit: milliseconds.
         self.gmt_modified = gmt_modified  # type: long
+        # The ID of the Alibaba Cloud account to which the resource belongs.
         self.owner_user_id = owner_user_id  # type: str
         # The pattern in which the protected object is protected.
         self.pattern = pattern  # type: str
         # The name of the cloud service.
         self.product = product  # type: str
         # The name of the protected object.
         self.resource = resource  # type: str
@@ -4013,15 +4288,15 @@
         self.domain = domain  # type: str
         # The ID of the Web Application Firewall (WAF) instance.
         # 
         # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
         self.instance_id = instance_id  # type: str
         # The region in which the WAF instance is deployed. Valid values:
         # 
-        # *   **cn-hangzhou**: Chinese mainland
+        # *   **cn-hangzhou**: Chinese mainland.
         # *   **ap-southeast-1**: outside the Chinese mainland.
         self.region_id = region_id  # type: str
         # The ID of the Alibaba Cloud resource group.
         self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
 
     def validate(self):
         pass
@@ -7890,14 +8165,365 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = DescribePeakTrendResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class DescribeProductInstancesRequest(TeaModel):
+    def __init__(self, instance_id=None, owner_user_id=None, page_number=None, page_size=None, region_id=None,
+                 resource_instance_id=None, resource_ip=None, resource_manager_resource_group_id=None, resource_name=None,
+                 resource_product=None, resource_region_id=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        self.owner_user_id = owner_user_id  # type: str
+        # The page number. Default value: **1**.
+        self.page_number = page_number  # type: long
+        # The number of entries per page. Default value: **10**.
+        self.page_size = page_size  # type: long
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the instance.
+        self.resource_instance_id = resource_instance_id  # type: str
+        # The public IP address of the instance.
+        self.resource_ip = resource_ip  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+        # The name of the instance.
+        self.resource_name = resource_name  # type: str
+        # The cloud service to which the instance belongs. Valid values:
+        # 
+        # *   **clb4**: Layer 4 Classic Load Balancer (CLB).
+        # *   **clb7**: Layer 7 CLB.
+        # *   **ecs**: Elastic Compute Service (ECS).
+        self.resource_product = resource_product  # type: str
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
+        self.resource_region_id = resource_region_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeProductInstancesRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, certificate_id=None, certificate_name=None):
+        # The ID of the certificate.
+        self.certificate_id = certificate_id  # type: str
+        # The name of the certificate.
+        self.certificate_name = certificate_name  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(DescribeProductInstancesResponseBodyProductInstancesResourcePortsCertificates, self).to_map()
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
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('CertificateId') is not None:
+            self.certificate_id = m.get('CertificateId')
+        if m.get('CertificateName') is not None:
+            self.certificate_name = m.get('CertificateName')
+        return self
+
+
+class DescribeProductInstancesResponseBodyProductInstancesResourcePorts(TeaModel):
+    def __init__(self, certificates=None, port=None, protocol=None):
+        # The information about the certificates.
+        self.certificates = certificates  # type: list[DescribeProductInstancesResponseBodyProductInstancesResourcePortsCertificates]
+        # The port number.
+        self.port = port  # type: int
+        # The protocol type. Valid values:
+        # 
+        # *   **http**\
+        # *   **https**\
+        self.protocol = protocol  # type: str
+
+    def validate(self):
+        if self.certificates:
+            for k in self.certificates:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeProductInstancesResponseBodyProductInstancesResourcePorts, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, owner_user_id=None, resource_instance_id=None, resource_ip=None, resource_name=None,
+                 resource_ports=None, resource_product=None, resource_region_id=None):
+        # The ID of the Alibaba Cloud account to which the resource belongs.
+        self.owner_user_id = owner_user_id  # type: str
+        # The ID of the instance.
+        self.resource_instance_id = resource_instance_id  # type: str
+        # The public IP address of the instance.
+        self.resource_ip = resource_ip  # type: str
+        # The name of the instance.
+        self.resource_name = resource_name  # type: str
+        # The information about the ports.
+        self.resource_ports = resource_ports  # type: list[DescribeProductInstancesResponseBodyProductInstancesResourcePorts]
+        # The cloud service to which the instance belongs. Valid values:
+        # 
+        # *   **clb4**: Layer 4 CLB.
+        # *   **clb7**: Layer 7 CLB.
+        # *   **ecs**: ECS.
+        self.resource_product = resource_product  # type: str
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
+        self.resource_region_id = resource_region_id  # type: str
+
+    def validate(self):
+        if self.resource_ports:
+            for k in self.resource_ports:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeProductInstancesResponseBodyProductInstances, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, product_instances=None, request_id=None, total_count=None):
+        # The information about the instances.
+        self.product_instances = product_instances  # type: list[DescribeProductInstancesResponseBodyProductInstances]
+        # The ID of the request.
+        self.request_id = request_id  # type: str
+        # The total number of entries returned.
+        self.total_count = total_count  # type: long
+
+    def validate(self):
+        if self.product_instances:
+            for k in self.product_instances:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super(DescribeProductInstancesResponseBody, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: DescribeProductInstancesResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(DescribeProductInstancesResponse, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, instance_id=None, page_number=None, page_size=None, region_id=None,
                  resource_instance_id=None, resource_manager_resource_group_id=None):
         self.instance_id = instance_id  # type: str
         self.page_number = page_number  # type: long
         self.page_size = page_size  # type: long
         self.region_id = region_id  # type: str
@@ -13357,7 +13983,110 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = ModifyTemplateResourcesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class SyncProductInstanceRequest(TeaModel):
+    def __init__(self, instance_id=None, region_id=None, resource_manager_resource_group_id=None):
+        # The ID of the WAF instance.
+        # 
+        # >  You can call the [DescribeInstance](~~433756~~) operation to query the ID of the WAF instance.
+        self.instance_id = instance_id  # type: str
+        # The region in which the WAF instance is deployed. Valid values:
+        # 
+        # *   **cn-hangzhou**: Chinese mainland.
+        # *   **ap-southeast-1**: outside the Chinese mainland.
+        self.region_id = region_id  # type: str
+        # The ID of the Alibaba Cloud resource group.
+        self.resource_manager_resource_group_id = resource_manager_resource_group_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SyncProductInstanceRequest, self).to_map()
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
+    def from_map(self, m=None):
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
+    def __init__(self, request_id=None):
+        # The request ID.
+        self.request_id = request_id  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(SyncProductInstanceResponseBody, self).to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['RequestId'] = self.request_id
+        return result
+
+    def from_map(self, m=None):
+        m = m or dict()
+        if m.get('RequestId') is not None:
+            self.request_id = m.get('RequestId')
+        return self
+
+
+class SyncProductInstanceResponse(TeaModel):
+    def __init__(self, headers=None, status_code=None, body=None):
+        self.headers = headers  # type: dict[str, str]
+        self.status_code = status_code  # type: int
+        self.body = body  # type: SyncProductInstanceResponseBody
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super(SyncProductInstanceResponse, self).to_map()
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
+    def from_map(self, m=None):
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

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO` & `alibabacloud_waf-openapi20211001_py2-3.3.0/alibabacloud_waf_openapi20211001_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-waf-openapi20211001-py2
-Version: 3.2.0
+Version: 3.3.0
 Summary: Alibaba Cloud waf-openapi (20211001) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_waf-openapi20211001_py2-3.2.0/setup.py` & `alibabacloud_waf-openapi20211001_py2-3.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_waf-openapi20211001_py2.
 
-Created on 28/03/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_waf_openapi20211001"
 NAME = "alibabacloud_waf-openapi20211001_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud waf-openapi (20211001) SDK Library for Python2"
```

