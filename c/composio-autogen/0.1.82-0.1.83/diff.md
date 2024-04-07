# Comparing `tmp/composio_autogen-0.1.82.tar.gz` & `tmp/composio_autogen-0.1.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.82.tar", last modified: Sun Apr  7 18:20:11 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.83.tar", last modified: Sun Apr  7 18:31:36 2024, max compression
```

## Comparing `composio_autogen-0.1.82.tar` & `composio_autogen-0.1.83.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:20:11.896316 composio_autogen-0.1.82/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 18:20:11.896102 composio_autogen-0.1.82/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.82/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:20:11.895010 composio_autogen-0.1.82/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.82/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7468 2024-04-07 18:18:17.000000 composio_autogen-0.1.82/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:20:11.895829 composio_autogen-0.1.82/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 18:20:11.000000 composio_autogen-0.1.82/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-07 18:20:11.000000 composio_autogen-0.1.82/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 18:20:11.000000 composio_autogen-0.1.82/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-07 18:20:11.000000 composio_autogen-0.1.82/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-07 18:20:11.000000 composio_autogen-0.1.82/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-07 18:19:29.000000 composio_autogen-0.1.82/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 18:20:11.896363 composio_autogen-0.1.82/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-07 18:19:29.000000 composio_autogen-0.1.82/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 18:31:36.656806 composio_autogen-0.1.83/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 18:31:36.656556 composio_autogen-0.1.83/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.83/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 18:31:36.651617 composio_autogen-0.1.83/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.83/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7468 2024-04-07 18:28:35.000000 composio_autogen-0.1.83/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 18:31:36.656265 composio_autogen-0.1.83/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 18:31:36.000000 composio_autogen-0.1.83/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-07 18:31:36.000000 composio_autogen-0.1.83/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 18:31:36.000000 composio_autogen-0.1.83/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-07 18:31:36.000000 composio_autogen-0.1.83/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-07 18:31:36.000000 composio_autogen-0.1.83/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-07 18:30:51.000000 composio_autogen-0.1.83/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 18:31:36.656851 composio_autogen-0.1.83/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-07 18:30:51.000000 composio_autogen-0.1.83/setup.py
```

### Comparing `composio_autogen-0.1.82/PKG-INFO` & `composio_autogen-0.1.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.82
+Version: 0.1.83
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.82
+Requires-Dist: composio_core===0.1.83
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.82/README.md` & `composio_autogen-0.1.83/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.82/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.83/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.82/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.83/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.82
+Version: 0.1.83
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.82
+Requires-Dist: composio_core===0.1.83
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.82/setup.py` & `composio_autogen-0.1.83/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.82",
+    version="0.1.83",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

