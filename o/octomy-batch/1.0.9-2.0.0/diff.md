# Comparing `tmp/octomy-batch-1.0.9.tar.gz` & `tmp/octomy-batch-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octomy-batch-1.0.9.tar", last modified: Tue Jan 19 03:35:36 2021, max compression
+gzip compressed data, was "octomy-batch-2.0.0.tar", last modified: Sat Apr  6 22:41:09 2024, max compression
```

## Comparing `octomy-batch-1.0.9.tar` & `octomy-batch-2.0.0.tar`

### file list

```diff
@@ -1,61 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/
--rw-rw-rw-   0 root         (0) root         (0)      489 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/.gitlab/
--rw-rw-rw-   0 root         (0) root         (0)      804 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/.gitlab/ci.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4982 2021-01-18 00:11:01.000000 octomy-batch-1.0.9/Makefile
--rw-r--r--   0 root         (0) root         (0)     1630 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      718 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/bin/
--rwxrwxrwx   0 root         (0) root         (0)     1936 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/bin/octomy-batch
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/code_quality/
--rw-rw-rw-   0 root         (0) root         (0)      136 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/.flake8
--rw-rw-rw-   0 root         (0) root         (0)     1919 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      117 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    11867 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/code_quality/pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     2574 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/config.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/design/
--rw-rw-rw-   0 root         (0) root         (0)    71853 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/design/logo-1024.png
--rw-rw-rw-   0 root         (0) root         (0)     7666 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/design/logo-1024.svg
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.774476 octomy-batch-1.0.9/fk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/fk/batch/
--rw-rw-rw-   0 root         (0) root         (0)    12257 2021-01-19 02:56:17.000000 octomy-batch-1.0.9/fk/batch/BatchProcessor.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/Server.py
--rw-rw-rw-   0 root         (0) root         (0)     5374 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/WebsiteIO.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13149 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk/batch/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.774476 octomy-batch-1.0.9/fk_batch_filters/
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.778476 octomy-batch-1.0.9/fk_batch_filters/default/
--rw-rw-rw-   0 root         (0) root         (0)        2 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk_batch_filters/default/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1181 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/fk_batch_filters/default/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/octomy_batch.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1630 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1077 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       35 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-01-19 03:35:36.000000 octomy-batch-1.0.9/octomy_batch.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/requirements/
--rw-rw-rw-   0 root         (0) root         (0)       35 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/requirements/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      776 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/requirements/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      215 2021-01-18 00:11:01.000000 octomy-batch-1.0.9/requirements/test_requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     2907 2021-01-19 03:35:31.000000 octomy-batch-1.0.9/requirements/test_requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      166 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     5190 2021-01-19 02:56:17.000000 octomy-batch-1.0.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1097 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/Makefile
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/integration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/integration/test_integration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/load/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/load/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/load/test_load.py
--rw-rw-rw-   0 root         (0) root         (0)      335 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.782476 octomy-batch-1.0.9/tests/regressions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/regressions/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      130 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/regressions/test_regressions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-01-19 03:35:36.786476 octomy-batch-1.0.9/tests/unit/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/unit/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      123 2021-01-16 18:23:47.000000 octomy-batch-1.0.9/tests/unit/test_unit.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.447478 octomy-batch-2.0.0/
+-rw-r--r--   0 leo       (1000) leo       (1000)      496 2021-12-17 22:49:10.000000 octomy-batch-2.0.0/.gitignore
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.439478 octomy-batch-2.0.0/.gitlab/
+-rw-r--r--   0 leo       (1000) leo       (1000)      804 2021-11-09 04:03:42.000000 octomy-batch-2.0.0/.gitlab/ci.yaml
+-rw-r--r--   0 leo       (1000) leo       (1000)     2021 2024-04-01 18:16:40.000000 octomy-batch-2.0.0/LICENSE
+-rw-r--r--   0 leo       (1000) leo       (1000)      284 2024-04-01 17:02:28.000000 octomy-batch-2.0.0/Makefile
+-rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-06 22:41:09.447478 octomy-batch-2.0.0/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     2292 2024-04-01 18:15:51.000000 octomy-batch-2.0.0/README.md
+-rw-r--r--   0 leo       (1000) leo       (1000)        6 2024-04-06 13:28:59.000000 octomy-batch-2.0.0/VERSION
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.439478 octomy-batch-2.0.0/bin/
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     3257 2024-04-06 21:53:07.000000 octomy-batch-2.0.0/bin/octomy-batch
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.439478 octomy-batch-2.0.0/code_quality/
+-rw-rw-r--   0 leo       (1000) leo       (1000)      136 2020-03-25 22:47:14.000000 octomy-batch-2.0.0/code_quality/.flake8
+-rw-r--r--   0 leo       (1000) leo       (1000)     1919 2021-11-09 04:03:42.000000 octomy-batch-2.0.0/code_quality/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)      117 2020-03-25 22:44:52.000000 octomy-batch-2.0.0/code_quality/mypy.ini
+-rw-rw-r--   0 leo       (1000) leo       (1000)    11867 2020-03-25 22:43:04.000000 octomy-batch-2.0.0/code_quality/pylintrc
+-rw-r--r--   0 leo       (1000) leo       (1000)     2789 2021-11-09 04:03:47.000000 octomy-batch-2.0.0/config.json
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.427478 octomy-batch-2.0.0/octomy/
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.435478 octomy-batch-2.0.0/octomy/batch/
+-rw-r--r--   0 leo       (1000) leo       (1000)    20940 2024-04-06 22:38:05.000000 octomy-batch-2.0.0/octomy/batch/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     7061 2024-04-01 16:52:41.000000 octomy-batch-2.0.0/octomy/batch/db.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.435478 octomy-batch-2.0.0/octomy/batch/filters/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2024-04-06 13:13:35.000000 octomy-batch-2.0.0/octomy/batch/filters/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.435478 octomy-batch-2.0.0/octomy/batch/filters/base/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.0/octomy/batch/filters/base/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      302 2024-04-01 17:33:21.000000 octomy-batch-2.0.0/octomy/batch/filters/base/hello.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.435478 octomy-batch-2.0.0/octomy/batch/filters/utils/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2021-11-09 04:03:42.000000 octomy-batch-2.0.0/octomy/batch/filters/utils/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      697 2024-04-01 20:23:49.000000 octomy-batch-2.0.0/octomy/batch/filters/utils/ping.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     1094 2024-04-01 20:24:16.000000 octomy-batch-2.0.0/octomy/batch/filters/utils/test.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.435478 octomy-batch-2.0.0/octomy/batch/server/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     4381 2024-03-22 18:00:16.000000 octomy-batch-2.0.0/octomy/batch/server/WebsiteIO.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2254 2024-04-06 21:57:46.000000 octomy-batch-2.0.0/octomy/batch/server/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     2567 2024-04-06 22:23:55.000000 octomy-batch-2.0.0/octomy/batch/types.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.439478 octomy-batch-2.0.0/octomy_batch.egg-info/
+-rw-r--r--   0 leo       (1000) leo       (1000)     3130 2024-04-06 22:41:09.000000 octomy-batch-2.0.0/octomy_batch.egg-info/PKG-INFO
+-rw-r--r--   0 leo       (1000) leo       (1000)     1322 2024-04-06 22:41:09.000000 octomy-batch-2.0.0/octomy_batch.egg-info/SOURCES.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2024-04-06 22:41:09.000000 octomy-batch-2.0.0/octomy_batch.egg-info/dependency_links.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 22:41:09.000000 octomy-batch-2.0.0/octomy_batch.egg-info/namespace_packages.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-06 22:41:09.000000 octomy-batch-2.0.0/octomy_batch.egg-info/requires.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        7 2024-04-06 22:41:09.000000 octomy-batch-2.0.0/octomy_batch.egg-info/top_level.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)        1 2020-11-28 23:26:57.000000 octomy-batch-2.0.0/octomy_batch.egg-info/zip-safe
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.443478 octomy-batch-2.0.0/requirements/
+-rw-r--r--   0 leo       (1000) leo       (1000)       21 2024-04-06 17:42:17.000000 octomy-batch-2.0.0/requirements/requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     1743 2024-04-06 21:16:53.000000 octomy-batch-2.0.0/requirements/requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      215 2021-11-09 04:03:42.000000 octomy-batch-2.0.0/requirements/test_requirements.in
+-rw-r--r--   0 leo       (1000) leo       (1000)     2903 2023-08-28 22:19:16.000000 octomy-batch-2.0.0/requirements/test_requirements.txt
+-rw-r--r--   0 leo       (1000) leo       (1000)      166 2024-04-06 22:41:09.447478 octomy-batch-2.0.0/setup.cfg
+-rwxr-xr-x   0 leo       (1000) leo       (1000)     7024 2024-04-06 13:28:48.000000 octomy-batch-2.0.0/setup.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.443478 octomy-batch-2.0.0/tests/
+-rw-rw-r--   0 leo       (1000) leo       (1000)     1097 2020-03-19 22:34:38.000000 octomy-batch-2.0.0/tests/Makefile
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-19 20:39:36.000000 octomy-batch-2.0.0/tests/__init__.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.443478 octomy-batch-2.0.0/tests/integration/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.0/tests/integration/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      130 2020-03-20 01:43:26.000000 octomy-batch-2.0.0/tests/integration/test_integration.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.443478 octomy-batch-2.0.0/tests/load/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:08.000000 octomy-batch-2.0.0/tests/load/__init__.py
+-rw-rw-r--   0 leo       (1000) leo       (1000)      123 2020-03-20 01:43:18.000000 octomy-batch-2.0.0/tests/load/test_load.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      339 2022-01-12 22:37:26.000000 octomy-batch-2.0.0/tests/pytest.ini
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.443478 octomy-batch-2.0.0/tests/regressions/
+-rw-r--r--   0 leo       (1000) leo       (1000)        0 2020-12-15 04:59:10.000000 octomy-batch-2.0.0/tests/regressions/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      130 2020-12-15 04:57:55.000000 octomy-batch-2.0.0/tests/regressions/test_regressions.py
+drwxr-xr-x   0 leo       (1000) leo       (1000)        0 2024-04-06 22:41:09.447478 octomy-batch-2.0.0/tests/unit/
+-rw-rw-r--   0 leo       (1000) leo       (1000)        0 2020-03-02 23:49:28.000000 octomy-batch-2.0.0/tests/unit/__init__.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      202 2022-01-12 22:37:26.000000 octomy-batch-2.0.0/tests/unit/test_batch_processor.py
+-rw-r--r--   0 leo       (1000) leo       (1000)      190 2022-01-12 22:37:26.000000 octomy-batch-2.0.0/tests/unit/test_server.py
+-rw-r--r--   0 leo       (1000) leo       (1000)     3502 2022-01-12 22:37:26.000000 octomy-batch-2.0.0/tests/unit/test_unit.py
```

### Comparing `octomy-batch-1.0.9/.gitlab/ci.yaml` & `octomy-batch-2.0.0/.gitlab/ci.yaml`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.9/code_quality/Makefile` & `octomy-batch-2.0.0/code_quality/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 h: help
 
 all: black flake
 # mypy detects some false positives, disabled for now
 #pylint is broken, disabled for now
 
 black:
-	black -l 999 -t py37 "${APP_DIR}"
-	black -l 999 -t py37 "${TESTS_DIR}"
+	black -l 999 -t py38 "${APP_DIR}"
+	black -l 999 -t py38 "${TESTS_DIR}"
 
 flake:
 	flake8 --exit-zero --config .flake8 "${APP_DIR}"
 	flake8 --exit-zero --config .flake8 "${TESTS_DIR}"
 
 pylint:
 	pylint --exit-zero --rcfile pylintrc --output-format=colorized "${APP_DIR}"
```

