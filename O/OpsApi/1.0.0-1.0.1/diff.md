# Comparing `tmp/OpsApi-1.0.0.tar.gz` & `tmp/OpsApi-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/OpsApi-1.0.0.tar", last modified: Sun Apr  7 10:02:18 2024, max compression
+gzip compressed data, was "dist/OpsApi-1.0.1.tar", last modified: Sun Apr  7 10:13:16 2024, max compression
```

## Comparing `OpsApi-1.0.0.tar` & `OpsApi-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 10:02:18.000000 OpsApi-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      221 2024-04-07 10:02:18.000000 OpsApi-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 10:02:18.000000 OpsApi-1.0.0/OpsApi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      221 2024-04-07 10:02:18.000000 OpsApi-1.0.0/OpsApi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      215 2024-04-07 10:02:18.000000 OpsApi-1.0.0/OpsApi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-07 10:02:18.000000 OpsApi-1.0.0/OpsApi.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-04-07 10:02:18.000000 OpsApi-1.0.0/OpsApi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 10:02:18.000000 OpsApi-1.0.0/OpsApi.egg-info/dependency_links.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 10:02:18.000000 OpsApi-1.0.0/OpsApi/
--rw-r--r--   0 root         (0) root         (0)       86 2024-04-07 08:01:46.000000 OpsApi-1.0.0/OpsApi/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)   169080 2024-04-07 08:50:25.000000 OpsApi-1.0.0/OpsApi/models.so
--rw-r--r--   0 root         (0) root         (0)      118 2024-04-07 09:55:27.000000 OpsApi-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 08:07:38.000000 OpsApi-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      674 2024-04-07 10:00:49.000000 OpsApi-1.0.0/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 10:02:18.000000 OpsApi-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 10:13:16.000000 OpsApi-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-07 10:13:16.000000 OpsApi-1.0.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 10:13:16.000000 OpsApi-1.0.1/OpsApi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-07 10:13:16.000000 OpsApi-1.0.1/OpsApi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-07 10:13:16.000000 OpsApi-1.0.1/OpsApi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-04-07 10:13:16.000000 OpsApi-1.0.1/OpsApi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-07 10:13:16.000000 OpsApi-1.0.1/OpsApi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 10:13:16.000000 OpsApi-1.0.1/OpsApi.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 10:13:16.000000 OpsApi-1.0.1/OpsApi/
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-07 08:01:46.000000 OpsApi-1.0.1/OpsApi/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)   169080 2024-04-07 10:12:08.000000 OpsApi-1.0.1/OpsApi/models.so
+-rw-r--r--   0 root         (0) root         (0)      118 2024-04-07 09:55:27.000000 OpsApi-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 08:07:38.000000 OpsApi-1.0.1/README.md
+-rw-r--r--   0 root         (0) root         (0)      674 2024-04-07 10:13:13.000000 OpsApi-1.0.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 10:13:16.000000 OpsApi-1.0.1/setup.cfg
```

### Comparing `OpsApi-1.0.0/OpsApi/models.so` & `OpsApi-1.0.1/OpsApi/models.so`

 * *Files identical despite different names*

### Comparing `OpsApi-1.0.0/setup.py` & `OpsApi-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # 定义要包含的共享库文件
 package_data = {
     "": ["*.so"],  # 包含当前目录下的所有 .so 文件
 }
 
 setup(
     name = 'OpsApi',
-    version = '1.0.0',
+    version = '1.0.1',
     package_data=package_data,
     keywords='tm',
     description = 'a library for tm Developer',
     license = 'License',
     url = 'https://github.com/tm',
     author = 'Tommi',
     author_email = 'xm6798121@gmail.com',
```

