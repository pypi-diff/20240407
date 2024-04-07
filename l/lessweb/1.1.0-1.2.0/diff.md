# Comparing `tmp/lessweb-1.1.0.tar.gz` & `tmp/lessweb-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-1.1.0.tar", last modified: Tue Apr  2 03:30:00 2024, max compression
+gzip compressed data, was "lessweb-1.2.0.tar", last modified: Sun Apr  7 07:34:04 2024, max compression
```

## Comparing `lessweb-1.1.0.tar` & `lessweb-1.2.0.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.389198 lessweb-1.1.0/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.380889 lessweb-1.1.0/.github/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.382704 lessweb-1.1.0/.github/workflows/
--rw-r--r--   0 zhangji    (502) staff       (20)      941 2024-03-28 06:37:50.000000 lessweb-1.1.0/.github/workflows/python-package.yml
--rw-r--r--   0 zhangji    (502) staff       (20)     1093 2024-03-28 06:00:47.000000 lessweb-1.1.0/.gitignore
--rw-r--r--   0 zhangji    (502) staff       (20)      556 2024-03-28 00:41:05.000000 lessweb-1.1.0/LICENSE.txt
--rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-02 03:30:00.388945 lessweb-1.1.0/PKG-INFO
--rw-r--r--   0 zhangji    (502) staff       (20)     1706 2024-03-28 00:41:05.000000 lessweb-1.1.0/README.md
--rw-r--r--   0 zhangji    (502) staff       (20)      315 2024-03-28 06:43:43.000000 lessweb-1.1.0/changelog.md
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.381551 lessweb-1.1.0/examples/
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.382949 lessweb-1.1.0/examples/100_hello_world/
--rw-r--r--   0 zhangji    (502) staff       (20)      244 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/100_hello_world/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.383380 lessweb-1.1.0/examples/100_hello_world_config/
--rw-r--r--   0 zhangji    (502) staff       (20)       21 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/100_hello_world_config/config.toml
--rw-r--r--   0 zhangji    (502) staff       (20)      264 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/100_hello_world_config/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.383592 lessweb-1.1.0/examples/101_handle_request/
--rw-r--r--   0 zhangji    (502) staff       (20)      676 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/101_handle_request/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384201 lessweb-1.1.0/examples/102_response/
--rw-r--r--   0 zhangji    (502) staff       (20)     1284 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/102_response/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384399 lessweb-1.1.0/examples/103_get_request/
--rw-r--r--   0 zhangji    (502) staff       (20)      772 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/103_get_request/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384737 lessweb-1.1.0/examples/205_mysql_crud/
--rw-r--r--   0 zhangji    (502) staff       (20)      169 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/config.toml
--rw-r--r--   0 zhangji    (502) staff       (20)      370 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384978 lessweb-1.1.0/examples/205_mysql_crud/myapp/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/__init__.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385406 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)      211 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/create_pet.py
--rw-r--r--   0 zhangji    (502) staff       (20)      225 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/get_pet_detail.py
--rw-r--r--   0 zhangji    (502) staff       (20)      295 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/get_pet_total.py
--rw-r--r--   0 zhangji    (502) staff       (20)     1544 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/mapper.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385526 lessweb-1.1.0/examples/205_mysql_crud/schema/
--rw-r--r--   0 zhangji    (502) staff       (20)      307 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/schema/pet.sql
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385639 lessweb-1.1.0/examples/302_cookie/
--rw-r--r--   0 zhangji    (502) staff       (20)      550 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/302_cookie/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385834 lessweb-1.1.0/examples/303_middleware/
--rw-r--r--   0 zhangji    (502) staff       (20)      533 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/303_middleware/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.386017 lessweb-1.1.0/examples/304_websocket/
--rw-r--r--   0 zhangji    (502) staff       (20)     1198 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/304_websocket/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.386602 lessweb-1.1.0/examples/305_schedule_task/
--rw-r--r--   0 zhangji    (502) staff       (20)      814 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/305_schedule_task/index.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.387241 lessweb-1.1.0/lessweb/
--rw-r--r--   0 zhangji    (502) staff       (20)      232 2024-03-28 00:41:05.000000 lessweb-1.1.0/lessweb/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)    14739 2024-03-28 06:00:47.000000 lessweb-1.1.0/lessweb/bridge.py
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.1.0/lessweb/py.typed
--rw-r--r--   0 zhangji    (502) staff       (20)     8932 2024-03-28 06:06:02.000000 lessweb-1.1.0/lessweb/typecast.py
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.388551 lessweb-1.1.0/lessweb.egg-info/
--rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (502) staff       (20)     1178 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (502) staff       (20)        1 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       43 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/requires.txt
--rw-r--r--   0 zhangji    (502) staff       (20)        8 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       62 2024-03-28 06:00:47.000000 lessweb-1.1.0/mypy.ini
--rw-r--r--   0 zhangji    (502) staff       (20)      538 2024-03-28 06:40:38.000000 lessweb-1.1.0/pyproject.toml
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.388116 lessweb-1.1.0/requirements/
--rw-r--r--   0 zhangji    (502) staff       (20)       42 2024-03-28 06:00:47.000000 lessweb-1.1.0/requirements/base.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       66 2024-03-28 06:00:47.000000 lessweb-1.1.0/requirements/test.txt
--rw-r--r--   0 zhangji    (502) staff       (20)       38 2024-04-02 03:30:00.389232 lessweb-1.1.0/setup.cfg
-drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.388292 lessweb-1.1.0/tests/
--rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 06:00:47.000000 lessweb-1.1.0/tests/__init__.py
--rw-r--r--   0 zhangji    (502) staff       (20)     3916 2024-03-28 06:12:06.000000 lessweb-1.1.0/tests/test_typecast.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.523677 lessweb-1.2.0/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.515708 lessweb-1.2.0/.github/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.517634 lessweb-1.2.0/.github/workflows/
+-rw-r--r--   0 zhangji    (502) staff       (20)      941 2024-03-28 06:37:50.000000 lessweb-1.2.0/.github/workflows/python-package.yml
+-rw-r--r--   0 zhangji    (502) staff       (20)     1093 2024-03-28 06:00:47.000000 lessweb-1.2.0/.gitignore
+-rw-r--r--   0 zhangji    (502) staff       (20)      556 2024-03-28 00:41:05.000000 lessweb-1.2.0/LICENSE.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-07 07:34:04.523489 lessweb-1.2.0/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1706 2024-03-28 00:41:05.000000 lessweb-1.2.0/README.md
+-rw-r--r--   0 zhangji    (502) staff       (20)      315 2024-03-28 06:43:43.000000 lessweb-1.2.0/changelog.md
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.516368 lessweb-1.2.0/examples/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.517879 lessweb-1.2.0/examples/100_hello_world/
+-rw-r--r--   0 zhangji    (502) staff       (20)      244 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/100_hello_world/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.518266 lessweb-1.2.0/examples/100_hello_world_config/
+-rw-r--r--   0 zhangji    (502) staff       (20)       21 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/100_hello_world_config/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      264 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/100_hello_world_config/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.518447 lessweb-1.2.0/examples/101_handle_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      676 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/101_handle_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.518977 lessweb-1.2.0/examples/102_response/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1284 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/102_response/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519096 lessweb-1.2.0/examples/103_get_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      772 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/103_get_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519315 lessweb-1.2.0/examples/205_mysql_crud/
+-rw-r--r--   0 zhangji    (502) staff       (20)      169 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      370 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519499 lessweb-1.2.0/examples/205_mysql_crud/myapp/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/__init__.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.519936 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      211 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/create_pet.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      225 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/get_pet_detail.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      295 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/endpoint/get_pet_total.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     1544 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/myapp/mapper.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520059 lessweb-1.2.0/examples/205_mysql_crud/schema/
+-rw-r--r--   0 zhangji    (502) staff       (20)      307 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/205_mysql_crud/schema/pet.sql
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520176 lessweb-1.2.0/examples/302_cookie/
+-rw-r--r--   0 zhangji    (502) staff       (20)      550 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/302_cookie/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520360 lessweb-1.2.0/examples/303_middleware/
+-rw-r--r--   0 zhangji    (502) staff       (20)      533 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/303_middleware/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.520548 lessweb-1.2.0/examples/304_websocket/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1198 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/304_websocket/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.521183 lessweb-1.2.0/examples/305_schedule_task/
+-rw-r--r--   0 zhangji    (502) staff       (20)      814 2024-03-28 00:41:05.000000 lessweb-1.2.0/examples/305_schedule_task/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.521773 lessweb-1.2.0/lessweb/
+-rw-r--r--   0 zhangji    (502) staff       (20)      232 2024-03-28 00:41:05.000000 lessweb-1.2.0/lessweb/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)    15065 2024-04-07 07:32:44.000000 lessweb-1.2.0/lessweb/bridge.py
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.2.0/lessweb/py.typed
+-rw-r--r--   0 zhangji    (502) staff       (20)    10000 2024-04-07 06:49:29.000000 lessweb-1.2.0/lessweb/typecast.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.523238 lessweb-1.2.0/lessweb.egg-info/
+-rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1178 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        1 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       43 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        8 2024-04-07 07:34:04.000000 lessweb-1.2.0/lessweb.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       62 2024-03-28 06:00:47.000000 lessweb-1.2.0/mypy.ini
+-rw-r--r--   0 zhangji    (502) staff       (20)      538 2024-04-07 07:17:36.000000 lessweb-1.2.0/pyproject.toml
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.522696 lessweb-1.2.0/requirements/
+-rw-r--r--   0 zhangji    (502) staff       (20)       42 2024-03-28 06:00:47.000000 lessweb-1.2.0/requirements/base.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       66 2024-03-28 06:00:47.000000 lessweb-1.2.0/requirements/test.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       38 2024-04-07 07:34:04.523711 lessweb-1.2.0/setup.cfg
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-07 07:34:04.523021 lessweb-1.2.0/tests/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 06:00:47.000000 lessweb-1.2.0/tests/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     4669 2024-04-07 06:48:10.000000 lessweb-1.2.0/tests/test_typecast.py
```

### Comparing `lessweb-1.1.0/.github/workflows/python-package.yml` & `lessweb-1.2.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/.gitignore` & `lessweb-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/LICENSE.txt` & `lessweb-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/PKG-INFO` & `lessweb-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lessweb
-Version: 1.1.0
+Version: 1.2.0
 Summary: A pythonic web framework
 Author-email: qorzj <goodhorsezxj@gmail.com>
 License: Apache 2
 Keywords: lessweb,web,web.py,aiohttp
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `lessweb-1.1.0/README.md` & `lessweb-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/101_handle_request/index.py` & `lessweb-1.2.0/examples/101_handle_request/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/102_response/index.py` & `lessweb-1.2.0/examples/102_response/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/103_get_request/index.py` & `lessweb-1.2.0/examples/103_get_request/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/205_mysql_crud/myapp/mapper.py` & `lessweb-1.2.0/examples/205_mysql_crud/myapp/mapper.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/302_cookie/index.py` & `lessweb-1.2.0/examples/302_cookie/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/303_middleware/index.py` & `lessweb-1.2.0/examples/303_middleware/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/304_websocket/index.py` & `lessweb-1.2.0/examples/304_websocket/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/examples/305_schedule_task/index.py` & `lessweb-1.2.0/examples/305_schedule_task/index.py`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/lessweb/bridge.py` & `lessweb-1.2.0/lessweb/bridge.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,28 @@
 import inspect
 import logging
 import re
 import sys
 from dataclasses import dataclass, is_dataclass
 from logging.handlers import TimedRotatingFileHandler
 from os import environ, listdir
