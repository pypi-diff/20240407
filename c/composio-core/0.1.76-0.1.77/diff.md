# Comparing `tmp/composio_core-0.1.76.tar.gz` & `tmp/composio_core-0.1.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.76.tar", last modified: Sun Apr  7 11:41:07 2024, max compression
+gzip compressed data, was "composio_core-0.1.77.tar", last modified: Sun Apr  7 14:48:24 2024, max compression
```

## Comparing `composio_core-0.1.76.tar` & `composio_core-0.1.77.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.973451 composio_core-0.1.76/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.76/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:41:07.973214 composio_core-0.1.76/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.76/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.970023 composio_core-0.1.76/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.76/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    12441 2024-04-07 11:39:39.000000 composio_core-0.1.76/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.972042 composio_core-0.1.76/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.76/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5679 2024-04-07 11:13:55.000000 composio_core-0.1.76/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6973 2024-04-07 11:39:25.000000 composio_core-0.1.76/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-07 11:17:47.000000 composio_core-0.1.76/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-04-07 11:38:27.000000 composio_core-0.1.76/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.76/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.972943 composio_core-0.1.76/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.76/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.76/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:41:07.973499 composio_core-0.1.76/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-07 11:40:51.000000 composio_core-0.1.76/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:24.810852 composio_core-0.1.77/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.77/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 14:48:24.810634 composio_core-0.1.77/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.77/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:24.806636 composio_core-0.1.77/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.77/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    12441 2024-04-07 11:39:39.000000 composio_core-0.1.77/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:24.809369 composio_core-0.1.77/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.77/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5679 2024-04-07 11:13:55.000000 composio_core-0.1.77/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6973 2024-04-07 11:39:25.000000 composio_core-0.1.77/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    16337 2024-04-07 14:47:23.000000 composio_core-0.1.77/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-04-07 11:38:27.000000 composio_core-0.1.77/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.77/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 14:48:24.810372 composio_core-0.1.77/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 14:48:24.000000 composio_core-0.1.77/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-07 14:48:24.000000 composio_core-0.1.77/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 14:48:24.000000 composio_core-0.1.77/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-07 14:48:24.000000 composio_core-0.1.77/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-07 14:48:24.000000 composio_core-0.1.77/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-07 14:48:24.000000 composio_core-0.1.77/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.77/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.77/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 14:48:24.810899 composio_core-0.1.77/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-07 14:47:54.000000 composio_core-0.1.77/setup.py
```

### Comparing `composio_core-0.1.76/PKG-INFO` & `composio_core-0.1.77/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.76
+Version: 0.1.77
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.76/composio/composio_cli.py` & `composio_core-0.1.77/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.76/composio/sdk/core.py` & `composio_core-0.1.77/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.76/composio/sdk/enums.py` & `composio_core-0.1.77/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.76/composio/sdk/sdk.py` & `composio_core-0.1.77/composio/sdk/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,29 +44,31 @@
                 return connection_info
             time.sleep(1)
         raise TimeoutError(
             "Connection did not become active within the timeout period."
         )
 
 
-class OAuth2ConnectionParams(BaseModel):
+class AuthConnectionParams(BaseModel):
     scope: Optional[str] = None
     base_url: Optional[str] = None
-    client_id: str
+    client_id: Optional[str] = None
     token_type: Optional[str] = None
     access_token: Optional[str] = None
-    client_secret: str
+    client_secret: Optional[str] = None
+    consumer_id: Optional[str] = None
+    consumer_secret: Optional[str] = None
     headers: Optional[dict] = None
     queryParams: Optional[dict] = None
 
 
 class ConnectedAccount(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     integrationId: str
-    connectionParams: OAuth2ConnectionParams
+    connectionParams: AuthConnectionParams
     appUniqueId: str
     id: str
     status: str
     createdAt: str
     updatedAt: str
 
     sdk_instance: "Composio" = None
```

### Comparing `composio_core-0.1.76/composio/sdk/storage.py` & `composio_core-0.1.77/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.76/composio/sdk/utils.py` & `composio_core-0.1.77/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.76/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.77/composio_core.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.76
+Version: 0.1.77
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.76/setup.py` & `composio_core-0.1.77/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.76",
+    version="0.1.77",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```
