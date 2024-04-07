# Comparing `tmp/DateTimeRange-2.2.0.tar.gz` & `tmp/DateTimeRange-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DateTimeRange-2.2.0.tar", last modified: Tue Oct  3 16:00:39 2023, max compression
+gzip compressed data, was "DateTimeRange-2.2.1.tar", last modified: Sun Apr  7 14:55:50 2024, max compression
```

## Comparing `DateTimeRange-2.2.0.tar` & `DateTimeRange-2.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.478905 DateTimeRange-2.2.0/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/DateTimeRange.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     9391 2023-10-03 16:00:39.000000 DateTimeRange-2.2.0/DateTimeRange.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      536 2023-10-03 16:00:39.000000 DateTimeRange-2.2.0/DateTimeRange.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-10-03 16:00:39.000000 DateTimeRange-2.2.0/DateTimeRange.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-10-03 16:00:04.000000 DateTimeRange-2.2.0/DateTimeRange.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)      148 2023-10-03 16:00:39.000000 DateTimeRange-2.2.0/DateTimeRange.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       14 2023-10-03 16:00:39.000000 DateTimeRange-2.2.0/DateTimeRange.egg-info/top_level.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1084 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      223 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     9391 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     7368 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/README.rst
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/datetimerange/
--rw-r--r--   0 toor      (1000) toor      (1000)      325 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/datetimerange/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/datetimerange/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    33411 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/datetimerange/_core.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/datetimerange/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/docs/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/docs/pages/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/docs/pages/introduction/
--rw-r--r--   0 toor      (1000) toor      (1000)      214 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/docs/pages/introduction/summary.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1191 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)       36 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/requirements/docs_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       53 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-10-03 16:00:39.478905 DateTimeRange-2.2.0/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     3138 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-10-03 16:00:39.468905 DateTimeRange-2.2.0/test/
--rw-r--r--   0 toor      (1000) toor      (1000)    49325 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/test/test_dtr.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1225 2023-10-03 15:59:48.000000 DateTimeRange-2.2.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/DateTimeRange.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9753 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      536 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 14:55:42.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-07 14:55:50.000000 DateTimeRange-2.2.1/DateTimeRange.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1084 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      205 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9753 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     7565 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/datetimerange/
+-rw-rw-r--   0 root         (0) root         (0)      325 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      201 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/__version__.py
+-rw-rw-r--   0 root         (0) root         (0)    33749 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/_core.py
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/datetimerange/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.325921 DateTimeRange-2.2.1/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.325921 DateTimeRange-2.2.1/docs/pages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/docs/pages/introduction/
+-rw-rw-r--   0 root         (0) root         (0)      214 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/docs/pages/introduction/summary.txt
+-rw-rw-r--   0 root         (0) root         (0)     1517 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/requirements/
+-rw-rw-r--   0 root         (0) root         (0)       64 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/requirements/docs_requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       53 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/requirements/requirements.txt
+-rw-rw-r--   0 root         (0) root         (0)       41 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/requirements/test_requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3190 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 14:55:50.329921 DateTimeRange-2.2.1/test/
+-rw-rw-r--   0 root         (0) root         (0)    49719 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/test/test_dtr.py
+-rw-rw-r--   0 root         (0) root         (0)     1523 2024-04-07 14:54:20.000000 DateTimeRange-2.2.1/tox.ini
```

### Comparing `DateTimeRange-2.2.0/DateTimeRange.egg-info/PKG-INFO` & `DateTimeRange-2.2.1/DateTimeRange.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: DateTimeRange
-Version: 2.2.0
+Version: 2.2.1
 Summary: DateTimeRange is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 Home-page: https://github.com/thombashi/DateTimeRange
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/DateTimeRange/releases
 Project-URL: Documentation, https://datetimerange.rtfd.io/
 Project-URL: Funding, https://github.com/sponsors/thombashi
 Project-URL: Source, https://github.com/thombashi/DateTimeRange
 Project-URL: Tracker, https://github.com/thombashi/DateTimeRange/issues
 Keywords: datetimerange,datetime,time range
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,50 +31,54 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: python-dateutil<3,>=2.4.2
 Requires-Dist: typepy[datetime]<2,>=1.3.2
 Provides-Extra: docs