-from typing import Any, Dict, Optional, Type, TypeVar, Union
+from typing import (Any, Awaitable, Callable, Dict, Optional, Type, TypeVar,
+                    Union)
 
 import orjson
 import toml
 from aiohttp.typedefs import LooseHeaders
 from aiohttp.web import (Application, HTTPBadRequest, HTTPError, Request,
                          Response, middleware, run_app)
 
 from .typecast import is_typeddict, isinstance_safe, typecast
 
+ENDPOINT_TYPE = Callable[..., Awaitable[Any]]
+HANDLER_TYPE = Callable[[Request], Awaitable[Any]]
+
 T = TypeVar('T')
 ORJSON_OPTION = 0
 POSITIONAL_ONLY = 0
 KEYWORD_ONLY = 3
 
 
 def make_environ_key(key_path: str):
@@ -221,15 +225,15 @@
             include_doc = getdoc(line.replace(':include ', '').strip())
             result.append(include_doc)
         else:
             result.append(line)
     return '\n'.join(result) + '\n'
 
 
-def make_router(sp_endpoint):
+def make_router(sp_endpoint: ENDPOINT_TYPE) -> HANDLER_TYPE:
     """
     :param sp_endpoint:
         1.POSITIONAL_ONLY参数表示requestbody
         2.int和str类型参数表示路径参数
         3.其他参数支持可注入类型
     :return: 形如foo(request)这样的函数
     """
