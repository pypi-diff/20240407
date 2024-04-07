# Comparing `tmp/acstore-20240406.tar.gz` & `tmp/acstore-20240407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acstore-20240406.tar", last modified: Sat Apr  6 04:12:34 2024, max compression
+gzip compressed data, was "acstore-20240407.tar", last modified: Sun Apr  7 05:37:05 2024, max compression
```

## Comparing `acstore-20240406.tar` & `acstore-20240407.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.366788 acstore-20240406/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.354789 acstore-20240406/.github/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.360789 acstore-20240406/.github/workflows/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2441 2024-04-06 04:12:17.000000 acstore-20240406/.github/workflows/test_docker.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-06 03:53:55.000000 acstore-20240406/.github/workflows/test_docs.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4063 2024-04-06 03:54:09.000000 acstore-20240406/.github/workflows/test_tox.yml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23143 2024-04-06 03:53:46.000000 acstore-20240406/.pylintrc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-04-06 03:53:46.000000 acstore-20240406/.readthedocs.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-12-03 09:37:37.000000 acstore-20240406/.yamllint.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      575 2023-12-03 09:37:37.000000 acstore-20240406/ACKNOWLEDGEMENTS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2023-12-03 09:37:37.000000 acstore-20240406/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 09:37:37.000000 acstore-20240406/LICENSE
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      494 2023-12-03 09:37:37.000000 acstore-20240406/MANIFEST.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      691 2024-04-06 04:12:34.366788 acstore-20240406/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      249 2023-12-03 09:37:37.000000 acstore-20240406/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.360789 acstore-20240406/acstore/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      215 2024-04-06 04:12:17.000000 acstore-20240406/acstore/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.361789 acstore-20240406/acstore/containers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240406/acstore/containers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6615 2024-03-30 05:07:58.000000 acstore-20240406/acstore/containers/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3816 2024-03-30 05:07:58.000000 acstore-20240406/acstore/containers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-12-03 09:38:00.000000 acstore-20240406/acstore/errors.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-03-30 05:07:58.000000 acstore-20240406/acstore/fake_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.362789 acstore-20240406/acstore/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:00.000000 acstore-20240406/acstore/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3656 2024-04-06 04:12:17.000000 acstore-20240406/acstore/helpers/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2242 2023-12-03 09:38:00.000000 acstore-20240406/acstore/helpers/schema.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4598 2023-12-03 09:38:00.000000 acstore-20240406/acstore/helpers/yaml_definitions_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7840 2024-03-30 05:07:58.000000 acstore-20240406/acstore/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-12-03 09:38:00.000000 acstore-20240406/acstore/profilers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35352 2024-04-06 04:12:17.000000 acstore-20240406/acstore/sqlite_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.366788 acstore-20240406/acstore.egg-info/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      691 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/PKG-INFO
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/SOURCES.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/dependency_links.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       13 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/requires.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        8 2024-04-06 04:12:34.000000 acstore-20240406/acstore.egg-info/top_level.txt
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2023-12-03 09:37:37.000000 acstore-20240406/acstore.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-04-06 03:53:46.000000 acstore-20240406/appveyor.yml
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.355789 acstore-20240406/config/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.362789 acstore-20240406/config/appveyor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2024-04-06 03:53:46.000000 acstore-20240406/config/appveyor/install.ps1
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-04-06 03:53:46.000000 acstore-20240406/config/appveyor/install.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-04-06 03:53:46.000000 acstore-20240406/config/appveyor/runtests.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.363788 acstore-20240406/config/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      170 2024-04-06 04:12:17.000000 acstore-20240406/config/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       20 2023-12-03 09:37:37.000000 acstore-20240406/config/dpkg/clean
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-04-06 03:53:46.000000 acstore-20240406/config/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2024-04-06 03:53:46.000000 acstore-20240406/config/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-12-03 09:37:37.000000 acstore-20240406/config/dpkg/copyright
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-04-06 03:53:46.000000 acstore-20240406/config/dpkg/rules
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.363788 acstore-20240406/config/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 09:37:37.000000 acstore-20240406/config/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2024-04-06 03:53:34.000000 acstore-20240406/dependencies.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/docs/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5091 2024-04-06 03:53:46.000000 acstore-20240406/docs/conf.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      511 2023-12-03 09:38:02.000000 acstore-20240406/docs/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-04-06 03:53:46.000000 acstore-20240406/docs/requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.356789 acstore-20240406/docs/sources/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/docs/sources/api/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      540 2023-12-03 09:38:02.000000 acstore-20240406/docs/sources/api/acstore.containers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-03-30 05:07:58.000000 acstore-20240406/docs/sources/api/acstore.helpers.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2024-04-06 03:54:38.000000 acstore-20240406/docs/sources/api/acstore.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       58 2023-12-03 09:38:02.000000 acstore-20240406/docs/sources/api/modules.rst
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/docs/sources/user/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-30 05:08:02.000000 acstore-20240406/docs/sources/user/Installation-instructions.md
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      286 2023-12-03 09:38:02.000000 acstore-20240406/docs/sources/user/index.rst
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-04-06 03:53:46.000000 acstore-20240406/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       15 2024-04-06 03:53:46.000000 acstore-20240406/requirements.txt
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      929 2023-12-03 09:37:37.000000 acstore-20240406/run_tests.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      886 2024-04-06 04:12:34.367788 acstore-20240406/setup.cfg
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-04-06 03:53:46.000000 acstore-20240406/setup.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.364789 acstore-20240406/test_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      161 2023-12-03 09:37:37.000000 acstore-20240406/test_data/definitions.yaml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 09:37:37.000000 acstore-20240406/test_dependencies.ini
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 03:53:46.000000 acstore-20240406/test_requirements.txt
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.365789 acstore-20240406/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240406/tests/__init__.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.365789 acstore-20240406/tests/containers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240406/tests/containers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5724 2024-03-30 05:07:58.000000 acstore-20240406/tests/containers/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2838 2024-03-30 05:07:58.000000 acstore-20240406/tests/containers/manager.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8446 2023-12-03 09:37:37.000000 acstore-20240406/tests/fake_store.py
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.365789 acstore-20240406/tests/helpers/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:38.000000 acstore-20240406/tests/helpers/__init__.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1874 2024-03-30 05:07:58.000000 acstore-20240406/tests/helpers/json_serializer.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-12-03 09:37:38.000000 acstore-20240406/tests/helpers/schema.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3052 2023-12-03 09:37:38.000000 acstore-20240406/tests/helpers/yaml_definitions_file.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3332 2024-03-30 05:07:58.000000 acstore-20240406/tests/interface.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2023-12-03 09:37:37.000000 acstore-20240406/tests/profilers.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20058 2024-03-30 05:07:58.000000 acstore-20240406/tests/sqlite_store.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2375 2024-01-21 17:37:54.000000 acstore-20240406/tests/test_lib.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1359 2024-04-06 03:53:46.000000 acstore-20240406/tox.ini
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 04:12:34.366788 acstore-20240406/utils/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240406/utils/__init__.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-04-06 03:53:46.000000 acstore-20240406/utils/check_dependencies.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-04-06 03:53:46.000000 acstore-20240406/utils/dependencies.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      773 2024-03-30 05:07:58.000000 acstore-20240406/utils/update_release.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.272698 acstore-20240407/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.251698 acstore-20240407/.github/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.256698 acstore-20240407/.github/workflows/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2441 2024-04-06 04:13:05.000000 acstore-20240407/.github/workflows/test_docker.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-06 04:13:05.000000 acstore-20240407/.github/workflows/test_docs.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4063 2024-04-06 04:13:05.000000 acstore-20240407/.github/workflows/test_tox.yml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23143 2024-04-06 08:14:17.000000 acstore-20240407/.pylintrc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      322 2024-04-06 03:53:46.000000 acstore-20240407/.readthedocs.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2023-12-03 09:37:37.000000 acstore-20240407/.yamllint.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      575 2023-12-03 09:37:37.000000 acstore-20240407/ACKNOWLEDGEMENTS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      368 2023-12-03 09:37:37.000000 acstore-20240407/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11358 2023-12-03 09:37:37.000000 acstore-20240407/LICENSE
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      494 2023-12-03 09:37:37.000000 acstore-20240407/MANIFEST.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      691 2024-04-07 05:37:05.272698 acstore-20240407/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      249 2023-12-03 09:37:37.000000 acstore-20240407/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.257698 acstore-20240407/acstore/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      215 2024-04-07 05:12:15.000000 acstore-20240407/acstore/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.259698 acstore-20240407/acstore/containers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240407/acstore/containers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6615 2024-03-30 05:07:58.000000 acstore-20240407/acstore/containers/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3816 2024-03-30 05:07:58.000000 acstore-20240407/acstore/containers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      175 2023-12-03 09:38:00.000000 acstore-20240407/acstore/errors.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-03-30 05:07:58.000000 acstore-20240407/acstore/fake_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.259698 acstore-20240407/acstore/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:00.000000 acstore-20240407/acstore/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4179 2024-04-06 08:14:28.000000 acstore-20240407/acstore/helpers/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2242 2023-12-03 09:38:00.000000 acstore-20240407/acstore/helpers/schema.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4598 2023-12-03 09:38:00.000000 acstore-20240407/acstore/helpers/yaml_definitions_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7840 2024-03-30 05:07:58.000000 acstore-20240407/acstore/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-12-03 09:38:00.000000 acstore-20240407/acstore/profilers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35114 2024-04-06 08:14:28.000000 acstore-20240407/acstore/sqlite_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.272698 acstore-20240407/acstore.egg-info/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      691 2024-04-07 05:37:05.000000 acstore-20240407/acstore.egg-info/PKG-INFO
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1784 2024-04-07 05:37:05.000000 acstore-20240407/acstore.egg-info/SOURCES.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        1 2024-04-07 05:37:05.000000 acstore-20240407/acstore.egg-info/dependency_links.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       13 2024-04-07 05:37:05.000000 acstore-20240407/acstore.egg-info/requires.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        8 2024-04-07 05:37:05.000000 acstore-20240407/acstore.egg-info/top_level.txt
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      411 2023-12-03 09:37:37.000000 acstore-20240407/acstore.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1757 2024-04-06 03:53:46.000000 acstore-20240407/appveyor.yml
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.252698 acstore-20240407/config/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.260698 acstore-20240407/config/appveyor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      804 2024-04-06 08:14:17.000000 acstore-20240407/config/appveyor/install.ps1
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      125 2024-04-06 03:53:46.000000 acstore-20240407/config/appveyor/install.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      620 2024-04-06 03:53:46.000000 acstore-20240407/config/appveyor/runtests.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.262698 acstore-20240407/config/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      170 2024-04-07 05:12:15.000000 acstore-20240407/config/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       20 2023-12-03 09:37:37.000000 acstore-20240407/config/dpkg/clean
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        2 2024-04-06 03:53:46.000000 acstore-20240407/config/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      583 2024-04-06 08:14:17.000000 acstore-20240407/config/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2023-12-03 09:37:37.000000 acstore-20240407/config/dpkg/copyright
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      122 2024-04-06 03:53:46.000000 acstore-20240407/config/dpkg/rules
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.262698 acstore-20240407/config/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-12-03 09:37:37.000000 acstore-20240407/config/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      151 2024-04-06 08:14:17.000000 acstore-20240407/dependencies.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.263698 acstore-20240407/docs/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5091 2024-04-06 03:53:46.000000 acstore-20240407/docs/conf.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      511 2023-12-03 09:38:02.000000 acstore-20240407/docs/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      118 2024-04-06 03:53:46.000000 acstore-20240407/docs/requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.252698 acstore-20240407/docs/sources/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.264698 acstore-20240407/docs/sources/api/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      540 2023-12-03 09:38:02.000000 acstore-20240407/docs/sources/api/acstore.containers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-03-30 05:07:58.000000 acstore-20240407/docs/sources/api/acstore.helpers.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      971 2024-04-06 03:54:38.000000 acstore-20240407/docs/sources/api/acstore.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       58 2023-12-03 09:38:02.000000 acstore-20240407/docs/sources/api/modules.rst
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.265698 acstore-20240407/docs/sources/user/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-03-30 05:08:02.000000 acstore-20240407/docs/sources/user/Installation-instructions.md
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      286 2023-12-03 09:38:02.000000 acstore-20240407/docs/sources/user/index.rst
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      296 2024-04-06 03:53:46.000000 acstore-20240407/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       15 2024-04-06 08:14:17.000000 acstore-20240407/requirements.txt
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      929 2023-12-03 09:37:37.000000 acstore-20240407/run_tests.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      886 2024-04-07 05:37:05.274698 acstore-20240407/setup.cfg
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      128 2024-04-06 03:53:46.000000 acstore-20240407/setup.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.265698 acstore-20240407/test_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      161 2023-12-03 09:37:37.000000 acstore-20240407/test_data/definitions.yaml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-12-03 09:37:37.000000 acstore-20240407/test_dependencies.ini
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-06 03:53:46.000000 acstore-20240407/test_requirements.txt
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.268698 acstore-20240407/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240407/tests/__init__.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.269698 acstore-20240407/tests/containers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:37.000000 acstore-20240407/tests/containers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5724 2024-03-30 05:07:58.000000 acstore-20240407/tests/containers/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2838 2024-03-30 05:07:58.000000 acstore-20240407/tests/containers/manager.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8446 2023-12-03 09:37:37.000000 acstore-20240407/tests/fake_store.py
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.270698 acstore-20240407/tests/helpers/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:37:38.000000 acstore-20240407/tests/helpers/__init__.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1874 2024-03-30 05:07:58.000000 acstore-20240407/tests/helpers/json_serializer.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-12-03 09:37:38.000000 acstore-20240407/tests/helpers/schema.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3052 2023-12-03 09:37:38.000000 acstore-20240407/tests/helpers/yaml_definitions_file.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3332 2024-03-30 05:07:58.000000 acstore-20240407/tests/interface.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1649 2023-12-03 09:37:37.000000 acstore-20240407/tests/profilers.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20058 2024-03-30 05:07:58.000000 acstore-20240407/tests/sqlite_store.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2375 2024-01-21 17:37:54.000000 acstore-20240407/tests/test_lib.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1359 2024-04-06 03:53:46.000000 acstore-20240407/tox.ini
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-07 05:37:05.272698 acstore-20240407/utils/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       24 2023-12-03 09:38:01.000000 acstore-20240407/utils/__init__.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      422 2024-04-06 03:53:46.000000 acstore-20240407/utils/check_dependencies.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11583 2024-04-06 03:53:46.000000 acstore-20240407/utils/dependencies.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)      773 2024-03-30 05:07:58.000000 acstore-20240407/utils/update_release.sh
```

### Comparing `acstore-20240406/.github/workflows/test_docker.yml` & `acstore-20240407/.github/workflows/test_docker.yml`

 * *Files identical despite different names*

### Comparing `acstore-20240406/.github/workflows/test_docs.yml` & `acstore-20240407/.github/workflows/test_docs.yml`

 * *Files identical despite different names*

### Comparing `acstore-20240406/.github/workflows/test_tox.yml` & `acstore-20240407/.github/workflows/test_tox.yml`

 * *Files identical despite different names*

### Comparing `acstore-20240406/.pylintrc` & `acstore-20240407/.pylintrc`

 * *Files identical despite different names*

### Comparing `acstore-20240406/ACKNOWLEDGEMENTS` & `acstore-20240407/ACKNOWLEDGEMENTS`

 * *Files identical despite different names*

### Comparing `acstore-20240406/LICENSE` & `acstore-20240407/LICENSE`

 * *Files identical despite different names*

### Comparing `acstore-20240406/PKG-INFO` & `acstore-20240407/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acstore
-Version: 20240406
+Version: 20240407
 Summary: Attribute Container Storage (ACStore).
 Home-page: https://github.com/log2timeline/acstore
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `acstore-20240406/acstore/containers/interface.py` & `acstore-20240407/acstore/containers/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/acstore/containers/manager.py` & `acstore-20240407/acstore/containers/manager.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/acstore/fake_store.py` & `acstore-20240407/acstore/fake_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/acstore/helpers/json_serializer.py` & `acstore-20240407/acstore/helpers/json_serializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 """Attribute container JSON serializer."""
 
+from acstore.containers import interface as containers_interface
 from acstore.containers import manager as containers_manager
 from acstore.helpers import schema as schema_helper
 
 
 class AttributeContainerJSONSerializer(object):
   """Attribute container JSON serializer."""
 
@@ -41,19 +42,22 @@
 
     json_dict = {
         '__type__': 'AttributeContainer',
         '__container_type__': attribute_container.CONTAINER_TYPE}
 
     for attribute_name, attribute_value in attribute_container.GetAttributes():
       data_type = schema.get(attribute_name, None)
-      serializer = schema_helper.SchemaHelper.GetAttributeSerializer(
-          data_type, 'json')
-
-      if serializer:
-        attribute_value = serializer.SerializeValue(attribute_value)
+      if data_type == 'AttributeContainerIdentifier' and isinstance(
+          attribute_value, containers_interface.AttributeContainerIdentifier):
+        attribute_value = attribute_value.CopyToString()
+      else:
+        serializer = schema_helper.SchemaHelper.GetAttributeSerializer(
+            data_type, 'json')
+        if serializer:
+          attribute_value = serializer.SerializeValue(attribute_value)
 
       # JSON will not serialize certain runtime types like set, therefore
       # these are cast to list first.
       if isinstance(attribute_value, set):
         attribute_value = list(attribute_value)
 
       json_dict[attribute_name] = attribute_value
@@ -100,16 +104,20 @@
         continue
 
       # Be strict about which attributes to set.
       if attribute_name not in supported_attribute_names:
         continue
 
       data_type = schema.get(attribute_name, None)
-      serializer = schema_helper.SchemaHelper.GetAttributeSerializer(
-          data_type, 'json')
-
-      if serializer:
-        attribute_value = serializer.DeserializeValue(attribute_value)
+      if data_type == 'AttributeContainerIdentifier':
+        identifier = containers_interface.AttributeContainerIdentifier()
+        identifier.CopyFromString(attribute_value)
+        attribute_value = identifier
+      else:
+        serializer = schema_helper.SchemaHelper.GetAttributeSerializer(
+            data_type, 'json')
+        if serializer:
+          attribute_value = serializer.DeserializeValue(attribute_value)
 
       setattr(attribute_container, attribute_name, attribute_value)
 
     return attribute_container
```

