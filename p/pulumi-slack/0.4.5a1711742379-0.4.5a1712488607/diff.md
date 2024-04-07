# Comparing `tmp/pulumi_slack-0.4.5a1711742379.tar.gz` & `tmp/pulumi_slack-0.4.5a1712488607.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_slack-0.4.5a1711742379.tar", last modified: Fri Mar 29 20:20:43 2024, max compression
+gzip compressed data, was "pulumi_slack-0.4.5a1712488607.tar", last modified: Sun Apr  7 11:20:34 2024, max compression
```

## Comparing `pulumi_slack-0.4.5a1711742379.tar` & `pulumi_slack-0.4.5a1712488607.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:20:43.287680 pulumi_slack-0.4.5a1711742379/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-29 20:20:43.287680 pulumi_slack-0.4.5a1711742379/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:20:43.287680 pulumi_slack-0.4.5a1711742379/pulumi_slack/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:20:43.287680 pulumi_slack-0.4.5a1711742379/pulumi_slack/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    39532 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/get_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/get_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18298 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack/usergroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 20:20:43.287680 pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-29 20:20:43.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-29 20:20:43.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 20:20:43.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-29 20:20:43.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-29 20:20:43.000000 pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-29 20:20:35.000000 pulumi_slack-0.4.5a1711742379/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 20:20:43.287680 pulumi_slack-0.4.5a1711742379/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:20:34.266485 pulumi_slack-0.4.5a1712488607/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-07 11:20:34.266485 pulumi_slack-0.4.5a1712488607/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:20:34.266485 pulumi_slack-0.4.5a1712488607/pulumi_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:20:34.266485 pulumi_slack-0.4.5a1712488607/pulumi_slack/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39532 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/get_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/get_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18298 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack/usergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:20:34.266485 pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-07 11:20:34.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-07 11:20:34.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:20:34.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 11:20:34.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-07 11:20:34.000000 pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-07 11:20:23.000000 pulumi_slack-0.4.5a1712488607/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:20:34.266485 pulumi_slack-0.4.5a1712488607/setup.cfg
```

### Comparing `pulumi_slack-0.4.5a1711742379/PKG-INFO` & `pulumi_slack-0.4.5a1712488607/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.5a1711742379
+Version: 0.4.5a1712488607
 Summary: A Pulumi package for managing Slack workspaces.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi,slack,category/utility
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_slack-0.4.5a1711742379/README.md` & `pulumi_slack-0.4.5a1712488607/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/__init__.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/_utilities.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/config/vars.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/conversation.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/get_conversation.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/get_conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/get_user.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/get_usergroup.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/get_usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/provider.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack/usergroup.py` & `pulumi_slack-0.4.5a1712488607/pulumi_slack/usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/PKG-INFO` & `pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.5a1711742379
+Version: 0.4.5a1712488607
 Summary: A Pulumi package for managing Slack workspaces.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi,slack,category/utility
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_slack-0.4.5a1711742379/pulumi_slack.egg-info/SOURCES.txt` & `pulumi_slack-0.4.5a1712488607/pulumi_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1711742379/pyproject.toml` & `pulumi_slack-0.4.5a1712488607/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_slack"
   description = "A Pulumi package for managing Slack workspaces."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "slack", "category/utility"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.4.5a1711742379"
+  version = "0.4.5a1712488607"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-slack"
 
 [build-system]
```

