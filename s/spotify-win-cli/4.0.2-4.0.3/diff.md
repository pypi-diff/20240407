# Comparing `tmp/spotify-win-cli-4.0.2.tar.gz` & `tmp/spotify-win-cli-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify-win-cli-4.0.2.tar", last modified: Sun Apr  7 19:31:16 2024, max compression
+gzip compressed data, was "spotify-win-cli-4.0.3.tar", last modified: Sun Apr  7 19:31:30 2024, max compression
```

## Comparing `spotify-win-cli-4.0.2.tar` & `spotify-win-cli-4.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:16.695500 spotify-win-cli-4.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:16.691500 spotify-win-cli-4.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:16.691500 spotify-win-cli-4.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-07 19:31:12.000000 spotify-win-cli-4.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:31:16.691500 spotify-win-cli-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-07 19:31:12.000000 spotify-win-cli-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-07 19:31:12.000000 spotify-win-cli-4.0.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:31:16.695500 spotify-win-cli-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-07 19:31:12.000000 spotify-win-cli-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:16.691500 spotify-win-cli-4.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:31:12.000000 spotify-win-cli-4.0.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 19:31:12.000000 spotify-win-cli-4.0.2/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:16.691500 spotify-win-cli-4.0.2/src/spotify_win_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:31:16.000000 spotify-win-cli-4.0.2/src/spotify_win_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 19:31:16.000000 spotify-win-cli-4.0.2/src/spotify_win_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:31:16.000000 spotify-win-cli-4.0.2/src/spotify_win_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 19:31:16.000000 spotify-win-cli-4.0.2/src/spotify_win_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 19:31:16.000000 spotify-win-cli-4.0.2/src/spotify_win_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.743312 spotify-win-cli-4.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.743312 spotify-win-cli-4.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3264 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.743312 spotify-win-cli-4.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-07 19:31:26.000000 spotify-win-cli-4.0.3/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 19:31:30.747312 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 19:31:30.000000 spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/top_level.txt
```

### Comparing `spotify-win-cli-4.0.2/.github/workflows/python-publish.yml` & `spotify-win-cli-4.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `spotify-win-cli-4.0.2/PKG-INFO` & `spotify-win-cli-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-win-cli
-Version: 4.0.2
+Version: 4.0.3
 Summary: interact with spotify through commands
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 Project-URL: Homepage, https://github.com/aghastmuffin/spotify-cli
 Project-URL: Bug Reports, https://github.com/aghastmuffin/spotify-cli/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spotify-cli,spotify
```

### Comparing `spotify-win-cli-4.0.2/pyproject.toml` & `spotify-win-cli-4.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 name = "spotify-win-cli"  # REQUIRED, is the only field that cannot be marked as dynamic.
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "4.0.2"  # REQUIRED, although can be dynamic
+version = "4.0.3"  # REQUIRED, although can be dynamic
 dynamic = ["readme"]
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "interact with spotify through commands"
 
 # This is an optional longer description of your project that represents
```

### Comparing `spotify-win-cli-4.0.2/readme.md` & `spotify-win-cli-4.0.3/readme.md`

 * *Files identical despite different names*

### Comparing `spotify-win-cli-4.0.2/src/spotify_win_cli.egg-info/PKG-INFO` & `spotify-win-cli-4.0.3/src/spotify_win_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-win-cli
-Version: 4.0.2
+Version: 4.0.3
 Summary: interact with spotify through commands
 Author-email: "A. Random Developer" <author@example.com>
 Maintainer-email: "A. Great Maintainer" <maintainer@example.com>
 Project-URL: Homepage, https://github.com/aghastmuffin/spotify-cli
 Project-URL: Bug Reports, https://github.com/aghastmuffin/spotify-cli/issues
 Project-URL: Funding, https://donate.pypi.org
 Keywords: spotify-cli,spotify
```

