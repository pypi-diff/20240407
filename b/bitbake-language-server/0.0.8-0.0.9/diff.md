# Comparing `tmp/bitbake-language-server-0.0.8.tar.gz` & `tmp/bitbake-language-server-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitbake-language-server-0.0.8.tar", last modified: Tue Jan 30 08:21:18 2024, max compression
+gzip compressed data, was "bitbake-language-server-0.0.9.tar", last modified: Fri Mar  1 07:55:45 2024, max compression
```

## Comparing `bitbake-language-server-0.0.8.tar` & `bitbake-language-server-0.0.9.tar`

### file list

```diff
@@ -1,55 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.691590 bitbake-language-server-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.683590 bitbake-language-server-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.683590 bitbake-language-server-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/.gitignore
--rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/.gitlint
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/.readthedocs.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/.yamllint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-01-30 08:21:18.691590 bitbake-language-server-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6802 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.683590 bitbake-language-server-0.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.683590 bitbake-language-server-0.0.8/docs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/docs/api/bitbake-language-server.md
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/docs/index.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.687590 bitbake-language-server-0.0.8/docs/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/docs/resources/configure.md
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/docs/resources/install.md
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/docs/resources/requirements.md
--rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.687590 bitbake-language-server-0.0.8/requirements/
--rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/requirements/dev.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       97 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.687590 bitbake-language-server-0.0.8/sdist/
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/sdist/_bitbake-language-server
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/sdist/bitbake-language-server
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/sdist/bitbake-language-server.1
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 08:21:18.691590 bitbake-language-server-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.683590 bitbake-language-server-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.687590 bitbake-language-server-0.0.8/src/bitbake_language_server/
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/src/bitbake_language_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/src/bitbake_language_server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server/_metainfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/src/bitbake_language_server/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/src/bitbake_language_server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/src/bitbake_language_server/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.691590 bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 08:21:18.000000 bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.687590 bitbake-language-server-0.0.8/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/templates/class.txt
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/templates/def.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/templates/noarg.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 08:21:18.687590 bitbake-language-server-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/tests/test.bb
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-01-30 08:21:05.000000 bitbake-language-server-0.0.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.383070 bitbake-language-server-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.375070 bitbake-language-server-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.375070 bitbake-language-server-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/.gitignore
+-rwxr-xr-x   0 runner    (1001) docker     (127)      101 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/.gitlint
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/.readthedocs.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      157 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/.yamllint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-01 07:55:45.383070 bitbake-language-server-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.375070 bitbake-language-server-0.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.375070 bitbake-language-server-0.0.9/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/docs/api/bitbake-language-server.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/docs/index.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      105 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.379070 bitbake-language-server-0.0.9/docs/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/docs/resources/configure.md
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/docs/resources/install.md
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/docs/resources/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2975 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.379070 bitbake-language-server-0.0.9/requirements/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       90 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/requirements/dev.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       51 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.379070 bitbake-language-server-0.0.9/sdist/
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/sdist/_bitbake-language-server
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/sdist/bitbake-language-server
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/sdist/bitbake-language-server.1
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 07:55:45.383070 bitbake-language-server-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.375070 bitbake-language-server-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.379070 bitbake-language-server-0.0.9/src/bitbake_language_server/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/_metainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/src/bitbake_language_server/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.383070 bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8376 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-01 07:55:45.000000 bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.379070 bitbake-language-server-0.0.9/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/templates/class.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/templates/def.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/templates/noarg.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 07:55:45.383070 bitbake-language-server-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/tests/test.bb
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-01 07:55:35.000000 bitbake-language-server-0.0.9/tests/test_utils.py
```

### Comparing `bitbake-language-server-0.0.8/.github/workflows/main.yml` & `bitbake-language-server-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/.gitignore` & `bitbake-language-server-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/.pre-commit-config.yaml` & `bitbake-language-server-0.0.9/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ---
-exclude: (^templates/.*|.*\.json$)
+exclude: ^templates/.*
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
       - id: check-added-large-files
       - id: fix-byte-order-marker
@@ -47,42 +47,43 @@
     hooks:
       - id: check-mailmap
   - repo: https://github.com/rhysd/actionlint
     rev: v1.6.26
     hooks:
       - id: actionlint
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.33.0
+    rev: v1.35.1
     hooks:
       - id: yamllint
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
       - id: mdformat
         additional_dependencies:
           - mdformat-pyproject
           - mdformat-gfm
           - mdformat-myst
           - mdformat-toc
           - mdformat-deflist
           - mdformat-beautysh
-          - mdformat-black
+          - mdformat-ruff
           - mdformat-config
+          - mdformat-web
   - repo: https://github.com/DavidAnson/markdownlint-cli2
     rev: v0.12.1
     hooks:
       - id: markdownlint-cli2
         additional_dependencies:
           - markdown-it-texmath
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.14
+    rev: v0.2.1
     hooks:
       - id: ruff
       - id: ruff-format
   - repo: https://github.com/kumaraditya303/mirrors-pyright
