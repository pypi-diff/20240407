# Comparing `tmp/check_params_by_swagger-1.0.0.tar.gz` & `tmp/check_params_by_swagger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/check_params_by_swagger-1.0.0.tar", last modified: Sun Apr  7 14:15:13 2024, max compression
+gzip compressed data, was "dist/check_params_by_swagger-1.0.1.tar", last modified: Sun Apr  7 14:06:52 2024, max compression
```

## Comparing `check_params_by_swagger-1.0.0.tar` & `check_params_by_swagger-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/
--rwxrwxrwx   0 root         (0) root         (0)     1073 2024-04-04 15:22:37.000000 check_params_by_swagger-1.0.0/LICENSE.txt
--rwxrwxrwx   0 root         (0) root         (0)     1977 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1581 2024-04-07 13:40:20.000000 check_params_by_swagger-1.0.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/check_params_by_swagger/
--rwxrwxrwx   0 root         (0) root         (0)      180 2024-04-03 16:00:09.000000 check_params_by_swagger-1.0.0/check_params_by_swagger/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    32066 2024-04-07 14:14:39.000000 check_params_by_swagger-1.0.0/check_params_by_swagger/check.py
--rwxrwxrwx   0 root         (0) root         (0)      602 2024-04-04 16:03:48.000000 check_params_by_swagger-1.0.0/check_params_by_swagger/expected_code.py
--rwxrwxrwx   0 root         (0) root         (0)     1235 2024-04-04 16:28:05.000000 check_params_by_swagger-1.0.0/check_params_by_swagger/log_file.py
--rwxrwxrwx   0 root         (0) root         (0)    40555 2024-04-04 16:16:34.000000 check_params_by_swagger-1.0.0/check_params_by_swagger/swagger_parser.py
--rwxrwxrwx   0 root         (0) root         (0)     1169 2024-04-07 12:52:15.000000 check_params_by_swagger-1.0.0/check_params_by_swagger/util.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/check_params_by_swagger.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     1977 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/check_params_by_swagger.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      438 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/check_params_by_swagger.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/check_params_by_swagger.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       24 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/check_params_by_swagger.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-07 14:15:13.000000 check_params_by_swagger-1.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1115 2024-04-07 14:15:10.000000 check_params_by_swagger-1.0.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/
+-rwxrwxrwx   0 root         (0) root         (0)     1073 2024-04-04 15:22:37.000000 check_params_by_swagger-1.0.1/LICENSE.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1977 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1581 2024-04-07 13:40:20.000000 check_params_by_swagger-1.0.1/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/check_params_by_swagger/
+-rwxrwxrwx   0 root         (0) root         (0)      180 2024-04-03 16:00:09.000000 check_params_by_swagger-1.0.1/check_params_by_swagger/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    32066 2024-04-07 13:40:20.000000 check_params_by_swagger-1.0.1/check_params_by_swagger/check.py
+-rwxrwxrwx   0 root         (0) root         (0)      602 2024-04-04 16:03:48.000000 check_params_by_swagger-1.0.1/check_params_by_swagger/expected_code.py
+-rwxrwxrwx   0 root         (0) root         (0)     1235 2024-04-04 16:28:05.000000 check_params_by_swagger-1.0.1/check_params_by_swagger/log_file.py
+-rwxrwxrwx   0 root         (0) root         (0)    40555 2024-04-04 16:16:34.000000 check_params_by_swagger-1.0.1/check_params_by_swagger/swagger_parser.py
+-rwxrwxrwx   0 root         (0) root         (0)     1169 2024-04-07 12:52:15.000000 check_params_by_swagger-1.0.1/check_params_by_swagger/util.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/check_params_by_swagger.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)     1977 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/check_params_by_swagger.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      438 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/check_params_by_swagger.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/check_params_by_swagger.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       24 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/check_params_by_swagger.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-07 14:06:52.000000 check_params_by_swagger-1.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1115 2024-04-07 14:06:48.000000 check_params_by_swagger-1.0.1/setup.py
```

### Comparing `check_params_by_swagger-1.0.0/LICENSE.txt` & `check_params_by_swagger-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `check_params_by_swagger-1.0.0/PKG-INFO` & `check_params_by_swagger-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check_params_by_swagger
-Version: 1.0.0
+Version: 1.0.1
 Summary: check param by swagger
 Home-page: 
 Author: Qredsun
 Author-email: 1410672725@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `check_params_by_swagger-1.0.0/README.md` & `check_params_by_swagger-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `check_params_by_swagger-1.0.0/check_params_by_swagger/check.py` & `check_params_by_swagger-1.0.1/check_params_by_swagger/check.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         temp_file = 'temp.json'
 
         def save_swagger_from_url(swagger_doc_url):
             try:
                 swagger_doc = requests.get(swagger_doc_url).json()
                 if swagger_doc is None or 'swagger' not in swagger_doc:
                     raise KeyError(f'{swagger_doc_url} 解析出错！')
-                with open(temp_file, 'w', encoding='utf8') as fp:
+                with open(temp_file, 'w', encoding='utf9') as fp:
                     json.dump(swagger_doc, fp, ensure_ascii=False, indent=4)
                 return True
             except Exception as e:
                 logger.error(f'保存PMS swagger 文档失败：{e}')
                 return False
 
         def read_swagger_from_json(file_name):
```

### Comparing `check_params_by_swagger-1.0.0/check_params_by_swagger/expected_code.py` & `check_params_by_swagger-1.0.1/check_params_by_swagger/expected_code.py`

 * *Files identical despite different names*

### Comparing `check_params_by_swagger-1.0.0/check_params_by_swagger/log_file.py` & `check_params_by_swagger-1.0.1/check_params_by_swagger/log_file.py`

 * *Files identical despite different names*

### Comparing `check_params_by_swagger-1.0.0/check_params_by_swagger/swagger_parser.py` & `check_params_by_swagger-1.0.1/check_params_by_swagger/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `check_params_by_swagger-1.0.0/check_params_by_swagger/util.py` & `check_params_by_swagger-1.0.1/check_params_by_swagger/util.py`

 * *Files identical despite different names*

### Comparing `check_params_by_swagger-1.0.0/check_params_by_swagger.egg-info/PKG-INFO` & `check_params_by_swagger-1.0.1/check_params_by_swagger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: check-params-by-swagger
-Version: 1.0.0
+Version: 1.0.1
 Summary: check param by swagger
 Home-page: 
 Author: Qredsun
 Author-email: 1410672725@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `check_params_by_swagger-1.0.0/setup.py` & `check_params_by_swagger-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import setuptools  # 导入setuptools打包工具
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="check_params_by_swagger",  # 用自己的名替换其中的YOUR_USERNAME_
-    version="1.0.0",  # 包版本号，便于维护版本
+    version="1.0.1",  # 包版本号，便于维护版本
     author="Qredsun",  # 作者，可以写自己的姓名
     author_email="1410672725@qq.com",  # 作者联系方式，可写自己的邮箱地址
     description="check param by swagger",  # 包的简述
     long_description=long_description,  # 包的详细介绍，一般在README.md文件内
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