@@ -277,58 +281,56 @@
     return aio_endpoint
 
 
 @dataclass
 class Route:
     method: str
     paths: list
-    handler: Any
+    handler: HANDLER_TYPE
 
 
-def rest_mapping(method: str, paths: list):
+def rest_mapping(method: str, paths: list) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
         handler = make_router(sp_endpoint)
         route = Route(method=method.upper(), paths=paths, handler=handler)
         route.__doc__ = inspect.getdoc(sp_endpoint)
         return route
 
     return g
 
 
-def get_mapping(path: str):
+def get_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
-        handler = make_router(sp_endpoint)
         return rest_mapping(method='GET', paths=[path])(sp_endpoint)
 
     return g
 
 
-def post_mapping(path: str):
+def post_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
-        handler = make_router(sp_endpoint)
         return rest_mapping(method='POST', paths=[path])(sp_endpoint)
 
     return g
 
 
-def put_mapping(path: str):
+def put_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
         return rest_mapping(method='PUT', paths=[path])(sp_endpoint)
 
     return g
 
 
-def patch_mapping(path: str):
+def patch_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
         return rest_mapping(method='PATCH', paths=[path])(sp_endpoint)
 
     return g
 
 
-def delete_mapping(path: str):
+def delete_mapping(path: str) -> Callable[[ENDPOINT_TYPE], Route]:
     def g(sp_endpoint) -> Route:
         return rest_mapping(method='DELETE', paths=[path])(sp_endpoint)
 
     return g
 
 
 class Bridge:
