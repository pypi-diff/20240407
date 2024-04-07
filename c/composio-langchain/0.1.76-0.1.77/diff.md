# Comparing `tmp/composio_langchain-0.1.76.tar.gz` & `tmp/composio_langchain-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.1.76.tar", last modified: Sun Apr  7 11:41:19 2024, max compression
+gzip compressed data, was "composio_langchain-0.1.77.tar", last modified: Sun Apr  7 14:48:36 2024, max compression
```

## Comparing `composio_langchain-0.1.76.tar` & `composio_langchain-0.1.77.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:19.343877 composio_langchain-0.1.76/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.76/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-07 11:41:19.343630 composio_langchain-0.1.76/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.76/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:19.342476 composio_langchain-0.1.76/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)       88 2024-03-24 04:08:45.000000 composio_langchain-0.1.76/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5257 2024-04-06 13:18:09.000000 composio_langchain-0.1.76/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.76/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:19.343396 composio_langchain-0.1.76/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-07 11:41:19.000000 composio_langchain-0.1.76/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-07 11:41:19.000000 composio_langchain-0.1.76/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:41:19.000000 composio_langchain-0.1.76/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      149 2024-04-07 11:41:19.000000 composio_langchain-0.1.76/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-07 11:41:19.000000 composio_langchain-0.1.76/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      455 2024-04-07 11:40:51.000000 composio_langchain-0.1.76/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:41:19.343918 composio_langchain-0.1.76/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-07 11:40:51.000000 composio_langchain-0.1.76/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:36.871626 composio_langchain-0.1.77/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.1.77/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-07 14:48:36.871420 composio_langchain-0.1.77/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.1.77/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:36.870107 composio_langchain-0.1.77/composio_langchain/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       88 2024-03-24 04:08:45.000000 composio_langchain-0.1.77/composio_langchain/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5257 2024-04-06 13:18:09.000000 composio_langchain-0.1.77/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.1.77/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:36.871159 composio_langchain-0.1.77/composio_langchain.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3334 2024-04-07 14:48:36.000000 composio_langchain-0.1.77/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-07 14:48:36.000000 composio_langchain-0.1.77/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 14:48:36.000000 composio_langchain-0.1.77/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      149 2024-04-07 14:48:36.000000 composio_langchain-0.1.77/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-07 14:48:36.000000 composio_langchain-0.1.77/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      455 2024-04-07 14:47:54.000000 composio_langchain-0.1.77/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 14:48:36.871687 composio_langchain-0.1.77/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      839 2024-04-07 14:47:54.000000 composio_langchain-0.1.77/setup.py
```

### Comparing `composio_langchain-0.1.76/PKG-INFO` & `composio_langchain-0.1.77/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.76
+Version: 0.1.77
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.76
+Requires-Dist: composio_core===0.1.77
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.76/README.md` & `composio_langchain-0.1.77/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.76/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.1.77/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.76/composio_langchain/pydantic_utils.py` & `composio_langchain-0.1.77/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.1.76/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.1.77/composio_langchain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.1.76
+Version: 0.1.77
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.1.76
+Requires-Dist: composio_core===0.1.77
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.1.76/setup.py` & `composio_langchain-0.1.77/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.1.76",
+    version="0.1.77",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

