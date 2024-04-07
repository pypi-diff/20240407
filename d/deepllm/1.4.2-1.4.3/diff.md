# Comparing `tmp/deepllm-1.4.2.tar.gz` & `tmp/deepllm-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepllm-1.4.2.tar", last modified: Thu Apr  4 03:14:58 2024, max compression
+gzip compressed data, was "deepllm-1.4.3.tar", last modified: Sun Apr  7 21:27:30 2024, max compression
```

## Comparing `deepllm-1.4.2.tar` & `deepllm-1.4.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:14:58.158783 deepllm-1.4.2/
--rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.4.2/LICENSE
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-04 03:14:58.158431 deepllm-1.4.2/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.4.2/README.md
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:14:58.136396 deepllm-1.4.2/deepllm/
--rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-04 03:11:38.000000 deepllm-1.4.2/deepllm/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2188 2024-03-22 05:04:24.000000 deepllm-1.4.2/deepllm/api.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:14:58.142416 deepllm-1.4.2/deepllm/apps/
--rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.4.2/deepllm/apps/README.md
--rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.4.2/deepllm/apps/app.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.4.2/deepllm/apps/app.sh
--rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.2/deepllm/apps/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)    11175 2024-03-25 01:01:26.000000 deepllm-1.4.2/deepllm/apps/rel_graph.html
--rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.4.2/deepllm/apps/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.4.2/deepllm/configurator.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:14:58.145307 deepllm-1.4.2/deepllm/demos/
--rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.4.2/deepllm/demos/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.2/deepllm/demos/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.4.2/deepllm/demos/demo.py
--rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.4.2/deepllm/demos/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.4.2/deepllm/demos/requirements.txt
--rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.4.2/deepllm/demos/viz.py
--rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.4.2/deepllm/horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)    10875 2024-03-04 01:12:04.000000 deepllm-1.4.2/deepllm/interactors.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:14:58.149663 deepllm-1.4.2/deepllm/local_llms/
--rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.4.2/deepllm/local_llms/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.2/deepllm/local_llms/__init__.py
--rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.2/deepllm/local_llms/install.sh
--rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.4.2/deepllm/local_llms/local_runs.py
--rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.4.2/deepllm/local_llms/requirements.txt
--rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.4.2/deepllm/local_llms/server.sh
--rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.4.2/deepllm/local_llms/test_vicuna.py
--rw-r--r--   0 tarau      (503) staff       (20)     3708 2024-03-24 18:59:54.000000 deepllm-1.4.2/deepllm/params.py
--rw-r--r--   0 tarau      (503) staff       (20)     9634 2024-03-25 00:11:40.000000 deepllm-1.4.2/deepllm/prompters.py
--rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.4.2/deepllm/questmaker.py
--rw-r--r--   0 tarau      (503) staff       (20)    10784 2024-03-25 00:48:51.000000 deepllm-1.4.2/deepllm/recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     6667 2024-03-24 21:51:28.000000 deepllm-1.4.2/deepllm/refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.4.2/deepllm/requirements.txt
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:14:58.157682 deepllm-1.4.2/deepllm/tests/
--rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.4.2/deepllm/tests/README.md
--rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.4.2/deepllm/tests/__init__.py
--rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.4.2/deepllm/tests/test_all.py
--rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.4.2/deepllm/tests/test_api.py
--rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.4.2/deepllm/tests/test_configurator.py
--rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.4.2/deepllm/tests/test_embedders.py
--rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.4.2/deepllm/tests/test_horn_prover.py
--rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.4.2/deepllm/tests/test_interactors.py
--rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.4.2/deepllm/tests/test_params.py
--rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.4.2/deepllm/tests/test_recursors.py
--rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.4.2/deepllm/tests/test_refiners.py
--rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.4.2/deepllm/tools.py
--rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.4.2/deepllm/vis.py
-drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-04 03:14:58.138362 deepllm-1.4.2/deepllm.egg-info/
--rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-04 03:14:58.000000 deepllm-1.4.2/deepllm.egg-info/PKG-INFO
--rw-r--r--   0 tarau      (503) staff       (20)     1319 2024-04-04 03:14:58.000000 deepllm-1.4.2/deepllm.egg-info/SOURCES.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:14:58.000000 deepllm-1.4.2/deepllm.egg-info/dependency_links.txt
--rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-04 03:14:58.000000 deepllm-1.4.2/deepllm.egg-info/not-zip-safe
--rw-r--r--   0 tarau      (503) staff       (20)       59 2024-04-04 03:14:58.000000 deepllm-1.4.2/deepllm.egg-info/requires.txt
--rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-04 03:14:58.000000 deepllm-1.4.2/deepllm.egg-info/top_level.txt
--rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-04 03:14:58.158901 deepllm-1.4.2/setup.cfg
--rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.4.2/setup.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-07 21:27:30.431853 deepllm-1.4.3/
+-rw-r--r--   0 tarau      (503) staff       (20)    35149 2023-06-23 23:27:38.000000 deepllm-1.4.3/LICENSE
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-07 21:27:30.431508 deepllm-1.4.3/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     4366 2023-07-18 14:36:48.000000 deepllm-1.4.3/README.md
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-07 21:27:30.412910 deepllm-1.4.3/deepllm/
+-rw-r--r--   0 tarau      (503) staff       (20)       22 2024-04-07 21:23:58.000000 deepllm-1.4.3/deepllm/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2188 2024-03-22 05:04:24.000000 deepllm-1.4.3/deepllm/api.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-07 21:27:30.418595 deepllm-1.4.3/deepllm/apps/
+-rw-r--r--   0 tarau      (503) staff       (20)       51 2023-07-08 16:25:29.000000 deepllm-1.4.3/deepllm/apps/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)     3615 2024-03-25 00:43:56.000000 deepllm-1.4.3/deepllm/apps/app.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       21 2023-08-09 18:23:15.000000 deepllm-1.4.3/deepllm/apps/app.sh
+-rwxr-xr-x   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.3/deepllm/apps/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)    11175 2024-03-25 01:01:26.000000 deepllm-1.4.3/deepllm/apps/rel_graph.html
+-rw-r--r--   0 tarau      (503) staff       (20)       18 2024-03-16 22:29:32.000000 deepllm-1.4.3/deepllm/apps/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)      663 2024-01-01 16:38:49.000000 deepllm-1.4.3/deepllm/configurator.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-07 21:27:30.421345 deepllm-1.4.3/deepllm/demos/
+-rw-r--r--   0 tarau      (503) staff       (20)       98 2023-07-10 19:44:29.000000 deepllm-1.4.3/deepllm/demos/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.3/deepllm/demos/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2151 2024-02-25 03:35:53.000000 deepllm-1.4.3/deepllm/demos/demo.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)       75 2024-01-02 02:47:22.000000 deepllm-1.4.3/deepllm/demos/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)       44 2024-01-02 02:54:03.000000 deepllm-1.4.3/deepllm/demos/requirements.txt
+-rw-r--r--   0 tarau      (503) staff       (20)     1951 2023-10-04 22:28:27.000000 deepllm-1.4.3/deepllm/demos/viz.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3825 2023-10-13 02:28:54.000000 deepllm-1.4.3/deepllm/horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)    10875 2024-03-04 01:12:04.000000 deepllm-1.4.3/deepllm/interactors.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-07 21:27:30.424279 deepllm-1.4.3/deepllm/local_llms/
+-rw-r--r--   0 tarau      (503) staff       (20)      108 2023-07-03 02:51:19.000000 deepllm-1.4.3/deepllm/local_llms/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-03 00:21:12.000000 deepllm-1.4.3/deepllm/local_llms/__init__.py
+-rw-r--r--   0 tarau      (503) staff       (20)       33 2023-07-03 02:30:00.000000 deepllm-1.4.3/deepllm/local_llms/install.sh
+-rw-r--r--   0 tarau      (503) staff       (20)      727 2023-07-03 05:58:58.000000 deepllm-1.4.3/deepllm/local_llms/local_runs.py
+-rw-r--r--   0 tarau      (503) staff       (20)        9 2023-07-03 02:40:19.000000 deepllm-1.4.3/deepllm/local_llms/requirements.txt
+-rwxr-xr-x   0 tarau      (503) staff       (20)      205 2023-07-03 02:43:48.000000 deepllm-1.4.3/deepllm/local_llms/server.sh
+-rw-r--r--   0 tarau      (503) staff       (20)     1028 2023-08-12 16:50:59.000000 deepllm-1.4.3/deepllm/local_llms/test_vicuna.py
+-rw-r--r--   0 tarau      (503) staff       (20)     3708 2024-03-24 18:59:54.000000 deepllm-1.4.3/deepllm/params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     9716 2024-04-07 21:18:58.000000 deepllm-1.4.3/deepllm/prompters.py
+-rw-r--r--   0 tarau      (503) staff       (20)     4061 2024-02-26 23:53:37.000000 deepllm-1.4.3/deepllm/questmaker.py
+-rw-r--r--   0 tarau      (503) staff       (20)    10784 2024-03-25 00:48:51.000000 deepllm-1.4.3/deepllm/recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     6758 2024-04-07 20:07:59.000000 deepllm-1.4.3/deepllm/refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-03-22 20:57:32.000000 deepllm-1.4.3/deepllm/requirements.txt
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-07 21:27:30.430786 deepllm-1.4.3/deepllm/tests/
+-rw-r--r--   0 tarau      (503) staff       (20)      126 2023-07-08 20:37:56.000000 deepllm-1.4.3/deepllm/tests/README.md
+-rw-r--r--   0 tarau      (503) staff       (20)        0 2023-07-02 23:51:45.000000 deepllm-1.4.3/deepllm/tests/__init__.py
+-rwxr-xr-x   0 tarau      (503) staff       (20)      596 2024-03-15 13:54:55.000000 deepllm-1.4.3/deepllm/tests/test_all.py
+-rw-r--r--   0 tarau      (503) staff       (20)      906 2023-08-13 18:57:17.000000 deepllm-1.4.3/deepllm/tests/test_api.py
+-rw-r--r--   0 tarau      (503) staff       (20)      381 2023-07-15 20:32:09.000000 deepllm-1.4.3/deepllm/tests/test_configurator.py
+-rw-r--r--   0 tarau      (503) staff       (20)      526 2024-03-16 00:51:59.000000 deepllm-1.4.3/deepllm/tests/test_embedders.py
+-rw-r--r--   0 tarau      (503) staff       (20)      100 2023-07-03 00:38:48.000000 deepllm-1.4.3/deepllm/tests/test_horn_prover.py
+-rw-r--r--   0 tarau      (503) staff       (20)      499 2023-07-19 14:10:18.000000 deepllm-1.4.3/deepllm/tests/test_interactors.py
+-rw-r--r--   0 tarau      (503) staff       (20)      294 2023-07-03 05:58:15.000000 deepllm-1.4.3/deepllm/tests/test_params.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1216 2024-01-29 22:45:46.000000 deepllm-1.4.3/deepllm/tests/test_recursors.py
+-rw-r--r--   0 tarau      (503) staff       (20)     2284 2023-07-08 20:38:27.000000 deepllm-1.4.3/deepllm/tests/test_refiners.py
+-rw-r--r--   0 tarau      (503) staff       (20)     1287 2023-12-28 01:58:47.000000 deepllm-1.4.3/deepllm/tools.py
+-rw-r--r--   0 tarau      (503) staff       (20)      882 2024-03-22 20:43:06.000000 deepllm-1.4.3/deepllm/vis.py
+drwxr-xr-x   0 tarau      (503) staff       (20)        0 2024-04-07 21:27:30.415175 deepllm-1.4.3/deepllm.egg-info/
+-rw-r--r--   0 tarau      (503) staff       (20)     4651 2024-04-07 21:27:30.000000 deepllm-1.4.3/deepllm.egg-info/PKG-INFO
+-rw-r--r--   0 tarau      (503) staff       (20)     1319 2024-04-07 21:27:30.000000 deepllm-1.4.3/deepllm.egg-info/SOURCES.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-07 21:27:30.000000 deepllm-1.4.3/deepllm.egg-info/dependency_links.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        1 2024-04-07 21:27:30.000000 deepllm-1.4.3/deepllm.egg-info/not-zip-safe
+-rw-r--r--   0 tarau      (503) staff       (20)       59 2024-04-07 21:27:30.000000 deepllm-1.4.3/deepllm.egg-info/requires.txt
+-rw-r--r--   0 tarau      (503) staff       (20)        8 2024-04-07 21:27:30.000000 deepllm-1.4.3/deepllm.egg-info/top_level.txt
+-rw-r--r--   0 tarau      (503) staff       (20)       38 2024-04-07 21:27:30.431978 deepllm-1.4.3/setup.cfg
+-rw-r--r--   0 tarau      (503) staff       (20)      967 2023-11-08 02:45:22.000000 deepllm-1.4.3/setup.py
```

### Comparing `deepllm-1.4.2/LICENSE` & `deepllm-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/PKG-INFO` & `deepllm-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.4.2
+Version: 1.4.3
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.4.2/README.md` & `deepllm-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/api.py` & `deepllm-1.4.3/deepllm/api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/apps/app.py` & `deepllm-1.4.3/deepllm/apps/app.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/apps/rel_graph.html` & `deepllm-1.4.3/deepllm/apps/rel_graph.html`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/configurator.py` & `deepllm-1.4.3/deepllm/configurator.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/demos/demo.py` & `deepllm-1.4.3/deepllm/demos/demo.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/demos/viz.py` & `deepllm-1.4.3/deepllm/demos/viz.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/horn_prover.py` & `deepllm-1.4.3/deepllm/horn_prover.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/interactors.py` & `deepllm-1.4.3/deepllm/interactors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/local_llms/local_runs.py` & `deepllm-1.4.3/deepllm/local_llms/local_runs.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/local_llms/test_vicuna.py` & `deepllm-1.4.3/deepllm/local_llms/test_vicuna.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/params.py` & `deepllm-1.4.3/deepllm/params.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/prompters.py` & `deepllm-1.4.3/deepllm/prompters.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,32 +143,34 @@
     """
 )
 
 summary_maker = dict(
     name='summary_maker',
     sum_p="""
     You are an expert in understanding documents and summarizing them.
-    Make a summary of $sum_size sentences and extract $kwd_count keyphrases from the following text.
+    First, make a summary of $sum_size sentences. Start the summary with "Summary:". 
+    Next, extract $kwd_count keywords separated by ";".
+    
+    Here is the text to work with:
        
-    $text 
+    $text   
     """
 )
 
 paper_reviewer = dict(
     name='paper_reviewer',
     rev_p="""
     You are an expert in in the research field of the following scientific paper given to you by a colleague who needs honest feedback about the strength and the weaknesses of the paper.
     Make a thorough and detailed review of the paper and recommend improvements to it, based on your extensive expertise in its research field.
     Here is the text of the paper.
 
     $text 
     """
 )
 
-
 retrieval_refiner = dict(
     name='retrieval_refiner',
     rev_p="""
     You are given a text containing sentences extracted from a document, all related to a question "$quest?" .
     Read the text carefully with the question in mind.
      
     Here is the text of the paper, ending with ||.
@@ -187,15 +189,14 @@
     No explanations needed, return just the hypernym as a string.
     Here is the text:
 
     "$g"
     """
 )
 
-
 sci_abstract_maker = dict(
     name='title_and_abstract_maker',
     writer_p="""
     Suggest a title and an abstract for a scientific paper about "$g" that has the following keywords: $context.
     """
 )
 
@@ -217,13 +218,14 @@
     causal_prompter,
     task_planning_prompter,
     recommendation_prompter,
     thesis_support_prompter,
     cons_and_pros_prompter
 ]
 
+
 def prompter_dict():
     d = dict()
     for prompter in prompter_vars:
         name = prompter['name']
         d[name] = prompter
     return d
```

