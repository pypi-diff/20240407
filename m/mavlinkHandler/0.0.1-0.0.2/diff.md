# Comparing `tmp/mavlinkHandler-0.0.1.tar.gz` & `tmp/mavlinkHandler-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavlinkHandler-0.0.1.tar", last modified: Sun Apr  7 08:10:22 2024, max compression
+gzip compressed data, was "mavlinkHandler-0.0.2.tar", last modified: Sun Apr  7 08:15:17 2024, max compression
```

## Comparing `mavlinkHandler-0.0.1.tar` & `mavlinkHandler-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:10:22.498131 mavlinkHandler-0.0.1/
--rw-r--r--   0 thatcher   (501) staff       (20)    35149 2024-04-07 07:45:38.000000 mavlinkHandler-0.0.1/LICENSE
--rw-r--r--   0 thatcher   (501) staff       (20)      896 2024-04-07 08:10:22.497943 mavlinkHandler-0.0.1/PKG-INFO
--rw-r--r--   0 thatcher   (501) staff       (20)      406 2024-04-07 07:52:22.000000 mavlinkHandler-0.0.1/README.md
-drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:10:22.497003 mavlinkHandler-0.0.1/mavlinkHandler/
--rw-r--r--   0 thatcher   (501) staff       (20)      100 2024-04-07 07:55:01.000000 mavlinkHandler-0.0.1/mavlinkHandler/__init__.py
--rw-r--r--   0 thatcher   (501) staff       (20)     7331 2024-04-07 07:53:19.000000 mavlinkHandler-0.0.1/mavlinkHandler/mavlinkHandler.py
-drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:10:22.497767 mavlinkHandler-0.0.1/mavlinkHandler.egg-info/
--rw-r--r--   0 thatcher   (501) staff       (20)      896 2024-04-07 08:10:22.000000 mavlinkHandler-0.0.1/mavlinkHandler.egg-info/PKG-INFO
--rw-r--r--   0 thatcher   (501) staff       (20)      238 2024-04-07 08:10:22.000000 mavlinkHandler-0.0.1/mavlinkHandler.egg-info/SOURCES.txt
--rw-r--r--   0 thatcher   (501) staff       (20)        1 2024-04-07 08:10:22.000000 mavlinkHandler-0.0.1/mavlinkHandler.egg-info/dependency_links.txt
--rw-r--r--   0 thatcher   (501) staff       (20)       15 2024-04-07 08:10:22.000000 mavlinkHandler-0.0.1/mavlinkHandler.egg-info/top_level.txt
--rw-r--r--   0 thatcher   (501) staff       (20)       38 2024-04-07 08:10:22.498175 mavlinkHandler-0.0.1/setup.cfg
--rw-r--r--   0 thatcher   (501) staff       (20)      699 2024-04-07 08:10:18.000000 mavlinkHandler-0.0.1/setup.py
+drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:15:17.689239 mavlinkHandler-0.0.2/
+-rw-r--r--   0 thatcher   (501) staff       (20)    35149 2024-04-07 07:45:38.000000 mavlinkHandler-0.0.2/LICENSE
+-rw-r--r--   0 thatcher   (501) staff       (20)     1063 2024-04-07 08:15:17.689038 mavlinkHandler-0.0.2/PKG-INFO
+-rw-r--r--   0 thatcher   (501) staff       (20)      573 2024-04-07 08:13:11.000000 mavlinkHandler-0.0.2/README.md
+drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:15:17.688067 mavlinkHandler-0.0.2/mavlinkHandler/
+-rw-r--r--   0 thatcher   (501) staff       (20)      100 2024-04-07 07:55:01.000000 mavlinkHandler-0.0.2/mavlinkHandler/__init__.py
+-rw-r--r--   0 thatcher   (501) staff       (20)     7331 2024-04-07 07:53:19.000000 mavlinkHandler-0.0.2/mavlinkHandler/mavlinkHandler.py
+drwxr-xr-x   0 thatcher   (501) staff       (20)        0 2024-04-07 08:15:17.688840 mavlinkHandler-0.0.2/mavlinkHandler.egg-info/
+-rw-r--r--   0 thatcher   (501) staff       (20)     1063 2024-04-07 08:15:17.000000 mavlinkHandler-0.0.2/mavlinkHandler.egg-info/PKG-INFO
+-rw-r--r--   0 thatcher   (501) staff       (20)      238 2024-04-07 08:15:17.000000 mavlinkHandler-0.0.2/mavlinkHandler.egg-info/SOURCES.txt
+-rw-r--r--   0 thatcher   (501) staff       (20)        1 2024-04-07 08:15:17.000000 mavlinkHandler-0.0.2/mavlinkHandler.egg-info/dependency_links.txt
+-rw-r--r--   0 thatcher   (501) staff       (20)       15 2024-04-07 08:15:17.000000 mavlinkHandler-0.0.2/mavlinkHandler.egg-info/top_level.txt
+-rw-r--r--   0 thatcher   (501) staff       (20)       38 2024-04-07 08:15:17.689284 mavlinkHandler-0.0.2/setup.cfg
+-rw-r--r--   0 thatcher   (501) staff       (20)      699 2024-04-07 08:11:34.000000 mavlinkHandler-0.0.2/setup.py
```

### Comparing `mavlinkHandler-0.0.1/LICENSE` & `mavlinkHandler-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mavlinkHandler-0.0.1/PKG-INFO` & `mavlinkHandler-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavlinkHandler
-Version: 0.0.1
+Version: 0.0.2
 Summary: A controller library for UAVs, compatible with both ArduPilot and DroneKit
 Home-page: https://github.com/0EA/mavlinkHandler
 Author: Nurullah Eren Acar
 Author-email: n.erenacar13@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,16 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your-username/mavlinkHandler/blob/main/LICENSE)
 
 mavlinkHandler is a controller library for UAVs, compatible with both ArduPilot and DroneKit.
 
 ## Installation
 
 You can install mavlinkHandler using pip:
+pip install mavlinkHandler
+
+## Usage
+
+```
+from mavlinkHandler import MAVLinkHandlerDronekit as MAVLinkHandler
+
+mavlink_handler = MAVLinkHandler('127.0.0.1:14591')
+```
```

### Comparing `mavlinkHandler-0.0.1/mavlinkHandler/mavlinkHandler.py` & `mavlinkHandler-0.0.2/mavlinkHandler/mavlinkHandler.py`

 * *Files identical despite different names*

### Comparing `mavlinkHandler-0.0.1/mavlinkHandler.egg-info/PKG-INFO` & `mavlinkHandler-0.0.2/mavlinkHandler.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mavlinkHandler
-Version: 0.0.1
+Version: 0.0.2
 Summary: A controller library for UAVs, compatible with both ArduPilot and DroneKit
 Home-page: https://github.com/0EA/mavlinkHandler
 Author: Nurullah Eren Acar
 Author-email: n.erenacar13@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,16 @@
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/your-username/mavlinkHandler/blob/main/LICENSE)
 
 mavlinkHandler is a controller library for UAVs, compatible with both ArduPilot and DroneKit.
 
 ## Installation
 
 You can install mavlinkHandler using pip:
+pip install mavlinkHandler
+
+## Usage
+
+```
+from mavlinkHandler import MAVLinkHandlerDronekit as MAVLinkHandler
+
+mavlink_handler = MAVLinkHandler('127.0.0.1:14591')
+```
```

### Comparing `mavlinkHandler-0.0.1/setup.py` & `mavlinkHandler-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mavlinkHandler",
-    version="0.0.1",
+    version="0.0.2",
     author="Nurullah Eren Acar",
     author_email="n.erenacar13@gmail.com",
     description="A controller library for UAVs, compatible with both ArduPilot and DroneKit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/0EA/mavlinkHandler",
     packages=setuptools.find_packages(),
```

