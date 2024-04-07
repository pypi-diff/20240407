# Comparing `tmp/cleanpy-0.4.0.tar.gz` & `tmp/cleanpy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanpy-0.4.0.tar", last modified: Sun Feb  5 11:49:58 2023, max compression
+gzip compressed data, was "cleanpy-0.5.0.tar", last modified: Sun Apr  7 09:32:28 2024, max compression
```

## Comparing `cleanpy-0.4.0.tar` & `cleanpy-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 11:49:58.518602 cleanpy-0.4.0/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2021-03-20 04:14:01.000000 cleanpy-0.4.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      179 2021-03-20 04:14:01.000000 cleanpy-0.4.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5887 2023-02-05 11:49:58.518602 cleanpy-0.4.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     4554 2023-02-05 11:06:14.000000 cleanpy-0.4.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 11:49:58.518602 cleanpy-0.4.0/cleanpy/
--rw-r--r--   0 toor      (1000) toor      (1000)       88 2021-03-20 04:14:01.000000 cleanpy-0.4.0/cleanpy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7157 2023-02-05 10:49:46.000000 cleanpy-0.4.0/cleanpy/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-02-05 11:04:30.000000 cleanpy-0.4.0/cleanpy/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4114 2023-02-05 10:33:10.000000 cleanpy-0.4.0/cleanpy/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3231 2023-02-05 10:33:10.000000 cleanpy-0.4.0/cleanpy/_finder.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2836 2021-07-10 10:21:37.000000 cleanpy-0.4.0/cleanpy/_manipulator.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 11:49:58.518602 cleanpy-0.4.0/cleanpy.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5887 2023-02-05 11:49:58.000000 cleanpy-0.4.0/cleanpy.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      456 2023-02-05 11:49:58.000000 cleanpy-0.4.0/cleanpy.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-02-05 11:49:58.000000 cleanpy-0.4.0/cleanpy.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       50 2023-02-05 11:49:58.000000 cleanpy-0.4.0/cleanpy.egg-info/entry_points.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-02-05 11:49:58.000000 cleanpy-0.4.0/cleanpy.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        8 2023-02-05 11:49:58.000000 cleanpy-0.4.0/cleanpy.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      986 2023-02-05 10:55:21.000000 cleanpy-0.4.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 11:49:58.518602 cleanpy-0.4.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2021-03-20 04:14:01.000000 cleanpy-0.4.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       21 2021-03-20 04:14:01.000000 cleanpy-0.4.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-02-05 11:49:58.518602 cleanpy-0.4.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2379 2023-02-05 10:55:09.000000 cleanpy-0.4.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-02-05 11:49:58.518602 cleanpy-0.4.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)     6117 2023-02-05 10:42:08.000000 cleanpy-0.4.0/test/test_cli.py
--rw-r--r--   0 toor      (1000) toor      (1000)      738 2023-02-05 10:56:13.000000 cleanpy-0.4.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 09:32:28.474940 cleanpy-0.5.0/
+-rw-rw-r--   0 root         (0) root         (0)     1074 2024-04-07 09:31:29.000000 cleanpy-0.5.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      161 2024-04-07 09:31:29.000000 cleanpy-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6465 2024-04-07 09:32:28.474940 cleanpy-0.5.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     4970 2024-04-07 09:31:29.000000 cleanpy-0.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 09:32:28.470940 cleanpy-0.5.0/cleanpy/
+-rw-rw-r--   0 root         (0) root         (0)      198 2024-04-07 09:31:29.000000 cleanpy-0.5.0/cleanpy/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7190 2024-04-07 09:31:29.000000 cleanpy-0.5.0/cleanpy/__main__.py
+-rw-rw-r--   0 root         (0) root         (0)      201 2024-04-07 09:31:29.000000 cleanpy-0.5.0/cleanpy/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)     4377 2024-04-07 09:31:29.000000 cleanpy-0.5.0/cleanpy/_const.py
+-rw-rw-r--   0 root         (0) root         (0)     3376 2024-04-07 09:31:29.000000 cleanpy-0.5.0/cleanpy/_finder.py
+-rw-rw-r--   0 root         (0) root         (0)     2836 2024-04-07 09:31:29.000000 cleanpy-0.5.0/cleanpy/_manipulator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 09:32:28.470940 cleanpy-0.5.0/cleanpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6465 2024-04-07 09:32:28.000000 cleanpy-0.5.0/cleanpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      456 2024-04-07 09:32:28.000000 cleanpy-0.5.0/cleanpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 09:32:28.000000 cleanpy-0.5.0/cleanpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-07 09:32:28.000000 cleanpy-0.5.0/cleanpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2024-04-07 09:32:28.000000 cleanpy-0.5.0/cleanpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-07 09:32:28.000000 cleanpy-0.5.0/cleanpy.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1326 2024-04-07 09:31:29.000000 cleanpy-0.5.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 09:32:28.470940 cleanpy-0.5.0/requirements/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-07 09:31:29.000000 cleanpy-0.5.0/requirements/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       28 2024-04-07 09:31:29.000000 cleanpy-0.5.0/requirements/test_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 09:32:28.474940 cleanpy-0.5.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2466 2024-04-07 09:31:29.000000 cleanpy-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 09:32:28.470940 cleanpy-0.5.0/test/
+-rw-rw-r--   0 root         (0) root         (0)     6740 2024-04-07 09:31:29.000000 cleanpy-0.5.0/test/test_cli.py
+-rw-rw-r--   0 root         (0) root         (0)     1031 2024-04-07 09:31:29.000000 cleanpy-0.5.0/tox.ini
```

### Comparing `cleanpy-0.4.0/LICENSE` & `cleanpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanpy-0.4.0/PKG-INFO` & `cleanpy-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cleanpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: cleanpy is a CLI tool to remove caches and temporary files that related to Python.
 Home-page: https://github.com/thombashi/cleanpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/cleanpy/releases
 Project-URL: Source, https://github.com/thombashi/cleanpy
 Project-URL: Tracker, https://github.com/thombashi/cleanpy/issues
 Keywords: cleaner,command
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,54 +24,40 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: subprocrunner>=2.0.1; extra == "test"
 
 .. contents:: **cleanpy**
    :backlinks: top
    :depth: 2
 