@@ -416,15 +418,15 @@
             await make_app_signal(handler_on_cleanup)(app)
 
         self.app.cleanup_ctx.append(aio_handler)
 
     def add_on_shutdown(self, handler):
         self.app.on_shutdown.append(make_app_signal(handler))
 
-    def add_route(self, route):
+    def add_route(self, route: Route) -> None:
         for path in route.paths:
             self.app.router.add_route(
                 method=route.method, path=path, handler=route.handler)
 
     def add_route_scan(self, endpoint_package: str):
         endpoint_mdl = importlib.import_module(endpoint_package)
         if endpoint_mdl.__spec__ is None or not endpoint_mdl.__spec__.submodule_search_locations:
```

### Comparing `lessweb-1.1.0/lessweb/typecast.py` & `lessweb-1.2.0/lessweb/typecast.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import csv
 import datetime
 import enum
 import inspect
 import json
 import re
 import sys
-from typing import Any, Dict, List, Literal, Type, Union, get_type_hints
+from typing import (Any, Dict, List, Literal, NewType, Type, Union,
+                    get_type_hints)
 
 import typing_inspect
 
 
 class TypeCastError(Exception):
     pass
 
@@ -60,34 +61,37 @@
     inspect_type(int) => (int,)
     inspect_type(list) => (list,)
     inspect_type(list[int]) => (list, int)
     inspect_type(int | None) => (Union, (int, NoneType))
     inspect_type(int | str) => (Union, (int, str))
     inspect_type(int | str | None) => (Union, (int, str, NoneType))
     inspect_type(Literal['a', 'b']) => (Literal, ('a', 'b'))
