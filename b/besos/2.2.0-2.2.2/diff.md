# Comparing `tmp/besos-2.2.0.tar.gz` & `tmp/besos-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "besos-2.2.0.tar", last modified: Tue Oct 31 03:07:45 2023, max compression
+gzip compressed data, was "besos-2.2.2.tar", last modified: Sat Apr  6 22:16:19 2024, max compression
```

## Comparing `besos-2.2.0.tar` & `besos-2.2.2.tar`

### file list

```diff
@@ -1,83 +1,84 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-10-31 03:07:45.649367 besos-2.2.0/
--rw-r--r--   0 user      (1000) user      (1000)    35069 2023-09-02 17:28:20.000000 besos-2.2.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)       12 2023-09-02 17:28:20.000000 besos-2.2.0/MANIFEST.in
--rw-r--r--   0 user      (1000) user      (1000)     8426 2023-10-31 03:07:45.646367 besos-2.2.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     6475 2023-09-02 17:28:20.000000 besos-2.2.0/README.md
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-10-31 03:07:45.317365 besos-2.2.0/besos/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-10-31 03:07:45.366365 besos-2.2.0/besos/.ipynb_checkpoints/
--rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.0/besos/.ipynb_checkpoints/config-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    11982 2023-09-02 19:14:29.000000 besos-2.2.0/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.0/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    35684 2023-10-30 00:44:53.000000 besos-2.2.0/besos/.ipynb_checkpoints/evaluator-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.0/besos/.ipynb_checkpoints/parameters-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)     4719 2023-10-30 00:54:36.000000 besos-2.2.0/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    23926 2023-09-02 19:14:36.000000 besos-2.2.0/besos/.ipynb_checkpoints/sampling-checkpoint.py
--rw-r--r--   0 user      (1000) user      (1000)    17589 2023-09-02 17:28:20.000000 besos-2.2.0/besos/IDF_class.py
--rw-r--r--   0 user      (1000) user      (1000)     4818 2023-09-02 17:28:20.000000 besos-2.2.0/besos/IO_Objects.py
--rw-r--r--   0 user      (1000) user      (1000)       98 2023-09-02 17:28:20.000000 besos-2.2.0/besos/__init__.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-10-31 03:07:45.437366 besos-2.2.0/besos/__pycache__/
--rw-r--r--   0 user      (1000) user      (1000)    14604 2023-09-02 18:23:33.000000 besos-2.2.0/besos/__pycache__/IDF_class.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     6844 2023-09-02 18:23:33.000000 besos-2.2.0/besos/__pycache__/IO_Objects.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      250 2023-09-02 18:23:09.000000 besos-2.2.0/besos/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      995 2023-09-02 18:24:32.000000 besos-2.2.0/besos/__pycache__/besos_utils.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      397 2023-09-02 18:23:33.000000 besos-2.2.0/besos/__pycache__/besostypes.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     1657 2023-09-02 18:23:33.000000 besos-2.2.0/besos/__pycache__/config.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      402 2023-09-02 18:49:25.000000 besos-2.2.0/besos/__pycache__/dask_utils.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     8826 2023-10-29 18:10:49.000000 besos-2.2.0/besos/__pycache__/eplus_funcs.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    21973 2023-09-02 18:23:09.000000 besos-2.2.0/besos/__pycache__/eppy_funcs.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     1769 2023-09-02 18:23:33.000000 besos-2.2.0/besos/__pycache__/errors.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    29998 2023-10-30 00:48:27.000000 besos-2.2.0/besos/__pycache__/evaluator.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    15992 2023-10-29 18:10:48.000000 besos-2.2.0/besos/__pycache__/objectives.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    12215 2023-09-02 18:49:25.000000 besos-2.2.0/besos/__pycache__/optimizer.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    22598 2023-10-29 18:10:50.000000 besos-2.2.0/besos/__pycache__/parameters.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    14204 2023-09-02 18:24:32.000000 besos-2.2.0/besos/__pycache__/problem.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)     2987 2023-10-30 01:00:11.000000 besos-2.2.0/besos/__pycache__/pyehub_funcs.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    16306 2023-09-02 19:33:27.000000 besos-2.2.0/besos/__pycache__/sampling.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)    17484 2023-09-02 18:55:05.000000 besos-2.2.0/besos/__pycache__/weather.cpython-38.pyc
--rw-r--r--   0 user      (1000) user      (1000)      761 2023-09-02 17:28:20.000000 besos-2.2.0/besos/besos_utils.py
--rw-r--r--   0 user      (1000) user      (1000)      272 2023-09-02 17:28:20.000000 besos-2.2.0/besos/besostypes.py
--rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.0/besos/config.py
--rw-r--r--   0 user      (1000) user      (1000)      221 2023-09-02 17:28:20.000000 besos-2.2.0/besos/dask_utils.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-10-31 03:07:45.586367 besos-2.2.0/besos/data/
--rw-r--r--   0 user      (1000) user      (1000)  4378096 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/Custom_Long_Fields.idd
--rw-r--r--   0 user      (1000) user      (1000)  9591568 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/Energy+.schema.epJSON
--rw-r--r--   0 user      (1000) user      (1000)   230178 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/example_bad_idf.idf
--rw-r--r--   0 user      (1000) user      (1000)   293683 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/example_building.epJSON
--rw-r--r--   0 user      (1000) user      (1000)  1639985 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/example_epw.epw
--rw-r--r--   0 user      (1000) user      (1000)  4364459 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/example_idd.idd
--rw-r--r--   0 user      (1000) user      (1000)   230171 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/example_idf.idf
--rw-r--r--   0 user      (1000) user      (1000)    38772 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/example_xlsx.xlsx
--rw-r--r--   0 user      (1000) user      (1000)    83738 2023-09-02 17:28:20.000000 besos-2.2.0/besos/data/unexpanded.idf
--rw-r--r--   0 user      (1000) user      (1000)    11982 2023-10-29 18:07:36.000000 besos-2.2.0/besos/eplus_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.0/besos/eppy_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)     1564 2023-09-02 17:28:20.000000 besos-2.2.0/besos/errors.py
--rw-r--r--   0 user      (1000) user      (1000)    35685 2023-10-31 03:04:31.000000 besos-2.2.0/besos/evaluator.py
--rw-r--r--   0 user      (1000) user      (1000)     4223 2023-09-02 17:28:20.000000 besos-2.2.0/besos/example_ui.py
--rw-r--r--   0 user      (1000) user      (1000)    19196 2023-10-29 18:07:36.000000 besos-2.2.0/besos/objectives.py
--rw-r--r--   0 user      (1000) user      (1000)    15486 2023-09-02 17:28:20.000000 besos-2.2.0/besos/optimizer.py
--rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.0/besos/parameters.py
--rw-r--r--   0 user      (1000) user      (1000)    16842 2023-09-02 17:28:20.000000 besos-2.2.0/besos/problem.py
--rw-r--r--   0 user      (1000) user      (1000)     4719 2023-10-31 03:04:31.000000 besos-2.2.0/besos/pyehub_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)    23926 2023-09-02 19:14:36.000000 besos-2.2.0/besos/sampling.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-10-31 03:07:45.338365 besos-2.2.0/besos.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     8426 2023-10-31 03:07:45.000000 besos-2.2.0/besos.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)     2258 2023-10-31 03:07:45.000000 besos-2.2.0/besos.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-10-31 03:07:45.000000 besos-2.2.0/besos.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)      384 2023-10-31 03:07:45.000000 besos-2.2.0/besos.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)        6 2023-10-31 03:07:45.000000 besos-2.2.0/besos.egg-info/top_level.txt
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-10-31 03:07:45.650367 besos-2.2.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)     1183 2023-10-31 03:04:31.000000 besos-2.2.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-10-31 03:07:45.635367 besos-2.2.0/test/
--rw-r--r--   0 user      (1000) user      (1000)     3327 2023-10-30 00:59:47.000000 besos-2.2.0/test/test_adaptive_surrogate.py
--rw-r--r--   0 user      (1000) user      (1000)     1300 2023-09-02 17:28:21.000000 besos-2.2.0/test/test_eplus_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)     2884 2023-10-31 03:04:31.000000 besos-2.2.0/test/test_eppy_funcs.py
--rw-r--r--   0 user      (1000) user      (1000)     6710 2023-10-29 18:07:37.000000 besos-2.2.0/test/test_error_handling.py
--rw-r--r--   0 user      (1000) user      (1000)    12856 2023-10-31 03:04:31.000000 besos-2.2.0/test/test_evaluators.py
--rw-r--r--   0 user      (1000) user      (1000)     2522 2023-09-02 17:28:21.000000 besos-2.2.0/test/test_fit_surrogate.py
--rw-r--r--   0 user      (1000) user      (1000)     1642 2023-10-29 18:07:37.000000 besos-2.2.0/test/test_mixed_optimisation.py
--rw-r--r--   0 user      (1000) user      (1000)     3121 2023-09-02 17:28:21.000000 besos-2.2.0/test/test_objectives_constraints.py
--rw-r--r--   0 user      (1000) user      (1000)     7785 2023-10-29 18:07:37.000000 besos-2.2.0/test/test_parameter.py
--rw-r--r--   0 user      (1000) user      (1000)     3052 2023-10-29 18:07:37.000000 besos-2.2.0/test/test_platypus.py
--rw-r--r--   0 user      (1000) user      (1000)     1182 2023-10-29 18:07:37.000000 besos-2.2.0/test/test_rbfopt.py
--rw-r--r--   0 user      (1000) user      (1000)     4687 2023-09-02 17:28:21.000000 besos-2.2.0/test/test_selectors.py
--rw-r--r--   0 user      (1000) user      (1000)     3711 2023-09-02 19:14:36.000000 besos-2.2.0/test/test_simulation.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.434650 besos-2.2.2/
+-rw-r--r--   0 user      (1000) user      (1000)    35069 2023-09-02 17:28:20.000000 besos-2.2.2/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)       12 2023-09-02 17:28:20.000000 besos-2.2.2/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)     8426 2024-04-06 22:16:19.431650 besos-2.2.2/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     6475 2023-09-02 17:28:20.000000 besos-2.2.2/README.md
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.142648 besos-2.2.2/besos/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.190648 besos-2.2.2/besos/.ipynb_checkpoints/
+-rw-r--r--   0 user      (1000) user      (1000)      761 2023-09-02 17:28:20.000000 besos-2.2.2/besos/.ipynb_checkpoints/besos_utils-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.2/besos/.ipynb_checkpoints/config-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    11982 2023-09-02 19:14:29.000000 besos-2.2.2/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.2/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    35684 2023-10-30 00:44:53.000000 besos-2.2.2/besos/.ipynb_checkpoints/evaluator-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.2/besos/.ipynb_checkpoints/parameters-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)     4719 2023-10-30 00:54:36.000000 besos-2.2.2/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    23926 2023-09-02 19:14:36.000000 besos-2.2.2/besos/.ipynb_checkpoints/sampling-checkpoint.py
+-rw-r--r--   0 user      (1000) user      (1000)    17589 2023-09-02 17:28:20.000000 besos-2.2.2/besos/IDF_class.py
+-rw-r--r--   0 user      (1000) user      (1000)     4818 2023-09-02 17:28:20.000000 besos-2.2.2/besos/IO_Objects.py
+-rw-r--r--   0 user      (1000) user      (1000)       98 2023-09-02 17:28:20.000000 besos-2.2.2/besos/__init__.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.255648 besos-2.2.2/besos/__pycache__/
+-rw-r--r--   0 user      (1000) user      (1000)    14604 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/IDF_class.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     6844 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/IO_Objects.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      250 2023-09-02 18:23:09.000000 besos-2.2.2/besos/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      995 2023-09-02 18:24:32.000000 besos-2.2.2/besos/__pycache__/besos_utils.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      397 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/besostypes.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1657 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/config.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      402 2023-09-02 18:49:25.000000 besos-2.2.2/besos/__pycache__/dask_utils.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     8826 2023-10-29 18:10:49.000000 besos-2.2.2/besos/__pycache__/eplus_funcs.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    21973 2023-09-02 18:23:09.000000 besos-2.2.2/besos/__pycache__/eppy_funcs.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     1769 2023-09-02 18:23:33.000000 besos-2.2.2/besos/__pycache__/errors.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    29998 2023-10-31 06:10:03.000000 besos-2.2.2/besos/__pycache__/evaluator.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    15992 2023-10-29 18:10:48.000000 besos-2.2.2/besos/__pycache__/objectives.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    12215 2023-09-02 18:49:25.000000 besos-2.2.2/besos/__pycache__/optimizer.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    22598 2023-10-29 18:10:50.000000 besos-2.2.2/besos/__pycache__/parameters.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    14204 2023-09-02 18:24:32.000000 besos-2.2.2/besos/__pycache__/problem.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)     2987 2023-10-31 06:09:41.000000 besos-2.2.2/besos/__pycache__/pyehub_funcs.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    16306 2023-09-02 19:33:27.000000 besos-2.2.2/besos/__pycache__/sampling.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)    17484 2023-09-02 18:55:05.000000 besos-2.2.2/besos/__pycache__/weather.cpython-38.pyc
+-rw-r--r--   0 user      (1000) user      (1000)      761 2023-09-02 17:28:20.000000 besos-2.2.2/besos/besos_utils.py
+-rw-r--r--   0 user      (1000) user      (1000)      272 2023-09-02 17:28:20.000000 besos-2.2.2/besos/besostypes.py
+-rw-r--r--   0 user      (1000) user      (1000)     2824 2023-09-02 17:28:20.000000 besos-2.2.2/besos/config.py
+-rw-r--r--   0 user      (1000) user      (1000)      221 2023-09-02 17:28:20.000000 besos-2.2.2/besos/dask_utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.384650 besos-2.2.2/besos/data/
+-rw-r--r--   0 user      (1000) user      (1000)  4378096 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/Custom_Long_Fields.idd
+-rw-r--r--   0 user      (1000) user      (1000)  9591568 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/Energy+.schema.epJSON
+-rw-r--r--   0 user      (1000) user      (1000)   230178 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_bad_idf.idf
+-rw-r--r--   0 user      (1000) user      (1000)   293683 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_building.epJSON
+-rw-r--r--   0 user      (1000) user      (1000)  1639985 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_epw.epw
+-rw-r--r--   0 user      (1000) user      (1000)  4364459 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_idd.idd
+-rw-r--r--   0 user      (1000) user      (1000)   230171 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_idf.idf
+-rw-r--r--   0 user      (1000) user      (1000)    38772 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/example_xlsx.xlsx
+-rw-r--r--   0 user      (1000) user      (1000)    83738 2023-09-02 17:28:20.000000 besos-2.2.2/besos/data/unexpanded.idf
+-rw-r--r--   0 user      (1000) user      (1000)    11982 2023-10-29 18:07:36.000000 besos-2.2.2/besos/eplus_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)    28138 2023-09-02 17:28:20.000000 besos-2.2.2/besos/eppy_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)     1564 2023-09-02 17:28:20.000000 besos-2.2.2/besos/errors.py
+-rw-r--r--   0 user      (1000) user      (1000)    35617 2024-04-06 22:09:53.000000 besos-2.2.2/besos/evaluator.py
+-rw-r--r--   0 user      (1000) user      (1000)     4223 2023-09-02 17:28:20.000000 besos-2.2.2/besos/example_ui.py
+-rw-r--r--   0 user      (1000) user      (1000)    19371 2024-04-06 22:09:53.000000 besos-2.2.2/besos/objectives.py
+-rw-r--r--   0 user      (1000) user      (1000)    15486 2023-09-02 17:28:20.000000 besos-2.2.2/besos/optimizer.py
+-rw-r--r--   0 user      (1000) user      (1000)    23107 2023-10-29 18:07:36.000000 besos-2.2.2/besos/parameters.py
+-rw-r--r--   0 user      (1000) user      (1000)    16842 2023-09-02 17:28:20.000000 besos-2.2.2/besos/problem.py
+-rw-r--r--   0 user      (1000) user      (1000)     4579 2024-04-06 22:09:53.000000 besos-2.2.2/besos/pyehub_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)    23926 2023-09-02 19:14:36.000000 besos-2.2.2/besos/sampling.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.419650 besos-2.2.2/besos.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     8426 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)     2309 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)      384 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)        6 2024-04-06 22:16:19.000000 besos-2.2.2/besos.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2024-04-06 22:16:19.434650 besos-2.2.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1183 2024-04-06 22:09:53.000000 besos-2.2.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2024-04-06 22:16:19.416650 besos-2.2.2/test/
+-rw-r--r--   0 user      (1000) user      (1000)     3327 2023-10-30 00:59:47.000000 besos-2.2.2/test/test_adaptive_surrogate.py
+-rw-r--r--   0 user      (1000) user      (1000)     1300 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_eplus_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)     2884 2023-10-31 03:04:31.000000 besos-2.2.2/test/test_eppy_funcs.py
+-rw-r--r--   0 user      (1000) user      (1000)     6710 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_error_handling.py
+-rw-r--r--   0 user      (1000) user      (1000)    12856 2023-10-31 03:04:31.000000 besos-2.2.2/test/test_evaluators.py
+-rw-r--r--   0 user      (1000) user      (1000)     2522 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_fit_surrogate.py
+-rw-r--r--   0 user      (1000) user      (1000)     1642 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_mixed_optimisation.py
+-rw-r--r--   0 user      (1000) user      (1000)     3121 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_objectives_constraints.py
+-rw-r--r--   0 user      (1000) user      (1000)     7785 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_parameter.py
+-rw-r--r--   0 user      (1000) user      (1000)     3052 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_platypus.py
+-rw-r--r--   0 user      (1000) user      (1000)     1182 2023-10-29 18:07:37.000000 besos-2.2.2/test/test_rbfopt.py
+-rw-r--r--   0 user      (1000) user      (1000)     4687 2023-09-02 17:28:21.000000 besos-2.2.2/test/test_selectors.py
+-rw-r--r--   0 user      (1000) user      (1000)     3711 2023-09-02 19:14:36.000000 besos-2.2.2/test/test_simulation.py
```

### Comparing `besos-2.2.0/LICENSE` & `besos-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/PKG-INFO` & `besos-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besos
-Version: 2.2.0
+Version: 2.2.2
 Summary: A library for Building and Energy Simulation, Optimization and Surrogate-modelling
 Home-page: https://gitlab.com/energyincities/besos
 Author: Ralph Evins
 Author-email: revins@uvic.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `besos-2.2.0/README.md` & `besos-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/.ipynb_checkpoints/config-checkpoint.py` & `besos-2.2.2/besos/.ipynb_checkpoints/config-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py` & `besos-2.2.2/besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py` & `besos-2.2.2/besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/.ipynb_checkpoints/evaluator-checkpoint.py` & `besos-2.2.2/besos/.ipynb_checkpoints/evaluator-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/.ipynb_checkpoints/parameters-checkpoint.py` & `besos-2.2.2/besos/.ipynb_checkpoints/parameters-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py` & `besos-2.2.2/besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/.ipynb_checkpoints/sampling-checkpoint.py` & `besos-2.2.2/besos/.ipynb_checkpoints/sampling-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/IDF_class.py` & `besos-2.2.2/besos/IDF_class.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/IO_Objects.py` & `besos-2.2.2/besos/IO_Objects.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/IDF_class.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/IDF_class.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/IO_Objects.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/IO_Objects.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/besos_utils.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/besos_utils.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/config.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/config.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/eplus_funcs.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/eplus_funcs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/eppy_funcs.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/eppy_funcs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/errors.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/errors.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/evaluator.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/evaluator.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Oct 30 00:44:53 2023 UTC, .py size: 35684 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 85fc 3e65 648b 0000  U.........>ed...
+00000000: 550d 0d0a 0000 0000 bf6e 4065 658b 0000  U........n@ee...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 a201 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6402 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 5a02 6401 6402 6c03 5a03 6401 6402 6c04  Z.d.d.l.Z.d.d.l.
 00000050: 5a04 6401 6402 6c05 5a05 6401 6403 6c06  Z.d.d.l.Z.d.d.l.
 00000060: 6d07 5a07 6d08 5a08 0100 6401 6404 6c09  m.Z.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6401 6405 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -538,15 +538,15 @@
 00002190: 7461 696e 696e 6720 7468 6520 7265 7375  taining the resu
 000021a0: 6c74 7320 666f 7220 6561 6368 206f 626a  lts for each obj
 000021b0: 6563 7469 7665 2e0a 2020 2020 2020 2020  ective..        
 000021c0: 7266 0000 0029 015a 0b6e 7061 7274 6974  rf...).Z.npartit
 000021d0: 696f 6e73 da09 6b65 6570 5f64 6972 73a9  ions..keep_dirs.
 000021e0: 01da 0763 6f6c 756d 6e73 da06 6578 7061  ...columns..expa
 000021f0: 6e64 2903 da04 6178 6973 da04 6d65 7461  nd)...axis..meta
-00002200: da0b 7265 7375 6c74 5f74 7970 655a 0945  ..result_typeZ.E
+00002200: da0b 7265 7375 6c74 5f74 7970 65da 0945  ..result_type..E
 00002210: 7865 6375 7469 6e67 da03 726f 7729 03da  xecuting..row)..
 00002220: 0574 6f74 616c da04 6465 7363 da04 756e  .total..desc..un
 00002230: 6974 2902 727c 0000 0072 7e00 0000 6301  it).r|...r~...c.
 00002240: 0000 0000 0000 0000 0000 0003 0000 0004  ................
 00002250: 0000 0053 0000 0073 1600 0000 6900 7c00  ...S...s....i.|.
 00002260: 5d0e 5c02 7d01 7d02 7c01 7c02 9302 7104  ].\.}.}.|.|...q.
 00002270: 5300 721e 0000 0072 1e00 0000 2903 721b  S.r....r....).r.
@@ -604,66 +604,66 @@
 000025b0: 616d 6264 613e 2301 0000 7304 0000 0004  ambda>#...s.....
 000025c0: 0106 ff7a 2f41 6273 7472 6163 7445 7661  ...z/AbstractEva
 000025d0: 6c75 6174 6f72 2e74 6f5f 706c 6174 7970  luator.to_platyp
 000025e0: 7573 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d  us.<locals>.<lam
 000025f0: 6264 613e 2903 7232 0000 00da 0b74 6f5f  bda>).r2.....to_
 00002600: 706c 6174 7970 7573 da08 6675 6e63 7469  platypus..functi
 00002610: 6f6e 2902 723a 0000 0072 3200 0000 721e  on).r:...r2...r.
-00002620: 0000 0072 5f00 0000 721f 0000 0072 9800  ...r_...r....r..
+00002620: 0000 0072 5f00 0000 721f 0000 0072 9900  ...r_...r....r..
 00002630: 0000 1d01 0000 7306 0000 0000 050a 010e  ......s.........
 00002640: 037a 1d41 6273 7472 6163 7445 7661 6c75  .z.AbstractEvalu
 00002650: 6174 6f72 2e74 6f5f 706c 6174 7970 7573  ator.to_platypus
-00002660: 2902 7296 0000 0072 3d00 0000 6302 0000  ).r....r=...c...
+00002660: 2902 7297 0000 0072 3d00 0000 6302 0000  ).r....r=...c...
 00002670: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 00002680: 0043 0000 0073 3400 0000 7c00 6a00 6a01  .C...s4...|.j.j.
 00002690: 6401 6b04 722c 7c01 6400 7c00 6a00 6a02  d.k.r,|.d.|.j.j.
 000026a0: 8502 1900 7c01 7c00 6a00 6a02 6400 8502  ....|.|.j.j.d...
 000026b0: 1900 6602 5300 7c01 5300 6400 5300 2902  ..f.S.|.S.d.S.).
 000026c0: 4e72 0100 0000 2903 7232 0000 0072 4700  Nr....).r2...rG.
-000026d0: 0000 7246 0000 0029 0272 3a00 0000 7296  ..rF...).r:...r.
+000026d0: 0000 7246 0000 0029 0272 3a00 0000 7297  ..rF...).r:...r.
 000026e0: 0000 0072 1e00 0000 721e 0000 0072 1f00  ...r....r....r..
-000026f0: 0000 7295 0000 0028 0100 0073 0a00 0000  ..r....(...s....
+000026f0: 0000 7296 0000 0028 0100 0073 0a00 0000  ..r....(...s....
 00002700: 0003 0c02 0e01 0efe 0405 7a26 4162 7374  ..........z&Abst
 00002710: 7261 6374 4576 616c 7561 746f 722e 7061  ractEvaluator.pa
 00002720: 636b 6167 655f 666f 725f 706c 6174 7970  ckage_for_platyp
 00002730: 7573 2902 da0b 6e75 6d5f 7361 6d70 6c65  us)...num_sample
 00002740: 7372 3d00 0000 6302 0000 0000 0000 0000  sr=...c.........
 00002750: 0000 0003 0000 0005 0000 0043 0000 0073  ...........C...s
 00002760: 1c00 0000 7400 a001 7400 6a02 7c00 6a03  ....t...t.j.|.j.
 00002770: 7c01 a103 7d02 7c00 a004 7c02 a101 5300  |...}.|...|...S.
 00002780: 7218 0000 0029 0572 1500 0000 da0c 6469  r....).r......di
 00002790: 7374 5f73 616d 706c 6572 da03 6c68 7372  st_sampler..lhsr
-000027a0: 3200 0000 7294 0000 0029 0372 3a00 0000  2...r....).r:...
-000027b0: 729a 0000 0072 5400 0000 721e 0000 0072  r....rT...r....r
+000027a0: 3200 0000 7295 0000 0029 0372 3a00 0000  2...r....).r:...
+000027b0: 729b 0000 0072 5400 0000 721e 0000 0072  r....rT...r....r
 000027c0: 1e00 0000 721f 0000 00da 0673 616d 706c  ....r......sampl
 000027d0: 6533 0100 0073 0400 0000 0001 1201 7a18  e3...s........z.
 000027e0: 4162 7374 7261 6374 4576 616c 7561 746f  AbstractEvaluato
 000027f0: 722e 7361 6d70 6c65 6301 0000 0000 0000  r.samplec.......
 00002800: 0000 0000 0001 0000 0008 0000 0043 0000  .............C..
 00002810: 0073 2e00 0000 7a14 7c00 6a00 a001 a100  .s....z.|.j.....
 00002820: 0100 6400 7c00 5f00 5700 6e14 0400 7402  ..d.|._.W.n...t.
 00002830: 6b0a 7228 0100 0100 0100 5900 6e02 5800  k.r(......Y.n.X.
 00002840: 6400 5300 7218 0000 0029 0372 3900 0000  d.S.r....).r9...
 00002850: da05 636c 6f73 65da 0e41 7474 7269 6275  ..close..Attribu
 00002860: 7465 4572 726f 7272 5f00 0000 721e 0000  teErrorr_...r...
-00002870: 0072 1e00 0000 721f 0000 0072 9200 0000  .r....r....r....
+00002870: 0072 1e00 0000 721f 0000 0072 9300 0000  .r....r....r....
 00002880: 3701 0000 730a 0000 0000 0102 010a 010a  7...s...........
 00002890: 010e 017a 1e41 6273 7472 6163 7445 7661  ...z.AbstractEva
 000028a0: 6c75 6174 6f72 2e63 6c65 616e 7570 5f70  luator.cleanup_p
 000028b0: 6261 7263 0100 0000 0000 0000 0000 0000  barc............
 000028c0: 0100 0000 0800 0000 4300 0000 732a 0000  ........C...s*..
 000028d0: 007a 107c 006a 00a0 0164 01a1 0101 0057  .z.|.j...d.....W
 000028e0: 006e 1404 0074 026b 0a72 2401 0001 0001  .n...t.k.r$.....
 000028f0: 0059 006e 0258 0064 0253 0029 037a 3c55  .Y.n.X.d.S.).z<U
 00002900: 7064 6174 6573 2074 6865 2070 726f 6772  pdates the progr
 00002910: 6573 7320 6261 722c 206d 6172 6b69 6e67  ess bar, marking
 00002920: 206f 6e65 206d 6f72 6520 726f 7720 6173   one more row as
 00002930: 2063 6f6d 706c 6574 6564 2e72 6600 0000   completed.rf...
 00002940: 4e29 0372 3900 0000 da06 7570 6461 7465  N).r9.....update
-00002950: 729f 0000 0072 5f00 0000 721e 0000 0072  r....r_...r....r
+00002950: 72a0 0000 0072 5f00 0000 721e 0000 0072  r....r_...r....r
 00002960: 1e00 0000 721f 0000 00da 0b75 7064 6174  ....r......updat
 00002970: 655f 7062 6172 3e01 0000 7308 0000 0000  e_pbar>...s.....
 00002980: 0202 0110 010e 017a 1d41 6273 7472 6163  .......z.Abstrac
 00002990: 7445 7661 6c75 6174 6f72 2e75 7064 6174  tEvaluator.updat
 000029a0: 655f 7062 6172 2902 725b 0000 0072 3d00  e_pbar).r[...r=.
 000029b0: 0000 6301 0000 0000 0000 0000 0000 0003  ..c.............
 000029c0: 0000 0005 0000 0043 0000 0073 6600 0000  .......C...sf...
@@ -802,20 +802,20 @@
 00003210: 7220 6465 7461 696c 7320 6f6e 2074 6865  r details on the
 00003220: 206e 6577 2066 6f72 6d61 742e 200a 596f   new format. .Yo
 00003230: 7572 2065 7272 6f72 206d 6f64 6520 6861  ur error mode ha
 00003240: 7320 6175 746f 6d61 7469 6361 6c6c 7920  s automatically 
 00003250: 6265 656e 2063 6f6e 7665 7274 6564 2074  been converted t
 00003260: 6f20 6120 6e65 7720 666f 726d 6174 2065  o a new format e
 00003270: 7175 6976 616c 656e 742e 4e29 024e 4e72  quivalent.N).NNr
-00003280: a200 0000 290b 722a 0000 0072 3200 0000  ....).r*...r2...
-00003290: 7246 0000 0072 4700 0000 72a5 0000 0072  rF...rG...r....r
-000032a0: 0b00 0000 72a6 0000 0072 4800 0000 7226  ....r....rH...r&
+00003280: a300 0000 290b 722a 0000 0072 3200 0000  ....).r*...r2...
+00003290: 7246 0000 0072 4700 0000 72a6 0000 0072  rF...rG...r....r
+000032a0: 0b00 0000 72a7 0000 0072 4800 0000 7226  ....r....rH...r&
 000032b0: 0000 0072 0a00 0000 7249 0000 0029 0572  ...r....rI...).r
 000032c0: 3a00 0000 7234 0000 00da 0777 6172 6e69  :...r4.....warni
-000032d0: 6e67 7286 0000 0072 a800 0000 721e 0000  ngr....r....r...
+000032d0: 6e67 7287 0000 0072 a900 0000 721e 0000  ngr....r....r...
 000032e0: 0072 1e00 0000 721f 0000 0072 3600 0000  .r....r....r6...
 000032f0: 6f01 0000 733e 0000 0000 0902 ff02 0608  o...s>..........
 00003300: 0104 010c 0114 0104 020c 0202 ff02 020e  ................
 00003310: fe04 030c 0104 0508 0114 010c 0108 0202  ................
 00003320: ff02 0206 fe04 0308 0108 0202 ff02 0206  ................
 00003330: fe04 0308 0108 017a 3541 6273 7472 6163  .......z5Abstrac
 00003340: 7445 7661 6c75 6174 6f72 2e5f 636f 6e76  tEvaluator._conv
@@ -825,20 +825,20 @@
 00003380: 4672 6600 0000 2920 da08 5f5f 6e61 6d65  Frf...) ..__name
 00003390: 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f da0c  __..__module__..
 000033a0: 5f5f 7175 616c 6e61 6d65 5f5f da07 5f5f  __qualname__..__
 000033b0: 646f 635f 5f72 4400 0000 7216 0000 00da  doc__rD...r.....
 000033c0: 0373 7472 722a 0000 00da 0462 6f6f 6c72  .strr*.....boolr
 000033d0: 3b00 0000 7237 0000 0072 0300 0000 720a  ;...r7...r....r.
 000033e0: 0000 0072 5200 0000 725e 0000 0072 6000  ...rR...r^...r`.