-Summary
+Introduction
 ============================================
 ``cleanpy`` is a CLI tool to remove caches and temporary files related to Python.
 
-.. image:: https://badge.fury.io/py/cleanpy.svg
-    :target: https://badge.fury.io/py/cleanpy
-    :alt: PyPI package version
-
-.. image:: https://github.com/thombashi/cleanpy/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/cleanpy/actions/workflows/lint_and_test.yml
-    :alt: CI status of Linux/macOS/Windows
-
-.. image:: https://github.com/thombashi/cleanpy/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/cleanpy/actions/workflows/codeql-analysis.yml
-    :alt: CodeQL
+|PyPI pkg ver| |CI status| |CodeQL|
 
 
 Installation
 ============================================
 
 Installation: pip
 --------------------------------------------
 ::
 
     pip install cleanpy
 
-.. image:: https://img.shields.io/pypi/pyversions/cleanpy.svg
-    :target: https://pypi.org/project/cleanpy
-    :alt: Supported Python versions
-
-.. image:: https://img.shields.io/pypi/implementation/cleanpy.svg
-    :target: https://pypi.org/project/cleanpy
-    :alt: Supported Python implementations
+|Supported Python versions| |Supported Python implementations|
 
 Installation: snap
 --------------------------------------------
 ::
 
     sudo snap install cleanpy
 
@@ -81,54 +68,55 @@
 
 Usage
 ============================================
 ::
 
     cleanpy DIR_PATH [DIR_PATH ...]
 
-``cleanpy`` will remove cache files and temporary files under the DIR_PATH
+``cleanpy`` will remove cache files and temporary files under the ``DIR_PATH``.
 
-Remove files/directories are as follows:
+Removing files or directories targets are as follows:
 
-- files:
+- Files to be deleted:
     - ``*.pyc``
     - ``*.pyo``
 
-- directories:
+- Directories to be deleted:
     - ``__pycache__``
     - ``.cache``
     - ``.mypy_cache``
     - ``.pytest_cache``
+    - ``.ruff_cache``
 
 You can also remove additional files/directories if the following options are specified:
 
 - ``--include-builds``:
-    - ``build``
-    - ``dist``
-    - ``docs/_build``: ``[sphinx]``
-    - ``*.manifest``: ``[pyinstaller]``
-    - ``*.spec``: ``[pyinstaller]``
+    - ``build`` directory
+    - ``dist`` directory
+    - ``docs/_build`` directory: ``[sphinx]``
+    - ``*.manifest`` files: ``[pyinstaller]``
+    - ``*.spec`` files: ``[pyinstaller]``
 - ``--include-envs``:
-    - ``.venv``
-    - ``.nox``
-    - ``.tox``
+    - ``.venv`` directory
+    - ``.nox`` directory
+    - ``.tox`` directory
 - ``--include-metadata``:
-    - ``.eggs``
-    - ``*.egg-info``
-    - ``.pyre/``
-    - ``.pytype/``
-    - ``pip-wheel-metadata``
+    - ``.eggs`` directory
+    - ``*.egg-info`` directories
+    - ``.pyre`` directory
+    - ``.pytype`` directory
+    - ``pip-wheel-metadata`` directory
 - ``--include-testing``:
-    - ``.coverage``
-    - ``coverage.xml``
-    - ``nosetests.xml``
+    - ``.coverage`` file
+    - ``coverage.xml`` file
+    - ``nosetests.xml`` file
 
 All the above options are specified if you use the ``--all`` option.
 
-The following directories are excluded from the remove:
+The following directories are always excluded from the remove:
 
 - ``.git``
 - ``.hg``
 - ``.svn``
 - ``node_modules``
 
 Execution example
@@ -142,15 +130,15 @@
 
 Command help
 --------------------------------------------
 ::
 
     usage: cleanpy [-h] [-V] [--list] [--follow-symlinks] [--dry-run] [-a] [--include-builds] [--include-envs] [--include-metadata] [--include-testing] [--exclude PATTERN] [--exclude-envs] [-i | -f] [-v | --debug | --quiet] DIR_PATH [DIR_PATH ...]
 
-    Remove cache files and temporary files that are related to Python.
+    cleanpy will remove cache files and temporary files under the DIR_PATH.
 
     Skip directories from recursive search: .git, .hg, .svn, node_modules
 
     positional arguments:
       DIR_PATH            path to a root directory to search.
 
     options:
@@ -179,7 +167,28 @@
 
 Dependencies
 ============================================
 Python 3.7+
 
 - no external package dependencies
 - platform independent
+
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/cleanpy.svg
+    :target: https://badge.fury.io/py/cleanpy
+    :alt: PyPI package version
+
+.. |CI status| image:: https://github.com/thombashi/cleanpy/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/cleanpy/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. |CodeQL| image:: https://github.com/thombashi/cleanpy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/cleanpy/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/cleanpy.svg
+    :target: https://pypi.org/project/cleanpy
+    :alt: Supported Python versions
+
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/cleanpy.svg
+    :target: https://pypi.org/project/cleanpy
+    :alt: Supported Python implementations
```

### Comparing `cleanpy-0.4.0/README.rst` & `cleanpy-0.5.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,28 @@
 .. contents:: **cleanpy**
    :backlinks: top
    :depth: 2
 
-Summary
+Introduction
 ============================================
 ``cleanpy`` is a CLI tool to remove caches and temporary files related to Python.
 
-.. image:: https://badge.fury.io/py/cleanpy.svg
-    :target: https://badge.fury.io/py/cleanpy
-    :alt: PyPI package version
-
-.. image:: https://github.com/thombashi/cleanpy/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/cleanpy/actions/workflows/lint_and_test.yml
-    :alt: CI status of Linux/macOS/Windows
-
-.. image:: https://github.com/thombashi/cleanpy/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/cleanpy/actions/workflows/codeql-analysis.yml
-    :alt: CodeQL
+|PyPI pkg ver| |CI status| |CodeQL|
 
 
 Installation
 ============================================
 
 Installation: pip
 --------------------------------------------
 ::
 
     pip install cleanpy
 
-.. image:: https://img.shields.io/pypi/pyversions/cleanpy.svg
-    :target: https://pypi.org/project/cleanpy
-    :alt: Supported Python versions
-
-.. image:: https://img.shields.io/pypi/implementation/cleanpy.svg
-    :target: https://pypi.org/project/cleanpy
-    :alt: Supported Python implementations
+|Supported Python versions| |Supported Python implementations|
 
 Installation: snap
 --------------------------------------------
 ::
 
     sudo snap install cleanpy
 
@@ -49,54 +33,55 @@
 
 Usage
 ============================================
 ::
 
     cleanpy DIR_PATH [DIR_PATH ...]
 
-``cleanpy`` will remove cache files and temporary files under the DIR_PATH
+``cleanpy`` will remove cache files and temporary files under the ``DIR_PATH``.
 
-Remove files/directories are as follows:
+Removing files or directories targets are as follows:
 
-- files:
+- Files to be deleted:
     - ``*.pyc``
     - ``*.pyo``
 
