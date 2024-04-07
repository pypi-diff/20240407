# Comparing `tmp/composio_core-0.1.75.tar.gz` & `tmp/composio_core-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_core-0.1.75.tar", last modified: Sun Apr  7 11:18:43 2024, max compression
+gzip compressed data, was "composio_core-0.1.76.tar", last modified: Sun Apr  7 11:41:07 2024, max compression
```

## Comparing `composio_core-0.1.75.tar` & `composio_core-0.1.76.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.906811 composio_core-0.1.75/
--rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.75/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:18:43.906599 composio_core-0.1.75/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.75/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.903422 composio_core-0.1.75/composio/
--rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.75/composio/__init__.py
--rwxr-xr-x   0 utkarsh    (501) staff       (20)    12391 2024-04-07 11:17:37.000000 composio_core-0.1.75/composio/composio_cli.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.904878 composio_core-0.1.75/composio/sdk/
--rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.75/composio/sdk/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5679 2024-04-07 11:13:55.000000 composio_core-0.1.75/composio/sdk/core.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     7414 2024-04-04 17:45:19.000000 composio_core-0.1.75/composio/sdk/enums.py
--rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-07 11:17:47.000000 composio_core-0.1.75/composio/sdk/sdk.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2211 2024-04-07 11:12:37.000000 composio_core-0.1.75/composio/sdk/storage.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.75/composio/sdk/utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:18:43.906116 composio_core-0.1.75/composio_core.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/entry_points.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-07 11:18:43.000000 composio_core-0.1.75/composio_core.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.75/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.75/requirements.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:18:43.906915 composio_core-0.1.75/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-07 11:18:29.000000 composio_core-0.1.75/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.973451 composio_core-0.1.76/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       48 2024-03-15 13:37:31.000000 composio_core-0.1.76/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:41:07.973214 composio_core-0.1.76/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      102 2024-03-16 10:06:01.000000 composio_core-0.1.76/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.970023 composio_core-0.1.76/composio/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      176 2024-03-27 14:52:24.000000 composio_core-0.1.76/composio/__init__.py
+-rwxr-xr-x   0 utkarsh    (501) staff       (20)    12441 2024-04-07 11:39:39.000000 composio_core-0.1.76/composio/composio_cli.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.972042 composio_core-0.1.76/composio/sdk/
+-rw-r--r--   0 utkarsh    (501) staff       (20)       85 2024-03-27 14:52:24.000000 composio_core-0.1.76/composio/sdk/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5679 2024-04-07 11:13:55.000000 composio_core-0.1.76/composio/sdk/core.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     6973 2024-04-07 11:39:25.000000 composio_core-0.1.76/composio/sdk/enums.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)    16227 2024-04-07 11:17:47.000000 composio_core-0.1.76/composio/sdk/sdk.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-04-07 11:38:27.000000 composio_core-0.1.76/composio/sdk/storage.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2861 2024-04-06 12:48:50.000000 composio_core-0.1.76/composio/sdk/utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-07 11:41:07.972943 composio_core-0.1.76/composio_core.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      770 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      466 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       60 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/entry_points.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       91 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        9 2024-04-07 11:41:07.000000 composio_core-0.1.76/composio_core.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      509 2024-04-06 14:07:21.000000 composio_core-0.1.76/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       92 2024-04-06 14:07:21.000000 composio_core-0.1.76/requirements.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-07 11:41:07.973499 composio_core-0.1.76/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)     1134 2024-04-07 11:40:51.000000 composio_core-0.1.76/setup.py
```

### Comparing `composio_core-0.1.75/PKG-INFO` & `composio_core-0.1.76/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.75
+Version: 0.1.76
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.75/composio/composio_cli.py` & `composio_core-0.1.76/composio/composio_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,16 @@
         client.set_global_trigger(args.callback_url)
         console.print(f"\n[green]✔ Global trigger callback set successfully![/green]\n")
     except Exception as e:
         console.print(f"[red] Error occurred during setting global trigger callback: {e}[/red]")
         sys.exit(1)
 
 def handle_update(args):
+    client = ComposioCore()
+    auth_user(client)
     generate_enums()
     console.print(f"\n[green]✔ Enums updated successfully![/green]\n")
 
 def add_integration(args):
     client = ComposioCore()
     auth_user(client)
     integration_name = args.integration_name
