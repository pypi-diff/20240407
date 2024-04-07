# Comparing `tmp/OpsApi-1.1.2.tar.gz` & `tmp/OpsApi-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpsApi-1.1.2.tar", last modified: Mon Apr  1 10:05:09 2024, max compression
+gzip compressed data, was "OpsApi-1.1.3.tar", last modified: Mon Apr  1 10:23:26 2024, max compression
```

## Comparing `OpsApi-1.1.2.tar` & `OpsApi-1.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:05:09.269838 OpsApi-1.1.2/
--rw-r--r--   0 tongming   (501) staff       (20)        0 2024-04-01 08:43:02.000000 OpsApi-1.1.2/LICENSE
--rw-r--r--   0 tongming   (501) staff       (20)       91 2024-04-01 08:53:51.000000 OpsApi-1.1.2/MANIFEST.in
--rw-r--r--   0 tongming   (501) staff       (20)      371 2024-04-01 10:05:09.269621 OpsApi-1.1.2/PKG-INFO
--rw-r--r--   0 tongming   (501) staff       (20)        0 2024-04-01 08:43:02.000000 OpsApi-1.1.2/README.md
--rw-r--r--   0 tongming   (501) staff       (20)      454 2024-04-01 10:02:28.000000 OpsApi-1.1.2/pyproject.toml
--rw-r--r--   0 tongming   (501) staff       (20)       38 2024-04-01 10:05:09.269885 OpsApi-1.1.2/setup.cfg
-drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:05:09.267589 OpsApi-1.1.2/src/
-drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:05:09.268216 OpsApi-1.1.2/src/OpsApi/
--rw-r--r--   0 tongming   (501) staff       (20)        0 2024-04-01 08:44:08.000000 OpsApi-1.1.2/src/OpsApi/__init__.py
--rw-r--r--   0 tongming   (501) staff       (20)       46 2024-04-01 09:58:46.000000 OpsApi-1.1.2/src/OpsApi/tm.py
-drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:05:09.269390 OpsApi-1.1.2/src/OpsApi.egg-info/
--rw-r--r--   0 tongming   (501) staff       (20)      371 2024-04-01 10:05:09.000000 OpsApi-1.1.2/src/OpsApi.egg-info/PKG-INFO
--rw-r--r--   0 tongming   (501) staff       (20)      253 2024-04-01 10:05:09.000000 OpsApi-1.1.2/src/OpsApi.egg-info/SOURCES.txt
--rw-r--r--   0 tongming   (501) staff       (20)        1 2024-04-01 10:05:09.000000 OpsApi-1.1.2/src/OpsApi.egg-info/dependency_links.txt
--rw-r--r--   0 tongming   (501) staff       (20)        9 2024-04-01 10:05:09.000000 OpsApi-1.1.2/src/OpsApi.egg-info/requires.txt
--rw-r--r--   0 tongming   (501) staff       (20)        7 2024-04-01 10:05:09.000000 OpsApi-1.1.2/src/OpsApi.egg-info/top_level.txt
+drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:23:26.851719 OpsApi-1.1.3/
+-rw-r--r--   0 tongming   (501) staff       (20)        0 2024-04-01 08:43:02.000000 OpsApi-1.1.3/LICENSE
+-rw-r--r--   0 tongming   (501) staff       (20)       91 2024-04-01 08:53:51.000000 OpsApi-1.1.3/MANIFEST.in
+-rw-r--r--   0 tongming   (501) staff       (20)      371 2024-04-01 10:23:26.851505 OpsApi-1.1.3/PKG-INFO
+-rw-r--r--   0 tongming   (501) staff       (20)        0 2024-04-01 08:43:02.000000 OpsApi-1.1.3/README.md
+-rw-r--r--   0 tongming   (501) staff       (20)      454 2024-04-01 10:21:54.000000 OpsApi-1.1.3/pyproject.toml
+-rw-r--r--   0 tongming   (501) staff       (20)       38 2024-04-01 10:23:26.851763 OpsApi-1.1.3/setup.cfg
+drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:23:26.849581 OpsApi-1.1.3/src/
+drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:23:26.850461 OpsApi-1.1.3/src/OpsApi/
+-rw-r--r--   0 tongming   (501) staff       (20)       10 2024-04-01 10:21:13.000000 OpsApi-1.1.3/src/OpsApi/__init__.py
+-rw-r--r--   0 tongming   (501) staff       (20)       46 2024-04-01 09:58:46.000000 OpsApi-1.1.3/src/OpsApi/tm.py
+drwxr-xr-x   0 tongming   (501) staff       (20)        0 2024-04-01 10:23:26.851268 OpsApi-1.1.3/src/OpsApi.egg-info/
+-rw-r--r--   0 tongming   (501) staff       (20)      371 2024-04-01 10:23:26.000000 OpsApi-1.1.3/src/OpsApi.egg-info/PKG-INFO
+-rw-r--r--   0 tongming   (501) staff       (20)      253 2024-04-01 10:23:26.000000 OpsApi-1.1.3/src/OpsApi.egg-info/SOURCES.txt
+-rw-r--r--   0 tongming   (501) staff       (20)        1 2024-04-01 10:23:26.000000 OpsApi-1.1.3/src/OpsApi.egg-info/dependency_links.txt
+-rw-r--r--   0 tongming   (501) staff       (20)        9 2024-04-01 10:23:26.000000 OpsApi-1.1.3/src/OpsApi.egg-info/requires.txt
+-rw-r--r--   0 tongming   (501) staff       (20)        7 2024-04-01 10:23:26.000000 OpsApi-1.1.3/src/OpsApi.egg-info/top_level.txt
```

