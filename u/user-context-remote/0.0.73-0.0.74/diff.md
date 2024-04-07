# Comparing `tmp/user-context-remote-0.0.73.tar.gz` & `tmp/user-context-remote-0.0.74.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-context-remote-0.0.73.tar", last modified: Thu Apr  4 23:17:13 2024, max compression
+gzip compressed data, was "user-context-remote-0.0.74.tar", last modified: Sun Apr  7 14:52:54 2024, max compression
```

## Comparing `user-context-remote-0.0.73.tar` & `user-context-remote-0.0.74.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:17:13.646877 user-context-remote-0.0.73/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 23:17:13.646877 user-context-remote-0.0.73/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-04 23:17:01.000000 user-context-remote-0.0.73/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-04 23:17:01.000000 user-context-remote-0.0.73/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 23:17:13.646877 user-context-remote-0.0.73/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-04 23:17:01.000000 user-context-remote-0.0.73/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:17:13.646877 user-context-remote-0.0.73/user_context_remote/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:17:13.646877 user-context-remote-0.0.73/user_context_remote/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 23:17:01.000000 user-context-remote-0.0.73/user_context_remote/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-04 23:17:01.000000 user-context-remote-0.0.73/user_context_remote/src/user_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 23:17:13.646877 user-context-remote-0.0.73/user_context_remote.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-04 23:17:13.000000 user-context-remote-0.0.73/user_context_remote.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-04 23:17:13.000000 user-context-remote-0.0.73/user_context_remote.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 23:17:13.000000 user-context-remote-0.0.73/user_context_remote.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-04 23:17:13.000000 user-context-remote-0.0.73/user_context_remote.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-04 23:17:13.000000 user-context-remote-0.0.73/user_context_remote.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:52:54.845940 user-context-remote-0.0.74/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-07 14:52:54.845940 user-context-remote-0.0.74/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-07 14:52:39.000000 user-context-remote-0.0.74/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 14:52:39.000000 user-context-remote-0.0.74/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:52:54.845940 user-context-remote-0.0.74/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-07 14:52:39.000000 user-context-remote-0.0.74/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:52:54.841940 user-context-remote-0.0.74/user_context_remote/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:52:54.845940 user-context-remote-0.0.74/user_context_remote/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:52:39.000000 user-context-remote-0.0.74/user_context_remote/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18994 2024-04-07 14:52:39.000000 user-context-remote-0.0.74/user_context_remote/src/user_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:52:54.845940 user-context-remote-0.0.74/user_context_remote.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-07 14:52:54.000000 user-context-remote-0.0.74/user_context_remote.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-07 14:52:54.000000 user-context-remote-0.0.74/user_context_remote.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:52:54.000000 user-context-remote-0.0.74/user_context_remote.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-07 14:52:54.000000 user-context-remote-0.0.74/user_context_remote.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 14:52:54.000000 user-context-remote-0.0.74/user_context_remote.egg-info/top_level.txt
```

### Comparing `user-context-remote-0.0.73/PKG-INFO` & `user-context-remote-0.0.74/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.73
+Version: 0.0.74
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `user-context-remote-0.0.73/README.md` & `user-context-remote-0.0.74/README.md`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.73/pyproject.toml` & `user-context-remote-0.0.74/pyproject.toml`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.73/setup.py` & `user-context-remote-0.0.74/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "user-context-remote"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name='user-context-remote',
-    version='0.0.73',  # https://pypi.org/project/user-context-remote/
+    version='0.0.74',  # https://pypi.org/project/user-context-remote/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles User Context Local/Remote Python",
     long_description="This is a package for sharing common user-context-remote functions used in different repositories",
     long_description_content_type="text/markdown",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `user-context-remote-0.0.73/user_context_remote/src/user_context.py` & `user-context-remote-0.0.74/user_context_remote/src/user_context.py`

 * *Files identical despite different names*

### Comparing `user-context-remote-0.0.73/user_context_remote.egg-info/PKG-INFO` & `user-context-remote-0.0.74/user_context_remote.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: user-context-remote
-Version: 0.0.73
+Version: 0.0.74
 Summary: PyPI Package for Circles User Context Local/Remote Python
 Home-page: https://github.com/circles-zone/user-context-remote-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

