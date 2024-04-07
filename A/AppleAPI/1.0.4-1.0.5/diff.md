# Comparing `tmp/AppleAPI-1.0.4.tar.gz` & `tmp/AppleAPI-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppleAPI-1.0.4.tar", last modified: Mon Mar 18 08:19:31 2024, max compression
+gzip compressed data, was "AppleAPI-1.0.5.tar", last modified: Sun Apr  7 08:04:49 2024, max compression
```

## Comparing `AppleAPI-1.0.4.tar` & `AppleAPI-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:19:31.052536 AppleAPI-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:19:31.048535 AppleAPI-1.0.4/AppleAPI/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-18 08:19:26.000000 AppleAPI-1.0.4/AppleAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36645 2024-03-18 08:19:26.000000 AppleAPI-1.0.4/AppleAPI/apple_api_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    14578 2024-03-18 08:19:26.000000 AppleAPI-1.0.4/AppleAPI/appstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    14348 2024-03-18 08:19:26.000000 AppleAPI-1.0.4/AppleAPI/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 08:19:31.052536 AppleAPI-1.0.4/AppleAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-03-18 08:19:31.000000 AppleAPI-1.0.4/AppleAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-18 08:19:31.000000 AppleAPI-1.0.4/AppleAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 08:19:31.000000 AppleAPI-1.0.4/AppleAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-18 08:19:31.000000 AppleAPI-1.0.4/AppleAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-18 08:19:31.000000 AppleAPI-1.0.4/AppleAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-18 08:19:26.000000 AppleAPI-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-03-18 08:19:31.052536 AppleAPI-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-18 08:19:26.000000 AppleAPI-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 08:19:31.052536 AppleAPI-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-18 08:19:26.000000 AppleAPI-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/AppleAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/apple_api_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/appstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/AppleAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/setup.py
```

### Comparing `AppleAPI-1.0.4/AppleAPI/apple_api_agent.py` & `AppleAPI-1.0.5/AppleAPI/apple_api_agent.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,28 +360,28 @@
             kdf_rounds(50000).
             key_cert_algorithm(pkcs12.PBES.PBESv1SHA1And3KeyTripleDESCBC).
             hmac_hash(hashes.SHA1()).build(password.encode("utf-8"))
         )
         p12 = pkcs12.serialize_key_and_certificates(None, privateKey, cert, None, encryption)
         save_path.write_bytes(p12)
 
-    def create_certificates_export_p12(self, info:CertificateInfo):
+    def create_certificates_export_p12(self, is_dev:bool, email:str, developer_name:str, password:str, country:str, save_path:Path):
         """创建dis证书，并保存成p12"""
         # 创建CSR文件
-        key, csrContent = self.make_csr_content(info.developer_name, info.email, info.country_name)
+        key, csrContent = self.make_csr_content(developer_name, email, country)
         # 找出 begin和end之间内容
         pattern = '-----BEGIN[^-]+-----(.+)-----END[^-]+-----'
         result = re.search(pattern, str(csrContent, 'UTF-8'), flags=re.DOTALL)
         csr_content = result.group(1).replace('\n', '')  # 删除所有换行符
-        certificate_type = CertificateType.DEVELOPMENT if info.is_dev else CertificateType.DISTRIBUTION
+        certificate_type = CertificateType.DEVELOPMENT if is_dev else CertificateType.DISTRIBUTION
         cer = self.create_certificates(csr_content=csr_content, certificate_type=certificate_type)
         if cer.attributes.certificate_content:
             cer_content = base64.b64decode(cer.attributes.certificate_content)
             # 将cer和私钥合并成p12