-000033f0: 0000 7256 0000 00da 0244 4672 a300 0000  ..rV.....DFr....
-00003400: 7277 0000 0072 9400 0000 da08 706c 6174  rw...r......plat
-00003410: 7970 7573 7298 0000 0072 0800 0000 7207  ypusr....r....r.
-00003420: 0000 0072 9500 0000 729d 0000 0072 9200  ...r....r....r..
-00003430: 0000 72a1 0000 00da 0c73 7461 7469 636d  ..r......staticm
-00003440: 6574 686f 6472 a900 0000 7236 0000 0072  ethodr....r6...r
+000033f0: 0000 7256 0000 00da 0244 4672 a400 0000  ..rV.....DFr....
+00003400: 7277 0000 0072 9500 0000 da08 706c 6174  rw...r......plat
+00003410: 7970 7573 7299 0000 0072 0800 0000 7207  ypusr....r....r.
+00003420: 0000 0072 9600 0000 729e 0000 0072 9300  ...r....r....r..
+00003430: 0000 72a2 0000 00da 0c73 7461 7469 636d  ..r......staticm
+00003440: 6574 686f 6472 aa00 0000 7236 0000 0072  ethodr....r6...r
 00003450: 1e00 0000 721e 0000 0072 1e00 0000 721f  ....r....r....r.
 00003460: 0000 0072 2e00 0000 4700 0000 7346 0000  ...r....G...sF..
 00003470: 0008 0104 0a0a 0500 0100 0100 fb02 0202  ................
 00003480: 0102 0102 0102 fb0c 1b0e 2b02 0112 0a10  ..........+.....
 00003490: 210e 0510 0b14 1700 0100 fc02 0202 0202  !...............
 000034a0: 0202 fa0c 3310 0c02 0112 fe0c 0b10 040e  ....3...........
 000034b0: 0708 0902 0112 2772 2e00 0000 6300 0000  ......'r....c...
@@ -886,42 +886,42 @@
 00003750: 7261 6d20 7072 6f67 7265 7373 5f62 6172  ram progress_bar
 00003760: 3a20 7768 6574 6865 7220 6f72 206e 6f74  : whether or not
 00003770: 2074 6f20 6469 7370 6c61 7920 6120 7072   to display a pr
 00003780: 6f67 7265 7373 2062 6172 0a20 2020 2020  ogress bar.     
 00003790: 2020 2072 3100 0000 4e29 03da 0573 7570     r1...N)...sup
 000037a0: 6572 723b 0000 00da 105f 6576 616c 7561  err;....._evalua
 000037b0: 7469 6f6e 5f66 756e 6329 0672 3a00 0000  tion_func).r:...
