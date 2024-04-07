# Comparing `tmp/loadimg-0.1.1.tar.gz` & `tmp/loadimg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadimg-0.1.1.tar", last modified: Sat Apr  6 07:35:01 2024, max compression
+gzip compressed data, was "loadimg-0.1.2.tar", last modified: Sun Apr  7 13:20:37 2024, max compression
```

## Comparing `loadimg-0.1.1.tar` & `loadimg-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:35:01.404891 loadimg-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 07:34:56.000000 loadimg-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-06 07:35:01.404891 loadimg-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-06 07:34:56.000000 loadimg-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-06 07:34:56.000000 loadimg-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 07:35:01.404891 loadimg-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-06 07:34:56.000000 loadimg-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:35:01.400891 loadimg-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:35:01.400891 loadimg-0.1.1/src/loadimg/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 07:34:56.000000 loadimg-0.1.1/src/loadimg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2413 2024-04-06 07:34:56.000000 loadimg-0.1.1/src/loadimg/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 07:35:01.404891 loadimg-0.1.1/src/loadimg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-06 07:35:01.000000 loadimg-0.1.1/src/loadimg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-06 07:35:01.000000 loadimg-0.1.1/src/loadimg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 07:35:01.000000 loadimg-0.1.1/src/loadimg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 07:35:01.000000 loadimg-0.1.1/src/loadimg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:20:37.447288 loadimg-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 13:20:33.000000 loadimg-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 13:20:37.447288 loadimg-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 13:20:33.000000 loadimg-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-07 13:20:33.000000 loadimg-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 13:20:37.447288 loadimg-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-07 13:20:33.000000 loadimg-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:20:37.447288 loadimg-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:20:37.447288 loadimg-0.1.2/src/loadimg/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 13:20:33.000000 loadimg-0.1.2/src/loadimg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-07 13:20:33.000000 loadimg-0.1.2/src/loadimg/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:20:37.447288 loadimg-0.1.2/src/loadimg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 13:20:37.000000 loadimg-0.1.2/src/loadimg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-07 13:20:37.000000 loadimg-0.1.2/src/loadimg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:20:37.000000 loadimg-0.1.2/src/loadimg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-07 13:20:37.000000 loadimg-0.1.2/src/loadimg.egg-info/top_level.txt
```

### Comparing `loadimg-0.1.1/LICENSE` & `loadimg-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loadimg-0.1.1/PKG-INFO` & `loadimg-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadimg
-Version: 0.1.1
+Version: 0.1.2
 Summary: a python package for loading images
 Home-page: https://github.com/not-lain/loadimg
 Author-email: hhichri60@gmail.com
 License: Apache 2.0 License
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Requires: setuptools
```

### Comparing `loadimg-0.1.1/setup.py` & `loadimg-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 setup(
     name="loadimg",
-    version="0.1.1",
+    version="0.1.2",
     description="a python package for loading images",
     long_description=pathlib.Path("README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     Homepage="https://github.com/not-lain/loadimg",
     url="https://github.com/not-lain/loadimg",
     Issues="https://github.com/not-lain/loadimg/issues",
     authors=[{"name": "hafedh hichri", "email": "hhichri60@gmail.com"}],
```

### Comparing `loadimg-0.1.1/src/loadimg/utils.py` & `loadimg-0.1.2/src/loadimg/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 
 
 def download_image(url: str):
     """A function to get a Pillow image from a URL."""
     try:
         if "github" in url and "raw=true" not in url:
             url += "?raw=true"
-        if "drive" in url and "uc?id=" not in url:
+        elif "drive" in url and "uc?id=" not in url:
             if "/view" in url or url.endswith("/"):
                 url = "/".join(url.split("/")[:-1])
             url = "https://drive.google.com/uc?id=" + url.split("/")[-1]
+        elif "hf.co" or "huggingface.co" in url : 
+            url = url.replace("/blob/","/resolve")
         response = requests.get(url, timeout=5)  # Timeout set to 5 seconds
         response.raise_for_status()  # Raise an exception for HTTP errors
         return Image.open(BytesIO(response.content))
     except requests.exceptions.RequestException as e:
         print(f"Error downloading image from {url}: {e}")
         return None  # Return None if there's an error
```

### Comparing `loadimg-0.1.1/src/loadimg.egg-info/PKG-INFO` & `loadimg-0.1.2/src/loadimg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadimg
-Version: 0.1.1
+Version: 0.1.2
 Summary: a python package for loading images
 Home-page: https://github.com/not-lain/loadimg
 Author-email: hhichri60@gmail.com
 License: Apache 2.0 License
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3.9
 Requires: setuptools
```