+Requires-Dist: path>=13; extra == "docs"
+Requires-Dist: readmemaker>=1.1.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.2.2; extra == "docs"
 Requires-Dist: Sphinx>=2.4; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0.1; extra == "test"
-Requires-Dist: pytest-md-report>=0.4.1; extra == "test"
+Requires-Dist: pytest-md-report>=0.5; extra == "test"
 Requires-Dist: pytz; extra == "test"
 
 .. contents:: **DateTimeRange**
    :backlinks: top
    :depth: 2
 
 Summary
 =========
 `DateTimeRange <https://github.com/thombashi/DateTimeRange>`__ is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 
-.. image:: https://badge.fury.io/py/DateTimeRange.svg
+|PyPI pkg ver| |conda pkg ver| |Supported Python versions| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/DateTimeRange.svg
     :target: https://badge.fury.io/py/DateTimeRange
     :alt: PyPI package version
 
-.. image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
+.. |conda pkg ver| image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
     :target: https://anaconda.org/conda-forge/datetimerange
     :alt: conda-forge package version
 
-.. image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
     :target: https://pypi.org/project/DateTimeRange
     :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/DateTimeRange/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/DateTimeRange/actions/workflows/tests.yml
-    :alt: Test result of Linux/macOS/Windows
+.. |CI status| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/DateTimeRange/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/DateTimeRange/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/DateTimeRange?branch=master
     :alt: Test coverage
 
-.. image:: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql/badge.svg
+.. |CodeQL| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql/badge.svg
     :target: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Installation
 ============
 
 Installation: pip
```

### Comparing `DateTimeRange-2.2.0/DateTimeRange.egg-info/SOURCES.txt` & `DateTimeRange-2.2.1/DateTimeRange.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DateTimeRange-2.2.0/LICENSE` & `DateTimeRange-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DateTimeRange-2.2.0/PKG-INFO` & `DateTimeRange-2.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: DateTimeRange
-Version: 2.2.0
+Version: 2.2.1
 Summary: DateTimeRange is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 Home-page: https://github.com/thombashi/DateTimeRange
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
+Project-URL: Changlog, https://github.com/thombashi/DateTimeRange/releases
 Project-URL: Documentation, https://datetimerange.rtfd.io/
 Project-URL: Funding, https://github.com/sponsors/thombashi
 Project-URL: Source, https://github.com/thombashi/DateTimeRange
 Project-URL: Tracker, https://github.com/thombashi/DateTimeRange/issues
 Keywords: datetimerange,datetime,time range
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -30,50 +31,54 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: python-dateutil<3,>=2.4.2
 Requires-Dist: typepy[datetime]<2,>=1.3.2
 Provides-Extra: docs
+Requires-Dist: path>=13; extra == "docs"
+Requires-Dist: readmemaker>=1.1.0; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.2.2; extra == "docs"
 Requires-Dist: Sphinx>=2.4; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=6.0.1; extra == "test"
-Requires-Dist: pytest-md-report>=0.4.1; extra == "test"
+Requires-Dist: pytest-md-report>=0.5; extra == "test"
 Requires-Dist: pytz; extra == "test"
 
 .. contents:: **DateTimeRange**
    :backlinks: top
    :depth: 2
 
 Summary
 =========
 `DateTimeRange <https://github.com/thombashi/DateTimeRange>`__ is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 
-.. image:: https://badge.fury.io/py/DateTimeRange.svg
+|PyPI pkg ver| |conda pkg ver| |Supported Python versions| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/DateTimeRange.svg
     :target: https://badge.fury.io/py/DateTimeRange
     :alt: PyPI package version
 
-.. image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
+.. |conda pkg ver| image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
     :target: https://anaconda.org/conda-forge/datetimerange
     :alt: conda-forge package version
 
-.. image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
     :target: https://pypi.org/project/DateTimeRange
     :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/DateTimeRange/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/DateTimeRange/actions/workflows/tests.yml
-    :alt: Test result of Linux/macOS/Windows
+.. |CI status| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/DateTimeRange/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/DateTimeRange/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/DateTimeRange?branch=master
     :alt: Test coverage
 