-            self.export_p12(cer_content, key, save_path=info.save_path, password=info.password)
+            self.export_p12(cer_content, key, save_path=save_path, password=password)
         else:
             raise ValueError('创建证书失败')
 
     def list_bundle_id(self, filters: Dict = None, verbose=False) -> List[BundleId]:
         """
         bundle id 列表
         https://developer.apple.com/documentation/appstoreconnectapi/list_bundle_ids
```

### Comparing `AppleAPI-1.0.4/AppleAPI/appstore.py` & `AppleAPI-1.0.5/AppleAPI/appstore.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,23 +83,15 @@
         if not developer_name:
             die('name不能为空')
         if not password:
             die('password不能为空')
         title = 'dev' if is_dev else 'dis'
         print(f'开始创建{title}证书')
         save_path = self.p12Path(is_dev, password=password)
-        info =  CertificateInfo(
-            is_dev=is_dev,
-            email=email,
-            password=password,
-            developer_name=developer_name,
-            country_name=country,
-            save_path=save_path
-        )
-        self.agent.create_certificates_export_p12(info)
+        self.agent.create_certificates_export_p12(is_dev=is_dev, email=email, developer_name=developer_name, password=password, country=country, save_path=save_path)
         print(f'{title}证书保存成功:{save_path}')
 
     def create_bundle_id(self, bundle_id:str, bundle_name:str, capabilitys: List[str]=None):
         """
         创建Bundle Id
         @param bundle_id: 唯一标识
         @param bundle_name: 名称
```

### Comparing `AppleAPI-1.0.4/AppleAPI/models.py` & `AppleAPI-1.0.5/AppleAPI/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,26 +8,14 @@
 import tempfile
 from collections import namedtuple
 from datetime import datetime
 from enum import Enum, auto
 from pathlib import Path
 from typing import Dict, Union
 
-from mobileprovision.parser import MobileProvisionModel
-
-class CertificateInfo:
-    """创建证书相关参数"""
-    def __init__(self, is_dev:bool = True, email: str = None, password:str = None, developer_name: str = None, country_name: str = None, save_path:Path = None) -> None:
-        self.is_dev = is_dev
-        self.email = email
-        self.password = password
-        self.developer_name = developer_name
-        self.country_name = country_name
-        self.save_path = save_path
-
 class EnumAutoName(Enum):
     def _generate_next_value_(name, start, count, last_values):
         return name
 
 
 class DeviceStatus(EnumAutoName):
     """设备的状态"""
