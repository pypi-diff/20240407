# Comparing `tmp/pyresp-1.0.2.tar.gz` & `tmp/pyresp-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyresp-1.0.2.tar", last modified: Mon Mar 25 13:19:15 2024, max compression
+gzip compressed data, was "pyresp-1.0.3.tar", last modified: Sun Apr  7 14:53:03 2024, max compression
```

## Comparing `pyresp-1.0.2.tar` & `pyresp-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:19:15.610893 pyresp-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-25 13:19:07.000000 pyresp-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-25 13:19:15.610893 pyresp-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-25 13:19:07.000000 pyresp-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:19:15.606893 pyresp-1.0.2/pyresp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:19:07.000000 pyresp-1.0.2/pyresp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-25 13:19:07.000000 pyresp-1.0.2/pyresp/pyresp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:19:15.610893 pyresp-1.0.2/pyresp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-25 13:19:15.000000 pyresp-1.0.2/pyresp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-25 13:19:15.000000 pyresp-1.0.2/pyresp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:19:15.000000 pyresp-1.0.2/pyresp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 13:19:15.000000 pyresp-1.0.2/pyresp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 13:19:15.000000 pyresp-1.0.2/pyresp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:19:15.000000 pyresp-1.0.2/pyresp.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 13:19:15.610893 pyresp-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-25 13:19:07.000000 pyresp-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:53:03.375283 pyresp-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 14:52:51.000000 pyresp-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-07 14:53:03.375283 pyresp-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-07 14:52:51.000000 pyresp-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:53:03.371283 pyresp-1.0.3/pyresp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:52:51.000000 pyresp-1.0.3/pyresp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-07 14:52:51.000000 pyresp-1.0.3/pyresp/pyresp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:53:03.375283 pyresp-1.0.3/pyresp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-07 14:53:03.000000 pyresp-1.0.3/pyresp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-07 14:53:03.000000 pyresp-1.0.3/pyresp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:53:03.000000 pyresp-1.0.3/pyresp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 14:53:03.000000 pyresp-1.0.3/pyresp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 14:53:03.000000 pyresp-1.0.3/pyresp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:53:03.000000 pyresp-1.0.3/pyresp.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:53:03.375283 pyresp-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-07 14:52:51.000000 pyresp-1.0.3/setup.py
```

### Comparing `pyresp-1.0.2/LICENSE` & `pyresp-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyresp-1.0.2/pyresp/pyresp.py` & `pyresp-1.0.3/pyresp/pyresp.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,15 +19,17 @@
             }
     else:
         response_data = {
             'code': code,
             'message': message,
             'data': data,
         }
-    logging.info(f'接口返回：{response_data}')
+    logging.info(f'\033[0;31m接口返回 {code}：'
+                 f'\033[0;32m{response_data}\033[0m'
+                 )
     return JSONResponse(
         status_code=status.HTTP_200_OK,
         content=response_data
     )
 
 
 def resp_400(code: int = 400, message='错误，请重试！'):
@@ -35,12 +37,14 @@
     400系列的响应结构体
     *：代表调用方法时必须传参数
     """
     response_data = {
         'code': code,
         'message': message,
     }
-    logging.error(f'接口返回：{response_data}')
+    logging.error(f'\033[0;31m接口返回 {code}：'
+                 f'{response_data}\033[0m'
+                 )
     return JSONResponse(
         status_code=status.HTTP_400_BAD_REQUEST,
         content=response_data
     )
```

### Comparing `pyresp-1.0.2/setup.py` & `pyresp-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
 
 
 setup(
     name='pyresp',
-    version='1.0.2',
+    version='1.0.3',
     description='fastapi的通用返回助手',
     author='buyfakett',
     author_email='buyfakett@vip.qq.com',
     license='MIT',
     url="https://github.com/buyfakett",
     packages=find_packages(),  # packages=["pytest"],
     long_description=long_description,
```