+    inspect_type(NewType) => (NewType, __supertype__)
     inspect_type(dict) => (dict,)
     inspect_type(dict[str, int]) => NotImplementedError
     inspect_type(typeddict) => (dict, __annotations__)
     inspect_type(cls) => (cls,)
     inspect_type(_else_) => NotImplementedError
     """
     if isinstance_safe(tp, str):
         tp = classname_dict[tp]
     tp_origin = typing_inspect.get_origin(tp)
     tp_args = typing_inspect.get_args(tp)
     if tp_origin is None and tp_args == ():
         if is_typeddict(tp):
             classname_dict[tp.__qualname__] = tp
             return dict, get_type_hints(tp)
+        elif hasattr(tp, '__supertype__'):
+            return NewType, tp.__supertype__
         return (tp,)
-    if tp_origin is list:
+    elif tp_origin is list:
         return list, tp_args[0]
-    if (tp_origin is None or tp_origin == Union) and tp_args:
+    elif (tp_origin is None or tp_origin == Union) and tp_args:
         return Union, tp_args
-    if tp_origin == Literal and tp_args:
+    elif tp_origin == Literal and tp_args:
         return Literal, tp_args
     raise NotImplementedError(f'cannot inspect type {tp=}')
 
 
 def is_list_type(tp):
     return tp is list or typing_inspect.get_origin(tp) is list
 
@@ -96,21 +100,32 @@
     if isinstance_safe(tp, str):
         if tp not in classname_dict:
             raise TypeCastError(
                 f'typename {tp=} is not valid ref')  # 5xx Error in fact
         else:
             tp = classname_dict[tp]
     type_inspect_seed = inspect_type(tp)
-    if type_inspect_seed[0] == Literal:
+    if type_inspect_seed[0] == Union:
+        if len(type_inspect_seed) != 2 or not type_inspect_seed[1]:
+            raise TypeCastError(f'{tp=} is empty')  # 5xx Error in fact
+        for item in type_inspect_seed[1]:
+            try:
+                return typecast(data, item)
+            except:
+                continue
+        raise TypeCastError(f'{data=} is not any member of {tp=}')
+    elif type_inspect_seed[0] == Literal:
         if len(type_inspect_seed) != 2 or not type_inspect_seed[1]:
             raise TypeCastError(f'{tp=} is empty')  # 5xx Error in fact
         for item in type_inspect_seed[1]:
             if item == data:
                 return data
         raise TypeCastError(f'{data=} is not member of {tp=}')
+    elif type_inspect_seed[0] == NewType:
+        return typecast(data, type_inspect_seed[1])
     if isinstance_safe(data, tp):
         return data
     elif issubclass_safe(tp, enum.Enum):
         return tp(data)
     elif issubclass_safe(tp, datetime.datetime):
         return datetime.datetime.fromisoformat(data)
     elif issubclass_safe(tp, datetime.date):
@@ -121,20 +136,21 @@
         if issubclass_safe(tp, str):
             return tp(data)
         elif is_list_type(tp):
             data = parse_csv(data)
             return typecast(data, tp)
         else:
             try:
-                data = json.loads(data)
-                return typecast(data, tp)
+                loaded_data = json.loads(data)
             except:
                 if re.match(r'^\w*$', data):
                     raise TypeCastError(f'{data=} is not an instance of {tp=}')
-                raise
+                else:
+                    raise
+            return typecast(loaded_data, tp)
     else:
         if len(type_inspect_seed) != 2:
             raise TypeCastError(f'{data=} is not instance of {tp=}')
         origin_type, type_args = type_inspect_seed
         if origin_type is list:
             assert isinstance(data, list)
             return [typecast(item, type_args) for item in data]
@@ -211,14 +227,22 @@
     print(f'{union_optional_origin=}')  # union_optional_origin=typing.Union
 
     literral_args = typing_inspect.get_args(Literal['a', 'b'])
     literal_origin = typing_inspect.get_origin(Literal['a', 'b'])
     print(f'{literral_args=}')  # literral_args=('a', 'b')
     print(f'{literal_origin=}')  # literal_origin=typing.Literal
 
+    UserId = NewType('UserId', int)
+    newtype_args = typing_inspect.get_args(UserId)
+    newtype_origin = typing_inspect.get_origin(UserId)
+    print(f'{newtype_args=}')  # newtype_args=()
+    print(f'{newtype_origin=}')  # newtype_origin=None
+    # newtype.__supertype__=<class 'int'>
+    print(f'newtype.__supertype__={UserId.__supertype__}')  # type: ignore
+
     class Pet(typing.TypedDict):
         name: str
         age: int
     pet_optional_args = typing_inspect.get_args(Pet)
     pet_optional_origin = typing_inspect.get_origin(Pet)
     is_dict = issubclass_safe(Pet, dict)
     print(f'{pet_optional_args=}')  # pet_optional_args=()
```

### Comparing `lessweb-1.1.0/lessweb.egg-info/PKG-INFO` & `lessweb-1.2.0/lessweb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lessweb
-Version: 1.1.0
+Version: 1.2.0
 Summary: A pythonic web framework
 Author-email: qorzj <goodhorsezxj@gmail.com>
 License: Apache 2
 Keywords: lessweb,web,web.py,aiohttp
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `lessweb-1.1.0/lessweb.egg-info/SOURCES.txt` & `lessweb-1.2.0/lessweb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.1.0/pyproject.toml` & `lessweb-1.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lessweb"
-version = "1.1.0"
+version = "1.2.0"
 description = 'A pythonic web framework'
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ['lessweb', 'web', 'web.py', 'aiohttp']
 authors = [
     {name = "qorzj", email = "goodhorsezxj@gmail.com"},
 ]
```

### Comparing `lessweb-1.1.0/tests/test_typecast.py` & `lessweb-1.2.0/tests/test_typecast.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 import unittest
 from datetime import date, datetime, time
 from enum import Enum
-from typing import Dict, Generator, List, Literal, Optional, TypedDict, Union
+from typing import (Dict, Generator, List, Literal, NewType, Optional,
+                    TypedDict, Union)
 
 from lessweb.typecast import TypeCastError, inspect_type, typecast
 
 NoneType = type(None)
 
 
 class SampleTypedDict(TypedDict):
@@ -14,28 +15,32 @@
     age: int
 
 
 class SampleElse:
     pass
 
 
+UserId = NewType('UserId', int)
+
+
 class TestInspectType(unittest.TestCase):
     def test_inspect_type(self):
         self.assertEqual(inspect_type(int), (int,))
         self.assertEqual(inspect_type(list), (list,))
         self.assertEqual(inspect_type(list[int]), (list, int))
         self.assertEqual(inspect_type(Optional[int]), (Union, (int, NoneType)))
         if sys.version_info[:2] >= (3, 11):
             self.assertEqual(inspect_type(int | None),
                              (Union, (int, NoneType)))
             self.assertEqual(inspect_type(int | str), (Union, (int, str)))
             self.assertEqual(inspect_type(int | str | None),
                              (Union, (int, str, NoneType)))
         self.assertEqual(inspect_type(
             Literal['a', 'b']), (Literal, ('a', 'b')))
+        self.assertEqual(inspect_type(UserId), (NewType, int))
         self.assertEqual(inspect_type(dict), (dict,))
         self.assertRaises(NotImplementedError, inspect_type, dict[str, int])
         self.assertRaises(NotImplementedError, inspect_type,
                           Dict[str, Union[str, int]])
         self.assertEqual(inspect_type(SampleTypedDict),
                          (dict, {'age': int, 'name': str}))
         self.assertEqual(inspect_type(SampleElse), (SampleElse,))
@@ -116,10 +121,31 @@
         tp = Literal
         try:
             typecast(data, tp)
             self.fail('should raise TypeCastError')
         except TypeCastError as e:
             self.assertEqual(str(e), f'{tp=} is empty')
 
+    def test_typecast_union(self):
+        data = "10"
+        tp = Union[int, list[int]]
+        result = typecast(data, tp)
+        self.assertEqual(result, 10)
+        data = "11,12"
+        result = typecast(data, tp)
+        self.assertEqual(result, [11, 12])
+        data = "12.3"
+        with self.assertRaises(TypeCastError):
+            typecast(data, tp)
+
+    def test_typecast_newtype(self):
+        data = "10"
+        tp = UserId
+        result = typecast(data, tp)
+        self.assertEqual(result, UserId(10))
+        data = "12.3"
+        with self.assertRaises(TypeCastError):
+            typecast(data, tp)
+
 
 if __name__ == '__main__':
     unittest.main()
```

