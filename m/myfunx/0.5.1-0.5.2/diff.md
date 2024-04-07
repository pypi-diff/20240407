# Comparing `tmp/myfunx-0.5.1.tar.gz` & `tmp/myfunx-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myfunx-0.5.1.tar", last modified: Mon Apr  1 12:38:05 2024, max compression
+gzip compressed data, was "myfunx-0.5.2.tar", last modified: Sun Apr  7 13:38:01 2024, max compression
```

## Comparing `myfunx-0.5.1.tar` & `myfunx-0.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:38:05.300567 myfunx-0.5.1/
--rw-r--r--   0 kali      (1000) root         (0)    35149 2024-03-21 10:11:00.000000 myfunx-0.5.1/LICENSE
--rw-r--r--   0 kali      (1000) root         (0)    40684 2024-04-01 12:38:05.300567 myfunx-0.5.1/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      350 2024-03-23 19:19:15.000000 myfunx-0.5.1/README.md
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:38:05.296567 myfunx-0.5.1/myfunx/
--rw-r--r--   0 kali      (1000) root         (0)      263 2024-04-01 12:37:41.000000 myfunx-0.5.1/myfunx/__init__.py
--rw-r--r--   0 kali      (1000) root         (0)     9938 2024-03-25 18:41:16.000000 myfunx-0.5.1/myfunx/client.py
--rw-r--r--   0 kali      (1000) root         (0)     7695 2024-04-01 08:04:27.000000 myfunx-0.5.1/myfunx/json_manager.py
-drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-01 12:38:05.300567 myfunx-0.5.1/myfunx.egg-info/
--rw-r--r--   0 kali      (1000) root         (0)    40684 2024-04-01 12:38:05.000000 myfunx-0.5.1/myfunx.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) root         (0)      240 2024-04-01 12:38:05.000000 myfunx-0.5.1/myfunx.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-01 12:38:05.000000 myfunx-0.5.1/myfunx.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-01 12:38:05.000000 myfunx-0.5.1/myfunx.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-01 12:38:05.000000 myfunx-0.5.1/myfunx.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) root         (0)      300 2024-04-01 12:37:33.000000 myfunx-0.5.1/pyproject.toml
--rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-01 12:38:05.300567 myfunx-0.5.1/setup.cfg
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 13:38:01.001371 myfunx-0.5.2/
+-rw-r--r--   0 kali      (1000) root         (0)    35149 2024-03-21 10:11:00.000000 myfunx-0.5.2/LICENSE
+-rw-r--r--   0 kali      (1000) root         (0)    40684 2024-04-07 13:38:01.001371 myfunx-0.5.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      350 2024-03-23 19:19:15.000000 myfunx-0.5.2/README.md
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 13:38:01.001371 myfunx-0.5.2/myfunx/
+-rw-r--r--   0 kali      (1000) root         (0)      263 2024-04-07 13:37:13.000000 myfunx-0.5.2/myfunx/__init__.py
+-rw-r--r--   0 kali      (1000) root         (0)     5723 2024-04-07 13:37:49.000000 myfunx-0.5.2/myfunx/client.py
+-rw-r--r--   0 kali      (1000) root         (0)     7695 2024-04-01 08:04:27.000000 myfunx-0.5.2/myfunx/json_manager.py
+drwxr-xr-x   0 kali      (1000) root         (0)        0 2024-04-07 13:38:01.001371 myfunx-0.5.2/myfunx.egg-info/
+-rw-r--r--   0 kali      (1000) root         (0)    40684 2024-04-07 13:38:00.000000 myfunx-0.5.2/myfunx.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) root         (0)      240 2024-04-07 13:38:00.000000 myfunx-0.5.2/myfunx.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) root         (0)        1 2024-04-07 13:38:00.000000 myfunx-0.5.2/myfunx.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-07 13:38:00.000000 myfunx-0.5.2/myfunx.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) root         (0)        7 2024-04-07 13:38:00.000000 myfunx-0.5.2/myfunx.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) root         (0)      300 2024-04-07 13:37:10.000000 myfunx-0.5.2/pyproject.toml
+-rw-r--r--   0 kali      (1000) root         (0)       38 2024-04-07 13:38:01.001371 myfunx-0.5.2/setup.cfg
```

### Comparing `myfunx-0.5.1/LICENSE` & `myfunx-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `myfunx-0.5.1/PKG-INFO` & `myfunx-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunx
-Version: 0.5.1
+Version: 0.5.2
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

### Comparing `myfunx-0.5.1/myfunx/json_manager.py` & `myfunx-0.5.2/myfunx/json_manager.py`

 * *Files identical despite different names*

### Comparing `myfunx-0.5.1/myfunx.egg-info/PKG-INFO` & `myfunx-0.5.2/myfunx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunx
-Version: 0.5.1
+Version: 0.5.2
 Author: unixtux
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
```

