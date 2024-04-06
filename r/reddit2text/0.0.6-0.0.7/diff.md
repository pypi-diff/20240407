# Comparing `tmp/reddit2text-0.0.6.tar.gz` & `tmp/reddit2text-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reddit2text-0.0.6.tar", last modified: Sat Apr  6 20:59:46 2024, max compression
+gzip compressed data, was "reddit2text-0.0.7.tar", last modified: Sat Apr  6 21:02:35 2024, max compression
```

## Comparing `reddit2text-0.0.6.tar` & `reddit2text-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 20:59:46.787539 reddit2text-0.0.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 20:59:46.787539 reddit2text-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2806 2024-04-06 20:46:04.000000 reddit2text-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 20:59:46.783539 reddit2text-0.0.6/reddit2text/
--rw-r--r--   0 root         (0) root         (0)       30 2024-04-06 20:45:56.000000 reddit2text-0.0.6/reddit2text/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2962 2024-04-06 20:45:56.000000 reddit2text-0.0.6/reddit2text/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 20:59:46.787539 reddit2text-0.0.6/reddit2text.egg-info/
--rw-r--r--   0 root         (0) root         (0)      960 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 20:59:46.000000 reddit2text-0.0.6/reddit2text.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 20:59:46.787539 reddit2text-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1547 2024-04-06 20:45:56.000000 reddit2text-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:02:35.351683 reddit2text-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-03-05 18:59:10.000000 reddit2text-0.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3494 2024-04-06 21:02:35.351683 reddit2text-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2806 2024-04-06 20:46:04.000000 reddit2text-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:02:35.347684 reddit2text-0.0.7/reddit2text/
+-rw-r--r--   0 root         (0) root         (0)       30 2024-04-06 20:45:56.000000 reddit2text-0.0.7/reddit2text/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2024-04-06 20:45:56.000000 reddit2text-0.0.7/reddit2text/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:02:35.351683 reddit2text-0.0.7/reddit2text.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3494 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-04-06 21:02:35.000000 reddit2text-0.0.7/reddit2text.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 21:02:35.351683 reddit2text-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4081 2024-04-06 21:01:07.000000 reddit2text-0.0.7/setup.py
```

### Comparing `reddit2text-0.0.6/LICENSE` & `reddit2text-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.6/README.md` & `reddit2text-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `reddit2text-0.0.6/reddit2text/main.py` & `reddit2text-0.0.7/reddit2text/main.py`

 * *Files identical despite different names*

