# Comparing `tmp/alibabacloud_foasconsole20190601-1.0.2.tar.gz` & `tmp/alibabacloud_foasconsole20190601-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_foasconsole20190601-1.0.2.tar", last modified: Sun Feb  4 17:14:26 2024, max compression
+gzip compressed data, was "dist/alibabacloud_foasconsole20190601-1.0.3.tar", last modified: Sun Apr  7 17:11:11 2024, max compression
```

## Comparing `alibabacloud_foasconsole20190601-1.0.2.tar` & `alibabacloud_foasconsole20190601-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      128 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2457 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1127 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1212 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66280 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601/client.py
--rw-r--r--   0 root         (0) root         (0)   183213 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2457 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      484 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-02-04 17:14:26.000000 alibabacloud_foasconsole20190601-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      670 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1127 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66280 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601/client.py
+-rw-r--r--   0 root         (0) root         (0)   200879 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      484 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-07 17:11:10.000000 alibabacloud_foasconsole20190601-1.0.3/setup.py
```

### Comparing `alibabacloud_foasconsole20190601-1.0.2/LICENSE` & `alibabacloud_foasconsole20190601-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601-1.0.2/PKG-INFO` & `alibabacloud_foasconsole20190601-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_foasconsole20190601
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud foasconsole (20190601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20190601-1.0.2/README-CN.md` & `alibabacloud_foasconsole20190601-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601-1.0.2/README.md` & `alibabacloud_foasconsole20190601-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601/client.py` & `alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601/models.py` & `alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3402,14 +3402,71 @@
         m = m or dict()
         if m.get('ConvertPostpayInstanceRequest') is not None:
             temp_model = QueryConvertInstancePriceRequestConvertPostpayInstanceRequest()
             self.convert_postpay_instance_request = temp_model.from_map(m['ConvertPostpayInstanceRequest'])
         return self
 
 
+class QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -3485,31 +3542,41 @@
 
 
 class QueryConvertInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryConvertInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -3521,54 +3588,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryConvertInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryConvertInstancePriceResponseBody(TeaModel):
     def __init__(
@@ -3710,14 +3794,71 @@
         m = m or dict()
         if m.get('ConvertPrepayInstanceRequest') is not None:
             temp_model = QueryConvertPrepayInstancePriceRequestConvertPrepayInstanceRequest()
             self.convert_prepay_instance_request = temp_model.from_map(m['ConvertPrepayInstanceRequest'])
         return self
 
 
+class QueryConvertPrepayInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryConvertPrepayInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -3793,31 +3934,41 @@
 
 
 class QueryConvertPrepayInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryConvertPrepayInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryConvertPrepayInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryConvertPrepayInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -3829,54 +3980,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryConvertPrepayInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryConvertPrepayInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryConvertPrepayInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryConvertPrepayInstancePriceResponseBody(TeaModel):
     def __init__(
@@ -4239,14 +4407,71 @@
         m = m or dict()
         if m.get('CreateInstanceRequest') is not None:
             temp_model = QueryCreateInstancePriceRequestCreateInstanceRequest()
             self.create_instance_request = temp_model.from_map(m['CreateInstanceRequest'])
         return self
 
 
+class QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -4322,31 +4547,41 @@
 
 
 class QueryCreateInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryCreateInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -4358,54 +4593,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryCreateInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryCreateInstancePriceResponseBody(TeaModel):
     def __init__(
@@ -4648,14 +4900,71 @@
         m = m or dict()
         if m.get('ModifyPrepayInstanceSpecRequest') is not None:
             temp_model = QueryModifyInstancePriceRequestModifyPrepayInstanceSpecRequest()
             self.modify_prepay_instance_spec_request = temp_model.from_map(m['ModifyPrepayInstanceSpecRequest'])
         return self
 
 
+class QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -4731,31 +5040,41 @@
 
 
 class QueryModifyInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryModifyInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -4767,54 +5086,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryModifyInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryModifyInstancePriceResponseBody(TeaModel):
     def __init__(
@@ -4968,14 +5304,71 @@
         m = m or dict()
         if m.get('RenewInstanceRequest') is not None:
             temp_model = QueryRenewInstancePriceRequestRenewInstanceRequest()
             self.renew_instance_request = temp_model.from_map(m['RenewInstanceRequest'])
         return self
 
 
+class QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(
+        self,
+        cheap_rate: str = None,
+        cheap_stand_amount: str = None,
+        is_show: bool = None,
+        month_price: str = None,
+        original_stand_amount: str = None,
+        start_time: str = None,
+    ):
+        self.cheap_rate = cheap_rate
+        self.cheap_stand_amount = cheap_stand_amount
+        self.is_show = is_show
+        self.month_price = month_price
+        self.original_stand_amount = original_stand_amount
+        self.start_time = start_time
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
+        if self.cheap_rate is not None:
+            result['CheapRate'] = self.cheap_rate
+        if self.cheap_stand_amount is not None:
+            result['CheapStandAmount'] = self.cheap_stand_amount
+        if self.is_show is not None:
+            result['IsShow'] = self.is_show
+        if self.month_price is not None:
+            result['MonthPrice'] = self.month_price
+        if self.original_stand_amount is not None:
+            result['OriginalStandAmount'] = self.original_stand_amount
+        if self.start_time is not None:
+            result['StartTime'] = self.start_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('CheapRate') is not None:
+            self.cheap_rate = m.get('CheapRate')
+        if m.get('CheapStandAmount') is not None:
+            self.cheap_stand_amount = m.get('CheapStandAmount')
+        if m.get('IsShow') is not None:
+            self.is_show = m.get('IsShow')
+        if m.get('MonthPrice') is not None:
+            self.month_price = m.get('MonthPrice')
+        if m.get('OriginalStandAmount') is not None:
+            self.original_stand_amount = m.get('OriginalStandAmount')
+        if m.get('StartTime') is not None:
+            self.start_time = m.get('StartTime')
+        return self
+
+
 class QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions(TeaModel):
     def __init__(
         self,
         promotion_desc: str = None,
         promotion_name: str = None,
         promotion_option_no: str = None,
         selected: bool = None,
@@ -5051,31 +5444,41 @@
 
 
 class QueryRenewInstancePriceResponseBodyPriceInfo(TeaModel):
     def __init__(
         self,
         code: str = None,
         currency: str = None,
+        depreciate_info: QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo = None,
         discount_amount: float = None,
+        is_contract_activity: bool = None,
         message: str = None,
         optional_promotions: List[QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions] = None,
         original_amount: float = None,
         rules: List[QueryRenewInstancePriceResponseBodyPriceInfoRules] = None,
+        stand_discount_price: str = None,
+        stand_price: str = None,
         trade_amount: float = None,
     ):
         self.code = code
         self.currency = currency
+        self.depreciate_info = depreciate_info
         self.discount_amount = discount_amount
+        self.is_contract_activity = is_contract_activity
         self.message = message
         self.optional_promotions = optional_promotions
         self.original_amount = original_amount
         self.rules = rules
+        self.stand_discount_price = stand_discount_price
+        self.stand_price = stand_price
         self.trade_amount = trade_amount
 
     def validate(self):
+        if self.depreciate_info:
+            self.depreciate_info.validate()
         if self.optional_promotions:
             for k in self.optional_promotions:
                 if k:
                     k.validate()
         if self.rules:
             for k in self.rules:
                 if k:
@@ -5087,54 +5490,71 @@
             return _map
 
         result = dict()
         if self.code is not None:
             result['Code'] = self.code
         if self.currency is not None:
             result['Currency'] = self.currency
+        if self.depreciate_info is not None:
+            result['DepreciateInfo'] = self.depreciate_info.to_map()
         if self.discount_amount is not None:
             result['DiscountAmount'] = self.discount_amount
+        if self.is_contract_activity is not None:
+            result['IsContractActivity'] = self.is_contract_activity
         if self.message is not None:
             result['Message'] = self.message
         result['OptionalPromotions'] = []
         if self.optional_promotions is not None:
             for k in self.optional_promotions:
                 result['OptionalPromotions'].append(k.to_map() if k else None)
         if self.original_amount is not None:
             result['OriginalAmount'] = self.original_amount
         result['Rules'] = []
         if self.rules is not None:
             for k in self.rules:
                 result['Rules'].append(k.to_map() if k else None)
+        if self.stand_discount_price is not None:
+            result['StandDiscountPrice'] = self.stand_discount_price
+        if self.stand_price is not None:
+            result['StandPrice'] = self.stand_price
         if self.trade_amount is not None:
             result['TradeAmount'] = self.trade_amount
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('Code') is not None:
             self.code = m.get('Code')
         if m.get('Currency') is not None:
             self.currency = m.get('Currency')
+        if m.get('DepreciateInfo') is not None:
+            temp_model = QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo()
+            self.depreciate_info = temp_model.from_map(m['DepreciateInfo'])
         if m.get('DiscountAmount') is not None:
             self.discount_amount = m.get('DiscountAmount')
+        if m.get('IsContractActivity') is not None:
+            self.is_contract_activity = m.get('IsContractActivity')
         if m.get('Message') is not None:
             self.message = m.get('Message')
         self.optional_promotions = []
         if m.get('OptionalPromotions') is not None:
             for k in m.get('OptionalPromotions'):
                 temp_model = QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions()
                 self.optional_promotions.append(temp_model.from_map(k))
         if m.get('OriginalAmount') is not None:
             self.original_amount = m.get('OriginalAmount')
         self.rules = []
         if m.get('Rules') is not None:
             for k in m.get('Rules'):
                 temp_model = QueryRenewInstancePriceResponseBodyPriceInfoRules()
                 self.rules.append(temp_model.from_map(k))
+        if m.get('StandDiscountPrice') is not None:
+            self.stand_discount_price = m.get('StandDiscountPrice')
+        if m.get('StandPrice') is not None:
+            self.stand_price = m.get('StandPrice')
         if m.get('TradeAmount') is not None:
             self.trade_amount = m.get('TradeAmount')
         return self
 
 
 class QueryRenewInstancePriceResponseBody(TeaModel):
     def __init__(
```

### Comparing `alibabacloud_foasconsole20190601-1.0.2/alibabacloud_foasconsole20190601.egg-info/PKG-INFO` & `alibabacloud_foasconsole20190601-1.0.3/alibabacloud_foasconsole20190601.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-foasconsole20190601
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud foasconsole (20190601) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20190601-1.0.2/setup.py` & `alibabacloud_foasconsole20190601-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_foasconsole20190601.
 
-Created on 04/02/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_foasconsole20190601"
 NAME = "alibabacloud_foasconsole20190601" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud foasconsole (20190601) SDK Library for Python"
```

