# Comparing `tmp/systembridgebackend-4.2.1.tar.gz` & `tmp/systembridgebackend-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgebackend-4.2.1.tar", last modified: Sun Apr  7 13:06:03 2024, max compression
+gzip compressed data, was "systembridgebackend-4.2.2.tar", last modified: Sun Apr  7 14:05:07 2024, max compression
```

## Comparing `systembridgebackend-4.2.1.tar` & `systembridgebackend-4.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.442973 systembridgebackend-4.2.1/systembridgebackend/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 13:06:00.000000 systembridgebackend-4.2.1/systembridgebackend/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.446973 systembridgebackend-4.2.1/systembridgebackend/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/keyboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.446973 systembridgebackend-4.2.1/systembridgebackend/handlers/media/
--rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/media/windows.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/power.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.446973 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/threads/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/handlers/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/systembridgebackend/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13483 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/modules/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/systembridgebackend/server/
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/mdns.py
--rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/systembridgebackend/server/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/systembridgebackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 13:06:03.000000 systembridgebackend-4.2.1/systembridgebackend.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:06:03.450973 systembridgebackend-4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 13:03:07.000000 systembridgebackend-4.2.1/tests/test__version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.253085 systembridgebackend-4.2.2/systembridgebackend/
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-07 14:05:04.000000 systembridgebackend-4.2.2/systembridgebackend/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.257085 systembridgebackend-4.2.2/systembridgebackend/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/keyboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.257085 systembridgebackend-4.2.2/systembridgebackend/handlers/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/media/windows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/power.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.257085 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/threads/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/handlers/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/systembridgebackend/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13397 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5976 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13483 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/modules/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/systembridgebackend/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6840 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36941 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/systembridgebackend/server/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/systembridgebackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 14:05:07.000000 systembridgebackend-4.2.2/systembridgebackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:05:07.261085 systembridgebackend-4.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-07 14:02:24.000000 systembridgebackend-4.2.2/tests/test__version.py
```

### Comparing `systembridgebackend-4.2.1/LICENSE` & `systembridgebackend-4.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/PKG-INFO` & `systembridgebackend-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.1
+Version: 4.2.2
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgebackend-4.2.1/pyproject.toml` & `systembridgebackend-4.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/setup.py` & `systembridgebackend-4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/__init__.py` & `systembridgebackend-4.2.2/systembridgebackend/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """System Bridge."""
 
 import asyncio
+import logging
 import sys
 
 from systembridgeshared.base import Base
 from systembridgeshared.logger import setup_logger
 from systembridgeshared.settings import Settings
 
 from ._version import __version__
@@ -16,17 +17,20 @@
     """Application."""
 
     def __init__(
         self,
         settings: Settings,
         init: bool = False,
         no_frontend: bool = False,
+        logger: logging.Logger | None = None,
     ) -> None:
         """Initialise."""
-        setup_logger(settings.data.log_level, "systembridgebackend")
+        if logger is None:
+            setup_logger(settings.data.log_level, "systembridgebackend")
+            logging.getLogger("zeroconf").setLevel(logging.ERROR)
         super().__init__()
         if init:
             self._logger.info("Initialised application. Exiting now.")
             sys.exit(0)
 
         self._logger.info("System Bridge Backend (%s)", __version__.public())
```

### Comparing `systembridgebackend-4.2.1/systembridgebackend/__main__.py` & `systembridgebackend-4.2.2/systembridgebackend/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     logging.getLogger("zeroconf").setLevel(logging.ERROR)
 
     try:
         Application(
             settings,
             init=init,
             no_frontend=no_frontend,
+            logger=logger,
         )
     except Exception as exception:  # pylint: disable=broad-except
         logger.fatal("Unhandled error in application", exc_info=exception)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/action.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/action.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/data.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/keyboard.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/keyboard.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/media/__init__.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/media/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/media/windows.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/media/windows.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/power.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/power.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/__init__.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/data.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/data.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/media.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/handlers/threads/update.py` & `systembridgebackend-4.2.2/systembridgebackend/handlers/threads/update.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/__init__.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/battery.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/battery.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/cpu.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/disks.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/displays.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/displays.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/gpus.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/listeners.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/listeners.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/media.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/memory.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/networks.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/processes.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/processes.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/sensors.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/modules/system.py` & `systembridgebackend-4.2.2/systembridgebackend/modules/system.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/server/__init__.py` & `systembridgebackend-4.2.2/systembridgebackend/server/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/server/api.py` & `systembridgebackend-4.2.2/systembridgebackend/server/api.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/server/mdns.py` & `systembridgebackend-4.2.2/systembridgebackend/server/mdns.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend/server/websocket.py` & `systembridgebackend-4.2.2/systembridgebackend/server/websocket.py`

 * *Files identical despite different names*

### Comparing `systembridgebackend-4.2.1/systembridgebackend.egg-info/PKG-INFO` & `systembridgebackend-4.2.2/systembridgebackend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systembridgebackend
-Version: 4.2.1
+Version: 4.2.2
 Summary: System Bridge Backend
 Home-page: https://github.com/timmo001/system-bridge-backend
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
```

### Comparing `systembridgebackend-4.2.1/systembridgebackend.egg-info/SOURCES.txt` & `systembridgebackend-4.2.2/systembridgebackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

