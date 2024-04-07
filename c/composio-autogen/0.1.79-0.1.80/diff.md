# Comparing `tmp/composio_autogen-0.1.79.tar.gz` & `tmp/composio_autogen-0.1.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.79.tar", last modified: Sun Apr  7 15:54:12 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.80.tar", last modified: Sun Apr  7 17:34:07 2024, max compression
```

## Comparing `composio_autogen-0.1.79.tar` & `composio_autogen-0.1.80.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 15:54:12.107082 composio_autogen-0.1.79/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 15:54:12.106880 composio_autogen-0.1.79/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.79/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 15:54:12.105566 composio_autogen-0.1.79/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.79/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7299 2024-04-06 13:52:08.000000 composio_autogen-0.1.79/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 15:54:12.106672 composio_autogen-0.1.79/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 15:54:12.000000 composio_autogen-0.1.79/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-07 15:54:12.000000 composio_autogen-0.1.79/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 15:54:12.000000 composio_autogen-0.1.79/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-07 15:54:12.000000 composio_autogen-0.1.79/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-07 15:54:12.000000 composio_autogen-0.1.79/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-07 15:53:40.000000 composio_autogen-0.1.79/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 15:54:12.107136 composio_autogen-0.1.79/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-07 15:53:40.000000 composio_autogen-0.1.79/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:07.240244 composio_autogen-0.1.80/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 17:34:07.240056 composio_autogen-0.1.80/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.80/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:07.238739 composio_autogen-0.1.80/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.80/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7299 2024-04-06 13:52:08.000000 composio_autogen-0.1.80/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:07.239851 composio_autogen-0.1.80/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-07 17:33:22.000000 composio_autogen-0.1.80/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 17:34:07.240287 composio_autogen-0.1.80/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-07 17:33:22.000000 composio_autogen-0.1.80/setup.py
```

### Comparing `composio_autogen-0.1.79/PKG-INFO` & `composio_autogen-0.1.80/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.79
+Version: 0.1.80
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.79
+Requires-Dist: composio_core===0.1.80
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.79/README.md` & `composio_autogen-0.1.80/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.79/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.80/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.79/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.80/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.79
+Version: 0.1.80
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.79
+Requires-Dist: composio_core===0.1.80
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.79/setup.py` & `composio_autogen-0.1.80/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.79",
+    version="0.1.80",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

