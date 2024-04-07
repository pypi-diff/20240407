# Comparing `tmp/Dav_vesit_codes-0.1.tar.gz` & `tmp/Dav_vesit_codes-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dav_vesit_codes-0.1.tar", last modified: Sun Apr  7 10:56:32 2024, max compression
+gzip compressed data, was "Dav_vesit_codes-0.2.tar", last modified: Sun Apr  7 11:02:13 2024, max compression
```

## Comparing `Dav_vesit_codes-0.1.tar` & `Dav_vesit_codes-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 10:56:32.399609 Dav_vesit_codes-0.1/
-drwxrwxrwx   0        0        0        0 2024-04-07 10:56:32.343077 Dav_vesit_codes-0.1/Dav_vesit_codes/
--rw-rw-rw-   0        0        0       23 2024-04-07 10:44:31.000000 Dav_vesit_codes-0.1/Dav_vesit_codes/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-04-07 10:43:10.000000 Dav_vesit_codes-0.1/Dav_vesit_codes/main.py
-drwxrwxrwx   0        0        0        0 2024-04-07 10:56:32.392415 Dav_vesit_codes-0.1/Dav_vesit_codes.egg-info/
--rw-rw-rw-   0        0        0       60 2024-04-07 10:56:31.000000 Dav_vesit_codes-0.1/Dav_vesit_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-04-07 10:56:32.000000 Dav_vesit_codes-0.1/Dav_vesit_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 10:56:31.000000 Dav_vesit_codes-0.1/Dav_vesit_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-07 10:56:31.000000 Dav_vesit_codes-0.1/Dav_vesit_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2024-04-07 10:56:32.392415 Dav_vesit_codes-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 10:39:13.000000 Dav_vesit_codes-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 10:56:32.399609 Dav_vesit_codes-0.1/setup.cfg
--rw-rw-rw-   0        0        0      174 2024-04-07 10:53:10.000000 Dav_vesit_codes-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:02:13.808825 Dav_vesit_codes-0.2/
+drwxrwxrwx   0        0        0        0 2024-04-07 11:02:13.734946 Dav_vesit_codes-0.2/Dav_vesit_codes/
+-rw-rw-rw-   0        0        0       27 2024-04-07 11:01:47.000000 Dav_vesit_codes-0.2/Dav_vesit_codes/__init__.py
+-rw-rw-rw-   0        0        0     2000 2024-04-07 10:43:10.000000 Dav_vesit_codes-0.2/Dav_vesit_codes/main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 11:02:13.800806 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/
+-rw-rw-rw-   0        0        0       60 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2024-04-07 11:02:13.800806 Dav_vesit_codes-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 10:39:13.000000 Dav_vesit_codes-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 11:02:13.808825 Dav_vesit_codes-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      174 2024-04-07 11:01:56.000000 Dav_vesit_codes-0.2/setup.py
```

### Comparing `Dav_vesit_codes-0.1/Dav_vesit_codes/main.py` & `Dav_vesit_codes-0.2/Dav_vesit_codes/main.py`

 * *Files identical despite different names*

