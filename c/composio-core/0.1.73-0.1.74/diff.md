# Comparing `tmp/composio_core-0.1.73.tar.gz` & `tmp/composio_core-0.1.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.73.tar", last modified: Sat Apr  6 14:08:04 2024, max compression
+gzip compressed data, was "composio_core-0.1.74.tar", last modified: Sun Apr  7 05:25:19 2024, max compression
```

## Comparing `composio_core-0.1.73.tar` & `composio_core-0.1.74.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 14:08:04.094663 composio_core-0.1.73/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.73/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-06 14:08:04.093920 composio_core-0.1.73/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.73/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 14:08:04.089421 composio_core-0.1.73/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.73/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    11895 2024-04-06 12:54:36.000000 composio_core-0.1.73/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 14:08:04.090814 composio_core-0.1.73/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.73/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5542 2024-04-06 12:52:11.000000 composio_core-0.1.73/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.73/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-06 12:36:58.000000 composio_core-0.1.73/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2210 2024-04-06 14:07:56.000000 composio_core-0.1.73/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.73/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-06 14:08:04.093155 composio_core-0.1.73/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-06 14:08:04.000000 composio_core-0.1.73/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-06 14:08:04.000000 composio_core-0.1.73/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-06 14:08:04.000000 composio_core-0.1.73/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-06 14:08:04.000000 composio_core-0.1.73/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-06 14:08:04.000000 composio_core-0.1.73/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-06 14:08:04.000000 composio_core-0.1.73/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.73/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.73/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-06 14:08:04.094842 composio_core-0.1.73/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-06 14:07:53.000000 composio_core-0.1.73/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.419823 composio_core-0.1.74/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.74/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 05:25:19.419608 composio_core-0.1.74/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.74/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.416267 composio_core-0.1.74/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.74/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    11895 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.418320 composio_core-0.1.74/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.74/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5542 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     7414 2024-04-04 15:13:54.000000 composio_core-0.1.74/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    16227 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2211 2024-04-07 05:24:38.000000 composio_core-0.1.74/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2861 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.419389 composio_core-0.1.74/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       91 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      509 2024-04-06 13:53:19.000000 composio_core-0.1.74/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       92 2024-04-06 13:54:53.000000 composio_core-0.1.74/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 05:25:19.419861 composio_core-0.1.74/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1134 2024-04-07 05:25:03.000000 composio_core-0.1.74/setup.py
```

### Comparing `composio_core-0.1.73/PKG-INFO` & `composio_core-0.1.74/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.73
+Version: 0.1.74
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.73/composio/composio_cli.py` & `composio_core-0.1.74/composio/composio_cli.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.73/composio/sdk/core.py` & `composio_core-0.1.74/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.73/composio/sdk/enums.py` & `composio_core-0.1.74/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.73/composio/sdk/sdk.py` & `composio_core-0.1.74/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.73/composio/sdk/storage.py` & `composio_core-0.1.74/composio/sdk/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,8 +59,8 @@
     return 'https://backend.composio.dev/api'
 
 def get_base_account_api_key():
     base_url = get_base_url()
     if base_url == 'https://backend.composio.dev/api':
         return "yw1qb4ls4340z696zh7sa"
     else:
-        return "pbmms5jl3z1pi9mv0bbi"
+        return "i4i8nasawcsumwg30tn6g"
```

### Comparing `composio_core-0.1.73/composio/sdk/utils.py` & `composio_core-0.1.74/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.73/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.74/composio_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.73
+Version: 0.1.74
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.73/setup.py` & `composio_core-0.1.74/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.73",
+    version="0.1.74",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

