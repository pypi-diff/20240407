# Comparing `tmp/encommon-0.7.6.tar.gz` & `tmp/encommon-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encommon-0.7.6.tar", last modified: Fri Apr  5 00:46:30 2024, max compression
+gzip compressed data, was "encommon-0.8.0.tar", last modified: Sun Apr  7 10:32:54 2024, max compression
```

## Comparing `encommon-0.7.6.tar` & `encommon-0.8.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.747415 encommon-0.7.6/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.7.6/LICENSE
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.7.6/MANIFEST.in
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-05 00:46:30.747415 encommon-0.7.6/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2177 2024-03-31 14:52:08.000000 encommon-0.7.6/README.md
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.744415 encommon-0.7.6/encommon/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-02 23:01:55.000000 encommon-0.7.6/encommon/__init__.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.745415 encommon-0.7.6/encommon/config/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      710 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/config/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2041 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/config/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4743 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/config/config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2313 2024-04-05 00:11:42.000000 encommon-0.7.6/encommon/config/files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13973 2024-04-05 00:11:42.000000 encommon-0.7.6/encommon/config/logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1816 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/config/params.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-05 00:11:42.000000 encommon-0.7.6/encommon/config/paths.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.745415 encommon-0.7.6/encommon/config/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-02 23:01:55.000000 encommon-0.7.6/encommon/config/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      731 2024-04-02 23:01:55.000000 encommon-0.7.6/encommon/config/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3327 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/config/test/test_config.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2292 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/config/test/test_files.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4740 2024-04-02 23:01:55.000000 encommon-0.7.6/encommon/config/test/test_logger.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2101 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/config/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      880 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/conftest.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.745415 encommon-0.7.6/encommon/crypts/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      318 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/crypts/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3500 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/crypts/crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3103 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/crypts/hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-04 05:02:38.000000 encommon-0.7.6/encommon/crypts/params.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.745415 encommon-0.7.6/encommon/crypts/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/crypts/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2433 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/crypts/test/test_crypts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1206 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/crypts/test/test_hashes.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.7.6/encommon/py.typed
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.745415 encommon-0.7.6/encommon/times/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      597 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2506 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9854 2024-04-05 00:11:42.000000 encommon-0.7.6/encommon/times/duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6411 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/times/parse.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.746415 encommon-0.7.6/encommon/times/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1477 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/test/test_common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3901 2024-04-05 00:11:42.000000 encommon-0.7.6/encommon/times/test/test_duration.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4308 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/test/test_parse.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2314 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/test/test_timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2023 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/test/test_times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4735 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/times/test/test_window.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6287 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/times/timers.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9688 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/times/times.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-04 05:08:51.000000 encommon-0.7.6/encommon/times/window.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.746415 encommon-0.7.6/encommon/types/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/types/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2208 2024-04-04 21:54:07.000000 encommon-0.7.6/encommon/types/dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2675 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/types/empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      560 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/types/strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.746415 encommon-0.7.6/encommon/types/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/types/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2673 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/types/test/test_dicts.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      981 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/types/test/test_empty.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      407 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/types/test/test_strings.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.746415 encommon-0.7.6/encommon/utils/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      833 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      466 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/common.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2462 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3236 2024-04-04 21:54:29.000000 encommon-0.7.6/encommon/utils/paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3230 2024-04-05 00:45:23.000000 encommon-0.7.6/encommon/utils/sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7360 2024-04-04 21:55:08.000000 encommon-0.7.6/encommon/utils/stdout.py
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.747415 encommon-0.7.6/encommon/utils/test/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/test/__init__.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/test/test_match.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1892 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/test/test_paths.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1464 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/test/test_sample.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-02 23:01:56.000000 encommon-0.7.6/encommon/utils/test/test_stdout.py
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-05 00:45:14.000000 encommon-0.7.6/encommon/version.txt
-drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-05 00:46:30.747415 encommon-0.7.6/encommon.egg-info/
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-05 00:46:30.000000 encommon-0.7.6/encommon.egg-info/PKG-INFO
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1891 2024-04-05 00:46:30.000000 encommon-0.7.6/encommon.egg-info/SOURCES.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-05 00:46:30.000000 encommon-0.7.6/encommon.egg-info/dependency_links.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-05 00:46:30.000000 encommon-0.7.6/encommon.egg-info/requires.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-05 00:46:30.000000 encommon-0.7.6/encommon.egg-info/top_level.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.7.6/pyproject.toml
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.7.6/reqs-install.txt
--rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      452 2024-04-05 00:46:30.747415 encommon-0.7.6/setup.cfg
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.685358 encommon-0.8.0/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1071 2024-03-20 05:52:00.000000 encommon-0.8.0/LICENSE
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       32 2023-12-31 23:18:53.000000 encommon-0.8.0/MANIFEST.in
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-07 10:32:54.685358 encommon-0.8.0/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2177 2024-03-31 14:52:08.000000 encommon-0.8.0/README.md
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.683358 encommon-0.8.0/encommon/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/__init__.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.683358 encommon-0.8.0/encommon/config/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      816 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2099 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4790 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2388 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    13488 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1809 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/params.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2535 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/paths.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.683358 encommon-0.8.0/encommon/config/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      313 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1069 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2329 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/test/test_config.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2230 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/test/test_files.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5135 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/test/test_logger.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2568 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/config/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1810 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/conftest.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.683358 encommon-0.8.0/encommon/crypts/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      371 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/crypts/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3540 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/crypts/crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3075 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/crypts/hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      590 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/crypts/params.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.684358 encommon-0.8.0/encommon/crypts/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/crypts/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2655 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/crypts/test/test_crypts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1129 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/crypts/test/test_hashes.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2023-12-31 23:18:53.000000 encommon-0.8.0/encommon/py.typed
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.684358 encommon-0.8.0/encommon/times/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      638 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3635 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)    10033 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6153 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/parse.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.684358 encommon-0.8.0/encommon/times/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2059 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4161 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/test/test_duration.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4055 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/test/test_parse.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3075 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/test/test_timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1691 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/test/test_times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     5411 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/test/test_window.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     6663 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/timers.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     9696 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/times.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7975 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/times/window.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.684358 encommon-0.8.0/encommon/types/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      420 2024-04-07 10:25:51.000000 encommon-0.8.0/encommon/types/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2265 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/types/dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2739 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/types/empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      632 2024-04-07 10:25:51.000000 encommon-0.8.0/encommon/types/strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.684358 encommon-0.8.0/encommon/types/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/types/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2678 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/types/test/test_dicts.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      971 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/types/test/test_empty.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      406 2024-04-07 10:25:51.000000 encommon-0.8.0/encommon/types/test/test_strings.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.685358 encommon-0.8.0/encommon/utils/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      927 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1355 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2463 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3545 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     3230 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     7531 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/stdout.py
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.685358 encommon-0.8.0/encommon/utils/test/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      218 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/test/__init__.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      681 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/test/test_common.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1124 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/test/test_match.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1919 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/test/test_paths.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1710 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/test/test_sample.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     4878 2024-04-07 10:21:05.000000 encommon-0.8.0/encommon/utils/test/test_stdout.py
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        6 2024-04-07 10:31:12.000000 encommon-0.8.0/encommon/version.txt
+drwxr-xr-x   0 enasisnetwork  (9200) enasisnetwork  (9200)        0 2024-04-07 10:32:54.685358 encommon-0.8.0/encommon.egg-info/
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     2671 2024-04-07 10:32:54.000000 encommon-0.8.0/encommon.egg-info/PKG-INFO
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)     1926 2024-04-07 10:32:54.000000 encommon-0.8.0/encommon.egg-info/SOURCES.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        1 2024-04-07 10:32:54.000000 encommon-0.8.0/encommon.egg-info/dependency_links.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-04-07 10:32:54.000000 encommon-0.8.0/encommon.egg-info/requires.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)        9 2024-04-07 10:32:54.000000 encommon-0.8.0/encommon.egg-info/top_level.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      525 2023-12-31 23:18:53.000000 encommon-0.8.0/pyproject.toml
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)       63 2024-01-01 10:25:04.000000 encommon-0.8.0/reqs-install.txt
+-rw-r--r--   0 enasisnetwork  (9200) enasisnetwork  (9200)      558 2024-04-07 10:32:54.686358 encommon-0.8.0/setup.cfg
```

### Comparing `encommon-0.7.6/LICENSE` & `encommon-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `encommon-0.7.6/PKG-INFO` & `encommon-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.7.6
+Version: 0.8.0
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.7.6/README.md` & `encommon-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `encommon-0.7.6/encommon/__init__.py` & `encommon-0.8.0/encommon/__init__.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.6/encommon/config/__init__.py` & `encommon-0.8.0/encommon/config/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,24 +10,28 @@
 from .common import config_load
 from .common import config_path
 from .common import config_paths
 from .config import Config
 from .files import ConfigFile
 from .files import ConfigFiles
 from .logger import Logger
+from .params import ConfigParams
+from .params import LoggerParams
 from .params import Params
 from .paths import ConfigPath
 from .paths import ConfigPaths
 
 
 
 __all__ = [
     'Config',
     'ConfigFile',
     'ConfigFiles',
+    'ConfigParams',
     'ConfigPath',
     'ConfigPaths',
     'Logger',
+    'LoggerParams',
     'Params',
     'config_load',
     'config_path',
     'config_paths']
```

### Comparing `encommon-0.7.6/encommon/config/common.py` & `encommon-0.8.0/encommon/config/common.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,23 +7,28 @@
 
 
 
 from pathlib import Path
 from typing import Any
 from typing import Literal
 from typing import Optional
+from typing import TYPE_CHECKING
 
 from yaml import SafeLoader
 from yaml import load
 
 from .. import PROJECT
 from .. import WORKSPACE
-from ..utils.common import PATHABLE
-from ..utils.paths import resolve_path
-from ..utils.paths import resolve_paths
+from ..utils import read_text
+from ..utils import resolve_path
+from ..utils import resolve_paths
+
+if TYPE_CHECKING:
+    from ..utils.common import PATHABLE
+    from ..utils.common import REPLACE
 
 
 
 LOGLEVELS = Literal[
     'critical',
     'debug',
     'error',
@@ -38,59 +43,58 @@
     """
     Load configuration using the directory or file provided.
 
     :param path: Complete or relative path to configuration.
     :returns: New resolved filesystem path object instance.
     """
 
-    loaded = (
-        config_path(path)
-        .read_text(encoding='utf-8'))
+    loaded = read_text(
+        config_path(path))
 
     parsed = load(loaded, SafeLoader)
 
     assert isinstance(parsed, dict)
 
     return parsed
 
 
 
 def config_path(
     path: str | Path,
 ) -> Path:
     """
-    Resolve the provided path and replace the magic keywords.
+    Resolve the provided path replacing the magic keywords.
 
     .. note::
        This function simply wraps one from utils subpackage.
 
     :param path: Complete or relative path for processing.
     :returns: New resolved filesystem path object instance.
     """
 
     replace = {
-        'PROJECT': str(PROJECT),
-        'WORKSPACE': str(WORKSPACE)}
+        'PROJECT': PROJECT,
+        'WORKSPACE': WORKSPACE}
 
     return resolve_path(path, replace)
 
 
 
 def config_paths(
-    paths: PATHABLE,
-    replace: Optional[dict[str, str]] = None,
+    paths: 'PATHABLE',
+    replace: Optional['REPLACE'] = None,
 ) -> tuple[Path, ...]:
     """
-    Resolve the provided paths and replace the magic keywords.
+    Resolve the provided paths replacing the magic keywords.
 
     .. note::
        This function simply wraps one from utils subpackage.
 
     :param paths: Complete or relative paths for processing.
     :returns: New resolved filesystem path object instances.
     """
 
     replace = {
-        'PROJECT': str(PROJECT),
-        'WORKSPACE': str(WORKSPACE)}
+        'PROJECT': PROJECT,
+        'WORKSPACE': WORKSPACE}
 
     return resolve_paths(paths, replace)
```

### Comparing `encommon-0.7.6/encommon/config/config.py` & `encommon-0.8.0/encommon/config/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,23 +7,26 @@
 
 
 
 from copy import deepcopy
 from typing import Any
 from typing import Callable
 from typing import Optional
+from typing import TYPE_CHECKING
 
 from .common import config_paths
 from .files import ConfigFiles
 from .logger import Logger
 from .params import Params
 from .paths import ConfigPaths
-from ..crypts.crypts import Crypts
-from ..types.dicts import merge_dicts
-from ..utils.common import PATHABLE
+from ..crypts import Crypts
+from ..types import merge_dicts
+
+if TYPE_CHECKING:
+    from ..utils.common import PATHABLE
 
 
 
 class Config:
     """
     Contain the configurations from the arguments and files.
 
@@ -48,16 +51,16 @@
     __logger: Optional[Logger]
     __crypts: Optional[Crypts]
 
 
     def __init__(
         self,
         *,
-        files: Optional[PATHABLE] = None,
-        paths: Optional[PATHABLE] = None,
+        files: Optional['PATHABLE'] = None,
+        paths: Optional['PATHABLE'] = None,
         cargs: Optional[dict[str, Any]] = None,
         model: Optional[Callable] = None,  # type: ignore
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
```

### Comparing `encommon-0.7.6/encommon/config/files.py` & `encommon-0.8.0/encommon/config/files.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,20 +7,23 @@
 
 
 
 from copy import deepcopy
 from pathlib import Path
 from typing import Any
 from typing import Optional
+from typing import TYPE_CHECKING
 
 from .common import config_load
 from .common import config_path
 from .common import config_paths
 from ..types import merge_dicts
-from ..utils.common import PATHABLE
+
+if TYPE_CHECKING:
+    from ..utils.common import PATHABLE
 
 
 
 class ConfigFile:
     """
     Contain the configuration content from filesystem path.
 
@@ -59,15 +62,15 @@
     config: dict[str, ConfigFile]
 
     __merged: Optional[dict[str, Any]]
 
 
     def __init__(
         self,
-        paths: PATHABLE,
+        paths: 'PATHABLE',
         force: bool = False,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
         self.paths = config_paths(paths)
@@ -85,26 +88,29 @@
     ) -> dict[str, Any]:
         """
         Return the configuration in dictionary format for files.
 
         :returns: Configuration in dictionary format for files.
         """
 
-        if self.__merged is not None:
-            return deepcopy(self.__merged)
+        config = self.config
+        merged = self.__merged
+
+        if merged is not None:
+            return deepcopy(merged)
 
-        merged: dict[str, Any] = {}
+        merged = {}
 
 
-        for _, file in self.config.items():
+        for file in config.values():
 
             source = file.config
 
             merge_dicts(
                 dict1=merged,
                 dict2=deepcopy(source),
                 force=False)
 
 
         self.__merged = merged
 
-        return deepcopy(self.__merged)
+        return deepcopy(merged)
```

### Comparing `encommon-0.7.6/encommon/config/logger.py` & `encommon-0.8.0/encommon/config/logger.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,26 +24,30 @@
 from typing import Any
 from typing import Literal
 from typing import Optional
 from typing import TYPE_CHECKING
 
 from .common import LOGLEVELS
 from .common import config_path
