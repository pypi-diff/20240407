# Comparing `tmp/systembridgebackend-4.2.0.tar.gz` & `tmp/systembridgebackend-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-4.2.0.tar", last modified: Sun Apr  7 12:51:00 2024, max compression
+gzip compressed data, was "systembridgebackend-4.2.1.tar", last modified: Sun Apr  7 13:06:03 2024, max compression
```

## Comparing `systembridgebackend-4.2.0.tar` & `systembridgebackend-4.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.585054 systembridgebackend-4.2.0/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 12:50:58.000000 systembridgebackend-4.2.0/systembridgebackend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.585054 systembridgebackend-4.2.0/systembridgebackend/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/handlers/media/
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/media/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/tests/test__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.442973 systembridgebackend-4.2.1/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 13:06:00.000000 systembridgebackend-4.2.1/systembridgebackend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.446973 systembridgebackend-4.2.1/systembridgebackend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.446973 systembridgebackend-4.2.1/systembridgebackend/handlers/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/media/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.446973 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13483 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/tests/test__version.py
```

### Comparing `systembridgebackend-4.2.0/LICENSE` & `systembridgebackend-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/PKG-INFO` & `systembridgebackend-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.0
+Version: 4.2.1
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgebackend-4.2.0/pyproject.toml` & `systembridgebackend-4.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/setup.py` & `systembridgebackend-4.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/__init__.py` & `systembridgebackend-4.2.1/systembridgebackend/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/__main__.py` & `systembridgebackend-4.2.1/systembridgebackend/__main__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/action.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/data.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/keyboard.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/media/__init__.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/media/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/media/windows.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/media/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/power.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/__init__.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/data.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/media.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/update.py` & `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/__init__.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/battery.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/battery.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/cpu.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/disks.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/displays.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/displays.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/gpus.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/listeners.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/media.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/memory.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/networks.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/processes.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/processes.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/sensors.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/modules/system.py` & `systembridgebackend-4.2.1/systembridgebackend/modules/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,30 +35,30 @@
         self._run_mode: RunMode = (
             RunMode.PYTHON if "python" in sys.executable.lower() else RunMode.STANDALONE
         )
         self._logger.info("Run mode: %s", self._run_mode)
 
         # Get the version
         self._version: str | None = None
-        if self._run_mode == "python":
+        if self._run_mode == RunMode.PYTHON:
             self._version = __version__.public()
-        if self._run_mode == "standalone":
+        if self._run_mode == RunMode.STANDALONE:
             # Read the version file from the package
             with open(
                 os.path.join(
                     get_user_data_directory(),
                     "systembridge-version.txt",
                 ),
                 encoding="utf-8",
             ) as version_file:
                 self._version = version_file.read().strip()
         self._logger.info("Version: %s", self._version)
 
         # Determine the latest version URL based on the run mode
-        self._version_latest_url = f"https://api.github.com/repos/timmo001/{(
+        self._version_latest_url = f"https://github.com/timmo001/{(
             'system-bridge' if self._run_mode == RunMode.STANDALONE else 'system-bridge-backend'
         )}/releases/latest"
 
         self._version_latest: str | None = None
 
     async def _get_active_user_id(self) -> int:
         """Get active user ID."""
@@ -267,29 +267,32 @@
         return 0
 
     async def _get_version_latest(self) -> Any | None:
         """Get latest version from GitHub."""
         self._logger.info("Get latest version from GitHub")
 
         # Check if the rate limit allows the request
-        rate_limit = await self._check_rate_limit()
-        self._logger.debug("Rate limit: %s", rate_limit)
-        if rate_limit < 1:
+        rate_limit_remaining = await self._check_rate_limit()
+        self._logger.debug("Rate limit: %s", rate_limit_remaining)
+        if rate_limit_remaining < 1:
             self._logger.warning("Rate limit exceeded. Skipping request.")
             return self._version_latest
 
+        url = f"https://api.github.com/repos/timmo001/{(
+            'system-bridge' if self._run_mode == RunMode.STANDALONE else 'system-bridge-backend'
+        )}/releases/latest"
+        self._logger.debug("GitHub API URL: %s", url)
+
         # Use the GitHub API to get the latest release
-        self._logger.debug("URL: %s", self._version_latest_url)
-        async with aiohttp.ClientSession() as session, session.get(
-            self._version_latest_url
-        ) as response:
+        async with aiohttp.ClientSession() as session, session.get(url) as response:
             if response.status == 200:
                 data = await response.json()
                 if data is not None and (tag_name := data.get("tag_name")) is not None:
                     self._version_latest = tag_name.replace("v", "")
+                    self._logger.info("Latest version: %s", self._version_latest)
 
         return self._version_latest
 
     async def _get_version_newer_available(self) -> bool | None:
         """Check if newer version is available."""
         if self._version_latest is not None and self._version is not None:
             return parse(self._version_latest) > parse(self._version)
```

### Comparing `systembridgebackend-4.2.0/systembridgebackend/server/__init__.py` & `systembridgebackend-4.2.1/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/server/api.py` & `systembridgebackend-4.2.1/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/server/mdns.py` & `systembridgebackend-4.2.1/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend/server/websocket.py` & `systembridgebackend-4.2.1/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.0/systembridgebackend.egg-info/PKG-INFO` & `systembridgebackend-4.2.1/systembridgebackend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.0
+Version: 4.2.1
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgebackend-4.2.0/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-4.2.1/systembridgebackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

