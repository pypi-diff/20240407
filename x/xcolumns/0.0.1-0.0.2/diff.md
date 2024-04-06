# Comparing `tmp/xcolumns-0.0.1.tar.gz` & `tmp/xcolumns-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xcolumns-0.0.1.tar", last modified: Wed Jan 10 01:58:53 2024, max compression
+gzip compressed data, was "xcolumns-0.0.2.tar", last modified: Sat Apr  6 23:33:54 2024, max compression
```

## Comparing `xcolumns-0.0.1.tar` & `xcolumns-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,29 @@
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-01-10 01:58:53.449337 xcolumns-0.0.1/
--rw-rw-r--   0 marek     (1000) marek     (1000)     1150 2024-01-10 01:58:35.000000 xcolumns-0.0.1/LICENSE
--rw-rw-r--   0 marek     (1000) marek     (1000)     1752 2024-01-10 01:58:53.449337 xcolumns-0.0.1/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)     1564 2024-01-10 01:58:35.000000 xcolumns-0.0.1/README.md
--rw-rw-r--   0 marek     (1000) marek     (1000)     3135 2024-01-10 01:58:35.000000 xcolumns-0.0.1/pyproject.toml
--rw-rw-r--   0 marek     (1000) marek     (1000)       38 2024-01-10 01:58:53.449337 xcolumns-0.0.1/setup.cfg
--rw-rw-r--   0 marek     (1000) marek     (1000)     1028 2024-01-10 01:58:35.000000 xcolumns-0.0.1/setup.py
-drwxrwxr-x   0 marek     (1000) marek     (1000)        0 2024-01-10 01:58:53.449337 xcolumns-0.0.1/xcolumns.egg-info/
--rw-rw-r--   0 marek     (1000) marek     (1000)     1752 2024-01-10 01:58:53.000000 xcolumns-0.0.1/xcolumns.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1000) marek     (1000)      169 2024-01-10 01:58:53.000000 xcolumns-0.0.1/xcolumns.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-01-10 01:58:53.000000 xcolumns-0.0.1/xcolumns.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1000) marek     (1000)        1 2024-01-10 01:58:53.000000 xcolumns-0.0.1/xcolumns.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:33:54.376707 xcolumns-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-06 23:33:50.000000 xcolumns-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-06 23:33:54.376707 xcolumns-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-06 23:33:50.000000 xcolumns-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-04-06 23:33:50.000000 xcolumns-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 23:33:54.376707 xcolumns-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-06 23:33:50.000000 xcolumns-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:33:54.376707 xcolumns-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-06 23:33:50.000000 xcolumns-0.0.2/tests/test_block_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-04-06 23:33:50.000000 xcolumns-0.0.2/tests/test_frank_wolfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-06 23:33:50.000000 xcolumns-0.0.2/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-04-06 23:33:50.000000 xcolumns-0.0.2/tests/test_weighted_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:33:54.376707 xcolumns-0.0.2/xcolumns/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/block_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/confusion_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27086 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/frank_wolfe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22188 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/metrics_original.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16994 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/numba_csr_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17951 2024-04-06 23:33:50.000000 xcolumns-0.0.2/xcolumns/weighted_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 23:33:54.376707 xcolumns-0.0.2/xcolumns.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-04-06 23:33:54.000000 xcolumns-0.0.2/xcolumns.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-06 23:33:54.000000 xcolumns-0.0.2/xcolumns.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 23:33:54.000000 xcolumns-0.0.2/xcolumns.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 23:33:54.000000 xcolumns-0.0.2/xcolumns.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 23:33:54.000000 xcolumns-0.0.2/xcolumns.egg-info/top_level.txt
```

### Comparing `xcolumns-0.0.1/LICENSE` & `xcolumns-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xcolumns-0.0.1/pyproject.toml` & `xcolumns-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "numpy",
     "scipy",
     "numba>=0.58.0",
     "click",
-    "torch",
+    "autograd>=1.6",
     "tqdm",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/mwydmuch/xcolumns"
 Repository = "https://github.com/mwydmuch/xcolumns"
```

### Comparing `xcolumns-0.0.1/setup.py` & `xcolumns-0.0.2/setup.py`

 * *Files identical despite different names*