-000037c0: 72b5 0000 0072 3200 0000 7233 0000 0072  r....r2...r3...r
+000037c0: 72b6 0000 0072 3200 0000 7233 0000 0072  r....r2...r3...r
 000037d0: 3400 0000 7235 0000 00a9 01da 095f 5f63  4...r5.......__c
 000037e0: 6c61 7373 5f5f 721e 0000 0072 1f00 0000  lass__r....r....
 000037f0: 723b 0000 00a7 0100 0073 0e00 0000 000f  r;.......s......
 00003800: 0601 0201 0201 0201 02fc 0606 7a19 4576  ............z.Ev
 00003810: 616c 7561 746f 7247 656e 6572 6963 2e5f  aluatorGeneric._
 00003820: 5f69 6e69 745f 5f72 4d00 0000 6302 0000  _init__rM...c...
 00003830: 0000 0000 0000 0000 0003 0000 0003 0000  ................
 00003840: 0043 0000 0073 2000 0000 7c00 a000 7c01  .C...s ...|...|.
 00003850: a101 7d02 7c00 a001 7c02 a101 7d02 7c00  ..}.|...|...}.|.
 00003860: a002 a100 0100 7c02 5300 7218 0000 0029  ......|.S.r....)
-00003870: 0372 b700 0000 72a9 0000 0072 a100 0000  .r....r....r....
+00003870: 0372 b800 0000 72aa 0000 0072 a200 0000  .r....r....r....
 00003880: 2903 723a 0000 0072 4e00 0000 725b 0000  ).r:...rN...r[..
 00003890: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
 000038a0: 7252 0000 00be 0100 0073 0800 0000 0001  rR.......s......
 000038b0: 0a01 0a01 0801 7a1c 4576 616c 7561 746f  ......z.Evaluato
 000038c0: 7247 656e 6572 6963 2e65 7661 6c5f 7369  rGeneric.eval_si
 000038d0: 6e67 6c65 2903 722f 0000 004e 5429 0f72  ngle).r/...NT).r
-000038e0: ab00 0000 72ac 0000 0072 ad00 0000 72ae  ....r....r....r.
+000038e0: ac00 0000 72ad 0000 0072 ae00 0000 72af  ....r....r....r.
 000038f0: 0000 0072 0500 0000 720a 0000 0072 0700  ...r....r....r..
 00003900: 0000 723f 0000 005a 1065 7661 6c5f 6675  ..r?...Z.eval_fu
-00003910: 6e63 5f66 6f72 6d61 7472 1600 0000 72af  nc_formatr....r.
-00003920: 0000 0072 b000 0000 723b 0000 0072 5200  ...r....r;...rR.
+00003910: 6e63 5f66 6f72 6d61 7472 1600 0000 72b0  nc_formatr....r.
+00003920: 0000 0072 b100 0000 723b 0000 0072 5200  ...r....r;...rR.
 00003930: 0000 da0d 5f5f 636c 6173 7363 656c 6c5f  ....__classcell_
-00003940: 5f72 1e00 0000 721e 0000 0072 b800 0000  _r....r....r....
-00003950: 721f 0000 0072 b400 0000 9e01 0000 731a  r....r........s.
+00003940: 5f72 1e00 0000 721e 0000 0072 b900 0000  _r....r....r....
+00003950: 721f 0000 0072 b500 0000 9e01 0000 731a  r....r........s.
 00003960: 0000 0008 0104 0616 0600 0100 0100 fa02  ................
-00003970: 0202 0102 0102 0102 0102 fa10 1772 b400  .............r..
+00003970: 0202 0102 0102 0102 0102 fa10 1772 b500  .............r..
 00003980: 0000 7a05 312e 362e 307a 4945 7661 6c75  ..z.1.6.0zIEvalu
 00003990: 6174 6f72 5352 2068 6173 2062 6565 6e20  atorSR has been 
 000039a0: 7265 6e61 6d65 6420 6173 2045 7661 6c75  renamed as Evalu
 000039b0: 6174 6f72 4765 6e65 7269 6320 7769 7468  atorGeneric with
 000039c0: 2073 616d 6520 6675 6e63 7469 6f6e 616c   same functional
 000039d0: 6974 792e 2902 da07 7665 7273 696f 6eda  ity.)...version.
 000039e0: 0672 6561 736f 6e63 0000 0000 0000 0000  .reasonc........
@@ -932,19 +932,19 @@
 00003a30: 4d6f 6465 6c20 4576 616c 7561 746f 720a  Model Evaluator.
 00003a40: 0a20 2020 2054 6869 7320 6576 616c 7561  .    This evalua
 00003a50: 746f 7220 6861 7320 6265 656e 2072 6570  tor has been rep
 00003a60: 6c61 6365 6420 6279 2045 7661 6c75 6174  laced by Evaluat
 00003a70: 6f72 4765 6e65 7269 632c 2077 696c 6c20  orGeneric, will 
 00003a80: 6265 2072 656d 6f76 6564 2069 6e20 6120  be removed in a 
 00003a90: 6675 7475 7265 2072 656c 6561 7365 2e0a  future release..
-00003aa0: 2020 2020 4e29 0472 ab00 0000 72ac 0000      N).r....r...
-00003ab0: 0072 ad00 0000 72ae 0000 0072 1e00 0000  .r....r....r....
+00003aa0: 2020 2020 4e29 0472 ac00 0000 72ad 0000      N).r....r...
+00003ab0: 0072 ae00 0000 72af 0000 0072 1e00 0000  .r....r....r....
 00003ac0: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-00003ad0: bd00 0000 c501 0000 7304 0000 0008 0504  ........s.......
-00003ae0: 0572 bd00 0000 6300 0000 0000 0000 0000  .r....c.........
+00003ad0: be00 0000 c501 0000 7304 0000 0008 0504  ........s.......
+00003ae0: 0572 be00 0000 6300 0000 0000 0000 0000  .r....c.........
 00003af0: 0000 0000 0000 0005 0000 0000 0000 0073  ...............s
 00003b00: e800 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
 00003b10: 6504 6505 6506 6a07 6602 1900 5a08 6423  e.e.e.j.f...Z.d#
 00003b20: 6509 650a 650b 6404 9c03 8700 6601 6405  e.e.e.d.....f.d.
 00003b30: 6406 840d 5a0c 650d 6407 6408 8400 8301  d...Z.e.d.d.....
 00003b40: 5a0e 650e 6a0f 6510 6409 9c01 640a 6408  Z.e.j.e.d...d.d.
 00003b50: 8404 8301 5a0e 6424 6508 6511 6402 640c  ....Z.d$e.e.d.d.
@@ -1001,39 +1001,39 @@
 00003e80: 0000 0000 0000 0000 0000 0400 0000 0500  ................
 00003e90: 0000 0300 0000 7342 0000 007c 017c 005f  ......sB...|.|._
 00003ea0: 0074 0183 006a 027c 016a 037c 027c 0364  .t...j.|.j.|.|.d
 00003eb0: 018d 0301 0064 007c 005f 0474 056a 067c  .....d.|._.t.j.|
 00003ec0: 006a 036a 0764 0264 0364 0467 0364 058d  .j.j.d.d.d.g.d..
 00003ed0: 0164 068d 017c 005f 0864 0053 0029 074e  .d...|._.d.S.).N
 00003ee0: 2903 7232 0000 0072 3300 0000 7234 0000  ).r2...r3...r4..
-00003ef0: 0072 5400 0000 7286 0000 0072 a800 0000  .rT...r....r....
+00003ef0: 0072 5400 0000 7287 0000 0072 a900 0000  .rT...r....r....
 00003f00: a901 da05 7061 7274 7372 7900 0000 2909  ....partsry...).
-00003f10: 72bf 0000 0072 b600 0000 723b 0000 0072  r....r....r;...r
-00003f20: 3200 0000 da05 6d6f 6465 6c72 8a00 0000  2.....modelr....
+00003f10: 72c0 0000 0072 b700 0000 723b 0000 0072  r....r....r;...r
+00003f20: 3200 0000 da05 6d6f 6465 6c72 8b00 0000  2.....modelr....
 00003f30: 720e 0000 0072 5900 0000 da04 6461 7461  r....rY.....data
-00003f40: 2904 723a 0000 0072 bf00 0000 7233 0000  ).r:...r....r3..
-00003f50: 0072 3400 0000 72b8 0000 0072 1e00 0000  .r4...r....r....
+00003f40: 2904 723a 0000 0072 c000 0000 7233 0000  ).r:...r....r3..
+00003f50: 0072 3400 0000 72b9 0000 0072 1e00 0000  .r4...r....r....
 00003f60: 721f 0000 0072 3b00 0000 f801 0000 7314  r....r;.......s.
 00003f70: 0000 0000 0606 0106 0104 0102 0102 fd06  ................
 00003f80: 0606 0104 0112 ff7a 1341 6461 7074 6976  .......z.Adaptiv
 00003f90: 6553 522e 5f5f 696e 6974 5f5f 6301 0000  eSR.__init__c...
 00003fa0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
 00003fb0: 0043 0000 0073 0800 0000 7c00 6a00 6a01  .C...s....|.j.j.
-00003fc0: 5300 7218 0000 00a9 0272 bf00 0000 7232  S.r......r....r2
+00003fc0: 5300 7218 0000 00a9 0272 c000 0000 7232  S.r......r....r2
 00003fd0: 0000 0072 5f00 0000 721e 0000 0072 1e00  ...r_...r....r..
 00003fe0: 0000 721f 0000 0072 3200 0000 0a02 0000  ..r....r2.......
 00003ff0: 7302 0000 0000 027a 1241 6461 7074 6976  s......z.Adaptiv
 00004000: 6553 522e 7072 6f62 6c65 6d72 2c00 0000  eSR.problemr,...
 00004010: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
 00004020: 0002 0000 0043 0000 0073 0c00 0000 7c01  .....C...s....|.
 00004030: 7c00 6a00 5f01 6400 5300 7218 0000 0072  |.j._.d.S.r....r
-00004040: c400 0000 a902 723a 0000 0072 2d00 0000  ......r:...r-...
+00004040: c500 0000 a902 723a 0000 0072 2d00 0000  ......r:...r-...
 00004050: 721e 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
 00004060: 3200 0000 0e02 0000 7302 0000 0000 0254  2.......s......T
-00004070: 2903 72c3 0000 00da 0b64 6564 7570 6c69  ).r......dedupli
+00004070: 2903 72c4 0000 00da 0b64 6564 7570 6c69  ).r......dedupli
 00004080: 6361 7465 723d 0000 0063 0300 0000 0000  cater=...c......
 00004090: 0000 0000 0000 0400 0000 0600 0000 4300  ..............C.
 000040a0: 0000 7348 0000 007c 00a0 00a1 0001 007c  ..sH...|.......|
 000040b0: 006a 01a0 027c 0164 0164 0264 0367 03a1  .j...|.d.d.d.g..
 000040c0: 027d 0374 036a 047c 006a 057c 0367 0264  .}.t.j.|.j.|.g.d
 000040d0: 0464 058d 027c 005f 057c 0272 447c 006a  .d...|._.|.rD|.j
 000040e0: 056a 0664 0464 068d 0101 0064 0753 0029  .j.d.d.....d.S.)
@@ -1048,21 +1048,21 @@
 00004170: 2020 2020 3a70 6172 616d 2064 6564 7570      :param dedup
 00004180: 6c69 6361 7465 3a20 7768 6574 6865 7220  licate: whether 
 00004190: 746f 2072 656d 6f76 6520 6475 706c 6963  to remove duplic
 000041a0: 6174 6573 2066 726f 6d20 7468 6520 636f  ates from the co
 000041b0: 6d62 696e 6564 2044 6174 6146 7261 6d65  mbined DataFrame
 000041c0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
 000041d0: 3a0a 2020 2020 2020 2020 7254 0000 0072  :.        rT...r