```

### Comparing `AppleAPI-1.0.4/AppleAPI.egg-info/PKG-INFO` & `AppleAPI-1.0.5/AppleAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppleAPI
-Version: 1.0.4
+Version: 1.0.5
 Summary: App Store Connect API
 Home-page: https://github.com/yingguqing/AppleAPI
 Author: 影孤清
 Author-email: yingguqing@163.com
 Keywords: ios apple appstore app store connect api appstoreconnectapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,20 @@
 Requires-Dist: pyOpenSSL>=20.0.0
 Requires-Dist: requests~=2.20
 
 # AppleAPI
 基于appstore connect api封装功能。
 代码是基于[OKAppleAPI](https://github.com/shede333/OKAppleAPI)原码。只是在原代码基础上，新增了部分接口，封装了些自用功能。
 
+## 安装
+```
+pip3 install appleapi
+```
 
-
-用法:
+## 用法
 
 ```python
 #!/usr/bin/python3
 # coding=utf-8
 
 from AppleAPI import AppStore
 
@@ -54,14 +57,15 @@
     bundle_id = 'com.test.test.a.b'
     name = 'Test'
     email = 'test@test.com'
     developer_name = 'Name'
     country = 'US'
     password = '123'
     appstore_version = '1.0'
+    # 可以填写相对此文件的相对路径
     screenshots = {
         'zh-Hans' : {
             "APP_IPHONE_67"             : "C:/Users/Administrator/Desktop/python/iPhone14PM-6.7",
             # "APP_IPHONE_65"           : "iPhone11PM-6.5",
             # "APP_IPHONE_55"           : "iPhone8P-5.5",
             # "APP_IPAD_PRO_3GEN_129"   : "iPadPro-12.9",
             # "APP_IPAD_PRO_129"        : "iPadPro-12.9",
```

### Comparing `AppleAPI-1.0.4/LICENSE` & `AppleAPI-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.4/PKG-INFO` & `AppleAPI-1.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppleAPI
-Version: 1.0.4
+Version: 1.0.5
 Summary: App Store Connect API
 Home-page: https://github.com/yingguqing/AppleAPI
 Author: 影孤清
 Author-email: yingguqing@163.com
 Keywords: ios apple appstore app store connect api appstoreconnectapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -20,17 +20,20 @@
 Requires-Dist: pyOpenSSL>=20.0.0
 Requires-Dist: requests~=2.20
 
 # AppleAPI
 基于appstore connect api封装功能。
 代码是基于[OKAppleAPI](https://github.com/shede333/OKAppleAPI)原码。只是在原代码基础上，新增了部分接口，封装了些自用功能。
 
+## 安装
+```
+pip3 install appleapi
+```
 
-
-用法:
+## 用法
 
 ```python
 #!/usr/bin/python3
 # coding=utf-8
 
 from AppleAPI import AppStore
 
@@ -54,14 +57,15 @@
     bundle_id = 'com.test.test.a.b'
     name = 'Test'
     email = 'test@test.com'
     developer_name = 'Name'
     country = 'US'
     password = '123'
     appstore_version = '1.0'
+    # 可以填写相对此文件的相对路径
     screenshots = {
         'zh-Hans' : {
             "APP_IPHONE_67"             : "C:/Users/Administrator/Desktop/python/iPhone14PM-6.7",
             # "APP_IPHONE_65"           : "iPhone11PM-6.5",
             # "APP_IPHONE_55"           : "iPhone8P-5.5",
             # "APP_IPAD_PRO_3GEN_129"   : "iPadPro-12.9",
             # "APP_IPAD_PRO_129"        : "iPadPro-12.9",
```

### Comparing `AppleAPI-1.0.4/README.md` & `AppleAPI-1.0.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # AppleAPI
 基于appstore connect api封装功能。
 代码是基于[OKAppleAPI](https://github.com/shede333/OKAppleAPI)原码。只是在原代码基础上，新增了部分接口，封装了些自用功能。
 
+## 安装
+```
+pip3 install appleapi
+```
 
-
-用法:
+## 用法
 
 ```python
 #!/usr/bin/python3
 # coding=utf-8
 
 from AppleAPI import AppStore
 
@@ -32,14 +35,15 @@
     bundle_id = 'com.test.test.a.b'
     name = 'Test'
     email = 'test@test.com'
     developer_name = 'Name'
     country = 'US'
     password = '123'
     appstore_version = '1.0'
+    # 可以填写相对此文件的相对路径
     screenshots = {
         'zh-Hans' : {
             "APP_IPHONE_67"             : "C:/Users/Administrator/Desktop/python/iPhone14PM-6.7",
             # "APP_IPHONE_65"           : "iPhone11PM-6.5",
             # "APP_IPHONE_55"           : "iPhone8P-5.5",
             # "APP_IPAD_PRO_3GEN_129"   : "iPadPro-12.9",
             # "APP_IPAD_PRO_129"        : "iPadPro-12.9",
```

### Comparing `AppleAPI-1.0.4/setup.py` & `AppleAPI-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = Path(__file__).resolve().with_name("README.md").read_text()
 
 print("{} - {}".format("*" * 10, find_packages()))
 
 setup(
     name='AppleAPI',  # 包名字
-    version='1.0.4',  # 包版本
+    version='1.0.5',  # 包版本
     author='影孤清',  # 作者
     author_email='yingguqing@163.com',  # 作者邮箱
     keywords='ios apple appstore app store connect api appstoreconnectapi',
     description='App Store Connect API',  # 简单描述
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/yingguqing/AppleAPI',  # 包的主页
```

