# Comparing `tmp/podcast_archiver-1.3.2.tar.gz` & `tmp/podcast_archiver-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_archiver-1.3.2.tar", max compression
+gzip compressed data, was "podcast_archiver-1.3.3.tar", max compression
```

## Comparing `podcast_archiver-1.3.2.tar` & `podcast_archiver-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1056 2024-04-07 14:20:09.440626 podcast_archiver-1.3.2/LICENSE
--rw-r--r--   0        0        0     5466 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/README.md
--rw-r--r--   0        0        0       23 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/__init__.py
--rwxr-xr-x   0        0        0     1860 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/base.py
--rw-r--r--   0        0        0     7971 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/cli.py
--rw-r--r--   0        0        0     5661 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/config.py
--rw-r--r--   0        0        0       54 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/console.py
--rw-r--r--   0        0        0      573 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/constants.py
--rw-r--r--   0        0        0     4734 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/download.py
--rw-r--r--   0        0        0      520 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/enums.py
--rw-r--r--   0        0        0      784 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/exceptions.py
--rw-r--r--   0        0        0      929 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/logging.py
--rw-r--r--   0        0        0     7368 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/models.py
--rw-r--r--   0        0        0     4972 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/processor.py
--rw-r--r--   0        0        0      806 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/quirks.py
--rw-r--r--   0        0        0      152 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/session.py
--rw-r--r--   0        0        0     3468 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/utils.py
--rw-r--r--   0        0        0     3306 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     6883 1970-01-01 00:00:00.000000 podcast_archiver-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-07 15:34:30.202453 podcast_archiver-1.3.3/LICENSE
+-rw-r--r--   0        0        0     5550 2024-04-07 15:34:30.202453 podcast_archiver-1.3.3/README.md
+-rw-r--r--   0        0        0       23 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/__init__.py
+-rwxr-xr-x   0        0        0     1860 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/base.py
+-rw-r--r--   0        0        0     7971 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/cli.py
+-rw-r--r--   0        0        0     5661 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/config.py
+-rw-r--r--   0        0        0       54 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/console.py
+-rw-r--r--   0        0        0      573 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/constants.py
+-rw-r--r--   0        0        0     4734 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/download.py
+-rw-r--r--   0        0        0      520 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/enums.py
+-rw-r--r--   0        0        0      784 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/exceptions.py
+-rw-r--r--   0        0        0      929 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/logging.py
+-rw-r--r--   0        0        0     7368 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/models.py
+-rw-r--r--   0        0        0     4972 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/processor.py
+-rw-r--r--   0        0        0      806 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/quirks.py
+-rw-r--r--   0        0        0      152 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/session.py
+-rw-r--r--   0        0        0     3468 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/podcast_archiver/utils.py
+-rw-r--r--   0        0        0     3306 2024-04-07 15:34:30.206453 podcast_archiver-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     6967 1970-01-01 00:00:00.000000 podcast_archiver-1.3.3/PKG-INFO
```

### Comparing `podcast_archiver-1.3.2/LICENSE` & `podcast_archiver-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/README.md` & `podcast_archiver-1.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
 Or use it via Docker:
 
 ```bash
 docker run --tty --rm ghcr.io/janw/podcast-archiver --help
 ```
 
+By default, the docker image downloads episodes to a volume mounted at `/archive`.
+
 ## Usage
 
 Run `podcast-archiver --help` for details on how to use it:
 
 <!-- RICH-CODEX fake_command: "podcast-archiver --help" -->
 ![`poetry run podcast-archiver --help`](.assets/podcast-archiver-help.svg)
```

### Comparing `podcast_archiver-1.3.2/podcast_archiver/base.py` & `podcast_archiver-1.3.3/podcast_archiver/base.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/cli.py` & `podcast_archiver-1.3.3/podcast_archiver/cli.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/config.py` & `podcast_archiver-1.3.3/podcast_archiver/config.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/constants.py` & `podcast_archiver-1.3.3/podcast_archiver/constants.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/download.py` & `podcast_archiver-1.3.3/podcast_archiver/download.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/enums.py` & `podcast_archiver-1.3.3/podcast_archiver/enums.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/exceptions.py` & `podcast_archiver-1.3.3/podcast_archiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/logging.py` & `podcast_archiver-1.3.3/podcast_archiver/logging.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/models.py` & `podcast_archiver-1.3.3/podcast_archiver/models.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/processor.py` & `podcast_archiver-1.3.3/podcast_archiver/processor.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/quirks.py` & `podcast_archiver-1.3.3/podcast_archiver/quirks.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/podcast_archiver/utils.py` & `podcast_archiver-1.3.3/podcast_archiver/utils.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.2/pyproject.toml` & `podcast_archiver-1.3.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "podcast-archiver"
-version = "1.3.2"
+version = "1.3.3"
 description = "Archive all episodes from your favorite podcasts"
 # cspell: disable
 authors = ["Jan Willhaus <mail@janwillhaus.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "podcast_archiver" }]
 classifiers = [
```

### Comparing `podcast_archiver-1.3.2/PKG-INFO` & `podcast_archiver-1.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-archiver
-Version: 1.3.2
+Version: 1.3.3
 Summary: Archive all episodes from your favorite podcasts
 Home-page: https://github.com/janw/podcast-archiver
 License: MIT
 Author: Jan Willhaus
 Author-email: mail@janwillhaus.de
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -79,14 +79,16 @@
 
 Or use it via Docker:
 
 ```bash
 docker run --tty --rm ghcr.io/janw/podcast-archiver --help
 ```
 
+By default, the docker image downloads episodes to a volume mounted at `/archive`.
+
 ## Usage
 
 Run `podcast-archiver --help` for details on how to use it:
 
 <!-- RICH-CODEX fake_command: "podcast-archiver --help" -->
 ![`poetry run podcast-archiver --help`](.assets/podcast-archiver-help.svg)
```