-000041e0: 8600 0000 72a8 0000 0054 2901 da0c 6967  ....r....T)...ig
+000041e0: 8700 0000 72a9 0000 0054 2901 da0c 6967  ....r....T)...ig
 000041f0: 6e6f 7265 5f69 6e64 6578 2901 da07 696e  nore_index)...in
 00004200: 706c 6163 654e 2907 7260 0000 0072 3200  placeN).r`...r2.
-00004210: 0000 da05 746f 5f64 6672 8a00 0000 7291  ....to_dfr....r.
-00004220: 0000 0072 c300 0000 da0f 6472 6f70 5f64  ...r......drop_d
+00004210: 0000 da05 746f 5f64 6672 8b00 0000 7292  ....to_dfr....r.
+00004220: 0000 0072 c400 0000 da0f 6472 6f70 5f64  ...r......drop_d
 00004230: 7570 6c69 6361 7465 7329 0472 3a00 0000  uplicates).r:...
-00004240: 72c3 0000 0072 c600 0000 da08 6e65 775f  r....r......new_
+00004240: 72c4 0000 0072 c700 0000 da08 6e65 775f  r....r......new_
 00004250: 6461 7461 721e 0000 0072 1e00 0000 721f  datar....r....r.
 00004260: 0000 00da 0b61 7070 656e 645f 6461 7461  .....append_data
 00004270: 1202 0000 730a 0000 0000 0708 0214 0216  ....s...........
 00004280: 0104 017a 1641 6461 7074 6976 6553 522e  ...z.AdaptiveSR.
 00004290: 6170 7065 6e64 5f64 6174 6129 02da 0e6e  append_data)...n
 000042a0: 756d 5f64 6174 6170 6f69 6e74 7372 3d00  um_datapointsr=.
 000042b0: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
@@ -1079,19 +1079,19 @@
 00004360: 6f66 2064 6174 6170 6f69 6e74 7320 746f  of datapoints to
 00004370: 2067 656e 6572 6174 650a 2020 2020 2020   generate.      
 00004380: 2020 3a72 6574 7572 6e3a 2074 6865 2064    :return: the d
 00004390: 6174 6170 6f69 6e74 7320 6765 6e65 7261  atapoints genera
 000043a0: 7465 642c 2069 6e20 736f 6d65 2074 6162  ted, in some tab
 000043b0: 756c 6172 2064 6174 6173 7472 7563 7475  ular datastructu
 000043c0: 7265 0a20 2020 2020 2020 204e 2901 724c  re.        N).rL
-000043d0: 0000 0029 0272 3a00 0000 72cd 0000 0072  ...).r:...r....r
+000043d0: 0000 0029 0272 3a00 0000 72ce 0000 0072  ...).r:...r....r
 000043e0: 1e00 0000 721e 0000 0072 1f00 0000 da0a  ....r....r......
 000043f0: 6765 745f 696e 6669 6c6c 2102 0000 7302  get_infill!...s.
 00004400: 0000 0000 067a 1541 6461 7074 6976 6553  .....z.AdaptiveS
-00004410: 522e 6765 745f 696e 6669 6c6c 2902 72c3  R.get_infill).r.
+00004410: 522e 6765 745f 696e 6669 6c6c 2902 72c4  R.get_infill).r.
 00004420: 0000 0072 3d00 0000 6302 0000 0000 0000  ...r=...c.......
 00004430: 0000 0000 0006 0000 0005 0000 0043 0000  .............C..
 00004440: 0073 7400 0000 7c00 6a00 7d02 7c00 6a01  .st...|.j.}.|.j.
 00004450: 6a02 7c01 6401 6402 6403 6703 6404 8d02  j.|.d.d.d.g.d...
 00004460: 5c02 7d03 7d04 7c04 6401 6701 6b02 7246  \.}.}.|.d.g.k.rF
 00004470: 7c00 a003 7c03 a101 7d05 7404 6a05 7c03  |...|...}.t.j.|.
 00004480: 7c05 6702 6405 6406 8d02 7d03 7c00 a006  |.g.d.d...}.|...
@@ -1103,30 +1103,30 @@
 000044e0: 2058 2061 6e64 206f 7574 7075 7473 2079   X and outputs y
 000044f0: 2c20 616e 6420 7374 6f72 6573 2074 6865  , and stores the
 00004500: 2061 6464 6564 2064 6174 610a 0a20 2020   added data..   
 00004510: 2020 2020 203a 7061 7261 6d20 6461 7461       :param data
 00004520: 3a20 6120 7461 626c 6520 6f66 2074 7261  : a table of tra
 00004530: 696e 696e 6720 6461 7461 0a20 2020 2020  ining data.     
 00004540: 2020 203a 7265 7475 726e 3a20 4e6f 6e65     :return: None
-00004550: 0a20 2020 2020 2020 2072 5400 0000 7286  .        rT...r.
-00004560: 0000 0072 a800 0000 72c0 0000 0072 6600  ...r....r....rf.
-00004570: 0000 7289 0000 004e 290a 72c3 0000 0072  ..r....N).r....r
+00004550: 0a20 2020 2020 2020 2072 5400 0000 7287  .        rT...r.
+00004560: 0000 0072 a900 0000 72c1 0000 0072 6600  ...r....r....rf.
+00004570: 0000 728a 0000 004e 290a 72c4 0000 0072  ..r....N).r....r
 00004580: 3200 0000 da0a 7061 7274 6961 6c5f 6466  2.....partial_df
 00004590: da12 6765 745f 6672 6f6d 5f72 6566 6572  ..get_from_refer
-000045a0: 656e 6365 728a 0000 0072 9100 0000 72cc  encer....r....r.
-000045b0: 0000 0072 c200 0000 da05 7472 6169 6eda  ...r......train.
+000045a0: 656e 6365 728b 0000 0072 9200 0000 72cd  encer....r....r.
+000045b0: 0000 0072 c300 0000 da05 7472 6169 6eda  ...r......train.
 000045c0: 0c75 7064 6174 655f 6d6f 6465 6c29 0672  .update_model).r
-000045d0: 3a00 0000 72c3 0000 005a 066f 6c64 5f64  :...r....Z.old_d
-000045e0: 6672 6700 0000 72c1 0000 0072 8600 0000  frg...r....r....
+000045d0: 3a00 0000 72c4 0000 005a 066f 6c64 5f64  :...r....Z.old_d
+000045e0: 6672 6700 0000 72c2 0000 0072 8700 0000  frg...r....r....
 000045f0: 721e 0000 0072 1e00 0000 721f 0000 00da  r....r....r.....
 00004600: 0964 6f5f 696e 6669 6c6c 2902 0000 7318  .do_infill)...s.
 00004610: 0000 0000 0606 0106 0102 0008 ff0a 030a  ................
 00004620: 010a 0112 010a 010a 010a 027a 1441 6461  ...........z.Ada
 00004630: 7074 6976 6553 522e 646f 5f69 6e66 696c  ptiveSR.do_infil
-00004640: 6c29 0372 cb00 0000 da08 6f6c 645f 6461  l).r......old_da
+00004640: 6c29 0372 cc00 0000 da08 6f6c 645f 6461  l).r......old_da
 00004650: 7461 723d 0000 0063 0300 0000 0000 0000  tar=...c........
 00004660: 0000 0000 0300 0000 0200 0000 4300 0000  ............C...
 00004670: 730c 0000 007c 00a0 00a1 0001 0064 0153  s....|.......d.S
 00004680: 0029 0261 0e01 0000 4d6f 6469 6669 6573  .).a....Modifies
 00004690: 2073 656c 662e 6d6f 6465 6c20 746f 2069   self.model to i
 000046a0: 6e63 6f72 706f 7261 7465 2074 6865 206e  ncorporate the n
 000046b0: 6577 2064 6174 612e 0a0a 2020 2020 2020  ew data...      
@@ -1139,17 +1139,17 @@
 00004720: 6420 6f75 7470 7574 730a 2020 2020 2020  d outputs.      
 00004730: 2020 3a70 6172 616d 206f 6c64 5f64 6174    :param old_dat
 00004740: 613a 2074 6865 2074 6162 6c65 206f 6620  a: the table of 
 00004750: 696e 7075 7473 2061 6e64 206f 7574 7075  inputs and outpu
 00004760: 7473 2077 6974 686f 7574 2074 6865 206e  ts without the n
 00004770: 6577 2064 6174 610a 2020 2020 2020 2020  ew data.        
 00004780: 3a72 6574 7572 6e3a 204e 6f6e 650a 2020  :return: None.  
-00004790: 2020 2020 2020 4e29 0172 d100 0000 2903        N).r....).
-000047a0: 723a 0000 0072 cb00 0000 72d4 0000 0072  r:...r....r....r
-000047b0: 1e00 0000 721e 0000 0072 1f00 0000 72d2  ....r....r....r.
+00004790: 2020 2020 2020 4e29 0172 d200 0000 2903        N).r....).
+000047a0: 723a 0000 0072 cc00 0000 72d5 0000 0072  r:...r....r....r
+000047b0: 1e00 0000 721e 0000 0072 1f00 0000 72d3  ....r....r....r.
 000047c0: 0000 003c 0200 0073 0200 0000 0009 7a17  ...<...s......z.
 000047d0: 4164 6170 7469 7665 5352 2e75 7064 6174  AdaptiveSR.updat
 000047e0: 655f 6d6f 6465 6c63 0200 0000 0000 0000  e_modelc........
 000047f0: 0000 0000 0400 0000 0600 0000 4300 0000  ............C...
 00004800: 733a 0000 007c 006a 00a0 017c 00a0 027c  s:...|.j...|...|
 00004810: 01a1 0164 01a1 027d 027c 00a0 037c 02a1  ...d...}.|...|..
 00004820: 017d 037c 00a0 0474 056a 067c 027c 0367  .}.|...t.j.|.|.g
@@ -1161,32 +1161,32 @@
 00004880: 2020 2020 203a 7061 7261 6d20 6e75 6d5f       :param num_
 00004890: 6461 7461 706f 696e 7473 3a20 6e75 6d62  datapoints: numb
 000048a0: 6572 206f 6620 6461 7461 706f 696e 7473  er of datapoints
 000048b0: 2074 6f20 6164 6420 746f 2074 6865 206d   to add to the m
 000048c0: 6f64 656c 2773 2074 7261 696e 696e 6720  odel's training 
 000048d0: 7365 740a 2020 2020 2020 2020 3a72 6574  set.        :ret
 000048e0: 7572 6e3a 204e 6f6e 650a 2020 2020 2020  urn: None.      
-000048f0: 2020 7254 0000 0072 6600 0000 7289 0000    rT...rf...r...
-00004900: 004e 2907 7232 0000 0072 c900 0000 72ce  .N).r2...r....r.
-00004910: 0000 0072 d000 0000 72d3 0000 0072 8a00  ...r....r....r..
-00004920: 0000 7291 0000 0029 0472 3a00 0000 72cd  ..r....).r:...r.
-00004930: 0000 0072 5400 0000 7286 0000 0072 1e00  ...rT...r....r..
+000048f0: 2020 7254 0000 0072 6600 0000 728a 0000    rT...rf...r...
+00004900: 004e 2907 7232 0000 0072 ca00 0000 72cf  .N).r2...r....r.
+00004910: 0000 0072 d100 0000 72d4 0000 0072 8b00  ...r....r....r..
+00004920: 0000 7292 0000 0029 0472 3a00 0000 72ce  ..r....).r:...r.
+00004930: 0000 0072 5400 0000 7287 0000 0072 1e00  ...rT...r....r..
 00004940: 0000 721e 0000 0072 1f00 0000 da06 696e  ..r....r......in
 00004950: 6669 6c6c 4702 0000 7306 0000 0000 0614  fillG...s.......
 00004960: 010a 017a 1141 6461 7074 6976 6553 522e  ...z.AdaptiveSR.
 00004970: 696e 6669 6c6c 723c 0000 0063 0100 0000  infillr<...c....
 00004980: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 00004990: 4300 0000 7304 0000 0064 0153 0029 027a  C...s....d.S.).z
 000049a0: 4847 656e 6572 6174 6573 2061 206e 6577  HGenerates a new
 000049b0: 206d 6f64 656c 2075 7369 6e67 2074 6865   model using the
 000049c0: 2073 746f 7265 6420 6461 7461 2c20 616e   stored data, an
 000049d0: 6420 7374 6f72 6573 2069 7420 6173 2073  d stores it as s
 000049e0: 656c 662e 6d6f 6465 6c4e 721e 0000 0072  elf.modelNr....r
 000049f0: 5f00 0000 721e 0000 0072 1e00 0000 721f  _...r....r....r.
-00004a00: 0000 0072 d100 0000 5102 0000 7302 0000  ...r....Q...s...
+00004a00: 0000 0072 d200 0000 5102 0000 7302 0000  ...r....Q...s...
 00004a10: 0000 037a 1041 6461 7074 6976 6553 522e  ...z.AdaptiveSR.
 00004a20: 7472 6169 6e72 4d00 0000 6302 0000 0000  trainrM...c.....
 00004a30: 0000 0000 0000 0003 0000 0001 0000 004b  ...............K
 00004a40: 0000 0073 0400 0000 6401 5300 2902 7ad2  ...s....d.S.).z.
 00004a50: 4576 616c 7561 7465 7320 6120 7369 6e67  Evaluates a sing
 00004a60: 6c65 2069 6e70 7574 2070 6f69 6e74 0a0a  le input point..
 00004a70: 2020 2020 2020 2020 3a70 6172 616d 2076          :param v
@@ -1219,37 +1219,37 @@
 00004c20: 6865 2064 6174 6170 6f69 6e74 7320 746f  he datapoints to
 00004c30: 2065 7661 6c75 6174 650a 2020 2020 2020   evaluate.      
 00004c40: 2020 3a72 6574 7572 6e3a 2061 2044 6174    :return: a Dat
 00004c50: 6146 7261 6d65 2063 6f6e 7461 696e 696e  aFrame containin
 00004c60: 6720 7468 6520 7265 7375 6c74 7320 6f66  g the results of
 00004c70: 2074 6865 2064 6174 6170 6f69 6e74 730a   the datapoints.
 00004c80: 2020 2020 2020 2020 7254 0000 0029 0472          rT...).r
-00004c90: 3200 0000 72c9 0000 0072 bf00 0000 7294  2...r....r....r.
-00004ca0: 0000 0029 0372 3a00 0000 72d6 0000 0072  ...).r:...r....r
+00004c90: 3200 0000 72ca 0000 0072 c000 0000 7295  2...r....r....r.
+00004ca0: 0000 0029 0372 3a00 0000 72d7 0000 0072  ...).r:...r....r
 00004cb0: 6700 0000 721e 0000 0072 1e00 0000 721f  g...r....r....r.
-00004cc0: 0000 0072 d000 0000 6002 0000 7304 0000  ...r....`...s...
+00004cc0: 0000 0072 d100 0000 6002 0000 7304 0000  ...r....`...s...
 00004cd0: 0000 060e 017a 1d41 6461 7074 6976 6553  .....z.AdaptiveS
 00004ce0: 522e 6765 745f 6672 6f6d 5f72 6566 6572  R.get_from_refer
 00004cf0: 656e 6365 2903 4e72 2f00 0000 4e29 0154  ence).Nr/...N).T
-00004d00: 2901 4e29 1e72 ab00 0000 72ac 0000 0072  ).N).r....r....r
-00004d10: ad00 0000 72ae 0000 0072 0800 0000 72b1  ....r....r....r.
+00004d00: 2901 4e29 1e72 ac00 0000 72ad 0000 0072  ).N).r....r....r
+00004d10: ae00 0000 72af 0000 0072 0800 0000 72b2  ....r....r....r.
 00004d20: 0000 0072 6d00 0000 da05 6172 7261 795a  ...rm.....arrayZ
-00004d30: 0774 6162 756c 6172 722e 0000 0072 af00  .tabularr....r..
+00004d30: 0774 6162 756c 6172 722e 0000 0072 b000  .tabularr....r..
 00004d40: 0000 720a 0000 0072 3b00 0000 da08 7072  ..r....r;.....pr
 00004d50: 6f70 6572 7479 7232 0000 00da 0673 6574  opertyr2.....set
-00004d60: 7465 7272 1600 0000 72b0 0000 0072 cc00  terr....r....r..
-00004d70: 0000 72a3 0000 0072 ce00 0000 72d3 0000  ..r....r....r...
-00004d80: 0072 d200 0000 72d5 0000 0072 0300 0000  .r....r....r....
-00004d90: 72d1 0000 0072 0700 0000 7252 0000 0072  r....r....rR...r
-00004da0: d000 0000 72ba 0000 0072 1e00 0000 721e  ....r....r....r.
-00004db0: 0000 0072 b800 0000 721f 0000 0072 be00  ...r....r....r..
+00004d60: 7465 7272 1600 0000 72b1 0000 0072 cd00  terr....r....r..
+00004d70: 0000 72a4 0000 0072 cf00 0000 72d4 0000  ..r....r....r...
+00004d80: 0072 d300 0000 72d6 0000 0072 0300 0000  .r....r....r....
+00004d90: 72d2 0000 0072 0700 0000 7252 0000 0072  r....r....rR...r
+00004da0: d100 0000 72bb 0000 0072 1e00 0000 721e  ....r....r....r.
+00004db0: 0000 0072 b900 0000 721f 0000 0072 bf00  ...r....r....r..
 00004dc0: 0000 d301 0000 7330 0000 0008 0104 220e  ......s0......".
 00004dd0: 0400 0100 0100 fc02 0202 0102 0102 fc10  ................
 00004de0: 1202 010a 0304 0110 0314 0f10 0810 1314  ................
-00004df0: 0b10 0a02 0110 0402 0112 0972 be00 0000  ...........r....
+00004df0: 0b10 0a02 0110 0402 0112 0972 bf00 0000  ...........r....
 00004e00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00004e10: 000c 0000 0000 0000 0073 f400 0000 6500  .........s....e.
 00004e20: 5a01 6400 5a02 6401 5a03 6504 6a05 6402  Z.d.Z.d.Z.e.j.d.
 00004e30: 1900 6504 6a06 6504 6a07 6403 6404 6404  ..e.j.e.j.d.d.d.
 00004e40: 6405 6404 6608 6404 6406 9c01 6508 6509  d.d.f.d.d...e.e.
 00004e50: 6509 6509 650a 650b 650c 1900 650d 6509  e.e.e.e.e...e.e.
 00004e60: 6509 6407 9c09 8700 6601 6408 6409 840f  e.d.....f.d.d...
@@ -1270,18 +1270,18 @@
 00004f50: 6c64 696e 672c 2061 6e64 2074 6865 6e20  lding, and then 
 00004f60: 7369 6d75 6c61 7465 2069 742e 0a20 2020  simulate it..   
 00004f70: 2049 7420 6b65 6570 7320 7472 6163 6b20   It keeps track 
 00004f80: 6f66 2074 6865 2062 7569 6c64 696e 6720  of the building 
 00004f90: 616e 6420 7468 6520 7765 6174 6865 7220  and the weather 
 00004fa0: 6669 6c65 2eda 0365 7077 722f 0000 004e  file...epwr/...N
 00004fb0: 5429 01da 0865 7077 5f66 696c 6529 0972  T)...epw_file).r
-00004fc0: 3200 0000 72db 0000 00da 076f 7574 5f64  2...r......out_d
+00004fc0: 3200 0000 72dc 0000 00da 076f 7574 5f64  2...r......out_d
 00004fd0: 6972 da07 6572 725f 6469 7272 3300 0000  ir..err_dirr3...
 00004fe0: 7234 0000 0072 3500 0000 da07 6570 5f70  r4...r5.....ep_p
-00004ff0: 6174 6872 dc00 0000 630b 0000 0000 0000  athr....c.......
+00004ff0: 6174 6872 dd00 0000 630b 0000 0000 0000  athr....c.......
 00005000: 0001 0000 000c 0000 0006 0000 0003 0000  ................
 00005010: 0073 f400 0000 7400 8300 6a01 7c01 7c06  .s....t...j.|.|.
 00005020: 7c07 7c09 6401 8d04 0100 7c04 6402 6b08  |.|.d.....|.d.k.
 00005030: 7224 7c04 7c00 5f02 6e28 7403 7c04 7404  r$|.|._.n(t.|.t.
 00005040: 6a05 8302 7c00 5f02 7406 6a07 a008 7c00  j...|._.t.j...|.
 00005050: 6a02 a101 734c 7406 a009 7c00 6a02 a101  j...sLt...|.j...
 00005060: 0100 7c0a 7c00 5f0a 7403 7c05 7404 6a0b  ..|.|._.t.|.t.j.
@@ -1355,15 +1355,15 @@
 000054a0: 7265 7373 2062 6172 0a20 2020 2020 2020  ress bar.       
 000054b0: 203a 7061 7261 6d20 6570 775f 6669 6c65   :param epw_file
 000054c0: 3a20 4465 7072 6563 6174 6564 2e20 5573  : Deprecated. Us
 000054d0: 6520 6570 7720 696e 7374 6561 642e 2050  e epw instead. P
 000054e0: 6174 6820 746f 2074 6865 2065 7077 2066  ath to the epw f
 000054f0: 696c 6520 7265 7072 6573 656e 7469 6e67  ile representing
 00005500: 2074 6865 2077 6561 7468 6572 2e0a 2020   the weather..  
-00005510: 2020 2020 2020 7231 0000 004e 72db 0000        r1...Nr...
+00005510: 2020 2020 2020 7231 0000 004e 72dc 0000        r1...Nr...
 00005520: 007a 5265 7077 5f66 696c 6520 616e 6420  .zRepw_file and 
 00005530: 6570 7720 6361 6e6e 6f74 2062 6520 7573  epw cannot be us
 00005540: 6564 2074 6f67 6574 6865 722e 204a 7573  ed together. Jus
 00005550: 7420 7573 6520 6570 772c 2061 7320 6570  t use epw, as ep
 00005560: 7720 6669 6c65 2069 7320 6465 7072 6563  w file is deprec
 00005570: 6174 6564 2e7a 5065 7077 5f66 696c 6520  ated.zPepw_file 
 00005580: 6861 7320 6265 656e 2064 6570 7265 6361  has been depreca
@@ -1377,40 +1377,40 @@
 00005600: 6420 7769 6c6c 2062 6520 7265 6d6f 7665  d will be remove
 00005610: 6420 696e 2074 6865 2066 7574 7572 657a  d in the futurez
 00005620: 1149 6e63 6f72 7265 6374 2076 6572 7369  .Incorrect versi
 00005630: 6f6e 7a04 2e65 7077 7a3d 6570 7720 6172  onz..epwz=epw ar
 00005640: 6775 6d65 6e74 2065 7870 6563 7473 2070  gument expects p
 00005650: 6174 6820 746f 2061 6e20 6570 7720 6669  ath to an epw fi
 00005660: 6c65 2c20 6669 6c65 2070 726f 7669 6465  le, file provide
-00005670: 6420 7761 733a 2029 1a72 b600 0000 723b  d was: ).r....r;
-00005680: 0000 0072 dd00 0000 7204 0000 0072 1100  ...r....r....r..
+00005670: 6420 7761 733a 2029 1a72 b700 0000 723b  d was: ).r....r;
+00005680: 0000 0072 de00 0000 7204 0000 0072 1100  ...r....r....r..
 00005690: 0000 da0b 6f75 745f 7772 6170 7065 72da  ....out_wrapper.
 000056a0: 026f 73da 0470 6174 68da 0665 7869 7374  .os..path..exist
-000056b0: 73da 086d 616b 6564 6972 7372 df00 0000  s..makedirsr....
+000056b0: 73da 086d 616b 6564 6972 7372 e000 0000  s..makedirsr....
 000056c0: da0d 6572 726f 725f 7772 6170 7065 7272  ..error_wrapperr
-000056d0: de00 0000 da08 6275 696c 6469 6e67 da05  ......building..
+000056d0: df00 0000 da08 6275 696c 6469 6e67 da05  ......building..
 000056e0: 6669 6c65 7372 4500 0000 720b 0000 0072  filesrE...r....r
-000056f0: a600 0000 72a5 0000 00da 0565 706c 7573  ....r......eplus
+000056f0: a700 0000 72a6 0000 00da 0565 706c 7573  ....r......eplus
 00005700: da0f 6765 745f 6964 665f 7665 7273 696f  ..get_idf_versio
 00005710: 6eda 0e41 7373 6572 7469 6f6e 4572 726f  n..AssertionErro
-00005720: 7272 af00 0000 da08 656e 6473 7769 7468  rr......endswith
-00005730: 72db 0000 005a 0c65 7077 5f63 6f6e 7465  r....Z.epw_conte
+00005720: 7272 b000 0000 da08 656e 6473 7769 7468  rr......endswith
+00005730: 72dc 0000 005a 0c65 7077 5f63 6f6e 7465  r....Z.epw_conte
 00005740: 6e74 7329 0c72 3a00 0000 7232 0000 0072  nts).r:...r2...r
-00005750: e600 0000 72db 0000 0072 dd00 0000 72de  ....r....r....r.
-00005760: 0000 0072 3300 0000 7234 0000 0072 bb00  ...r3...r4...r..
-00005770: 0000 7235 0000 0072 df00 0000 72dc 0000  ..r5...r....r...
-00005780: 0072 b800 0000 721e 0000 0072 1f00 0000  .r....r....r....
+00005750: e700 0000 72dc 0000 0072 de00 0000 72df  ....r....r....r.
+00005760: 0000 0072 3300 0000 7234 0000 0072 bc00  ...r3...r4...r..
+00005770: 0000 7235 0000 0072 e000 0000 72dd 0000  ..r5...r....r...
+00005780: 0072 b900 0000 721e 0000 0072 1f00 0000  .r....r....r....
 00005790: 723b 0000 006e 0200 0073 4a00 0000 0020  r;...n...sJ.... 
 000057a0: 0601 0201 0201 0201 02fc 0606 0801 0802  ................
 000057b0: 0e01 0e01 0c02 0601 0e02 0603 1201 0201  ................
 000057c0: 02ff 0603 0401 0401 0201 0201 02ff 02ff  ................
 000057d0: 0406 0401 0401 0202 02fd 0405 1602 1a01  ................
 000057e0: 0201 08ff 0403 0603 7a14 4576 616c 7561  ........z.Evalua
 000057f0: 746f 7245 502e 5f5f 696e 6974 5f5f 4672  torEP.__init__Fr
-00005800: 6600 0000 7230 0000 0029 0272 dd00 0000  f...r0...).r....
+00005800: 6600 0000 7230 0000 0029 0272 de00 0000  f...r0...).r....
 00005810: da0b 7374 646f 7574 5f6d 6f64 6529 0472  ..stdout_mode).r
 00005820: 6700 0000 7268 0000 0072 7800 0000 723d  g...rh...rx...r=
 00005830: 0000 0063 0500 0000 0000 0000 0200 0000  ...c............
 00005840: 0b00 0000 0800 0000 0b00 0000 7370 0000  ............sp..
 00005850: 007c 006a 007d 087c 057d 097c 0473 1864  .|.j.}.|.}.|.s.d
 00005860: 0104 007d 057c 005f 0074 0183 006a 027c  ...}.|._.t...j.|
 00005870: 0166 017c 027c 037c 047c 057c 0664 029c  .f.|.|.|.|.|.d..
@@ -1458,27 +1458,27 @@
 00005b10: 7269 6e74 6564 2074 6f20 7374 646f 7574  rinted to stdout
 00005b20: 2e0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
 00005b30: 6e3a 2052 6574 7572 6e73 2061 2044 6174  n: Returns a Dat
 00005b40: 6146 7261 6d65 2077 6974 6820 6f6e 6520  aFrame with one 
 00005b50: 636f 6c75 6d6e 2063 6f6e 7461 696e 696e  column containin
 00005b60: 6720 7468 6520 7265 7375 6c74 7320 666f  g the results fo
 00005b70: 7220 6561 6368 206f 626a 6563 7469 7665  r each objective
-00005b80: 2e0a 2020 2020 2020 2020 4e29 0572 9300  ..        N).r..
-00005b90: 0000 7268 0000 0072 7800 0000 72dd 0000  ..rh...rx...r...
-00005ba0: 0072 ec00 0000 e9ff ffff ffda 0a6f 7574  .r...........out
-00005bb0: 7075 745f 6469 7254 7287 0000 0029 0372  put_dirTr....).r
-00005bc0: 7a00 0000 72c8 0000 0072 8800 0000 2906  z...r....r....).
-00005bd0: 72dd 0000 0072 b600 0000 7294 0000 0072  r....r....r....r
-00005be0: 8f00 0000 727a 0000 0072 9200 0000 290b  ....rz...r....).
-00005bf0: 723a 0000 0072 6700 0000 7293 0000 0072  r:...rg...r....r
-00005c00: 6800 0000 7278 0000 0072 dd00 0000 72ec  h...rx...r....r.
+00005b80: 2e0a 2020 2020 2020 2020 4e29 0572 9400  ..        N).r..
+00005b90: 0000 7268 0000 0072 7800 0000 72de 0000  ..rh...rx...r...
+00005ba0: 0072 ed00 0000 e9ff ffff ffda 0a6f 7574  .r...........out
+00005bb0: 7075 745f 6469 7254 7288 0000 0029 0372  put_dirTr....).r
+00005bc0: 7a00 0000 72c9 0000 0072 8900 0000 2906  z...r....r....).
+00005bd0: 72de 0000 0072 b700 0000 7295 0000 0072  r....r....r....r
+00005be0: 9000 0000 727a 0000 0072 9300 0000 290b  ....rz...r....).
+00005bf0: 723a 0000 0072 6700 0000 7294 0000 0072  r:...rg...r....r
+00005c00: 6800 0000 7278 0000 0072 de00 0000 72ed  h...rx...r....r.
 00005c10: 0000 0072 5100 0000 5a09 7465 6d70 5f73  ...rQ...Z.temp_s
 00005c20: 656c 665a 0874 656d 705f 6f75 7472 5b00  elfZ.temp_outr[.
-00005c30: 0000 72b8 0000 0072 1e00 0000 721f 0000  ..r....r....r...
-00005c40: 0072 9400 0000 be02 0000 7334 0000 0000  .r........s4....
+00005c30: 0000 72b9 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00005c40: 0072 9500 0000 be02 0000 7334 0000 0000  .r........s4....
 00005c50: 1606 0104 0104 010a 0206 0102 ff02 0202  ................
 00005c60: 0102 0102 0102 0102 fa04 0702 f906 0a04  ................
 00005c70: 0104 010c 0002 0002 ff06 0304 0106 0104  ................
 00005c80: 0208 017a 1445 7661 6c75 6174 6f72 4550  ...z.EvaluatorEP
 00005c90: 2e64 665f 6170 706c 7929 0172 4e00 0000  .df_apply).rN...
 00005ca0: 6304 0000 0000 0000 0000 0000 000a 0000  c...............
 00005cb0: 0008 0000 000b 0000 0073 c400 0000 7c02  .........s....|.
@@ -1490,60 +1490,60 @@
 00005d10: 8700 6601 6402 6403 8408 7c00 6a0b 6a0c  ..f.d.d...|.j.j.
 00005d20: 4400 8301 8301 7d07 740a 8700 6601 6404  D.....}.t...f.d.
 00005d30: 6403 8408 7c00 6a0b 6a0d 4400 8301 8301  d...|.j.j.D.....
 00005d40: 7d08 7c07 7c08 1700 7d09 7c00 6a0b 6a0e  }.|.|...}.|.j.j.
 00005d50: 6405 6b09 72a6 7c00 6a0b a00f 7c01 8800  d.k.r.|.j...|...
 00005d60: a102 0100 7c00 a010 a100 0100 7c03 72bc  ....|.......|.r.
 00005d70: 7c09 7c02 6601 1700 5300 7c09 5300 6405  |.|.f...S.|.S.d.
-00005d80: 5300 2906 724f 0000 0029 0572 dd00 0000  S.).rO...).r....
-00005d90: 72de 0000 0072 db00 0000 7233 0000 0072  r....r....r3...r
-00005da0: df00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00005d80: 5300 2906 724f 0000 0029 0572 de00 0000  S.).rO...).r....
+00005d90: 72df 0000 0072 dc00 0000 7233 0000 0072  r....r....r3...r
+00005da0: e000 0000 6301 0000 0000 0000 0000 0000  ....c...........
 00005db0: 0002 0000 0003 0000 0033 0000 0073 1600  .........3...s..
 00005dc0: 0000 7c00 5d0e 7d01 7c01 8800 8301 5600  ..|.].}.|.....V.
 00005dd0: 0100 7102 6400 5300 7218 0000 0072 1e00  ..q.d.S.r....r..
 00005de0: 0000 a902 721b 0000 00da 096f 626a 6563  ....r......objec
 00005df0: 7469 7665 a901 da07 7265 7375 6c74 7372  tive....resultsr
 00005e00: 1e00 0000 721f 0000 0072 2000 0000 0a03  ....r....r .....
 00005e10: 0000 7304 0000 0004 0002 007a 2a45 7661  ..s........z*Eva
 00005e20: 6c75 6174 6f72 4550 2e65 7661 6c5f 7369  luatorEP.eval_si
 00005e30: 6e67 6c65 2e3c 6c6f 6361 6c73 3e2e 3c67  ngle.<locals>.<g
 00005e40: 656e 6578 7072 3e63 0100 0000 0000 0000  enexpr>c........
 00005e50: 0000 0000 0200 0000 0300 0000 3300 0000  ............3...
 00005e60: 7316 0000 007c 005d 0e7d 017c 0188 0083  s....|.].}.|....
 00005e70: 0156 0001 0071 0264 0053 0072 1800 0000  .V...q.d.S.r....
 00005e80: 721e 0000 0029 0272 1b00 0000 da0a 636f  r....).r......co
-00005e90: 6e73 7472 6169 6e74 72f1 0000 0072 1e00  nstraintr....r..
+00005e90: 6e73 7472 6169 6e74 72f2 0000 0072 1e00  nstraintr....r..
 00005ea0: 0000 721f 0000 0072 2000 0000 0c03 0000  ..r....r .......
-00005eb0: 7304 0000 0004 0002 004e 2911 72dd 0000  s........N).r...
-00005ec0: 0072 de00 0000 da02 6566 da0c 6765 6e65  .r......ef..gene
+00005eb0: 7304 0000 0004 0002 004e 2911 72de 0000  s........N).r...
+00005ec0: 0072 df00 0000 da02 6566 da0c 6765 6e65  .r......ef..gene
 00005ed0: 7261 7465 5f64 6972 da1b 5f67 656e 6572  rate_dir.._gener
 00005ee0: 6174 655f 6275 696c 6469 6e67 5f66 726f  ate_building_fro
-00005ef0: 6d5f 726f 7772 e800 0000 da0c 7275 6e5f  m_rowr......run_
-00005f00: 6275 696c 6469 6e67 72db 0000 0072 3300  buildingr....r3.
-00005f10: 0000 72df 0000 0072 2a00 0000 7232 0000  ..r....r*...r2..
-00005f20: 0072 8600 0000 72a8 0000 00da 1061 6464  .r....r......add
+00005ef0: 6d5f 726f 7772 e900 0000 da0c 7275 6e5f  m_rowr......run_
+00005f00: 6275 696c 6469 6e67 72dc 0000 0072 3300  buildingr....r3.
+00005f10: 0000 72e0 0000 0072 2a00 0000 7232 0000  ..r....r*...r2..
+00005f20: 0072 8700 0000 72a9 0000 00da 1061 6464  .r....r......add
 00005f30: 5f6f 7574 7075 7473 5f6c 6973 74da 0e72  _outputs_list..r
-00005f40: 6563 6f72 645f 7265 7375 6c74 7372 a100  ecord_resultsr..
-00005f50: 0000 290a 723a 0000 0072 4e00 0000 72dd  ..).r:...rN...r.
-00005f60: 0000 0072 7800 0000 7251 0000 0072 de00  ...rx...rQ...r..
+00005f40: 6563 6f72 645f 7265 7375 6c74 7372 a200  ecord_resultsr..
+00005f50: 0000 290a 723a 0000 0072 4e00 0000 72de  ..).r:...rN...r.
+00005f60: 0000 0072 7800 0000 7251 0000 0072 df00  ...rx...rQ...r..
 00005f70: 0000 da10 6375 7272 656e 745f 6275 696c  ....current_buil
-00005f80: 6469 6e67 7286 0000 0072 a800 0000 5a11  dingr....r....Z.
+00005f80: 6469 6e67 7287 0000 0072 a900 0000 5a11  dingr....r....Z.
 00005f90: 6578 7472 6163 7465 645f 7265 7375 6c74  extracted_result
-00005fa0: 7372 1e00 0000 72f1 0000 0072 1f00 0000  sr....r....r....
+00005fa0: 7372 1e00 0000 72f2 0000 0072 1f00 0000  sr....r....r....
 00005fb0: 7252 0000 00ee 0200 0073 3600 0000 000e  rR.......s6.....
 00005fc0: 0a01 0601 0401 0e01 0a01 0401 02ff 0202  ................
 00005fd0: 0201 0201 0401 0401 04fa 0407 02f9 0609  ................
 00005fe0: 1a01 0201 14ff 0403 0801 0c01 0e01 0801  ................
 00005ff0: 0401 0a02 7a17 4576 616c 7561 746f 7245  ....z.EvaluatorE
 00006000: 502e 6576 616c 5f73 696e 676c 6563 0100  P.eval_singlec..
 00006010: 0000 0000 0000 0000 0000 0100 0000 0100  ................
 00006020: 0000 4300 0000 7306 0000 007c 006a 0053  ..C...s....|.j.S
 00006030: 0072 1800 0000 2901 da09 5f62 7569 6c64  .r....)..._build
 00006040: 696e 6772 5f00 0000 721e 0000 0072 1e00  ingr_...r....r..
-00006050: 0000 721f 0000 0072 e600 0000 1703 0000  ..r....r........
+00006050: 0000 721f 0000 0072 e700 0000 1703 0000  ..r....r........
 00006060: 7302 0000 0000 027a 1445 7661 6c75 6174  s......z.Evaluat
 00006070: 6f72 4550 2e62 7569 6c64 696e 6772 3c00  orEP.buildingr<.
 00006080: 0000 6302 0000 0000 0000 0000 0000 0003  ..c.............
 00006090: 0000 0004 0000 0043 0000 0073 2800 0000  .......C...s(...
 000060a0: 7c00 6a00 4400 5d0e 7d02 7c02 a001 7c01  |.j.D.].}.|...|.
 000060b0: a101 0100 7106 7c00 a002 a100 0100 7c01  ....q.|.......|.
 000060c0: 7c00 5f03 6401 5300 2902 7a98 4368 616e  |._.d.S.).z.Chan
@@ -1553,24 +1553,24 @@
 00006100: 7320 7265 7365 7473 2074 6865 2063 6163  s resets the cac
 00006110: 6865 2e0a 0a20 2020 2020 2020 203a 7061  he...        :pa
 00006120: 7261 6d20 6e65 775f 6275 696c 6469 6e67  ram new_building
 00006130: 3a20 7468 6520 6275 696c 6469 6e67 2074  : the building t
 00006140: 6f20 7573 650a 2020 2020 2020 2020 3a72  o use.        :r
 00006150: 6574 7572 6e3a 204e 6f6e 650a 2020 2020  eturn: None.    
 00006160: 2020 2020 4e29 0472 3200 0000 da05 7365      N).r2.....se
-00006170: 7475 7072 6000 0000 72fb 0000 0029 0372  tupr`...r....).r
+00006170: 7475 7072 6000 0000 72fc 0000 0029 0372  tupr`...r....).r
 00006180: 3a00 0000 5a0c 6e65 775f 6275 696c 6469  :...Z.new_buildi
 00006190: 6e67 da02 696f 721e 0000 0072 1e00 0000  ng..ior....r....
-000061a0: 721f 0000 0072 e600 0000 1b03 0000 7308  r....r........s.
+000061a0: 721f 0000 0072 e700 0000 1b03 0000 7308  r....r........s.
 000061b0: 0000 0000 080a 010c 0108 0163 0100 0000  ...........c....
 000061c0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
 000061d0: 4300 0000 7306 0000 007c 006a 0053 0072  C...s....|.j.S.r
 000061e0: 1800 0000 2901 da04 5f65 7077 725f 0000  ....)..._epwr_..
 000061f0: 0072 1e00 0000 721e 0000 0072 1f00 0000  .r....r....r....
-00006200: 72db 0000 0028 0300 0073 0200 0000 0002  r....(...s......
+00006200: 72dc 0000 0028 0300 0073 0200 0000 0002  r....(...s......
 00006210: 7a0f 4576 616c 7561 746f 7245 502e 6570  z.EvaluatorEP.ep
 00006220: 7729 0272 2d00 0000 723d 0000 0063 0200  w).r-...r=...c..
 00006230: 0000 0000 0000 0000 0000 0200 0000 0200  ................
 00006240: 0000 4300 0000 7312 0000 007c 00a0 00a1  ..C...s....|....
 00006250: 0001 007c 017c 005f 0164 0153 0029 027a  ...|.|._.d.S.).z
 00006260: ac43 6861 6e67 6573 2074 6865 2065 7077  .Changes the epw
 00006270: 2066 696c 6520 7573 6564 2077 6974 6820   file used with 
@@ -1579,18 +1579,18 @@
 000062a0: 7468 6973 2072 6573 6574 7320 7468 6520  this resets the 
 000062b0: 6361 6368 652e 0a0a 2020 2020 2020 2020  cache...        
 000062c0: 3a70 6172 616d 2076 616c 7565 3a20 7061  :param value: pa
 000062d0: 7468 2074 6f20 7468 6520 6e65 7720 6570  th to the new ep
 000062e0: 7720 6669 6c65 2074 6f20 7573 652e 0a20  w file to use.. 
 000062f0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
 00006300: 4e6f 6e65 0a20 2020 2020 2020 204e 2902  None.        N).
-00006310: 7260 0000 0072 fe00 0000 72c5 0000 0072  r`...r....r....r
-00006320: 1e00 0000 721e 0000 0072 1f00 0000 72db  ....r....r....r.
+00006310: 7260 0000 0072 ff00 0000 72c6 0000 0072  r`...r....r....r
+00006320: 1e00 0000 721e 0000 0072 1f00 0000 72dc  ....r....r....r.
 00006330: 0000 002c 0300 0073 0400 0000 0008 0801  ...,...s........
-00006340: 2904 7267 0000 0072 8e00 0000 da09 6669  ).rg...r......fi
+00006340: 2904 7267 0000 0072 8f00 0000 da09 6669  ).rg...r......fi
 00006350: 6c65 5f6e 616d 6572 3d00 0000 6304 0000  le_namer=...c...
 00006360: 0000 0000 0000 0000 0007 0000 0009 0000  ................
 00006370: 0043 0000 0073 7000 0000 7c01 6a00 a001  .C...sp...|.j...
 00006380: a100 7c02 1900 6401 7402 7c00 6a03 6a04  ..|...d.t.|.j.j.
 00006390: 8301 8502 1900 7d04 7c00 a005 7c04 a101  ......}.|...|...
 000063a0: 7d05 7406 7c05 7407 8302 725c 7408 7c03  }.t.|.t...r\t.|.
 000063b0: 9b00 6402 9d02 6403 8302 8f12 7d06 7409  ..d...d.....}.t.
@@ -1607,19 +1607,19 @@
 00006460: 616d 2066 696c 655f 6e61 6d65 3a20 6669  am file_name: fi
 00006470: 6c65 206e 616d 6520 7573 6564 2074 6f20  le name used to 
 00006480: 7361 7665 2061 732e 0a20 2020 2020 2020  save as..       
 00006490: 203a 7265 7475 726e 3a20 4e6f 6e65 0a20   :return: None. 
 000064a0: 2020 2020 2020 204e 7a07 2e65 704a 534f         Nz..epJSO
 000064b0: 4eda 0177 7a04 2e69 6466 290c 724e 0000  N..wz..idf).rN..
 000064c0: 00da 0674 6f6c 6973 7472 4800 0000 7232  ...tolistrH...r2
-000064d0: 0000 0072 6400 0000 72f6 0000 0072 2600  ...rd...r....r&.
+000064d0: 0000 0072 6400 0000 72f7 0000 0072 2600  ...rd...r....r&.
 000064e0: 0000 7227 0000 00da 046f 7065 6eda 046a  ..r'.....open..j
 000064f0: 736f 6eda 0464 756d 70da 0673 6176 6561  son..dump..savea
-00006500: 7329 0772 3a00 0000 7267 0000 0072 8e00  s).r:...rg...r..
-00006510: 0000 72ff 0000 00da 016c 72fa 0000 00da  ..r......lr.....
+00006500: 7329 0772 3a00 0000 7267 0000 0072 8f00  s).r:...rg...r..
+00006510: 0000 7200 0100 00da 016c 72fb 0000 00da  ..r......lr.....
 00006520: 0266 7072 1e00 0000 721e 0000 0072 1f00  .fpr....r....r..
 00006530: 0000 da11 6765 6e65 7261 7465 5f62 7569  ....generate_bui
 00006540: 6c64 696e 6738 0300 0073 0c00 0000 0008  lding8...s......
 00006550: 1e01 0a01 0a01 1201 1802 7a1d 4576 616c  ..........z.Eval
 00006560: 7561 746f 7245 502e 6765 6e65 7261 7465  uatorEP.generate
 00006570: 5f62 7569 6c64 696e 6763 0200 0000 0000  _buildingc......
 00006580: 0000 0000 0000 0500 0000 0500 0000 4300  ..............C.
@@ -1634,65 +1634,65 @@
 00006610: 6469 6e67 2066 726f 6d20 6120 726f 7720  ding from a row 
 00006620: 6f66 2064 6174 6163 0100 0000 0000 0000  of datac........
 00006630: 0000 0000 0300 0000 0400 0000 5300 0000  ............S...
 00006640: 7316 0000 0069 007c 005d 0e5c 027d 017d  s....i.|.].\.}.}
 00006650: 027c 017c 0293 0271 0453 0072 1e00 0000  .|.|...q.S.r....
 00006660: 721e 0000 00a9 0372 1b00 0000 7265 0000  r......r....re..
 00006670: 0072 2d00 0000 721e 0000 0072 1e00 0000  .r-...r....r....
-00006680: 721f 0000 0072 8500 0000 4e03 0000 7306  r....r....N...s.
+00006680: 721f 0000 0072 8600 0000 4e03 0000 7306  r....r....N...s.
 00006690: 0000 0006 0206 ff02 007a 3b45 7661 6c75  .........z;Evalu
 000066a0: 6174 6f72 4550 2e5f 6765 6e65 7261 7465  atorEP._generate
 000066b0: 5f62 7569 6c64 696e 675f 6672 6f6d 5f72  _building_from_r
 000066c0: 6f77 2e3c 6c6f 6361 6c73 3e2e 3c64 6963  ow.<locals>.<dic
 000066d0: 7463 6f6d 703e 2909 7256 0000 00da 0463  tcomp>).rV.....c
-000066e0: 6f70 79da 0864 6565 7063 6f70 7972 e600  opy..deepcopyr..
+000066e0: 6f70 79da 0864 6565 7063 6f70 7972 e700  opy..deepcopyr..
 000066f0: 0000 724a 0000 0072 3200 0000 7264 0000  ..rJ...r2...rd..
 00006700: 00da 0a70 6172 616d 6574 6572 73da 1774  ...parameters..t
 00006710: 7261 6e73 666f 726d 6174 696f 6e5f 6675  ransformation_fu
-00006720: 6e63 7469 6f6e 2905 723a 0000 0072 7f00  nction).r:...r..
-00006730: 0000 72fa 0000 0072 4e00 0000 da09 7061  ..r....rN.....pa
+00006720: 6e63 7469 6f6e 2905 723a 0000 0072 8000  nction).r:...r..
+00006730: 0000 72fb 0000 0072 4e00 0000 da09 7061  ..r....rN.....pa
 00006740: 7261 6d65 7465 7272 1e00 0000 721e 0000  rameterr....r...
-00006750: 0072 1f00 0000 72f6 0000 004a 0300 0073  .r....r....J...s
+00006750: 0072 1f00 0000 72f7 0000 004a 0300 0073  .r....r....J...s
 00006760: 1000 0000 0002 0a01 0c01 0602 0cfe 0607  ................
 00006770: 0c01 0e01 7a27 4576 616c 7561 746f 7245  ....z'EvaluatorE
 00006780: 502e 5f67 656e 6572 6174 655f 6275 696c  P._generate_buil
 00006790: 6469 6e67 5f66 726f 6d5f 726f 7729 0346  ding_from_row).F
-000067a0: 7266 0000 0046 2902 4e46 291a 72ab 0000  rf...F).NF).r...
-000067b0: 0072 ac00 0000 72ad 0000 0072 ae00 0000  .r....r....r....
-000067c0: 7211 0000 0072 e700 0000 72dd 0000 0072  r....r....r....r
-000067d0: de00 0000 7216 0000 0072 1700 0000 72af  ....r....r....r.
-000067e0: 0000 0072 0600 0000 720a 0000 0072 b000  ...r....r....r..
-000067f0: 0000 723b 0000 0072 b100 0000 72a3 0000  ..r;...r....r...
-00006800: 0072 9400 0000 7252 0000 0072 d800 0000  .r....rR...r....
-00006810: 72e6 0000 0072 d900 0000 72db 0000 0072  r....r....r....r
-00006820: 0801 0000 72f6 0000 0072 ba00 0000 721e  ....r....r....r.
-00006830: 0000 0072 1e00 0000 72b8 0000 0072 1f00  ...r....r....r..
-00006840: 0000 72da 0000 006a 0200 0073 6200 0000  ..r....j...sb...
+000067a0: 7266 0000 0046 2902 4e46 291a 72ac 0000  rf...F).NF).r...
+000067b0: 0072 ad00 0000 72ae 0000 0072 af00 0000  .r....r....r....
+000067c0: 7211 0000 0072 e800 0000 72de 0000 0072  r....r....r....r
+000067d0: df00 0000 7216 0000 0072 1700 0000 72b0  ....r....r....r.
+000067e0: 0000 0072 0600 0000 720a 0000 0072 b100  ...r....r....r..
+000067f0: 0000 723b 0000 0072 b200 0000 72a4 0000  ..r;...r....r...
+00006800: 0072 9500 0000 7252 0000 0072 d900 0000  .r....rR...r....
+00006810: 72e7 0000 0072 da00 0000 72dc 0000 0072  r....r....r....r
+00006820: 0901 0000 72f7 0000 0072 bb00 0000 721e  ....r....r....r.
+00006830: 0000 0072 1e00 0000 72b9 0000 0072 1f00  ...r....r....r..
+00006840: 0000 72db 0000 006a 0200 0073 6200 0000  ..r....j...sb...
 00006850: 0801 0407 0801 0401 0401 0201 0201 0201  ................
 00006860: 0201 02f5 020d 02f3 0402 0202 0201 0201  ................
 00006870: 0201 0201 0602 0201 0202 02f3 1053 0001  .............S..
 00006880: 0001 00fb 0207 0401 02f8 0402 0202 0201  ................
 00006890: 0205 02f6 1033 0001 00fc 0202 02fe 0c29  .....3.........)
 000068a0: 0201 0a03 0401 100c 0201 1003 0401 120b  ................
-000068b0: 1412 72da 0000 0063 0000 0000 0000 0000  ..r....c........
+000068b0: 1412 72db 0000 0063 0000 0000 0000 0000  ..r....c........
 000068c0: 0000 0000 0000 0000 0800 0000 0000 0000  ................
 000068d0: 7364 0000 0065 005a 0164 005a 0264 015a  sd...e.Z.d.Z.d.Z
 000068e0: 0365 046a 0565 046a 0664 0264 0364 0466  .e.j.e.j.d.d.d.f
 000068f0: 0565 0765 0865 0865 0965 0a65 0b19 0065  .e.e.e.e.e.e...e
 00006900: 0c64 059c 0687 0066 0164 0664 0784 0d5a  .d.....f.d.d...Z
 00006910: 0d65 0b64 0364 089c 0264 0964 0a84 045a  .e.d.d...d.d...Z
 00006920: 0e65 0b65 0f64 089c 0264 0b64 0c84 045a  .e.e.d...d.d...Z
 00006930: 1087 0004 005a 1153 0029 0dda 0b45 7661  .....Z.S.)...Eva
 00006940: 6c75 6174 6f72 4548 7a49 5468 6973 2065  luatorEHzIThis e
 00006950: 7661 6c75 6174 6f72 2075 7365 7320 6120  valuator uses a 
 00006960: 5072 6f62 6c65 6d20 746f 206d 6f64 6966  Problem to modif
 00006970: 7920 616e 2065 6e65 7267 7920 6875 622c  y an energy hub,
 00006980: 2061 6e64 2074 6865 6e20 736f 6c76 6520   and then solve 
 00006990: 6974 2e72 2f00 0000 4e54 2906 7232 0000  it.r/...NT).r2..
-000069a0: 0072 dd00 0000 72de 0000 0072 3300 0000  .r....r....r3...
+000069a0: 0072 de00 0000 72df 0000 0072 3300 0000  .r....r....r3...
 000069b0: 7234 0000 0072 3500 0000 6308 0000 0000  r4...r5...c.....
 000069c0: 0000 0000 0000 0008 0000 0006 0000 0003  ................
 000069d0: 0000 0073 3800 0000 7400 8300 6a01 7c01  ...s8...t...j.|.
 000069e0: 7c05 7c06 7c07 6401 8d04 0100 7c03 7c00  |.|.|.d.....|.|.
 000069f0: 5f02 7c04 7c00 5f03 7c02 7c00 5f04 7c01  _.|.|._.|.|._.|.
 00006a00: 7c00 5f05 7406 6a07 7c00 5f08 6402 5300  |._.t.j.|._.d.S.
 00006a10: 2903 612f 0300 000a 0a20 2020 2020 2020  ).a/.....       
@@ -1742,22 +1742,22 @@
 00006cd0: 6e63 6f6d 7061 7469 626c 6520 7769 7468  ncompatible with
 00006ce0: 2065 7272 6f72 5f6d 6f64 653d 2746 6169   error_mode='Fai
 00006cf0: 6c66 6173 7427 2e0a 2020 2020 2020 2020  lfast'..        
 00006d00: 3a70 6172 616d 2070 726f 6772 6573 735f  :param progress_
 00006d10: 6261 723a 2077 6865 7468 6572 206f 7220  bar: whether or 
 00006d20: 6e6f 7420 746f 2064 6973 706c 6179 2061  not to display a
 00006d30: 2070 726f 6772 6573 7320 6261 720a 2020   progress bar.  
-00006d40: 2020 2020 2020 7231 0000 004e 2909 72b6        r1...N).r.
-00006d50: 0000 0072 3b00 0000 72dd 0000 0072 de00  ...r;...r....r..
+00006d40: 2020 2020 2020 7231 0000 004e 2909 72b7        r1...N).r.
+00006d50: 0000 0072 3b00 0000 72de 0000 0072 df00  ...r;...r....r..
 00006d60: 0000 da03 6875 6272 3200 0000 7211 0000  ....hubr2...r...
 00006d70: 00da 0f73 6f6c 7665 725f 7365 7474 696e  ...solver_settin
 00006d80: 6773 da0f 636f 6e66 6967 5f73 6574 7469  gs..config_setti
 00006d90: 6e67 7329 0872 3a00 0000 7232 0000 0072  ngs).r:...r2...r
-00006da0: 1001 0000 72dd 0000 0072 de00 0000 7233  ....r....r....r3
-00006db0: 0000 0072 3400 0000 7235 0000 0072 b800  ...r4...r5...r..
+00006da0: 1101 0000 72de 0000 0072 df00 0000 7233  ....r....r....r3
+00006db0: 0000 0072 3400 0000 7235 0000 0072 b900  ...r4...r5...r..
 00006dc0: 0000 721e 0000 0072 1f00 0000 723b 0000  ..r....r....r;..
 00006dd0: 005d 0300 0073 1600 0000 0018 0601 0201  .]...s..........
 00006de0: 0201 0201 02fc 0606 0601 0601 0601 0601  ................
 00006df0: 7a14 4576 616c 7561 746f 7245 482e 5f5f  z.EvaluatorEH.__
 00006e00: 696e 6974 5f5f 724d 0000 0063 0200 0000  init__rM...c....
 00006e10: 0000 0000 0000 0000 0200 0000 0600 0000  ................
 00006e20: 4300 0000 7332 0000 0074 007c 0183 017c  C...s2...t.|...|
@@ -1787,89 +1787,89 @@
 00006fa0: 6601 640b 640c 8408 7c05 4400 8301 8301  f.d.d...|.D.....
 00006fb0: 7d08 7c00 6a05 6a13 6400 6b09 72e4 7c00  }.|.j.j.d.k.r.|.
 00006fc0: 6a05 a014 7c01 8800 a102 0100 7c00 a015  j...|.......|...
 00006fd0: a100 0100 7c08 5300 290d 4e63 0100 0000  ....|.S.).Nc....
 00006fe0: 0000 0000 0000 0000 0300 0000 0400 0000  ................
 00006ff0: 5300 0000 7316 0000 0069 007c 005d 0e5c  S...s....i.|.].\
 00007000: 027d 017d 027c 017c 0293 0271 0453 0072  .}.}.|.|...q.S.r
-00007010: 1e00 0000 721e 0000 0072 0901 0000 721e  ....r....r....r.
-00007020: 0000 0072 1e00 0000 721f 0000 0072 8500  ...r....r....r..
+00007010: 1e00 0000 721e 0000 0072 0a01 0000 721e  ....r....r....r.
+00007020: 0000 0072 1e00 0000 721f 0000 0072 8600  ...r....r....r..
 00007030: 0000 8e03 0000 7306 0000 0006 0206 ff02  ......s.........
 00007040: 007a 2b45 7661 6c75 6174 6f72 4548 2e65  .z+EvaluatorEH.e
 00007050: 7661 6c5f 7369 6e67 6c65 2e3c 6c6f 6361  val_single.<loca
-00007060: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7286  ls>.<dictcomp>r.
+00007060: 6c73 3e2e 3c64 6963 7463 6f6d 703e 7287  ls>.<dictcomp>r.
 00007070: 0000 0072 0100 0000 da0b 6f75 7470 7574  ...r......output
 00007080: 5f66 696c 65da 0873 6f6c 7574 696f 6eda  _file..solution.
 00007090: 056f 7468 6572 da10 6361 7061 6369 7479  .other..capacity
 000070a0: 5f73 746f 7261 6765 da0d 6361 7061 6369  _storage..capaci
 000070b0: 7479 5f74 6563 6829 025a 0a74 696d 655f  ty_tech).Z.time_
 000070c0: 7374 6570 73da 0673 6865 6574 7363 0100  steps..sheetsc..
 000070d0: 0000 0000 0000 0000 0000 0200 0000 0500  ................
 000070e0: 0000 3300 0000 7320 0000 007c 005d 187d  ..3...s ...|.].}
 000070f0: 0174 00a0 0188 0064 0019 007c 0167 01a1  .t.....d...|.g..
-00007100: 0256 0001 0071 0264 0153 0029 0272 1401  .V...q.d.S.).r..
+00007100: 0256 0001 0071 0264 0153 0029 0272 1501  .V...q.d.S.).r..
 00007110: 0000 4e29 02da 0270 66da 0b67 6574 5f62  ..N)...pf..get_b
-00007120: 795f 7061 7468 72ef 0000 0072 f100 0000  y_pathr....r....
+00007120: 795f 7061 7468 72f0 0000 0072 f200 0000  y_pathr....r....
 00007130: 721e 0000 0072 1f00 0000 7220 0000 00a7  r....r....r ....
 00007140: 0300 0073 0400 0000 0402 02ff 7a2a 4576  ...s........z*Ev
 00007150: 616c 7561 746f 7245 482e 6576 616c 5f73  aluatorEH.eval_s
 00007160: 696e 676c 652e 3c6c 6f63 616c 733e 2e3c  ingle.<locals>.<
-00007170: 6765 6e65 7870 723e 2916 720a 0100 0072  genexpr>).r....r
-00007180: 0b01 0000 7210 0100 0072 5600 0000 724a  ....r....rV...rJ
-00007190: 0000 0072 3200 0000 7264 0000 0072 0c01  ...r2...rd...r..
-000071a0: 0000 720d 0100 0072 5900 0000 da07 636f  ..r....rY.....co
-000071b0: 6d70 696c 6572 f000 0000 da05 736f 6c76  mpiler......solv
-000071c0: 6572 dd00 0000 7212 0100 0072 0f00 0000  er....r....r....
+00007170: 6765 6e65 7870 723e 2916 720b 0100 0072  genexpr>).r....r
+00007180: 0c01 0000 7211 0100 0072 5600 0000 724a  ....r....rV...rJ
+00007190: 0000 0072 3200 0000 7264 0000 0072 0d01  ...r2...rd...r..
+000071a0: 0000 720e 0100 0072 5900 0000 da07 636f  ..r....rY.....co
+000071b0: 6d70 696c 6572 f100 0000 da05 736f 6c76  mpiler......solv
+000071c0: 6572 de00 0000 7213 0100 0072 0f00 0000  er....r....r....
 000071d0: 7248 0000 0072 6a00 0000 722a 0000 0072  rH...rj...r*...r
-000071e0: f800 0000 72f9 0000 0072 a100 0000 2909  ....r....r....).
+000071e0: f900 0000 72fa 0000 0072 a200 0000 2909  ....r....r....).
 000071f0: 723a 0000 0072 4e00 0000 5a0b 6375 7272  r:...rN...Z.curr
 00007200: 656e 745f 6875 625a 0b76 616c 7565 5f70  ent_hubZ.value_p
-00007210: 6169 7273 720e 0100 0072 a700 0000 5a11  airsr....r....Z.
+00007210: 6169 7273 720f 0100 0072 a800 0000 5a11  airsr....r....Z.
 00007220: 7072 696d 6172 795f 6f62 6a65 6374 6976  primary_objectiv
-00007230: 6572 1301 0000 7286 0000 0072 1e00 0000  er....r....r....
-00007240: 72f1 0000 0072 1f00 0000 7252 0000 0089  r....r....rR....
+00007230: 6572 1401 0000 7287 0000 0072 1e00 0000  er....r....r....
+00007240: 72f2 0000 0072 1f00 0000 7252 0000 0089  r....r....rR....
 00007250: 0300 0073 3c00 0000 0001 0c03 0a01 0602  ...s<...........
 00007260: 0cfe 0604 0c01 0e02 0c01 0801 0801 0602  ................
 00007270: 0802 0a01 0a01 0c01 0201 0601 0401 0801  ................
 00007280: 08fc 0607 0201 0a02 02fe 04ff 0406 0c01  ................
 00007290: 0e01 0802 7a17 4576 616c 7561 746f 7245  ....z.EvaluatorE
 000072a0: 482e 6576 616c 5f73 696e 676c 6529 1272  H.eval_single).r
-000072b0: ab00 0000 72ac 0000 0072 ad00 0000 72ae  ....r....r....r.
-000072c0: 0000 0072 1100 0000 72dd 0000 0072 de00  ...r....r....r..
-000072d0: 0000 7216 0000 0072 1700 0000 72af 0000  ..r....r....r...
-000072e0: 0072 0600 0000 720a 0000 0072 b000 0000  .r....r....r....
+000072b0: ac00 0000 72ad 0000 0072 ae00 0000 72af  ....r....r....r.
+000072c0: 0000 0072 1100 0000 72de 0000 0072 df00  ...r....r....r..
+000072d0: 0000 7216 0000 0072 1700 0000 72b0 0000  ..r....r....r...
+000072e0: 0072 0600 0000 720a 0000 0072 b100 0000  .r....r....r....
 000072f0: 723b 0000 0072 5600 0000 722a 0000 0072  r;...rV...r*...r
-00007300: 5200 0000 72ba 0000 0072 1e00 0000 721e  R...r....r....r.
-00007310: 0000 0072 b800 0000 721f 0000 0072 0f01  ...r....r....r..
+00007300: 5200 0000 72bb 0000 0072 1e00 0000 721e  R...r....r....r.
+00007310: 0000 0072 b900 0000 721f 0000 0072 1001  ...r....r....r..
 00007320: 0000 5a03 0000 7320 0000 0008 0104 0604  ..Z...s ........
 00007330: 0104 0102 0102 0102 f802 0202 0202 0102  ................
-00007340: 0102 0106 0102 f810 2510 0772 0f01 0000  ........%..r....
-00007350: 2937 72ae 0000 0072 0a01 0000 7203 0100  )7r....r....r...
-00007360: 0072 e100 0000 726a 0000 0072 a500 0000  .r....rj...r....
+00007340: 0102 0106 0102 f810 2510 0772 1001 0000  ........%..r....
+00007350: 2937 72af 0000 0072 0b01 0000 7204 0100  )7r....r....r...
+00007360: 0072 e200 0000 726a 0000 0072 a600 0000  .r....rj...r....
 00007370: da03 6162 6372 0200 0000 7203 0000 00da  ..abcr....r.....
 00007380: 0770 6174 686c 6962 7204 0000 00da 0674  .pathlibr......t
 00007390: 7970 696e 6772 0500 0000 7206 0000 0072  ypingr....r....r
 000073a0: 0700 0000 7208 0000 0072 0900 0000 720a  ....r....r....r.
 000073b0: 0000 0072 0b00 0000 da05 6e75 6d70 7972  ...r......numpyr
-000073c0: 6d00 0000 da06 7061 6e64 6173 728a 0000  m.....pandasr...
-000073d0: 0072 b200 0000 da04 7961 6d6c 5a0e 6461  .r......yamlZ.da
+000073c0: 6d00 0000 da06 7061 6e64 6173 728b 0000  m.....pandasr...
+000073d0: 0072 b300 0000 da04 7961 6d6c 5a0e 6461  .r......yamlZ.da
 000073e0: 736b 2e64 6174 6166 7261 6d65 720c 0000  sk.dataframer...
 000073f0: 00da 1164 6570 7265 6361 7465 642e 7370  ...deprecated.sp
-00007400: 6869 6e78 720d 0000 0072 0e00 0000 72b1  hinxr....r....r.
+00007400: 6869 6e78 720d 0000 0072 0e00 0000 72b2  hinxr....r....r.
 00007410: 0000 005a 1070 7965 6875 622e 6f75 7470  ...Z.pyehub.outp
 00007420: 7574 7465 7272 0f00 0000 5a09 7471 646d  utterr....Z.tqdm
 00007430: 2e61 7574 6f72 1000 0000 da05 6265 736f  .autor......beso
-00007440: 7372 1100 0000 7212 0000 0072 e800 0000  sr....r....r....
-00007450: 7213 0000 0072 f400 0000 7214 0000 0072  r....r....r....r
-00007460: 1901 0000 7215 0000 00da 0d62 6573 6f73  ....r......besos
+00007440: 7372 1100 0000 7212 0000 0072 e900 0000  sr....r....r....
+00007450: 7213 0000 0072 f500 0000 7214 0000 0072  r....r....r....r
+00007460: 1a01 0000 7215 0000 00da 0d62 6573 6f73  ....r......besos
 00007470: 2e70 726f 626c 656d 7216 0000 00da 1062  .problemr......b
 00007480: 6573 6f73 2e62 6573 6f73 7479 7065 7372  esos.besostypesr
-00007490: 1700 0000 721a 0000 0072 2e00 0000 72b4  ....r....r....r.
-000074a0: 0000 0072 bd00 0000 72be 0000 0072 da00  ...r....r....r..
-000074b0: 0000 720f 0100 0072 1e00 0000 721e 0000  ..r....r....r...
+00007490: 1700 0000 721a 0000 0072 2e00 0000 72b5  ....r....r....r.
+000074a0: 0000 0072 be00 0000 72bf 0000 0072 db00  ...r....r....r..
+000074b0: 0000 7210 0100 0072 1e00 0000 721e 0000  ..r....r....r...
 000074c0: 0072 1e00 0000 721f 0000 00da 083c 6d6f  .r....r......<mo
 000074d0: 6475 6c65 3e01 0000 0073 5000 0000 040c  dule>....sP.....
 000074e0: 0801 0801 0801 0801 0801 1001 0c01 2001  .............. .
 000074f0: 0c03 0801 0801 0801 0801 0c01 0c01 0c01  ................
 00007500: 0c01 0c03 0c01 0c01 0c01 0c01 0c01 0c01  ................
 00007510: 0c03 081b 107f 007f 0059 1027 0201 0201  .........Y.'....
 00007520: 02fe 0404 120a 127f 0018 127f 0071       .............q
```