-.. image:: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql/badge.svg
+.. |CodeQL| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql/badge.svg
     :target: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Installation
 ============
 
 Installation: pip
```

### Comparing `DateTimeRange-2.2.0/README.rst` & `DateTimeRange-2.2.1/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,37 @@
    :backlinks: top
    :depth: 2
 
 Summary
 =========
 `DateTimeRange <https://github.com/thombashi/DateTimeRange>`__ is a Python library to handle a time range. e.g. check whether a time is within the time range, get the intersection of time ranges, truncate a time range, iterate through a time range, and so forth.
 
-.. image:: https://badge.fury.io/py/DateTimeRange.svg
+|PyPI pkg ver| |conda pkg ver| |Supported Python versions| |CI status| |Test coverage| |CodeQL|
+
+.. |PyPI pkg ver| image:: https://badge.fury.io/py/DateTimeRange.svg
     :target: https://badge.fury.io/py/DateTimeRange
     :alt: PyPI package version
 
-.. image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
+.. |conda pkg ver| image:: https://anaconda.org/conda-forge/datetimerange/badges/version.svg
     :target: https://anaconda.org/conda-forge/datetimerange
     :alt: conda-forge package version
 
-.. image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
+.. |Supported Python versions| image:: https://img.shields.io/pypi/pyversions/DateTimeRange.svg
     :target: https://pypi.org/project/DateTimeRange
     :alt: Supported Python versions
 
-.. image:: https://github.com/thombashi/DateTimeRange/workflows/Tests/badge.svg
-    :target: https://github.com/thombashi/DateTimeRange/actions/workflows/tests.yml
-    :alt: Test result of Linux/macOS/Windows
+.. |CI status| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml/badge.svg
+    :target: https://github.com/thombashi/DateTimeRange/actions/workflows/ci.yml
+    :alt: CI status of Linux/macOS/Windows
 
-.. image:: https://coveralls.io/repos/github/thombashi/DateTimeRange/badge.svg?branch=master
+.. |Test coverage| image:: https://coveralls.io/repos/github/thombashi/DateTimeRange/badge.svg?branch=master
     :target: https://coveralls.io/github/thombashi/DateTimeRange?branch=master
     :alt: Test coverage
 
-.. image:: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql/badge.svg
+.. |CodeQL| image:: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql/badge.svg
     :target: https://github.com/thombashi/DateTimeRange/actions/workflows/github-code-scanning/codeql
     :alt: CodeQL
 
 Installation
 ============
 
 Installation: pip
```

### Comparing `DateTimeRange-2.2.0/datetimerange/_core.py` & `DateTimeRange-2.2.1/datetimerange/_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,19 +170,21 @@
 
         return DateTimeRange(start_datetime, end_datetime)
 
     def __iadd__(self, other: Union[datetime.timedelta, rdelta.relativedelta]) -> "DateTimeRange":
         if self.start_datetime is None and self.end_datetime is None:
             raise TypeError("range is not set")
 
+        timezone = self.timezone
+
         if self.start_datetime:
-            self.set_start_datetime(self.start_datetime + other)
+            self.set_start_datetime(self.start_datetime + other, timezone)
 
         if self.end_datetime:
-            self.set_end_datetime(self.end_datetime + other)
+            self.set_end_datetime(self.end_datetime + other, timezone)
 
         return self
 
     def __sub__(self, other: Union[datetime.timedelta, rdelta.relativedelta]) -> "DateTimeRange":
         if self.start_datetime is None and self.end_datetime is None:
             raise TypeError("range is not set")
 
@@ -196,19 +198,21 @@
 
         return DateTimeRange(start_datetime, end_datetime)
 
     def __isub__(self, other: Union[datetime.timedelta, rdelta.relativedelta]) -> "DateTimeRange":
         if self.start_datetime is None and self.end_datetime is None:
             raise TypeError("range is not set")
 
+        timezone = self.timezone
+
         if self.start_datetime:
-            self.set_start_datetime(self.start_datetime - other)
+            self.set_start_datetime(self.start_datetime - other, timezone)
 
         if self.end_datetime:
