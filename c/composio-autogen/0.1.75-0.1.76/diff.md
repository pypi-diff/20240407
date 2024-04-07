# Comparing `tmp/composio_autogen-0.1.75.tar.gz` & `tmp/composio_autogen-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.75.tar", last modified: Sun Apr  7 11:19:16 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.76.tar", last modified: Sun Apr  7 11:41:40 2024, max compression
```

## Comparing `composio_autogen-0.1.75.tar` & `composio_autogen-0.1.76.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:19:16.300037 composio_autogen-0.1.75/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 11:19:16.299818 composio_autogen-0.1.75/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.75/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:19:16.298742 composio_autogen-0.1.75/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.75/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7299 2024-04-06 13:20:20.000000 composio_autogen-0.1.75/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:19:16.299601 composio_autogen-0.1.75/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 11:19:16.000000 composio_autogen-0.1.75/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-07 11:19:16.000000 composio_autogen-0.1.75/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:19:16.000000 composio_autogen-0.1.75/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-07 11:19:16.000000 composio_autogen-0.1.75/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-07 11:19:16.000000 composio_autogen-0.1.75/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-07 11:18:29.000000 composio_autogen-0.1.75/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:19:16.300078 composio_autogen-0.1.75/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-07 11:18:29.000000 composio_autogen-0.1.75/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:40.621907 composio_autogen-0.1.76/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 11:41:40.621708 composio_autogen-0.1.76/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.76/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:40.620710 composio_autogen-0.1.76/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.76/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7299 2024-04-06 13:20:20.000000 composio_autogen-0.1.76/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:40.621501 composio_autogen-0.1.76/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-07 11:41:40.000000 composio_autogen-0.1.76/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-07 11:40:51.000000 composio_autogen-0.1.76/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:41:40.622094 composio_autogen-0.1.76/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-07 11:40:51.000000 composio_autogen-0.1.76/setup.py
```

### Comparing `composio_autogen-0.1.75/PKG-INFO` & `composio_autogen-0.1.76/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.75
+Version: 0.1.76
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.75
+Requires-Dist: composio_core===0.1.76
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.75/README.md` & `composio_autogen-0.1.76/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.75/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.76/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.75/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.76/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.75
+Version: 0.1.76
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.75
+Requires-Dist: composio_core===0.1.76
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.75/setup.py` & `composio_autogen-0.1.76/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.75",
+    version="0.1.76",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

