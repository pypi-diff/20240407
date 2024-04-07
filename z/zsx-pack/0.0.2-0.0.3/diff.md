# Comparing `tmp/zsx_pack-0.0.2.tar.gz` & `tmp/zsx_pack-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsx_pack-0.0.2.tar", last modified: Wed Apr  3 10:02:17 2024, max compression
+gzip compressed data, was "zsx_pack-0.0.3.tar", last modified: Sun Apr  7 02:55:32 2024, max compression
```

## Comparing `zsx_pack-0.0.2.tar` & `zsx_pack-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:16.999696 zsx_pack-0.0.2/
--rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0      883 2024-04-03 10:02:16.997698 zsx_pack-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-03 09:41:27.000000 zsx_pack-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:16.971695 zsx_pack-0.0.2/logger/
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:16.994699 zsx_pack-0.0.2/logger/zsx_pack.egg-info/
--rw-rw-rw-   0        0        0      883 2024-04-03 10:02:16.000000 zsx_pack-0.0.2/logger/zsx_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-04-03 10:02:16.000000 zsx_pack-0.0.2/logger/zsx_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:02:16.000000 zsx_pack-0.0.2/logger/zsx_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:02:16.000000 zsx_pack-0.0.2/logger/zsx_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 10:02:17.000737 zsx_pack-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2024-04-03 10:01:49.000000 zsx_pack-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:55:32.844422 zsx_pack-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1587 2024-04-07 02:55:32.841422 zsx_pack-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2024-04-07 01:39:14.000000 zsx_pack-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 02:55:32.814421 zsx_pack-0.0.3/logger/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:55:32.837422 zsx_pack-0.0.3/logger/zsx_pack.egg-info/
+-rw-rw-rw-   0        0        0     1587 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:55:32.000000 zsx_pack-0.0.3/logger/zsx_pack.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 02:55:32.844422 zsx_pack-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2024-04-07 02:55:29.000000 zsx_pack-0.0.3/setup.py
```

### Comparing `zsx_pack-0.0.2/LICENSE.txt` & `zsx_pack-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zsx_pack-0.0.2/setup.py` & `zsx_pack-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zsx_pack",
-    version="0.0.2",
+    version="0.0.3",
     author="zsx",
     author_email="17630583910@163.com",
-    description="自用包，主要是为了不行使用logger无法屏蔽第三方包日志",
+    description="自用包，主要是为了logger无法屏蔽第三方包日志而开发的",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ziyueguyi/zsx_pack",
     project_urls={
         "Bug Tracker": "https://github.com/ziyueguyi/zsx_pack",
     },
     classifiers=[
```

