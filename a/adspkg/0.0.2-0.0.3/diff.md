# Comparing `tmp/adspkg-0.0.2.tar.gz` & `tmp/adspkg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\adspkg-0.0.2.tar", last modified: Sun Apr  7 18:20:04 2024, max compression
+gzip compressed data, was "dist\adspkg-0.0.3.tar", last modified: Sun Apr  7 18:53:54 2024, max compression
```

## Comparing `adspkg-0.0.2.tar` & `adspkg-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 18:20:04.925582 adspkg-0.0.2/
--rw-rw-rw-   0        0        0      553 2024-04-07 18:20:04.924582 adspkg-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 18:20:04.916571 adspkg-0.0.2/SMA/
--rw-rw-rw-   0        0        0       40 2024-04-07 18:16:56.000000 adspkg-0.0.2/SMA/__init__.py
--rw-rw-rw-   0        0        0       32 2024-04-07 17:24:30.000000 adspkg-0.0.2/SMA/hello.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:20:04.923582 adspkg-0.0.2/adspkg.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-07 18:20:04.000000 adspkg-0.0.2/adspkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2024-04-07 18:20:04.000000 adspkg-0.0.2/adspkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 18:20:04.000000 adspkg-0.0.2/adspkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-07 18:20:04.000000 adspkg-0.0.2/adspkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 18:20:04.925582 adspkg-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      702 2024-04-07 18:19:15.000000 adspkg-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:53:54.069314 adspkg-0.0.3/
+-rw-rw-rw-   0        0        0      553 2024-04-07 18:53:54.068317 adspkg-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 18:53:54.051255 adspkg-0.0.3/adspkg/
+-rw-rw-rw-   0        0        0     2679 2024-04-07 16:58:29.000000 adspkg-0.0.3/adspkg/A.py
+-rw-rw-rw-   0        0        0     1914 2024-04-07 12:47:41.000000 adspkg-0.0.3/adspkg/B.py
+-rw-rw-rw-   0        0        0     4079 2024-04-07 12:47:30.000000 adspkg-0.0.3/adspkg/C.py
+-rw-rw-rw-   0        0        0     3526 2024-04-07 16:57:36.000000 adspkg-0.0.3/adspkg/D.py
+-rw-rw-rw-   0        0        0     5590 2024-04-07 16:58:01.000000 adspkg-0.0.3/adspkg/E.py
+-rw-rw-rw-   0        0        0       28 2024-04-07 18:52:13.000000 adspkg-0.0.3/adspkg/__init__.py
+-rw-rw-rw-   0        0        0       32 2024-04-07 17:24:30.000000 adspkg-0.0.3/adspkg/hello.py
+-rw-rw-rw-   0        0        0      201 2024-04-07 14:52:25.000000 adspkg-0.0.3/adspkg/main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:53:54.066314 adspkg-0.0.3/adspkg.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-07 18:53:53.000000 adspkg-0.0.3/adspkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-04-07 18:53:53.000000 adspkg-0.0.3/adspkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 18:53:53.000000 adspkg-0.0.3/adspkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-07 18:53:53.000000 adspkg-0.0.3/adspkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 18:53:54.069314 adspkg-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      702 2024-04-07 18:53:17.000000 adspkg-0.0.3/setup.py
```

### Comparing `adspkg-0.0.2/PKG-INFO` & `adspkg-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adspkg
-Version: 0.0.2
+Version: 0.0.3
 Summary: basic hello pkg
 Home-page: UNKNOWN
 Author: Mathew Patil
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
```

### Comparing `adspkg-0.0.2/adspkg.egg-info/PKG-INFO` & `adspkg-0.0.3/adspkg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: adspkg
-Version: 0.0.2
+Version: 0.0.3
 Summary: basic hello pkg
 Home-page: UNKNOWN
 Author: Mathew Patil
 Author-email: UNKNOWN
 License: UNKNOWN
 Description: UNKNOWN
 Keywords: python,video,stream,video stream,camera stream,sockets
```

### Comparing `adspkg-0.0.2/setup.py` & `adspkg-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'basic hello pkg'
 
 # Setting up
 setup(
     name="adspkg",
     version=VERSION,
     author="Mathew Patil",
```