### Comparing `besos-2.2.0/besos/__pycache__/objectives.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/objectives.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/optimizer.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/optimizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/parameters.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/parameters.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/problem.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/problem.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/pyehub_funcs.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/pyehub_funcs.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Oct 30 00:54:36 2023 UTC, .py size: 4719 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 ccfe 3e65 6f12 0000  U.........>eo...
+00000000: 550d 0d0a 0000 0000 bf6e 4065 6f12 0000  U........n@eo...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
 00000030: 5a00 6401 6402 6c01 5a01 6401 6403 6c02  Z.d.d.l.Z.d.d.l.
 00000040: 6d03 5a03 0100 6401 6404 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6401 6402 6c06 5a07 6401 6402 6c08  ..d.d.l.Z.d.d.l.
 00000060: 5a09 6401 6402 6c0a 5a0a 6401 6405 6c0b  Z.d.d.l.Z.d.d.l.
 00000070: 6d0b 5a0b 0100 6401 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
@@ -34,48 +34,48 @@
 00000210: 0000 7400 8300 7d00 7401 6a02 6a03 7c00  ..t...}.t.j.j.|.
 00000220: 6401 8d01 7d01 7c01 5300 2902 7a34 4765  d...}.|.S.).z4Ge
 00000230: 6e65 7261 7465 7320 7468 6520 6261 7365  nerates the base
 00000240: 2050 7945 4875 6220 6d6f 6465 6c20 6672   PyEHub model fr
 00000250: 6f6d 2074 6865 2065 7863 656c 2066 696c  om the excel fil
 00000260: 652e 2901 da05 6578 6365 6c29 0472 0b00  e.)...excel).r..
 00000270: 0000 da06 7079 6568 7562 5a0a 656e 6572  ....pyehubZ.ener
