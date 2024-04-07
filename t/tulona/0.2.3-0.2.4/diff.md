# Comparing `tmp/tulona-0.2.3.tar.gz` & `tmp/tulona-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tulona-0.2.3.tar", last modified: Sat Apr  6 15:10:31 2024, max compression
+gzip compressed data, was "tulona-0.2.4.tar", last modified: Sun Apr  7 05:17:15 2024, max compression
```

## Comparing `tulona-0.2.3.tar` & `tulona-0.2.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.279014 tulona-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-06 15:10:27.000000 tulona-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-06 15:10:31.279014 tulona-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-04-06 15:10:27.000000 tulona-0.2.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.271014 tulona-0.2.3/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.275014 tulona-0.2.3/core/tulona/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.275014 tulona-0.2.3/core/tulona/adapter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.275014 tulona-0.2.3/core/tulona/adapter/base/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/adapter/base/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/adapter/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/adapter/mssql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/adapter/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/adapter/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/adapter/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.275014 tulona-0.2.3/core/tulona/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/cli/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.275014 tulona-0.2.3/core/tulona/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.275014 tulona-0.2.3/core/tulona/task/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/task/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/task/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/task/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/task/test_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.279014 tulona-0.2.3/core/tulona/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/profiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-06 15:10:27.000000 tulona-0.2.3/core/tulona/util/yaml_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:10:31.279014 tulona-0.2.3/core/tulona.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-06 15:10:31.000000 tulona-0.2.3/core/tulona.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 15:10:31.000000 tulona-0.2.3/core/tulona.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:10:31.000000 tulona-0.2.3/core/tulona.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-06 15:10:31.000000 tulona-0.2.3/core/tulona.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-06 15:10:31.000000 tulona-0.2.3/core/tulona.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-06 15:10:31.000000 tulona-0.2.3/core/tulona.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-06 15:10:27.000000 tulona-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:10:31.279014 tulona-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.498631 tulona-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-07 05:17:10.000000 tulona-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-07 05:17:15.498631 tulona-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-04-07 05:17:10.000000 tulona-0.2.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.494631 tulona-0.2.4/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.494631 tulona-0.2.4/core/tulona/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.494631 tulona-0.2.4/core/tulona/adapter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.494631 tulona-0.2.4/core/tulona/adapter/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/adapter/base/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/adapter/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/adapter/mssql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/adapter/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/adapter/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/adapter/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.498631 tulona-0.2.4/core/tulona/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/cli/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.498631 tulona-0.2.4/core/tulona/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.498631 tulona-0.2.4/core/tulona/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13431 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/task/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/task/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8011 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/task/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/task/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.498631 tulona-0.2.4/core/tulona/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3515 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/profiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-07 05:17:10.000000 tulona-0.2.4/core/tulona/util/yaml_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 05:17:15.498631 tulona-0.2.4/core/tulona.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9274 2024-04-07 05:17:15.000000 tulona-0.2.4/core/tulona.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-07 05:17:15.000000 tulona-0.2.4/core/tulona.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 05:17:15.000000 tulona-0.2.4/core/tulona.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 05:17:15.000000 tulona-0.2.4/core/tulona.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-07 05:17:15.000000 tulona-0.2.4/core/tulona.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 05:17:15.000000 tulona-0.2.4/core/tulona.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-04-07 05:17:10.000000 tulona-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 05:17:15.498631 tulona-0.2.4/setup.cfg
```

### Comparing `tulona-0.2.3/LICENSE` & `tulona-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/PKG-INFO` & `tulona-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -29,17 +29,25 @@
 Requires-Dist: pyodbc~=5.1
 Requires-Dist: pandas~=1.5
 Requires-Dist: openpyxl~=3.1
 Requires-Dist: Jinja2~=3.1
 
 Tulona
 ======
-A utility to compare tables, espacially useful perform validations for migration projects.
+A utility to compare tables, espacially useful to perform validations for migration projects.
 
