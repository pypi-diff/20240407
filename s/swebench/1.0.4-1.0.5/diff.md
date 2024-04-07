# Comparing `tmp/swebench-1.0.4.tar.gz` & `tmp/swebench-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swebench-1.0.4.tar", last modified: Fri Apr  5 23:38:06 2024, max compression
+gzip compressed data, was "swebench-1.0.5.tar", last modified: Sun Apr  7 16:27:19 2024, max compression
```

## Comparing `swebench-1.0.4.tar` & `swebench-1.0.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.956869 swebench-1.0.4/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.4/LICENSE
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-05 23:38:06.956811 swebench-1.0.4/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.4/README.md
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.949287 swebench-1.0.4/inference/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.949728 swebench-1.0.4/inference/llamao/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/llamao/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/llamao/distributed_attention.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/llamao/modeling_flash_llama.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.950815 swebench-1.0.4/inference/make_datasets/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/make_datasets/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/bm25_retrieval.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/make_datasets/create_instance.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/create_text_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/eval_retrieval.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/tokenize_dataset.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.4/inference/make_datasets/utils.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.4/inference/run_api.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.4/inference/run_live.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.4/inference/run_llama.py
--rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.4/pyproject.toml
--rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-05 23:38:06.957064 swebench-1.0.4/setup.cfg
--rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.4/setup.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.950983 swebench-1.0.4/swebench/
--rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-05 23:37:51.000000 swebench-1.0.4/swebench/__init__.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.952393 swebench-1.0.4/swebench/collect/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/__init__.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/build_dataset.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/build_dataset_ft.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/get_tasks_pipeline.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/get_top_pypi.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/print_pulls.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/collect/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.953891 swebench-1.0.4/swebench/harness/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/harness/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    18858 2024-04-05 22:22:32.000000 swebench-1.0.4/swebench/harness/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    30665 2024-04-05 19:15:08.000000 swebench-1.0.4/swebench/harness/context_manager.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/harness/engine_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/harness/engine_validation.py
--rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.4/swebench/harness/run_evaluation.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.4/swebench/harness/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.955726 swebench-1.0.4/swebench/metrics/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/conversion.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.4/swebench/metrics/getters.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     5932 2024-04-04 17:22:14.000000 swebench-1.0.4/swebench/metrics/log_parsers.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/metrics.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/metrics/monitor.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.4/swebench/metrics/report.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.956405 swebench-1.0.4/swebench/versioning/
--rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/__init__.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/constants.py
--rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/get_versions.py
--rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.4/swebench/versioning/utils.py
-drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-05 23:38:06.956564 swebench-1.0.4/swebench.egg-info/
--rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/PKG-INFO
--rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/SOURCES.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/dependency_links.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/requires.txt
--rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-05 23:38:06.000000 swebench-1.0.4/swebench.egg-info/top_level.txt
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.560950 swebench-1.0.5/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1159 2024-04-02 05:16:15.000000 swebench-1.0.5/LICENSE
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-07 16:27:19.560882 swebench-1.0.5/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     5352 2024-04-05 18:50:18.000000 swebench-1.0.5/README.md
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.554256 swebench-1.0.5/inference/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.554738 swebench-1.0.5/inference/llamao/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/llamao/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2491 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/llamao/distributed_attention.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    37884 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/llamao/modeling_flash_llama.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.555910 swebench-1.0.5/inference/make_datasets/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/make_datasets/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18785 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/bm25_retrieval.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14957 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/make_datasets/create_instance.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     8534 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/create_text_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2618 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/eval_retrieval.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     7717 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/tokenize_dataset.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10607 2024-03-19 11:00:02.000000 swebench-1.0.5/inference/make_datasets/utils.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    19671 2024-03-28 15:18:33.000000 swebench-1.0.5/inference/run_api.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10090 2024-03-28 15:18:33.000000 swebench-1.0.5/inference/run_live.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15798 2024-03-14 17:15:25.000000 swebench-1.0.5/inference/run_llama.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)       84 2024-04-02 05:16:15.000000 swebench-1.0.5/pyproject.toml
+-rw-r--r--   0 johnbyang   (501) staff       (20)      111 2024-04-07 16:27:19.561147 swebench-1.0.5/setup.cfg
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1329 2024-04-02 05:16:15.000000 swebench-1.0.5/setup.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.556096 swebench-1.0.5/swebench/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1691 2024-04-07 16:27:14.000000 swebench-1.0.5/swebench/__init__.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.557600 swebench-1.0.5/swebench/collect/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/__init__.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     6693 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/build_dataset.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     2677 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/build_dataset_ft.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     4633 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/get_tasks_pipeline.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     3671 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/get_top_pypi.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)     1751 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/print_pulls.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14635 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/collect/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.558698 swebench-1.0.5/swebench/harness/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/harness/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    18858 2024-04-05 22:22:32.000000 swebench-1.0.5/swebench/harness/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    30665 2024-04-05 19:15:08.000000 swebench-1.0.5/swebench/harness/context_manager.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7478 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/harness/engine_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6331 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/harness/engine_validation.py
+-rwxr-xr-x   0 johnbyang   (501) staff       (20)    10392 2024-04-02 13:57:05.000000 swebench-1.0.5/swebench/harness/run_evaluation.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    14702 2024-04-05 20:21:29.000000 swebench-1.0.5/swebench/harness/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.559791 swebench-1.0.5/swebench/metrics/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)      730 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2178 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/conversion.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4625 2024-04-02 13:57:05.000000 swebench-1.0.5/swebench/metrics/getters.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     7097 2024-04-07 16:01:31.000000 swebench-1.0.5/swebench/metrics/log_parsers.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2829 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/metrics.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     4338 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/metrics/monitor.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    10931 2024-04-02 13:57:05.000000 swebench-1.0.5/swebench/metrics/report.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.560469 swebench-1.0.5/swebench/versioning/
+-rw-r--r--   0 johnbyang   (501) staff       (20)        0 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/__init__.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     2214 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/constants.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)    15492 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/get_versions.py
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1221 2024-04-02 05:16:15.000000 swebench-1.0.5/swebench/versioning/utils.py
+drwxr-xr-x   0 johnbyang   (501) staff       (20)        0 2024-04-07 16:27:19.560638 swebench-1.0.5/swebench.egg-info/
+-rw-r--r--   0 johnbyang   (501) staff       (20)     6408 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/PKG-INFO
+-rw-r--r--   0 johnbyang   (501) staff       (20)     1543 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/SOURCES.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)        1 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/dependency_links.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       76 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/requires.txt
+-rw-r--r--   0 johnbyang   (501) staff       (20)       19 2024-04-07 16:27:19.000000 swebench-1.0.5/swebench.egg-info/top_level.txt
```

### Comparing `swebench-1.0.4/LICENSE` & `swebench-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/PKG-INFO` & `swebench-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.4
+Version: 1.0.5
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.4 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.5 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.4/README.md` & `swebench-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/llamao/distributed_attention.py` & `swebench-1.0.5/inference/llamao/distributed_attention.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/llamao/modeling_flash_llama.py` & `swebench-1.0.5/inference/llamao/modeling_flash_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/make_datasets/bm25_retrieval.py` & `swebench-1.0.5/inference/make_datasets/bm25_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/make_datasets/create_instance.py` & `swebench-1.0.5/inference/make_datasets/create_instance.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/make_datasets/create_text_dataset.py` & `swebench-1.0.5/inference/make_datasets/create_text_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/make_datasets/eval_retrieval.py` & `swebench-1.0.5/inference/make_datasets/eval_retrieval.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/make_datasets/tokenize_dataset.py` & `swebench-1.0.5/inference/make_datasets/tokenize_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/make_datasets/utils.py` & `swebench-1.0.5/inference/make_datasets/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/run_api.py` & `swebench-1.0.5/inference/run_api.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/run_live.py` & `swebench-1.0.5/inference/run_live.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/inference/run_llama.py` & `swebench-1.0.5/inference/run_llama.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/setup.py` & `swebench-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/__init__.py` & `swebench-1.0.5/swebench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 
 from swebench.collect.build_dataset import main as build_dataset
 from swebench.collect.get_tasks_pipeline import main as get_tasks_pipeline
 from swebench.collect.print_pulls import main as print_pulls
 
 from swebench.harness.constants import (
     KEY_INSTANCE_ID,
```

### Comparing `swebench-1.0.4/swebench/collect/build_dataset.py` & `swebench-1.0.5/swebench/collect/build_dataset.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/collect/build_dataset_ft.py` & `swebench-1.0.5/swebench/collect/build_dataset_ft.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/collect/get_tasks_pipeline.py` & `swebench-1.0.5/swebench/collect/get_tasks_pipeline.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/collect/get_top_pypi.py` & `swebench-1.0.5/swebench/collect/get_top_pypi.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/collect/print_pulls.py` & `swebench-1.0.5/swebench/collect/print_pulls.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/collect/utils.py` & `swebench-1.0.5/swebench/collect/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/harness/constants.py` & `swebench-1.0.5/swebench/harness/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/harness/context_manager.py` & `swebench-1.0.5/swebench/harness/context_manager.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/harness/engine_evaluation.py` & `swebench-1.0.5/swebench/harness/engine_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/harness/engine_validation.py` & `swebench-1.0.5/swebench/harness/engine_validation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/harness/run_evaluation.py` & `swebench-1.0.5/swebench/harness/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/harness/utils.py` & `swebench-1.0.5/swebench/harness/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/metrics/constants.py` & `swebench-1.0.5/swebench/metrics/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/metrics/conversion.py` & `swebench-1.0.5/swebench/metrics/conversion.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/metrics/getters.py` & `swebench-1.0.5/swebench/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/metrics/log_parsers.py` & `swebench-1.0.5/swebench/metrics/log_parsers.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,45 @@
             test_case = line.split()
             if len(test_case) <= 1:
                 continue
             test_status_map[test_case[1]] = test_case[0]
     return test_status_map
 
 
+def parse_log_pytest_options(log: str) -> dict:
+    """
+    Parser for test logs generated with PyTest framework with options
+
+    Args:
+        log (str): log content
+    Returns:
+        dict: test case to test status mapping
+    """
+    option_pattern = re.compile(r'(.*?)\[(.*)\]')
+    test_status_map = {}
+    for line in log.split("\n"):
+        if any([line.startswith(x.value) for x in TestStatus]):
+            # Additional parsing for FAILED status
+            if line.startswith(TestStatus.FAILED.value):
+                line = line.replace(" - ", " ")
+            test_case = line.split()
+            if len(test_case) <= 1:
+                continue
+            has_option = option_pattern.search(test_case[1])
+            if has_option:
+                main, option = has_option.groups()
+                if option.startswith('/') and not option.startswith('//') and '*' not in option:
+                    option = option.split('/')[-1]
+                test_name = f'{main}[/{option}]'
+            else:
+                test_name = test_case[1]
+            test_status_map[test_name] = test_case[0]
+    return test_status_map
+
+
 def parse_log_django(log: str) -> dict:
     """
     Parser for test logs generated with Django tester framework
 
     Args:
         log (str): log content
     Returns:
@@ -138,22 +169,23 @@
     return test_status_map
 
 
 parse_log_astroid = parse_log_pytest
 parse_log_flask = parse_log_pytest
 parse_log_marshmallow = parse_log_pytest
 parse_log_matplotlib = parse_log_pytest
-parse_log_pydicom = parse_log_pytest
 parse_log_pvlib = parse_log_pytest
-parse_log_pylint = parse_log_pytest
 parse_log_pyvista = parse_log_pytest
-parse_log_requests = parse_log_pytest
 parse_log_sqlfluff = parse_log_pytest
 parse_log_xarray = parse_log_pytest
 
+parse_log_pydicom = parse_log_pytest_options
+parse_log_requests = parse_log_pytest_options
+parse_log_pylint = parse_log_pytest_options
+
 parse_log_astropy = parse_log_pytest_v2
 parse_log_scikit = parse_log_pytest_v2
 parse_log_sphinx = parse_log_pytest_v2
 
 
 MAP_REPO_TO_PARSER = {
     "astropy/astropy": parse_log_astropy,
```

### Comparing `swebench-1.0.4/swebench/metrics/metrics.py` & `swebench-1.0.5/swebench/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/metrics/monitor.py` & `swebench-1.0.5/swebench/metrics/monitor.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/metrics/report.py` & `swebench-1.0.5/swebench/metrics/report.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/versioning/constants.py` & `swebench-1.0.5/swebench/versioning/constants.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/versioning/get_versions.py` & `swebench-1.0.5/swebench/versioning/get_versions.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench/versioning/utils.py` & `swebench-1.0.5/swebench/versioning/utils.py`

 * *Files identical despite different names*

### Comparing `swebench-1.0.4/swebench.egg-info/PKG-INFO` & `swebench-1.0.5/swebench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swebench
-Version: 1.0.4
+Version: 1.0.5
 Summary: The official SWE-bench package - a benchmark for evaluating LMs on software engineering
 Home-page: https://swebench.com
 Author: John Yang
 Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench
 Project-URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues
 Project-URL: Source Code, http://github.com/princeton-nlp/SWE-bench
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: swebench Version: 1.0.4 Summary: The official SWE-
+Metadata-Version: 2.1 Name: swebench Version: 1.0.5 Summary: The official SWE-
 bench package - a benchmark for evaluating LMs on software engineering Home-
 page: https://swebench.com Author: John Yang Author-email: byjohnyang@gmail.com
 Project-URL: Documentation, https://github.com/princeton-nlp/SWE-bench Project-
 URL: Bug Reports, http://github.com/princeton-nlp/SWE-bench/issues Project-URL:
 Source Code, http://github.com/princeton-nlp/SWE-bench Project-URL: Website,
 https://swebench.com Keywords: nlp,benchmark,code Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `swebench-1.0.4/swebench.egg-info/SOURCES.txt` & `swebench-1.0.5/swebench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