-00000280: 6779 5f68 7562 7205 0000 0029 02da 0964  gy_hubr....)...d
+00000280: 6779 5f68 7562 7205 0000 0029 025a 0964  gy_hubr....).Z.d
 00000290: 6174 615f 6669 6c65 da05 6d6f 6465 6c72  ata_file..modelr
 000002a0: 0900 0000 7209 0000 0072 0a00 0000 da07  ....r....r......
 000002b0: 6765 745f 6875 621c 0000 0073 0600 0000  get_hub....s....
-000002c0: 0003 0601 0e01 7210 0000 0063 0200 0000  ......r....c....
+000002c0: 0003 0601 0e01 720f 0000 0063 0200 0000  ......r....c....
 000002d0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
 000002e0: 4300 0000 730e 0000 0074 0074 016a 027c  C...s....t.t.j.|
 000002f0: 017c 0083 0353 0029 017a 5941 6363 6573  .|...S.).zYAcces
 00000300: 7320 6120 6e65 7374 6564 206f 626a 6563  s a nested objec
 00000310: 7420 696e 2072 6f6f 7420 6279 2069 7465  t in root by ite
 00000320: 6d20 7365 7175 656e 6365 2e20 5573 6564  m sequence. Used
 00000330: 2074 6f20 6e61 7669 6761 7465 2050 7945   to navigate PyE
 00000340: 4875 6227 7320 6e6f 7420 666c 6174 2064  Hub's not flat d
 00000350: 6963 742e 2903 7202 0000 00da 086f 7065  ict.).r......ope
 00000360: 7261 746f 72da 0767 6574 6974 656d 2902  rator..getitem).
 00000370: da04 726f 6f74 da05 6974 656d 7372 0900  ..root..itemsr..
 00000380: 0000 7209 0000 0072 0a00 0000 da0b 6765  ..r....r......ge
 00000390: 745f 6279 5f70 6174 6824 0000 0073 0200  t_by_path$...s..