```

### Comparing `composio_core-0.1.75/composio/sdk/core.py` & `composio_core-0.1.76/composio/sdk/core.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.75/composio/sdk/enums.py` & `composio_core-0.1.76/composio/sdk/enums.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,14 @@
     FRESHDESK = "freshdesk"
     HUBSPOT = "hubspot"
     EVENTBRITE = "eventbrite"
     GITLAB = "gitlab"
     SHOPIFY = "shopify"
     MIRO = "miro"
     SPLITWISE = "splitwise"
-    APIFY = "apify"
 
 class TestIntegration(Enum):
     CLICKUP = "test-clickup-connector"
     GOOGLE_DRIVE = "test-google-drive-connector"
     GOOGLE_SHEETS = "test-google-sheets-connector"
     CALENDLY = "test-calendly-connector"
     ZENDESK = "test-zendesk-connector"
@@ -92,15 +91,14 @@
     FRESHDESK = "test-freshdesk-connector"
     HUBSPOT = "test-hubspot-connector"
     EVENTBRITE = "test-eventbrite-connector"
     GITLAB = "test-gitlab-connector"
     SHOPIFY = "test-shopify-connector"
     MIRO = "test-miro-connector"
     SPLITWISE = "test-splitwise-connector"
-    APIFY = "test-apify-connector"
 
 class Action(Enum):
     def __init__(self, service, action):
         self.service = service
         self.action = action
 
     CLICKUP_CREATE_TASK = ("clickup", "clickup_create_task")
@@ -148,20 +146,14 @@
     NOTION_ARCHIVE_NOTION_PAGE = ("notion", "notion_archive_notion_page")
     NOTION_FETCH_NOTION_DATABASE = ("notion", "notion_fetch_notion_database")
     NOTION_UPDATE_NOTION_DATABASE = ("notion", "notion_update_notion_database")
     NOTION_CREATE_PAGE_COMMENT = ("notion", "notion_create_page_comment")
     NOTION_GET_ABOUT_ME = ("notion", "notion_get_about_me")
     DROPBOX_GET_ABOUT_ME = ("dropbox", "dropbox_get_about_me")
     TYPEFORM_GET_ABOUT_ME = ("typeform", "typeform_get_about_me")
-    APIFY_GET_APIFY_ACTORS = ("apify", "apify_list_apify_actors")
-    APIFY_CREATE_APIFY_ACTOR = ("apify", "apify_create_apify_actor")
-    APIFY_GET_ACTOR_ID = ("apify", "apify_get_actor_id")
-    APIFY_SEARCH_APIFY_STORE = ("apify", "apify_search_store")
-    APIFY_GET_LAST_RUN_DATA = ("apify", "apify_get_last_run_data")
-    APIFY_GET_APIFY_TASKS = ("apify", "apify_list_apify_tasks")
 
 class Trigger(Enum):
     def __init__(self, service, trigger):
         self.service = service
         self.trigger = trigger
 
     GITHUB_PULL_REQUEST_EVENT = ("github", "github_pull_request_event")
```

### Comparing `composio_core-0.1.75/composio/sdk/sdk.py` & `composio_core-0.1.76/composio/sdk/sdk.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.75/composio/sdk/storage.py` & `composio_core-0.1.76/composio/sdk/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -55,12 +55,9 @@
 def get_base_url():
     user_data = load_user_data()
     if 'base_url' in user_data:
         return user_data['base_url']
     return 'https://backend.composio.dev/api'
 
 def get_base_account_api_key():
-    base_url = get_base_url()
-    if base_url == 'https://backend.composio.dev/api':
-        return "yw1qb4ls4340z696zh7sa"
-    else:
-        return "i4i8nasawcsumwg30tn6g"
+    user_data = load_user_data()
+    return user_data.get('api_key')
```

### Comparing `composio_core-0.1.75/composio/sdk/utils.py` & `composio_core-0.1.76/composio/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `composio_core-0.1.75/composio_core.egg-info/PKG-INFO` & `composio_core-0.1.76/composio_core.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_core
-Version: 0.1.75
+Version: 0.1.76
 Summary: Core package to act as a bridge between composio platform and other services.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Utkarsh
 Author-email: utkarsh@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `composio_core-0.1.75/setup.py` & `composio_core-0.1.76/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     def run(self):
         install.run(self)
 
 
 setup(
     name="composio_core",
-    version="0.1.75",
+    version="0.1.76",
     author="Utkarsh",
     author_email="utkarsh@composio.dev",
     description="Core package to act as a bridge between composio platform and other services.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

