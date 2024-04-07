# Comparing `tmp/composio_crewai-0.1.80.tar.gz` & `tmp/composio_crewai-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.1.80.tar", last modified: Sun Apr  7 17:34:00 2024, max compression
+gzip compressed data, was "composio_crewai-0.1.81.tar", last modified: Sun Apr  7 18:13:36 2024, max compression
```

## Comparing `composio_crewai-0.1.80.tar` & `composio_crewai-0.1.81.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:00.264289 composio_crewai-0.1.80/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3078 2024-04-07 17:34:00.264076 composio_crewai-0.1.80/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2576 2024-04-02 18:29:17.000000 composio_crewai-0.1.80/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:00.262800 composio_crewai-0.1.80/composio_crewai/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       89 2024-04-02 18:29:17.000000 composio_crewai-0.1.80/composio_crewai/__init__.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:00.263795 composio_crewai-0.1.80/composio_crewai.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3078 2024-04-07 17:34:00.000000 composio_crewai-0.1.80/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      255 2024-04-07 17:34:00.000000 composio_crewai-0.1.80/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 17:34:00.000000 composio_crewai-0.1.80/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       28 2024-04-07 17:34:00.000000 composio_crewai-0.1.80/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-04-07 17:34:00.000000 composio_crewai-0.1.80/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      276 2024-04-07 17:33:22.000000 composio_crewai-0.1.80/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 17:34:00.264340 composio_crewai-0.1.80/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      839 2024-04-07 17:33:22.000000 composio_crewai-0.1.80/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:13:36.325003 composio_crewai-0.1.81/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-07 18:13:36.322996 composio_crewai-0.1.81/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2576 2024-04-02 16:50:40.000000 composio_crewai-0.1.81/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:13:36.311308 composio_crewai-0.1.81/composio_crewai/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       89 2024-03-20 12:04:29.000000 composio_crewai-0.1.81/composio_crewai/__init__.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:13:36.321573 composio_crewai-0.1.81/composio_crewai.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3078 2024-04-07 18:13:36.000000 composio_crewai-0.1.81/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      255 2024-04-07 18:13:36.000000 composio_crewai-0.1.81/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 18:13:36.000000 composio_crewai-0.1.81/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       28 2024-04-07 18:13:36.000000 composio_crewai-0.1.81/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-04-07 18:13:36.000000 composio_crewai-0.1.81/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      276 2024-04-07 18:12:16.000000 composio_crewai-0.1.81/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 18:13:36.325379 composio_crewai-0.1.81/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-07 18:12:16.000000 composio_crewai-0.1.81/setup.py
```

### Comparing `composio_crewai-0.1.80/PKG-INFO` & `composio_crewai-0.1.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.1.80
+Version: 0.1.81
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.1.80
+Requires-Dist: composio_langchain===0.1.81
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.1.80/README.md` & `composio_crewai-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `composio_crewai-0.1.80/composio_crewai.egg-info/PKG-INFO` & `composio_crewai-0.1.81/composio_crewai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.1.80
+Version: 0.1.81
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.1.80
+Requires-Dist: composio_langchain===0.1.81
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.1.80/setup.py` & `composio_crewai-0.1.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_crewai",
-    version="0.1.80",
+    version="0.1.81",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

