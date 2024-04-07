# Comparing `tmp/spotify-win-cli-4.0.4.tar.gz` & `tmp/spotify-win-cli-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-win-cli-4.0.4.tar", last modified: Sun Apr  7 19:55:05 2024, max compression
+gzip compressed data, was "spotify-win-cli-4.0.5.tar", last modified: Sun Apr  7 19:55:40 2024, max compression
```

## Comparing `spotify-win-cli-4.0.4.tar` & `spotify-win-cli-4.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:40.927662 spotify-win-cli-4.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:40.923662 spotify-win-cli-4.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:40.923662 spotify-win-cli-4.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-07 19:55:36.000000 spotify-win-cli-4.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:55:40.927662 spotify-win-cli-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-04-07 19:55:36.000000 spotify-win-cli-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-07 19:55:36.000000 spotify-win-cli-4.0.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:55:40.927662 spotify-win-cli-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-07 19:55:36.000000 spotify-win-cli-4.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:40.923662 spotify-win-cli-4.0.5/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:36.000000 spotify-win-cli-4.0.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 19:55:36.000000 spotify-win-cli-4.0.5/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:40.927662 spotify-win-cli-4.0.5/src/spotify_win_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:55:40.000000 spotify-win-cli-4.0.5/src/spotify_win_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 19:55:40.000000 spotify-win-cli-4.0.5/src/spotify_win_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:40.000000 spotify-win-cli-4.0.5/src/spotify_win_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 19:55:40.000000 spotify-win-cli-4.0.5/src/spotify_win_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:40.000000 spotify-win-cli-4.0.5/src/spotify_win_cli.egg-info/top_level.txt
```

### Comparing `spotify-win-cli-4.0.4/.github/workflows/python-publish.yml` & `spotify-win-cli-4.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `spotify-win-cli-4.0.4/PKG-INFO` & `spotify-win-cli-4.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-win-cli
-Version: 4.0.4
+Version: 4.0.5
 Summary: interact with spotify through commands
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 Project-URL: Homepage, https://github.com/aghastmuffin/spotify-cli
 Project-URL: Bug Reports, https://github.com/aghastmuffin/spotify-cli/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spotify-cli,spotify
```

### Comparing `spotify-win-cli-4.0.4/pyproject.toml` & `spotify-win-cli-4.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 [build-system]
 # A list of packages that are needed to build your package:
 requires = ["setuptools>=64.0.0", "setuptools-scm>1.5.4"]  # REQUIRED if [build-system] table is used
 # The name of the Python object that frontends will use to perform the build:
 build-backend = "setuptools.build_meta"  # If not defined, then legacy behavior can happen.
 
 [tool.setuptools.packages.find]
-where = ["src/"]
+where = ["src/"] #https://packaging.python.org/en/latest/guides/packaging-namespace-packages/
 
 [project]
 # This is the name of your project. The first time you publish this
 # package, this name will be registered for you. It will determine how
 # users can install this project, e.g.:
 #
 # $ pip install sampleproject
@@ -31,15 +31,15 @@
 name = "spotify-win-cli"  # REQUIRED, is the only field that cannot be marked as dynamic.
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "4.0.4"  # REQUIRED, although can be dynamic
+version = "4.0.5"  # REQUIRED, although can be dynamic
 dynamic = ["readme"]
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "interact with spotify through commands"
 
 # This is an optional longer description of your project that represents
```

### Comparing `spotify-win-cli-4.0.4/readme.md` & `spotify-win-cli-4.0.5/readme.md`

 * *Files identical despite different names*

### Comparing `spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/PKG-INFO` & `spotify-win-cli-4.0.5/src/spotify_win_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-win-cli
-Version: 4.0.4
+Version: 4.0.5
 Summary: interact with spotify through commands
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 Project-URL: Homepage, https://github.com/aghastmuffin/spotify-cli
 Project-URL: Bug Reports, https://github.com/aghastmuffin/spotify-cli/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spotify-cli,spotify
```

