# Comparing `tmp/crawlab-ai-0.0.2.tar.gz` & `tmp/crawlab-ai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlab-ai-0.0.2.tar", last modified: Wed Apr  3 06:08:31 2024, max compression
+gzip compressed data, was "crawlab-ai-0.0.3.tar", last modified: Sun Apr  7 06:00:08 2024, max compression
```

## Comparing `crawlab-ai-0.0.2.tar` & `crawlab-ai-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:08:31.659355 crawlab-ai-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 06:08:31.655356 crawlab-ai-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:08:31.655356 crawlab-ai-0.0.2/crawlab_ai/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/crawlab_ai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:08:31.655356 crawlab-ai-0.0.2/crawlab_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 06:08:31.000000 crawlab-ai-0.0.2/crawlab_ai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:08:31.659355 crawlab-ai-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 06:08:02.000000 crawlab-ai-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/crawlab_ai/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/crawlab_ai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/crawlab_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 06:00:08.000000 crawlab-ai-0.0.3/crawlab_ai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:00:08.096147 crawlab-ai-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-07 05:59:47.000000 crawlab-ai-0.0.3/setup.py
```

### Comparing `crawlab-ai-0.0.2/LICENSE` & `crawlab-ai-0.0.3/LICENSE`

 * *Files identical despite different names*

