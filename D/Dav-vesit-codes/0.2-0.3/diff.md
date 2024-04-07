# Comparing `tmp/Dav_vesit_codes-0.2.tar.gz` & `tmp/Dav_vesit_codes-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dav_vesit_codes-0.2.tar", last modified: Sun Apr  7 11:02:13 2024, max compression
+gzip compressed data, was "Dav_vesit_codes-0.3.tar", last modified: Sun Apr  7 14:48:24 2024, max compression
```

## Comparing `Dav_vesit_codes-0.2.tar` & `Dav_vesit_codes-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 11:02:13.808825 Dav_vesit_codes-0.2/
-drwxrwxrwx   0        0        0        0 2024-04-07 11:02:13.734946 Dav_vesit_codes-0.2/Dav_vesit_codes/
--rw-rw-rw-   0        0        0       27 2024-04-07 11:01:47.000000 Dav_vesit_codes-0.2/Dav_vesit_codes/__init__.py
--rw-rw-rw-   0        0        0     2000 2024-04-07 10:43:10.000000 Dav_vesit_codes-0.2/Dav_vesit_codes/main.py
-drwxrwxrwx   0        0        0        0 2024-04-07 11:02:13.800806 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/
--rw-rw-rw-   0        0        0       60 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-07 11:02:13.000000 Dav_vesit_codes-0.2/Dav_vesit_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2024-04-07 11:02:13.800806 Dav_vesit_codes-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-04-07 10:39:13.000000 Dav_vesit_codes-0.2/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 11:02:13.808825 Dav_vesit_codes-0.2/setup.cfg
--rw-rw-rw-   0        0        0      174 2024-04-07 11:01:56.000000 Dav_vesit_codes-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:48:24.926904 Dav_vesit_codes-0.3/
+drwxrwxrwx   0        0        0        0 2024-04-07 14:48:24.905799 Dav_vesit_codes-0.3/Dav_vesit_codes/
+-rw-rw-rw-   0        0        0       23 2024-04-07 14:45:26.000000 Dav_vesit_codes-0.3/Dav_vesit_codes/__init__.py
+-rw-rw-rw-   0        0        0    14517 2024-04-07 14:45:26.000000 Dav_vesit_codes-0.3/Dav_vesit_codes/main.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:48:24.923910 Dav_vesit_codes-0.3/Dav_vesit_codes.egg-info/
+-rw-rw-rw-   0        0        0       60 2024-04-07 14:48:24.000000 Dav_vesit_codes-0.3/Dav_vesit_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-04-07 14:48:24.000000 Dav_vesit_codes-0.3/Dav_vesit_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 14:48:24.000000 Dav_vesit_codes-0.3/Dav_vesit_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-07 14:48:24.000000 Dav_vesit_codes-0.3/Dav_vesit_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2024-04-07 14:48:24.925905 Dav_vesit_codes-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-04-07 10:39:13.000000 Dav_vesit_codes-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 14:48:24.926904 Dav_vesit_codes-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      176 2024-04-07 14:47:53.000000 Dav_vesit_codes-0.3/setup.py
```

