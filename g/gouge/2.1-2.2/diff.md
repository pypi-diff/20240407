# Comparing `tmp/gouge-2.1.tar.gz` & `tmp/gouge-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gouge-2.1.tar", last modified: Sat Mar 16 10:39:39 2024, max compression
+gzip compressed data, was "gouge-2.2.tar", last modified: Sun Apr  7 09:02:00 2024, max compression
```

## Comparing `gouge-2.1.tar` & `gouge-2.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.620861 gouge-2.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.612861 gouge-2.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-03-16 10:39:32.000000 gouge-2.1/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-16 10:39:32.000000 gouge-2.1/.devcontainer/init.bash
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.616861 gouge-2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-16 10:39:32.000000 gouge-2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.616861 gouge-2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-16 10:39:32.000000 gouge-2.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-16 10:39:32.000000 gouge-2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-16 10:39:32.000000 gouge-2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-16 10:39:32.000000 gouge-2.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.616861 gouge-2.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-16 10:39:32.000000 gouge-2.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-16 10:39:32.000000 gouge-2.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-16 10:39:39.620861 gouge-2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-16 10:39:32.000000 gouge-2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.616861 gouge-2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:32.000000 gouge-2.1/docs/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-03-16 10:39:32.000000 gouge-2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.616861 gouge-2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:32.000000 gouge-2.1/docs/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-03-16 10:39:32.000000 gouge-2.1/docs/_static/pre-formatter-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-03-16 10:39:32.000000 gouge-2.1/docs/_static/pre-formatter-not-applied.png
--rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-03-16 10:39:32.000000 gouge-2.1/docs/_static/snapshot1.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.616861 gouge-2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:32.000000 gouge-2.1/docs/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-16 10:39:32.000000 gouge-2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-03-16 10:39:32.000000 gouge-2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-03-16 10:39:32.000000 gouge-2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-16 10:39:32.000000 gouge-2.1/fabfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-16 10:39:32.000000 gouge-2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-16 10:39:39.620861 gouge-2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.612861 gouge-2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.616861 gouge-2.1/src/gouge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:32.000000 gouge-2.1/src/gouge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-03-16 10:39:32.000000 gouge-2.1/src/gouge/colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-03-16 10:39:32.000000 gouge-2.1/src/gouge/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-03-16 10:39:32.000000 gouge-2.1/src/gouge/parseable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-03-16 10:39:32.000000 gouge-2.1/src/gouge/preformatters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:32.000000 gouge-2.1/src/gouge/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.620861 gouge-2.1/src/gouge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-03-16 10:39:39.000000 gouge-2.1/src/gouge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-03-16 10:39:39.000000 gouge-2.1/src/gouge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-16 10:39:39.000000 gouge-2.1/src/gouge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-16 10:39:39.000000 gouge-2.1/src/gouge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-16 10:39:39.000000 gouge-2.1/src/gouge.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-16 10:39:39.620861 gouge-2.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-16 10:39:32.000000 gouge-2.1/test/test_caplog.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-16 10:39:32.000000 gouge-2.1/test/test_coloring.py
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-03-16 10:39:32.000000 gouge-2.1/test/test_colourcli.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-03-16 10:39:32.000000 gouge-2.1/test/test_preformatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-03-16 10:39:32.000000 gouge-2.1/test/test_shifting_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.497964 gouge-2.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.493965 gouge-2.2/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-07 09:01:54.000000 gouge-2.2/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-07 09:01:54.000000 gouge-2.2/.devcontainer/init.bash
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.493965 gouge-2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-07 09:01:54.000000 gouge-2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.493965 gouge-2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-07 09:01:54.000000 gouge-2.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-07 09:01:54.000000 gouge-2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-07 09:01:54.000000 gouge-2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-07 09:01:54.000000 gouge-2.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.493965 gouge-2.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 09:01:54.000000 gouge-2.2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-07 09:01:54.000000 gouge-2.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-07 09:02:00.497964 gouge-2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-07 09:01:54.000000 gouge-2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.493965 gouge-2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:01:54.000000 gouge-2.2/docs/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-07 09:01:54.000000 gouge-2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.493965 gouge-2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:01:54.000000 gouge-2.2/docs/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)    46724 2024-04-07 09:01:54.000000 gouge-2.2/docs/_static/pre-formatter-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45528 2024-04-07 09:01:54.000000 gouge-2.2/docs/_static/pre-formatter-not-applied.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31000 2024-04-07 09:01:54.000000 gouge-2.2/docs/_static/snapshot1.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.493965 gouge-2.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:01:54.000000 gouge-2.2/docs/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-07 09:01:54.000000 gouge-2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-04-07 09:01:54.000000 gouge-2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6782 2024-04-07 09:01:54.000000 gouge-2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-07 09:01:54.000000 gouge-2.2/fabfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-07 09:01:54.000000 gouge-2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:02:00.497964 gouge-2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.489965 gouge-2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.497964 gouge-2.2/src/gouge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:01:54.000000 gouge-2.2/src/gouge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-07 09:01:54.000000 gouge-2.2/src/gouge/colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-07 09:01:54.000000 gouge-2.2/src/gouge/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-07 09:01:54.000000 gouge-2.2/src/gouge/parseable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-07 09:01:54.000000 gouge-2.2/src/gouge/preformatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 09:01:54.000000 gouge-2.2/src/gouge/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.497964 gouge-2.2/src/gouge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-07 09:02:00.000000 gouge-2.2/src/gouge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-07 09:02:00.000000 gouge-2.2/src/gouge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:02:00.000000 gouge-2.2/src/gouge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 09:02:00.000000 gouge-2.2/src/gouge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 09:02:00.000000 gouge-2.2/src/gouge.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:02:00.497964 gouge-2.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-07 09:01:54.000000 gouge-2.2/test/test_caplog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-07 09:01:54.000000 gouge-2.2/test/test_coloring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-04-07 09:01:54.000000 gouge-2.2/test/test_colourcli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-07 09:01:54.000000 gouge-2.2/test/test_preformatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5601 2024-04-07 09:01:54.000000 gouge-2.2/test/test_shifting_filter.py
```

### Comparing `gouge-2.1/.devcontainer/devcontainer.json` & `gouge-2.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gouge-2.1/.github/workflows/main.yml` & `gouge-2.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gouge-2.1/.gitignore` & `gouge-2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gouge-2.1/.pre-commit-config.yaml` & `gouge-2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gouge-2.1/PKG-INFO` & `gouge-2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.1
+Version: 2.2
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.1/README.rst` & `gouge-2.2/README.rst`

 * *Files identical despite different names*

### Comparing `gouge-2.1/docs/Makefile` & `gouge-2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gouge-2.1/docs/_static/pre-formatter-applied.png` & `gouge-2.2/docs/_static/pre-formatter-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.1/docs/_static/pre-formatter-not-applied.png` & `gouge-2.2/docs/_static/pre-formatter-not-applied.png`

 * *Files identical despite different names*

### Comparing `gouge-2.1/docs/_static/snapshot1.png` & `gouge-2.2/docs/_static/snapshot1.png`

 * *Files identical despite different names*

### Comparing `gouge-2.1/docs/changelog.rst` & `gouge-2.2/docs/changelog.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changelog
 =========
 
