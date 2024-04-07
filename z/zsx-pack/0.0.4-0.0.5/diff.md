# Comparing `tmp/zsx_pack-0.0.4.tar.gz` & `tmp/zsx_pack-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsx_pack-0.0.4.tar", last modified: Sun Apr  7 03:00:33 2024, max compression
+gzip compressed data, was "zsx_pack-0.0.5.tar", last modified: Sun Apr  7 03:08:10 2024, max compression
```

## Comparing `zsx_pack-0.0.4.tar` & `zsx_pack-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 03:00:33.649646 zsx_pack-0.0.4/
--rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1587 2024-04-07 03:00:33.646644 zsx_pack-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      984 2024-04-07 01:39:14.000000 zsx_pack-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 03:00:33.617645 zsx_pack-0.0.4/logger/
-drwxrwxrwx   0        0        0        0 2024-04-07 03:00:33.642646 zsx_pack-0.0.4/logger/zsx_pack.egg-info/
--rw-rw-rw-   0        0        0     1587 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 03:00:33.000000 zsx_pack-0.0.4/logger/zsx_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 03:00:33.649646 zsx_pack-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1075 2024-04-07 03:00:31.000000 zsx_pack-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 03:08:10.459709 zsx_pack-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1587 2024-04-07 03:08:10.453709 zsx_pack-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2024-04-07 01:39:14.000000 zsx_pack-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 03:08:10.416707 zsx_pack-0.0.5/logger/
+-rw-rw-rw-   0        0        0      171 2024-04-03 09:06:53.000000 zsx_pack-0.0.5/logger/__init__.py
+-rw-rw-rw-   0        0        0    17681 2024-04-03 09:04:55.000000 zsx_pack-0.0.5/logger/logger.py
+-rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 03:08:10.459709 zsx_pack-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1079 2024-04-07 03:08:00.000000 zsx_pack-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 03:08:10.439705 zsx_pack-0.0.5/zsx_pack.egg-info/
+-rw-rw-rw-   0        0        0     1587 2024-04-07 03:08:10.000000 zsx_pack-0.0.5/zsx_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-07 03:08:10.000000 zsx_pack-0.0.5/zsx_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 03:08:10.000000 zsx_pack-0.0.5/zsx_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-07 03:08:10.000000 zsx_pack-0.0.5/zsx_pack.egg-info/top_level.txt
```

### Comparing `zsx_pack-0.0.4/LICENSE.txt` & `zsx_pack-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zsx_pack-0.0.4/PKG-INFO` & `zsx_pack-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zsx_pack
-Version: 0.0.4
+Version: 0.0.5
 Summary: 自用包，主要是为了logger无法屏蔽第三方包日志而开发的
 Home-page: https://github.com/ziyueguyi/zsx_pack
 Author: zsx
 Author-email: 17630583910@163.com
 Project-URL: Bug Tracker, https://github.com/ziyueguyi/zsx_pack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zsx_pack-0.0.4/README.md` & `zsx_pack-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zsx_pack-0.0.4/logger/zsx_pack.egg-info/PKG-INFO` & `zsx_pack-0.0.5/zsx_pack.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zsx_pack
-Version: 0.0.4
+Version: 0.0.5
 Summary: 自用包，主要是为了logger无法屏蔽第三方包日志而开发的
 Home-page: https://github.com/ziyueguyi/zsx_pack
 Author: zsx
 Author-email: 17630583910@163.com
 Project-URL: Bug Tracker, https://github.com/ziyueguyi/zsx_pack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `zsx_pack-0.0.4/setup.py` & `zsx_pack-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zsx_pack",
-    version="0.0.4",
+    version="0.0.5",
     author="zsx",
     author_email="17630583910@163.com",
     description="自用包，主要是为了logger无法屏蔽第三方包日志而开发的",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ziyueguyi/zsx_pack",
     project_urls={
@@ -26,11 +26,11 @@
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Natural Language :: Chinese (Simplified)",
     ],
-    package_dir={"": "logger"},
-    packages=setuptools.find_packages(where="src"),
+    # package_dir={"": "logger"},
+    # packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
 )
```

