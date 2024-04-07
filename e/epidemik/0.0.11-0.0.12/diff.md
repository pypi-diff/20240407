# Comparing `tmp/epidemik-0.0.11.tar.gz` & `tmp/epidemik-0.0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.11.tar", last modified: Sat Apr  6 19:09:52 2024, max compression
+gzip compressed data, was "epidemik-0.0.12.tar", last modified: Sun Apr  7 18:38:03 2024, max compression
```

## Comparing `epidemik-0.0.11.tar` & `epidemik-0.0.12.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:09:52.328239 epidemik-0.0.11/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.11/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)      593 2024-04-06 19:09:52.328053 epidemik-0.0.11/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.11/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      683 2024-04-06 19:09:37.000000 epidemik-0.0.11/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 19:09:52.328275 epidemik-0.0.11/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:09:52.326450 epidemik-0.0.11/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:09:52.327216 epidemik-0.0.11/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    17904 2024-04-06 19:09:23.000000 epidemik-0.0.11/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.11/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-06 19:09:43.000000 epidemik-0.0.11/src/epidemik/__init__.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:09:52.327844 epidemik-0.0.11/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      593 2024-04-06 19:09:52.000000 epidemik-0.0.11/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-06 19:09:52.000000 epidemik-0.0.11/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 19:09:52.000000 epidemik-0.0.11/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 19:09:52.000000 epidemik-0.0.11/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.579688 epidemik-0.0.12/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.12/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5232 2024-04-07 18:38:03.579496 epidemik-0.0.12/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)     4693 2024-04-07 18:32:21.000000 epidemik-0.0.12/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      683 2024-04-07 18:37:40.000000 epidemik-0.0.12/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-07 18:38:03.579727 epidemik-0.0.12/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.577886 epidemik-0.0.12/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.578595 epidemik-0.0.12/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    17904 2024-04-06 19:09:23.000000 epidemik-0.0.12/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.12/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      290 2024-04-06 19:09:43.000000 epidemik-0.0.12/src/epidemik/__init__.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-07 18:38:03.579302 epidemik-0.0.12/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5232 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-07 18:38:03.000000 epidemik-0.0.12/src/epidemik.egg-info/top_level.txt
```

### Comparing `epidemik-0.0.11/LICENSE` & `epidemik-0.0.12/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.11/pyproject.toml` & `epidemik-0.0.12/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epidemik"
-version = "0.0.11"
+version = "0.0.12"
 authors = [
   { name="Bruno Gonçalves", email="bgoncalves@data4sci.com" },
 ]
 description = "A pakage to simulate compartmental epidemic models"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `epidemik-0.0.11/src/epidemik/EpiModel.py` & `epidemik-0.0.12/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.11/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.12/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

