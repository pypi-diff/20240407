# Comparing `tmp/systembridgebackend-4.1.6.tar.gz` & `tmp/systembridgebackend-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-4.1.6.tar", last modified: Sun Mar 31 14:39:24 2024, max compression
+gzip compressed data, was "systembridgebackend-4.2.0.tar", last modified: Sun Apr  7 12:51:00 2024, max compression
```

## Comparing `systembridgebackend-4.1.6.tar` & `systembridgebackend-4.2.0.tar`

### file list

```diff
@@ -1,57 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.747674 systembridgebackend-4.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-31 14:39:24.743674 systembridgebackend-4.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:39:24.747674 systembridgebackend-4.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.739673 systembridgebackend-4.1.6/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-31 14:39:22.000000 systembridgebackend-4.1.6/systembridgebackend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.739673 systembridgebackend-4.1.6/systembridgebackend/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.739673 systembridgebackend-4.1.6/systembridgebackend/handlers/autostart/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/autostart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/autostart/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/autostart/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.739673 systembridgebackend-4.1.6/systembridgebackend/handlers/media/
--rw-r--r--   0 runner    (1001) docker     (127)    16402 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/media/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.743674 systembridgebackend-4.1.6/systembridgebackend/handlers/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/threads/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/threads/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/threads/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/handlers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.743674 systembridgebackend-4.1.6/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13432 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)     5948 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    11140 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/modules/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.743674 systembridgebackend-4.1.6/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6832 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)    37266 2024-03-31 14:38:53.000000 systembridgebackend-4.1.6/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:39:24.743674 systembridgebackend-4.1.6/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-03-31 14:39:24.000000 systembridgebackend-4.1.6/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-03-31 14:39:24.000000 systembridgebackend-4.1.6/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:39:24.000000 systembridgebackend-4.1.6/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-31 14:39:24.000000 systembridgebackend-4.1.6/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-31 14:39:24.000000 systembridgebackend-4.1.6/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.585054 systembridgebackend-4.2.0/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 12:50:58.000000 systembridgebackend-4.2.0/systembridgebackend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.585054 systembridgebackend-4.2.0/systembridgebackend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/handlers/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/media/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/threads/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/handlers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13239 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/modules/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.589054 systembridgebackend-4.2.0/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 12:51:00.000000 systembridgebackend-4.2.0/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:51:00.593054 systembridgebackend-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 12:48:13.000000 systembridgebackend-4.2.0/tests/test__version.py
```

### Comparing `systembridgebackend-4.1.6/LICENSE` & `systembridgebackend-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.1.6/PKG-INFO` & `systembridgebackend-4.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.1.6
+Version: 4.2.0
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
-Requires-Dist: fastapi==0.110.0
+Requires-Dist: fastapi==0.110.1
 Requires-Dist: incremental==22.10.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
+Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: screeninfo==0.8.1
 Requires-Dist: systembridgeconnector>=4.0.5
 Requires-Dist: systembridgemodels>=4.0.4
 Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.0
+Requires-Dist: typer==0.12.1
 Requires-Dist: uvicorn[standard]==0.29.0
-Requires-Dist: zeroconf==0.131.0
+Requires-Dist: zeroconf==0.132.0
 
 # System Bridge - Backend
 
 This is the backend package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgebackend-4.1.6/pyproject.toml` & `systembridgebackend-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.1.6/setup.py` & `systembridgebackend-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.1.6/systembridgebackend/__init__.py` & `systembridgebackend-4.2.0/systembridgebackend/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """System Bridge."""
-from __future__ import annotations
 
 import asyncio
 import sys
 
 from systembridgeshared.base import Base
 from systembridgeshared.logger import setup_logger
 from systembridgeshared.settings import Settings
@@ -19,21 +18,21 @@
     def __init__(
         self,
         settings: Settings,
         init: bool = False,
         no_frontend: bool = False,
     ) -> None:
         """Initialise."""
-        setup_logger(settings.data.log_level, "system-bridge-backend")
+        setup_logger(settings.data.log_level, "systembridgebackend")
         super().__init__()
         if init:
             self._logger.info("Initialised application. Exiting now.")
             sys.exit(0)
 