-|Build Status| |Coverage|
+.. list-table::
+   :widths: 50 200
+
+   * - Testing
+     - |CI Test| |Deployment| |Coverage|
+   * - Package
+     - |PyPI Latest Release| |PyPI Downloads|
+   * - Meta
+     - |License Apache-2.0| |Codestyle Black|
 
 
 Connection Profiles
 -------------------
 Connection profiles is a `yaml` file that will store credentials and other details to connect to the databases/data sources.
 
 It must be setup in `profiles.yml` file and it must be placed under `$HOME/.tulona` dierctory.
@@ -145,29 +153,33 @@
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
+* **ping**: To test connectivity to the databases for the datasources. Sample command:
+
+  * To ping one data source pass the name to the `--datasources` parameter:
+
+    ``tulona ping --datasources employee_postgres``
+
+  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
+
+    ``tulona ping --datasources employee_postgres,employee_mysql``
+
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
-* **test-connection**: To test connectivity to the databases for the datasources. Sample command:
-
-  * One or more datasources can be passed to the `--datasources` parameter separated by commas:
-
-    ``tulona test-connection --datasources employee_postgres,employee_mysql``
-
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Development Environment Setup
 -----------------------------
 * For live installation execute `pip install --editable core`.
 
@@ -177,12 +189,22 @@
 * Execute `python -m build`.
 
 Install wheel executable file
 -----------------------------
 * Execute `pip install <wheel-file.whl>`
 
 
-.. |Build Status| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
+.. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
+   :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
+.. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
 .. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
    :target: https://codecov.io/gh/mrinalsardar/tulona
    :alt: Coverage status
+.. |PyPI Latest Release| image:: https://img.shields.io/pypi/v/tulona.svg
+   :target: https://pypi.python.org/pypi/tulona/
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/tulona.svg?label=PyPI%20downloads
+   :target: https://pypi.org/project/tulona/
+.. |License Apache-2.0| image:: https://img.shields.io/:license-Apache%202-brightgreen.svg
+   :target: http://www.apache.org/licenses/LICENSE-2.0.txt
+.. |Codestyle Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
```

### Comparing `tulona-0.2.3/README.rst` & `tulona-0.2.4/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 Tulona
 ======
-A utility to compare tables, espacially useful perform validations for migration projects.
+A utility to compare tables, espacially useful to perform validations for migration projects.
 
-|Build Status| |Coverage|
+.. list-table::
+   :widths: 50 200
+
+   * - Testing
+     - |CI Test| |Deployment| |Coverage|
+   * - Package
+     - |PyPI Latest Release| |PyPI Downloads|
+   * - Meta
+     - |License Apache-2.0| |Codestyle Black|
 
 
 Connection Profiles
 -------------------
 Connection profiles is a `yaml` file that will store credentials and other details to connect to the databases/data sources.
 
 It must be setup in `profiles.yml` file and it must be placed under `$HOME/.tulona` dierctory.
@@ -112,29 +120,33 @@
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
+* **ping**: To test connectivity to the databases for the datasources. Sample command:
+
+  * To ping one data source pass the name to the `--datasources` parameter:
+
+    ``tulona ping --datasources employee_postgres``
+
+  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
+
+    ``tulona ping --datasources employee_postgres,employee_mysql``
+
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
-* **test-connection**: To test connectivity to the databases for the datasources. Sample command:
-
-  * One or more datasources can be passed to the `--datasources` parameter separated by commas:
-
-    ``tulona test-connection --datasources employee_postgres,employee_mysql``
-
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Development Environment Setup
 -----------------------------
 * For live installation execute `pip install --editable core`.
 
@@ -144,12 +156,22 @@
 * Execute `python -m build`.
 
 Install wheel executable file
 -----------------------------
 * Execute `pip install <wheel-file.whl>`
 
 
-.. |Build Status| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
+.. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
+   :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
+.. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
 .. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
    :target: https://codecov.io/gh/mrinalsardar/tulona
