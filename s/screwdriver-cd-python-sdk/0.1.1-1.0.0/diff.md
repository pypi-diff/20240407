# Comparing `tmp/screwdriver-cd-python-sdk-0.1.1.tar.gz` & `tmp/screwdriver-cd-python-sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "screwdriver-cd-python-sdk-0.1.1.tar", last modified: Wed Feb 21 08:46:53 2024, max compression
+gzip compressed data, was "screwdriver-cd-python-sdk-1.0.0.tar", last modified: Sun Apr  7 10:09:33 2024, max compression
```

## Comparing `screwdriver-cd-python-sdk-0.1.1.tar` & `screwdriver-cd-python-sdk-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:46:53.400351 screwdriver-cd-python-sdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-21 08:46:53.400351 screwdriver-cd-python-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:46:53.400351 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/screwdriver_initializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:46:53.400351 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-21 08:46:53.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-02-21 08:46:53.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 08:46:53.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 08:46:53.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-02-21 08:46:53.000000 screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 08:46:53.400351 screwdriver-cd-python-sdk-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-21 08:46:50.000000 screwdriver-cd-python-sdk-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/screwdriver_initializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 10:09:32.000000 screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:09:33.011651 screwdriver-cd-python-sdk-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-07 10:09:29.000000 screwdriver-cd-python-sdk-1.0.0/setup.py
```

### Comparing `screwdriver-cd-python-sdk-0.1.1/LICENSE` & `screwdriver-cd-python-sdk-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-0.1.1/README.md` & `screwdriver-cd-python-sdk-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/events.py` & `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/events.py`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/pipeline.py` & `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/pipeline.py`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/screwdriver_initializer.py` & `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/screwdriver_initializer.py`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-0.1.1/screwdriver_cd_python_sdk/secrets.py` & `screwdriver-cd-python-sdk-1.0.0/screwdriver_cd_python_sdk/secrets.py`

 * *Files identical despite different names*

### Comparing `screwdriver-cd-python-sdk-0.1.1/setup.py` & `screwdriver-cd-python-sdk-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="screwdriver-cd-python-sdk",
-    version="0.1.1",
+    version="1.0.0",
     description="Screwdriver CD Python Software Development Kit (SDK) used to write Python automation scripts that create and manage resources in Screwdriver",
     url="https://github.com/QubitPi/screwdriver-cd-python-sdk",
     author="Jiaqi liu",
     author_email="jack20220723@gmail.com",
     license="Apache-2.0",
     packages=find_packages(),
     python_requires='>=3.10',
```

