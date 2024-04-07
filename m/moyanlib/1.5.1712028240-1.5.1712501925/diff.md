# Comparing `tmp/moyanlib-1.5.1712028240.tar.gz` & `tmp/moyanlib-1.5.1712501925.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moyanlib-1.5.1712028240.tar", last modified: Tue Apr  2 03:24:00 2024, max compression
+gzip compressed data, was "moyanlib-1.5.1712501925.tar", last modified: Sun Apr  7 14:58:46 2024, max compression
```

## Comparing `moyanlib-1.5.1712028240.tar` & `moyanlib-1.5.1712501925.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.319382 moyanlib-1.5.1712028240/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-02 03:24:00.319382 moyanlib-1.5.1712028240/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.319382 moyanlib-1.5.1712028240/moyanlib/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.319382 moyanlib-1.5.1712028240/moyanlib/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/jsons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/moyanlib/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.319382 moyanlib-1.5.1712028240/moyanlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-02 03:24:00.000000 moyanlib-1.5.1712028240/moyanlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-02 03:24:00.000000 moyanlib-1.5.1712028240/moyanlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 03:24:00.000000 moyanlib-1.5.1712028240/moyanlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 03:24:00.000000 moyanlib-1.5.1712028240/moyanlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-02 03:24:00.000000 moyanlib-1.5.1712028240/moyanlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 03:24:00.000000 moyanlib-1.5.1712028240/moyanlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 03:24:00.319382 moyanlib-1.5.1712028240/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 03:24:00.319382 moyanlib-1.5.1712028240/test/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/test/test_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 03:23:47.000000 moyanlib-1.5.1712028240/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.051429 moyanlib-1.5.1712501925/moyanlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.051429 moyanlib-1.5.1712501925/moyanlib/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/jsons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.051429 moyanlib-1.5.1712501925/moyanlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_utils.py
```

### Comparing `moyanlib-1.5.1712028240/moyanlib/__init__.py` & `moyanlib-1.5.1712501925/moyanlib/__init__.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712028240/moyanlib/cache.py` & `moyanlib-1.5.1712501925/moyanlib/cache.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712028240/moyanlib/cli/__init__.py` & `moyanlib-1.5.1712501925/moyanlib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712028240/moyanlib/decorators.py` & `moyanlib-1.5.1712501925/moyanlib/decorators.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712028240/moyanlib/jsons.py` & `moyanlib-1.5.1712501925/moyanlib/jsons.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712028240/moyanlib/logger.py` & `moyanlib-1.5.1712501925/moyanlib/logger.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712028240/moyanlib/system.py` & `moyanlib-1.5.1712501925/moyanlib/system.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712028240/setup.py` & `moyanlib-1.5.1712501925/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,16 +7,15 @@
     description="莫颜的个人python函数包",
     author="MoYan",
     packages=find_packages(),
     install_requires=[
         # 添加你的依赖库
         "requests",
         "psutil",
-        "click",
-        "rsa",
+        "click"
     ],
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `moyanlib-1.5.1712028240/test/test_cache.py` & `moyanlib-1.5.1712501925/test/test_cache.py`

 * *Files identical despite different names*

