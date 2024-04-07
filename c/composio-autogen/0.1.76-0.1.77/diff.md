# Comparing `tmp/composio_autogen-0.1.76.tar.gz` & `tmp/composio_autogen-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.76.tar", last modified: Sun Apr  7 11:41:40 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.77.tar", last modified: Sun Apr  7 14:48:58 2024, max compression
```

## Comparing `composio_autogen-0.1.76.tar` & `composio_autogen-0.1.77.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:40.621907 composio_autogen-0.1.76/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 11:41:40.621708 composio_autogen-0.1.76/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.76/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:40.620710 composio_autogen-0.1.76/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.76/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7299 2024-04-06 13:20:20.000000 composio_autogen-0.1.76/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:40.621501 composio_autogen-0.1.76/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-07 11:40:51.000000 composio_autogen-0.1.76/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:41:40.622094 composio_autogen-0.1.76/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-07 11:40:51.000000 composio_autogen-0.1.76/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:58.274696 composio_autogen-0.1.77/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 14:48:58.274501 composio_autogen-0.1.77/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.77/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:58.273553 composio_autogen-0.1.77/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.77/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7299 2024-04-06 13:20:20.000000 composio_autogen-0.1.77/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:58.274295 composio_autogen-0.1.77/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 14:48:58.000000 composio_autogen-0.1.77/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-07 14:48:58.000000 composio_autogen-0.1.77/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 14:48:58.000000 composio_autogen-0.1.77/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-07 14:48:58.000000 composio_autogen-0.1.77/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-07 14:48:58.000000 composio_autogen-0.1.77/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-07 14:47:54.000000 composio_autogen-0.1.77/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 14:48:58.274738 composio_autogen-0.1.77/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-07 14:47:54.000000 composio_autogen-0.1.77/setup.py
```

### Comparing `composio_autogen-0.1.76/PKG-INFO` & `composio_autogen-0.1.77/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.76
+Version: 0.1.77
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.76
+Requires-Dist: composio_core===0.1.77
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.76/README.md` & `composio_autogen-0.1.77/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.76/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.77/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.76/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.77/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.76
+Version: 0.1.77
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.76
+Requires-Dist: composio_core===0.1.77
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

