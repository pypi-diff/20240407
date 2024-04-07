# Comparing `tmp/Kodistubs-21.0.0.tar.gz` & `tmp/Kodistubs-21.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Kodistubs-21.0.0.tar", last modified: Sun Apr  7 13:44:03 2024, max compression
+gzip compressed data, was "Kodistubs-21.0.0rc1.tar", last modified: Sun Mar 10 14:38:58 2024, max compression
```

## Comparing `Kodistubs-21.0.0.tar` & `Kodistubs-21.0.0rc1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:44:03.794458 Kodistubs-21.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:44:03.794458 Kodistubs-21.0.0/Kodistubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-07 13:44:03.000000 Kodistubs-21.0.0/Kodistubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-07 13:44:03.000000 Kodistubs-21.0.0/Kodistubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:44:03.000000 Kodistubs-21.0.0/Kodistubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:44:03.000000 Kodistubs-21.0.0/Kodistubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-07 13:44:03.000000 Kodistubs-21.0.0/Kodistubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-07 13:44:03.794458 Kodistubs-21.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-07 13:44:03.798458 Kodistubs-21.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    99206 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/xbmc.py
--rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/xbmcaddon.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/xbmcdrm.py
--rw-r--r--   0 runner    (1001) docker     (127)   165121 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/xbmcgui.py
--rw-r--r--   0 runner    (1001) docker     (127)    17257 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/xbmcplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-07 13:44:01.000000 Kodistubs-21.0.0/xbmcvfs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:38:58.135844 Kodistubs-21.0.0rc1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:38:58.135844 Kodistubs-21.0.0rc1/Kodistubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-10 14:38:58.000000 Kodistubs-21.0.0rc1/Kodistubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-10 14:38:58.000000 Kodistubs-21.0.0rc1/Kodistubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 14:38:58.000000 Kodistubs-21.0.0rc1/Kodistubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 14:38:58.000000 Kodistubs-21.0.0rc1/Kodistubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-10 14:38:58.000000 Kodistubs-21.0.0rc1/Kodistubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    32472 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-03-10 14:38:58.135844 Kodistubs-21.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-10 14:38:58.135844 Kodistubs-21.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99206 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/xbmc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17043 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/xbmcaddon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/xbmcdrm.py
+-rw-r--r--   0 runner    (1001) docker     (127)   165121 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/xbmcgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17257 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/xbmcplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-03-10 14:38:51.000000 Kodistubs-21.0.0rc1/xbmcvfs.py
```

### Comparing `Kodistubs-21.0.0/Kodistubs.egg-info/PKG-INFO` & `Kodistubs-21.0.0rc1/Kodistubs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kodistubs
-Version: 21.0.0
+Version: 21.0.0rc1
 Summary: Stub modules that re-create Kodi Python API
 Home-page: https://github.com/romanvm/Kodistubs
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
 License: GPL-3.0-only
 Keywords: kodi documentation inspection
 Platform: any
```

### Comparing `Kodistubs-21.0.0/LICENSE.txt` & `Kodistubs-21.0.0rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Kodistubs-21.0.0/PKG-INFO` & `Kodistubs-21.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Kodistubs
-Version: 21.0.0
+Version: 21.0.0rc1
 Summary: Stub modules that re-create Kodi Python API
 Home-page: https://github.com/romanvm/Kodistubs
 Author: Roman Miroshnychenko
 Author-email: roman1972@gmail.com
 License: GPL-3.0-only
 Keywords: kodi documentation inspection
 Platform: any
```

### Comparing `Kodistubs-21.0.0/README.rst` & `Kodistubs-21.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `Kodistubs-21.0.0/setup.cfg` & `Kodistubs-21.0.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Kodistubs
-version = 21.0.0
+version = 21.0.0rc1
 author = Roman Miroshnychenko
 author_email = roman1972@gmail.com
 url = https://github.com/romanvm/Kodistubs
 description = Stub modules that re-create Kodi Python API
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 keywords = kodi documentation inspection
```

### Comparing `Kodistubs-21.0.0/xbmc.py` & `Kodistubs-21.0.0rc1/xbmc.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-21.0.0/xbmcaddon.py` & `Kodistubs-21.0.0rc1/xbmcaddon.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-21.0.0/xbmcdrm.py` & `Kodistubs-21.0.0rc1/xbmcdrm.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-21.0.0/xbmcgui.py` & `Kodistubs-21.0.0rc1/xbmcgui.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-21.0.0/xbmcplugin.py` & `Kodistubs-21.0.0rc1/xbmcplugin.py`

 * *Files identical despite different names*

### Comparing `Kodistubs-21.0.0/xbmcvfs.py` & `Kodistubs-21.0.0rc1/xbmcvfs.py`

 * *Files identical despite different names*