-   :alt: Coverage status
+   :alt: Coverage status
+.. |PyPI Latest Release| image:: https://img.shields.io/pypi/v/tulona.svg
+   :target: https://pypi.python.org/pypi/tulona/
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/tulona.svg?label=PyPI%20downloads
+   :target: https://pypi.org/project/tulona/
+.. |License Apache-2.0| image:: https://img.shields.io/:license-Apache%202-brightgreen.svg
+   :target: http://www.apache.org/licenses/LICENSE-2.0.txt
+.. |Codestyle Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
```

### Comparing `tulona-0.2.3/core/tulona/adapter/connection.py` & `tulona-0.2.4/core/tulona/adapter/connection.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/adapter/mssql.py` & `tulona-0.2.4/core/tulona/adapter/mssql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/adapter/mysql.py` & `tulona-0.2.4/core/tulona/adapter/mysql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/adapter/postgres.py` & `tulona-0.2.4/core/tulona/adapter/postgres.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/adapter/snowflake.py` & `tulona-0.2.4/core/tulona/adapter/snowflake.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/cli/base.py` & `tulona-0.2.4/core/tulona/cli/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 from tulona.cli import params as p
 from tulona.config.profile import Profile
 from tulona.config.project import Project
 from tulona.config.runtime import RunConfig
 from tulona.exceptions import TulonaMissingArgumentError
 from tulona.task.compare import CompareColumnTask, CompareDataTask
-from tulona.task.profile import ProfileTask
 
 # from tulona.task.scan import ScanTask
-from tulona.task.test_connection import TestConnectionTask
+from tulona.task.ping import PingTask
+from tulona.task.profile import ProfileTask
 
 log = logging.getLogger(__name__)
 logging.basicConfig(
     level=logging.DEBUG,  # TODO: Set level to INFO once verbosity is fixed
     format="[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s",
 )
 
@@ -30,27 +30,27 @@
     epilog="Execute: tulona <command> -h/--help for more help with specific commands",
 )
 @click.pass_context
 def cli(ctx):
     """Tulona compares data sources to find out differences"""
 
 
-# command: tulona test-connection
-@cli.command("test-connection")
+# command: tulona ping
+@cli.command("ping")
 @click.pass_context
 @p.exec_engine
 @p.outdir
 @p.verbose
 @p.datasources
-def test_connection(ctx, **kwargs):
+def ping(ctx, **kwargs):
     """Test connectivity to datasources"""
 
     if "datasources" not in kwargs:
         raise TulonaMissingArgumentError(
-            "--datasources argument must be provided with command: test-connection"
+            "--datasources argument must be provided with command: ping"
         )
 
     if kwargs["verbose"]:
         # TODO: Fix me
         # This setting doesn't enable debug level logging
         handler = logging.StreamHandler()
         handler.setLevel(logging.DEBUG)
@@ -60,15 +60,15 @@
 
     ctx.obj = ctx.obj or {}
     ctx.obj["project"] = proj.load_project_config()
     ctx.obj["profile"] = prof.load_profile_config()[ctx.obj["project"]["name"]]
 
     datasource_list = kwargs["datasources"].split(",")
 
-    task = TestConnectionTask(ctx.obj["profile"], ctx.obj["project"], datasource_list)
+    task = PingTask(ctx.obj["profile"], ctx.obj["project"], datasource_list)
     task.execute()
 
 
 # # command: tulona scan
 # @cli.command("scan")
 # @click.pass_context
 # @p.exec_engine
```

### Comparing `tulona-0.2.3/core/tulona/cli/params.py` & `tulona-0.2.4/core/tulona/cli/params.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/config/profile.py` & `tulona-0.2.4/core/tulona/config/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/config/project.py` & `tulona-0.2.4/core/tulona/config/project.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/exceptions.py` & `tulona-0.2.4/core/tulona/exceptions.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/task/base.py` & `tulona-0.2.4/core/tulona/task/base.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/task/compare.py` & `tulona-0.2.4/core/tulona/task/compare.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/task/profile.py` & `tulona-0.2.4/core/tulona/task/profile.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/task/scan.py` & `tulona-0.2.4/core/tulona/task/scan.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/task/test_connection.py` & `tulona-0.2.4/core/tulona/task/ping.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from tulona.task.base import BaseTask
 from tulona.util.profiles import get_connection_profile
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
-class TestConnectionTask(BaseTask):
+class PingTask(BaseTask):
     profile: Dict
     project: Dict
     datasources: List[str]
 
     def execute(self):
 
