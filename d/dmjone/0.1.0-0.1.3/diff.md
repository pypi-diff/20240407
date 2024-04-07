# Comparing `tmp/dmjone-0.1.0.tar.gz` & `tmp/dmjone-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dmjone-0.1.0.tar", last modified: Sun Apr  7 06:00:22 2024, max compression
+gzip compressed data, was "dmjone-0.1.3.tar", last modified: Sun Apr  7 07:05:34 2024, max compression
```

## Comparing `dmjone-0.1.0.tar` & `dmjone-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:22.811932 dmjone-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-07 06:00:18.000000 dmjone-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-07 06:00:22.811932 dmjone-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 06:00:18.000000 dmjone-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-07 06:00:18.000000 dmjone-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:00:22.811932 dmjone-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:22.811932 dmjone-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:22.811932 dmjone-0.1.0/src/dmjone/
--rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-07 06:00:18.000000 dmjone-0.1.0/src/dmjone/StudentManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:18.000000 dmjone-0.1.0/src/dmjone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 06:00:18.000000 dmjone-0.1.0/src/dmjone/lab4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:22.811932 dmjone-0.1.0/src/dmjone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-04-07 06:00:22.000000 dmjone-0.1.0/src/dmjone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-07 06:00:22.000000 dmjone-0.1.0/src/dmjone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:00:22.000000 dmjone-0.1.0/src/dmjone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 06:00:22.000000 dmjone-0.1.0/src/dmjone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 06:00:22.000000 dmjone-0.1.0/src/dmjone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.070443 dmjone-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 07:05:22.000000 dmjone-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 07:05:22.000000 dmjone-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    41708 2024-04-07 07:05:34.070443 dmjone-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 07:05:22.000000 dmjone-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-07 07:05:22.000000 dmjone-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 07:05:34.070443 dmjone-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.066443 dmjone-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.070443 dmjone-0.1.3/src/dmjone/
+-rw-r--r--   0 runner    (1001) docker     (127)    12482 2024-04-07 07:05:22.000000 dmjone-0.1.3/src/dmjone/StudentManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-07 07:05:22.000000 dmjone-0.1.3/src/dmjone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 07:05:22.000000 dmjone-0.1.3/src/dmjone/lab4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 07:05:34.070443 dmjone-0.1.3/src/dmjone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    41708 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 07:05:34.000000 dmjone-0.1.3/src/dmjone.egg-info/top_level.txt
```

### Comparing `dmjone-0.1.0/src/dmjone/StudentManagementSystem.py` & `dmjone-0.1.3/src/dmjone/StudentManagementSystem.py`

 * *Files identical despite different names*

