# Comparing `tmp/soundtools-0.1.3.1.tar.gz` & `tmp/soundtools-0.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundtools-0.1.3.1.tar", last modified: Sat Apr  6 19:19:41 2024, max compression
+gzip compressed data, was "soundtools-0.1.3.2.tar", last modified: Sat Apr  6 19:24:42 2024, max compression
```

## Comparing `soundtools-0.1.3.1.tar` & `soundtools-0.1.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 19:19:41.693376 soundtools-0.1.3.1/
--rw-rw-rw-   0        0        0      345 2024-04-06 19:19:41.693376 soundtools-0.1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-03-26 02:19:51.000000 soundtools-0.1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 19:19:41.693376 soundtools-0.1.3.1/setup.cfg
--rw-rw-rw-   0        0        0      411 2024-04-06 19:17:40.000000 soundtools-0.1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:19:41.680921 soundtools-0.1.3.1/soundtools/
--rw-rw-rw-   0        0        0       24 2024-04-06 19:17:57.000000 soundtools-0.1.3.1/soundtools/__init__.py
--rw-rw-rw-   0        0        0    31723 2024-03-29 13:04:18.000000 soundtools-0.1.3.1/soundtools/soundtools.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:19:41.692371 soundtools-0.1.3.1/soundtools.egg-info/
--rw-rw-rw-   0        0        0      345 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-06 19:19:41.000000 soundtools-0.1.3.1/soundtools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-06 19:24:42.849425 soundtools-0.1.3.2/
+-rw-rw-rw-   0        0        0      345 2024-04-06 19:24:42.848425 soundtools-0.1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-03-26 02:19:51.000000 soundtools-0.1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 19:24:42.849425 soundtools-0.1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      411 2024-04-06 19:23:47.000000 soundtools-0.1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:24:42.845917 soundtools-0.1.3.2/soundtools/
+-rw-rw-rw-   0        0        0       25 2024-04-06 19:22:41.000000 soundtools-0.1.3.2/soundtools/__init__.py
+-rw-rw-rw-   0        0        0    31723 2024-03-29 13:04:18.000000 soundtools-0.1.3.2/soundtools/soundtools.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:24:42.848425 soundtools-0.1.3.2/soundtools.egg-info/
+-rw-rw-rw-   0        0        0      345 2024-04-06 19:24:42.000000 soundtools-0.1.3.2/soundtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2024-04-06 19:24:42.000000 soundtools-0.1.3.2/soundtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 19:24:42.000000 soundtools-0.1.3.2/soundtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-06 19:24:42.000000 soundtools-0.1.3.2/soundtools.egg-info/top_level.txt
```

### Comparing `soundtools-0.1.3.1/soundtools/soundtools.py` & `soundtools-0.1.3.2/soundtools/soundtools.py`

 * *Files identical despite different names*