+Version 2.2
+-----------
+
+* Provide new keyword-argument ``highlighted_path`` to visually distinguish
+  traceback elements which are path of a subtree. It defaults to
+  ``<current-working-directory>/src`` if it exists.
+
+  This helps reading tracebacks when using complex frameworks (like SQLAlchemy,
+  Flask, Starlette, ...).
+
 Version 2.1
 -----------
 
 * Added support for pre-formatters.
 * Provide bundled pre-formatter for ``uvicorn.access`` via
   ``gouge.preformatters``
```

### Comparing `gouge-2.1/docs/conf.py` & `gouge-2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gouge-2.1/docs/index.rst` & `gouge-2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gouge-2.1/fabfile.py` & `gouge-2.2/fabfile.py`

 * *Files identical despite different names*

### Comparing `gouge-2.1/pyproject.toml` & `gouge-2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gouge"
-version = "2.1"
+version = "2.2"
 authors = [
     {name = "Michel Albert", email = "michel@albert.lu"},
 ]
 description = "Collection of logging formatters."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {text = "BSD-3-Clause"}
```

### Comparing `gouge-2.1/src/gouge/colourcli.py` & `gouge-2.2/src/gouge/colourcli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 """
 This module contains everything needed to emit colourful messages on the CLI
 """
 
 import logging