-000003a0: 0000 0003 7215 0000 0063 0300 0000 0000  ....r....c......
+000003a0: 0000 0003 7214 0000 0063 0300 0000 0000  ....r....c......
 000003b0: 0000 0000 0000 0300 0000 0600 0000 4300  ..............C.
 000003c0: 0000 731e 0000 007c 0274 007c 007c 0164  ..s....|.t.|.|.d
 000003d0: 0164 0285 0219 0083 027c 0164 0219 003c  .d.......|.d...<
 000003e0: 0064 0153 0029 037a 6653 6574 2061 2076  .d.S.).zfSet a v
 000003f0: 616c 7565 2069 6e20 6120 6e65 7374 6564  alue in a nested
 00000400: 206f 626a 6563 7420 696e 2072 6f6f 7420   object in root 
 00000410: 6279 2069 7465 6d20 7365 7175 656e 6365  by item sequence
 00000420: 2e20 5573 6564 2074 6f20 7365 7420 7661  . Used to set va
 00000430: 6c75 6573 2069 6e20 5079 4548 7562 2773  lues in PyEHub's
 00000440: 206e 6f74 2066 6c61 7420 6469 6374 2e4e   not flat dict.N
-00000450: e9ff ffff ff29 0172 1500 0000 2903 7213  .....).r....).r.
-00000460: 0000 0072 1400 0000 da05 7661 6c75 6572  ...r......valuer
+00000450: e9ff ffff ff29 0172 1400 0000 2903 7212  .....).r....).r.
+00000460: 0000 0072 1300 0000 da05 7661 6c75 6572  ...r......valuer
 00000470: 0900 0000 7209 0000 0072 0a00 0000 da0b  ....r....r......
 00000480: 7365 745f 6279 5f70 6174 682a 0000 0073  set_by_path*...s
-00000490: 0200 0000 0002 7218 0000 007a 0532 2e30  ......r....z.2.0
+00000490: 0200 0000 0002 7217 0000 007a 0532 2e30  ......r....z.2.0
 000004a0: 2e30 7a64 4675 6e63 7469 6f6e 2072 652d  .0zdFunction re-
 000004b0: 696d 706c 656d 656e 7473 2074 6865 2065  implements the e
 000004c0: 7661 6c75 6174 6f72 2773 2073 6574 2070  valuator's set p
 000004d0: 6861 7365 2c20 616e 6420 6361 6e6e 6f74  hase, and cannot
 000004e0: 2068 616e 646c 6520 7061 7261 6d65 7465   handle paramete
 000004f0: 7273 2077 6974 6820 6d75 6c74 6970 6c65  rs with multiple
 00000500: 2069 6e70 7574 732e 2902 da07 7665 7273   inputs.)...vers
