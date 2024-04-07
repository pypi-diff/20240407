# Comparing `tmp/composio_core-0.1.78.tar.gz` & `tmp/composio_core-0.1.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.78.tar", last modified: Sun Apr  7 15:00:12 2024, max compression
+gzip compressed data, was "composio_core-0.1.79.tar", last modified: Sun Apr  7 15:53:51 2024, max compression
```

## Comparing `composio_core-0.1.78.tar` & `composio_core-0.1.79.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 15:00:12.862949 composio_core-0.1.78/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.78/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 15:00:12.862745 composio_core-0.1.78/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.78/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 15:00:12.859329 composio_core-0.1.78/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.78/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    12441 2024-04-07 14:58:07.000000 composio_core-0.1.78/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 15:00:12.861152 composio_core-0.1.78/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.78/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5757 2024-04-07 14:58:17.000000 composio_core-0.1.78/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     6973 2024-04-07 11:39:25.000000 composio_core-0.1.78/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16337 2024-04-07 14:47:23.000000 composio_core-0.1.78/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-04-07 11:38:27.000000 composio_core-0.1.78/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.78/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 15:00:12.862502 composio_core-0.1.78/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 15:00:12.000000 composio_core-0.1.78/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-07 15:00:12.000000 composio_core-0.1.78/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 15:00:12.000000 composio_core-0.1.78/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-07 15:00:12.000000 composio_core-0.1.78/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-07 15:00:12.000000 composio_core-0.1.78/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-07 15:00:12.000000 composio_core-0.1.78/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.78/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.78/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 15:00:12.862991 composio_core-0.1.78/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-07 15:00:04.000000 composio_core-0.1.78/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 15:53:51.120872 composio_core-0.1.79/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       48 2024-04-02 18:29:17.000000 composio_core-0.1.79/MANIFEST.in
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 15:53:51.120675 composio_core-0.1.79/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      102 2024-04-02 18:29:17.000000 composio_core-0.1.79/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 15:53:51.116898 composio_core-0.1.79/composio/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      176 2024-04-02 18:29:17.000000 composio_core-0.1.79/composio/__init__.py
+-rwxr-xr-x   0 karanvaidya   (501) staff       (20)    12557 2024-04-07 15:53:03.000000 composio_core-0.1.79/composio/composio_cli.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 15:53:51.119179 composio_core-0.1.79/composio/sdk/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       85 2024-04-02 18:29:17.000000 composio_core-0.1.79/composio/sdk/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     5757 2024-04-07 15:47:29.000000 composio_core-0.1.79/composio/sdk/core.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     6973 2024-04-07 15:47:29.000000 composio_core-0.1.79/composio/sdk/enums.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)    16561 2024-04-07 15:47:39.000000 composio_core-0.1.79/composio/sdk/sdk.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2107 2024-04-07 15:47:29.000000 composio_core-0.1.79/composio/sdk/storage.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2861 2024-04-06 13:52:08.000000 composio_core-0.1.79/composio/sdk/utils.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-07 15:53:51.120442 composio_core-0.1.79/composio_core.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      770 2024-04-07 15:53:51.000000 composio_core-0.1.79/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      466 2024-04-07 15:53:51.000000 composio_core-0.1.79/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-07 15:53:51.000000 composio_core-0.1.79/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       60 2024-04-07 15:53:51.000000 composio_core-0.1.79/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       91 2024-04-07 15:53:51.000000 composio_core-0.1.79/composio_core.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        9 2024-04-07 15:53:51.000000 composio_core-0.1.79/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      509 2024-04-06 13:53:19.000000 composio_core-0.1.79/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       92 2024-04-06 13:54:53.000000 composio_core-0.1.79/requirements.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-07 15:53:51.120915 composio_core-0.1.79/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     1134 2024-04-07 15:53:40.000000 composio_core-0.1.79/setup.py
```

### Comparing `composio_core-0.1.78/PKG-INFO` & `composio_core-0.1.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.78
+Version: 0.1.79
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.78/composio/composio_cli.py` & `composio_core-0.1.79/composio/composio_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,18 @@
         user_connection = get_user_connection(app_key)
         if not user_connection:
             console.print(f"[red]No connection found for {app_key}.\nUse the following command to add a connection: [green]composio-cli add {app_key}[/green][/red]")
             sys.exit(1)
         
         connected_account_id = get_user_connection(app_key)
         # Assuming there's a function to enable the trigger with user inputs
-        client.enable_trigger(trigger_name, connected_account_id, user_inputs)
+        resp = client.enable_trigger(trigger_name, connected_account_id, user_inputs)
         console.print(f"\n[green]✔ Trigger enabled successfully![/green]\n")
+        if 'triggerId' in resp:
+            console.print(f"[green]Trigger ID: {resp['triggerId']}[/green]")
     except Exception as e:
         console.print(f"[red] Error occurred during enabling trigger: {e}[/red]")
         sys.exit(1)
 
 def set_global_trigger_callback(args): 
     client = ComposioCore()
     auth_user(client)
```

### Comparing `composio_core-0.1.78/composio/sdk/core.py` & `composio_core-0.1.79/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.78/composio/sdk/enums.py` & `composio_core-0.1.79/composio/sdk/enums.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.78/composio/sdk/sdk.py` & `composio_core-0.1.79/composio/sdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,16 +110,16 @@
                             "parameters": action.get("parameters", {}),
                         },
                     }
                     for action in actions["items"]
                 ]
             else:
                 return actions["items"]
-
-        raise Exception("Failed to get actions")
+            
+        raise Exception("Failed to get actions. You might want to run composio-cli update and restart the python notebook to reload the updated library.")
 
     def handle_tools_calls(self, tool_calls: ChatCompletion) -> list[any]:
         output = []
         try:
             if tool_calls.choices:
                 for choice in tool_calls.choices:
                     if choice.message.tool_calls:
@@ -244,15 +244,15 @@
                 for item in actions_response["items"]:
                     if item["name"] in action_names_list:
                         filtered_actions.append(item)
                 return filtered_actions
             else:
                 return actions_response["items"]
 
-        raise Exception("Failed to get actions")
+        raise Exception("Failed to get actions. You might want to run composio-cli update and restart the python notebook to reload the updated library.")
     
     def get_list_of_triggers(
         self, apps: list[App] = None
     ) -> list:
         if apps is None or len(apps) == 0:
             resp = self.http_client.get(f"{self.base_url}/v1/triggers")
         else:
```

### Comparing `composio_core-0.1.78/composio/sdk/storage.py` & `composio_core-0.1.79/composio/sdk/storage.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.78/composio/sdk/utils.py` & `composio_core-0.1.79/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.78/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.79/composio_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.78
+Version: 0.1.79
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.78/setup.py` & `composio_core-0.1.79/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.78",
+    version="0.1.79",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

