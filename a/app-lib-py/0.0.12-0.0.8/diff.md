# Comparing `tmp/app_lib_py-0.0.12.tar.gz` & `tmp/app_lib_py-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_lib_py-0.0.12.tar", last modified: Sun Apr  7 19:23:14 2024, max compression
+gzip compressed data, was "app_lib_py-0.0.8.tar", last modified: Sun Apr  7 16:32:33 2024, max compression
```

## Comparing `app_lib_py-0.0.12.tar` & `app_lib_py-0.0.8.tar`

### file list

```diff
@@ -1,53 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.145791 app_lib_py-0.0.12/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.149791 app_lib_py-0.0.12/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.149791 app_lib_py-0.0.12/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/workflows/docker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/workflows/lint_style.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/workflows/pydoctor.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/workflows/pytest_app.yml
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/workflows/pytest_lib.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    35823 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.149791 app_lib_py-0.0.12/app/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/app/home.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/app/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/app/pages/2_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/app/pages/3_use_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/app/pages/4_about.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)     9262 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/app/static/a_l_p.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.145791 app_lib_py-0.0.12/app/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/app/tests/use_cases/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/app/tests/use_cases/test_add_curve.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/citation.cff
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/dev.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/docs/docs.md
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/requirements_lib.txt
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/src/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/src/app_lib_py/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/src/app_lib_py/ClassCurves.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/src/app_lib_py/ModulePredict.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/src/app_lib_py/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/src/app_lib_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-07 19:23:14.000000 app_lib_py-0.0.12/src/app_lib_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-07 19:23:14.000000 app_lib_py-0.0.12/src/app_lib_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:23:14.000000 app_lib_py-0.0.12/src/app_lib_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 19:23:14.000000 app_lib_py-0.0.12/src/app_lib_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.149791 app_lib_py-0.0.12/src/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/src/tests/speed/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/src/tests/speed/speed_log.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:23:14.153791 app_lib_py-0.0.12/src/tests/utility/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-07 19:23:08.000000 app_lib_py-0.0.12/src/tests/utility/test_curves.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      548 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       41 2024-04-07 15:19:09.000000 app_lib_py-0.0.8/README.md
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      117 2024-04-07 15:24:38.000000 app_lib_py-0.0.8/pyproject.toml
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       39 2024-04-06 21:59:37.000000 app_lib_py-0.0.8/requirements.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      654 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/setup.cfg
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/src/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/src/app_lib_py/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     1150 2024-04-06 22:49:59.000000 app_lib_py-0.0.8/src/app_lib_py/ClassCurves.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2024-04-06 22:06:58.000000 app_lib_py-0.0.8/src/app_lib_py/ModulePredict.py
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        0 2024-04-06 20:23:30.000000 app_lib_py-0.0.8/src/app_lib_py/__init__.py
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/src/app_lib_py.egg-info/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      548 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/PKG-INFO
+-rw-r--r--   0 rachel    (1000) rachel    (1000)      347 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/SOURCES.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)        1 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/dependency_links.txt
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       11 2024-04-07 16:32:33.000000 app_lib_py-0.0.8/src/app_lib_py.egg-info/top_level.txt
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/tests/
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/tests/speed/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)       35 2024-04-06 21:59:58.000000 app_lib_py-0.0.8/tests/speed/speed_log.csv
+drwxr-xr-x   0 rachel    (1000) rachel    (1000)        0 2024-04-07 16:32:33.904053 app_lib_py-0.0.8/tests/utility/
+-rw-r--r--   0 rachel    (1000) rachel    (1000)     1506 2024-04-07 10:53:27.000000 app_lib_py-0.0.8/tests/utility/test_curves.py
```

### Comparing `app_lib_py-0.0.12/setup.cfg` & `app_lib_py-0.0.8/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [metadata]
 name = app_lib_py
+version = 0.0.8
 author = Rachel Alcraft
 author_email = rachelalcraft@gmail.com
 description = Example library for scientific software.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RachelAlcraft/app-lib-py
 project_urls =
```

### Comparing `app_lib_py-0.0.12/src/app_lib_py/ClassCurves.py` & `app_lib_py-0.0.8/src/app_lib_py/ClassCurves.py`

 * *Files identical despite different names*

### Comparing `app_lib_py-0.0.12/src/tests/utility/test_curves.py` & `app_lib_py-0.0.8/tests/utility/test_curves.py`

 * *Files identical despite different names*

