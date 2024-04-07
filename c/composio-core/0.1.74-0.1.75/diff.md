# Comparing `tmp/composio_core-0.1.74.tar.gz` & `tmp/composio_core-0.1.75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.74.tar", last modified: Sun Apr  7 05:25:19 2024, max compression
+gzip compressed data, was "composio_core-0.1.75.tar", last modified: Sun Apr  7 11:18:43 2024, max compression
```

## Comparing `composio_core-0.1.74.tar` & `composio_core-0.1.75.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.419823 composio_core-0.1.74/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.74/MANIFEST.in
--rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 05:25:19.419608 composio_core-0.1.74/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.74/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.416267 composio_core-0.1.74/composio/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.74/composio/__init__.py
--rwxr-xr-x   0 karanvaidya   (501) staff       (20)    11895 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/composio_cli.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.418320 composio_core-0.1.74/composio/sdk/
--rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.74/composio/sdk/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     5542 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/sdk/core.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     7414 2024-04-04 15:13:54.000000 composio_core-0.1.74/composio/sdk/enums.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)    16227 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/sdk/sdk.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2211 2024-04-07 05:24:38.000000 composio_core-0.1.74/composio/sdk/storage.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2861 2024-04-06 13:52:08.000000 composio_core-0.1.74/composio/sdk/utils.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 05:25:19.419389 composio_core-0.1.74/composio_core.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       91 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-07 05:25:19.000000 composio_core-0.1.74/composio_core.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      509 2024-04-06 13:53:19.000000 composio_core-0.1.74/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       92 2024-04-06 13:54:53.000000 composio_core-0.1.74/requirements.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 05:25:19.419861 composio_core-0.1.74/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)     1134 2024-04-07 05:25:03.000000 composio_core-0.1.74/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.906811 composio_core-0.1.75/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.75/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:18:43.906599 composio_core-0.1.75/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.75/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.903422 composio_core-0.1.75/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.75/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    12391 2024-04-07 11:17:37.000000 composio_core-0.1.75/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.904878 composio_core-0.1.75/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.75/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5679 2024-04-07 11:13:55.000000 composio_core-0.1.75/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.75/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-07 11:17:47.000000 composio_core-0.1.75/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2211 2024-04-07 11:12:37.000000 composio_core-0.1.75/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.75/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.906116 composio_core-0.1.75/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.75/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.75/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:18:43.906915 composio_core-0.1.75/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-07 11:18:29.000000 composio_core-0.1.75/setup.py
```

### Comparing `composio_core-0.1.74/PKG-INFO` & `composio_core-0.1.75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.74
+Version: 0.1.75
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.74/composio/composio_cli.py` & `composio_core-0.1.75/composio/composio_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,16 +164,24 @@
 def handle_update(args):
     generate_enums()
     console.print(f"\n[green]✔ Enums updated successfully![/green]\n")
 
 def add_integration(args):
     client = ComposioCore()
     auth_user(client)
-
     integration_name = args.integration_name
+
+    existing_connection = get_user_connection(integration_name)
+    if existing_connection is not None:
+        console.print(f"[yellow]Warning: An existing connection for {integration_name} was found.[/yellow]\n")
+        replace_connection = input("> Do you want to replace the existing connection? (yes/no): ").lower()
+        if replace_connection not in ['yes', 'y']:
+            console.print("\n[green]Existing connection retained. No new connection added.[/green]\n")
+            return
+
     console.print(f"\n[green]> Adding integration: {integration_name.capitalize()}...[/green]\n")
     try:
         # @TODO: add logic to wait and ask for API_KEY
         connection = client.initiate_connection("test-" + integration_name.lower() + "-connector")
         webbrowser.open(connection.redirectUrl)
         print(f"Please authenticate {integration_name} in the browser and come back here. URL: {connection.redirectUrl}")
         spinner = Spinner(DOTS, f"[yellow]⚠[/yellow] Waiting for {integration_name} authentication...")
```

### Comparing `composio_core-0.1.74/composio/sdk/core.py` & `composio_core-0.1.75/composio/sdk/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,15 +113,19 @@
             raise Exception(f"Failed to enable trigger: {e}")
     
     def enable_trigger(self, trigger_id: str, connected_account_id: str, user_inputs: dict):
         try:
             return self.sdk.enable_trigger(trigger_id, connected_account_id, user_inputs)
         except Exception as e:
             raise Exception(e)
-    
+
+    def get_saved_connections(self, app_name: str = None):
+        connectionId = get_user_connection(app_name)
+        return connectionId
+
     def execute_action(self, action: Action, params: dict):
         tool_name  = action.value[0]
         connectionId = get_user_connection(tool_name)
         if not connectionId:
             raise Exception(f"User not authenticated or connection not found. Please authenticate using: composio-cli add {tool_name}")
 
         account = self.sdk.get_connected_account(connectionId)
```

### Comparing `composio_core-0.1.74/composio/sdk/enums.py` & `composio_core-0.1.75/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.74/composio/sdk/sdk.py` & `composio_core-0.1.75/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.74/composio/sdk/storage.py` & `composio_core-0.1.75/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.74/composio/sdk/utils.py` & `composio_core-0.1.75/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.74/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.75/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.74
+Version: 0.1.75
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.74/setup.py` & `composio_core-0.1.75/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.74",
+    version="0.1.75",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