-        log.info("Starting task: Test Connection")
+        log.info("Starting task: Ping")
         start_time = time.time()
 
         for ds in self.datasources:
             log.debug(f"Testing connection to data source: {ds}")
 
             connection_profile = get_connection_profile(self.profile, self.project, ds)
             try:
@@ -32,9 +32,9 @@
                     ).fetchone()
                     _ = results[0]
                     log.info("Connection successful")
             except Exception as exp:
                 log.error(f"Connection to data source {ds} failed because of: {exp}")
 
         end_time = time.time()
-        log.info("Finished task: Test Connection")
-        log.info(f"Total time taken: {end_time - start_time} seconds")
+        log.info("Finished task: Ping")
+        log.info(f"Total time taken: {(end_time - start_time):.2f} seconds")
```

### Comparing `tulona-0.2.3/core/tulona/util/database.py` & `tulona-0.2.4/core/tulona/util/database.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/util/dataframe.py` & `tulona-0.2.4/core/tulona/util/dataframe.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/util/excel.py` & `tulona-0.2.4/core/tulona/util/excel.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/util/filesystem.py` & `tulona-0.2.4/core/tulona/util/filesystem.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/util/profiles.py` & `tulona-0.2.4/core/tulona/util/profiles.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona/util/sql.py` & `tulona-0.2.4/core/tulona/util/sql.py`

 * *Files identical despite different names*

### Comparing `tulona-0.2.3/core/tulona.egg-info/PKG-INFO` & `tulona-0.2.4/core/tulona.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tulona
-Version: 0.2.3
+Version: 0.2.4
 Summary: A tool to compare data from different sources.
 Author: Mrinal Kanti Sardar
 Project-URL: Homepage, https://github.com/mrinalsardar/tulona
 Project-URL: Documentation, https://github.com/mrinalsardar/tulona
 Project-URL: Repository, https://github.com/mrinalsardar/tulona.git
 Project-URL: Issues, https://github.com/mrinalsardar/tulona/issues
 Keywords: tulona,comparison,data comparison,database scan,database profile
@@ -29,17 +29,25 @@
 Requires-Dist: pyodbc~=5.1
 Requires-Dist: pandas~=1.5
 Requires-Dist: openpyxl~=3.1
 Requires-Dist: Jinja2~=3.1
 
 Tulona
 ======
-A utility to compare tables, espacially useful perform validations for migration projects.
+A utility to compare tables, espacially useful to perform validations for migration projects.
 
-|Build Status| |Coverage|
+.. list-table::
+   :widths: 50 200
+
+   * - Testing
+     - |CI Test| |Deployment| |Coverage|
+   * - Package
+     - |PyPI Latest Release| |PyPI Downloads|
+   * - Meta
+     - |License Apache-2.0| |Codestyle Black|
 
 
 Connection Profiles
 -------------------
 Connection profiles is a `yaml` file that will store credentials and other details to connect to the databases/data sources.
 
 It must be setup in `profiles.yml` file and it must be placed under `$HOME/.tulona` dierctory.
@@ -145,29 +153,33 @@
   * Command without `--sample-count` parameter:
 
     ``tulona compare-data --datasources employee_postgres,employee_mysql``
   * Command with `--sample-count` parameter:
 
     ``tulona compare-data --sample-count 50 --datasources employee_postgres,employee_mysql``
 