@@ -92,20 +92,20 @@
 000005b0: 7920 6875 6220 666f 7220 7468 6520 7061  y hub for the pa
 000005c0: 7261 6d65 7465 7273 2073 7065 6369 6669  rameters specifi
 000005d0: 6564 0a20 2020 206f 6e20 696e 6974 6961  ed.    on initia
 000005e0: 6c69 7a61 7469 6f6e 2077 6974 6820 7468  lization with th
 000005f0: 6520 7661 6c75 6573 2067 6976 656e 2074  e values given t
 00000600: 6f20 6576 616c 7561 746f 722e 4e29 03da  o evaluator.N)..
 00000610: 037a 6970 da08 7365 6c65 6374 6f72 da03  .zip..selector..
-00000620: 7365 7429 05da 0368 7562 721b 0000 0072  set)...hubr....r
-00000630: 1c00 0000 da09 7061 7261 6d65 7465 7272  ......parameterr
-00000640: 1700 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+00000620: 7365 7429 055a 0368 7562 721a 0000 0072  set).Z.hubr....r
+00000630: 1b00 0000 da09 7061 7261 6d65 7465 7272  ......parameterr
+00000640: 1600 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
 00000650: 0000 00da 1770 7965 6875 625f 7061 7261  .....pyehub_para
 00000660: 6d65 7465 725f 6564 6974 6f72 3000 0000  meter_editor0...
-00000670: 7304 0000 0000 0a12 0172 2200 0000 6301  s........r"...c.
+00000670: 7304 0000 0000 0a12 0172 2000 0000 6301  s........r ...c.
 00000680: 0000 0000 0000 0000 0000 0003 0000 0003  ................
 00000690: 0000 0043 0000 0073 2c00 0000 7c00 a000  ...C...s,...|...
 000006a0: 6401 a101 7d01 7c01 a001 a100 7d01 7c00  d...}.|.....}.|.
 000006b0: a002 6401 a101 7d02 7c02 a001 a100 7d02  ..d...}.|.....}.
 000006c0: 7c01 7c02 6602 5300 2902 7a8a 0a20 2020  |.|.f.S.).z..   
 000006d0: 2053 706c 6974 7320 7468 6520 686f 7572   Splits the hour
 000006e0: 6c79 2073 6572 6965 7320 6f66 2045 5020  ly series of EP 
@@ -114,19 +114,19 @@
 00000710: 6c65 2064 6179 7320 696e 2064 6966 6665  le days in diffe
 00000720: 7265 6e74 2073 6561 736f 6e73 2069 6e74  rent seasons int
 00000730: 6f20 7370 6563 6966 6963 2065 6e65 7267  o specific energ
 00000740: 7968 7562 2074 696d 6520 7365 7269 6573  yhub time series
 00000750: 2e0a 2020 2020 e918 0000 0029 03da 0468  ..    .....)...h
 00000760: 6561 64da 0b72 6573 6574 5f69 6e64 6578  ead..reset_index
 00000770: da04 7461 696c 2903 5a0d 686f 7572 6c79  ..tail).Z.hourly
-00000780: 5f73 6572 6965 73da 0772 6573 756c 7431  _series..result1
+00000780: 5f73 6572 6965 735a 0772 6573 756c 7431  _seriesZ.result1
 00000790: da07 7265 7375 6c74 3272 0900 0000 7209  ..result2r....r.
 000007a0: 0000 0072 0a00 0000 da0e 5f73 706c 6974  ...r......_split
 000007b0: 5f45 505f 6461 7973 3e00 0000 730a 0000  _EP_days>...s...
-000007c0: 0000 050a 0108 010a 0108 0172 2900 0000  ...........r)...
+000007c0: 0000 050a 0108 010a 0108 0172 2600 0000  ...........r&...
 000007d0: 6302 0000 0000 0000 0000 0000 0011 0000  c...............
 000007e0: 0006 0000 0043 0000 0073 f000 0000 7c00  .....C...s....|.
 000007f0: a000 a100 7d02 6700 7d03 7c02 4400 5d0e  ....}.g.}.|.D.].
 00000800: 7d04 7c03 a001 7c04 a101 0100 7110 7402  }.|...|.....q.t.
 00000810: 6a03 7c03 6401 8d01 7d05 7c02 4400 5dba  j.|.d...}.|.D.].
 00000820: 7d06 7c02 7c06 1900 4400 5dac 7d07 7c02  }.|.|...D.].}.|.
 00000830: 7c06 1900 7c07 1900 a004 a100 7d08 7405  |...|.......}.t.
@@ -146,42 +146,42 @@
 00000910: 5079 4548 7562 2063 6f6d 7061 7469 626c  PyEHub compatibl
 00000920: 6520 696e 7075 7473 2e0a 2020 2020 2901  e inputs..    ).
 00000930: da07 636f 6c75 6d6e 7369 80ee 3600 da05  ..columnsi..6...
 00000940: 5661 6c75 6554 2901 da0c 6967 6e6f 7265  ValueT)...ignore
 00000950: 5f69 6e64 6578 2909 da07 746f 5f64 6963  _index)...to_dic
 00000960: 74da 0661 7070 656e 64da 0270 64da 0944  t..append..pd..D
 00000970: 6174 6146 7261 6d65 da08 746f 5f66 7261  ataFrame..to_fra
-00000980: 6d65 7229 0000 00da 026e 70da 0561 7272  mer).....np..arr
+00000980: 6d65 7226 0000 00da 026e 70da 0561 7272  mer&.....np..arr
 00000990: 6179 da06 636f 6e63 6174 2911 da05 696e  ay..concat)...in
-000009a0: 7075 74da 0a69 6e64 6578 5f73 697a 655a  put..index_sizeZ
+000009a0: 7075 74da 0a69 6e64 6578 5f73 697a 65da  put..index_size.
 000009b0: 0a69 6e70 7574 5f64 6963 745a 0b63 6f6c  .input_dictZ.col
 000009c0: 756d 6e6e 616d 6573 da01 6a5a 0864 665f  umnnames..jZ.df_
 000009d0: 696e 7075 74da 096f 626a 6563 7469 7665  input..objective
 000009e0: da06 7365 7269 6573 da06 7265 7375 6c74  ..series..result
 000009f0: 5a0b 636f 6c64 5f72 6573 756c 745a 0b77  Z.cold_resultZ.w
 00000a00: 6172 6d5f 7265 7375 6c74 5a09 636f 6c64  arm_resultZ.cold
 00000a10: 5f64 6963 745a 0977 6172 6d5f 6469 6374  _dictZ.warm_dict
 00000a20: 5a0a 636f 6c64 5f69 6e70 7574 5a0a 7761  Z.cold_inputZ.wa
 00000a30: 726d 5f69 6e70 7574 5a08 7465 6d70 5f64  rm_inputZ.temp_d
 00000a40: 6631 5a08 7465 6d70 5f64 6632 7209 0000  f1Z.temp_df2r...
 00000a50: 0072 0900 0000 720a 0000 00da 0865 705f  .r....r......ep_
 00000a60: 746f 5f65 684c 0000 0073 2c00 0000 0006  to_ehL...s,.....
 00000a70: 0804 0401 0801 0c09 0c02 0801 0c01 1002  ................
 00000a80: 0c04 0801 0801 0801 0801 0801 0802 0601  ................
-00000a90: 0602 1601 1608 1201 1602 723b 0000 0029  ..........r;...)
-00000aa0: 1bda 075f 5f64 6f63 5f5f 7211 0000 00da  ...__doc__r.....
+00000a90: 0602 1601 1608 1201 1602 7239 0000 0029  ..........r9...)
+00000aa0: 1bda 075f 5f64 6f63 5f5f 7210 0000 00da  ...__doc__r.....
 00000ab0: 0966 756e 6374 6f6f 6c73 7202 0000 00da  .functoolsr.....
 00000ac0: 0674 7970 696e 6772 0300 0000 da05 6e75  .typingr......nu
-00000ad0: 6d70 7972 3200 0000 da06 7061 6e64 6173  mpyr2.....pandas
-00000ae0: 722f 0000 0072 0d00 0000 7204 0000 005a  r/...r....r....Z
+00000ad0: 6d70 7972 2f00 0000 da06 7061 6e64 6173  mpyr/.....pandas
+00000ae0: 722c 0000 0072 0d00 0000 7204 0000 005a  r,...r....r....Z
 00000af0: 1c70 7965 6875 622e 656e 6572 6779 5f68  .pyehub.energy_h
 00000b00: 7562 2e65 6875 625f 6d6f 6465 6c72 0500  ub.ehub_modelr..
 00000b10: 0000 da05 6265 736f 7372 0600 0000 da05  ....besosr......
 00000b20: 6669 6c65 73da 0367 6574 da03 7374 7272  files..get..strr
-00000b30: 0b00 0000 7210 0000 0072 1500 0000 7218  ....r....r....r.
-00000b40: 0000 00da 046c 6973 7472 2200 0000 7229  .....listr"...r)
-00000b50: 0000 0072 3b00 0000 7209 0000 0072 0900  ...r;...r....r..
+00000b30: 0b00 0000 720f 0000 0072 1400 0000 7217  ....r....r....r.
+00000b40: 0000 00da 046c 6973 7472 2000 0000 7226  .....listr ...r&
+00000b50: 0000 0072 3900 0000 7209 0000 0072 0900  ...r9...r....r..
 00000b60: 0000 7209 0000 0072 0a00 0000 da08 3c6d  ..r....r......<m
 00000b70: 6f64 756c 653e 0100 0000 732c 0000 0004  odule>....s,....
 00000b80: 0508 010c 010c 0308 0108 0108 010c 010c  ................
 00000b90: 030c 061a 0408 0808 0608 0602 0102 0102  ................
 00000ba0: fe04 0606 0002 ff0e 0908 0e              ...........
```

### Comparing `besos-2.2.0/besos/__pycache__/sampling.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/sampling.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/__pycache__/weather.cpython-38.pyc` & `besos-2.2.2/besos/__pycache__/weather.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/besos_utils.py` & `besos-2.2.2/besos/.ipynb_checkpoints/besos_utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/config.py` & `besos-2.2.2/besos/config.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/Custom_Long_Fields.idd` & `besos-2.2.2/besos/data/Custom_Long_Fields.idd`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/Energy+.schema.epJSON` & `besos-2.2.2/besos/data/Energy+.schema.epJSON`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/example_bad_idf.idf` & `besos-2.2.2/besos/data/example_bad_idf.idf`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/example_building.epJSON` & `besos-2.2.2/besos/data/example_building.epJSON`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/example_epw.epw` & `besos-2.2.2/besos/data/example_epw.epw`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/example_idd.idd` & `besos-2.2.2/besos/data/example_idd.idd`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/example_idf.idf` & `besos-2.2.2/besos/data/example_idf.idf`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/example_xlsx.xlsx` & `besos-2.2.2/besos/data/example_xlsx.xlsx`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/data/unexpanded.idf` & `besos-2.2.2/besos/data/unexpanded.idf`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/eplus_funcs.py` & `besos-2.2.2/besos/eplus_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/eppy_funcs.py` & `besos-2.2.2/besos/eppy_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/errors.py` & `besos-2.2.2/besos/errors.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/evaluator.py` & `besos-2.2.2/besos/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -533,15 +533,14 @@
         :param data: a table of training data to store
         :param deduplicate: whether to remove duplicates from the combined DataFrame
         :return:
         """
         self.cache_clear()  # TODO: decide on a consistent way of tracking this
         # can we assume users will only modify the data using this method or will call cache_clear themselves
         new_data = self.problem.to_df(data, ["inputs", "outputs", "constraints"])
-        # self.data = self.data.append(new_data, ignore_index=True)
         self.data = pd.concat([self.data, new_data], ignore_index=True)
         if deduplicate:
             self.data.drop_duplicates(inplace=True)
 
     def get_infill(self, num_datapoints: int) -> tabular:
         """Generates data that is most likely to improve the model, and can be used for retraining.
```

### Comparing `besos-2.2.0/besos/example_ui.py` & `besos-2.2.2/besos/example_ui.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/objectives.py` & `besos-2.2.2/besos/objectives.py`

 * *Files 1% similar despite different names*

```diff
@@ -491,17 +491,20 @@
         self.key_value = key_value
         self._add_repr("key_value")
         self.variable_name = variable_name
         if self.variable_name != "*":
             self._add_repr("variable_name")
 
     def results_name(self):
-        # E+ forces key_values to upper case in the eso file
+        # E+ forces key_values (except for "Environment") to upper case in the eso file
         # To ensure matching, the input key_value is forced to uppercase.
-        return f"{self.key_value.upper()},{self.variable_name}"
+        if self.key_value.capitalize() == "Environment":
+            return f"{self.key_value.capitalize()},{self.variable_name}"
+        else:
+            return f"{self.key_value.upper()},{self.variable_name}"
 
     @property
     def _default_name(self):
         return self.variable_name
 
     # FIXME: The return types for this function are inconsistent
     def __call__(self, results: _results_format) -> list:
```

### Comparing `besos-2.2.0/besos/optimizer.py` & `besos-2.2.2/besos/optimizer.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/parameters.py` & `besos-2.2.2/besos/parameters.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/problem.py` & `besos-2.2.2/besos/problem.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos/pyehub_funcs.py` & `besos-2.2.2/besos/pyehub_funcs.py`

 * *Files 11% similar despite different names*

```diff
@@ -117,13 +117,11 @@
             temp_df1 = pd.DataFrame(np.array(cold_input), columns=[j])
             temp_df2 = pd.DataFrame(np.array(warm_input), columns=[j])
             # instead of appending I can edit the value of the specific cell with the input
             # (ah that gets difficult with dictionaries)
             # df_input.at[i, j] = [cold_dict]
             # df_input.iloc[i+len(EPdf), df_input.columns.get_loc(j)] = warm_dict
             # could do some sort of join on the
-            # df_input = df_input.append(temp_df1, ignore_index=True)
-            # df_input = df_input.append(temp_df2, ignore_index=True)
             df_input = pd.concat([df_input, temp_df1], ignore_index=True)
             df_input = pd.concat([df_input, temp_df2], ignore_index=True)
 
     return df_input
```

### Comparing `besos-2.2.0/besos/sampling.py` & `besos-2.2.2/besos/sampling.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/besos.egg-info/PKG-INFO` & `besos-2.2.2/besos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: besos
-Version: 2.2.0
+Version: 2.2.2
 Summary: A library for Building and Energy Simulation, Optimization and Surrogate-modelling
 Home-page: https://gitlab.com/energyincities/besos
 Author: Ralph Evins
 Author-email: revins@uvic.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
```

### Comparing `besos-2.2.0/besos.egg-info/SOURCES.txt` & `besos-2.2.2/besos.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 besos/pyehub_funcs.py
 besos/sampling.py
 besos.egg-info/PKG-INFO
 besos.egg-info/SOURCES.txt
 besos.egg-info/dependency_links.txt
 besos.egg-info/requires.txt
 besos.egg-info/top_level.txt
+besos/.ipynb_checkpoints/besos_utils-checkpoint.py
 besos/.ipynb_checkpoints/config-checkpoint.py
 besos/.ipynb_checkpoints/eplus_funcs-checkpoint.py
 besos/.ipynb_checkpoints/eppy_funcs-checkpoint.py
 besos/.ipynb_checkpoints/evaluator-checkpoint.py
 besos/.ipynb_checkpoints/parameters-checkpoint.py
 besos/.ipynb_checkpoints/pyehub_funcs-checkpoint.py
 besos/.ipynb_checkpoints/sampling-checkpoint.py
```

### Comparing `besos-2.2.0/setup.py` & `besos-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     dev = f.read().splitlines()
 
 complete = complete[1:]  # Remove reference to requirements file
 dev = dev[1:]  # Remove reference to requirement-complete file
 
 setup(
     name="besos",
-    version="2.2.0",
+    version="2.2.2",
     description="A library for Building and Energy Simulation, Optimization and Surrogate-modelling",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Ralph Evins",
     author_email="revins@uvic.ca",
     url="https://gitlab.com/energyincities/besos",
     packages=["besos"],
```

### Comparing `besos-2.2.0/test/test_adaptive_surrogate.py` & `besos-2.2.2/test/test_adaptive_surrogate.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_eplus_funcs.py` & `besos-2.2.2/test/test_eplus_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_eppy_funcs.py` & `besos-2.2.2/test/test_eppy_funcs.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_error_handling.py` & `besos-2.2.2/test/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_evaluators.py` & `besos-2.2.2/test/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_fit_surrogate.py` & `besos-2.2.2/test/test_fit_surrogate.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_mixed_optimisation.py` & `besos-2.2.2/test/test_mixed_optimisation.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_objectives_constraints.py` & `besos-2.2.2/test/test_objectives_constraints.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_parameter.py` & `besos-2.2.2/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_platypus.py` & `besos-2.2.2/test/test_platypus.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_rbfopt.py` & `besos-2.2.2/test/test_rbfopt.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_selectors.py` & `besos-2.2.2/test/test_selectors.py`

 * *Files identical despite different names*

### Comparing `besos-2.2.0/test/test_simulation.py` & `besos-2.2.2/test/test_simulation.py`

 * *Files identical despite different names*

