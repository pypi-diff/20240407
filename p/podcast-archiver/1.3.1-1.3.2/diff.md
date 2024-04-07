# Comparing `tmp/podcast_archiver-1.3.1.tar.gz` & `tmp/podcast_archiver-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "podcast_archiver-1.3.1.tar", max compression
+gzip compressed data, was "podcast_archiver-1.3.2.tar", max compression
```

## Comparing `podcast_archiver-1.3.1.tar` & `podcast_archiver-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1056 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/LICENSE
--rw-r--r--   0        0        0     5466 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/README.md
--rw-r--r--   0        0        0       23 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/__init__.py
--rwxr-xr-x   0        0        0     1860 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/base.py
--rw-r--r--   0        0        0     7923 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/cli.py
--rw-r--r--   0        0        0     5661 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/config.py
--rw-r--r--   0        0        0       54 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/console.py
--rw-r--r--   0        0        0      573 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/constants.py
--rw-r--r--   0        0        0     4734 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/download.py
--rw-r--r--   0        0        0      520 2024-04-01 12:47:17.564755 podcast_archiver-1.3.1/podcast_archiver/enums.py
--rw-r--r--   0        0        0      784 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/podcast_archiver/exceptions.py
--rw-r--r--   0        0        0      929 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/podcast_archiver/logging.py
--rw-r--r--   0        0        0     7368 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/podcast_archiver/models.py
--rw-r--r--   0        0        0     4972 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/podcast_archiver/processor.py
--rw-r--r--   0        0        0      806 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/podcast_archiver/quirks.py
--rw-r--r--   0        0        0      152 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/podcast_archiver/session.py
--rw-r--r--   0        0        0     3468 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/podcast_archiver/utils.py
--rw-r--r--   0        0        0     3306 2024-04-01 12:47:17.568755 podcast_archiver-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     6883 1970-01-01 00:00:00.000000 podcast_archiver-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-04-07 14:20:09.440626 podcast_archiver-1.3.2/LICENSE
+-rw-r--r--   0        0        0     5466 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/README.md
+-rw-r--r--   0        0        0       23 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/__init__.py
+-rwxr-xr-x   0        0        0     1860 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/base.py
+-rw-r--r--   0        0        0     7971 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/cli.py
+-rw-r--r--   0        0        0     5661 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/config.py
+-rw-r--r--   0        0        0       54 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/console.py
+-rw-r--r--   0        0        0      573 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/constants.py
+-rw-r--r--   0        0        0     4734 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/download.py
+-rw-r--r--   0        0        0      520 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/enums.py
+-rw-r--r--   0        0        0      784 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/exceptions.py
+-rw-r--r--   0        0        0      929 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/logging.py
+-rw-r--r--   0        0        0     7368 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/models.py
+-rw-r--r--   0        0        0     4972 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/processor.py
+-rw-r--r--   0        0        0      806 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/quirks.py
+-rw-r--r--   0        0        0      152 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/session.py
+-rw-r--r--   0        0        0     3468 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/podcast_archiver/utils.py
+-rw-r--r--   0        0        0     3306 2024-04-07 14:20:09.444626 podcast_archiver-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     6883 1970-01-01 00:00:00.000000 podcast_archiver-1.3.2/PKG-INFO
```

### Comparing `podcast_archiver-1.3.1/LICENSE` & `podcast_archiver-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/README.md` & `podcast_archiver-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/base.py` & `podcast_archiver-1.3.2/podcast_archiver/base.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/cli.py` & `podcast_archiver-1.3.2/podcast_archiver/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,14 +253,15 @@
     "-c",
     "--config",
     "config_path",
     type=ConfigFile(),
     default=get_default_config_path,
     show_default=False,
     is_eager=True,
+    envvar=constants.ENVVAR_PREFIX + "_CONFIG",
     show_envvar=True,
     help="Path to a config file. Command line arguments will take precedence.",
 )
 @click.pass_context
 def main(ctx: click.RichContext, /, **kwargs: Any) -> int:
     configure_logging(kwargs["verbose"])
     console.quiet = kwargs["quiet"] or kwargs["verbose"] > 1
```

### Comparing `podcast_archiver-1.3.1/podcast_archiver/config.py` & `podcast_archiver-1.3.2/podcast_archiver/config.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/constants.py` & `podcast_archiver-1.3.2/podcast_archiver/constants.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/download.py` & `podcast_archiver-1.3.2/podcast_archiver/download.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/enums.py` & `podcast_archiver-1.3.2/podcast_archiver/enums.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/exceptions.py` & `podcast_archiver-1.3.2/podcast_archiver/exceptions.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/logging.py` & `podcast_archiver-1.3.2/podcast_archiver/logging.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/models.py` & `podcast_archiver-1.3.2/podcast_archiver/models.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/processor.py` & `podcast_archiver-1.3.2/podcast_archiver/processor.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/quirks.py` & `podcast_archiver-1.3.2/podcast_archiver/quirks.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/podcast_archiver/utils.py` & `podcast_archiver-1.3.2/podcast_archiver/utils.py`

 * *Files identical despite different names*

### Comparing `podcast_archiver-1.3.1/pyproject.toml` & `podcast_archiver-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "podcast-archiver"
-version = "1.3.1"
+version = "1.3.2"
 description = "Archive all episodes from your favorite podcasts"
 # cspell: disable
 authors = ["Jan Willhaus <mail@janwillhaus.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "podcast_archiver" }]
 classifiers = [
```

### Comparing `podcast_archiver-1.3.1/PKG-INFO` & `podcast_archiver-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: podcast-archiver
-Version: 1.3.1
+Version: 1.3.2
 Summary: Archive all episodes from your favorite podcasts
 Home-page: https://github.com/janw/podcast-archiver
 License: MIT
 Author: Jan Willhaus
 Author-email: mail@janwillhaus.de
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

