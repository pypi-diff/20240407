# Comparing `tmp/electrostats-0.1.tar.gz` & `tmp/electrostats-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "electrostats-0.1.tar", last modified: Sun Apr  7 20:13:45 2024, max compression
+gzip compressed data, was "electrostats-0.2.tar", last modified: Sun Apr  7 20:16:43 2024, max compression
```

## Comparing `electrostats-0.1.tar` & `electrostats-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 20:13:45.185391 electrostats-0.1/
--rw-rw-rw-   0        0        0     1063 2024-04-07 17:34:54.000000 electrostats-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      338 2024-04-07 20:13:45.183385 electrostats-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 20:13:45.156171 electrostats-0.1/electrostats/
--rw-rw-rw-   0        0        0        2 2024-04-07 20:04:14.000000 electrostats-0.1/electrostats/__init__.py
--rw-rw-rw-   0        0        0      258 2024-04-07 20:04:04.000000 electrostats-0.1/electrostats/electrostats.py
-drwxrwxrwx   0        0        0        0 2024-04-07 20:13:45.179389 electrostats-0.1/electrostats.egg-info/
--rw-rw-rw-   0        0        0      338 2024-04-07 20:13:44.000000 electrostats-0.1/electrostats.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2024-04-07 20:13:45.000000 electrostats-0.1/electrostats.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 20:13:44.000000 electrostats-0.1/electrostats.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-07 20:13:44.000000 electrostats-0.1/electrostats.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 20:13:45.185391 electrostats-0.1/setup.cfg
--rw-rw-rw-   0        0        0      415 2024-04-07 17:43:35.000000 electrostats-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:16:43.704854 electrostats-0.2/
+-rw-rw-rw-   0        0        0     1063 2024-04-07 17:34:54.000000 electrostats-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      338 2024-04-07 20:16:43.702879 electrostats-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 20:16:43.680186 electrostats-0.2/electrostats/
+-rw-rw-rw-   0        0        0        2 2024-04-07 20:04:14.000000 electrostats-0.2/electrostats/__init__.py
+-rw-rw-rw-   0        0        0      258 2024-04-07 20:04:04.000000 electrostats-0.2/electrostats/electrostats.py
+drwxrwxrwx   0        0        0        0 2024-04-07 20:16:43.700859 electrostats-0.2/electrostats.egg-info/
+-rw-rw-rw-   0        0        0      338 2024-04-07 20:16:43.000000 electrostats-0.2/electrostats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2024-04-07 20:16:43.000000 electrostats-0.2/electrostats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 20:16:43.000000 electrostats-0.2/electrostats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-07 20:16:43.000000 electrostats-0.2/electrostats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 20:16:43.705852 electrostats-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      415 2024-04-07 20:15:24.000000 electrostats-0.2/setup.py
```

### Comparing `electrostats-0.1/LICENSE.txt` & `electrostats-0.2/LICENSE.txt`

 * *Files identical despite different names*

