# Comparing `tmp/prosperity2submit-0.1.0.tar.gz` & `tmp/prosperity2submit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2submit-0.1.0.tar", last modified: Sun Apr  7 00:58:34 2024, max compression
+gzip compressed data, was "prosperity2submit-0.1.1.tar", last modified: Sun Apr  7 01:01:25 2024, max compression
```

## Comparing `prosperity2submit-0.1.0.tar` & `prosperity2submit-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:58:34.862799 prosperity2submit-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 00:58:22.000000 prosperity2submit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-07 00:58:34.862799 prosperity2submit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-07 00:58:22.000000 prosperity2submit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:58:34.862799 prosperity2submit-0.1.0/prosperity2submit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:58:22.000000 prosperity2submit-0.1.0/prosperity2submit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-07 00:58:22.000000 prosperity2submit-0.1.0/prosperity2submit/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 00:58:22.000000 prosperity2submit-0.1.0/prosperity2submit/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:58:34.862799 prosperity2submit-0.1.0/prosperity2submit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-04-07 00:58:34.000000 prosperity2submit-0.1.0/prosperity2submit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 00:58:34.000000 prosperity2submit-0.1.0/prosperity2submit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:58:34.000000 prosperity2submit-0.1.0/prosperity2submit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 00:58:34.000000 prosperity2submit-0.1.0/prosperity2submit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 00:58:34.000000 prosperity2submit-0.1.0/prosperity2submit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 00:58:34.000000 prosperity2submit-0.1.0/prosperity2submit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 00:58:31.000000 prosperity2submit-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:58:34.862799 prosperity2submit-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/prosperity2submit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/prosperity2submit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/prosperity2submit/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 01:01:21.000000 prosperity2submit-0.1.1/prosperity2submit/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/prosperity2submit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4727 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 01:01:25.000000 prosperity2submit-0.1.1/prosperity2submit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 01:01:23.000000 prosperity2submit-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:01:25.926389 prosperity2submit-0.1.1/setup.cfg
```

### Comparing `prosperity2submit-0.1.0/LICENSE` & `prosperity2submit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.1.0/PKG-INFO` & `prosperity2submit-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 Requires-Dist: requests-toolbelt
 
 # IMC Prosperity 2 Submitter
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-submitter/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-submitter/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2submit)](https://pypi.org/project/prosperity2submit/)
 
-This repository contains a command-line submitter for [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. It uploads the algorithm, monitors its progress, downloads the logs, logs the final profit / loss, and opens the result in my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (optional), all in one command.
+This repository contains a command-line submitter for [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. It uploads the algorithm, monitors its progress, downloads the logs, logs the final profit / loss, and opens the submission in my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (optional), all in one command.
 
 ## Usage
 
 Basic usage:
 ```sh
 # Install the latest version of the submitter
 $ pip install -U prosperity2submit
```

### Comparing `prosperity2submit-0.1.0/README.md` & `prosperity2submit-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # IMC Prosperity 2 Submitter
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-submitter/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-submitter/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2submit)](https://pypi.org/project/prosperity2submit/)
 
-This repository contains a command-line submitter for [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. It uploads the algorithm, monitors its progress, downloads the logs, logs the final profit / loss, and opens the result in my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (optional), all in one command.
+This repository contains a command-line submitter for [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. It uploads the algorithm, monitors its progress, downloads the logs, logs the final profit / loss, and opens the submission in my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (optional), all in one command.
 
 ## Usage
 
 Basic usage:
 ```sh
 # Install the latest version of the submitter
 $ pip install -U prosperity2submit
```

### Comparing `prosperity2submit-0.1.0/prosperity2submit/core.py` & `prosperity2submit-0.1.1/prosperity2submit/core.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.1.0/prosperity2submit/main.py` & `prosperity2submit-0.1.1/prosperity2submit/main.py`

 * *Files identical despite different names*

### Comparing `prosperity2submit-0.1.0/prosperity2submit.egg-info/PKG-INFO` & `prosperity2submit-0.1.1/prosperity2submit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2submit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command-line submitter for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 Requires-Dist: requests-toolbelt
 
 # IMC Prosperity 2 Submitter
 
 [![Build Status](https://github.com/jmerle/imc-prosperity-2-submitter/workflows/Build/badge.svg)](https://github.com/jmerle/imc-prosperity-2-submitter/actions/workflows/build.yml)
 [![PyPI Version](https://img.shields.io/pypi/v/prosperity2submit)](https://pypi.org/project/prosperity2submit/)
 
-This repository contains a command-line submitter for [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. It uploads the algorithm, monitors its progress, downloads the logs, logs the final profit / loss, and opens the result in my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (optional), all in one command.
+This repository contains a command-line submitter for [IMC Prosperity 2](https://prosperity.imc.com/) algorithms. It uploads the algorithm, monitors its progress, downloads the logs, logs the final profit / loss, and opens the submission in my [IMC Prosperity 2 Visualizer](https://github.com/jmerle/imc-prosperity-2-visualizer) (optional), all in one command.
 
 ## Usage
 
 Basic usage:
 ```sh
 # Install the latest version of the submitter
 $ pip install -U prosperity2submit
```

### Comparing `prosperity2submit-0.1.0/pyproject.toml` & `prosperity2submit-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2submit"
 description = "Command-line submitter for IMC Prosperity 2 algorithms"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "submit", "submitter"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