-        self._logger.info("System Bridge %s: Startup", __version__.public())
+        self._logger.info("System Bridge Backend (%s)", __version__.public())
 
         self._logger.info("Your token is: %s", settings.data.api.token)
 
         listeners = Listeners()
 
         loop = asyncio.new_event_loop()
         asyncio.set_event_loop(loop)
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/__main__.py` & `systembridgebackend-4.2.0/systembridgebackend/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Main."""
+
 import logging
 
 import typer
 
 from systembridgebackend import Application
 from systembridgeshared.logger import setup_logger
 from systembridgeshared.settings import Settings
@@ -14,15 +15,15 @@
 def main(
     init: bool = typer.Option(False, "--init", help="Initialise"),
     no_frontend: bool = typer.Option(False, "--no-frontend", help="No Frontend"),
 ) -> None:
     """Run the main application."""
     settings = Settings()
 
-    logger = setup_logger(settings.data.log_level, "system-bridge-backend")
+    logger = setup_logger(settings.data.log_level, "systembridgebackend")
     logging.getLogger("zeroconf").setLevel(logging.ERROR)
 
     try:
         Application(
             settings,
             init=init,
             no_frontend=no_frontend,
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/action.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/action.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Action Utilities."""
+
 from typing import Any
 
-from systembridgeconnector.http_client import HTTPClient
-from systembridgemodels.action import Action
-from systembridgeshared.base import Base
-from systembridgeshared.exceptions import (
+from systembridgeconnector.exceptions import (
     AuthenticationException,
     ConnectionErrorException,
 )
+from systembridgeconnector.http_client import HTTPClient
+from systembridgemodels.action import Action
+from systembridgeshared.base import Base
 from systembridgeshared.settings import Settings
 
 
 class ActionHandler(Base):
     """Handle actions."""
 
     def __init__(
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/data.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Data."""
+
 from collections.abc import Awaitable, Callable
 from typing import Any
 
 from systembridgemodels.modules import ModulesData
 from systembridgeshared.base import Base
 
 from .threads.data import DataUpdateThread
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/keyboard.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/keyboard.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Keyboard handlers."""
+
 from collections.abc import Callable
 
 from keyboard import (
     add_hotkey,
     press_and_release,
     remove_hotkey,
     unhook_all_hotkeys,
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/media/__init__.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/media/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Media handlers."""
-from __future__ import annotations
 
 import asyncio
 from collections.abc import Callable
 from dataclasses import asdict
 from datetime import datetime
 import mimetypes
 import os
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/media/windows.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/media/windows.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Windows Media handler."""
+
 from winsdk.windows.media import (  # pylint: disable=import-error
     MediaPlaybackAutoRepeatMode,
     control as wmc,  # pylint: disable=import-error
 )
 
 
 class WindowsMediaException(Exception):
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/power.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/power.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Power handlers."""
+
 import asyncio
 from collections.abc import Callable
 import os
 import sys
 
 
 async def schedule_power_event(
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/threads/__init__.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Thread handlers."""
+
 import asyncio
 from threading import Thread
 
 from systembridgeshared.base import Base
 
 
 class BaseThread(Thread, Base):
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/threads/data.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Data update thread handler."""
+
 from collections.abc import Awaitable, Callable
 from typing import Any, Final, override
 
 from ...modules import ModulesUpdate
 from .update import UpdateThread
 
 UPDATE_INTERVAL: Final[int] = 30
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/threads/media.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/media.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Media update thread handler."""
+
 from collections.abc import Awaitable, Callable
 import platform
 from typing import Final, override
 
 from systembridgemodels.modules.media import Media as MediaInfo
 
 from .update import UpdateThread
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/handlers/threads/update.py` & `systembridgebackend-4.2.0/systembridgebackend/handlers/threads/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Update thread handler."""
+
 import asyncio
 from datetime import datetime, timedelta
 import threading
 import time
 from typing import override
 
 from . import BaseThread
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/__init__.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/battery.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/battery.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Battery."""
-from __future__ import annotations
 
 from typing import override
 
 from plyer import battery
 import psutil
 
 from systembridgemodels.modules.battery import Battery
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/cpu.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """CPU."""
-from __future__ import annotations
 
 import asyncio
 from typing import override
 
 from psutil import (
     cpu_count,
     cpu_freq,
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/disks.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/disks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Disks."""
 
-from __future__ import annotations
-
 import asyncio
 from typing import override
 
 from psutil import disk_io_counters, disk_partitions, disk_usage
 from psutil._common import sdiskio, sdiskpart, sdiskusage
 
 from systembridgemodels.modules.disks import (
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/displays.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/displays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Displays."""
-from __future__ import annotations
 
 from typing import override
 
 from screeninfo import ScreenInfoError, get_monitors
 
 from systembridgemodels.modules.displays import Display
 from systembridgemodels.modules.sensors import Sensors
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/gpus.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/gpus.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """GPUs."""
-from __future__ import annotations
 
 from typing import override
 
 from systembridgemodels.modules.gpus import GPU
 from systembridgemodels.modules.sensors import Sensors
 
 from .base import ModuleUpdateBase
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/listeners.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/media.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/media.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Media."""
-# pylint: disable=import-error
-from __future__ import annotations
 
+# pylint: disable=import-error
 import asyncio
 from collections.abc import Awaitable, Callable
 import datetime
 import platform
 from typing import Final
 
 from winsdk.windows.foundation import EventRegistrationToken
@@ -13,14 +12,15 @@
 
 from systembridgemodels.modules.media import Media as MediaInfo
 from systembridgeshared.base import Base
 
 IDLE_UPDATE_INTERVAL: Final[int] = 20
 PLAYING_UPDATE_INTERVAL: Final[int] = 5
 
+
 class Media(Base):
     """Media."""
 
     def __init__(
         self,
         changed_callback: Callable[[str, MediaInfo], Awaitable[None]],
         update_media_info_interval: Callable[[int], None],
@@ -149,15 +149,16 @@
                     media_info.is_stop_enabled = info.controls.is_stop_enabled
 
             if timeline := self.current_session.get_timeline_properties():
                 media_info.duration = timeline.end_time.total_seconds()
                 media_info.position = timeline.position.total_seconds()
 
             if (
-                properties := await self.current_session.try_get_media_properties_async()
+                properties
+                := await self.current_session.try_get_media_properties_async()
             ):
                 media_info.title = properties.title
                 media_info.subtitle = properties.subtitle
                 media_info.artist = properties.artist
                 media_info.album_artist = properties.album_artist
                 media_info.album_title = properties.album_title
                 media_info.track_number = properties.track_number
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/memory.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/memory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Memory."""
+
 import asyncio
 from typing import NamedTuple, override
 
 from psutil import swap_memory, virtual_memory
 from psutil._common import sswap
 
 from systembridgemodels.modules.memory import Memory, MemorySwap, MemoryVirtual
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/networks.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Network."""
+
 import asyncio
 from typing import override
 
 from psutil import net_connections, net_if_addrs, net_if_stats, net_io_counters
 from psutil._common import sconn, snetio, snicaddr, snicstats
 
 from systembridgemodels.modules.networks import (
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/processes.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/processes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Processes."""
-from __future__ import annotations
 
 from typing import override
 
 from psutil import AccessDenied, NoSuchProcess, process_iter
 
 from systembridgemodels.modules.processes import Process
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/sensors.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/sensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Sensors."""
-from __future__ import annotations
 
 import asyncio
 import json
 import subprocess
 import sys
 from typing import Any
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/modules/system.py` & `systembridgebackend-4.2.0/systembridgebackend/modules/system.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,76 @@
 """System."""
 
-from __future__ import annotations
-
 import asyncio
+import getpass
 import os
 import platform
 import re
 import socket
 import sys
 from typing import Any, override
 import uuid
 
 import aiohttp
-from pkg_resources import parse_version
+from packaging.version import parse
 from plyer import uniqueid
 from psutil import boot_time, users
 from psutil._common import suser
 
-from systembridgemodels.modules.system import System, SystemUser
+from systembridgemodels.modules.system import RunMode, System, SystemUser
+from systembridgeshared.common import get_user_data_directory
 
 from .._version import __version__
 from .base import ModuleUpdateBase
 
 
 class SystemUpdate(ModuleUpdateBase):
     """System Update."""
 
     def __init__(self) -> None:
         """Initialise."""
         super().__init__()
         self._mac_address: str = self._get_mac_address()
-        self._version: str = __version__.public()
+
+        # Determine the run mode based on the running executable
+        self._run_mode: RunMode = (
+            RunMode.PYTHON if "python" in sys.executable.lower() else RunMode.STANDALONE
+        )
+        self._logger.info("Run mode: %s", self._run_mode)
+
+        # Get the version
+        self._version: str | None = None
+        if self._run_mode == "python":
+            self._version = __version__.public()
+        if self._run_mode == "standalone":
+            # Read the version file from the package
+            with open(
+                os.path.join(
+                    get_user_data_directory(),
+                    "systembridge-version.txt",
+                ),
+                encoding="utf-8",
+            ) as version_file:
+                self._version = version_file.read().strip()
+        self._logger.info("Version: %s", self._version)
+
+        # Determine the latest version URL based on the run mode
+        self._version_latest_url = f"https://api.github.com/repos/timmo001/{(
+            'system-bridge' if self._run_mode == RunMode.STANDALONE else 'system-bridge-backend'
+        )}/releases/latest"
+
         self._version_latest: str | None = None
 
     async def _get_active_user_id(self) -> int:
         """Get active user ID."""
         return os.getpid()
 
-    async def _get_active_user_name(self) -> str:
+    async def _get_active_user_name(self) -> str | None:
         """Get active user."""
-        return os.getlogin()
+        return getpass.getuser()
 
     async def _get_boot_time(self) -> float:
         """Get boot time."""
         return boot_time()
 
     async def _get_camera_usage(self) -> list[str]:
         """Return a list of apps that are currently using the webcam."""
@@ -224,32 +251,52 @@
                 return self._mac_address
 
         try:
             return uniqueid.id or self._mac_address
         except Exception:  # pylint: disable=broad-except
             return self._mac_address
 
+    async def _check_rate_limit(self) -> int:
+        """Check the GitHub API rate limit."""
+        async with aiohttp.ClientSession() as session, session.get(
+            "https://api.github.com/rate_limit"
+        ) as response:
+            if response.status == 200:
+                data = await response.json()
+                rate_limit = data.get("rate", {})
+                return rate_limit.get("remaining", 0)
+        return 0
+
     async def _get_version_latest(self) -> Any | None:
         """Get latest version from GitHub."""
         self._logger.info("Get latest version from GitHub")
 
+        # Check if the rate limit allows the request
+        rate_limit = await self._check_rate_limit()
+        self._logger.debug("Rate limit: %s", rate_limit)
+        if rate_limit < 1:
+            self._logger.warning("Rate limit exceeded. Skipping request.")
+            return self._version_latest
+
+        # Use the GitHub API to get the latest release
+        self._logger.debug("URL: %s", self._version_latest_url)
         async with aiohttp.ClientSession() as session, session.get(
-            "https://api.github.com/repos/timmo001/system-bridge/releases/latest"
+            self._version_latest_url
         ) as response:
             if response.status == 200:
                 data = await response.json()
                 if data is not None and (tag_name := data.get("tag_name")) is not None:
-                    return tag_name.replace("v", "")
+                    self._version_latest = tag_name.replace("v", "")
 
-        return None
+        return self._version_latest
 
     async def _get_version_newer_available(self) -> bool | None:
         """Check if newer version is available."""
-        if self._version_latest is not None:
-            return parse_version(self._version_latest) > parse_version(self._version)
+        if self._version_latest is not None and self._version is not None:
+            return parse(self._version_latest) > parse(self._version)
         return None
 
     @override
     async def update_all_data(self) -> System:
         """Update all data."""
         self._logger.debug("Update all data")
 
@@ -290,26 +337,28 @@
             fqdn=fqdn,
             hostname=hostname,
             ip_address_4=ip_address_4,
             mac_address=self._mac_address,
             platform_version=platform_version,
             platform=platform_result,
             uptime=uptime,
+            run_mode=self._run_mode,
             users=[
                 SystemUser(
                     name=user.name,
                     active=user.name == active_user_name,
                     terminal=user.terminal,
                     host=user.host,
                     started=user.started,
                     pid=user.pid,
                 )
                 for user in users_result
             ],
             uuid=self._uuid,
-            version=self._version,
+            version=self._version or "",
             camera_usage=camera_usage,
             ip_address_6=ip_address_6,
             pending_reboot=pending_reboot,
+            version_latest_url=self._version_latest_url,
             version_latest=version_latest,
             version_newer_available=await self._get_version_newer_available(),
         )
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/server/__init__.py` & `systembridgebackend-4.2.0/systembridgebackend/server/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 from systembridgemodels.action import Action
 from systembridgemodels.settings import SettingHotkey
 from systembridgeshared.base import Base
 from systembridgeshared.settings import Settings
 
 from ..handlers.action import ActionHandler
-from ..handlers.autostart import autostart_disable, autostart_enable
 from ..handlers.data import DataUpdate
 from ..handlers.keyboard import keyboard_hotkey_register
 from ..modules.listeners import Listeners
 from ..server.mdns import MDNSAdvertisement
 from .api import app as api_app
 
 
@@ -63,20 +62,14 @@
 
         self._logger.info("Setup API app")
         api_app.callback_exit = self.exit_application
         api_app.data_update = DataUpdate(self.data_updated)
         api_app.listeners = listeners
         api_app.loop = asyncio.get_event_loop()
 
-        self._logger.info("Autostart enabled: %s", self._settings.data.autostart)
-        if self._settings.data.autostart:
-            autostart_enable()
-        else:
-            autostart_disable()
-
         self._logger.info("Setup API server")
         self._api_server = APIServer(
             config=uvicorn.Config(
                 api_app,
                 host="0.0.0.0",
                 loop="asyncio",
                 log_config=None,
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/server/api.py` & `systembridgebackend-4.2.0/systembridgebackend/server/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         self.callback_open_gui: Callable[[str, str], None]
         self.data_update: DataUpdate
         self.listeners: Listeners
         self.loop: asyncio.AbstractEventLoop = asyncio_get_loop()
 
 
 app = API(
-    title="System Bridge",
+    title="System Bridge Backend",
     version=__version__.public(),
 )
 
 
 @app.get("/")
 def get_root() -> dict[str, str]:
     """Get root."""
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend/server/mdns.py` & `systembridgebackend-4.2.0/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.1.6/systembridgebackend/server/websocket.py` & `systembridgebackend-4.2.0/systembridgebackend/server/websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,15 +88,14 @@
     TYPE_SETTINGS_RESULT,
     TYPE_UNREGISTER_DATA_LISTENER,
     TYPE_UPDATE_SETTINGS,
 )
 from systembridgeshared.settings import Settings
 from systembridgeshared.update import Update
 
-from ..handlers.autostart import autostart_disable, autostart_enable
 from ..handlers.data import DataUpdate
 from ..handlers.keyboard import keyboard_keypress, keyboard_text
 from ..handlers.media import (
     control_fastforward,
     control_mute,
     control_next,
     control_pause,
@@ -858,22 +857,14 @@
                 Response(
                     id=request.id,
                     type=TYPE_SETTINGS_RESULT,
                     message="Updated settings",
                     data=asdict(self._settings.data),
                 )
             )
-
-            # Update autostart
-            self._logger.info("Setting autostart to %s", self._settings.data.autostart)
-            if self._settings.data.autostart:
-                autostart_enable()
-            else:
-                autostart_disable()
-
         elif request.event == TYPE_POWER_SLEEP:
             self._logger.info("Sleeping")
             await self._send_response(
                 Response(
                     id=request.id,
                     type=TYPE_POWER_SLEEPING,
                     message="Sleeping",
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend.egg-info/PKG-INFO` & `systembridgebackend-4.2.0/systembridgebackend.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.1.6
+Version: 4.2.0
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
-Requires-Dist: fastapi==0.110.0
+Requires-Dist: fastapi==0.110.1
 Requires-Dist: incremental==22.10.0
 Requires-Dist: keyboard==0.13.5
 Requires-Dist: mutagen==1.47.0
+Requires-Dist: packaging>=24.0
 Requires-Dist: plyer==2.1.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: python-multipart==0.0.9
 Requires-Dist: screeninfo==0.8.1
 Requires-Dist: systembridgeconnector>=4.0.5
 Requires-Dist: systembridgemodels>=4.0.4
 Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.0
+Requires-Dist: typer==0.12.1
 Requires-Dist: uvicorn[standard]==0.29.0
-Requires-Dist: zeroconf==0.131.0
+Requires-Dist: zeroconf==0.132.0
 
 # System Bridge - Backend
 
 This is the backend package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgebackend-4.1.6/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-4.2.0/systembridgebackend.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -13,17 +13,14 @@
 systembridgebackend/handlers/__init__.py
 systembridgebackend/handlers/action.py
 systembridgebackend/handlers/data.py
 systembridgebackend/handlers/keyboard.py
 systembridgebackend/handlers/open.py
 systembridgebackend/handlers/power.py
 systembridgebackend/handlers/update.py
-systembridgebackend/handlers/autostart/__init__.py
-systembridgebackend/handlers/autostart/linux.py
-systembridgebackend/handlers/autostart/windows.py
 systembridgebackend/handlers/media/__init__.py
 systembridgebackend/handlers/media/windows.py
 systembridgebackend/handlers/threads/__init__.py
 systembridgebackend/handlers/threads/data.py
 systembridgebackend/handlers/threads/media.py
 systembridgebackend/handlers/threads/update.py
 systembridgebackend/modules/__init__.py
@@ -39,8 +36,9 @@
 systembridgebackend/modules/networks.py
 systembridgebackend/modules/processes.py
 systembridgebackend/modules/sensors.py
 systembridgebackend/modules/system.py
 systembridgebackend/server/__init__.py
 systembridgebackend/server/api.py
 systembridgebackend/server/mdns.py
-systembridgebackend/server/websocket.py
+systembridgebackend/server/websocket.py
+tests/test__version.py
```

