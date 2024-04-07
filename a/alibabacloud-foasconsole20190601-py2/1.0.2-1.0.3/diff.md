# Comparing `tmp/alibabacloud_foasconsole20190601_py2-1.0.2.tar.gz` & `tmp/alibabacloud_foasconsole20190601_py2-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_foasconsole20190601_py2-1.0.2.tar", last modified: Sun Feb  4 17:12:04 2024, max compression
+gzip compressed data, was "dist/alibabacloud_foasconsole20190601_py2-1.0.3.tar", last modified: Sun Apr  7 17:10:49 2024, max compression
```

## Comparing `alibabacloud_foasconsole20190601_py2-1.0.2.tar` & `alibabacloud_foasconsole20190601_py2-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      129 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1057 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1140 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601/
--rw-r--r--   0 root         (0) root         (0)       21 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26864 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601/client.py
--rw-r--r--   0 root         (0) root         (0)   185928 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      504 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       33 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-02-04 17:12:04.000000 alibabacloud_foasconsole20190601_py2-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2943 2024-02-04 17:12:03.000000 alibabacloud_foasconsole20190601_py2-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      671 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1057 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26864 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601/client.py
+-rw-r--r--   0 root         (0) root         (0)   203881 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      504 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2943 2024-04-07 17:10:49.000000 alibabacloud_foasconsole20190601_py2-1.0.3/setup.py
```

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/LICENSE` & `alibabacloud_foasconsole20190601_py2-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/PKG-INFO` & `alibabacloud_foasconsole20190601_py2-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_foasconsole20190601_py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud foasconsole (20190601) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/README-CN.md` & `alibabacloud_foasconsole20190601_py2-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/README.md` & `alibabacloud_foasconsole20190601_py2-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601/client.py` & `alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601/models.py` & `alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -2999,14 +2999,64 @@
         m = m or dict()
         if m.get('ConvertPostpayInstanceRequest') is not None:
             temp_model = QueryConvertInstancePriceRequestConvertPostpayInstanceRequest()
             self.convert_postpay_instance_request = temp_model.from_map(m['ConvertPostpayInstanceRequest'])
         return self
 
 
+class QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -3068,26 +3118,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryConvertInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryConvertInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryConvertInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryConvertInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -3099,54 +3156,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
@@ -3271,14 +3345,64 @@
         m = m or dict()
         if m.get('ConvertPrepayInstanceRequest') is not None:
             temp_model = QueryConvertPrepayInstancePriceRequestConvertPrepayInstanceRequest()
             self.convert_prepay_instance_request = temp_model.from_map(m['ConvertPrepayInstanceRequest'])
         return self
 
 
+class QueryConvertPrepayInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryConvertPrepayInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -3340,26 +3464,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryConvertPrepayInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryConvertPrepayInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryConvertPrepayInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryConvertPrepayInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -3371,54 +3502,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
@@ -3737,14 +3885,64 @@
         m = m or dict()
         if m.get('CreateInstanceRequest') is not None:
             temp_model = QueryCreateInstancePriceRequestCreateInstanceRequest()
             self.create_instance_request = temp_model.from_map(m['CreateInstanceRequest'])
         return self
 
 
+class QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -3806,26 +4004,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryCreateInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryCreateInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryCreateInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryCreateInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -3837,54 +4042,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
@@ -4098,14 +4320,64 @@
         m = m or dict()
         if m.get('ModifyPrepayInstanceSpecRequest') is not None:
             temp_model = QueryModifyInstancePriceRequestModifyPrepayInstanceSpecRequest()
             self.modify_prepay_instance_spec_request = temp_model.from_map(m['ModifyPrepayInstanceSpecRequest'])
         return self
 
 
+class QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -4167,26 +4439,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryModifyInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryModifyInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryModifyInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryModifyInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -4198,54 +4477,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
@@ -4380,14 +4676,64 @@
         m = m or dict()
         if m.get('RenewInstanceRequest') is not None:
             temp_model = QueryRenewInstancePriceRequestRenewInstanceRequest()
             self.renew_instance_request = temp_model.from_map(m['RenewInstanceRequest'])
         return self
 
 
+class QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo(TeaModel):
+    def __init__(self, cheap_rate=None, cheap_stand_amount=None, is_show=None, month_price=None,
+                 original_stand_amount=None, start_time=None):
+        self.cheap_rate = cheap_rate  # type: str
+        self.cheap_stand_amount = cheap_stand_amount  # type: str
+        self.is_show = is_show  # type: bool
+        self.month_price = month_price  # type: str
+        self.original_stand_amount = original_stand_amount  # type: str
+        self.start_time = start_time  # type: str
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super(QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo, self).to_map()
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
+    def from_map(self, m=None):
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
     def __init__(self, promotion_desc=None, promotion_name=None, promotion_option_no=None, selected=None):
         self.promotion_desc = promotion_desc  # type: str
         self.promotion_name = promotion_name  # type: str
         self.promotion_option_no = promotion_option_no  # type: str
         self.selected = selected  # type: bool
 
@@ -4449,26 +4795,33 @@
             self.description = m.get('Description')
         if m.get('RuleId') is not None:
             self.rule_id = m.get('RuleId')
         return self
 
 
 class QueryRenewInstancePriceResponseBodyPriceInfo(TeaModel):
-    def __init__(self, code=None, currency=None, discount_amount=None, message=None, optional_promotions=None,
-                 original_amount=None, rules=None, trade_amount=None):
+    def __init__(self, code=None, currency=None, depreciate_info=None, discount_amount=None,
+                 is_contract_activity=None, message=None, optional_promotions=None, original_amount=None, rules=None,
+                 stand_discount_price=None, stand_price=None, trade_amount=None):
         self.code = code  # type: str
         self.currency = currency  # type: str
+        self.depreciate_info = depreciate_info  # type: QueryRenewInstancePriceResponseBodyPriceInfoDepreciateInfo
         self.discount_amount = discount_amount  # type: float
+        self.is_contract_activity = is_contract_activity  # type: bool
         self.message = message  # type: str
         self.optional_promotions = optional_promotions  # type: list[QueryRenewInstancePriceResponseBodyPriceInfoOptionalPromotions]
         self.original_amount = original_amount  # type: float
         self.rules = rules  # type: list[QueryRenewInstancePriceResponseBodyPriceInfoRules]
+        self.stand_discount_price = stand_discount_price  # type: str
+        self.stand_price = stand_price  # type: str
         self.trade_amount = trade_amount  # type: float
 
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
@@ -4480,54 +4833,71 @@
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
 
     def from_map(self, m=None):
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
     def __init__(self, price_info=None, request_id=None, success=None):
```

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/alibabacloud_foasconsole20190601_py2.egg-info/PKG-INFO` & `alibabacloud_foasconsole20190601_py2-1.0.3/alibabacloud_foasconsole20190601_py2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-foasconsole20190601-py2
-Version: 1.0.2
+Version: 1.0.3
 Summary: Alibaba Cloud foasconsole (20190601) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_foasconsole20190601_py2-1.0.2/setup.py` & `alibabacloud_foasconsole20190601_py2-1.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_foasconsole20190601_py2.
 
-Created on 04/02/2024
+Created on 07/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_foasconsole20190601"
 NAME = "alibabacloud_foasconsole20190601_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud foasconsole (20190601) SDK Library for Python2"
```

