# Comparing `tmp/dialog-workflow-local-0.0.87.tar.gz` & `tmp/dialog-workflow-local-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.87.tar", last modified: Thu Apr  4 22:19:32 2024, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.88.tar", last modified: Sun Apr  7 03:24:25 2024, max compression
```

## Comparing `dialog-workflow-local-0.0.87.tar` & `dialog-workflow-local-0.0.88.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:19:32.516029 dialog-workflow-local-0.0.87/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 22:19:32.516029 dialog-workflow-local-0.0.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:19:32.512029 dialog-workflow-local-0.0.87/dialog_workflow_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:19:32.516029 dialog-workflow-local-0.0.87/dialog_workflow_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/dialog_workflow_local/src/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4093 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/dialog_workflow_local/src/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/dialog_workflow_local/src/ProfileContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/dialog_workflow_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/dialog_workflow_local/src/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/dialog_workflow_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:19:32.516029 dialog-workflow-local-0.0.87/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 22:19:32.000000 dialog-workflow-local-0.0.87/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-04 22:19:32.000000 dialog-workflow-local-0.0.87/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:19:32.000000 dialog-workflow-local-0.0.87/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-04 22:19:32.000000 dialog-workflow-local-0.0.87/dialog_workflow_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-04 22:19:32.000000 dialog-workflow-local-0.0.87/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 22:19:32.516029 dialog-workflow-local-0.0.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-04 22:18:59.000000 dialog-workflow-local-0.0.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:24:25.742105 dialog-workflow-local-0.0.88/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 03:24:25.742105 dialog-workflow-local-0.0.88/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:24:25.738105 dialog-workflow-local-0.0.88/dialog_workflow_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:24:25.742105 dialog-workflow-local-0.0.88/dialog_workflow_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/dialog_workflow_local/src/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/dialog_workflow_local/src/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/dialog_workflow_local/src/ProfileContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/dialog_workflow_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/dialog_workflow_local/src/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/dialog_workflow_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:24:25.742105 dialog-workflow-local-0.0.88/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 03:24:25.000000 dialog-workflow-local-0.0.88/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-07 03:24:25.000000 dialog-workflow-local-0.0.88/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:24:25.000000 dialog-workflow-local-0.0.88/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 03:24:25.000000 dialog-workflow-local-0.0.88/dialog_workflow_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 03:24:25.000000 dialog-workflow-local-0.0.88/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:24:25.742105 dialog-workflow-local-0.0.88/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 03:23:54.000000 dialog-workflow-local-0.0.88/setup.py
```

### Comparing `dialog-workflow-local-0.0.87/PKG-INFO` & `dialog-workflow-local-0.0.88/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.87
+Version: 0.0.88
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.87/README.md` & `dialog-workflow-local-0.0.88/README.md`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.87/dialog_workflow_local/src/Constants.py` & `dialog-workflow-local-0.0.88/dialog_workflow_local/src/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.87/dialog_workflow_local/src/DialogWorkflow.py` & `dialog-workflow-local-0.0.88/dialog_workflow_local/src/DialogWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 import random
 
 from database_mysql_local.connector import Connector
 from logger_local.LoggerLocal import Logger
 from message_local.CompoundMessage import CompoundMessage
 from user_context_remote.user_context import UserContext
 from variable_local.variable import VariablesLocal
+from language_remote.lang_code import LangCode
 
 from .Constants import DIALOG_WORKFLOW_CODE_LOGGER_OBJECT
 from .ProfileContext import DialogWorkflowRecord
 from .action import Action
 from .utils import get_curr_state, update_profile_curr_state_in_db
 
 user = UserContext()
 logger = Logger.create_logger(object=DIALOG_WORKFLOW_CODE_LOGGER_OBJECT)
 
 
 # Get all potential records in a specific state and choose randomly one of them
 # TODO Please use MessagesLocal to store the message(s) recieved and anwers
 # TODO Please use the function defined in avatar similar to get_dialog_workflow_avatar_profile_id( profile_id1, prompt, group_id, profile_id2...) using avatar_table and avtar_group_table
-def get_dialog_workflow_record(profile_curr_state: int, language: str):
+def get_dialog_workflow_record(profile_curr_state: int, language: LangCode):
     logger.start(
         object={'profile_curr_state': profile_curr_state, 'language': language})
     # TODO Change * to the fields required
     connection = Connector.connect('dialog_workflow')
     cursor = connection.cursor(dictionary=True, buffered=True)
     cursor.execute("""SELECT * FROM dialog_workflow_state_view WHERE state_id = %s AND lang_code = %s""",
-                   (profile_curr_state, language))
+                   (profile_curr_state, language.value))
     optional_records = cursor.fetchall()
     if not optional_records:
         error_message = f"No records found for state_id: {profile_curr_state} and language: {language}"
         logger.error(error_message)
         logger.end()
         raise Exception(error_message)
     random_index = random.randint(0, len(optional_records) - 1)
@@ -46,15 +47,15 @@
         2. incoming_message: the message he sent"""
     # TODO: remove profile_id an use user context
     logger.start(object={'profile_id': profile_id,
                          'incoming_message': incoming_message})
     # TODO Save the message using MessagesLocal (from DIALOG_WORKFLOW_PROFILE_ID, to UserContext.getEffectiveProfileId, ...)
     variables = VariablesLocal()
     profile_curr_state = get_curr_state(profile_id)
-    language = user.get_effective_profile_prefered_language()
+    language = user.get_effective_profile_preferred_lang_code()
     got_response = incoming_message.strip() != ""  # This variable indicates if we must act now as we got a response from the user or as if we should send one to him
     init_action = Action(incoming_message, profile_id,
                          language, profile_curr_state, variables)
     while True:
         dialog_workflow_record = get_dialog_workflow_record(
             init_action.profile_curr_state, language)
         is_state_changed, outgoing_message = init_action.act(
```

### Comparing `dialog-workflow-local-0.0.87/dialog_workflow_local/src/ProfileContext.py` & `dialog-workflow-local-0.0.88/dialog_workflow_local/src/ProfileContext.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.87/dialog_workflow_local/src/action.py` & `dialog-workflow-local-0.0.88/dialog_workflow_local/src/action.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.87/dialog_workflow_local/src/utils.py` & `dialog-workflow-local-0.0.88/dialog_workflow_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.87/dialog_workflow_local.egg-info/PKG-INFO` & `dialog-workflow-local-0.0.88/dialog_workflow_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.87
+Version: 0.0.88
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.87/setup.py` & `dialog-workflow-local-0.0.88/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "dialog-workflow-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.87',  # https://pypi.org/project/dialog-workflow-local/
+    version='0.0.88',  # https://pypi.org/project/dialog-workflow-local/
     author="Circles",
     author_email="info@circle.life",
     description="PyPI Package for dialog workflow",
     long_description="This is a package for running the dialog workflow",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