+import re
 import sys
 from logging import Handler, LogRecord
+from pathlib import Path
 from typing import Any, Callable, Dict, List, Mapping, Optional
 
 import colorama as clr
 
+P_FILENAME = re.compile(r"File \"([^\"]+)\", line (\d+), in ([^\s]+)")
+
 
 class Simple(logging.Formatter):
     """
     Fancy, colorised log output adding ANSI escape codes to the log output.
 
     :params show_threads: Whether to display thread names or not.
     :params show_exc: Whether to display tracebacks or not.
@@ -27,23 +31,29 @@
 
     @staticmethod
     def basicConfig(
         show_exc: bool = True,
         show_threads: bool = False,
         force_styling: bool = False,
         show_pid: bool = False,
+        highlighted_path: Optional[Path] = None,
         **kwargs: Any,
     ) -> List[Handler]:
         """
         Convenience method to have a one-liner set-up.
 
         *show_exc*, *show_threads*, *show_pid* and *force_styling* are directly
         passed to :py:class:`~.Simple`. The remaining *kwargs* are passed on to
         :py:func:`logging.basicConfig`.
 
+        If *highlighted_path* is set, it will highlight local filenames in
+        tracebacks. This is useful if you want to highlight the current working
+        directory. If a "src" directory exists in the current working directory,
+        it will be used as the default.
+
         After returning from :py:func:`logging.basicConfig`, it will fetch the
         *stderr* and *stdout* handlers and replace the formatter.
 
         The function also returns a list of all handlers which have been
         modified. This is useful if you want to modify the handlers any further
         (for example using :py:class:`~gouge.filters.ShiftingFilter`).
         """
@@ -61,14 +71,15 @@
                 continue
 
             handler.setFormatter(
                 Simple(
                     show_exc=show_exc,
                     show_threads=show_threads,
                     show_pid=show_pid,
+                    highlighted_path=highlighted_path,
                 )
             )
             output.append(handler)
         return output
 
     def __init__(
         self,
@@ -79,36 +90,32 @@
         *,
         defaults: Optional[Mapping[str, Any]] = None,
         show_exc: bool = False,
         show_threads: bool = False,
         force_styling: bool = False,
         show_pid: bool = False,
         pre_formatters: Optional[Dict[str, List[Callable[[str], str]]]] = None,
+        highlighted_path: Optional[Path] = None,
     ):
         python_310_args = {"defaults": defaults, "validate": validate}
         if sys.version_info < (3, 10):
             python_310_args.pop("defaults")
         if sys.version_info < (3, 8):
             python_310_args.pop("validate")
         super().__init__(fmt, datefmt, style, **python_310_args)
         self.show_threads = show_threads
         self.show_exc = show_exc
         self.force_styling = force_styling
         self.show_pid = show_pid
         self.pre_formatters = pre_formatters or {}
-
-    def colorised_exception(self, level: int, exc_text: str) -> str:
-        """
-        Colorises the exception text based on log level
-        """
-        if level >= logging.ERROR:
-            output = "\n{f.RED}{exc_text}{s.RESET_ALL}"
+        self.highlighted_path = highlighted_path
+        if (Path.cwd() / "src").exists():
+            self.highlighted_path = Path.cwd() / "src"
         else:
-            output = "\n{f.WHITE}{s.DIM}{exc_text}{s.RESET_ALL}"
-        return output
+            self.highlighted_path = None
 
     def format(self, record: LogRecord) -> str:
         if record.levelno <= logging.DEBUG:
             colorize = clr.Style.BRIGHT + clr.Fore.BLACK
         elif record.levelno <= logging.INFO:
             colorize = clr.Fore.CYAN
         elif record.levelno <= logging.WARNING:
@@ -146,14 +153,36 @@
                 # (it's constant anyway)
                 exc_text = getattr(record, "exc_text", "")
                 if not exc_text:
                     record.exc_text = self.formatException(record.exc_info)
 
             exc_text = getattr(record, "exc_text", "")
             if exc_text:
-                message_template += self.colorised_exception(
-                    record.levelno, exc_text
-                )
+                if record.levelno >= logging.ERROR:
+                    message_template += "\n{f.RED}"
+                else:
+                    message_template += "\n{f.WHITE}{s.DIM}"
+                message_template += self.formatException(record.exc_info)
+                message_template += "{s.RESET_ALL}"
 
         return message_template.format(
             levelcolor=colorize, f=clr.Fore, s=clr.Style, **vars(record)
         )
+
+    def formatException(self, exc_info: tuple) -> str:
+        exc_text = super().formatException(exc_info)
+        if self.highlighted_path is None:
+            return exc_text
+
+        pth = self.highlighted_path
+
+        def highlight_local_filenames(match: re.Match) -> str:
+            filename = Path(match.group(1))
+            if filename.is_relative_to(pth):
+                return match.group(0).replace(
+                    match.group(1),
+                    f"{clr.Fore.YELLOW}{match.group(1)}{clr.Fore.RED}",
+                )
+            return match.group(0)
+
+        exc_text = P_FILENAME.sub(highlight_local_filenames, exc_text)
+        return exc_text
```

### Comparing `gouge-2.1/src/gouge/filters.py` & `gouge-2.2/src/gouge/filters.py`

 * *Files identical despite different names*

### Comparing `gouge-2.1/src/gouge/parseable.py` & `gouge-2.2/src/gouge/parseable.py`

 * *Files identical despite different names*

### Comparing `gouge-2.1/src/gouge/preformatters.py` & `gouge-2.2/src/gouge/preformatters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import re
+
 from gouge.colourcli import clr
 
 P_UVICORN_ACCESS = re.compile(
-    r'^(?P<remote_host>\S+) - "(?P<method>GET|POST|PUT|DELETE|PATCH|HEAD|OPTIONS) (?P<path>\S+) (?P<http>\S+)" (?P<status>\d+)'
+    r'^(?P<remote_host>\S+) - "'
+    r"(?P<method>GET|POST|PUT|DELETE|PATCH|HEAD|OPTIONS) "
+    r'(?P<path>\S+) (?P<http>\S+)" (?P<status>\d+)'
 )
 METHOD_COLORS = {
     "GET": clr.Fore.GREEN,
     "POST": clr.Fore.YELLOW,
     "PUT": clr.Fore.YELLOW,
     "DELETE": clr.Fore.RED,
     "PATCH": clr.Fore.YELLOW,
```

### Comparing `gouge-2.1/src/gouge.egg-info/PKG-INFO` & `gouge-2.2/src/gouge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gouge
-Version: 2.1
+Version: 2.2
 Summary: Collection of logging formatters.
 Author-email: Michel Albert <michel@albert.lu>
 License: BSD-3-Clause
 Project-URL: Repository, https://github.com/exhuma/gouge
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `gouge-2.1/src/gouge.egg-info/SOURCES.txt` & `gouge-2.2/src/gouge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gouge-2.1/test/test_coloring.py` & `gouge-2.2/test/test_coloring.py`

 * *Files identical despite different names*

### Comparing `gouge-2.1/test/test_colourcli.py` & `gouge-2.2/test/test_colourcli.py`

 * *Files identical despite different names*

### Comparing `gouge-2.1/test/test_shifting_filter.py` & `gouge-2.2/test/test_shifting_filter.py`

 * *Files identical despite different names*