-from ..times.common import PARSABLE
-from ..times.times import Times
-from ..types.empty import Empty
-from ..utils.stdout import kvpair_ansi
+from ..times import Times
+from ..types import Empty
+from ..types.strings import COMMAD
+from ..types.strings import COMMAS
+from ..types.strings import SPACED
+from ..utils import kvpair_ansi
+from ..utils.common import JOINABLE
 
 if TYPE_CHECKING:
     from .params import LoggerParams
+    from ..times.common import PARSABLE
 
 
 
-LOGGER_FILE = 'encommon.logger.file'
-LOGGER_STDO = 'encommon.logger.stdo'
+LOGR_FILE = 'encommon.logger.file'
+LOGR_STDO = 'encommon.logger.stdo'
 
 LOGSEVERS = {
     'critical': int(CRITICAL),
     'debug': int(DEBUG),
     'error': int(ERROR),
     'info': int(INFO),
     'warning': int(WARNING)}
@@ -75,38 +79,52 @@
     __time: Times
     __fields: dict[str, str] = {}
 
 
     def __init__(
         self,
         level: LOGLEVELS,
-        time: Optional[PARSABLE] = None,
+        time: Optional['PARSABLE'] = None,
         **kwargs: Any,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
         self.__level = level
         self.__time = Times(time)
         self.__fields = {}
 
-        for key, value in kwargs.items():
+        items = kwargs.items()
+
+        for key, value in items:
+
 
             if (hasattr(value, '__len__')
                     and not len(value)):
                 continue
 
             if value in [None, Empty]:
                 continue
 
-            if (key == 'elapsed'
-                    and isinstance(value, float)):
+
+            if isinstance(value, JOINABLE):
+
+                values = sorted(
+                    str(x) for x in value)
+
+                value = COMMAD.join(values)
+
+
+            if (isinstance(value, float)
+                    and key == 'elapsed'):
+
                 value = round(value, 2)
 
+
             value = str(value)
 
             self.__fields[key] = value
 
 
     def __repr__(
         self,
@@ -119,15 +137,15 @@
 
         fields: dict[str, str] = {
             'level': self.__level,
             'time': self.__time.subsec}
 
         fields |= dict(self.__fields)
 
-        message = ', '.join([
+        message = COMMAS.join([
             f'{k}="{v}"' for k, v
             in fields.items()])
 
         return f'Message({message})'
 
 
     def __str__(
@@ -201,19 +219,24 @@
         fields['time'] = (
             fields['time']
             .replace('+0000', 'Z'))
 
 
         output: list[str] = []
 
-        for key, value in fields.items():
-            output.append(
-                kvpair_ansi(key, value))
+        items = fields.items()
+
+        for field, value in items:
+
+            _value = kvpair_ansi(
+                field, value)
+
+            output.append(_value)
 
-        return ' '.join(output)
+        return SPACED.join(output)
 
 
     @property
     def file_output(
         self,
     ) -> str:
         """
@@ -231,15 +254,15 @@
 
         return dumps(fields)
 
 
 
 class FileFormatter(Formatter):
     """
-    Supplement class for built-in logging exception formatter.
+    Supplement class for built-in logger exception formatter.
     """
 
 
     def formatException(
         self,
         ei: Any,  # noqa: ANN401
     ) -> str:
@@ -295,16 +318,16 @@
 
     __stdo_level: Optional[LOGLEVELS]
     __file_level: Optional[LOGLEVELS]
     __file_path: Optional[Path]
 
     __started: bool
 
-    __logger_stdo: _Logger
-    __logger_file: _Logger
+    __logr_stdo: _Logger
+    __logr_file: _Logger
 
 
     def __init__(
         self,
         *,
         stdo_level: Optional[LOGLEVELS] = None,
         file_level: Optional[LOGLEVELS] = None,
@@ -325,16 +348,19 @@
 
         self.__stdo_level = stdo_level
         self.__file_level = file_level
         self.__file_path = file_path
 
         self.__started = False
 
-        self.__logger_stdo = getLogger(LOGGER_STDO)
-        self.__logger_file = getLogger(LOGGER_FILE)
+        logr_stdo = getLogger(LOGR_STDO)
+        logr_file = getLogger(LOGR_FILE)
+
+        self.__logr_stdo = logr_stdo
+        self.__logr_file = logr_file
 
 
     @property
     def stdo_level(
         self,
     ) -> Optional[LOGLEVELS]:
         """
@@ -391,220 +417,200 @@
     ) -> _Logger:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return self.__logger_stdo
+        return self.__logr_stdo
 
 
     @property
     def logger_file(
         self,
     ) -> _Logger:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return self.__logger_file
+        return self.__logr_file
 
 
     def start(
         self,
     ) -> None:
         """
         Initialize the Python logging library using parameters.
         """
 
         stdo_level = self.__stdo_level
         file_level = self.__file_level
         file_path = self.__file_path
 
-        logger_stdo = self.__logger_stdo
-        logger_file = self.__logger_file
+        logr_stdo = self.__logr_stdo
+        logr_file = self.__logr_file
+
 
+        logr_root = getLogger()
 
-        logger_root = getLogger()
-        logger_root.setLevel(NOTSET)
+        logr_root.setLevel(NOTSET)
 
-        logger_stdo.handlers = [NullHandler()]
-        logger_file.handlers = [NullHandler()]
+        logr_stdo.handlers = [NullHandler()]
+        logr_file.handlers = [NullHandler()]
 
 
         if stdo_level is not None:
 
-            stdoh = StreamHandler()
-            format = Formatter('%(message)s')
             level = LOGSEVERS[stdo_level]
 
-            stdoh.setLevel(level)
-            stdoh.setFormatter(format)
+            handstdo = StreamHandler()
+
+            format = Formatter(
+                '%(message)s')
+
+            logr_stdo.handlers = [handstdo]
 
-            logger_stdo.handlers = [stdoh]
+            handstdo.setLevel(level)
+            handstdo.setFormatter(format)
 
 
         if file_path and file_level:
 
-            fileh = FileHandler(file_path)
-            format = FileFormatter('%(message)s')
             level = LOGSEVERS[file_level]
 
-            fileh.setLevel(level)
-            fileh.setFormatter(format)
+            handfile = (
+                FileHandler(file_path))
 
-            logger_file.handlers = [fileh]
+            format = FileFormatter(
+                '%(message)s')
+
+            logr_file.handlers = [handfile]
+
+            handfile.setLevel(level)
+            handfile.setFormatter(format)
 
 
         self.__started = True
 
 
     def stop(
         self,
     ) -> None:
         """
         Deinitialize the Python logging library using parameters.
         """
 
-        logger_stdo = self.__logger_stdo
-        logger_file = self.__logger_file
+        logr_stdo = self.__logr_stdo
+        logr_file = self.__logr_file
 
-        logger_stdo.handlers = [NullHandler()]
-        logger_file.handlers = [NullHandler()]
+        logr_stdo.handlers = [NullHandler()]
+        logr_file.handlers = [NullHandler()]
 
         self.__started = False
 
 
     def log(
         self,
         level: Literal[LOGLEVELS],
         *,
         exc_info: Optional[Exception] = None,
         **kwargs: Any,
     ) -> None:
         """
-        Prepare keyword arguments and log to the relevant outputs.
+        Prepare keyword arguments and log to configured output.
 
-        :param exc_info: Optional exception to include with trace.
+        :param exc_info: Optional exception included with trace.
         :param kwargs: Keyword arguments for populating message.
         """
 
         if self.__started is False:
             return
 
         stdo_level = self.__stdo_level
         file_level = self.__file_level
         file_path = self.__file_path
 
-        logger_stdo = self.__logger_stdo
-        logger_file = self.__logger_file
+        logr_stdo = self.__logr_stdo
+        logr_file = self.__logr_file
 
         message = Message(level, **kwargs)
 
         if stdo_level is not None:
-            logger_stdo.log(
+
+            logr_stdo.log(
                 level=LOGSEVERS[level],
                 msg=message.stdo_output,
                 exc_info=exc_info)
 
         if file_path and file_level:
-            logger_file.log(
+
+            logr_file.log(
                 level=LOGSEVERS[level],
                 msg=message.file_output,
                 exc_info=exc_info)
 
 
     def log_c(
         self,
-        *,
-        exc_info: Optional[Exception] = None,
         **kwargs: Any,
     ) -> None:
         """
-        Prepare keyword arguments and log to the relevant outputs.
+        Prepare keyword arguments and log to configured output.
 
-        :param exc_info: Optional exception to include with trace.
         :param kwargs: Keyword arguments for populating message.
         """
 
-        self.log(
-            level='critical',
-            exc_info=exc_info,
-            **kwargs)
+        self.log('critical', **kwargs)
 
 
     def log_d(
         self,
-        *,
-        exc_info: Optional[Exception] = None,
         **kwargs: Any,
     ) -> None:
         """
-        Prepare keyword arguments and log to the relevant outputs.
+        Prepare keyword arguments and log to configured output.
 
-        :param exc_info: Optional exception to include with trace.
         :param kwargs: Keyword arguments for populating message.
         """
 
-        self.log(
-            level='debug',
-            exc_info=exc_info,
-            **kwargs)
+        self.log('debug', **kwargs)
 
 
     def log_e(
         self,
-        *,
-        exc_info: Optional[Exception] = None,
         **kwargs: Any,
     ) -> None:
         """
-        Prepare keyword arguments and log to the relevant outputs.
+        Prepare keyword arguments and log to configured output.
 
-        :param exc_info: Optional exception to include with trace.
         :param kwargs: Keyword arguments for populating message.
         """
 
-        self.log(
-            level='error',
-            exc_info=exc_info,
-            **kwargs)
+        self.log('error', **kwargs)
 
 
     def log_i(
         self,
-        *,
-        exc_info: Optional[Exception] = None,
         **kwargs: Any,
     ) -> None:
         """
-        Prepare keyword arguments and log to the relevant outputs.
+        Prepare keyword arguments and log to configured output.
 
-        :param exc_info: Optional exception to include with trace.
         :param kwargs: Keyword arguments for populating message.
         """
 
-        self.log(
-            level='info',
-            exc_info=exc_info,
-            **kwargs)
+        self.log('info', **kwargs)
 
 
     def log_w(
         self,
-        *,
-        exc_info: Optional[Exception] = None,
         **kwargs: Any,
     ) -> None:
         """
-        Prepare keyword arguments and log to the relevant outputs.
+        Prepare keyword arguments and log to configured output.
 
-        :param exc_info: Optional exception to include with trace.
         :param kwargs: Keyword arguments for populating message.
         """
 
-        self.log(
-            level='warning',
-            exc_info=exc_info,
-            **kwargs)
+        self.log('warning', **kwargs)
```

### Comparing `encommon-0.7.6/encommon/config/params.py` & `encommon-0.8.0/encommon/config/params.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 from typing import Optional
 
 from pydantic import BaseModel
 
 from .common import LOGLEVELS
-from ..crypts.params import CryptsParams
+from ..crypts import CryptsParams
 
 
 
 class ConfigParams(BaseModel, extra='forbid'):
     """
     Process and validate the common configuration parameters.
```

### Comparing `encommon-0.7.6/encommon/config/paths.py` & `encommon-0.8.0/encommon/config/paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,22 @@
 
 
 from copy import deepcopy
 from glob import glob
 from pathlib import Path
 from typing import Any
 from typing import Optional
+from typing import TYPE_CHECKING
 
 from .common import config_path
 from .common import config_paths
 from .files import ConfigFile
-from ..utils.common import PATHABLE
+
+if TYPE_CHECKING:
+    from ..utils.common import PATHABLE
 
 
 
 class ConfigPath:
     """
     Contain the configuration content from filesystem path.
 
@@ -67,15 +70,15 @@
     config: dict[str, ConfigPath]
 
     __merged: Optional[dict[str, Any]]
 
 
     def __init__(
         self,
-        paths: PATHABLE,
+        paths: 'PATHABLE',
         force: bool = False,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
         self.paths = config_paths(paths)
@@ -93,23 +96,28 @@
     ) -> dict[str, Any]:
         """
         Return the configuration in dictionary format for paths.
 
         :returns: Configuration in dictionary format for paths.
         """
 
-        if self.__merged is not None:
-            return deepcopy(self.__merged)
+        config = self.config
+        merged = self.__merged
+
+        if merged is not None:
+            return deepcopy(merged)
+
+        merged = {}
 
-        merged: dict[str, Any] = {}
 
+        for path in config.values():
 
-        for _, path in self.config.items():
+            items = path.config.items()
 
-            for key, file in path.config.items():
+            for key, file in items:
 
                 merged[key] = file.config
 
 
         self.__merged = merged
 
-        return deepcopy(self.__merged)
+        return deepcopy(merged)
```

### Comparing `encommon-0.7.6/encommon/config/test/test_common.py` & `encommon-0.8.0/encommon/config/test/test_common.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,30 +5,53 @@
 is permitted, for more information consult the project license file.
 """
 
 
 
 from ..common import config_load
 from ..common import config_path
+from ..common import config_paths
 from ... import PROJECT
 from ... import WORKSPACE
 
 
 
 def test_config_load() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
-    path = 'PROJECT/../.yamllint'
+    loaded = config_load(
+        'PROJECT/../.yamllint')
 
-    assert len(config_load(path)) == 2
+    assert list(loaded) == [
+        'extends', 'rules']
 
 
 
 def test_config_path() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
-    assert config_path('PROJECT') == PROJECT
-    assert config_path('WORKSPACE') == WORKSPACE
+
+    path = config_path('PROJECT')
+
+    assert path == PROJECT
+
+
+    path = config_path('WORKSPACE')
+
+    assert path == WORKSPACE
+
+
+
+def test_config_paths() -> None:
+    """
+    Perform various tests associated with relevant routines.
+    """
+
+    paths = config_paths([
+        'PROJECT', 'WORKSPACE'])
+
+    assert paths == (
+        PROJECT, WORKSPACE)
```

### Comparing `encommon-0.7.6/encommon/config/test/test_config.py` & `encommon-0.8.0/encommon/config/test/test_config.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,148 +4,114 @@
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
 from pathlib import Path
+from typing import TYPE_CHECKING
 
 from . import SAMPLES
-from ..config import Config
 from ..logger import Logger
 from ..params import Params
 from ... import ENPYRWS
-from ...crypts.crypts import Crypts
-from ...utils.sample import load_sample
-from ...utils.sample import prep_sample
+from ... import PROJECT
+from ...crypts import Crypts
+from ...utils import load_sample
+from ...utils import prep_sample
 
+if TYPE_CHECKING:
+    from ..config import Config
 
 
-def test_Config(  # noqa: CFQ001
-    config_path: Path,
+
+def test_Config(
+    tmp_path: Path,
+    config: 'Config',
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
-    :param config_path: Custom fixture for populating paths.
+    :param tmp_path: pytest object for temporal filesystem.
+    :param config: Primary class instance for configuration.
     """
 
-    (config_path
-        .joinpath('one.yml')
-        .write_text(
-            'enconfig:\n'
-            f'  paths: ["{config_path}"]\n'
-            'enlogger:\n'
-            '  stdo_level: info\n'))
-
-    (config_path
-        .joinpath('two.yml')
-        .write_text(
-            'encrypts:\n'
-            '  phrases:\n'
-            '    default: fernetphrase\n'
-            'enlogger:\n'
-            '  stdo_level: debug\n'
-            '  file_level: info\n'))
-
-
-    config = Config(
-        files=[
-            f'{config_path}/one.yml',
-            f'{config_path}/two.yml'],
-        cargs={
-            'enlogger': {
-                'file_level': 'warning'}})
 
     attrs = list(config.__dict__)
 
     assert attrs == [
         '_Config__model',
         '_Config__files',
         '_Config__cargs',
         '_Config__params',
         '_Config__paths',
         '_Config__logger',
         '_Config__crypts']
 
 
-    assert repr(config).startswith(
-        '<encommon.config.config.Config')
-    assert isinstance(hash(config), int)
-    assert str(config).startswith(
-        '<encommon.config.config.Config')
-
+    assert repr(config)[:23] == (
+        '<encommon.config.config')
 
-    assert len(config.files.paths) == 2
-    assert len(config.paths.paths) == 1
-    assert len(config.cargs) == 1
-    assert isinstance(config.config, dict)
-    assert config.model is Params
-    assert isinstance(config.params, Params)
+    assert hash(config) > 0
 
+    assert str(config)[:23] == (
+        '<encommon.config.config')
 
-    _config1 = config.config
-    _config2 = config.config
 
-    assert _config1 is not _config2
+    assert 'ConfigFiles' in str(config.files)
 
+    assert 'ConfigPaths' in str(config.paths)
 
-    sample_path = Path(
-        f'{SAMPLES}/config.json')
+    assert len(config.cargs) == 1
 
-    sample = load_sample(
-        path=sample_path,
-        update=ENPYRWS,
-        content=_config1,
-        replace={
-            'config_path': str(config_path)})
+    assert len(config.config) == 3
 
-    expect = prep_sample(
-        content=_config2,
-        replace={
-            'config_path': str(config_path)})
+    assert config.model is Params
 
-    assert sample == expect
+    assert isinstance(config.params, Params)
 
+    assert isinstance(config.logger, Logger)
 
-    _params1 = config.params
-    _params2 = config.params
+    assert isinstance(config.crypts, Crypts)
 
-    assert _params1 is _params2
 
+    replaces = {
+        'pytemp': tmp_path,
+        'PROJECT': PROJECT}
 
-    sample_path = Path(
-        f'{SAMPLES}/params.json')
+    sample_path = (
+        f'{SAMPLES}/config.json')
 
     sample = load_sample(
         path=sample_path,
         update=ENPYRWS,
-        content=_params1.model_dump(),
-        replace={
-            'config_path': str(config_path)})
+        content=config.config,
+        replace=replaces)
 
     expect = prep_sample(
-        content=_params2.model_dump(),
-        replace={
-            'config_path': str(config_path)})
+        content=config.config,
+        replace=replaces)
 
     assert sample == expect
 
 
-    logger = config.logger
 
-    assert isinstance(logger, Logger)
+def test_Config_cover(
+    config: 'Config',
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
 
-    _logger1 = config.logger
-    _logger2 = config.logger
+    :param config: Primary class instance for configuration.
+    """
 
-    assert _logger1 is _logger2
 
+    logger1 = config.logger
+    logger2 = config.logger
 
-    crypts = config.crypts
+    assert logger1 is logger2
 
-    assert isinstance(crypts, Crypts)
 
-    _crypts1 = config.crypts
-    _crypts2 = config.crypts
+    crypts1 = config.crypts
+    crypts2 = config.crypts
 
-    assert _crypts1 is _crypts2
+    assert crypts1 is crypts2
```

### Comparing `encommon-0.7.6/encommon/config/test/test_files.py` & `encommon-0.8.0/encommon/config/test/test_files.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,101 +5,116 @@
 is permitted, for more information consult the project license file.
 """
 
 
 
 from pathlib import Path
 
+from pytest import fixture
+
 from . import SAMPLES
 from ..files import ConfigFile
 from ..files import ConfigFiles
-from ... import ENPYRWS
-from ...utils.sample import load_sample
-from ...utils.sample import prep_sample
+
+
+
+@fixture
+def files(
+    config_path: Path,
+) -> ConfigFiles:
+    """
+    Construct the instance for use in the downstream tests.
+
+    :param config_path: Custom fixture for populating paths.
+    :returns: Newly constructed instance of related class.
+    """
+
+    return ConfigFiles([
+        f'{SAMPLES}/wayne/bwayne.yml',
+        f'{SAMPLES}/stark/tstark.yml'])
 
 
 
 def test_ConfigFile(
     config_path: Path,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param config_path: Custom fixture for populating paths.
     """
 
     file = ConfigFile(
-        f'{config_path}/wayne/bwayne.yml')
+        f'{config_path}/config.yml')
+
 
     attrs = list(file.__dict__)
 
-    assert attrs == ['path', 'config']
+    assert attrs == [
+        'path',
+        'config']
+
 
+    assert repr(file)[:22] == (
+        '<encommon.config.files')
 
-    assert repr(file).startswith(
-        '<encommon.config.files.ConfigFile')
-    assert isinstance(hash(file), int)
-    assert str(file).startswith(
-        '<encommon.config.files.ConfigFile')
+    assert hash(file) > 0
 
+    assert str(file)[:22] == (
+        '<encommon.config.files')
 
-    assert file.path.name == 'bwayne.yml'
-    assert list(file.config) == ['name']
+
+    assert file.path.name == 'config.yml'
+
+    assert len(file.config) == 3
 
 
 
 def test_ConfigFiles(
-    config_path: Path,
+    files: ConfigFiles,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
-    :param config_path: Custom fixture for populating paths.
+    :param files: Custom fixture for the configuration files.
     """
 
-    files = ConfigFiles([
-        f'{config_path}/wayne/bwayne.yml',
-        f'{config_path}/stark/tstark.yml'])
 
     attrs = list(files.__dict__)
 
     assert attrs == [
-        'paths', 'config',
+        'paths',
+        'config',
         '_ConfigFiles__merged']
 
 
-    assert repr(files).startswith(
-        '<encommon.config.files.ConfigFiles')
-    assert isinstance(hash(files), int)
-    assert str(files).startswith(
-        '<encommon.config.files.ConfigFiles')
+    assert repr(files)[:22] == (
+        '<encommon.config.files')
 
+    assert hash(files) > 0
 
-    assert len(files.paths) == 2
-    assert len(files.config) == 2
+    assert str(files)[:22] == (
+        '<encommon.config.files')
 
 
-    files = ConfigFiles(
-        f'{config_path}/wayne/bwayne.yml')
+    assert len(files.paths) == 2
 
+    assert len(files.config) == 2
+
+    assert files.merged == {
+        'name': 'Bruce Wayne'}
 
-    _merged1 = files.merged
-    _merged2 = files.merged
 
-    assert _merged1 is not _merged2
 
-    sample_path = Path(
-        f'{SAMPLES}/files.json')
+def test_ConfigFiles_cover(
+    files: ConfigFiles,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
 
-    sample = load_sample(
-        path=sample_path,
-        update=ENPYRWS,
-        content=_merged1,
-        replace={
-            'config_path': str(config_path)})
+    :param files: Custom fixture for the configuration files.
+    """
 
-    expect = prep_sample(
-        content=_merged2,
-        replace={
-            'config_path': str(config_path)})
+    merged1 = files.merged
+    merged2 = files.merged
 
-    assert sample == expect
+    assert merged1 is not merged2
```

### Comparing `encommon-0.7.6/encommon/config/test/test_logger.py` & `encommon-0.8.0/encommon/config/test/test_logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,175 +3,221 @@
 
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
-from logging import Logger as _Logger
 from pathlib import Path
 
 from _pytest.logging import LogCaptureFixture
 
+from pytest import fixture
+
 from ..logger import Logger
 from ..logger import Message
+from ..params import LoggerParams
 from ...times.common import UNIXMPOCH
-from ...utils.stdout import strip_ansi
+from ...times.common import UNIXSPOCH
+from ...utils import strip_ansi
+
+
+
+_CAPLOG = list[tuple[str, int, str]]
+
+
+
+@fixture
+def logger(
+    tmp_path: Path,
+) -> Logger:
+    """
+    Construct the instance for use in the downstream tests.
+
+    :param tmp_path: pytest object for temporal filesystem.
+    :returns: Newly constructed instance of related class.
+    """
+
+    params = LoggerParams(
+        stdo_level='info',
+        file_level='info',
+        file_path=f'{tmp_path}/test.log')
+
+    return Logger(params=params)
 
 
 
 def test_Message() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
-
     message = Message(
         time=UNIXMPOCH,
         level='info',
-        dict={'foo': 'bar'},
-        empty=[],
-        float=1.0,
-        int=1,
-        list=[1, '2', 3],
+        string='foobar',
         none=None,
-        string='foo',
-        elapsed=0.69420)
+        list=['1', 2],
+        tuple=('1', 2),
+        set={'1', 2},
+        dict={'1': 2},
+        empty_list=[],
+        empty_dict={},
+        int=1,
+        float=2.0,
+        elapsed=3.69420)
+
 
     attrs = list(message.__dict__)
 
     assert attrs == [
         '_Message__level',
         '_Message__time',
         '_Message__fields']
 
 
-    assert repr(message).startswith(
-        'Message(level="info", time="1970')
-    assert isinstance(hash(message), int)
-    assert str(message).startswith(
-        'Message(level="info", time="1970')
-
-
-    assert repr(message) == (
-        'Message('
-        'level="info", '
-        f'time="{UNIXMPOCH}", '
-        'dict="{\'foo\': \'bar\'}", '
-        'float="1.0", '
-        'int="1", '
-        'list="[1, \'2\', 3]", '
-        'string="foo", '
-        'elapsed="0.69")')
+    assert repr(message)[:20] == (
+        'Message(level="info"')
+
+    assert hash(message) > 0
 
-    assert str(message) == repr(message)
+    assert str(message)[:20] == (
+        'Message(level="info"')
 
 
     assert message.level == 'info'
-    assert message.time == '1970-01-01'
 
-    assert message.fields == {
-        'dict': "{'foo': 'bar'}",
-        'float': '1.0',
-        'int': '1',
-        'list': "[1, '2', 3]",
-        'string': 'foo',
-        'elapsed': '0.69'}
+    assert message.time == 0
+
+    assert len(message.fields) == 8
 
 
-    output = strip_ansi(message.stdo_output)
+    output = strip_ansi(
+        message.stdo_output)
 
     assert output == (
         'level="info"'
-        ' time="1970-01-01T00:00:00Z"'
-        ' dict="{\'foo\': \'bar\'}"'
-        ' float="1.0"'
+        f' time="{UNIXSPOCH}"'
+        ' string="foobar"'
+        ' list="1,2"'
+        ' tuple="1,2"'
+        ' set="1,2"'
+        ' dict="{\'1\': 2}"'
         ' int="1"'
-        ' list="[1, \'2\', 3]"'
-        ' string="foo"'
-        ' elapsed="0.69"')
+        ' float="2.0"'
+        ' elapsed="3.69"')
 
 
-    assert message.file_output == (
+    output = message.file_output
+
+    assert output == (
         '{"level": "info",'
         f' "time": "{UNIXMPOCH}",'
-        ' "dict": "{\'foo\': \'bar\'}",'
-        ' "float": "1.0",'
+        ' "string": "foobar",'
+        ' "list": "1,2",'
+        ' "tuple": "1,2",'
+        ' "set": "1,2",'
+        ' "dict": "{\'1\': 2}",'
         ' "int": "1",'
-        ' "list": "[1, \'2\', 3]",'
-        ' "string": "foo",'
-        ' "elapsed": "0.69"}')
+        ' "float": "2.0",'
+        ' "elapsed": "3.69"}')
 
 
 
 def test_Logger(
-    tmp_path: Path,
+    logger: Logger,
     caplog: LogCaptureFixture,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
-    :param tmp_path: pytest object for temporal filesystem.
+    :param logger: Custom fixture for the logger instance.
     :param caplog: pytest object for capturing log message.
     """
 
 
-    logger = Logger(
-        stdo_level='info',
-        file_level='info',
-        file_path=f'{tmp_path}/test.log')
-
     attrs = list(logger.__dict__)
 
     assert attrs == [
         '_Logger__stdo_level',
         '_Logger__file_level',
         '_Logger__file_path',
         '_Logger__started',
-        '_Logger__logger_stdo',
-        '_Logger__logger_file']
+        '_Logger__logr_stdo',
+        '_Logger__logr_file']
+
+
+    assert repr(logger)[:23] == (
+        '<encommon.config.logger')
 
+    assert hash(logger) > 0
 
-    assert repr(logger).startswith(
-        '<encommon.config.logger.Logger')
-    assert isinstance(hash(logger), int)
-    assert str(logger).startswith(
-        '<encommon.config.logger.Logger')
+    assert str(logger)[:23] == (
+        '<encommon.config.logger')
 
 
     assert logger.stdo_level == 'info'
+
     assert logger.file_level == 'info'
+
     assert logger.file_path is not None
-    assert logger.file_path.name == 'test.log'
+
     assert logger.started is False
-    assert isinstance(logger.logger_stdo, _Logger)
-    assert isinstance(logger.logger_file, _Logger)
+
+    assert logger.logger_stdo is not None
+
+    assert logger.logger_file is not None
+
+
+    logger.log_d(msg='pytest')
+    logger.log_c(msg='pytest')
+    logger.log_e(msg='pytest')
+    logger.log_i(msg='pytest')
+    logger.log_w(msg='pytest')
+
+
+
+def test_Logger_cover(
+    logger: Logger,
+    caplog: LogCaptureFixture,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param logger: Custom fixture for the logger instance.
+    :param caplog: pytest object for capturing log message.
+    """
 
 
     def _logger_logs() -> None:
-        logger.log_d(message='pytest')
-        logger.log_c(message='pytest')
-        logger.log_e(message='pytest')
-        logger.log_i(message='pytest')
-        logger.log_w(message='pytest')
+        logger.log_d(msg='pytest')
+        logger.log_c(msg='pytest')
+        logger.log_e(msg='pytest')
+        logger.log_i(msg='pytest')
+        logger.log_w(msg='pytest')
 
 
-    _caplog = list[tuple[str, int, str]]
+    def _logger_stdo() -> _CAPLOG:
 
+        output = caplog.record_tuples
+        key = 'encommon.logger.stdo'
 
-    def _logger_stdo() -> _caplog:
         return [
-            x for x in caplog.record_tuples
-            if x[0] == 'encommon.logger.stdo']
+            x for x in output
+            if x[0] == key]
+
+
+    def _logger_file() -> _CAPLOG:
 
+        output = caplog.record_tuples
+        key = 'encommon.logger.file'
 
-    def _logger_file() -> _caplog:
         return [
-            x for x in caplog.record_tuples
-            if x[0] == 'encommon.logger.file']
+            x for x in output
+            if x[0] == key]
 
 
     logger.start()
 
     _logger_logs()
 
     assert len(_logger_stdo()) == 5
@@ -185,24 +231,25 @@
     assert len(_logger_stdo()) == 5
     assert len(_logger_file()) == 5
 
 
     logger.start()
 
     message = 'unknown exception'
+    raises = Exception('pytest')
 
     logger.log_e(
         message=message,
-        exc_info=Exception('pytest'))
+        exc_info=raises)
 
-    stdo_text = _logger_stdo()[-1][2]
-    file_text = _logger_file()[-1][2]
+    stdo = _logger_stdo()[-1][2]
+    file = _logger_file()[-1][2]
 
-    assert message in str(stdo_text)
-    assert message in str(file_text)
+    assert message in str(stdo)
+    assert message in str(file)
 
     assert len(_logger_stdo()) == 6
     assert len(_logger_file()) == 6
 
     logger.stop()
```

### Comparing `encommon-0.7.6/encommon/config/test/test_paths.py` & `encommon-0.8.0/encommon/config/test/test_paths.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,94 +5,134 @@
 is permitted, for more information consult the project license file.
 """
 
 
 
 from pathlib import Path
 
+from pytest import fixture
+
 from . import SAMPLES
 from ..paths import ConfigPath
 from ..paths import ConfigPaths
 from ... import ENPYRWS
-from ...utils.sample import load_sample
-from ...utils.sample import prep_sample
+from ... import PROJECT
+from ...utils import load_sample
+from ...utils import prep_sample
+
+
+
+@fixture
+def paths(
+    config_path: Path,
+) -> ConfigPaths:
+    """
+    Construct the instance for use in the downstream tests.
+
+    :param config_path: Custom fixture for populating paths.
+    :returns: Newly constructed instance of related class.
+    """
+
+    return ConfigPaths([
+        f'{SAMPLES}/stark',
+        f'{SAMPLES}/wayne'])
 
 
 
 def test_ConfigPath(
     config_path: Path,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param config_path: Custom fixture for populating paths.
     """
 
     path = ConfigPath(config_path)
 
+
     attrs = list(path.__dict__)
 
-    assert attrs == ['path', 'config']
+    assert attrs == [
+        'path',
+        'config']
+
+
+    assert repr(path)[:22] == (
+        '<encommon.config.paths')
+
+    assert hash(path) > 0
 
+    assert str(path)[:22] == (
+        '<encommon.config.paths')
 
-    assert repr(path).startswith(
-        '<encommon.config.paths.ConfigPath')
-    assert isinstance(hash(path), int)
-    assert str(path).startswith(
-        '<encommon.config.paths.ConfigPath')
 
+    assert 'test' in path.path.name
 
-    assert path.path == config_path
-    assert len(path.config) == 2
+    assert len(path.config) == 1
 
 
 
 def test_ConfigPaths(
-    config_path: Path,
+    paths: ConfigPaths,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
-    :param config_path: Custom fixture for populating paths.
+    :param paths: Custom fixture for the configuration paths.
     """
 
-    paths = ConfigPaths(config_path)
 
     attrs = list(paths.__dict__)
 
     assert attrs == [
         'paths', 'config',
         '_ConfigPaths__merged']
 
 
-    assert repr(paths).startswith(
-        '<encommon.config.paths.ConfigPaths')
-    assert isinstance(hash(paths), int)
-    assert str(paths).startswith(
-        '<encommon.config.paths.ConfigPaths')
+    assert repr(paths)[:22] == (
+        '<encommon.config.paths')
+
+    assert hash(paths) > 0
+
+    assert str(paths)[:22] == (
+        '<encommon.config.paths')
 
 
-    assert len(paths.paths) == 1
-    assert len(paths.config) == 1
+    assert len(paths.paths) == 2
 
+    assert len(paths.config) == 2
 
-    _merged1 = paths.merged
-    _merged2 = paths.merged
 
-    assert _merged1 is not _merged2
+    replaces = {
+        'PROJECT': PROJECT}
 
-    sample_path = Path(
+    sample_path = (
         f'{SAMPLES}/paths.json')
 
     sample = load_sample(
         path=sample_path,
         update=ENPYRWS,
-        content=_merged1,
-        replace={
-            'config_path': str(config_path)})
+        content=paths.merged,
+        replace=replaces)
 
     expect = prep_sample(
-        content=_merged2,
-        replace={
-            'config_path': str(config_path)})
+        content=paths.merged,
+        replace=replaces)
 
     assert sample == expect
+
+
+
+def test_ConfigPaths_cover(
+    paths: ConfigPaths,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param paths: Custom fixture for the configuration paths.
+    """
+
+    merged1 = paths.merged
+    merged2 = paths.merged
+
+    assert merged1 is not merged2
```

### Comparing `encommon-0.7.6/encommon/crypts/crypts.py` & `encommon-0.8.0/encommon/crypts/crypts.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from re import match as re_match
 from re import sub as re_sub
 from typing import Optional
 from typing import TYPE_CHECKING
 
 from cryptography.fernet import Fernet
 
+from ..types.strings import SEMPTY
+
 if TYPE_CHECKING:
     from .params import CryptsParams
 
 
 
 ENCRYPT = compile(
     r'^\$ENCRYPT;1\.\d;\S+\;.+?$')
@@ -153,8 +155,8 @@
 ) -> str:
     """
     Return the parsed and normalized encrypted string value.
 
     :param value: String value that will returned decrypted.
     """
 
-    return re_sub(r'[\n\s]', '', value)
+    return re_sub(r'[\n\s]', SEMPTY, value)
```

### Comparing `encommon-0.7.6/encommon/crypts/hashes.py` & `encommon-0.8.0/encommon/crypts/hashes.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
         string = self.__string.encode()
 
-        return sha1(string).hexdigest()  # noqa: S324
+        return sha1(string).hexdigest()
 
 
     @property
     def sha256(
         self,
     ) -> str:
         """
@@ -147,10 +147,10 @@
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
         string = self.__string.encode()
 
-        digest = sha1(string).digest()  # noqa: S324
+        digest = sha1(string).digest()
 
         return b64encode(digest).decode()
```

### Comparing `encommon-0.7.6/encommon/crypts/params.py` & `encommon-0.8.0/encommon/crypts/params.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.6/encommon/crypts/test/test_crypts.py` & `encommon-0.8.0/encommon/crypts/test/test_crypts.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,113 +8,135 @@
 
 
 from pytest import fixture
 from pytest import mark
 from pytest import raises
 
 from ..crypts import Crypts
+from ..params import CryptsParams
 
 
 
 @fixture
-def phrases() -> dict[str, str]:
+def crypts() -> Crypts:
     """
-    Construct randomly generated Fernet keys for passphrases.
+    Construct the instance for use in the downstream tests.
 
-    :returns: Randomly generated Fernet keys for passphrases.
+    :returns: Newly constructed instance of related class.
     """
 
-    return {
+    phrases = {
         'default': Crypts.keygen(),
         'secrets': Crypts.keygen()}
 
+    params = CryptsParams(
+        phrases=phrases)
+
+    return Crypts(params=params)
+
 
 
 def test_Crypts(
-    phrases: dict[str, str],
+    crypts: Crypts,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
-    :param phrases: Dictionary of randomly generated phrases.
+    :param crypts: Primary class instance for the encryption.
     """
 
-    crypts = Crypts(phrases)
 
     attrs = list(crypts.__dict__)
 
     assert attrs == [
         '_Crypts__phrases']
 
 
-    assert repr(crypts).startswith(
-        '<encommon.crypts.crypts.Crypts')
-    assert isinstance(hash(crypts), int)
-    assert str(crypts).startswith(
-        '<encommon.crypts.crypts.Crypts')
+    assert repr(crypts)[:23] == (
+        '<encommon.crypts.crypts')
+
+    assert hash(crypts) > 0
 
+    assert str(crypts)[:23] == (
+        '<encommon.crypts.crypts')
 
-    assert crypts.phrases == phrases
+
+    assert len(crypts.phrases) == 2
+
+    assert len(crypts.keygen()) == 44
 
 
 
 @mark.parametrize(
     'value,unique',
     [('foo', 'default'),
      ('foo', 'secrets')])
 def test_Crypts_iterate(
+    crypts: Crypts,
     value: str,
     unique: str,
-    phrases: dict[str, str],
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
+    :param crypts: Primary class instance for the encryption.
     :param value: String value that will returned encrypted.
     :param unique: Unique identifier of mapping passphrase.
-    :param phrases: Dictionary of randomly generated phrases.
     """
 
-    crypts = Crypts(phrases)
-
-    encrypt = crypts.encrypt(value, unique)
+    encrypt = (
+        crypts.encrypt(value, unique))
 
     split = encrypt.split(';')
 
     assert split[1] == '1.0'
     assert split[2] == unique
 
     decrypt = crypts.decrypt(encrypt)
 
     assert decrypt == value
 
 
 
 def test_Crypts_raises(
-    phrases: dict[str, str],
+    crypts: Crypts,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
-    :param phrases: Dictionary of randomly generated phrases.
+    :param crypts: Primary class instance for the encryption.
     """
 
 
-    with raises(ValueError) as reason:
+    _raises = raises(ValueError)
+
+    with _raises as reason:
         Crypts({'foo': 'bar'})
 
-    assert str(reason.value) == 'default'
+    _reason = str(reason.value)
+
+    assert _reason == 'default'
+
 
+    crypts = Crypts(
+        crypts.phrases)
 
-    crypts = Crypts(phrases)
 
+    _raises = raises(ValueError)
 
-    with raises(ValueError) as reason:
+    with _raises as reason:
         crypts.decrypt('foo')
 
-    assert str(reason.value) == 'string'
+    _reason = str(reason.value)
+
+    assert _reason == 'string'
+
+
+    _raises = raises(ValueError)
 
+    with _raises as reason:
+        string = '$ENCRYPT;1.1;f;oo'
+        crypts.decrypt(string)
 
-    with raises(ValueError) as reason:
-        crypts.decrypt('$ENCRYPT;1.1;f;oo')
+    _reason = str(reason.value)
 
-    assert str(reason.value) == 'version'
+    assert _reason == 'version'
```

### Comparing `encommon-0.7.6/encommon/times/__init__.py` & `encommon-0.8.0/encommon/times/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
+from .common import findtz
 from .duration import Duration
 from .parse import parse_time
 from .parse import shift_time
 from .parse import since_time
 from .parse import string_time
 from .timers import Timers
 from .times import Times
 from .window import Window
 
 
 
 __all__ = [
     'Duration',
+    'findtz',
     'Timers',
     'Times',
     'Window',
     'parse_time',
     'shift_time',
     'since_time',
     'string_time']
```

### Comparing `encommon-0.7.6/encommon/times/common.py` & `encommon-0.8.0/encommon/times/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,38 +6,72 @@
 """
 
 
 
 from contextlib import suppress
 from datetime import datetime
 from datetime import timezone
+from datetime import tzinfo
 from re import compile
 from typing import Any
+from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
+
+from dateutil.tz import gettz
+
 if TYPE_CHECKING:
     from .times import Times
 
 
 
-NUMERISH = compile(r'^\-?\d+(\.\d+)?$')
-SNAPABLE = compile(r'^(\-|\+)[\d\@a-z\-\+]+$')
-STRINGNOW = {'None', 'null', 'now'}
+NUMERISH = compile(
+    r'^\-?\d+(\.\d+)?$')
+
+SNAPABLE = compile(
+    r'^(\-|\+)[\d\@a-z\-\+]+$')
+
+STRINGNOW = {
+    'None', 'null', 'now'}
+
+
 
 NUMERIC = Union[int, float]
-PARSABLE = Union[str, NUMERIC, datetime, 'Times']
-SCHEDULE = Union[str, dict[str, int]]
 
-UNIXEPOCH = '1970-01-01T00:00:00+0000'
-UNIXMPOCH = '1970-01-01T00:00:00.000000+0000'
-UNIXHPOCH = '01/01/1970 12:00AM UTC'
-
-STAMP_SIMPLE = '%Y-%m-%dT%H:%M:%S%z'
-STAMP_SUBSEC = '%Y-%m-%dT%H:%M:%S.%f%z'
-STAMP_HUMAN = '%m/%d/%Y %I:%M%p %Z'
+PARSABLE = Union[
+    str, NUMERIC,
+    datetime, 'Times']
+
+SCHEDULE = Union[
+    str, dict[str, int]]
+
+
+
+UNIXEPOCH = (
+    '1970-01-01T00:00:00+0000')
+
+UNIXMPOCH = (
+    '1970-01-01T00:00:00.000000+0000')
+
+UNIXSPOCH = (
+    '1970-01-01T00:00:00Z')
+
+UNIXHPOCH = (
+    '01/01/1970 12:00AM UTC')
+
+
+
+STAMP_SIMPLE = (
+    '%Y-%m-%dT%H:%M:%S%z')
+
+STAMP_SUBSEC = (
+    '%Y-%m-%dT%H:%M:%S.%f%z')
+
+STAMP_HUMAN = (
+    '%m/%d/%Y %I:%M%p %Z')
 
 
 
 def utcdatetime(
     *args: Any,
     **kwargs: Any,
 ) -> datetime:
@@ -53,22 +87,24 @@
     datetime.datetime(1970, 1, 1, 0...
 
     :param args: Positional arguments passed for downstream.
     :param kwargs: Keyword arguments passed for downstream.
     :returns: Instance of datetime within the UTC timezone.
     """
 
+    tzinfo = timezone.utc
+
     if not args and not kwargs:
-        return datetime.now(tz=timezone.utc)
+        return datetime.now(tz=tzinfo)
 
     if 'tzinfo' not in kwargs:
-        kwargs['tzinfo'] = timezone.utc
+        kwargs['tzinfo'] = tzinfo
 
     return (
-        datetime(*args, **kwargs)  # noqa: DTZ001
+        datetime(*args, **kwargs)
         .astimezone(timezone.utc))
 
 
 
 def strptime(
     source: str,
     formats: str | list[str],
@@ -82,25 +118,73 @@
     datetime.datetime(2023, 1, 1, 0...
 
     :param source: Time in various forms that will be parsed.
     :param formats: Various formats compatable with strptime.
     :returns: Python datetime object containing related time.
     """
 
+    tzinfo = timezone.utc
+
     if isinstance(formats, str):
         formats = [formats]
 
 
     def _strptime(
         format: str,
     ) -> datetime:
+
         return (
             datetime
             .strptime(source, format)
-            .astimezone(timezone.utc))
+            .astimezone(tzinfo))
 
 
     for format in formats:
+
         with suppress(ValueError):
             return _strptime(format)
 
+
     raise ValueError('invalid')
+
+
+
+def strftime(
+    source: datetime,
+    format: str,
+) -> str:
+    """
+    Return the timestamp string for datetime object provided.
+
+    .. note::
+       This function is extremely pedantic and cosmetic.
+
+    :param source: Python datetime instance containing source.
+    :param format: Format for the timestamp string returned.
+    :returns: Timestamp string for datetime object provided.
+    """
+
+    return (
+        datetime
+        .strftime(source, format))
+
+
+
+def findtz(
+    tzname: Optional[str] = None,
+) -> tzinfo:
+    """
+    Return the located timezone object for the provided name.
+
+    :param tzname: Name of the timezone associated to source.
+    :returns: Located timezone object for the provided name.
+    """
+
+    if tzname is None:
+        return timezone.utc
+
+    tzinfo = gettz(tzname)
+
+    if tzinfo is None:
+        raise ValueError('tzname')
+
+    return tzinfo
```

### Comparing `encommon-0.7.6/encommon/times/duration.py` & `encommon-0.8.0/encommon/times/duration.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 
 
 from typing import Literal
 from typing import Union
 from typing import get_args
 
+from ..types.strings import COMMAS
+from ..types.strings import SEMPTY
+from ..types.strings import SPACED
+
 
 
 DURAGROUP = Literal[
     'year', 'month', 'week',
     'day', 'hour', 'minute',
     'second']
 
@@ -29,15 +33,15 @@
 DURAUNITS = Union[
     DURAGROUP, DURASHORT]
 
 
 
 class Duration:
     """
-    Convert provided the seconds into a human friendly format.
+    Convert the provided seconds in a human friendly format.
 
     Example
     -------
     >>> Duration(86400 * 700).compact
     '1y11mon5d'
 
     Example
@@ -48,16 +52,16 @@
     Example
     -------
     >>> Duration(7201, False).verbose
     '2 hours, 1 second'
 
     :param seconds: Period in seconds that will be iterated.
     :param smart: Determines if we hide seconds after minute.
-    :param groups: Determine the amount of groups to show,
-        ensuring the larger units are returned before smaller.
+    :param groups: Determine the quantity of groups to show,
+        ensuring larger units are returned before smaller.
     """
 
     __source: float
     __smart: bool
     __groups: int
 
 
@@ -118,27 +122,27 @@
 
     def __int__(
         self,
     ) -> int:
         """
         Built-in method representing numeric value for instance.
 
-        :returns: Numeric representation for values from instance.
+        :returns: Numeric representation for value in instance.
         """
 
         return int(self.__source)
 
 
     def __float__(
         self,
     ) -> float:
         """
         Built-in method representing numeric value for instance.
 
-        :returns: Numeric representation for values from instance.
+        :returns: Numeric representation for value in instance.
         """
 
         return float(self.__source)
 
 
     def __add__(
         self,
@@ -322,125 +326,135 @@
         :param short: Determine if we should use the short hand.
         :returns: Groups of time units with each relevant value.
         """
 
         source = self.__source
         seconds = int(source)
 
-        returned: dict[DURAUNITS, int] = {}
+        units: dict[DURAUNITS, int] = {}
 
         groups: dict[DURAGROUP, int] = {
             'year': 31536000,
             'month': 2592000,
             'week': 604800,
             'day': 86400,
             'hour': 3600,
             'minute': 60}
 
 
-        for key, value in groups.items():
+        items = groups.items()
+
+        for key, value in items:
 
             if seconds < value:
                 continue
 
             _value = seconds // value
+            seconds %= value
 
-            returned[key] = _value
+            units[key] = _value
 
-            seconds %= value
 
+        if ((seconds >= 1
+                and source > 60)
+                or source < 60):
+            units['second'] = seconds
 
-        if (source < 60
-                or (seconds >= 1
-                    and source > 60)):
-            returned['second'] = seconds
-
-        if (self.__smart
-                and 'second' in returned
-                and len(returned) >= 2):
-            del returned['second']
+        if ('second' in units
+                and len(units) >= 2
+                and self.__smart):
+            del units['second']
 
 
-        items = (
-            list(returned.items())
+        _groups = (
+            list(units.items())
             [:self.__groups])
 
         if short is False:
-            return dict(items)
+            return dict(_groups)
 
         return {
             DURAMAPS[k]: v
-            for k, v in items}
+            for k, v in _groups}
 
 
     def __duration(
         self,
-        delim: str = ' ',
+        delim: str = SPACED,
         short: bool = True,
     ) -> str:
         """
-        Return the compact format calculated from source duration.
+        Return the compact format determined by source duration.
 
         :param delim: Optional delimiter for between the groups.
         :param short: Determine if we should use the short hand.
-        :returns: Compact format calculated from source duration.
+        :returns: Compact format determined by source duration.
         """
 
         parts: list[str] = []
 
         groups = self.units(short)
-        spaced = '' if short else ' '
 
-        for part, value in groups.items():
+        space = (
+            SEMPTY if short
+            else SPACED)
+
+
+        items = groups.items()
+
+        for part, value in items:
 
             unit: str = part
 
             if (short is False
                     and value != 1):
                 unit += 's'
 
             parts.append(
-                f'{value}{spaced}{unit}')
+                f'{value}{space}{unit}')
+
 
         return delim.join(parts)
 
 
     @property
     def short(
         self,
     ) -> str:
         """
-        Return the compact format calculated from source duration.
+        Return the compact format determined by source duration.
 
-        :returns: Compact format calculated from source duration.
+        :returns: Compact format determined by source duration.
         """
 
         return self.__duration()
 
 
     @property
     def compact(
         self,
     ) -> str:
         """
-        Return the compact format calculated from source duration.
+        Return the compact format determined by source duration.
 
-        :returns: Compact format calculated from source duration.
+        :returns: Compact format determined by source duration.
         """
 
-        return self.short.replace(' ', '')
+        return self.short.replace(
+            SPACED, SEMPTY)
 
 
     @property
     def verbose(
         self,
     ) -> str:
         """
-        Return the verbose format calculated from source duration.
+        Return the verbose format determined by source duration.
 
-        :returns: Compact format calculated from source duration.
+        :returns: Verbose format determined by source duration.
         """
 
         if self.__source < 60:
             return 'just now'
 
-        return self.__duration(', ', False)
+        return self.__duration(
+            COMMAS, False)
```

### Comparing `encommon-0.7.6/encommon/times/parse.py` & `encommon-0.8.0/encommon/times/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from datetime import datetime
 from datetime import timezone
 from re import match as re_match
 from typing import Optional
 from typing import TYPE_CHECKING
 
 from dateutil import parser
-from dateutil.tz import gettz
 
 from snaptime import snap
 
 from .common import NUMERISH
 from .common import PARSABLE
 from .common import SNAPABLE
 from .common import STRINGNOW
+from .common import findtz
 from .common import strptime
 from .common import utcdatetime
 
 if TYPE_CHECKING:
     from .times import Times  # noqa: F401
 
 
@@ -83,22 +83,15 @@
             and hasattr(source, 'source')):
         source = source.source
 
     if (isinstance(source, str)
             and re_match(NUMERISH, source)):
         source = float(source)
 
-
-    if tzname is not None:
-        tzinfo = gettz(tzname)
-    else:
-        tzinfo = timezone.utc
-
-    if tzinfo is None:
-        raise ValueError('tzname')
+    tzinfo = findtz(tzname)
 
 
     if isinstance(source, (int, float)):
         source = datetime.fromtimestamp(
             float(source), tz=tzinfo)
 
     if str(source) in STRINGNOW:
@@ -125,15 +118,15 @@
 
     if isinstance(source, datetime):
         return (
             source.replace(tzinfo=tzinfo)
             .astimezone(timezone.utc))
 
 
-    raise ValueError('source')
+    raise ValueError('source')  # NOCVR
 
 
 
 def shift_time(
     notate: str,
     anchor: Optional[PARSABLE] = None,
     *,
@@ -155,21 +148,18 @@
     :param notate: Syntax compatable using snaptime library.
     :param anchor: Optional relative time; for snap notation.
     :param tzname: Name of the timezone associated to anchor.
         This is not relevant in timezone included in anchor.
     :returns: Python datetime object containing related time.
     """
 
-    anchor = parse_time(anchor, tzname=tzname)
-
-    parsed = snap(anchor, notate)
-
-    assert isinstance(parsed, datetime)
+    anchor = parse_time(
+        anchor, tzname=tzname)
 
-    return parsed
+    return snap(anchor, notate)
 
 
 
 def string_time(
     source: str,
     *,
     formats: Optional[str | list[str]] = None,
@@ -191,26 +181,22 @@
     :param source: Time in various forms that will be parsed.
     :param formats: Various formats compatable with strptime.
     :param tzname: Name of the timezone associated to source.
         This is not relevant in timezone included in source.
     :returns: Python datetime object containing related time.
     """
 
-    parsed: Optional[datetime] = None
-
     if formats is not None:
         with suppress(ValueError):
-            parsed = strptime(source, formats)
-
-    if parsed is None:
-        parsed = parser.parse(source)
+            return strptime(source, formats)
 
-    assert isinstance(parsed, datetime)
+    parsed = parser.parse(source)
 
-    return parse_time(parsed, tzname=tzname)
+    return parse_time(
+        parsed, tzname=tzname)
 
 
 
 def since_time(
     start: PARSABLE,
     stop: Optional[PARSABLE] = None,
 ) -> float:
@@ -230,8 +216,10 @@
     """
 
     start = parse_time(start)
     stop = parse_time(stop)
 
     delta = stop - start
 
-    return abs(delta.total_seconds())
+    since = delta.total_seconds()
+
+    return abs(since)
```

### Comparing `encommon-0.7.6/encommon/times/test/test_parse.py` & `encommon-0.8.0/encommon/times/test/test_parse.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,108 +6,89 @@
 """
 
 
 
 from datetime import timedelta
 
 from pytest import mark
-from pytest import raises
 
 from ..common import utcdatetime
 from ..parse import parse_time
 from ..parse import shift_time
 from ..parse import since_time
 from ..parse import string_time
 
 
 
 def test_parse_time() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
-    utcnow = utcdatetime()
+    dtime = utcdatetime()
     delta = timedelta(seconds=1)
 
 
-    dtime = parse_time(
+    parsed = parse_time(
         '1/1/1970 6:00am')
 
-    assert dtime.year == 1970
-    assert dtime.month == 1
-    assert dtime.day == 1
-    assert dtime.hour == 6
+    assert parsed.year == 1970
+    assert parsed.month == 1
+    assert parsed.day == 1
+    assert parsed.hour == 6
 
 
-    dtime = parse_time(
+    parsed = parse_time(
         '12/31/1969 6:00pm',
         tzname='US/Central')
 
-    assert dtime.year == 1970
-    assert dtime.month == 1
-    assert dtime.day == 1
-    assert dtime.hour == 0
+    assert parsed.year == 1970
+    assert parsed.month == 1
+    assert parsed.day == 1
+    assert parsed.hour == 0
 
 
-    dtime = parse_time(0)
-    assert dtime.year == 1970
+    parsed = parse_time(0)
+    assert parsed.year == 1970
 
-    dtime = parse_time('0')
-    assert dtime.year == 1970
+    parsed = parse_time('0')
+    assert parsed.year == 1970
 
 
-    dtime = parse_time('max')
+    parsed = parse_time('max')
 
-    assert dtime.year == 9999
-    assert dtime.month == 12
-    assert dtime.day == 31
-    assert dtime.hour == 23
+    assert parsed.year == 9999
+    assert parsed.month == 12
+    assert parsed.day == 31
+    assert parsed.hour == 23
 
-    dtime = parse_time('min')
+    parsed = parse_time('min')
 
-    assert dtime.year == 1
-    assert dtime.month == 1
-    assert dtime.day == 1
-    assert dtime.hour == 0
+    assert parsed.year == 1
+    assert parsed.month == 1
+    assert parsed.day == 1
+    assert parsed.hour == 0
 
 
-    dtime = parse_time('now')
-    assert dtime - utcnow <= delta
+    parsed = parse_time('now')
+    assert parsed - dtime <= delta
 
-    dtime = parse_time(None)
-    assert dtime - utcnow <= delta
+    parsed = parse_time(None)
+    assert parsed - dtime <= delta
 
-    dtime = parse_time('None')
-    assert dtime - utcnow <= delta
+    parsed = parse_time('None')
+    assert parsed - dtime <= delta
 
 
-    dtime = parse_time('+1y')
-    assert dtime - utcnow > delta
+    parsed = parse_time('+1y')
+    assert parsed - dtime > delta
 
 
-    assert parse_time(dtime) == dtime
-
-
-
-def test_parse_time_raises() -> None:
-    """
-    Perform various tests associated with relevant routines.
-    """
-
-
-    with raises(ValueError) as reason:
-        parse_time(0, tzname='foo/bar')
-
-    assert str(reason.value) == 'tzname'
-
-
-    with raises(ValueError) as reason:
-        parse_time(parse_time)  # type: ignore
-
-    assert str(reason.value) == 'source'
+    _parsed = parse_time(parsed)
+    assert _parsed == parsed
 
 
 
 @mark.parametrize(
     'notate,expect',
     [('+1y', (1981, 1, 1)),
      ('-1y', (1979, 1, 1)),
@@ -141,68 +122,77 @@
     Perform various tests associated with relevant routines.
 
     :param notate: Syntax compatable using snaptime library.
     :param expect: Expected output from the testing routine.
     """
 
     anchor = utcdatetime(1980, 1, 1)
+    dtime = utcdatetime(*expect)
 
     parsed = shift_time(notate, anchor)
 
-    assert parsed == utcdatetime(*expect)
+    assert parsed == dtime
 
 
 
 def test_string_time() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
     expect = utcdatetime(1980, 1, 1)
 
 
     strings = [
         '1980-01-01T00:00:00Z',
+        '1980-01-01T00:00:00 +0000',
         '1980-01-01T00:00:00',
         '1980-01-01 00:00:00 +0000',
         '1980-01-01 00:00:00']
 
     for string in strings:
-        assert string_time(string) == expect
+
+        parsed = string_time(string)
+
+        assert parsed == expect
 
 
     parsed = string_time(
         '1980_01_01',
-        formats=['%Y', '%Y_%m_%d'])
+        formats=['%Y_%m_%d'])
 
     assert parsed == expect
 
+
     parsed = string_time(
         '1980_01_01',
         formats='%Y_%m_%d')
 
     assert parsed == expect
 
+
     parsed = string_time(
         '1979-12-31 18:00:00',
         tzname='US/Central')
 
     assert parsed == expect
 
 
 
 def test_since_time() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
 
-    dtime = shift_time('-1s')
+    parsed = shift_time('-1s')
+    since = since_time(parsed)
 
-    assert since_time(dtime) >= 1
-    assert since_time(dtime) < 2
+    assert since >= 1
+    assert since < 2
 
 
-    dtime = shift_time('+1s')
+    parsed = shift_time('+1s')
+    since = since_time(parsed)
 
-    assert since_time(dtime) > 0
-    assert since_time(dtime) < 2
+    assert since > 0
+    assert since < 2
```

### Comparing `encommon-0.7.6/encommon/times/test/test_timers.py` & `encommon-0.8.0/encommon/times/test/test_timers.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,114 +6,168 @@
 """
 
 
 
 from pathlib import Path
 from time import sleep
 
+from pytest import fixture
 from pytest import raises
 
 from ..timers import Timers
 
 
 
-def test_Timers() -> None:
+@fixture
+def timers(
+    tmp_path: Path,
+) -> Timers:
+    """
+    Construct the instance for use in the downstream tests.
+
+    :param tmp_path: pytest object for temporal filesystem.
+    :returns: Newly constructed instance of related class.
+    """
+
+    return Timers(
+        timers={'one': 1},
+        file=f'{tmp_path}/cache.db')
+
+
+
+def test_Timers(
+    timers: Timers,
+) -> None:
     """
     Perform various tests associated with relevant routines.
+
+    :param timers: Primary class instance for timers object.
     """
 
-    timers = Timers({'one': 1})
 
     attrs = list(timers.__dict__)
 
     assert attrs == [
-        '_Timers__timers',
-        '_Timers__cache_file',
-        '_Timers__cache_name',
-        '_Timers__cache_dict']
+        '_Timers__config',
+        '_Timers__sqlite',
+        '_Timers__file',
+        '_Timers__table',
+        '_Timers__cache']
+
+
+    assert repr(timers)[:22] == (
+        '<encommon.times.timers')
 
+    assert hash(timers) > 0
 
-    assert repr(timers).startswith(
-        '<encommon.times.timers.Timers')
-    assert isinstance(hash(timers), int)
-    assert str(timers).startswith(
-        '<encommon.times.timers.Timers')
+    assert str(timers)[:22] == (
+        '<encommon.times.timers')
 
 
     assert timers.timers == {'one': 1}
-    assert timers.cache_file is not None
-    assert len(timers.cache_dict) == 1
-    assert timers.cache_name is not None
+
+    assert timers.sqlite is not None
+
+    assert timers.file[-8:] == 'cache.db'
+
+    assert timers.table == 'timers'
+
+    assert list(timers.cache) == ['one']
+
+
+
+def test_Timers_cover(
+    timers: Timers,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param timers: Primary class instance for timers object.
+    """
 
 
     assert not timers.ready('one')
+
     sleep(1.1)
+
     assert timers.ready('one')
 
 
     timers.create('two', 2, 0)
 
     assert timers.ready('two')
+
     assert not timers.ready('two')
 
 
 
 def test_Timers_cache(
-    tmp_path: Path,
+    timers: Timers,
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
-    :param tmp_path: pytest object for temporal filesystem.
+    :param timers: Primary class instance for timers object.
     """
 
-    cache_file = (
-        f'{tmp_path}/timers.db')
-
     timers1 = Timers(
-        timers={'one': 1},
-        cache_file=cache_file)
+        timers={'uno': 1},
+        file=timers.file)
 
-    assert not timers1.ready('one')
+    assert not timers1.ready('uno')
 
     sleep(0.75)
 
     timers2 = Timers(
-        timers={'one': 1},
-        cache_file=cache_file)
+        timers={'uno': 1},
+        file=timers.file)
 
-    assert not timers1.ready('one')
-    assert not timers2.ready('one')
+    assert not timers1.ready('uno')
+    assert not timers2.ready('uno')
 
     sleep(0.25)
 
     timers2.load_cache()
 
-    assert timers1.ready('one')
-    assert timers2.ready('one')
+    assert timers1.ready('uno')
+    assert timers2.ready('uno')
 
 
 
-def test_Timers_raises() -> None:
+def test_Timers_raises(
+    timers: Timers,
+) -> None:
     """
     Perform various tests associated with relevant routines.
+
+    :param timers: Primary class instance for timers object.
     """
 
-    timers = Timers({'one': 1})
 
+    _raises = raises(ValueError)
 
-    with raises(ValueError) as reason:
+    with _raises as reason:
         timers.ready('dne')
 
-    assert str(reason.value) == 'unique'
+    _reason = str(reason.value)
 
+    assert _reason == 'unique'
 
-    with raises(ValueError) as reason:
+
+    _raises = raises(ValueError)
+
+    with _raises as reason:
         timers.update('dne')
 
-    assert str(reason.value) == 'unique'
+    _reason = str(reason.value)
+
+    assert _reason == 'unique'
 
 
-    with raises(ValueError) as reason:
+    _raises = raises(ValueError)
+
+    with _raises as reason:
         timers.create('one', 1)
 
-    assert str(reason.value) == 'unique'
+    _reason = str(reason.value)
+
+    assert _reason == 'unique'
```

### Comparing `encommon-0.7.6/encommon/times/test/test_window.py` & `encommon-0.8.0/encommon/times/test/test_window.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,98 +3,150 @@
 
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
+from typing import TYPE_CHECKING
+
+from pytest import fixture
 from pytest import mark
 
-from ..common import PARSABLE
 from ..window import Window
 from ..window import window_croniter
 from ..window import window_interval
 
+if TYPE_CHECKING:
+    from ..common import PARSABLE
+
+
+
+@fixture
+def window() -> Window:
+    """
+    Construct the instance for use in the downstream tests.
+
+    :returns: Newly constructed instance of related class.
+    """
+
+    return Window(
+        schedule='* * * * *',
+        start=330, stop=630)
 
 
-def test_Window() -> None:
+
+def test_Window(
+    window: Window,
+) -> None:
     """
     Perform various tests associated with relevant routines.
+
+    :param window: Primary class instance for window object.
     """
 
-    window = Window('* * * * *', 330, 630)
 
     attrs = list(window.__dict__)
 
     assert attrs == [
         '_Window__schedule',
         '_Window__start',
         '_Window__stop',
         '_Window__anchor',
         '_Window__delay',
         '_Window__wilast',
         '_Window__winext',
         '_Window__walked']
 
 
-    assert repr(window).startswith(
-        '<encommon.times.window.Window')
-    assert isinstance(hash(window), int)
-    assert str(window).startswith(
-        '<encommon.times.window.Window')
+    assert repr(window)[:22] == (
+        '<encommon.times.window')
+
+    assert hash(window) > 0
+
+    assert str(window)[:22] == (
+        '<encommon.times.window')
 
 
     assert window.schedule == '* * * * *'
+
     assert window.start == '1970-01-01T00:05:30Z'
+
     assert window.stop == '1970-01-01T00:10:30Z'
+
     assert window.anchor == window.start
+
     assert window.delay == 0.0
+
     assert window.last == '1970-01-01T00:05:00Z'
+
     assert window.next == '1970-01-01T00:06:00Z'
+
     assert window.walked is False
 
 
+
+def test_Window_cover(
+    window: Window,
+) -> None:
+    """
+    Perform various tests associated with relevant routines.
+
+    :param window: Primary class instance for window object.
+    """
+
+
+    window = Window(
+        schedule='* * * * *',
+        start=window.start,
+        stop=window.stop)
+
+    assert window.last == '1970-01-01T00:05:00Z'
+    assert window.next == '1970-01-01T00:06:00Z'
+    assert window.walked is False
+
     for count in range(100):
         if window.walk() is False:
             break
         assert window.walk(False)
 
     assert count == 4
     assert not window.walk()
 
     assert window.last == '1970-01-01T00:10:00Z'
     assert window.next == '1970-01-01T00:10:00Z'
     assert window.walked is True
 
 
-    window = Window({'minutes': 1}, 300, 600)
+    window = Window(
+        schedule={'minutes': 1},
+        start=window.start,
+        stop=window.stop)
 
-    assert window.schedule == {'minutes': 1}
-    assert window.start == '1970-01-01T00:05:00Z'
-    assert window.stop == '1970-01-01T00:10:00Z'
-    assert window.anchor == window.start
-    assert window.delay == 0.0
-    assert window.last == '1970-01-01T00:04:00Z'
-    assert window.next == '1970-01-01T00:05:00Z'
+    assert window.last == '1970-01-01T00:04:30Z'
+    assert window.next == '1970-01-01T00:05:30Z'
     assert window.walked is False
 
     for count in range(100):
         if window.walk() is False:
             break
         assert window.walk(False)
 
     assert count == 5
     assert not window.walk()
 
-    assert window.last == '1970-01-01T00:10:00Z'
-    assert window.next == '1970-01-01T00:10:00Z'
+    assert window.last == '1970-01-01T00:10:30Z'
+    assert window.next == '1970-01-01T00:10:30Z'
     assert window.walked is True
 
 
-    window = Window('* * * * *', '+5m', '+10m')
+    window = Window(
+        schedule='* * * * *',
+        start='+5m', stop='+10m')
+
     assert not window.walk(False)
 
 
 
 @mark.parametrize(
     'schedule,anchor,backward,expect',
     [('* * * * *', 0, False, (0, 60)),
@@ -106,15 +158,15 @@
      ('* * * * *', 3660, False, (3660, 3720)),
      ('* * * * *', 3661, False, (3660, 3720)),
      ('0 * * * *', 3559, False, (0, 3600)),
      ('0 * * * *', 3660, False, (3600, 7200)),
      ('0 * * * *', 3661, False, (3600, 7200))])
 def test_window_croniter(
     schedule: str,
-    anchor: PARSABLE,
+    anchor: 'PARSABLE',
     backward: bool,
     expect: tuple[int, int],
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param schedule: Parameters for defining scheduled time.
@@ -142,15 +194,15 @@
      ({'seconds': 60}, 3660, False, (3660, 3720)),
      ({'seconds': 60}, 3661, False, (3661, 3721)),
      ({'hours': 1}, 3559, False, (3559, 7159)),
      ({'hours': 1}, 3660, False, (3660, 7260)),
      ({'hours': 1}, 3661, False, (3661, 7261))])
 def test_window_interval(
     schedule: dict[str, int],
-    anchor: PARSABLE,
+    anchor: 'PARSABLE',
     backward: bool,
     expect: tuple[int, int],
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param schedule: Parameters for defining scheduled time.
```

### Comparing `encommon-0.7.6/encommon/times/timers.py` & `encommon-0.8.0/encommon/times/timers.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,26 +16,30 @@
 from .times import Times
 
 if TYPE_CHECKING:
     from sqlite3 import Connection
 
 
 
-TABLE = (
+CACHE_TABLE = (
     """
-    create table
-     if not exists
+    create table if not exists
      {0} (
       "unique" text not null,
       "update" text not null,
      primary key ("unique"));
     """)  # noqa: LIT003
 
 
 
+_TIMERS = dict[str, float]
+_CACHED = dict[str, Times]
+
+
+
 class Timers:
     """
     Track timers on unique key and determine when to proceed.
 
     .. warning::
        This class will use an in-memory database for cache,
        unless a cache file is explicity defined.
@@ -49,75 +53,81 @@
     >>> timers.ready('one')
     False
     >>> sleep(1)
     >>> timers.ready('one')
     True
 
     :param timers: Seconds that are used for each of timers.
-    :param cache_file: Optional path to SQLite database for
+    :param file: Optional path to SQLite database for
         cache. This will allow for use between executions.
-    :param cache_name: Optional override default table name.
+    :param table: Optional override default table name.
     """
 
-    __timers: dict[str, float]
-    __cache_file: 'Connection'
-    __cache_name: str
-    __cache_dict: dict[str, Times]
+    __config: _TIMERS
+    __sqlite: 'Connection'
+    __file: str
+    __table: str
+    __cache: _CACHED
 
 
     def __init__(
         self,
         timers: Optional[dict[str, NUMERIC]] = None,
-        cache_file: str = ':memory:',
-        cache_name: str = 'encommon_timers',
+        file: str = ':memory:',
+        table: str = 'timers',
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
-        timers = timers or {}
 
+        timers = dict(timers or {})
 
-        self.__timers = {
-            k: float(v)
-            for k, v in
-            timers.items()}
+        items = timers.items()
 
+        for key, value in items:
+            timers[key] = float(value)
 
-        cached = SQLite(cache_file)
 
-        cached.execute(
-            TABLE.format(cache_name))
+        sqlite = SQLite(file)
 
-        cached.commit()
+        sqlite.execute(
+            CACHE_TABLE
+            .format(table))
+
+        sqlite.commit()
+
+
+        cached: _CACHED = {}
 
-        self.__cache_file = cached
-        self.__cache_name = cache_name
+        for timer in timers:
+            cached[timer] = Times()
 
 
-        self.__cache_dict = {
-            x: Times()
-            for x in
-            self.__timers}
+        self.__config = timers
+        self.__sqlite = sqlite
+        self.__file = file
+        self.__table = table
+        self.__cache = cached
 
 
         self.load_cache()
         self.save_cache()
 
 
     def load_cache(
         self,
     ) -> None:
         """
         Load the timers cache from the database into attribute.
         """
 
-        cached = self.__cache_file
-        table = self.__cache_name
-        cachem = self.__cache_dict
+        cached = self.__sqlite
+        table = self.__table
+        cachem = self.__cache
 
         cursor = cached.execute(
             f'select * from {table}'
             ' order by "unique" asc')
 
         records = cursor.fetchall()
 
@@ -134,107 +144,130 @@
     def save_cache(
         self,
     ) -> None:
         """
         Save the timers cache from the attribute into database.
         """
 
-        cached = self.__cache_file
-        table = self.__cache_name
-        cachem = self.__cache_dict
-
-        insert = [
-            (k, str(v)) for k, v
-            in cachem.items()]
+        insert = tuple[str, str]
+        inserts: list[insert] = []
+
+
+        cached = self.__sqlite
+        table = self.__table
+        cachem = self.__cache
+
+
+        items = cachem.items()
+
+        for key, value in items:
+
+            append = (key, str(value))
+
+            inserts.append(append)
+
 
         cached.executemany(
             (f'replace into {table}'
              ' ("unique", "update")'
              ' values (?, ?)'),
-            tuple(insert))
+            tuple(sorted(inserts)))
 
         cached.commit()
 
 
     @property
     def timers(
         self,
-    ) -> dict[str, float]:
+    ) -> _TIMERS:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return dict(self.__timers)
+        return dict(self.__config)
 
 
     @property
-    def cache_file(
+    def sqlite(
         self,
     ) -> 'Connection':
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return self.__cache_file
+        return self.__sqlite
 
 
     @property
-    def cache_dict(
+    def file(
         self,
-    ) -> dict[str, Times]:
+    ) -> str:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return dict(self.__cache_dict)
+        return self.__file
 
 
     @property
-    def cache_name(
+    def table(
         self,
     ) -> str:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return self.__cache_name
+        return self.__table
+
+
+    @property
+    def cache(
+        self,
+    ) -> _CACHED:
+        """
+        Return the value for the attribute from class instance.
+
+        :returns: Value for the attribute from class instance.
+        """
+
+        return dict(self.__cache)
 
 
     def ready(
         self,
         unique: str,
         update: bool = True,
     ) -> bool:
         """
         Determine whether or not the appropriate time has passed.
 
         .. note::
            For performance reasons, this method will not notice
            changes within the database unless refreshed first.
 
-        :param unique: Unique identifier for the timer in mapping.
+        :param unique: Which timer configuration from reference.
         :param update: Determines whether or not time is updated.
         """
 
-        timers = self.__timers
-        caches = self.__cache_dict
+        config = self.__config
+        caches = self.__cache
 
         if unique not in caches:
             raise ValueError('unique')
 
         cache = caches[unique]
-        timer = timers[unique]
+        timer = config[unique]
 
         ready = cache.since >= timer
 
         if ready and update:
             self.update(unique)
 
         return ready
@@ -244,19 +277,19 @@
         self,
         unique: str,
         started: Optional[PARSABLE] = None,
     ) -> None:
         """
         Update the existing timer from mapping within the cache.
 
-        :param unique: Unique identifier for the timer in mapping.
+        :param unique: Which timer configuration from reference.
         :param started: Override the start time for timer value.
         """
 
-        caches = self.__cache_dict
+        caches = self.__cache
 
         if unique not in caches:
             raise ValueError('unique')
 
         caches[unique] = Times(started)
 
         self.save_cache()
@@ -267,22 +300,22 @@
         unique: str,
         minimum: int | float,
         started: Optional[PARSABLE] = None,
     ) -> None:
         """
         Update the existing timer from mapping within the cache.
 
-        :param unique: Unique identifier for the timer in mapping.
-        :param minimum: Determines minimum seconds that must pass.
-        :param started: Determines when the time starts for timer.
+        :param unique: Which timer configuration from reference.
+        :param minimum: Determine minimum seconds that must pass.
+        :param started: Determine when time starts for the timer.
         """
 
-        timers = self.__timers
-        caches = self.__cache_dict
+        config = self.__config
+        caches = self.__cache
 
-        if unique in timers:
+        if unique in config:
             raise ValueError('unique')
 
-        timers[unique] = float(minimum)
+        config[unique] = float(minimum)
         caches[unique] = Times(started)
 
         self.save_cache()
```

### Comparing `encommon-0.7.6/encommon/times/times.py` & `encommon-0.8.0/encommon/times/times.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
+from contextlib import suppress
 from datetime import datetime
 from datetime import timedelta
-from datetime import timezone
 from typing import Optional
 
-from dateutil.tz import gettz
-
 from .common import PARSABLE
 from .common import STAMP_HUMAN
 from .common import STAMP_SIMPLE
 from .common import STAMP_SUBSEC
+from .common import findtz
+from .common import strftime
 from .parse import parse_time
 from .parse import since_time
 
 
 
 class Times:
     """
@@ -36,34 +36,39 @@
     :param anchor: Optional relative time; for snap notation.
     :param format: Optional format when source is timestamp.
     :param tzname: Name of the timezone associated to source.
         This is not relevant in timezone included in source.
     """
 
     __source: datetime
+    __hashed: int
 
 
     def __init__(
         self,
         source: Optional[PARSABLE] = None,
         *,
         anchor: Optional[PARSABLE] = None,
         format: str = STAMP_SUBSEC,
         tzname: Optional[str] = None,
     ) -> None:
         """
         Initialize instance for class using provided parameters.
         """
 
-        self.__source = parse_time(
+        parsed = parse_time(
             source=source,
             anchor=anchor,
             format=format,
             tzname=tzname)
 
+        self.__source = parsed
+        self.__hashed = int(
+            self.mpoch * 1000)
+
 
     def __repr__(
         self,
     ) -> str:
         """
         Built-in method for representing the values for instance.
 
@@ -78,15 +83,15 @@
     ) -> int:
         """
         Built-in method called when performing hashing operation.
 
         :returns: Boolean indicating outcome from the operation.
         """
 
-        return int(self.mpoch * 100000)
+        return int(1e9 + self.__hashed)
 
 
     def __str__(
         self,
     ) -> str:
         """
         Built-in method for representing the values for instance.
@@ -99,27 +104,27 @@
 
     def __int__(
         self,
     ) -> int:
         """
         Built-in method representing numeric value for instance.
 
-        :returns: Numeric representation for values from instance.
+        :returns: Numeric representation for value in instance.
         """
 
         return int(self.epoch)
 
 
     def __float__(
         self,
     ) -> float:
         """
         Built-in method representing numeric value for instance.
 
-        :returns: Numeric representation for values from instance.
+        :returns: Numeric representation for value in instance.
         """
 
         return float(self.epoch)
 
 
     def __add__(
         self,
@@ -164,21 +169,24 @@
         """
         Built-in method for comparing this instance with another.
 
         :param other: Other value being compared with instance.
         :returns: Boolean indicating outcome from the operation.
         """
 
-        try:
-            parsed = parse_time(other)  # type: ignore
+        source = self.__source
+
+        with suppress(Exception):
 
-        except Exception:
-            return False
+            parsed = parse_time(
+                other)  # type: ignore
 
-        return self.__source == parsed
+            return source == parsed
+
+        return False
 
 
     def __ne__(
         self,
         other: object,
     ) -> bool:
         """
@@ -274,15 +282,17 @@
     ) -> float:
         """
         Return the seconds since the Unix epoch for the instance.
 
         :returns: Seconds since the Unix epoch for the instance.
         """
 
-        return self.__source.timestamp()
+        source = self.__source
+
+        return source.timestamp()
 
 
     @property
     def mpoch(
         self,
     ) -> float:
         """
@@ -365,36 +375,36 @@
     ) -> 'Times':
         """
         Return new object containing time just before the time.
 
         :returns: Object containing time just before the time.
         """
 
-        delta = timedelta(
-            microseconds=1)
+        source = self.__source
 
-        source = self.__source - delta
+        source -= timedelta(
+            microseconds=1)
 
         return Times(source)
 
 
     @property
     def after(
         self,
     ) -> 'Times':
         """
         Return new object containing time just after the time.
 
         :returns: Object containing time just after the time.
         """
 
-        delta = timedelta(
-            microseconds=1)
+        source = self.__source
 
-        source = self.__source + delta
+        source += timedelta(
+            microseconds=1)
 
         return Times(source)
 
 
     def stamp(
         self,
         format: str = STAMP_SUBSEC,
@@ -405,38 +415,30 @@
 
         :param format: Optional format when source is timestamp.
         :param tzname: Name of the timezone associated to source.
             This is not relevant in timezone included in source.
         :returns: Timestamp using provided format for instance.
         """
 
-        parsed = self.__source
+        source = self.__source
 
+        tzinfo = findtz(tzname)
 
-        if tzname is not None:
-            tzinfo = gettz(tzname)
-        else:
-            tzinfo = timezone.utc
+        parsed = source.astimezone(tzinfo)
 
-        if tzinfo is None:
-            raise ValueError('tzname')
-
-
-        return datetime.strftime(
-            parsed.astimezone(tzinfo),
-            format)
+        return strftime(parsed, format)
 
 
     def shift(
         self,
         notate: str,
     ) -> 'Times':
         """
         Return the new instance of object shifted using snaptime.
 
         :param notate: Syntax compatable using snaptime library.
         :returns: New instance of the class using shifted time.
         """
 
-        return Times(
-            source=notate,
-            anchor=self.__source)
+        source = self.__source
+
+        return Times(notate, anchor=source)
```

### Comparing `encommon-0.7.6/encommon/times/window.py` & `encommon-0.8.0/encommon/times/window.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -166,37 +166,37 @@
         :returns: Value for the attribute from class instance.
         """
 
         return self.__delay
 
 
     @property
-    def next(
+    def last(
         self,
     ) -> Times:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return Times(self.__winext)
+        return Times(self.__wilast)
 
 
     @property
-    def last(
+    def next(
         self,
     ) -> Times:
         """
         Return the value for the attribute from class instance.
 
         :returns: Value for the attribute from class instance.
         """
 
-        return Times(self.__wilast)
+        return Times(self.__winext)
 
 
     @property
     def walked(
         self,
     ) -> bool:
         """
```

### Comparing `encommon-0.7.6/encommon/types/dicts.py` & `encommon-0.8.0/encommon/types/dicts.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,20 +45,24 @@
 
         if key not in dict1:
             dict1[key] = value
 
         elif (isinstance(dict1[key], list)
                 and isinstance(value, list)
                 and merge_list is True):
-            dict1[key] = [] + dict1[key] + value
+
+            dict1[key] = (
+                [] + dict1[key] + value)
 
         elif (isinstance(dict1[key], dict)
                 and isinstance(value, dict)
                 and merge_dict is True):
-            merge_dicts(dict1[key], value, force)
+
+            merge_dicts(
+                dict1[key], value, force)
 
         elif force is True:
             dict1[key] = value
 
 
 
 def sort_dict(
@@ -77,10 +81,12 @@
     {'b': 'be', 'a': 'ey'}
 
     :param value: Dictionary whose keys are sorted into new.
     :param reverse: Optionally reverse the sort direction.
     :returns: New dictionary with keys sorted alphabetical.
     """
 
-    return dict(sorted(
+    items = sorted(
         value.items(),
-        reverse=reverse))
+        reverse=reverse)
+
+    return dict(items)
```

### Comparing `encommon-0.7.6/encommon/types/empty.py` & `encommon-0.8.0/encommon/types/empty.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,16 +47,21 @@
     ) -> 'EmptyType':
         """
         Built-in method called when creating new class instance.
 
         :returns: Same instance of class that first instantiated.
         """
 
-        if cls.__empty is None:
-            cls.__empty = object.__new__(cls)
+        empty = cls.__empty
+
+        if empty is not None:
+            return empty
+
+        cls.__empty = (
+            object.__new__(cls))
 
         return cls.__empty
 
 
     def __repr__(
         self,
     ) -> str:
```

### Comparing `encommon-0.7.6/encommon/types/test/test_dicts.py` & `encommon-0.8.0/encommon/types/test/test_dicts.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,37 +10,37 @@
 from copy import deepcopy
 
 from ..dicts import merge_dicts
 from ..dicts import sort_dict
 
 
 
-DICT1 = {
+_DICT1 = {
     'dict1': 'dict1',
     'str': 'd1string',
     'list': ['d1list'],
     'dict': {'key': 'd1value'},
     'bool': False}
 
-DICT2 = {
+_DICT2 = {
     'dict2': 'dict2',
     'str': 'd2string',
     'list': ['d2list'],
     'dict': {'key': 'd2value'},
     'bool': True}
 
 
 
 def test_merge_dicts() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
-    dict1 = deepcopy(DICT1)
-    dict2 = deepcopy(DICT2)
+    dict1 = deepcopy(_DICT1)
+    dict2 = deepcopy(_DICT2)
 
     dict1['recurse'] = deepcopy(dict1)
     dict2['recurse'] = deepcopy(dict2)
 
 
     source = deepcopy(dict1)
     update = deepcopy(dict2)
@@ -110,13 +110,13 @@
 
 
 def test_sort_dict() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
-    assert sort_dict(DICT1) == {
+    assert sort_dict(_DICT1) == {
         'bool': False,
         'dict': {'key': 'd1value'},
         'dict1': 'dict1',
         'list': ['d1list'],
         'str': 'd1string'}
```

### Comparing `encommon-0.7.6/encommon/types/test/test_empty.py` & `encommon-0.8.0/encommon/types/test/test_empty.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,23 +18,26 @@
 def test_EmptyType() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
     empty = EmptyType()
 
+
     attrs = list(empty.__dict__)
 
     assert attrs == [
         '_EmptyType__empty']
 
+
     assert repr(empty) == 'Empty'
-    assert isinstance(hash(empty), int)
+    assert hash(empty) > 0
     assert str(empty) == 'Empty'
 
+
     assert not (Empty or None)
     assert Empty is empty
     assert Empty is Empty
     assert Empty is EmptyType()
     assert Empty == empty
     assert Empty == Empty
     assert Empty == EmptyType()
```

### Comparing `encommon-0.7.6/encommon/utils/__init__.py` & `encommon-0.8.0/encommon/utils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 This file is part of Enasis Network software eco-system. Distribution
 is permitted, for more information consult the project license file.
 """
 
 
 
+from .common import read_text
+from .common import save_text
 from .match import fuzz_match
 from .match import rgxp_match
 from .paths import resolve_path
 from .paths import resolve_paths
 from .paths import stats_path
 from .sample import load_sample
 from .sample import prep_sample
@@ -26,12 +28,14 @@
     'array_ansi',
     'fuzz_match',
     'kvpair_ansi',
     'load_sample',
     'make_ansi',
     'prep_sample',
     'print_ansi',
+    'read_text',
     'resolve_path',
     'resolve_paths',
     'rgxp_match',
+    'save_text',
     'stats_path',
     'strip_ansi']
```

### Comparing `encommon-0.7.6/encommon/utils/match.py` & `encommon-0.8.0/encommon/utils/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
     function = (
         re_fmatch if complete
         else re_match)
 
 
     def _matches() -> bool:
+
         return bool(
             function(pattern, value))
 
 
     for value in values:
 
         matched = False
```

### Comparing `encommon-0.7.6/encommon/utils/paths.py` & `encommon-0.8.0/encommon/utils/paths.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,124 +6,142 @@
 """
 
 
 
 from os import stat_result
 from pathlib import Path
 from typing import Optional
+from typing import TYPE_CHECKING
 
-from .common import PATHABLE
 from .match import rgxp_match
+from ..types import sort_dict
 
+if TYPE_CHECKING:
+    from .common import PATHABLE
+    from .common import REPLACE
 
 
-_REPLACE = dict[str, str]
+
+STATS_PATH = dict[str, stat_result]
 
 
 
 def resolve_path(
     path: str | Path,
-    replace: Optional[_REPLACE] = None,
+    replace: Optional['REPLACE'] = None,
 ) -> Path:
     """
-    Resolve the provided path and replace the magic keywords.
+    Resolve the provided path replacing the magic keywords.
 
     Example
     -------
     >>> resolve_path('/foo/bar')
     PosixPath('/foo/bar')
 
     :param path: Complete or relative path for processing.
-    :param replace: Optional string values to replace in path.
+    :param replace: Optional values to replace in the path.
     :returns: New resolved filesystem path object instance.
     """
 
     path = str(path).strip()
 
     if replace is not None:
-        for old, new in replace.items():
+
+        items = replace.items()
+
+        for old, new in items:
+
+            if isinstance(old, Path):
+                old = str(old)
+
+            if isinstance(new, Path):
+                new = str(new)
+
             path = path.replace(old, new)
 
     return Path(path).resolve()
 
 
 
 def resolve_paths(
-    paths: PATHABLE,
-    replace: Optional[_REPLACE] = None,
+    paths: 'PATHABLE',
+    replace: Optional['REPLACE'] = None,
 ) -> tuple[Path, ...]:
     """
-    Resolve the provided paths and replace the magic keywords.
+    Resolve the provided paths replacing the magic keywords.
 
     .. note::
        This will remove duplicative paths from the returned.
 
     Example
     -------
     >>> resolve_paths(['/foo/bar'])
     (PosixPath('/foo/bar'),)
 
     :param paths: Complete or relative paths for processing.
-    :param replace: Optional string values to replace in path.
+    :param replace: Optional values to replace in the path.
     :returns: New resolved filesystem path object instances.
     """
 
     returned: list[Path] = []
 
     if isinstance(paths, str | Path):
         paths = [paths]
 
     for path in paths:
 
-        _path = resolve_path(
-            str(path), replace)
+        resolved = resolve_path(
+            path, replace)
 
-        if _path in returned:
+        if resolved in returned:
             continue
 
-        returned.append(_path)
+        returned.append(resolved)
 
     return tuple(returned)
 
 
 
 def stats_path(
     path: str | Path,
-    replace: Optional[_REPLACE] = None,
+    replace: Optional['REPLACE'] = None,
     ignore: Optional[list[str]] = None,
-) -> dict[str, stat_result]:
+) -> STATS_PATH:
     """
     Collect stats object for the complete or relative path.
 
     .. testsetup::
+       >>> from . import save_text
        >>> path = Path(getfixture('tmpdir'))
        >>> file = path.joinpath('hello.txt')
-       >>> file.write_text('Hello world!')
-       12
+       >>> save_text(file, 'Hello world!')
+       'Hello world!'
 
     Example
     -------
     >>> replace = {str(path): '/'}
     >>> stats = stats_path(path, replace)
     >>> stats['/hello.txt'].st_size
     12
 
     :param path: Complete or relative path for enumeration.
-    :param replace: Optional string values to replace in path.
+    :param replace: Optional values to replace in the path.
     :param ignore: Paths matching these patterns are ignored.
     :returns: Metadata for files recursively found in path.
     """
 
     path = Path(path).resolve()
 
-    returned: dict[str, stat_result] = {}
+    returned: STATS_PATH = {}
 
 
     def _ignore() -> bool:
+
         assert ignore is not None
+
         return rgxp_match(
             str(item), ignore)
 
 
     for item in path.iterdir():
 
         if ignore and _ignore():
@@ -137,12 +155,13 @@
             returned.update(meta)
 
         elif item.is_file():
 
             key = resolve_path(
                 item, replace)
 
-            returned[str(key)] = (
-                item.stat())
+            stat = item.stat()
+
+            returned[str(key)] = stat
 
 
-    return dict(sorted(returned.items()))
+    return sort_dict(returned)
```

### Comparing `encommon-0.7.6/encommon/utils/sample.py` & `encommon-0.8.0/encommon/utils/sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,33 +9,29 @@
 
 from json import dumps
 from json import loads
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Optional
-from typing import Union
+from typing import TYPE_CHECKING
 
-from .. import PROJECT
-from .. import WORKSPACE
+from . import read_text
+from . import save_text
 
-
-
-_REPLACE = Union[
-    dict[str, str],
-    dict[str, str | Path],
-    dict[str, Path]]
+if TYPE_CHECKING:
+    from .common import REPLACE
 
 
 
 def prep_sample(
     content: Any,
     *,
     default: Callable[[Any], str] = str,
-    replace: Optional[_REPLACE] = None,
+    replace: Optional['REPLACE'] = None,
 ) -> Any:
     """
     Return the content after processing using JSON functions.
 
     .. testsetup::
        >>> from ..types import Empty
 
@@ -45,50 +41,51 @@
     ['one', 'two']
 
     Example
     -------
     >>> prep_sample({'one': Empty})
     {'one': 'Empty'}
 
-    :param content: Content which will be processed for JSON.
+    :param content: Content that will be processed as JSON.
     :param default: Callable used when stringifying values.
-    :param replace: Optional string values to replace in path.
+    :param replace: Optional values to replace in the file.
     :returns: Content after processing using JSON functions.
     """
 
     content = dumps(
         content, default=default)
 
     prefix = 'encommon_sample'
 
-    replace = dict(replace or {})
+    replace = replace or {}
+
+    items = replace.items()
 
-    replace |= {
-        'PROJECT': PROJECT,
-        'WORKSPACE': WORKSPACE}
+    for old, new in items:
 
-    for old, new in replace.items():
+        if isinstance(old, Path):
+            old = str(old)
 
         if isinstance(new, Path):
             new = str(new)
 
         content = content.replace(
             new, f'_/{prefix}/{old}/_')
 
     return loads(content)
 
 
 
 def load_sample(
-    path: Path,
+    path: str | Path,
     content: Optional[Any] = None,
     update: bool = False,
     *,
     default: Callable[[Any], str] = str,
-    replace: Optional[_REPLACE] = None,
+    replace: Optional['REPLACE'] = None,
 ) -> Any:
     """
     Load the sample file and compare using provided content.
 
     .. testsetup::
        >>> from json import dumps
        >>> from json import loads
@@ -102,39 +99,46 @@
     {'one': 'two'}
 
     Example
     -------
     >>> load_sample(sample)
     {'one': 'two'}
 
-    :param path: Complete or relative path to the sample file.
+    :param path: Complete or relative path for the sample.
     :param update: Determine whether the sample is updated.
-    :param content: Content which will be processed for JSON.
+    :param content: Content that will be processed as JSON.
     :param default: Callable used when stringifying values.
-    :param replace: Optional string values to replace in file.
+    :param replace: Optional values to replace in the file.
     :returns: Content after processing using JSON functions.
     """
 
+    path = Path(path).resolve()
+
     loaded: Optional[Any] = None
 
+
     content = prep_sample(
         content=content,
         default=default,
         replace=replace)
 
 
     def _save_sample() -> None:
-        path.write_text(
-            dumps(content, indent=2))
+
+        dumped = dumps(
+            content, indent=2)
+
+        save_text(path, dumped)
 
 
     def _load_sample() -> Any:
-        return loads(
-            path.read_text(
-                encoding='utf-8'))
+
+        loaded = read_text(path)
+
+        return loads(loaded)
 
 
     if path.exists():
         loaded = _load_sample()
 
     if not path.exists():
         _save_sample()
```

### Comparing `encommon-0.7.6/encommon/utils/stdout.py` & `encommon-0.8.0/encommon/utils/stdout.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 from re import sub as re_sub
 from sys import stdout
 from typing import Any
 from typing import Literal
 from typing import Optional
 from typing import Union
 
-from encommon.times import Duration
-from encommon.times import Times
-from encommon.types import Empty
-
 from .common import JOINABLE
+from ..times import Duration
+from ..times import Times
+from ..types import Empty
+from ..types.strings import COMMAD
+from ..types.strings import NEWLINE
+from ..types.strings import SEMPTY
 
 
 
 ANSICODE = compile(
     r'\x1b\[[^A-Za-z]*[A-Za-z]')
 
 ANSIARRAL = Union[
@@ -36,39 +38,43 @@
 
 ANSIARRAY = Union[
     ANSIARRAL,
     ANSIARRAD]
 
 
 
+_REPEAT = (list, tuple, dict)
+
+
+
 @dataclass(frozen=True)
 class ArrayColors:
     """
     Colors used to colorize the provided array like object.
     """
 
     label: int = 37
     key: int = 97
 
+    colon: int = 37
+    hyphen: int = 37
+
     bool: int = 93
     none: int = 33
     str: int = 92
     num: int = 93
 
     times: int = 96
     empty: int = 36
     other: int = 91
 
-    colon: int = 37
-    hyphen: int = 37
-
 
 
 def print_ansi(
-    string: str = '',
+    string: str = SEMPTY,
     method: Literal['stdout', 'print'] = 'stdout',
     output: bool = True,
 ) -> str:
     """
     Print the ANSI colorized string to the standard output.
 
     Example
@@ -129,16 +135,16 @@
     '\\x1b[0;90mk\\x1b[0;37m="\\x1b[0;0m...
 
     :param key: String value to use for the key name portion.
     :param value: String value to use for the value portion.
     :returns: ANSI colorized string using inline directives.
     """  # noqa: D301 LIT102
 
-    if isinstance(value, JOINABLE):  # type: ignore
-        value = ','.join([
+    if isinstance(value, JOINABLE):
+        value = COMMAD.join([
             str(x) for x in value])
 
     elif not isinstance(value, str):
         value = str(value)
 
     return make_ansi(
         f'<c90>{key}<c37>="<c0>'
@@ -157,15 +163,15 @@
     >>> strip_ansi('\\x1b[0;91mERROR\\x1b[0;0m')
     'ERROR'
 
     :param string: String which contains ANSI codes to strip.
     :returns: Provided string with the ANSI codes removed.
     """  # noqa: D301 LIT102
 
-    return re_sub(ANSICODE, '', string)
+    return re_sub(ANSICODE, SEMPTY, string)
 
 
 
 def array_ansi(  # noqa: CFQ001, CFQ004
     source: ANSIARRAY,
     *,
     indent: int = 0,
@@ -202,33 +208,36 @@
     ) -> None:
 
         if id(value) in refers:
             return output.append(
                 f'{prefix} {repeat}')
 
 
-        if isinstance(value, list | tuple | dict):
+        if isinstance(value, _REPEAT):
             refers.add(id(value))
 
 
-        types = {
+        typing = {
             'list': list,
             'tuple': tuple,
             'dict': dict,
             'frozenset': frozenset,
             'set': set}
 
-        for name, _type in types.items():
+        items = typing.items()
+
+        for name, _type in items:
 
             if not isinstance(value, _type):
                 continue
 
             output.append(
                 f'{prefix} '
-                f'<c{colors.label}>{name}<c0>')
+                f'<c{colors.label}>'
+                f'{name}<c0>')
 
             return _process(
                 source=value,
                 indent=indent + 2,
                 refers=refers)
 
 
@@ -277,15 +286,17 @@
         source: ANSIARRAD,
         indent: int,
         refers: Optional[set[int]] = None,
     ) -> None:
 
         assert isinstance(source, dict)
 
-        for key, value in source.items():
+        items = source.items()
+
+        for key, value in items:
 
             prefix = (
                 f'{" " * indent}'
                 f'<c{colors.key}>{key}'
                 f'<c{colors.colon}>:<c0>')
 
             _append(
@@ -336,8 +347,8 @@
     elif isinstance(source, set):
         _list(source, indent)
 
 
     _output = [
         make_ansi(x) for x in output]
 
-    return '\n'.join(_output)
+    return NEWLINE.join(_output)
```

### Comparing `encommon-0.7.6/encommon/utils/test/test_match.py` & `encommon-0.8.0/encommon/utils/test/test_match.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.6/encommon/utils/test/test_paths.py` & `encommon-0.8.0/encommon/utils/test/test_paths.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from pathlib import PosixPath
 
 from ..paths import resolve_path
 from ..paths import resolve_paths
 from ..paths import stats_path
 from ... import PROJECT
-from ...times.times import Times
+from ...times import Times
 
 
 
 def test_resolve_path() -> None:
     """
     Perform various tests associated with relevant routines.
     """
@@ -57,15 +57,15 @@
 def test_stats_path() -> None:
     """
     Perform various tests associated with relevant routines.
     """
 
     stats = stats_path(
         f'{PROJECT}/utils',
-        replace={str(PROJECT): '/'},
+        replace={PROJECT: '/'},
         ignore=[r'\S+\.pyc'])
 
     stat = stats['/utils/paths.py']
 
     assert stat.st_ctime >= (
         Times('2023-01-01').epoch)
     assert stat.st_mtime >= (
@@ -77,11 +77,12 @@
         '/utils/__init__.py',
         '/utils/common.py',
         '/utils/match.py',
         '/utils/paths.py',
         '/utils/sample.py',
         '/utils/stdout.py',
         '/utils/test/__init__.py',
+        '/utils/test/test_common.py',
         '/utils/test/test_match.py',
         '/utils/test/test_paths.py',
         '/utils/test/test_sample.py',
         '/utils/test/test_stdout.py']
```

### Comparing `encommon-0.7.6/encommon/utils/test/test_sample.py` & `encommon-0.8.0/encommon/utils/test/test_sample.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,38 +30,54 @@
 ) -> None:
     """
     Perform various tests associated with relevant routines.
 
     :param tmp_path: pytest object for temporal filesystem.
     """
 
-    path = (
-        Path(tmp_path)
-        .joinpath('samples.json'))
+    prefix = 'encommon_sample'
 
     source = {
         'list': ['bar', 'baz'],
         'tuple': (1, 2),
         'project': PROJECT,
-        'other': '/path/to/other'}
+        'other': '/pat/h',
+        'devnull': '/dev/null'}
 
     expect = {
         'list': ['bar', 'baz'],
         'tuple': [1, 2],
-        'project': '_/encommon_sample/PROJECT/_',
-        'other': '_/encommon_sample/tmp_path/_'}
+        'project': f'_/{prefix}/PROJECT/_',
+        'other': f'_/{prefix}/pytemp/_',
+        'devnull': '/dev/null'}
+
+
+    devnull = Path('/dev/null')
+
+    replaces = {
+        devnull: 'nothing here',
+        'PROJECT': str(PROJECT),
+        'pytemp': '/pat/h'}
+
+
+    sample_path = (
+        f'{tmp_path}/samples.json')
 
     sample = load_sample(
-        path=path,
+        path=sample_path,
         update=ENPYRWS,
         content=source,
-        replace={'tmp_path': '/path/to/other'})
+        replace=replaces)  # type: ignore
 
     assert sample == expect
 
+
+    source |= {'list': [1, 3, 2]}
+    expect |= {'list': [1, 3, 2]}
+
     sample = load_sample(
-        path=path,
-        content=source | {'list': [1]},
+        path=sample_path,
+        content=source,
         update=True,
-        replace={'tmp_path': '/path/to/other'})
+        replace=replaces)  # type: ignore
 
-    assert sample == expect | {'list': [1]}
+    assert sample == expect
```

### Comparing `encommon-0.7.6/encommon/utils/test/test_stdout.py` & `encommon-0.8.0/encommon/utils/test/test_stdout.py`

 * *Files identical despite different names*

### Comparing `encommon-0.7.6/encommon.egg-info/PKG-INFO` & `encommon-0.8.0/encommon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encommon
-Version: 0.7.6
+Version: 0.8.0
 Summary: Enasis Network Common Library
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `encommon-0.7.6/encommon.egg-info/SOURCES.txt` & `encommon-0.8.0/encommon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -58,11 +58,12 @@
 encommon/utils/__init__.py
 encommon/utils/common.py
 encommon/utils/match.py
 encommon/utils/paths.py
 encommon/utils/sample.py
 encommon/utils/stdout.py
 encommon/utils/test/__init__.py
+encommon/utils/test/test_common.py
 encommon/utils/test/test_match.py
 encommon/utils/test/test_paths.py
 encommon/utils/test/test_sample.py
 encommon/utils/test/test_stdout.py
```

### Comparing `encommon-0.7.6/pyproject.toml` & `encommon-0.8.0/pyproject.toml`

 * *Files identical despite different names*