-- directories:
+- Directories to be deleted:
     - ``__pycache__``
     - ``.cache``
     - ``.mypy_cache``
     - ``.pytest_cache``
+    - ``.ruff_cache``
 
 You can also remove additional files/directories if the following options are specified:
 
 - ``--include-builds``:
-    - ``build``
-    - ``dist``
-    - ``docs/_build``: ``[sphinx]``
-    - ``*.manifest``: ``[pyinstaller]``
-    - ``*.spec``: ``[pyinstaller]``
+    - ``build`` directory
+    - ``dist`` directory
+    - ``docs/_build`` directory: ``[sphinx]``
+    - ``*.manifest`` files: ``[pyinstaller]``
+    - ``*.spec`` files: ``[pyinstaller]``
 - ``--include-envs``:
-    - ``.venv``
-    - ``.nox``
-    - ``.tox``
+    - ``.venv`` directory
+    - ``.nox`` directory
+    - ``.tox`` directory
 - ``--include-metadata``:
-    - ``.eggs``
-    - ``*.egg-info``
-    - ``.pyre/``
-    - ``.pytype/``
-    - ``pip-wheel-metadata``
+    - ``.eggs`` directory
+    - ``*.egg-info`` directories
+    - ``.pyre`` directory
+    - ``.pytype`` directory
+    - ``pip-wheel-metadata`` directory
 - ``--include-testing``:
-    - ``.coverage``
-    - ``coverage.xml``
-    - ``nosetests.xml``
+    - ``.coverage`` file
+    - ``coverage.xml`` file
+    - ``nosetests.xml`` file
 
 All the above options are specified if you use the ``--all`` option.
 
-The following directories are excluded from the remove:
+The following directories are always excluded from the remove:
 
 - ``.git``
 - ``.hg``
 - ``.svn``
 - ``node_modules``
 
 Execution example
@@ -110,15 +95,15 @@
 
 Command help
 --------------------------------------------
 ::
 
     usage: cleanpy [-h] [-V] [--list] [--follow-symlinks] [--dry-run] [-a] [--include-builds] [--include-envs] [--include-metadata] [--include-testing] [--exclude PATTERN] [--exclude-envs] [-i | -f] [-v | --debug | --quiet] DIR_PATH [DIR_PATH ...]
 
-    Remove cache files and temporary files that are related to Python.
+    cleanpy will remove cache files and temporary files under the DIR_PATH.
 
     Skip directories from recursive search: .git, .hg, .svn, node_modules
 
     positional arguments:
       DIR_PATH            path to a root directory to search.
 
     options:
@@ -147,7 +132,28 @@
 
 Dependencies
 ============================================
 Python 3.7+
 
 - no external package dependencies
 - platform independent