-            self.set_end_datetime(self.end_datetime - other)
+            self.set_end_datetime(self.end_datetime - other, timezone)
 
         return self
 
     def __contains__(self, x: Union[datetime.datetime, "DateTimeRange", str]) -> bool:
         """
         :param x:
             |datetime|/``DateTimeRange`` instance to compare.
@@ -727,16 +731,22 @@
             start_datetime = max(self.start_datetime, x.start_datetime)
             end_datetime = min(self.end_datetime, x.end_datetime)
         else:
             start_datetime = None
             end_datetime = None
 
         if intersection_threshold is not None:
-            assert start_datetime is not None
-            assert end_datetime is not None
+            if start_datetime is None or end_datetime is None:
+                return DateTimeRange(
+                    start_datetime=None,
+                    end_datetime=None,
+                    start_time_format=self.start_time_format,
+                    end_time_format=self.end_time_format,
+                )
+
             delta = end_datetime - start_datetime
 
             if (
                 _compare_relativedelta(
                     _to_norm_relativedelta(delta),
                     _to_norm_relativedelta(intersection_threshold),
                 )
```

### Comparing `DateTimeRange-2.2.0/pyproject.toml` & `DateTimeRange-2.2.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   '*/.eggs/*',
   '*/.pytype/*',
   '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.7
+python_version = "3.7"
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
 
@@ -68,7 +68,31 @@
   "test",
 ]
 
 md_report = true
 md_report_color = "auto"
 md_report_margin = 0
 md_report_verbose = 1
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
+line-length = 120
+target-version = "py37"
+exclude = [
+    ".eggs/",
+    ".tox/",
+    "_sandbox/*",
+    "build/",
+    "docs/conf.py",
+]
```

### Comparing `DateTimeRange-2.2.0/setup.py` & `DateTimeRange-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
     include_package_data=True,
     keywords=["datetimerange", "datetime", "time range"],
     license=pkg_info["__license__"],
     long_description=long_description,
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     project_urls={
+        "Changlog": f"{REPOSITORY_URL:s}/releases",
         "Documentation": f"https://{MODULE_NAME.lower():s}.rtfd.io/",
         "Funding": "https://github.com/sponsors/thombashi",
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
     python_requires=">=3.7",
     install_requires=install_requires,
```

### Comparing `DateTimeRange-2.2.0/test/test_dtr.py` & `DateTimeRange-2.2.1/test/test_dtr.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,46 +26,50 @@
     import locale
 
     locale.setlocale(locale.LC_ALL, ("C", "ascii"))
 
 
 @pytest.fixture
 def datetimerange_normal():
-    value = DateTimeRange(TEST_START_DATETIME, TEST_END_DATETIME)
-    value.start_time_format = ISO_TIME_FORMAT
-    value.end_time_format = ISO_TIME_FORMAT
-
-    return value
+    return DateTimeRange(
+        TEST_START_DATETIME,
+        TEST_END_DATETIME,
+        start_time_format=ISO_TIME_FORMAT,
+        end_time_format=ISO_TIME_FORMAT,
+    )
 
 
 @pytest.fixture
 def datetimerange_inversion():
-    value = DateTimeRange(TEST_END_DATETIME, TEST_START_DATETIME)
-    value.start_time_format = ISO_TIME_FORMAT
-    value.end_time_format = ISO_TIME_FORMAT
-
-    return value
+    return DateTimeRange(
+        TEST_END_DATETIME,
+        TEST_START_DATETIME,
+        start_time_format=ISO_TIME_FORMAT,
+        end_time_format=ISO_TIME_FORMAT,
+    )
 
 
 @pytest.fixture
 def datetimerange_null():
-    value = DateTimeRange(None, None)
-    value.time_format = None
-    value.end_time_format = None
-
-    return value
+    return DateTimeRange(
+        None,
+        None,
+        start_time_format=None,
+        end_time_format=None,
+    )
 
 
 @pytest.fixture
 def datetimerange_null_start():
-    value = DateTimeRange(None, TEST_END_DATETIME)
-    value.time_format = None
-    value.end_time_format = ISO_TIME_FORMAT
-
-    return value
+    return DateTimeRange(
+        None,
+        TEST_END_DATETIME,
+        start_time_format=None,
+        end_time_format=ISO_TIME_FORMAT,
+    )
 
 
 class TestDateTimeRange_repr:
     @pytest.mark.parametrize(
         ["start", "start_format", "end", "end_format", "separator", "is_output_elapse", "expected"],
         [
             [
@@ -323,15 +327,19 @@
         new_datetimerange = value + add_value
 
         assert new_datetimerange == expected
         assert value != new_datetimerange
 
     @pytest.mark.parametrize(
         ["value", "expected"],
-        [["2015-03-22T10:10:00+0900", TypeError], [1, TypeError], [None, TypeError]],
+        [
+            ["2015-03-22T10:10:00+0900", TypeError],
+            [1, TypeError],
+            [None, TypeError],
+        ],
     )
     def test_exception(self, datetimerange_normal, value, expected):
         with pytest.raises(TypeError):
             datetimerange_normal + value
 
     def test_null(self, datetimerange_null):
         with pytest.raises(TypeError):
@@ -606,15 +614,15 @@
                     datetime(2015, 3, 22, 18, 0, 0),
                     datetime(2015, 3, 22, 12, 0, 0),
                     datetime(2015, 3, 22, 6, 0, 0),
                     datetime(2015, 3, 22, 0, 0, 0),
                 ],
             ],
             [
-                DateTimeRange(date(2015, 3, 23), date(2015, 3, 26)),
+                DateTimeRange(datetime(2015, 3, 23), datetime(2015, 3, 26)),
                 relativedelta(days=+1),
                 [
                     datetime(2015, 3, 23, 0, 0, 0),
                     datetime(2015, 3, 24, 0, 0, 0),
                     datetime(2015, 3, 25, 0, 0, 0),
                     datetime(2015, 3, 26, 0, 0, 0),
                 ],
@@ -736,14 +744,21 @@
             ],
             [
                 DateTimeRange("2015-01-22T09:50:00 JST", "2015-01-22T10:00:01 JST"),
                 DateTimeRange("2015-01-22T10:00:00 JST", "2015-03-22T10:20:00 JST"),
                 timedelta(seconds=1),
                 True,
             ],
+            [
+                # https://github.com/thombashi/DateTimeRange/issues/48
+                DateTimeRange("2015-03-22T10:00:00+0900", "2015-03-22T10:10:00+0900"),
+                DateTimeRange("2015-03-23T10:05:00+0900", "2015-03-23T10:15:00+0900"),
+                timedelta(seconds=1),
+                False,
+            ],
         ],
     )
     def test_normal_w_intersection_threshold(self, lhs, rhs, threshold, expected):
         lhs_org = deepcopy(lhs)
 
         assert lhs.is_intersection(rhs, threshold) == expected
         assert lhs == lhs_org
```

### Comparing `DateTimeRange-2.2.0/tox.ini` & `DateTimeRange-2.2.1/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -39,38 +39,55 @@
 
 [testenv:docs]
 extras =
     docs
 commands =
     sphinx-build docs/ docs/_build
 
-[testenv:fmt]
+[testenv:fmt-black]
 skip_install = true
 deps =
     autoflake>=2
-    black[jupyter]>=23.1
+    black[jupyter]>=24.1
     isort>=5
 commands =
     autoflake --in-place --recursive --remove-all-unused-imports .
     isort .
     black setup.py docs/ datetimerange/ examples/ test/
 
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
+    docs
+    test
+deps =
     codespell
     mypy>=1
-    pylama>=8.4.1
+    releasecmd
+    ; pylama>=8.4.1
+    pyright>=1.1
+    ruff>=0.3.5
     types-python-dateutil
 commands =
     mypy datetimerange/ setup.py
+    pyright
     -codespell -q2 --check-filenames docs/pages datetimerange/ examples/ test/ README.rst
-    pylama
+    ; pylama
+    ruff format --check
+    ruff check
 
 [testenv:readme]
-skip_install = true
 changedir = docs
-deps =
-    path
-    readmemaker>=1.1.0
+extras =
+    docs
 commands =
     python make_readme.py
```

