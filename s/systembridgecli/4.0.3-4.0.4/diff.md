# Comparing `tmp/systembridgecli-4.0.3.tar.gz` & `tmp/systembridgecli-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgecli-4.0.3.tar", last modified: Sun Mar 31 14:38:51 2024, max compression
+gzip compressed data, was "systembridgecli-4.0.4.tar", last modified: Sun Apr  7 12:17:41 2024, max compression
```

## Comparing `systembridgecli-4.0.3.tar` & `systembridgecli-4.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:38:51.504132 systembridgecli-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-31 14:38:30.000000 systembridgecli-4.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-31 14:38:51.504132 systembridgecli-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-31 14:38:30.000000 systembridgecli-4.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-03-31 14:38:30.000000 systembridgecli-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 14:38:51.504132 systembridgecli-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-31 14:38:30.000000 systembridgecli-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:38:51.504132 systembridgecli-4.0.3/systembridgecli/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-31 14:38:30.000000 systembridgecli-4.0.3/systembridgecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-03-31 14:38:30.000000 systembridgecli-4.0.3/systembridgecli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-31 14:38:50.000000 systembridgecli-4.0.3/systembridgecli/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 14:38:51.504132 systembridgecli-4.0.3/systembridgecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-31 14:38:51.000000 systembridgecli-4.0.3/systembridgecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-31 14:38:51.000000 systembridgecli-4.0.3/systembridgecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 14:38:51.000000 systembridgecli-4.0.3/systembridgecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-31 14:38:51.000000 systembridgecli-4.0.3/systembridgecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-31 14:38:51.000000 systembridgecli-4.0.3/systembridgecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7668 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/systembridgecli/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/systembridgecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-04-07 12:17:15.000000 systembridgecli-4.0.4/systembridgecli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-07 12:17:39.000000 systembridgecli-4.0.4/systembridgecli/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:17:41.679540 systembridgecli-4.0.4/systembridgecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 12:17:41.000000 systembridgecli-4.0.4/systembridgecli.egg-info/top_level.txt
```

### Comparing `systembridgecli-4.0.3/LICENSE` & `systembridgecli-4.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgecli-4.0.3/PKG-INFO` & `systembridgecli-4.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: systembridgecli
-Version: 4.0.3
+Version: 4.0.4
 Summary: System Bridge CLI
 Home-page: https://github.com/timmo001/system-bridge-cli
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: incremental==22.10.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: systembridgeconnector>=4.0.5
 Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.0
+Requires-Dist: typer==0.12.1
 
 # System Bridge - CLI
 
 This is a CLI interface package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

### Comparing `systembridgecli-4.0.3/pyproject.toml` & `systembridgecli-4.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgecli-4.0.3/setup.py` & `systembridgecli-4.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgecli-4.0.3/systembridgecli/__main__.py` & `systembridgecli-4.0.4/systembridgecli/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """System Bridge CLI."""
+
 from __future__ import annotations
 
 import asyncio
 import concurrent.futures
 from dataclasses import asdict, is_dataclass
 import json
 import os
@@ -11,21 +12,21 @@
 from typing import Any
 from uuid import uuid4
 
 import aiohttp
 import typer
 
 from systembridgecli._version import __version__
-from systembridgeconnector.websocket_client import WebSocketClient
-from systembridgemodels.modules import GetData, ModulesData
-from systembridgeshared.common import get_user_data_directory
-from systembridgeshared.exceptions import (
+from systembridgeconnector.exceptions import (
     ConnectionClosedException,
     ConnectionErrorException,
 )
+from systembridgeconnector.websocket_client import WebSocketClient
+from systembridgemodels.modules import GetData, ModulesData
+from systembridgeshared.common import get_user_data_directory
 from systembridgeshared.logger import setup_logger
 from systembridgeshared.settings import Settings
 
 setup_logger("ERROR", "system-bridge-cli")
 
 app = typer.Typer()
 settings = Settings()
```

### Comparing `systembridgecli-4.0.3/systembridgecli.egg-info/PKG-INFO` & `systembridgecli-4.0.4/systembridgecli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: systembridgecli
-Version: 4.0.3
+Version: 4.0.4
 Summary: System Bridge CLI
 Home-page: https://github.com/timmo001/system-bridge-cli
 Author: Aidan Timson (Timmo)
 Author-email: aidan@timmo.dev
 License: Apache-2.0
 Keywords: system-bridge
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: incremental==22.10.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: systembridgeconnector>=4.0.5
 Requires-Dist: systembridgeshared>=4.0.4
-Requires-Dist: typer==0.12.0
+Requires-Dist: typer==0.12.1
 
 # System Bridge - CLI
 
 This is a CLI interface package for the [System Bridge](https://github.com/timmo001/system-bridge) project.
```