### Comparing `acstore-20240406/acstore/helpers/schema.py` & `acstore-20240407/acstore/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/acstore/helpers/yaml_definitions_file.py` & `acstore-20240407/acstore/helpers/yaml_definitions_file.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/acstore/interface.py` & `acstore-20240407/acstore/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/acstore/profilers.py` & `acstore-20240407/acstore/profilers.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/acstore/sqlite_store.py` & `acstore-20240407/acstore/sqlite_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,31 +176,23 @@
     serialization_format (str): serialization format.
   """
 
   _FORMAT_VERSION = 20230312
 
   # The earliest format version, stored in-file, that this class
   # is able to append (write).
-  _APPEND_COMPATIBLE_FORMAT_VERSION = 20221023
+  _APPEND_COMPATIBLE_FORMAT_VERSION = 20230312
 
   # The earliest format version, stored in-file, that this class
   # is able to upgrade (write new format features).
-  _UPGRADE_COMPATIBLE_FORMAT_VERSION = 20221023
+  _UPGRADE_COMPATIBLE_FORMAT_VERSION = 20230312
 
   # The earliest format version, stored in-file, that this class
   # is able to read.
-  _READ_COMPATIBLE_FORMAT_VERSION = 20221023
-
-  # TODO: kept for backwards compatibility.
-  _CONTAINER_SCHEMA_TO_SQLITE_TYPE_MAPPINGS = {
-      'AttributeContainerIdentifier': 'TEXT',
-      'bool': 'INTEGER',
-      'int': 'INTEGER',
-      'str': 'TEXT',
-      'timestamp': 'BIGINT'}
+  _READ_COMPATIBLE_FORMAT_VERSION = 20230312
 
   _CREATE_METADATA_TABLE_QUERY = (
       'CREATE TABLE metadata (key TEXT, value TEXT);')
 
   _HAS_TABLE_QUERY = (
       'SELECT name FROM sqlite_master '
       'WHERE type = "table" AND name = "{0:s}"')
```

### Comparing `acstore-20240406/acstore.egg-info/PKG-INFO` & `acstore-20240407/acstore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acstore
-Version: 20240406
+Version: 20240407
 Summary: Attribute Container Storage (ACStore).
 Home-page: https://github.com/log2timeline/acstore
 Maintainer: Log2Timeline maintainers
 Maintainer-email: log2timeline-maintainers@googlegroups.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `acstore-20240406/acstore.egg-info/SOURCES.txt` & `acstore-20240407/acstore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acstore-20240406/appveyor.yml` & `acstore-20240407/appveyor.yml`

 * *Files identical despite different names*

### Comparing `acstore-20240406/config/appveyor/install.ps1` & `acstore-20240407/config/appveyor/install.ps1`

 * *Files identical despite different names*

### Comparing `acstore-20240406/config/appveyor/runtests.sh` & `acstore-20240407/config/appveyor/runtests.sh`

 * *Files identical despite different names*

### Comparing `acstore-20240406/config/dpkg/control` & `acstore-20240407/config/dpkg/control`

 * *Files identical despite different names*

### Comparing `acstore-20240406/config/dpkg/copyright` & `acstore-20240407/config/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `acstore-20240406/docs/conf.py` & `acstore-20240407/docs/conf.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/docs/sources/api/acstore.containers.rst` & `acstore-20240407/docs/sources/api/acstore.containers.rst`

 * *Files identical despite different names*

### Comparing `acstore-20240406/docs/sources/api/acstore.helpers.rst` & `acstore-20240407/docs/sources/api/acstore.helpers.rst`

 * *Files identical despite different names*

### Comparing `acstore-20240406/docs/sources/api/acstore.rst` & `acstore-20240407/docs/sources/api/acstore.rst`

 * *Files identical despite different names*

### Comparing `acstore-20240406/docs/sources/user/Installation-instructions.md` & `acstore-20240407/docs/sources/user/Installation-instructions.md`

 * *Files identical despite different names*

### Comparing `acstore-20240406/run_tests.py` & `acstore-20240407/run_tests.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/setup.cfg` & `acstore-20240407/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = acstore
-version = 20240406
+version = 20240407
 description = Attribute Container Storage (ACStore).
 long_description = ACStore, or Attribute Container Storage, provides a stand-alone implementation to read and write attribute container storage files.
 long_description_content_type = text/plain
 url = https://github.com/log2timeline/acstore
 maintainer = Log2Timeline maintainers
 maintainer_email = log2timeline-maintainers@googlegroups.com
 license = Apache License, Version 2.0
```

### Comparing `acstore-20240406/tests/containers/interface.py` & `acstore-20240407/tests/containers/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/containers/manager.py` & `acstore-20240407/tests/containers/manager.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/fake_store.py` & `acstore-20240407/tests/fake_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/helpers/json_serializer.py` & `acstore-20240407/tests/helpers/json_serializer.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/helpers/schema.py` & `acstore-20240407/tests/helpers/schema.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/helpers/yaml_definitions_file.py` & `acstore-20240407/tests/helpers/yaml_definitions_file.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/interface.py` & `acstore-20240407/tests/interface.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/profilers.py` & `acstore-20240407/tests/profilers.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/sqlite_store.py` & `acstore-20240407/tests/sqlite_store.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tests/test_lib.py` & `acstore-20240407/tests/test_lib.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/tox.ini` & `acstore-20240407/tox.ini`

 * *Files identical despite different names*

### Comparing `acstore-20240406/utils/dependencies.py` & `acstore-20240407/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `acstore-20240406/utils/update_release.sh` & `acstore-20240407/utils/update_release.sh`

 * *Files identical despite different names*