### Comparing `deepllm-1.4.2/deepllm/questmaker.py` & `deepllm-1.4.3/deepllm/questmaker.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/recursors.py` & `deepllm-1.4.3/deepllm/recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/refiners.py` & `deepllm-1.4.3/deepllm/refiners.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,14 +174,17 @@
     def run(self):
         answer = self.agent.ask(
             text=self.text,
             sum_size=self.sum_size,
             kwd_count=self.kwd_count
         )
         if self.cache: self.agent.persist()
+        print("\n\nANSWER:----------\n")
+        print(answer)
+        print('------\n\n')
         return str(answer)
 
 
 class PaperReviewer:
     def __init__(self, text, tname=None, cache=True):
         self.text = text
         self.cache = cache
```

### Comparing `deepllm-1.4.2/deepllm/tests/test_all.py` & `deepllm-1.4.3/deepllm/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/tests/test_api.py` & `deepllm-1.4.3/deepllm/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/tests/test_embedders.py` & `deepllm-1.4.3/deepllm/tests/test_embedders.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/tests/test_recursors.py` & `deepllm-1.4.3/deepllm/tests/test_recursors.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/tests/test_refiners.py` & `deepllm-1.4.3/deepllm/tests/test_refiners.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/tools.py` & `deepllm-1.4.3/deepllm/tools.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm/vis.py` & `deepllm-1.4.3/deepllm/vis.py`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/deepllm.egg-info/PKG-INFO` & `deepllm-1.4.3/deepllm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepllm
-Version: 1.4.2
+Version: 1.4.3
 Summary: Deep, recursive, goal-driven LLM explorer
 Home-page: https://github.com/ptarau/recursors.git
 Author: Paul Tarau
 Author-email: paul.tarau@gmail.com
 License: GPL-3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deepllm-1.4.2/deepllm.egg-info/SOURCES.txt` & `deepllm-1.4.3/deepllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepllm-1.4.2/setup.py` & `deepllm-1.4.3/setup.py`

 * *Files identical despite different names*

