# Comparing `tmp/kibo_unibs_fp_lib-1.0.0.tar.gz` & `tmp/kibo_unibs_fp_lib-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kibo_unibs_fp_lib-1.0.0.tar", last modified: Fri Apr  5 10:03:09 2024, max compression
+gzip compressed data, was "kibo_unibs_fp_lib-1.0.2.tar", last modified: Sun Apr  7 16:44:43 2024, max compression
```

## Comparing `kibo_unibs_fp_lib-1.0.0.tar` & `kibo_unibs_fp_lib-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:03:09.366963 kibo_unibs_fp_lib-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-05 10:03:04.000000 kibo_unibs_fp_lib-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-05 10:03:09.362962 kibo_unibs_fp_lib-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-05 10:03:04.000000 kibo_unibs_fp_lib-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 10:03:09.362962 kibo_unibs_fp_lib-1.0.0/kibo_unibs_fp_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      926 2024-04-05 10:03:09.000000 kibo_unibs_fp_lib-1.0.0/kibo_unibs_fp_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-05 10:03:09.000000 kibo_unibs_fp_lib-1.0.0/kibo_unibs_fp_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:03:09.000000 kibo_unibs_fp_lib-1.0.0/kibo_unibs_fp_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 10:03:09.000000 kibo_unibs_fp_lib-1.0.0/kibo_unibs_fp_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 10:03:04.000000 kibo_unibs_fp_lib-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 10:03:09.366963 kibo_unibs_fp_lib-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 10:03:04.000000 kibo_unibs_fp_lib-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:44:43.493869 kibo_unibs_fp_lib-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-07 16:44:43.493869 kibo_unibs_fp_lib-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:44:43.489869 kibo_unibs_fp_lib-1.0.2/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:44:43.489869 kibo_unibs_fp_lib-1.0.2/it/kibo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:44:43.489869 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:44:43.493869 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/ansi_colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/file_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10039 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/input_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/known_problems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/pretty_strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/it/kibo/fp/lib/random_draws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:44:43.493869 kibo_unibs_fp_lib-1.0.2/kibo_unibs_fp_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-04-07 16:44:43.000000 kibo_unibs_fp_lib-1.0.2/kibo_unibs_fp_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-07 16:44:43.000000 kibo_unibs_fp_lib-1.0.2/kibo_unibs_fp_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:44:43.000000 kibo_unibs_fp_lib-1.0.2/kibo_unibs_fp_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-07 16:44:43.000000 kibo_unibs_fp_lib-1.0.2/kibo_unibs_fp_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:44:43.493869 kibo_unibs_fp_lib-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-07 16:44:37.000000 kibo_unibs_fp_lib-1.0.2/setup.py
```

### Comparing `kibo_unibs_fp_lib-1.0.0/LICENSE.txt` & `kibo_unibs_fp_lib-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

