# Comparing `tmp/reqless-0.13.0.tar.gz` & `tmp/reqless-0.13.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reqless-0.13.0.tar", last modified: Sat Apr  6 02:30:06 2024, max compression
+gzip compressed data, was "reqless-0.13.1.tar", last modified: Sun Apr  7 00:45:31 2024, max compression
```

## Comparing `reqless-0.13.0.tar` & `reqless-0.13.1.tar`

### file list

```diff
@@ -1,101 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.599914 reqless-0.13.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.583914 reqless-0.13.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.587914 reqless-0.13.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-04-06 02:28:43.000000 reqless-0.13.0/.github/workflows/main-build-and-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-06 02:28:43.000000 reqless-0.13.0/.github/workflows/other-check-quality-and-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-06 02:28:43.000000 reqless-0.13.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-06 02:28:43.000000 reqless-0.13.0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-04-06 02:28:43.000000 reqless-0.13.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-06 02:28:43.000000 reqless-0.13.0/.safety-policy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-06 02:28:43.000000 reqless-0.13.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-06 02:28:43.000000 reqless-0.13.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-04-06 02:30:06.599914 reqless-0.13.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19937 2024-04-06 02:28:43.000000 reqless-0.13.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 02:28:43.000000 reqless-0.13.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-06 02:28:43.000000 reqless-0.13.0/Vagrantfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.587914 reqless-0.13.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-06 02:28:43.000000 reqless-0.13.0/bin/reqless-py-worker
--rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-04-06 02:28:43.000000 reqless-0.13.0/forgetful-bench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-06 02:28:43.000000 reqless-0.13.0/provision.sh
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-06 02:28:43.000000 reqless-0.13.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.587914 reqless-0.13.0/qmore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:28:43.000000 reqless-0.13.0/qmore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-06 02:28:43.000000 reqless-0.13.0/qmore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:28:43.000000 reqless-0.13.0/qmore/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.587914 reqless-0.13.0/reqless/
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-06 02:30:06.000000 reqless-0.13.0/reqless/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.591914 reqless-0.13.0/reqless/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_job_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_job_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_queue_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_throttles.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/abstract/abstract_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.591914 reqless-0.13.0/reqless/lua/
--rw-r--r--   0 runner    (1001) docker     (127)    97685 2024-04-06 02:29:55.000000 reqless-0.13.0/reqless/lua/qless-lib.lua
--rw-r--r--   0 runner    (1001) docker     (127)    71833 2024-04-06 02:29:55.000000 reqless-0.13.0/reqless/lua/qless.lua
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/proctitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.591914 reqless-0.13.0/reqless/queue_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/queue_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/queue_resolvers/transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.595914 reqless-0.13.0/reqless/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/workers/forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/workers/greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/workers/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/workers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless/workers/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.599914 reqless-0.13.0/reqless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21720 2024-04-06 02:30:06.000000 reqless-0.13.0/reqless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-06 02:30:06.000000 reqless-0.13.0/reqless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:30:06.000000 reqless-0.13.0/reqless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-06 02:30:06.000000 reqless-0.13.0/reqless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-06 02:30:06.000000 reqless-0.13.0/reqless.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:30:06.599914 reqless-0.13.0/reqless_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_job_processor_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_qmore_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-06 02:28:43.000000 reqless-0.13.0/reqless_test/test_worker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-06 02:29:36.000000 reqless-0.13.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:30:06.599914 reqless-0.13.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-06 02:28:43.000000 reqless-0.13.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-06 02:28:43.000000 reqless-0.13.0/whitelist.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.099907 reqless-0.13.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.079908 reqless-0.13.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.083907 reqless-0.13.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-04-07 00:44:24.000000 reqless-0.13.1/.github/workflows/main-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-07 00:44:24.000000 reqless-0.13.1/.github/workflows/other-branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-07 00:44:24.000000 reqless-0.13.1/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 00:44:24.000000 reqless-0.13.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-07 00:44:24.000000 reqless-0.13.1/.gitmodules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.079908 reqless-0.13.1/.meta/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.083907 reqless-0.13.1/.meta/coverage/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-07 00:45:27.000000 reqless-0.13.1/.meta/coverage/badge.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6222 2024-04-07 00:45:27.000000 reqless-0.13.1/.meta/coverage/report.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-07 00:44:24.000000 reqless-0.13.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-07 00:44:24.000000 reqless-0.13.1/.safety-policy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-07 00:44:24.000000 reqless-0.13.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-07 00:44:24.000000 reqless-0.13.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-07 00:45:31.099907 reqless-0.13.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20235 2024-04-07 00:44:24.000000 reqless-0.13.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-07 00:44:24.000000 reqless-0.13.1/Vagrantfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.083907 reqless-0.13.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3376 2024-04-07 00:44:24.000000 reqless-0.13.1/bin/reqless-py-worker
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5194 2024-04-07 00:44:24.000000 reqless-0.13.1/forgetful-bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-07 00:44:24.000000 reqless-0.13.1/provision.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-07 00:44:24.000000 reqless-0.13.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.087907 reqless-0.13.1/qmore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/qmore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-04-07 00:44:24.000000 reqless-0.13.1/qmore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/qmore/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.087907 reqless-0.13.1/reqless/
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-07 00:45:30.000000 reqless-0.13.1/reqless/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_job_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_throttles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/abstract/abstract_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/lua/
+-rw-r--r--   0 runner    (1001) docker     (127)    97685 2024-04-07 00:45:19.000000 reqless-0.13.1/reqless/lua/qless-lib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    71833 2024-04-07 00:45:19.000000 reqless-0.13.1/reqless/lua/qless.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/proctitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8929 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/queue_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4229 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4594 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/queue_resolvers/transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.091908 reqless-0.13.1/reqless/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/forking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/greenlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless/workers/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.095908 reqless-0.13.1/reqless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22072 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 00:45:31.000000 reqless-0.13.1/reqless.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:45:31.095908 reqless-0.13.1/reqless_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9858 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_forking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_greenlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_job_processor_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5143 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_qmore_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14386 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15099 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3623 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-04-07 00:44:24.000000 reqless-0.13.1/reqless_test/test_worker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-07 00:45:01.000000 reqless-0.13.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:45:31.099907 reqless-0.13.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-07 00:44:24.000000 reqless-0.13.1/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-07 00:44:24.000000 reqless-0.13.1/whitelist.txt
```

### Comparing `reqless-0.13.0/.github/workflows/main-build-and-publish.yaml` & `reqless-0.13.1/.github/workflows/main-branch.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: Test, build, and publish the package
 
 on:
   push:
     branches: [main]
 
 jobs:
-  test-build-and-publish:
+  test-and-build-and-update-metadata:
     name: Test, build, and publish the package
     runs-on: ubuntu-latest
 
     steps:
       - name: Check out code
         uses: actions/checkout@v3
         with:
@@ -32,58 +32,46 @@
           source venv/bin/activate
           pip install .[all]
           pip uninstall -y reqless
           pip freeze > requirements.txt
 
           if ! `git diff --quiet`; then
             echo "pip freeze caused file changes, failing!"
+            git diff
             exit 1
           fi
 
       - name: Check style
         run: |
           source venv/bin/activate
           make style
+
           if ! `git diff --quiet`; then
             echo "make style caused file changes, failing!"
+            git diff
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
           make nose
-          export SETUPTOOLS_SCM_PRETEND_VERSION_FOR_REQLESS="$(cat VERSION)"
+          coverage report | tee .meta/coverage/report.txt
+          coverage-badge -f -o .meta/coverage/badge.svg
           python -m build
 
       - name: Checkout tdg5/github-action-pack
         uses: actions/checkout@v4
         with:
           path: .github/actions/tdg5/github-action-pack
-          ref: v0.0.4
+          ref: v0.0.5
           repository: tdg5/github-action-pack
 
-      - name: Increment version
-        uses: ./.github/actions/tdg5/github-action-pack/packages/increment-version-file-action/src
+      - name: Commit and push code coverage snapshot
+        uses: ./.github/actions/tdg5/github-action-pack/packages/stage-files-and-commit-and-push-action/src
         with:
           authorEmail: dannyguinther+spamburglar@gmail.com
           authorName: Spamburglar
