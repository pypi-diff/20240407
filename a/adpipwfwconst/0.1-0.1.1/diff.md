# Comparing `tmp/adpipwfwconst-0.1.tar.gz` & `tmp/adpipwfwconst-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adpipwfwconst-0.1.tar", last modified: Thu Apr  4 00:38:37 2024, max compression
+gzip compressed data, was "adpipwfwconst-0.1.1.tar", last modified: Sun Apr  7 17:04:33 2024, max compression
```

## Comparing `adpipwfwconst-0.1.tar` & `adpipwfwconst-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 00:38:37.839111 adpipwfwconst-0.1/
--rw-r--r--   0 root         (0) root         (0)     1067 2024-04-04 00:38:14.000000 adpipwfwconst-0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-04 00:38:37.839111 adpipwfwconst-0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-04 00:38:14.000000 adpipwfwconst-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 00:38:37.839111 adpipwfwconst-0.1/adpipwfwconst/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-04 00:38:14.000000 adpipwfwconst-0.1/adpipwfwconst/__init__.py
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-04 00:38:14.000000 adpipwfwconst-0.1/adpipwfwconst/pipelineconstants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-04 00:38:37.839111 adpipwfwconst-0.1/adpipwfwconst.egg-info/
--rw-r--r--   0 root         (0) root         (0)      311 2024-04-04 00:38:37.000000 adpipwfwconst-0.1/adpipwfwconst.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      235 2024-04-04 00:38:37.000000 adpipwfwconst-0.1/adpipwfwconst.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-04 00:38:37.000000 adpipwfwconst-0.1/adpipwfwconst.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-04 00:38:37.000000 adpipwfwconst-0.1/adpipwfwconst.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-04 00:38:37.839111 adpipwfwconst-0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-04 00:38:14.000000 adpipwfwconst-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:04:33.662995 adpipwfwconst-0.1.1/
+-rw-r--r--   0 root         (0) root         (0)     1067 2024-04-07 17:04:07.000000 adpipwfwconst-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-07 17:04:33.662995 adpipwfwconst-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-07 17:04:07.000000 adpipwfwconst-0.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:04:33.662995 adpipwfwconst-0.1.1/adpipwfwconst/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 17:04:07.000000 adpipwfwconst-0.1.1/adpipwfwconst/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      992 2024-04-07 17:04:07.000000 adpipwfwconst-0.1.1/adpipwfwconst/pipelineconstants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 17:04:33.662995 adpipwfwconst-0.1.1/adpipwfwconst.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      313 2024-04-07 17:04:33.000000 adpipwfwconst-0.1.1/adpipwfwconst.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-07 17:04:33.000000 adpipwfwconst-0.1.1/adpipwfwconst.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 17:04:33.000000 adpipwfwconst-0.1.1/adpipwfwconst.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-07 17:04:33.000000 adpipwfwconst-0.1.1/adpipwfwconst.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 17:04:33.662995 adpipwfwconst-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      408 2024-04-07 17:04:07.000000 adpipwfwconst-0.1.1/setup.py
```

### Comparing `adpipwfwconst-0.1/LICENSE` & `adpipwfwconst-0.1.1/LICENSE`

 * *Files identical despite different names*

