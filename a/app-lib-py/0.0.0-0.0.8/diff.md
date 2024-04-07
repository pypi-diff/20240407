# Comparing `tmp/app_lib_py-0.0.0.tar.gz` & `tmp/app_lib_py-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_lib_py-0.0.0.tar", last modified: Sun Apr  7 14:27:47 2024, max compression
+gzip compressed data, was "app_lib_py-0.0.8.tar", last modified: Sun Apr  7 16:32:33 2024, max compression
```

## Comparing `app_lib_py-0.0.0.tar` & `app_lib_py-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:47.485337 app_lib_py-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-07 14:27:47.485337 app_lib_py-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 14:27:41.000000 app_lib_py-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-07 14:27:47.485337 app_lib_py-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:47.485337 app_lib_py-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:47.485337 app_lib_py-0.0.0/src/app_lib_py/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 14:27:41.000000 app_lib_py-0.0.0/src/app_lib_py/ClassCurves.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:41.000000 app_lib_py-0.0.0/src/app_lib_py/ModulePredict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:41.000000 app_lib_py-0.0.0/src/app_lib_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:27:47.485337 app_lib_py-0.0.0/src/app_lib_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-04-07 14:27:47.000000 app_lib_py-0.0.0/src/app_lib_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-07 14:27:47.000000 app_lib_py-0.0.0/src/app_lib_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:27:47.000000 app_lib_py-0.0.0/src/app_lib_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 14:27:47.000000 app_lib_py-0.0.0/src/app_lib_py.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      548 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       41 2024-04-07 15:19:09.000000 app_lib_py-0.0.8/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      117 2024-04-07 15:24:38.000000 app_lib_py-0.0.8/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       39 2024-04-06 21:59:37.000000 app_lib_py-0.0.8/requirements.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      654 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/src/app_lib_py/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     1150 2024-04-06 22:49:59.000000 app_lib_py-0.0.8/src/app_lib_py/ClassCurves.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2024-04-06 22:06:58.000000 app_lib_py-0.0.8/src/app_lib_py/ModulePredict.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2024-04-06 20:23:30.000000 app_lib_py-0.0.8/src/app_lib_py/__init__.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/src/app_lib_py.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      548 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      347 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       11 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/tests/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/tests/speed/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       35 2024-04-06 21:59:58.000000 app_lib_py-0.0.8/tests/speed/speed_log.csv
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/tests/utility/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     1506 2024-04-07 10:53:27.000000 app_lib_py-0.0.8/tests/utility/test_curves.py
```

### Comparing `app_lib_py-0.0.0/setup.cfg` & `app_lib_py-0.0.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [metadata]
 name = app_lib_py
+version = 0.0.8
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = Example library for scientific software.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RachelAlcraft/app-lib-py
 project_urls =
```

### Comparing `app_lib_py-0.0.0/src/app_lib_py/ClassCurves.py` & `app_lib_py-0.0.8/src/app_lib_py/ClassCurves.py`

 * *Files identical despite different names*

