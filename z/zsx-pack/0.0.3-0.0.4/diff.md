# Comparing `tmp/zsx_pack-0.0.3.tar.gz` & `tmp/zsx_pack-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsx_pack-0.0.3.tar", last modified: Sun Apr  7 02:55:32 2024, max compression
+gzip compressed data, was "zsx_pack-0.0.4.tar", last modified: Sun Apr  7 03:00:33 2024, max compression
```

## Comparing `zsx_pack-0.0.3.tar` & `zsx_pack-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 02:55:32.844422 zsx_pack-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1587 2024-04-07 02:55:32.841422 zsx_pack-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      984 2024-04-07 01:39:14.000000 zsx_pack-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 02:55:32.814421 zsx_pack-0.0.3/logger/
-drwxrwxrwx   0        0        0        0 2024-04-07 02:55:32.837422 zsx_pack-0.0.3/logger/zsx_pack.egg-info/
--rw-rw-rw-   0        0        0     1587 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 02:55:32.844422 zsx_pack-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1075 2024-04-07 02:55:29.000000 zsx_pack-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 03:00:33.649646 zsx_pack-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1587 2024-04-07 03:00:33.646644 zsx_pack-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2024-04-07 01:39:14.000000 zsx_pack-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 03:00:33.617645 zsx_pack-0.0.4/logger/
+drwxrwxrwx   0        0        0        0 2024-04-07 03:00:33.642646 zsx_pack-0.0.4/logger/zsx_pack.egg-info/
+-rw-rw-rw-   0        0        0     1587 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 03:00:33.649646 zsx_pack-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2024-04-07 03:00:31.000000 zsx_pack-0.0.4/setup.py
```

### Comparing `zsx_pack-0.0.3/LICENSE.txt` & `zsx_pack-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zsx_pack-0.0.3/PKG-INFO` & `zsx_pack-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zsx_pack
-Version: 0.0.3
+Version: 0.0.4
 Summary: 自用包，主要是为了logger无法屏蔽第三方包日志而开发的
 Home-page: https://github.com/ziyueguyi/zsx_pack
 Author: zsx
 Author-email: 17630583910@163.com
 Project-URL: Bug Tracker, https://github.com/ziyueguyi/zsx_pack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zsx_pack-0.0.3/README.md` & `zsx_pack-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `zsx_pack-0.0.3/logger/zsx_pack.egg-info/PKG-INFO` & `zsx_pack-0.0.4/logger/zsx_pack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zsx_pack
-Version: 0.0.3
+Version: 0.0.4
 Summary: 自用包，主要是为了logger无法屏蔽第三方包日志而开发的
 Home-page: https://github.com/ziyueguyi/zsx_pack
 Author: zsx
 Author-email: 17630583910@163.com
 Project-URL: Bug Tracker, https://github.com/ziyueguyi/zsx_pack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zsx_pack-0.0.3/setup.py` & `zsx_pack-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zsx_pack",
-    version="0.0.3",
+    version="0.0.4",
     author="zsx",
     author_email="17630583910@163.com",
     description="自用包，主要是为了logger无法屏蔽第三方包日志而开发的",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ziyueguyi/zsx_pack",
     project_urls={
```

