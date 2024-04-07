# Comparing `tmp/pharindoko.cdk-internal-gateway-1.4.8.tar.gz` & `tmp/pharindoko.cdk-internal-gateway-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharindoko.cdk-internal-gateway-1.4.8.tar", last modified: Mon Mar 25 14:57:23 2024, max compression
+gzip compressed data, was "pharindoko.cdk-internal-gateway-1.4.9.tar", last modified: Sun Apr  7 18:43:57 2024, max compression
```

## Comparing `pharindoko.cdk-internal-gateway-1.4.8.tar` & `pharindoko.cdk-internal-gateway-1.4.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/cdk_internal_gateway/
--rw-r--r--   0 runner    (1001) docker     (127)   119161 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/cdk_internal_gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/cdk_internal_gateway/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/cdk_internal_gateway/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   195392 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.4.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:57:13.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/cdk_internal_gateway/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 14:57:23.791527 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-03-25 14:57:23.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-25 14:57:23.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 14:57:23.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-25 14:57:23.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-25 14:57:23.000000 pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:43:57.851470 pharindoko.cdk-internal-gateway-1.4.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-07 18:43:57.851470 pharindoko.cdk-internal-gateway-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6746 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:43:57.851470 pharindoko.cdk-internal-gateway-1.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:43:57.847470 pharindoko.cdk-internal-gateway-1.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:43:57.847470 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:43:57.847470 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/cdk_internal_gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)   119161 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/cdk_internal_gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:43:57.851470 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/cdk_internal_gateway/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/cdk_internal_gateway/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195391 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.4.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:43:44.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/cdk_internal_gateway/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:43:57.847470 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7683 2024-04-07 18:43:57.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-07 18:43:57.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:43:57.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 18:43:57.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 18:43:57.000000 pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/top_level.txt
```

### Comparing `pharindoko.cdk-internal-gateway-1.4.8/LICENSE` & `pharindoko.cdk-internal-gateway-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pharindoko.cdk-internal-gateway-1.4.8/PKG-INFO` & `pharindoko.cdk-internal-gateway-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharindoko.cdk-internal-gateway
-Version: 1.4.8
+Version: 1.4.9
 Summary: CDK construct to create to create internal serverless applications.
 Home-page: https://github.com/pharindoko/cdk-internal-gateway.git
 Author: Florian Fuß
 License: Apache-2.0
 Project-URL: Source, https://github.com/pharindoko/cdk-internal-gateway.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pharindoko.cdk-internal-gateway-1.4.8/README.md` & `pharindoko.cdk-internal-gateway-1.4.9/README.md`

 * *Files identical despite different names*

### Comparing `pharindoko.cdk-internal-gateway-1.4.8/setup.py` & `pharindoko.cdk-internal-gateway-1.4.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "pharindoko.cdk-internal-gateway",
-    "version": "1.4.8",
+    "version": "1.4.9",
     "description": "CDK construct to create to create internal serverless applications.",
     "license": "Apache-2.0",
     "url": "https://github.com/pharindoko/cdk-internal-gateway.git",
     "long_description_content_type": "text/markdown",
     "author": "Florian Fuß",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "pharindoko.cdk_internal_gateway",
         "pharindoko.cdk_internal_gateway._jsii"
     ],
     "package_data": {
         "pharindoko.cdk_internal_gateway._jsii": [
-            "cdk-internal-gateway@1.4.8.jsii.tgz"
+            "cdk-internal-gateway@1.4.9.jsii.tgz"
         ],
         "pharindoko.cdk_internal_gateway": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko/cdk_internal_gateway/__init__.py` & `pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko/cdk_internal_gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO` & `pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharindoko.cdk-internal-gateway
-Version: 1.4.8
+Version: 1.4.9
 Summary: CDK construct to create to create internal serverless applications.
 Home-page: https://github.com/pharindoko/cdk-internal-gateway.git
 Author: Florian Fuß
 License: Apache-2.0
 Project-URL: Source, https://github.com/pharindoko/cdk-internal-gateway.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `pharindoko.cdk-internal-gateway-1.4.8/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt` & `pharindoko.cdk-internal-gateway-1.4.9/src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/pharindoko.cdk_internal_gateway.egg-info/SOURCES.txt
 src/pharindoko.cdk_internal_gateway.egg-info/dependency_links.txt
 src/pharindoko.cdk_internal_gateway.egg-info/requires.txt
 src/pharindoko.cdk_internal_gateway.egg-info/top_level.txt
 src/pharindoko/cdk_internal_gateway/__init__.py
 src/pharindoko/cdk_internal_gateway/py.typed
 src/pharindoko/cdk_internal_gateway/_jsii/__init__.py
-src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.4.8.jsii.tgz
+src/pharindoko/cdk_internal_gateway/_jsii/cdk-internal-gateway@1.4.9.jsii.tgz
```

