# Comparing `tmp/easydebugger-0.0.1.tar.gz` & `tmp/easydebugger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydebugger-0.0.1.tar", last modified: Sun Apr  7 15:24:07 2024, max compression
+gzip compressed data, was "easydebugger-1.0.0.tar", last modified: Sun Apr  7 15:57:55 2024, max compression
```

## Comparing `easydebugger-0.0.1.tar` & `easydebugger-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 15:24:07.226676 easydebugger-0.0.1/
--rw-rw-rw-   0        0        0      144 2024-04-07 15:24:07.224681 easydebugger-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 15:24:07.206149 easydebugger-0.0.1/easydebugger/
--rw-rw-rw-   0        0        0     6105 2024-04-07 15:16:44.000000 easydebugger-0.0.1/easydebugger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:24:07.222687 easydebugger-0.0.1/easydebugger.egg-info/
--rw-rw-rw-   0        0        0      144 2024-04-07 15:24:07.000000 easydebugger-0.0.1/easydebugger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-07 15:24:07.000000 easydebugger-0.0.1/easydebugger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 15:24:07.000000 easydebugger-0.0.1/easydebugger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-07 15:24:07.000000 easydebugger-0.0.1/easydebugger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 15:24:07.226676 easydebugger-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      360 2024-04-07 15:22:28.000000 easydebugger-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:57:55.454981 easydebugger-1.0.0/
+-rw-rw-rw-   0        0        0      207 2024-04-07 15:57:55.447002 easydebugger-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 15:57:55.428048 easydebugger-1.0.0/easydebugger/
+-rw-rw-rw-   0        0        0     6105 2024-04-07 15:16:44.000000 easydebugger-1.0.0/easydebugger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 15:57:55.446005 easydebugger-1.0.0/easydebugger.egg-info/
+-rw-rw-rw-   0        0        0      207 2024-04-07 15:57:55.000000 easydebugger-1.0.0/easydebugger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-07 15:57:55.000000 easydebugger-1.0.0/easydebugger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 15:57:55.000000 easydebugger-1.0.0/easydebugger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-07 15:57:55.000000 easydebugger-1.0.0/easydebugger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 15:57:55.454981 easydebugger-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      480 2024-04-07 15:57:44.000000 easydebugger-1.0.0/setup.py
```

### Comparing `easydebugger-0.0.1/easydebugger/__init__.py` & `easydebugger-1.0.0/easydebugger/__init__.py`

 * *Files identical despite different names*