+
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/cleanpy.svg
+    :target: https://badge.fury.io/py/cleanpy
+    :alt: PyPI package version
+
+.. |CI status| image:: https://github.com/thombashi/cleanpy/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/cleanpy/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. |CodeQL| image:: https://github.com/thombashi/cleanpy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/cleanpy/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/cleanpy.svg
+    :target: https://pypi.org/project/cleanpy
+    :alt: Supported Python versions
+
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/cleanpy.svg
+    :target: https://pypi.org/project/cleanpy
+    :alt: Supported Python implementations
```

### Comparing `cleanpy-0.4.0/cleanpy/__main__.py` & `cleanpy-0.5.0/cleanpy/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,31 +15,32 @@
 
 
 def parse_option() -> Namespace:
     parser = ArgumentParser(
         formatter_class=RawDescriptionHelpFormatter,
         description=dedent(
             """\
-            Remove cache files and temporary files that are related to Python.
+            cleanpy will remove cache files and temporary files under the DIR_PATH.
 
             Skip directories from recursive search: {}
-            """.format(
-                ", ".join(IGNORE_DIRS)
-            )
+            """.format(", ".join(IGNORE_DIRS))
         ),
         epilog=dedent(
             """\
             Issue tracker: https://github.com/thombashi/cleanpy/issues
             """
         ),
     )
     parser.add_argument("-V", "--version", action="version", version="%(prog)s " + __version__)
 
     parser.add_argument(
-        "target_dirs", metavar="DIR_PATH", nargs="+", help="path to a root directory to search."
+        "target_dirs",
+        metavar="DIR_PATH",
+        nargs="+",
+        help="path to a root directory to search.",
     )
 
     parser.add_argument(
         "--list",
         dest="listing",
         action="store_true",
         default=False,
@@ -72,15 +73,18 @@
     group_rm.add_argument(
         "--include-envs",
         action="store_true",
         default=False,
         help="remove virtual environment caches.",
     )
     group_rm.add_argument(
-        "--include-metadata", action="store_true", default=False, help="remove metadata."
+        "--include-metadata",
+        action="store_true",
+        default=False,
+        help="remove metadata.",
     )
     group_rm.add_argument(
         "--include-testing",
         action="store_true",
         default=False,
         help="remove test results and coverage files.",
     )
@@ -202,15 +206,15 @@
             exclude_pattern = f"{options.exclude}|{virtual_env_pattern}"
         else:
             exclude_pattern = virtual_env_pattern
 
     return exclude_pattern
 
 
-def main():
+def main() -> None:
     options = parse_option()
     logger = get_logger(extract_log_level(options.log_level, options.dry_run))
     manipulator = DirEntryManipulator(
         logger,
         interactive=options.interactive,
         follow_symlinks=options.follow_symlinks,
         dry_run=options.dry_run,
```

### Comparing `cleanpy-0.4.0/cleanpy/_const.py` & `cleanpy-0.5.0/cleanpy/_const.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,14 +98,26 @@
                     r"^\.mypy_cache$",
                 ]
             )
         ),
     ),
     RemoveTarget(
         category=Category.CACHE,
+        name="ruff",
+        target_type=EntryType.DIR,
+        regexp=re.compile(
+            "|".join(
+                [
+                    r"^\.ruff_cache$",
+                ]
+            )
+        ),
+    ),
+    RemoveTarget(
+        category=Category.CACHE,
         name="temporary files",
         target_type=EntryType.FILE,
         regexp=re.compile(
             "|".join(
                 [
                     r".+\.py\.[0-9a-z]{32}\.py$",
                 ]
```

### Comparing `cleanpy-0.4.0/cleanpy/_finder.py` & `cleanpy-0.5.0/cleanpy/_finder.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,16 +40,18 @@
             if target.regexp.search(entry.name):
                 self.__logger.debug(
                     f"match remove pattern: path={entry.path}, pattern={target.regexp.pattern}"
                 )
                 return (True, target)
 
         if Category.BUILD in self.__include_categories:
+            # sphinx build path (docs/_build) is a special case
+            # because it is not a single directory name but a path.
             if entry.name == "_build" and SPHINX_BUILD_TARGET.regexp.search(entry.path) is not None:
-                return (True, target)
+                return (True, SPHINX_BUILD_TARGET)
 
         return (False, None)
 
     def is_skip_entry(self, entry: DirEntry) -> bool:
         if self.__exclude_pattern and self.__exclude_pattern.search(entry.name):
             self.__logger.debug(f"match exclude pattern: {entry.path}")
             return True
```

### Comparing `cleanpy-0.4.0/cleanpy/_manipulator.py` & `cleanpy-0.5.0/cleanpy/_manipulator.py`

 * *Files identical despite different names*

### Comparing `cleanpy-0.4.0/cleanpy.egg-info/PKG-INFO` & `cleanpy-0.5.0/cleanpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cleanpy
-Version: 0.4.0
+Version: 0.5.0
 Summary: cleanpy is a CLI tool to remove caches and temporary files that related to Python.
 Home-page: https://github.com/thombashi/cleanpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/cleanpy/releases
 Project-URL: Source, https://github.com/thombashi/cleanpy
 Project-URL: Tracker, https://github.com/thombashi/cleanpy/issues
 Keywords: cleaner,command
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -23,54 +24,40 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE
+Provides-Extra: test
+Requires-Dist: pytest; extra == "test"
+Requires-Dist: subprocrunner>=2.0.1; extra == "test"
 
 .. contents:: **cleanpy**
    :backlinks: top
    :depth: 2
 
-Summary
+Introduction
 ============================================
 ``cleanpy`` is a CLI tool to remove caches and temporary files related to Python.
 
-.. image:: https://badge.fury.io/py/cleanpy.svg
-    :target: https://badge.fury.io/py/cleanpy
-    :alt: PyPI package version
-
-.. image:: https://github.com/thombashi/cleanpy/actions/workflows/lint_and_test.yml/badge.svg
-    :target: https://github.com/thombashi/cleanpy/actions/workflows/lint_and_test.yml
-    :alt: CI status of Linux/macOS/Windows
-
-.. image:: https://github.com/thombashi/cleanpy/actions/workflows/codeql-analysis.yml/badge.svg
-    :target: https://github.com/thombashi/cleanpy/actions/workflows/codeql-analysis.yml
-    :alt: CodeQL
+|PyPI pkg ver| |CI status| |CodeQL|
 
 
 Installation
 ============================================
 
 Installation: pip
 --------------------------------------------
 ::
 
     pip install cleanpy
 
-.. image:: https://img.shields.io/pypi/pyversions/cleanpy.svg
-    :target: https://pypi.org/project/cleanpy
-    :alt: Supported Python versions
-
-.. image:: https://img.shields.io/pypi/implementation/cleanpy.svg
-    :target: https://pypi.org/project/cleanpy
-    :alt: Supported Python implementations
+|Supported Python versions| |Supported Python implementations|
 
 Installation: snap
 --------------------------------------------
 ::
 
     sudo snap install cleanpy
 
@@ -81,54 +68,55 @@
 
 Usage
 ============================================
 ::
 
     cleanpy DIR_PATH [DIR_PATH ...]
 
-``cleanpy`` will remove cache files and temporary files under the DIR_PATH
+``cleanpy`` will remove cache files and temporary files under the ``DIR_PATH``.
 
-Remove files/directories are as follows:
+Removing files or directories targets are as follows:
 
-- files:
+- Files to be deleted:
     - ``*.pyc``
     - ``*.pyo``
 
-- directories:
+- Directories to be deleted:
     - ``__pycache__``
     - ``.cache``
     - ``.mypy_cache``
     - ``.pytest_cache``
+    - ``.ruff_cache``
 
 You can also remove additional files/directories if the following options are specified:
 
 - ``--include-builds``:
-    - ``build``
-    - ``dist``
-    - ``docs/_build``: ``[sphinx]``
-    - ``*.manifest``: ``[pyinstaller]``
-    - ``*.spec``: ``[pyinstaller]``
+    - ``build`` directory
+    - ``dist`` directory
+    - ``docs/_build`` directory: ``[sphinx]``
+    - ``*.manifest`` files: ``[pyinstaller]``
+    - ``*.spec`` files: ``[pyinstaller]``
 - ``--include-envs``:
-    - ``.venv``
-    - ``.nox``
-    - ``.tox``
+    - ``.venv`` directory
+    - ``.nox`` directory
+    - ``.tox`` directory
 - ``--include-metadata``:
-    - ``.eggs``
-    - ``*.egg-info``
-    - ``.pyre/``
-    - ``.pytype/``
-    - ``pip-wheel-metadata``
+    - ``.eggs`` directory
+    - ``*.egg-info`` directories
+    - ``.pyre`` directory
+    - ``.pytype`` directory
+    - ``pip-wheel-metadata`` directory
 - ``--include-testing``:
-    - ``.coverage``
-    - ``coverage.xml``
-    - ``nosetests.xml``
+    - ``.coverage`` file
+    - ``coverage.xml`` file
+    - ``nosetests.xml`` file
 
 All the above options are specified if you use the ``--all`` option.
 
-The following directories are excluded from the remove:
+The following directories are always excluded from the remove:
 
 - ``.git``
 - ``.hg``
 - ``.svn``
 - ``node_modules``
 
 Execution example
@@ -142,15 +130,15 @@
 
 Command help
 --------------------------------------------
 ::
 
     usage: cleanpy [-h] [-V] [--list] [--follow-symlinks] [--dry-run] [-a] [--include-builds] [--include-envs] [--include-metadata] [--include-testing] [--exclude PATTERN] [--exclude-envs] [-i | -f] [-v | --debug | --quiet] DIR_PATH [DIR_PATH ...]
 
-    Remove cache files and temporary files that are related to Python.
+    cleanpy will remove cache files and temporary files under the DIR_PATH.
 
     Skip directories from recursive search: .git, .hg, .svn, node_modules
 
     positional arguments:
       DIR_PATH            path to a root directory to search.
 
     options:
@@ -179,7 +167,28 @@
 
 Dependencies
 ============================================
 Python 3.7+
 
 - no external package dependencies
 - platform independent
+
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/cleanpy.svg
+    :target: https://badge.fury.io/py/cleanpy
+    :alt: PyPI package version
+
+.. |CI status| image:: https://github.com/thombashi/cleanpy/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/cleanpy/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
+
+.. |CodeQL| image:: https://github.com/thombashi/cleanpy/actions/workflows/github-code-scanning/codeql/badge.svg
+    :target: https://github.com/thombashi/cleanpy/actions/workflows/github-code-scanning/codeql
+    :alt: CodeQL
+
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/cleanpy.svg
+    :target: https://pypi.org/project/cleanpy
+    :alt: Supported Python versions
+
+.. |Supported Python implementations| image:: https://img.shields.io/pypi/implementation/cleanpy.svg
+    :target: https://pypi.org/project/cleanpy
+    :alt: Supported Python implementations
```

### Comparing `cleanpy-0.4.0/pyproject.toml` & `cleanpy-0.5.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [build-system]
-requires = ["setuptools", "wheel"]
+build-backend = "setuptools.build_meta"
+requires = ["setuptools>=61.0"]
 
 [tool.black]
-line-length = 100
 exclude = '''
 /(
       \.eggs
     | \.git
     | \.mypy_cache
     | \.tox
     | \.venv
@@ -14,48 +14,72 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
+line-length = 100
 target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.coverage.run]
-source = ['cleanpy']
 branch = true
+source = ['cleanpy']
 
 [tool.coverage.report]
-show_missing = true
-precision = 1
 exclude_lines = [
-    'except ImportError',
-    'raise NotImplementedError',
-    'pass',
-    'ABCmeta',
-    'abstractmethod',
-    'abstractproperty',
-    'abstractclassmethod',
-    'warnings.warn',
+  'except ImportError',
+  'raise NotImplementedError',
+  'pass',
+  'ABCmeta',
+  'abstractmethod',
+  'abstractproperty',
+  'abstractclassmethod',
+  'warnings.warn',
 ]
+precision = 1
+show_missing = true
 
 [tool.isort]
-known_third_party = [
-]
 include_trailing_comma = true
+known_third_party = []
 line_length = 100
 lines_after_imports = 2
 multi_line_output = 3
 skip_glob = [
-    '*/.eggs/*',
-    '*/.pytype/*',
-    '*/.tox/*',
+  '*/.eggs/*',
+  '*/.pytype/*',
+  '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.7
+python_version = "3.7"
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unused_configs = true
+
+[tool.pyright]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    ".tox",
+    ".venv",
+    "_build",
+    "_sandbox",
+    "build",
+    "dist"
+]
+pythonVersion = "3.7"
+
+[tool.ruff]
+line-length = 100
+target-version = "py37"
+exclude = [
+    ".eggs/",
+    ".tox/",
+    "_sandbox/*",
+    "build/",
+    "docs/conf.py",
+]
```

### Comparing `cleanpy-0.4.0/setup.py` & `cleanpy-0.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "cleanpy"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 ENCODING = "utf8"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -41,15 +41,19 @@
     ),
     include_package_data=True,
     keywords=["cleaner", "command"],
     license=pkg_info["__license__"],
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
-    project_urls={"Source": REPOSITORY_URL, "Tracker": f"{REPOSITORY_URL:s}/issues"},
+    project_urls={
+        "Changlog": f"{REPOSITORY_URL:s}/releases",
+        "Source": REPOSITORY_URL,
+        "Tracker": f"{REPOSITORY_URL:s}/issues",
+    },
     python_requires=">=3.7",
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

### Comparing `cleanpy-0.4.0/test/test_cli.py` & `cleanpy-0.5.0/test/test_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         p.write("dummy")
 
         runner = SubprocessRunner([MODULE, "-f", str(tmpdir), "-v"])
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed 1 directories", runner.stderr) is not None
         assert re.search("removed 1 files", runner.stderr) is not None
 
     def test_normal_multi_dir(self, tmpdir):
         first_dir = tmpdir.mkdir("first")
         first_dir.mkdir("__pycache__")
         first_dir.mkdir("build")
@@ -53,51 +54,62 @@
         second_dir.mkdir("__pycache__")
 
         runner = SubprocessRunner([MODULE, "-f", str(first_dir), str(second_dir), "-v"])
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed 2 directories", runner.stderr) is not None
 
     def test_normal_exclude(self, tmpdir):
         p = tmpdir.mkdir("__pycache__").join("dummy.pyc")
         p.write("dummy")
 
         p = tmpdir.join("test.pyc")
         p.write("dummy")
 
         runner = SubprocessRunner([MODULE, "-f", str(tmpdir), "--exclude", "__pycache__", "-v"])
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed [0-9]+ directories", runner.stderr) is None
         assert re.search("removed 1 files", runner.stderr) is not None
 
     def test_normal_include_builds(self, tmpdir):
         first_dir, second_dir = make_dirs(tmpdir)
         runner = SubprocessRunner(
-            [MODULE, "-f", str(first_dir), str(second_dir), "--debug", "--include-builds"]
+            [
+                MODULE,
+                "-f",
+                str(first_dir),
+                str(second_dir),
+                "--debug",
+                "--include-builds",
+            ]
         )
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed 3 directories", runner.stderr) is not None
 
     def test_normal_include_envs(self, tmpdir):
         first_dir, second_dir = make_dirs(tmpdir)
         runner = SubprocessRunner(
             [MODULE, "-f", str(first_dir), str(second_dir), "--debug", "--include-envs"]
         )
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed 3 directories", runner.stderr) is not None
 
     def test_normal_exclude_envs_with_exclude_pattern(self, tmpdir):
         first_dir, second_dir = make_dirs(tmpdir)
         runner = SubprocessRunner(
             [
                 MODULE,
@@ -110,56 +122,75 @@
                 "__pycache__",
             ]
         )
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed [0-9]+ directories", runner.stderr) is None
 
     def test_normal_include_metadata(self, tmpdir):
         first_dir, second_dir = make_dirs(tmpdir)
         runner = SubprocessRunner(
-            [MODULE, "-f", str(first_dir), str(second_dir), "--debug", "--include-metadata"]
+            [
+                MODULE,
+                "-f",
+                str(first_dir),
+                str(second_dir),
+                "--debug",
+                "--include-metadata",
+            ]
         )
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed 3 directories", runner.stderr) is not None
 
     def test_normal_include_tests(self, tmpdir):
         first_dir, second_dir = make_dirs(tmpdir)
         runner = SubprocessRunner(
-            [MODULE, "-f", str(first_dir), str(second_dir), "--debug", "--include-testing"]
+            [
+                MODULE,
+                "-f",
+                str(first_dir),
+                str(second_dir),
+                "--debug",
+                "--include-testing",
+            ]
         )
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed 2 directories", runner.stderr) is not None
         assert re.search("removed 1 files", runner.stderr) is not None
 
     def test_normal_all(self, tmpdir):
         first_dir, second_dir = make_dirs(tmpdir)
         runner = SubprocessRunner([MODULE, "-f", str(first_dir), str(second_dir), "--debug", "-a"])
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stderr
         assert re.search("removed 5 directories", runner.stderr) is not None
         assert re.search("removed 1 files", runner.stderr) is not None
 
     def test_normal_list(self, tmpdir):
         first_dir, second_dir = make_dirs(tmpdir)
         runner = SubprocessRunner([MODULE, "--list", str(first_dir), str(second_dir), "-a"])
         assert runner.run() == 0, runner.stderr
 
         print_result(stdout=runner.stdout, stderr=runner.stderr)
 
+        assert runner.stdout
         targets = runner.stdout.splitlines()
         assert len(targets) == 6
         for target in targets:
             assert str(tmpdir) in target
 
 
 def make_dirs(dir_obj):
```

### Comparing `cleanpy-0.4.0/tox.ini` & `cleanpy-0.5.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -10,35 +10,53 @@
 extras =
     test
 commands =
     pytest {posargs}
 
 [testenv:build]
 deps =
+    build>=1
     twine
     wheel
 commands =
-    python setup.py sdist bdist_wheel
+    python -m build
     twine check dist/*
 
-[testenv:fmt]
+[testenv:fmt-black]
 skip_install = true
 deps =
-    autoflake>=1.4
-    black>=22.1
+    autoflake>=2
+    black>=24.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
     isort .
     black setup.py test cleanpy
 
-[testenv:lint]
+[testenv:fmt]
 skip_install = true
 deps =
+    autoflake>=2
+    isort>=5
+    ruff>=0.3.5
+commands =
+    autoflake --in-place --recursive --remove-all-unused-imports --ignore-init-module-imports .
+    isort .
+    ruff format
+
+[testenv:lint]
+extras =
+    test
+deps =
     codespell
-    mypy>=0.931
-    pylama>=8.3.6
+    mypy>=1
+    releasecmd
+    ; pylama>=8.4.1
+    pyright>=1.1
+    ruff>=0.3.5
 commands =
-    python setup.py check
     codespell cleanpy test README.rst -q2 --check-filenames -L temporaly
     mypy cleanpy setup.py
-    pylama
+    ; pylama
+    pyright
+    ruff format --check
+    ruff check
```

