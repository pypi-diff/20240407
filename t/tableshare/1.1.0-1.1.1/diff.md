# Comparing `tmp/tableshare-1.1.0.tar.gz` & `tmp/tableshare-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tableshare-1.1.0.tar", last modified: Wed Feb 28 06:41:40 2024, max compression
+gzip compressed data, was "tableshare-1.1.1.tar", last modified: Sun Apr  7 12:33:06 2024, max compression
```

## Comparing `tableshare-1.1.0.tar` & `tableshare-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 06:41:40.370260 tableshare-1.1.0/
--rw-rw-rw-   0        0        0     1085 2024-02-25 08:58:56.000000 tableshare-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      931 2024-02-28 06:41:40.370260 tableshare-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2305 2024-02-28 05:51:28.000000 tableshare-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-02-28 06:41:40.370260 tableshare-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1661 2024-02-28 06:41:31.000000 tableshare-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-28 06:41:40.368260 tableshare-1.1.0/tableshare.egg-info/
--rw-rw-rw-   0        0        0      931 2024-02-28 06:41:40.000000 tableshare-1.1.0/tableshare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2024-02-28 06:41:40.000000 tableshare-1.1.0/tableshare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 06:41:40.000000 tableshare-1.1.0/tableshare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-02-28 06:41:40.000000 tableshare-1.1.0/tableshare.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 06:41:40.000000 tableshare-1.1.0/tableshare.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 12:33:06.612865 tableshare-1.1.1/
+-rw-rw-rw-   0        0        0     1085 2024-02-25 08:58:56.000000 tableshare-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0      931 2024-04-07 12:33:06.612865 tableshare-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2305 2024-02-28 05:51:28.000000 tableshare-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 12:33:06.612865 tableshare-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1661 2024-04-07 12:27:33.000000 tableshare-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 12:33:06.610871 tableshare-1.1.1/tableshare.egg-info/
+-rw-rw-rw-   0        0        0      931 2024-04-07 12:33:06.000000 tableshare-1.1.1/tableshare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2024-04-07 12:33:06.000000 tableshare-1.1.1/tableshare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:33:06.000000 tableshare-1.1.1/tableshare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-07 12:33:06.000000 tableshare-1.1.1/tableshare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 12:33:06.000000 tableshare-1.1.1/tableshare.egg-info/top_level.txt
```

### Comparing `tableshare-1.1.0/LICENSE` & `tableshare-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tableshare-1.1.0/PKG-INFO` & `tableshare-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableshare
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for scraping and sharing table data from web pages.
 Home-page: https://github.com/baiguanba/tableshare
 Author: Guanba
 Author-email: baiguanba@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baiguanba/tableshare/issues
 Keywords: python,table,webtable,scrawler
```

### Comparing `tableshare-1.1.0/README.md` & `tableshare-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tableshare-1.1.0/setup.py` & `tableshare-1.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 from setuptools import setup, find_packages
-VERSION = '1.1.0'
+VERSION = '1.1.1'
 DESCRIPTION = 'A Python library for scraping and sharing table data from web pages.'
 
 setup(
     name='tableshare',
     version=VERSION,  # 请在发布新版本时更新这个版本号
     packages=find_packages(),  # 自动查找所有包
     install_requires=['requests', 'pandas', 'bs4', 'DrissionPage'],# 如果有其他依赖，请在这里添加
```

### Comparing `tableshare-1.1.0/tableshare.egg-info/PKG-INFO` & `tableshare-1.1.1/tableshare.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tableshare
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python library for scraping and sharing table data from web pages.
 Home-page: https://github.com/baiguanba/tableshare
 Author: Guanba
 Author-email: baiguanba@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baiguanba/tableshare/issues
 Keywords: python,table,webtable,scrawler
```

