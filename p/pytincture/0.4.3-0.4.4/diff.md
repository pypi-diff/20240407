# Comparing `tmp/pytincture-0.4.3.tar.gz` & `tmp/pytincture-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytincture-0.4.3.tar", last modified: Wed Apr  3 18:32:15 2024, max compression
+gzip compressed data, was "pytincture-0.4.4.tar", last modified: Sun Apr  7 18:50:29 2024, max compression
```

## Comparing `pytincture-0.4.3.tar` & `pytincture-0.4.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.919792 pytincture-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-03 18:32:06.000000 pytincture-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 18:32:15.919792 pytincture-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-03 18:32:06.000000 pytincture-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/backend/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/dataclass.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture/frontend/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/frontend/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-03 18:32:06.000000 pytincture-0.4.3/pytincture/frontend/pytincture.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:32:15.915792 pytincture-0.4.3/pytincture.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 18:32:15.000000 pytincture-0.4.3/pytincture.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:32:15.919792 pytincture-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 18:32:06.000000 pytincture-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:50:29.392153 pytincture-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-07 18:50:21.000000 pytincture-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-07 18:50:29.392153 pytincture-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-07 18:50:21.000000 pytincture-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:50:29.392153 pytincture-0.4.4/pytincture/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-07 18:50:21.000000 pytincture-0.4.4/pytincture/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:50:29.392153 pytincture-0.4.4/pytincture/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:50:21.000000 pytincture-0.4.4/pytincture/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-04-07 18:50:21.000000 pytincture-0.4.4/pytincture/backend/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-07 18:50:21.000000 pytincture-0.4.4/pytincture/dataclass.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:50:29.392153 pytincture-0.4.4/pytincture/frontend/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-07 18:50:21.000000 pytincture-0.4.4/pytincture/frontend/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-07 18:50:21.000000 pytincture-0.4.4/pytincture/frontend/pytincture.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:50:29.392153 pytincture-0.4.4/pytincture.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-07 18:50:29.000000 pytincture-0.4.4/pytincture.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-07 18:50:29.000000 pytincture-0.4.4/pytincture.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:50:29.000000 pytincture-0.4.4/pytincture.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-07 18:50:29.000000 pytincture-0.4.4/pytincture.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 18:50:29.000000 pytincture-0.4.4/pytincture.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:50:29.392153 pytincture-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-07 18:50:21.000000 pytincture-0.4.4/setup.py
```

### Comparing `pytincture-0.4.3/PKG-INFO` & `pytincture-0.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytincture
-Version: 0.4.3
+Version: 0.4.4
 Summary: UI Builder
 Home-page: https://github.com/pytincture/pytincture
 Description-Content-Type: text/markdown
 
 # pyTincture
 
 ## Overview
@@ -19,15 +19,15 @@
 ## Requirements
 - Python 3.x
 - Pyodide
 
 ## Docker Quick Start
 Run the docker image directly from Dockerhub
 ~~~
-docker run -p8070:8070 -i pytincture/pytincture:example043
+docker run -p8070:8070 -i pytincture/pytincture:example044
 ~~~
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 ## Docker build from repo
@@ -42,10 +42,10 @@
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 
 ## License
-`pyTincture` is licensed under the GPL 2.0 License.
+`pyTincture` is licensed under the MIT License.
```

### Comparing `pytincture-0.4.3/README.md` & `pytincture-0.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ## Requirements
 - Python 3.x
 - Pyodide
 
 ## Docker Quick Start
 Run the docker image directly from Dockerhub
 ~~~
-docker run -p8070:8070 -i pytincture/pytincture:example043
+docker run -p8070:8070 -i pytincture/pytincture:example044
 ~~~
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 ## Docker build from repo
@@ -35,10 +35,10 @@
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 
 ## License
-`pyTincture` is licensed under the GPL 2.0 License.
+`pyTincture` is licensed under the MIT License.
```

### Comparing `pytincture-0.4.3/pytincture/__init__.py` & `pytincture-0.4.4/pytincture/__init__.py`

 * *Files identical despite different names*

### Comparing `pytincture-0.4.3/pytincture/backend/app.py` & `pytincture-0.4.4/pytincture/backend/app.py`

 * *Files identical despite different names*

### Comparing `pytincture-0.4.3/pytincture/dataclass.py` & `pytincture-0.4.4/pytincture/dataclass.py`

 * *Files identical despite different names*

### Comparing `pytincture-0.4.3/pytincture/frontend/index.html` & `pytincture-0.4.4/pytincture/frontend/index.html`

 * *Files identical despite different names*

### Comparing `pytincture-0.4.3/pytincture/frontend/pytincture.js` & `pytincture-0.4.4/pytincture/frontend/pytincture.js`

 * *Files identical despite different names*

### Comparing `pytincture-0.4.3/pytincture.egg-info/PKG-INFO` & `pytincture-0.4.4/pytincture.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytincture
-Version: 0.4.3
+Version: 0.4.4
 Summary: UI Builder
 Home-page: https://github.com/pytincture/pytincture
 Description-Content-Type: text/markdown
 
 # pyTincture
 
 ## Overview
@@ -19,15 +19,15 @@
 ## Requirements
 - Python 3.x
 - Pyodide
 
 ## Docker Quick Start
 Run the docker image directly from Dockerhub
 ~~~
-docker run -p8070:8070 -i pytincture/pytincture:example043
+docker run -p8070:8070 -i pytincture/pytincture:example044
 ~~~
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 ## Docker build from repo
@@ -42,10 +42,10 @@
 Load url in browser
 ~~~
 http://localhost:8070/py_ui
 ~~~
 
 
 ## License
-`pyTincture` is licensed under the GPL 2.0 License.
+`pyTincture` is licensed under the MIT License.
```

### Comparing `pytincture-0.4.3/setup.py` & `pytincture-0.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     install_requires = reqs.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='pytincture',
-    version='0.4.3',
+    version='0.4.4',
     description=(
         'UI Builder'
     ),
     url="https://github.com/pytincture/pytincture",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages = find_packages(),
```

