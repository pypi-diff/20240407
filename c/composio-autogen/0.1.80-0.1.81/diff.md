# Comparing `tmp/composio_autogen-0.1.80.tar.gz` & `tmp/composio_autogen-0.1.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.1.80.tar", last modified: Sun Apr  7 17:34:07 2024, max compression
+gzip compressed data, was "composio_autogen-0.1.81.tar", last modified: Sun Apr  7 18:13:55 2024, max compression
```

## Comparing `composio_autogen-0.1.80.tar` & `composio_autogen-0.1.81.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:07.240244 composio_autogen-0.1.80/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 17:34:07.240056 composio_autogen-0.1.80/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-02 18:29:17.000000 composio_autogen-0.1.80/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:07.238739 composio_autogen-0.1.80/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       79 2024-04-02 18:29:17.000000 composio_autogen-0.1.80/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7299 2024-04-06 13:52:08.000000 composio_autogen-0.1.80/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 17:34:07.239851 composio_autogen-0.1.80/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3308 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       41 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-07 17:34:07.000000 composio_autogen-0.1.80/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-07 17:33:22.000000 composio_autogen-0.1.80/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 17:34:07.240287 composio_autogen-0.1.80/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      841 2024-04-07 17:33:22.000000 composio_autogen-0.1.80/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:13:55.629236 composio_autogen-0.1.81/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 18:13:55.629013 composio_autogen-0.1.81/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.1.81/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:13:55.627827 composio_autogen-0.1.81/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       79 2024-03-21 07:30:14.000000 composio_autogen-0.1.81/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7469 2024-04-07 18:10:12.000000 composio_autogen-0.1.81/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 18:13:55.628756 composio_autogen-0.1.81/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3308 2024-04-07 18:13:55.000000 composio_autogen-0.1.81/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-07 18:13:55.000000 composio_autogen-0.1.81/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 18:13:55.000000 composio_autogen-0.1.81/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       41 2024-04-07 18:13:55.000000 composio_autogen-0.1.81/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-07 18:13:55.000000 composio_autogen-0.1.81/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-07 18:12:16.000000 composio_autogen-0.1.81/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 18:13:55.629280 composio_autogen-0.1.81/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      841 2024-04-07 18:12:16.000000 composio_autogen-0.1.81/setup.py
```

### Comparing `composio_autogen-0.1.80/PKG-INFO` & `composio_autogen-0.1.81/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.80
+Version: 0.1.81
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.80
+Requires-Dist: composio_core===0.1.81
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.80/README.md` & `composio_autogen-0.1.81/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.1.80/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.1.81/composio_autogen/autogen_toolspec.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,17 @@
             executor: ConversableAgent = None
         ):
         if isinstance(tools, App):
             tools = [tools]
         assert caller or self.caller, "If caller hasn't been specified during initialization, has to be specified during registration"
         assert executor or self.executor, "If executor hasn't been specified during initialization, has to be specified during registration"
 
+        if self.client.is_authenticated() == False:
+            raise Exception("User not authenticated. Please authenticate using composio-cli add <tool_name>")
+    
         action_schemas = self.client.sdk.get_list_of_actions(
                                                 apps=tools)
         
         for schema in action_schemas:
             self._register_schema_to_autogen(action_schema=schema,
                                             caller = caller if caller else self.caller,
                                             executor = executor if executor else self.executor)
```

### Comparing `composio_autogen-0.1.80/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.1.81/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.1.80
+Version: 0.1.81
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.1.80
+Requires-Dist: composio_core===0.1.81
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.1.80/setup.py` & `composio_autogen-0.1.81/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.1.80",
+    version="0.1.81",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

