# Comparing `tmp/pulumi_rke-3.4.0a1712402957.tar.gz` & `tmp/pulumi_rke-3.4.0a1712470927.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rke-3.4.0a1712402957.tar", last modified: Sat Apr  6 11:34:45 2024, max compression
+gzip compressed data, was "pulumi_rke-3.4.0a1712470927.tar", last modified: Sun Apr  7 06:26:57 2024, max compression
```

## Comparing `pulumi_rke-3.4.0a1712402957.tar` & `pulumi_rke-3.4.0a1712470927.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:34:45.903129 pulumi_rke-3.4.0a1712402957/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-06 11:34:45.903129 pulumi_rke-3.4.0a1712402957/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:34:45.899129 pulumi_rke-3.4.0a1712402957/pulumi_rke/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   398152 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)   139188 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:34:45.903129 pulumi_rke-3.4.0a1712402957/pulumi_rke/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)   359046 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:34:45.903129 pulumi_rke-3.4.0a1712402957/pulumi_rke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-06 11:34:45.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-06 11:34:45.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:34:45.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 11:34:45.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 11:34:45.000000 pulumi_rke-3.4.0a1712402957/pulumi_rke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-06 11:34:37.000000 pulumi_rke-3.4.0a1712402957/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 11:34:45.903129 pulumi_rke-3.4.0a1712402957/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:26:57.742864 pulumi_rke-3.4.0a1712470927/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-07 06:26:57.742864 pulumi_rke-3.4.0a1712470927/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:26:57.742864 pulumi_rke-3.4.0a1712470927/pulumi_rke/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   398152 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139188 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:26:57.742864 pulumi_rke-3.4.0a1712470927/pulumi_rke/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)   359046 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:26:57.742864 pulumi_rke-3.4.0a1712470927/pulumi_rke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-07 06:26:57.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-07 06:26:57.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:26:57.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 06:26:57.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 06:26:57.000000 pulumi_rke-3.4.0a1712470927/pulumi_rke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-07 06:26:46.000000 pulumi_rke-3.4.0a1712470927/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:26:57.742864 pulumi_rke-3.4.0a1712470927/setup.cfg
```

### Comparing `pulumi_rke-3.4.0a1712402957/PKG-INFO` & `pulumi_rke-3.4.0a1712470927/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rke
-Version: 3.4.0a1712402957
+Version: 3.4.0a1712470927
 Summary: A Pulumi package for creating and managing rke cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi,rke
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.4.0a1712402957/README.md` & `pulumi_rke-3.4.0a1712470927/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke/__init__.py` & `pulumi_rke-3.4.0a1712470927/pulumi_rke/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke/_inputs.py` & `pulumi_rke-3.4.0a1712470927/pulumi_rke/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke/_utilities.py` & `pulumi_rke-3.4.0a1712470927/pulumi_rke/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke/cluster.py` & `pulumi_rke-3.4.0a1712470927/pulumi_rke/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke/config/vars.py` & `pulumi_rke-3.4.0a1712470927/pulumi_rke/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke/outputs.py` & `pulumi_rke-3.4.0a1712470927/pulumi_rke/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke/provider.py` & `pulumi_rke-3.4.0a1712470927/pulumi_rke/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.4.0a1712402957/pulumi_rke.egg-info/PKG-INFO` & `pulumi_rke-3.4.0a1712470927/pulumi_rke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rke
-Version: 3.4.0a1712402957
+Version: 3.4.0a1712470927
 Summary: A Pulumi package for creating and managing rke cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi,rke
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.4.0a1712402957/pyproject.toml` & `pulumi_rke-3.4.0a1712470927/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rke"
   description = "A Pulumi package for creating and managing rke cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rke"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.4.0a1712402957"
+  version = "3.4.0a1712470927"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rke"
 
 [build-system]
```

