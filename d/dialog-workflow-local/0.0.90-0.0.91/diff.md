# Comparing `tmp/dialog-workflow-local-0.0.90.tar.gz` & `tmp/dialog-workflow-local-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialog-workflow-local-0.0.90.tar", last modified: Sun Apr  7 03:57:45 2024, max compression
+gzip compressed data, was "dialog-workflow-local-0.0.91.tar", last modified: Sun Apr  7 04:15:30 2024, max compression
```

## Comparing `dialog-workflow-local-0.0.90.tar` & `dialog-workflow-local-0.0.91.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:57:45.530778 dialog-workflow-local-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 03:57:45.530778 dialog-workflow-local-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:57:45.526778 dialog-workflow-local-0.0.90/dialog_workflow_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:57:45.530778 dialog-workflow-local-0.0.90/dialog_workflow_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/dialog_workflow_local/src/Constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/dialog_workflow_local/src/DialogWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/dialog_workflow_local/src/ProfileContext.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/dialog_workflow_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/dialog_workflow_local/src/action.py
--rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/dialog_workflow_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:57:45.530778 dialog-workflow-local-0.0.90/dialog_workflow_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 03:57:45.000000 dialog-workflow-local-0.0.90/dialog_workflow_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-07 03:57:45.000000 dialog-workflow-local-0.0.90/dialog_workflow_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:57:45.000000 dialog-workflow-local-0.0.90/dialog_workflow_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 03:57:45.000000 dialog-workflow-local-0.0.90/dialog_workflow_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 03:57:45.000000 dialog-workflow-local-0.0.90/dialog_workflow_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:57:45.530778 dialog-workflow-local-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 03:57:18.000000 dialog-workflow-local-0.0.90/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:15:30.655169 dialog-workflow-local-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 04:15:30.655169 dialog-workflow-local-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:15:30.651169 dialog-workflow-local-0.0.91/dialog_workflow_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:15:30.655169 dialog-workflow-local-0.0.91/dialog_workflow_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/dialog_workflow_local/src/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/dialog_workflow_local/src/DialogWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/dialog_workflow_local/src/ProfileContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/dialog_workflow_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29234 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/dialog_workflow_local/src/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10318 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/dialog_workflow_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:15:30.655169 dialog-workflow-local-0.0.91/dialog_workflow_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-07 04:15:30.000000 dialog-workflow-local-0.0.91/dialog_workflow_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-07 04:15:30.000000 dialog-workflow-local-0.0.91/dialog_workflow_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:15:30.000000 dialog-workflow-local-0.0.91/dialog_workflow_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 04:15:30.000000 dialog-workflow-local-0.0.91/dialog_workflow_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 04:15:30.000000 dialog-workflow-local-0.0.91/dialog_workflow_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 04:15:30.655169 dialog-workflow-local-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 04:14:56.000000 dialog-workflow-local-0.0.91/setup.py
```

### Comparing `dialog-workflow-local-0.0.90/PKG-INFO` & `dialog-workflow-local-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.90
+Version: 0.0.91
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.90/README.md` & `dialog-workflow-local-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.90/dialog_workflow_local/src/Constants.py` & `dialog-workflow-local-0.0.91/dialog_workflow_local/src/Constants.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.90/dialog_workflow_local/src/DialogWorkflow.py` & `dialog-workflow-local-0.0.91/dialog_workflow_local/src/DialogWorkflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,14 +47,15 @@
         2. incoming_message: the message he sent"""
     # TODO: remove profile_id an use user context
     logger.start(object={'profile_id': profile_id,
                          'incoming_message': incoming_message})
     # TODO Save the message using MessagesLocal (from DIALOG_WORKFLOW_PROFILE_ID, to UserContext.getEffectiveProfileId, ...)
     variables = VariablesLocal()
     profile_curr_state = get_curr_state(profile_id)
+    # TODO lang_code =
     language = user.get_effective_profile_preferred_lang_code()
     got_response = incoming_message.strip() != ""  # This variable indicates if we must act now as we got a response from the user or as if we should send one to him
     init_action = Action(incoming_message, profile_id,
                          language, profile_curr_state, variables)
     while True:
         dialog_workflow_record = get_dialog_workflow_record(
             init_action.profile_curr_state, language)
```

### Comparing `dialog-workflow-local-0.0.90/dialog_workflow_local/src/ProfileContext.py` & `dialog-workflow-local-0.0.91/dialog_workflow_local/src/ProfileContext.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.90/dialog_workflow_local/src/action.py` & `dialog-workflow-local-0.0.91/dialog_workflow_local/src/action.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.90/dialog_workflow_local/src/utils.py` & `dialog-workflow-local-0.0.91/dialog_workflow_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `dialog-workflow-local-0.0.90/dialog_workflow_local.egg-info/PKG-INFO` & `dialog-workflow-local-0.0.91/dialog_workflow_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialog-workflow-local
-Version: 0.0.90
+Version: 0.0.91
 Summary: PyPI Package for dialog workflow
 Home-page: https://github.com/circles-zone/dialog-workflow-local-python-package
 Author: Circles
 Author-email: info@circle.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `dialog-workflow-local-0.0.90/setup.py` & `dialog-workflow-local-0.0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "dialog-workflow-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.90',  # https://pypi.org/project/dialog-workflow-local/
+    version='0.0.91',  # https://pypi.org/project/dialog-workflow-local/
     author="Circles",
     author_email="info@circle.life",
     description="PyPI Package for dialog workflow",
     long_description="This is a package for running the dialog workflow",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

