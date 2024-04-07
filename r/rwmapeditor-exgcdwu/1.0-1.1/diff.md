# Comparing `tmp/rwmapeditor_exgcdwu-1.0.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.0.tar", last modified: Thu Apr  4 11:57:32 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.1.tar", last modified: Sun Apr  7 13:53:04 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.0.tar` & `rwmapeditor_exgcdwu-1.1.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:57:32.141222 rwmapeditor_exgcdwu-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 11:57:32.141222 rwmapeditor_exgcdwu-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:57:32.141222 rwmapeditor_exgcdwu-1.0/rwgraph/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_default_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:57:32.141222 rwmapeditor_exgcdwu-1.0/rwgraph/_util/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_util/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_util/_object.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_util/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_util/_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/rwgraph/_util/_tileset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 11:57:32.141222 rwmapeditor_exgcdwu-1.0/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-04 11:57:32.000000 rwmapeditor_exgcdwu-1.0/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-04 11:57:32.000000 rwmapeditor_exgcdwu-1.0/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 11:57:32.000000 rwmapeditor_exgcdwu-1.0/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 11:57:32.000000 rwmapeditor_exgcdwu-1.0/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 11:57:32.141222 rwmapeditor_exgcdwu-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-04 11:57:25.000000 rwmapeditor_exgcdwu-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_default_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-07 13:53:03.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 13:53:04.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:53:03.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 13:53:03.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-07 13:53:04.013264 rwmapeditor_exgcdwu-1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.0/LICENSE` & `rwmapeditor_exgcdwu-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.0/setup.py` & `rwmapeditor_exgcdwu-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 #import os
 from setuptools import setup, find_packages
 
-__version__ = '1.0'
+__version__ = '1.1'
 #current_dir = os.path.dirname(__file__)
 #requirements = open(current_dir + '/requirements.txt').readlines()
 
 def readme():
     with open('README.md') as file:
         return file.read()
```

