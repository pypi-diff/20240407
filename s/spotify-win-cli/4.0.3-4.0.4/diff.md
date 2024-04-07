# Comparing `tmp/spotify-win-cli-4.0.3.tar.gz` & `tmp/spotify-win-cli-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-win-cli-4.0.3.tar", last modified: Sun Apr  7 19:31:30 2024, max compression
+gzip compressed data, was "spotify-win-cli-4.0.4.tar", last modified: Sun Apr  7 19:55:05 2024, max compression
```

## Comparing `spotify-win-cli-4.0.3.tar` & `spotify-win-cli-4.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.743312 spotify-win-cli-4.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.743312 spotify-win-cli-4.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.743312 spotify-win-cli-4.0.3/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6861 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 19:55:01.000000 spotify-win-cli-4.0.4/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:55:05.493353 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:55:05.000000 spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/top_level.txt
```

### Comparing `spotify-win-cli-4.0.3/.github/workflows/python-publish.yml` & `spotify-win-cli-4.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `spotify-win-cli-4.0.3/PKG-INFO` & `spotify-win-cli-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-win-cli
-Version: 4.0.3
+Version: 4.0.4
 Summary: interact with spotify through commands
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 Project-URL: Homepage, https://github.com/aghastmuffin/spotify-cli
 Project-URL: Bug Reports, https://github.com/aghastmuffin/spotify-cli/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spotify-cli,spotify
```

### Comparing `spotify-win-cli-4.0.3/pyproject.toml` & `spotify-win-cli-4.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 # https://packaging.python.org/en/latest/tutorials/packaging-projects/#choosing-a-build-backend
 [build-system]
 # A list of packages that are needed to build your package:
 requires = ["setuptools>=64.0.0", "setuptools-scm>1.5.4"]  # REQUIRED if [build-system] table is used
 # The name of the Python object that frontends will use to perform the build:
 build-backend = "setuptools.build_meta"  # If not defined, then legacy behavior can happen.
 
+[tool.setuptools.packages.find]
+where = ["src/"]
 
 [project]
 # This is the name of your project. The first time you publish this
 # package, this name will be registered for you. It will determine how
 # users can install this project, e.g.:
 #
 # $ pip install sampleproject
@@ -29,15 +31,15 @@
 name = "spotify-win-cli"  # REQUIRED, is the only field that cannot be marked as dynamic.
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "4.0.3"  # REQUIRED, although can be dynamic
+version = "4.0.4"  # REQUIRED, although can be dynamic
 dynamic = ["readme"]
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "interact with spotify through commands"
 
 # This is an optional longer description of your project that represents
@@ -146,15 +148,15 @@
 [project.urls]
 "Homepage" = "https://github.com/aghastmuffin/spotify-cli"
 "Bug Reports" = "https://github.com/aghastmuffin/spotify-cli/issues"
 "Funding" = "https://donate.pypi.org"
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]
-spotify-win-cli = "spotify_win_cli:main.hw"
+spotify-win-cli = "main:hw"
 
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 # [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
```

### Comparing `spotify-win-cli-4.0.3/readme.md` & `spotify-win-cli-4.0.4/readme.md`

 * *Files identical despite different names*

### Comparing `spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/PKG-INFO` & `spotify-win-cli-4.0.4/src/spotify_win_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-win-cli
-Version: 4.0.3
+Version: 4.0.4
 Summary: interact with spotify through commands
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 Project-URL: Homepage, https://github.com/aghastmuffin/spotify-cli
 Project-URL: Bug Reports, https://github.com/aghastmuffin/spotify-cli/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spotify-cli,spotify
```