-    rev: v1.1.348
+    rev: v1.1.350
     hooks:
       - id: pyright
 
 ci:
   skip:
     - pyright
```

### Comparing `bitbake-language-server-0.0.8/LICENSE` & `bitbake-language-server-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/PKG-INFO` & `bitbake-language-server-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: oelint-parser>=3.0.2
+Requires-Dist: oelint-adv
 Requires-Dist: pygls
 Provides-Extra: dev
 Requires-Dist: pytest-cov; extra == "dev"
 
 # bitbake-language-server
 
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
@@ -69,24 +69,26 @@
 [![pypi/format](https://shields.io/pypi/format/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 
 Language server for
 [bitbake](https://docs.yoctoproject.org/bitbake/index.html).
 
-- [ ] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic)
+- [x] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic)
 - [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink)
 - [x] [Goto Definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_definition)
 - [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
 - [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion)
 
 A video is [here](https://asciinema.org/a/628560):
 
 ![628560](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/5720403e-7bf4-436c-91aa-578482a7ba07)
 
+![diagnostic](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/455f9b9c-1985-4b20-aae0-ebc1ead1f7d9)
+
 ![document hover](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/843dda35-4378-4295-83ad-7d5552d37c4f)
 
 ![document link](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/a61a132f-18cf-42a7-8cef-0dd5d830bc34)
 
 Read
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
 to know more.
```

### Comparing `bitbake-language-server-0.0.8/README.md` & `bitbake-language-server-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,24 +36,26 @@
 [![pypi/format](https://shields.io/pypi/format/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 
 Language server for
 [bitbake](https://docs.yoctoproject.org/bitbake/index.html).
 
-- [ ] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic)
+- [x] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic)
 - [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink)
 - [x] [Goto Definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_definition)
 - [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
 - [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion)
 
 A video is [here](https://asciinema.org/a/628560):
 
 ![628560](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/5720403e-7bf4-436c-91aa-578482a7ba07)
 
+![diagnostic](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/455f9b9c-1985-4b20-aae0-ebc1ead1f7d9)
+
 ![document hover](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/843dda35-4378-4295-83ad-7d5552d37c4f)
 
 ![document link](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/a61a132f-18cf-42a7-8cef-0dd5d830bc34)
 
 Read
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
 to know more.
```

### Comparing `bitbake-language-server-0.0.8/docs/conf.py` & `bitbake-language-server-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/docs/resources/configure.md` & `bitbake-language-server-0.0.9/docs/resources/configure.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/docs/resources/install.md` & `bitbake-language-server-0.0.9/docs/resources/install.md`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/pyproject.toml` & `bitbake-language-server-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/sdist/_bitbake-language-server` & `bitbake-language-server-0.0.9/sdist/_bitbake-language-server`

 * *Files 17% similar despite different names*

```diff
@@ -35,8 +35,16 @@
       esac
   esac
 }
 
 
 
 typeset -A opt_args
-_shtab_bitbake_language_server "$@"
+
+if [[ $zsh_eval_context[-1] == eval ]]; then
+  # eval/source/. command, register function for later
+  compdef _shtab_bitbake_language_server -N bitbake-language-server
+else
+  # autoload from fpath, call function directly
+  _shtab_bitbake_language_server "$@"
+fi
+
```

### Comparing `bitbake-language-server-0.0.8/sdist/bitbake-language-server` & `bitbake-language-server-0.0.9/sdist/bitbake-language-server`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/src/bitbake_language_server/__main__.py` & `bitbake-language-server-0.0.9/src/bitbake_language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/src/bitbake_language_server/_metainfo.py` & `bitbake-language-server-0.0.9/src/bitbake_language_server/_metainfo.py`

 * *Files identical despite different names*

### Comparing `bitbake-language-server-0.0.8/src/bitbake_language_server/server.py` & `bitbake-language-server-0.0.9/src/bitbake_language_server/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,53 @@
 r"""Server
 ==========
 """
 
 import os
 import re
+import sys
 from typing import Any
 
 from lsprotocol.types import (
     INITIALIZE,
     TEXT_DOCUMENT_COMPLETION,
     TEXT_DOCUMENT_DEFINITION,
     TEXT_DOCUMENT_DID_CHANGE,
     TEXT_DOCUMENT_DID_OPEN,
     TEXT_DOCUMENT_DOCUMENT_LINK,
     TEXT_DOCUMENT_HOVER,
     CompletionItem,
     CompletionItemKind,
     CompletionList,
     CompletionParams,
+    Diagnostic,
+    DiagnosticSeverity,
     DidChangeTextDocumentParams,
     DocumentLink,
     DocumentLinkParams,
     Hover,
     InitializeParams,
     Location,
     MarkupContent,
     MarkupKind,
     Position,
     Range,
     TextDocumentPositionParams,
 )
+from oelint_adv.__main__ import arguments_post, create_argparser
 from oelint_parser.cls_item import Function, Inherit, Variable
 from oelint_parser.cls_stash import Stash
 from pygls.server import LanguageServer
 from pygls.uris import from_fs_path
 
+from .tool import run2
 from .utils import render_document
 
+parser = create_argparser()
+
 
 class BitbakeLanguageServer(LanguageServer):
     r"""Bitbake language server."""
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         r"""Init.
 
@@ -69,14 +76,32 @@
             :param params:
             :type params: DidChangeTextDocumentParams
             :rtype: None
             """
             document = self.workspace.get_document(params.text_document.uri)
             self.stash.AddFile(document.path)
             self.show_message(f"Add {document.path}")
+            args = arguments_post(
+                create_argparser().parse_args([sys.argv[0], document.path])
+            )
+            diagnostics = []
+            for issue in run2(args):
+                line = issue[0][1]
+                words = issue[1].split(":")
+                severity = {
+                    "info": DiagnosticSeverity.Information,
+                    "warning": DiagnosticSeverity.Warning,
+                }.get(words[-2], DiagnosticSeverity.Error)
+                diagnostic = Diagnostic(
+                    Range(Position(line - 1, 0), Position(line, 0)),
+                    words[-1],
+                    severity,
+                )
+                diagnostics += [diagnostic]
+            self.publish_diagnostics(params.text_document.uri, diagnostics)
 
         @self.feature(TEXT_DOCUMENT_DOCUMENT_LINK)
         def document_link(params: DocumentLinkParams) -> list[DocumentLink]:
             r"""Get document links.
             Wait `<https://github.com/priv-kweihmann/oelint-parser/issues/189>_`
 
             :param params:
```

### Comparing `bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/PKG-INFO` & `bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitbake-language-server
-Version: 0.0.8
+Version: 0.0.9
 Summary: bitbake language server
 Author-email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Project-URL: Homepage, https://bitbake-language-server.readthedocs.io
 Project-URL: Download, https://github.com/Freed-Wu/bitbake-language-server/releases
 Project-URL: Bug Report, https://github.com/Freed-Wu/bitbake-language-server/issues
 Project-URL: Source, https://github.com/Freed-Wu/bitbake-language-server
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: oelint-parser>=3.0.2
+Requires-Dist: oelint-adv
 Requires-Dist: pygls
 Provides-Extra: dev
 Requires-Dist: pytest-cov; extra == "dev"
 
 # bitbake-language-server
 
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
@@ -69,24 +69,26 @@
 [![pypi/format](https://shields.io/pypi/format/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 [![pypi/implementation](https://shields.io/pypi/implementation/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 [![pypi/pyversions](https://shields.io/pypi/pyversions/bitbake-language-server)](https://pypi.org/project/bitbake-language-server/#files)
 
 Language server for
 [bitbake](https://docs.yoctoproject.org/bitbake/index.html).
 
-- [ ] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic)
+- [x] [Diagnostic](https://microsoft.github.io/language-server-protocol/specifications/specification-current#diagnostic)
 - [x] [Document Link](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_documentLink)
 - [x] [Goto Definition](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_definition)
 - [x] [Hover](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_hover)
 - [x] [Completion](https://microsoft.github.io/language-server-protocol/specifications/specification-current#textDocument_completion)
 
 A video is [here](https://asciinema.org/a/628560):
 
 ![628560](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/5720403e-7bf4-436c-91aa-578482a7ba07)
 
+![diagnostic](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/455f9b9c-1985-4b20-aae0-ebc1ead1f7d9)
+
 ![document hover](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/843dda35-4378-4295-83ad-7d5552d37c4f)
 
 ![document link](https://github.com/Freed-Wu/bitbake-language-server/assets/32936898/a61a132f-18cf-42a7-8cef-0dd5d830bc34)
 
 Read
 [![readthedocs](https://shields.io/readthedocs/bitbake-language-server)](https://bitbake-language-server.readthedocs.io)
 to know more.
```

### Comparing `bitbake-language-server-0.0.8/src/bitbake_language_server.egg-info/SOURCES.txt` & `bitbake-language-server-0.0.9/src/bitbake_language_server.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 sdist/bitbake-language-server.1
 src/bitbake_language_server/__init__.py
 src/bitbake_language_server/__main__.py
 src/bitbake_language_server/_metainfo.py
 src/bitbake_language_server/_version.py
 src/bitbake_language_server/py.typed
 src/bitbake_language_server/server.py
+src/bitbake_language_server/tool.py
 src/bitbake_language_server/utils.py
 src/bitbake_language_server.egg-info/PKG-INFO
 src/bitbake_language_server.egg-info/SOURCES.txt
 src/bitbake_language_server.egg-info/dependency_links.txt
 src/bitbake_language_server.egg-info/entry_points.txt
 src/bitbake_language_server.egg-info/requires.txt
 src/bitbake_language_server.egg-info/top_level.txt
```