-          commitMessage: "[skip actions] Increment version for next development cycle"
-          versionFilePath: VERSION
-          versionFormat: python
-
-      - name: Publish package to pypi
-        env:
-          TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
-          TWINE_USERNAME: __token__
-        run: |
-          source venv/bin/activate
-          python -m twine upload dist/*
-
-      # Add the tag after publishing the package so it is more likely that we
-      # end up with a package without a tag than a tag without a package.
-      - name: Create and push tag for published version
-        run: |
-          VERSION="$(git show HEAD~1:VERSION)"
-          TAG_NAME="v${VERSION}"
-          git tag "$TAG_NAME" HEAD~1
-          git push origin "$TAG_NAME"
+          commitMessage: "[skip actions] Update code coverage snapshot"
+          optionalFilePaths: |
+            .meta/coverage/badge.svg
+            .meta/coverage/report.txt
```

### Comparing `reqless-0.13.0/.github/workflows/other-check-quality-and-tests.yaml` & `reqless-0.13.1/.github/workflows/other-branch.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-name: Style, test, build, and publish the package
+name: Style, test, and build package
 
 on:
   push:
     branches-ignore: [main]
 
 jobs:
   style-test-and-build:
-    name: Test, build, and publish the package
+    name: Style, test, and build package
     runs-on: ubuntu-latest
 
     steps:
       - name: Check out code
         uses: actions/checkout@v3
         with:
           submodules: true
@@ -46,9 +46,9 @@
             exit 1
           fi
 
       - name: Run tests and build package
         run: |
           source venv/bin/activate
           make nose
-          export SETUPTOOLS_SCM_PRETEND_VERSION_FOR_REQLESS="$(cat VERSION)"
+          coverage report
           python -m build
```

### Comparing `reqless-0.13.0/.pre-commit-config.yaml` & `reqless-0.13.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.3.0
     hooks:
       - id: trailing-whitespace
         args: [--markdown-linebreak-ext=md]
         exclude: reqless/lua|reqless/qless-core
       - id: end-of-file-fixer
-        exclude: README.md|VERSION|reqless/lua|reqless/qless-core
+        exclude: README.md|reqless/lua|reqless/qless-core
       - id: check-docstring-first
       - id: debug-statements
       - id: name-tests-test
         args: ["--pytest-test-first"]
         exclude: factories.py
       - id: requirements-txt-fixer
       - id: check-yaml
```

### Comparing `reqless-0.13.0/LICENSE` & `reqless-0.13.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/Makefile` & `reqless-0.13.1/Makefile`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/PKG-INFO` & `reqless-0.13.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.0
+Version: 0.13.1
 Summary: Redis-based Queue Management
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
 Keywords: job,qless,redis,reqless
@@ -34,21 +34,25 @@
 Requires-Dist: removestar~=1.3.1; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
 Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: types-decorator~=5.1.8.4; extra == "dev"
 Requires-Dist: types-mock~=5.1.0.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
+Requires-Dist: coverage-badge~=1.1.0; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: nose; extra == "test"
 Requires-Dist: rednose; extra == "test"
 Requires-Dist: setuptools>=69; extra == "test"
 Provides-Extra: all
 Requires-Dist: reqless[dev,test]; extra == "all"
 
+[![code coverage](https://github.com/tdg5/reqless-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/reqless-py/main/.meta/coverage/report.txt)
+[![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
+
 # reqless
 
 This is a fork of [seomoz/qless-py](https://github.com/seomoz/qless-py) that
 includes significant type improvements and support for throttles.
 
 `qless` is a powerful `Redis`-based job queueing system inspired by
 [resque](https://github.com/defunkt/resque#readme), but built on a collection
```

### Comparing `reqless-0.13.0/README.md` & `reqless-0.13.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+[![code coverage](https://github.com/tdg5/reqless-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/reqless-py/main/.meta/coverage/report.txt)
+[![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
+
 # reqless
 
 This is a fork of [seomoz/qless-py](https://github.com/seomoz/qless-py) that
 includes significant type improvements and support for throttles.
 
 `qless` is a powerful `Redis`-based job queueing system inspired by
 [resque](https://github.com/defunkt/resque#readme), but built on a collection
```

### Comparing `reqless-0.13.0/bin/reqless-py-worker` & `reqless-0.13.1/bin/reqless-py-worker`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/forgetful-bench.py` & `reqless-0.13.1/forgetful-bench.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/provision.sh` & `reqless-0.13.1/provision.sh`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/pyproject.toml` & `reqless-0.13.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
   "safety==2.3.4",
   "twine~=4.0.2",
   "types-decorator~=5.1.8.4",
   "types-mock~=5.1.0.2",
 ]
 test = [
     "coverage",
+    "coverage-badge~=1.1.0",
     "mock",
     "nose",
     "rednose",
     "setuptools>=69",
 ]
 all = ["reqless[dev,test]"]
```

### Comparing `reqless-0.13.0/qmore/client.py` & `reqless-0.13.1/qmore/client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/__init__.py` & `reqless-0.13.1/reqless/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/__init__.py` & `reqless-0.13.1/reqless/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_client.py` & `reqless-0.13.1/reqless/abstract/abstract_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_config.py` & `reqless-0.13.1/reqless/abstract/abstract_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_job.py` & `reqless-0.13.1/reqless/abstract/abstract_job.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_job_processor.py` & `reqless-0.13.1/reqless/abstract/abstract_job_processor.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_jobs.py` & `reqless-0.13.1/reqless/abstract/abstract_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_queue.py` & `reqless-0.13.1/reqless/abstract/abstract_queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_queue_jobs.py` & `reqless-0.13.1/reqless/abstract/abstract_queue_jobs.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/abstract/abstract_throttle.py` & `reqless-0.13.1/reqless/abstract/abstract_throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/config.py` & `reqless-0.13.1/reqless/config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/importer.py` & `reqless-0.13.1/reqless/importer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/job.py` & `reqless-0.13.1/reqless/job.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/listener.py` & `reqless-0.13.1/reqless/listener.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/lua/qless-lib.lua` & `reqless-0.13.1/reqless/lua/qless-lib.lua`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/lua/qless.lua` & `reqless-0.13.1/reqless/lua/qless.lua`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/profile.py` & `reqless-0.13.1/reqless/profile.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/queue.py` & `reqless-0.13.1/reqless/queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/queue_resolvers/__init__.py` & `reqless-0.13.1/reqless/queue_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-0.13.1/reqless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/queue_resolvers/transforming_queue_resolver.py` & `reqless-0.13.1/reqless/queue_resolvers/transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/throttle.py` & `reqless-0.13.1/reqless/throttle.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/workers/forking.py` & `reqless-0.13.1/reqless/workers/forking.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/workers/greenlet.py` & `reqless-0.13.1/reqless/workers/greenlet.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/workers/serial.py` & `reqless-0.13.1/reqless/workers/serial.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/workers/util.py` & `reqless-0.13.1/reqless/workers/util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless/workers/worker.py` & `reqless-0.13.1/reqless/workers/worker.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless.egg-info/PKG-INFO` & `reqless-0.13.1/reqless.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reqless
-Version: 0.13.0
+Version: 0.13.1
 Summary: Redis-based Queue Management
 Author: Danny Guinther
 License: MIT
 Project-URL: Homepage, https://github.com/tdg5/reqless-py
 Project-URL: Source, https://github.com/tdg5/reqless-py
 Project-URL: Tracker, https://github.com/tdg5/reqless-py/issues
 Keywords: job,qless,redis,reqless
@@ -34,21 +34,25 @@
 Requires-Dist: removestar~=1.3.1; extra == "dev"
 Requires-Dist: safety==2.3.4; extra == "dev"
 Requires-Dist: twine~=4.0.2; extra == "dev"
 Requires-Dist: types-decorator~=5.1.8.4; extra == "dev"
 Requires-Dist: types-mock~=5.1.0.2; extra == "dev"
 Provides-Extra: test
 Requires-Dist: coverage; extra == "test"
+Requires-Dist: coverage-badge~=1.1.0; extra == "test"
 Requires-Dist: mock; extra == "test"
 Requires-Dist: nose; extra == "test"
 Requires-Dist: rednose; extra == "test"
 Requires-Dist: setuptools>=69; extra == "test"
 Provides-Extra: all
 Requires-Dist: reqless[dev,test]; extra == "all"
 
+[![code coverage](https://github.com/tdg5/reqless-py/raw/main/.meta/coverage/badge.svg)](https://raw.githubusercontent.com/tdg5/reqless-py/main/.meta/coverage/report.txt)
+[![license](https://img.shields.io/github/license/tdg5/reqless-py.svg)](https://github.com/tdg5/reqless-py/blob/main/LICENSE)
+
 # reqless
 
 This is a fork of [seomoz/qless-py](https://github.com/seomoz/qless-py) that
 includes significant type improvements and support for throttles.
 
 `qless` is a powerful `Redis`-based job queueing system inspired by
 [resque](https://github.com/defunkt/resque#readme), but built on a collection
```

### Comparing `reqless-0.13.0/reqless.egg-info/SOURCES.txt` & `reqless-0.13.1/reqless.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 .gitignore
 .gitmodules
 .pre-commit-config.yaml
 .safety-policy.yaml
 LICENSE
 Makefile
 README.md
-VERSION
 Vagrantfile
 forgetful-bench.py
 provision.sh
 pyproject.toml
 requirements.txt
 tox.ini
 whitelist.txt
-.github/workflows/main-build-and-publish.yaml
-.github/workflows/other-check-quality-and-tests.yaml
+.github/workflows/main-branch.yaml
+.github/workflows/other-branch.yaml
+.github/workflows/release.yaml
+.meta/coverage/badge.svg
+.meta/coverage/report.txt
 bin/reqless-py-worker
 qmore/__init__.py
 qmore/client.py
 qmore/py.typed
 reqless/__init__.py
 reqless/__version__.py
 reqless/config.py
```

### Comparing `reqless-0.13.0/reqless_test/common.py` & `reqless-0.13.1/reqless_test/common.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_client.py` & `reqless-0.13.1/reqless_test/test_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_config.py` & `reqless-0.13.1/reqless_test/test_config.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_events.py` & `reqless-0.13.1/reqless_test/test_events.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_forking.py` & `reqless-0.13.1/reqless_test/test_forking.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_greenlet.py` & `reqless-0.13.1/reqless_test/test_greenlet.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_importer.py` & `reqless-0.13.1/reqless_test/test_importer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_job.py` & `reqless-0.13.1/reqless_test/test_job.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_job_processor_api.py` & `reqless-0.13.1/reqless_test/test_job_processor_api.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_listener.py` & `reqless-0.13.1/reqless_test/test_listener.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_qmore_client.py` & `reqless-0.13.1/reqless_test/test_qmore_client.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py` & `reqless-0.13.1/reqless_test/test_qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py` & `reqless-0.13.1/reqless_test/test_qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_queue.py` & `reqless-0.13.1/reqless_test/test_queue.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_serial.py` & `reqless-0.13.1/reqless_test/test_serial.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_transforming_queue_resolver.py` & `reqless-0.13.1/reqless_test/test_transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_worker.py` & `reqless-0.13.1/reqless_test/test_worker.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/reqless_test/test_worker_util.py` & `reqless-0.13.1/reqless_test/test_worker_util.py`

 * *Files identical despite different names*

### Comparing `reqless-0.13.0/requirements.txt` & `reqless-0.13.1/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 certifi==2023.11.17
 cffi==1.16.0
 cfgv==3.4.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
 coverage==7.3.0
+coverage-badge==1.1.0
 cryptography==42.0.5
 decorator==5.1.1
 distlib==0.3.7
 docutils==0.20.1
 dparse==0.6.3
 filelock==3.13.1
 flake8==7.0.0
```

### Comparing `reqless-0.13.0/whitelist.txt` & `reqless-0.13.1/whitelist.txt`

 * *Files identical despite different names*