+* **ping**: To test connectivity to the databases for the datasources. Sample command:
+
+  * To ping one data source pass the name to the `--datasources` parameter:
+
+    ``tulona ping --datasources employee_postgres``
+
+  * More than one datasources can be passed to the `--datasources` parameter separated by commas:
+
+    ``tulona ping --datasources employee_postgres,employee_mysql``
+
 * **profile**: To extract and compare metadata of two sources/tables. It includes metadata from `information_schema` related to the tables and some column level metrics (min, max, average, count & distinct_count). Sample commands:
 
   * Profiling without `--compare` flag. It will write metadata and metrics about different sources/tables in different sheets/tabs in the excel file (not a comparison view):
 
     ``tulona profile --datasources employee_postgres,employee_mysql``
   * Profiling with `--compare` flag. It will produce a comparison view (side by side):
 
     ``tulona profile --compare --datasources employee_postgres,employee_mysql``
 
-* **test-connection**: To test connectivity to the databases for the datasources. Sample command:
-
-  * One or more datasources can be passed to the `--datasources` parameter separated by commas:
-
-    ``tulona test-connection --datasources employee_postgres,employee_mysql``
-
 To know more about any specific command, execute `tulona <command> -h`.
 
 
 Development Environment Setup
 -----------------------------
 * For live installation execute `pip install --editable core`.
 
@@ -177,12 +189,22 @@
 * Execute `python -m build`.
 
 Install wheel executable file
 -----------------------------
 * Execute `pip install <wheel-file.whl>`
 
 
-.. |Build Status| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
+.. |CI Test| image:: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml/badge.svg
+   :target: https://github.com/mrinalsardar/tulona/actions/workflows/test.yaml
+.. |Deployment| image:: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml/badge.svg
    :target: https://github.com/mrinalsardar/tulona/actions/workflows/publish.yaml
 .. |Coverage| image:: https://codecov.io/gh/mrinalsardar/tulona/graph/badge.svg?token=UGNjjgRskE
    :target: https://codecov.io/gh/mrinalsardar/tulona
    :alt: Coverage status
+.. |PyPI Latest Release| image:: https://img.shields.io/pypi/v/tulona.svg
+   :target: https://pypi.python.org/pypi/tulona/
+.. |PyPI Downloads| image:: https://img.shields.io/pypi/dm/tulona.svg?label=PyPI%20downloads
+   :target: https://pypi.org/project/tulona/
+.. |License Apache-2.0| image:: https://img.shields.io/:license-Apache%202-brightgreen.svg
+   :target: http://www.apache.org/licenses/LICENSE-2.0.txt
+.. |Codestyle Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
```

### Comparing `tulona-0.2.3/core/tulona.egg-info/SOURCES.txt` & `tulona-0.2.4/core/tulona.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 core/tulona/cli/params.py
 core/tulona/config/__init__.py
 core/tulona/config/profile.py
 core/tulona/config/project.py
 core/tulona/config/runtime.py
 core/tulona/task/base.py
 core/tulona/task/compare.py
+core/tulona/task/ping.py
 core/tulona/task/profile.py
 core/tulona/task/scan.py
-core/tulona/task/test_connection.py
 core/tulona/util/__init__.py
 core/tulona/util/database.py
 core/tulona/util/dataframe.py
 core/tulona/util/excel.py
 core/tulona/util/filesystem.py
 core/tulona/util/profiles.py
 core/tulona/util/project.py
```

### Comparing `tulona-0.2.3/pyproject.toml` & `tulona-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tulona"
-version = "0.2.3"
+version = "0.2.4"
 description = "A tool to compare data from different sources."
 dependencies = [
   "click~=8.1",
   "ruamel.yaml~=0.18",
   "psycopg2-binary~=2.9",
   "pymysql~=1.1",
   "cryptography~=42.0",
@@ -96,22 +96,22 @@
 
 [tool.isort]
 profile = "black"
 line_length = 90
 skip = [".gitignore"]
 
 [tool.bumpversion]
-current_version = "0.2.3"
+current_version = "0.2.4"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 search = "{current_version}"
 replace = "{new_version}"
 regex = false
 ignore_missing_version = false
-tag = false
+tag = true
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 commit_args = ""
```