### Comparing `octomy-batch-1.0.9/code_quality/pylintrc` & `octomy-batch-2.0.0/code_quality/pylintrc`

 * *Files identical despite different names*

### Comparing `octomy-batch-1.0.9/config.json` & `octomy-batch-2.0.0/config.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'project'": "'Merchbot'",*

 * * "'shopify-api-throttle-limit'": '1',*

 * * "'shopify-api-throttle-period'": '3000',*

 * * "'shopify-api-version'": "'2021-07'",*

 * * "'shopify-app-company-name'": "'The company name behind this app'",*

 * * "'shopify-app-company-website'": "'The official website url for company behind this app'",*

 * * "'shopify-app-domain'": "'PLEASE OVERRIDE THIS DEFAULT'",*

 * * "'smtp-headers'": "'PLEASE OVERRIDE THIS DEFAULT'",*

 * * "'smtp-hostname'": "'PLEASE OVERRIDE THIS DEFAULT'",*

 * * "'smtp-password'": "'PLEASE OVERRIDE  […]*

```diff
@@ -11,50 +11,54 @@
     "crawler-socket-timeout": 15,
     "crawler-user-agent": "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)",
     "db-database": "postgres",
     "db-hostname": "localhost",
     "db-password": "PLEASE OVERRIDE THIS DEFAULT",
     "db-port": "5432",
     "db-username": "PLEASE OVERRIDE THIS DEFAULT",
-    "email-domain": "fk.z5.no",
-    "email-password": "PLEASE OVERRIDE THIS DEFAULT",
-    "email-user": "PLEASE OVERRIDE THIS DEFAULT",
     "influx-dbname": "sales",
     "influx-hostname": "localhost",
     "influx-password": "PLEASE OVERRIDE THIS DEFAULT",
     "influx-port": "8086",
     "influx-username": "PLEASE OVERRIDE THIS DEFAULT",
     "n2report-dir-name": "_n2report",
     "n2report-index-name": "index.html",
     "overwatch-password": "PLEASE OVERRIDE THIS DEFAULT",
     "overwatch-user": "PLEASE OVERRIDE THIS DEFAULT",
     "preferred-url-scheme": "http",
     "printful-api-endpoint": "https://api.printful.com/",
     "printful-api-key": "PLEASE OVERRIDE THIS DEFAULT",
     "printful-api-key-base64": "PLEASE OVERRIDE THIS DEFAULT",
-    "project": "Bonkers Sales Pop",
+    "project": "Merchbot",
     "project-root": "/app",
     "screenshots-dir-name": "_screenshots",
     "screenshots-index-name": "screenshots.html",
     "shop-id-generator-batch-size": 200,
     "shop-id-generator-max": 25000000000,
     "shop-id-generator-min": 0,
     "shop-id-thread-count": 300,
     "shopify-api-key": "PLEASE OVERRIDE THIS DEFAULT",
     "shopify-api-secret": "PLEASE OVERRIDE THIS DEFAULT",
-    "shopify-api-version": "2019-04",
-    "shopify-app-api-key": "PLEASE OVERRIDE THIS DEFAULT",
-    "shopify-app-api-secret": "PLEASE OVERRIDE THIS DEFAULT",
-    "shopify-app-api-version": "2020-10",
+    "shopify-api-throttle-limit": 1,
+    "shopify-api-throttle-period": 3000,
+    "shopify-api-version": "2021-07",
     "shopify-app-author": "The author of this app",
     "shopify-app-author-email": "The email of the author of this app",
+    "shopify-app-company-name": "The company name behind this app",
+    "shopify-app-company-website": "The official website url for company behind this app",
     "shopify-app-description": "The description of this app",
+    "shopify-app-domain": "PLEASE OVERRIDE THIS DEFAULT",
     "shopify-app-name": "The name of this app",
     "shopify-app-preferred-url-scheme": "https",
     "shopify-password": "PLEASE OVERRIDE THIS DEFAULT",
     "shopify-shared-secret": "PLEASE OVERRIDE THIS DEFAULT",
     "shopify-shop-name": "",
+    "smtp-headers": "PLEASE OVERRIDE THIS DEFAULT",
+    "smtp-hostname": "PLEASE OVERRIDE THIS DEFAULT",
+    "smtp-password": "PLEASE OVERRIDE THIS DEFAULT",
+    "smtp-port": "2525",
+    "smtp-user": "PLEASE OVERRIDE THIS DEFAULT",
     "static-files-root": "/app/shopify_app/static",
     "webdriver-max-windows": 5,
     "webdriver-url": "http://127.0.0.1:4444/wd/hub",
     "webdriver-wait-time-sec": 10
 }
```

### Comparing `octomy-batch-1.0.9/tests/Makefile` & `octomy-batch-2.0.0/tests/Makefile`

 * *Files identical despite different names*

