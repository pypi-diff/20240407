# Comparing `tmp/AppleAPI-1.0.5.tar.gz` & `tmp/AppleAPI-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AppleAPI-1.0.5.tar", last modified: Sun Apr  7 08:04:49 2024, max compression
+gzip compressed data, was "AppleAPI-1.0.6.tar", last modified: Sun Apr  7 08:09:14 2024, max compression
```

## Comparing `AppleAPI-1.0.5.tar` & `AppleAPI-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/AppleAPI/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/apple_api_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/appstore.py
--rw-r--r--   0 runner    (1001) docker     (127)    13853 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/AppleAPI/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/AppleAPI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 08:04:49.000000 AppleAPI-1.0.5/AppleAPI.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:04:49.884619 AppleAPI-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-07 08:04:43.000000 AppleAPI-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:09:14.937566 AppleAPI-1.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:09:14.937566 AppleAPI-1.0.6/AppleAPI/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 08:09:10.000000 AppleAPI-1.0.6/AppleAPI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36675 2024-04-07 08:09:10.000000 AppleAPI-1.0.6/AppleAPI/apple_api_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14453 2024-04-07 08:09:10.000000 AppleAPI-1.0.6/AppleAPI/appstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13391 2024-04-07 08:09:10.000000 AppleAPI-1.0.6/AppleAPI/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:09:14.937566 AppleAPI-1.0.6/AppleAPI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:09:14.000000 AppleAPI-1.0.6/AppleAPI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-07 08:09:14.000000 AppleAPI-1.0.6/AppleAPI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:09:14.000000 AppleAPI-1.0.6/AppleAPI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 08:09:14.000000 AppleAPI-1.0.6/AppleAPI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 08:09:14.000000 AppleAPI-1.0.6/AppleAPI.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 08:09:10.000000 AppleAPI-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 08:09:14.937566 AppleAPI-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-04-07 08:09:10.000000 AppleAPI-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:09:14.937566 AppleAPI-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-07 08:09:10.000000 AppleAPI-1.0.6/setup.py
```

### Comparing `AppleAPI-1.0.5/AppleAPI/apple_api_agent.py` & `AppleAPI-1.0.6/AppleAPI/apple_api_agent.py`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.5/AppleAPI/appstore.py` & `AppleAPI-1.0.6/AppleAPI/appstore.py`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.5/AppleAPI/models.py` & `AppleAPI-1.0.6/AppleAPI/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -204,25 +204,14 @@
         self.name = attributes.get('name')
         self.uuid = attributes.get('uuid')
         self.profile_content = attributes.get('profileContent')
         self.created_date = datetime.fromisoformat(attributes.get('createdDate'))
         self.expiration_date = datetime.fromisoformat(attributes.get('expirationDate'))
         self.profile_type = attributes.get('profileType')
 
-        self._mobile_provision = None
-
-    @property
-    def mobile_provision(self) -> MobileProvisionModel:
-        if not self._mobile_provision:
-            with tempfile.TemporaryDirectory() as temp_dir_path:
-                tmp_file_path = Path(temp_dir_path).joinpath('tmp.mobileprovision')
-                self.save_content(tmp_file_path)
-                self._mobile_provision = MobileProvisionModel(tmp_file_path)
-        return self._mobile_provision
-
     @property
     def platform(self) -> BundleIdPlatform:
         """设备系统类型"""
         return BundleIdPlatform(self.attributes.get('platform'))
 
     @property
     def is_active(self) -> bool:
```

### Comparing `AppleAPI-1.0.5/AppleAPI.egg-info/PKG-INFO` & `AppleAPI-1.0.6/AppleAPI.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppleAPI
-Version: 1.0.5
+Version: 1.0.6
 Summary: App Store Connect API
 Home-page: https://github.com/yingguqing/AppleAPI
 Author: 影孤清
 Author-email: yingguqing@163.com
 Keywords: ios apple appstore app store connect api appstoreconnectapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AppleAPI-1.0.5/LICENSE` & `AppleAPI-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.5/PKG-INFO` & `AppleAPI-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AppleAPI
-Version: 1.0.5
+Version: 1.0.6
 Summary: App Store Connect API
 Home-page: https://github.com/yingguqing/AppleAPI
 Author: 影孤清
 Author-email: yingguqing@163.com
 Keywords: ios apple appstore app store connect api appstoreconnectapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AppleAPI-1.0.5/README.md` & `AppleAPI-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `AppleAPI-1.0.5/setup.py` & `AppleAPI-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = Path(__file__).resolve().with_name("README.md").read_text()
 
 print("{} - {}".format("*" * 10, find_packages()))
 
 setup(
     name='AppleAPI',  # 包名字
-    version='1.0.5',  # 包版本
+    version='1.0.6',  # 包版本
     author='影孤清',  # 作者
     author_email='yingguqing@163.com',  # 作者邮箱
     keywords='ios apple appstore app store connect api appstoreconnectapi',
     description='App Store Connect API',  # 简单描述
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/yingguqing/AppleAPI',  # 包的主页
```

