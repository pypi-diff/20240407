# Comparing `tmp/postgresql-integration-test-0.0.1.tar.gz` & `tmp/postgresql-integration-test-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgresql-integration-test-0.0.1.tar", last modified: Sun Apr  7 00:34:02 2024, max compression
+gzip compressed data, was "postgresql-integration-test-0.0.2.tar", last modified: Sun Apr  7 15:11:43 2024, max compression
```

## Comparing `postgresql-integration-test-0.0.1.tar` & `postgresql-integration-test-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2024-04-07 00:34:02.916164 postgresql-integration-test-0.0.1/
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)    11358 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/LICENSE
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     4048 2024-04-07 00:34:02.916164 postgresql-integration-test-0.0.1/PKG-INFO
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     2939 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/README.md
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2024-04-07 00:34:02.912165 postgresql-integration-test-0.0.1/postgresql_integration_test/
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)        0 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/postgresql_integration_test/__init__.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       43 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/postgresql_integration_test/exceptions.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      802 2024-04-07 00:24:46.000000 postgresql-integration-test-0.0.1/postgresql_integration_test/helpers.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1276 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/postgresql_integration_test/log.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     7769 2024-04-07 00:29:55.000000 postgresql-integration-test-0.0.1/postgresql_integration_test/postgresql.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     3489 2024-04-07 00:24:58.000000 postgresql-integration-test-0.0.1/postgresql_integration_test/settings.py
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       22 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/postgresql_integration_test/version.py
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2024-04-07 00:34:02.914164 postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     4048 2024-04-07 00:34:02.000000 postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/PKG-INFO
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      694 2024-04-07 00:34:02.000000 postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/SOURCES.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)        1 2024-04-07 00:34:02.000000 postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/dependency_links.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)      168 2024-04-07 00:34:02.000000 postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/requires.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       28 2024-04-07 00:34:02.000000 postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/top_level.txt
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)     1615 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/pyproject.toml
--rw-r--r--   0 jcamp     (1000) jcamp     (1000)       38 2024-04-07 00:34:02.916164 postgresql-integration-test-0.0.1/setup.cfg
-drwxr-xr-x   0 jcamp     (1000) jcamp     (1000)        0 2024-04-07 00:34:02.914164 postgresql-integration-test-0.0.1/tests/
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1941 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/tests/test_helpers.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1908 2024-04-06 22:59:01.000000 postgresql-integration-test-0.0.1/tests/test_integration.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     1222 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/tests/test_log.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      568 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/tests/test_pgsql.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)     3013 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/tests/test_settings.py
--rwxr-xr-x   0 jcamp     (1000) jcamp     (1000)      266 2024-04-06 21:09:10.000000 postgresql-integration-test-0.0.1/tests/test_version.py
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.036170 postgresql-integration-test-0.0.2/
+-rw-r--r--   0 jcamp      (501) staff       (20)    11358 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/LICENSE
+-rw-r--r--   0 jcamp      (501) staff       (20)     4218 2024-04-07 15:11:43.035289 postgresql-integration-test-0.0.2/PKG-INFO
+-rw-r--r--   0 jcamp      (501) staff       (20)     2908 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/README.md
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.027504 postgresql-integration-test-0.0.2/postgresql_integration_test/
+-rw-r--r--   0 jcamp      (501) staff       (20)       76 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/__init__.py
+-rw-r--r--   0 jcamp      (501) staff       (20)       32 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/attributes.py
+-rw-r--r--   0 jcamp      (501) staff       (20)       43 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/exceptions.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     1670 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/helpers.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     1276 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/log.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     7778 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/postgresql.py
+-rw-r--r--   0 jcamp      (501) staff       (20)     2947 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/settings.py
+-rw-r--r--   0 jcamp      (501) staff       (20)       22 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/postgresql_integration_test/version.py
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.032393 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/
+-rw-r--r--   0 jcamp      (501) staff       (20)     4218 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/PKG-INFO
+-rw-r--r--   0 jcamp      (501) staff       (20)      736 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/SOURCES.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)        1 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/dependency_links.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)      168 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/requires.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)       28 2024-04-07 15:11:43.000000 postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/top_level.txt
+-rw-r--r--   0 jcamp      (501) staff       (20)     1796 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/pyproject.toml
+-rw-r--r--   0 jcamp      (501) staff       (20)       38 2024-04-07 15:11:43.036352 postgresql-integration-test-0.0.2/setup.cfg
+drwxr-xr-x   0 jcamp      (501) staff       (20)        0 2024-04-07 15:11:43.031876 postgresql-integration-test-0.0.2/tests/
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     1941 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/tests/test_helpers.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     1908 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/tests/test_integration.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     1222 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/tests/test_log.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)      568 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/tests/test_pgsql.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)     3002 2024-04-07 15:05:53.000000 postgresql-integration-test-0.0.2/tests/test_settings.py
+-rwxr-xr-x   0 jcamp      (501) staff       (20)      266 2024-04-07 13:12:52.000000 postgresql-integration-test-0.0.2/tests/test_version.py
```

### Comparing `postgresql-integration-test-0.0.1/LICENSE` & `postgresql-integration-test-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.1/PKG-INFO` & `postgresql-integration-test-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: postgresql-integration-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application.
 Author-email: Jason Camp <me@jason.camp>, Ian Meyer <k@imeyer.io>
 License: Apache
 Project-URL: Homepage, https://github.com/jasondcamp/postgresql-integration-test
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psycopg2-binary>=2.9.9
 Requires-Dist: pyyaml>=6.0.1
 Provides-Extra: tests
 Requires-Dist: pytest>=8.1.1; extra == "tests"
@@ -22,15 +26,15 @@
 Requires-Dist: mock==5.0.1; extra == "tests"
 Requires-Dist: pytest-mock==3.10.0; extra == "tests"
 Requires-Dist: pytest-skip-slow==0.0.5; extra == "tests"
 
 # postgresql-integration-test
 ![](https://img.shields.io/pypi/v/postgresql-integration-test.svg) ![](https://img.shields.io/badge/status-alpha-red) ![](https://github.com/jasondcamp/postgresql-integration-test/actions/workflows/postgresql-integration-test.yml/badge.svg)  ![](https://img.shields.io/pypi/pyversions/postgresql-integration-test.svg) ![](https://img.shields.io/badge/license-Apache-lightgrey)
 
-![](https://api.codeclimate.com/v1/badges/e5505727f2fa988debcb/maintainability) ![](https://api.codeclimate.com/v1/badges/e5505727f2fa988debcb/test_coverage)
+![](https://api.codeclimate.com/v1/badges/c4e922d83662be40871c/maintainability) ![](https://api.codeclimate.com/v1/badges/c4e922d83662be40871c/test_coverage)
 
 ## Overview
 postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application. You will need a working PostgreSQL install. It does not have to be running, the binaries are needed.
 
 ## Download and Install
 To install use pip:
 
@@ -45,20 +49,19 @@
 The following class arguments can be overridden by passing them in, these arguments will override the config file arguments.
 | Argument | Description | Default |
 | --------------- | -------------- | -------------- |
 |username|Username for database|root|
 |password|Password for database|root|
 |host|Host to bind|127.0.0.1|
 |port|Port to bind|random|
-|mysql_install_db_binary|Location of mysql_install_db|Searches paths|
-|mysqld_binary|Location of mysqld|Searches paths|
-|timeout_start|Timeout to start MySQL|30 seconds|
-|timeout_stop|Timeout to stop MySQL|30 seconds|
+|postgres_binary|Location of postgres binary|Searches paths|
+|timeout_start|Timeout to start PostgreSQL|30 seconds|
+|timeout_stop|Timeout to stop PostgreSQL|30 seconds|
 |log_level|Log level|INFO|
-|config_file|Configuration file|mysqld-integration-test.cfg|
+|config_file|Configuration file|postgresql-integration-test.cfg|
 
 ### postgresql-integration-test config file
 Default settings can be overridden in  a config file. The default name is `posgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
 
 #### Example config
 ```
 database:
@@ -101,16 +104,16 @@
 
 ```
 #!/usr/bin/env python3
 
 from postgresql_integration_test import PostgreSQL
 import psycopg2
 
-mysqld = Mysqld(config='/some/dir/mysqld-integration-test.cfg')
-instance = mysqld.run()
+postgresql = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
+instance = postgres.run()
 
 # Make query to database
 cnx = mysql.connector.connect(user=instance.username, password=instance.password,
                       host=instance.host, port=instance.port)
 cursor = cnx.cursor()
 cursor.execute(f"SHOW databases;")
```

### Comparing `postgresql-integration-test-0.0.1/README.md` & `postgresql-integration-test-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # postgresql-integration-test
 ![](https://img.shields.io/pypi/v/postgresql-integration-test.svg) ![](https://img.shields.io/badge/status-alpha-red) ![](https://github.com/jasondcamp/postgresql-integration-test/actions/workflows/postgresql-integration-test.yml/badge.svg)  ![](https://img.shields.io/pypi/pyversions/postgresql-integration-test.svg) ![](https://img.shields.io/badge/license-Apache-lightgrey)
 
-![](https://api.codeclimate.com/v1/badges/e5505727f2fa988debcb/maintainability) ![](https://api.codeclimate.com/v1/badges/e5505727f2fa988debcb/test_coverage)
+![](https://api.codeclimate.com/v1/badges/c4e922d83662be40871c/maintainability) ![](https://api.codeclimate.com/v1/badges/c4e922d83662be40871c/test_coverage)
 
 ## Overview
 postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application. You will need a working PostgreSQL install. It does not have to be running, the binaries are needed.
 
 ## Download and Install
 To install use pip:
 
@@ -20,20 +20,19 @@
 The following class arguments can be overridden by passing them in, these arguments will override the config file arguments.
 | Argument | Description | Default |
 | --------------- | -------------- | -------------- |
 |username|Username for database|root|
 |password|Password for database|root|
 |host|Host to bind|127.0.0.1|
 |port|Port to bind|random|
-|mysql_install_db_binary|Location of mysql_install_db|Searches paths|
-|mysqld_binary|Location of mysqld|Searches paths|
-|timeout_start|Timeout to start MySQL|30 seconds|
-|timeout_stop|Timeout to stop MySQL|30 seconds|
+|postgres_binary|Location of postgres binary|Searches paths|
+|timeout_start|Timeout to start PostgreSQL|30 seconds|
+|timeout_stop|Timeout to stop PostgreSQL|30 seconds|
 |log_level|Log level|INFO|
-|config_file|Configuration file|mysqld-integration-test.cfg|
+|config_file|Configuration file|postgresql-integration-test.cfg|
 
 ### postgresql-integration-test config file
 Default settings can be overridden in  a config file. The default name is `posgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
 
 #### Example config
 ```
 database:
@@ -76,16 +75,16 @@
 
 ```
 #!/usr/bin/env python3
 
 from postgresql_integration_test import PostgreSQL
 import psycopg2
 
-mysqld = Mysqld(config='/some/dir/mysqld-integration-test.cfg')
-instance = mysqld.run()
+postgresql = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
+instance = postgres.run()
 
 # Make query to database
 cnx = mysql.connector.connect(user=instance.username, password=instance.password,
                       host=instance.host, port=instance.port)
 cursor = cnx.cursor()
 cursor.execute(f"SHOW databases;")
```

### Comparing `postgresql-integration-test-0.0.1/postgresql_integration_test/log.py` & `postgresql-integration-test-0.0.2/postgresql_integration_test/log.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.1/postgresql_integration_test/postgresql.py` & `postgresql-integration-test-0.0.2/postgresql_integration_test/postgresql.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 import socket
 import subprocess
 from datetime import datetime
 
 from postgresql_integration_test.log import logger
 from postgresql_integration_test import settings
 from postgresql_integration_test.version import __version__
+from postgresql_integration_test.helpers import Utils
 from postgresql_integration_test.settings import ConfigFile
 from postgresql_integration_test.settings import ConfigInstance
 
 
 class PostgreSQL:
     def __init__(self, **kwargs):
         logger.debug(f"postgresql-integration-test {__version__}")
 
         self.child_process = None
         self.terminate_signal = signal.SIGTERM
         self.owner_pid = None
         self.user = getpass.getuser()
-        self.base_dir = tempfile.mkdtemp("postgresql_integration_test", dir=tempfile.gettempdir())
+        self.base_dir = tempfile.mkdtemp()
         self.config = ConfigFile(base_dir=self.base_dir)
 
         if "config_file" in kwargs:
             self.config.general.config_file = kwargs["config_file"]
 
         self.config = settings.parse_config(self.config, kwargs)
         logger.setlevel(self.config.general.log_level)
 
         atexit.register(self.stop)
 
     def __del__(self):
-        logger.debug(f"Cleaning up temp dir {self.config.dirs.base_dir}")
-        # Sleep for a 1/2 sec to allow mysql to shut down
-
+        logger.debug(f"Cleaning up temp dir {self.base_dir}")
+        # Sleep for a 1/4 sec to allow mysql to shut down
         while self.child_process is not None:
             time.sleep(0.25)
         if self.config.general.cleanup_dirs and os.path.exists(self.base_dir):
             try:
                 shutil.rmtree(self.base_dir)
             except Exception as exc:
                 raise RuntimeError(f"Uh oh! {exc}")
@@ -64,15 +64,15 @@
         os.mkdir(self.config.dirs.etc_dir)
         os.mkdir(self.config.dirs.data_dir)
 
         # Run initdb
         try:
             logger.debug("Initializing PostgreSQL w/initdb")
             pgsql_command_line = [
-                shutil.which("initdb"),
+                Utils.find_program("initdb"),
                 "-g",
                 "-D",
                 os.path.join(self.config.dirs.data_dir),
                 "-U",
                 self.user,
             ]
             logger.debug(f"PG_CTL_INITDB_CMD: {pgsql_command_line}")
@@ -88,15 +88,15 @@
 
         # Start postgreSQL
         try:
             logger.debug(
                 f"Starting PostgreSQL at {os.path.join(self.config.dirs.data_dir)}"
             )
             pgsql_command_line = [
-                shutil.which("postgres"),
+                Utils.find_program("postgres"),
                 "-D",
                 os.path.join(self.config.dirs.data_dir),
                 "-h",
                 "localhost",
                 "-p",
                 str(self.config.database.port),
                 "-k",
@@ -116,15 +116,15 @@
                 raise
 
         # Create the role user
         try:
             logger.debug(f"Creating role {self.user}")
 
             pgsql_command_line = [
-                shutil.which("createuser"),
+                Utils.find_program("createuser"),
                 "-U",
                 self.user,
                 "-h",
                 "localhost",
                 "-p",
                 str(self.config.database.port),
                 self.user,
@@ -141,15 +141,15 @@
         except Exception as exc:
             raise RuntimeError(f"Failed creating role: {self.config.database.name} - {exc}")
 
         # Create the test database
         try:
             logger.debug("Creating Database 'test'")
             pgsql_command_line = [
-                shutil.which("createdb"),
+                Utils.find_program("createdb"),
                 "-U",
                 self.user,
                 "-h",
                 "localhost",
                 "-p",
                 str(self.config.database.port),
                 "test",
```

### Comparing `postgresql-integration-test-0.0.1/postgresql_integration_test/settings.py` & `postgresql-integration-test-0.0.2/postgresql_integration_test/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import functools
 import yaml
-import subprocess
-import shutil
 import getpass
 
 from postgresql_integration_test.helpers import Utils
+from postgresql_integration_test.attributes import ConfigAttribute
 
 config_settings = {}
 config_settings["database"] = [
     "username",
     "password",
     "host",
     "port",
@@ -60,56 +59,37 @@
         if section in cfg:
             config = merge_configs(config, section, cfg[section])
 
     # Merge in any class arguments
     for section in config_settings:
         config = merge_configs(config, section, config_args)
 
-    # Get the version of PostgreSQL in case the binary has changed
-    (variant, version_major, version_minor) = Utils.parse_version(
-        subprocess.check_output([config.database.postgres_binary, "--version"]).decode(
-            "utf-8"
-        )
-    )
-    config.version.variant = variant
-    config.version.major = version_major
-    config.version.minor = version_minor
+    # Get the PostgreSQL variant and version
+    config.version = Utils.get_binary_version(config.database.postgres_binary)
 
     return config
 
 
-class ConfigAttribute:
-    pass
-
-
 class ConfigFile:
     def __init__(self, base_dir):
         self.dirs = ConfigAttribute()
         self.dirs.base_dir = base_dir
         self.dirs.data_dir = os.path.join(self.dirs.base_dir, "var")
         self.dirs.etc_dir = os.path.join(self.dirs.base_dir, "etc")
         self.dirs.tmp_dir = os.path.join(self.dirs.base_dir, "tmp")
 
         self.database = ConfigAttribute()
         self.database.host = "localhost"
         self.database.port = Utils.get_unused_port()
         self.database.name = getpass.getuser()
         self.database.username = getpass.getuser()
-        self.database.postgres_binary = shutil.which("postgres")
+        self.database.postgres_binary = Utils.find_program("postgres")
 
         # Get the PostgreSQL variant and version
-        (variant, version_major, version_minor) = Utils.parse_version(
-            subprocess.check_output(
-                [self.database.postgres_binary, "--version"]
-            ).decode("utf-8")
-        )
-        self.version = ConfigAttribute()
-        self.version.variant = variant
-        self.version.major = version_major
-        self.version.minor = version_minor
+        self.version = Utils.get_binary_version(self.database.postgres_binary)
 
         self.general = ConfigAttribute()
         self.general.timeout_start = 30
         self.general.timeout_stop = 30
         self.general.log_level = "DEBUG"
         self.general.config_file = "postgresql-integration-test.cfg"
         self.general.cleanup_dirs = True
```

### Comparing `postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/PKG-INFO` & `postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: postgresql-integration-test
-Version: 0.0.1
+Version: 0.0.2
 Summary: postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application.
 Author-email: Jason Camp <me@jason.camp>, Ian Meyer <k@imeyer.io>
 License: Apache
 Project-URL: Homepage, https://github.com/jasondcamp/postgresql-integration-test
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: psycopg2-binary>=2.9.9
 Requires-Dist: pyyaml>=6.0.1
 Provides-Extra: tests
 Requires-Dist: pytest>=8.1.1; extra == "tests"
@@ -22,15 +26,15 @@
 Requires-Dist: mock==5.0.1; extra == "tests"
 Requires-Dist: pytest-mock==3.10.0; extra == "tests"
 Requires-Dist: pytest-skip-slow==0.0.5; extra == "tests"
 
 # postgresql-integration-test
 ![](https://img.shields.io/pypi/v/postgresql-integration-test.svg) ![](https://img.shields.io/badge/status-alpha-red) ![](https://github.com/jasondcamp/postgresql-integration-test/actions/workflows/postgresql-integration-test.yml/badge.svg)  ![](https://img.shields.io/pypi/pyversions/postgresql-integration-test.svg) ![](https://img.shields.io/badge/license-Apache-lightgrey)
 
-![](https://api.codeclimate.com/v1/badges/e5505727f2fa988debcb/maintainability) ![](https://api.codeclimate.com/v1/badges/e5505727f2fa988debcb/test_coverage)
+![](https://api.codeclimate.com/v1/badges/c4e922d83662be40871c/maintainability) ![](https://api.codeclimate.com/v1/badges/c4e922d83662be40871c/test_coverage)
 
 ## Overview
 postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application. You will need a working PostgreSQL install. It does not have to be running, the binaries are needed.
 
 ## Download and Install
 To install use pip:
 
@@ -45,20 +49,19 @@
 The following class arguments can be overridden by passing them in, these arguments will override the config file arguments.
 | Argument | Description | Default |
 | --------------- | -------------- | -------------- |
 |username|Username for database|root|
 |password|Password for database|root|
 |host|Host to bind|127.0.0.1|
 |port|Port to bind|random|
-|mysql_install_db_binary|Location of mysql_install_db|Searches paths|
-|mysqld_binary|Location of mysqld|Searches paths|
-|timeout_start|Timeout to start MySQL|30 seconds|
-|timeout_stop|Timeout to stop MySQL|30 seconds|
+|postgres_binary|Location of postgres binary|Searches paths|
+|timeout_start|Timeout to start PostgreSQL|30 seconds|
+|timeout_stop|Timeout to stop PostgreSQL|30 seconds|
 |log_level|Log level|INFO|
-|config_file|Configuration file|mysqld-integration-test.cfg|
+|config_file|Configuration file|postgresql-integration-test.cfg|
 
 ### postgresql-integration-test config file
 Default settings can be overridden in  a config file. The default name is `posgresql-integration-test.cfg` in the local directory and can be overridden by passing in the `config` option to the instance creation.
 
 #### Example config
 ```
 database:
@@ -101,16 +104,16 @@
 
 ```
 #!/usr/bin/env python3
 
 from postgresql_integration_test import PostgreSQL
 import psycopg2
 
-mysqld = Mysqld(config='/some/dir/mysqld-integration-test.cfg')
-instance = mysqld.run()
+postgresql = PostgreSQL(config='/some/dir/postgresql-integration-test.cfg')
+instance = postgres.run()
 
 # Make query to database
 cnx = mysql.connector.connect(user=instance.username, password=instance.password,
                       host=instance.host, port=instance.port)
 cursor = cnx.cursor()
 cursor.execute(f"SHOW databases;")
```

### Comparing `postgresql-integration-test-0.0.1/postgresql_integration_test.egg-info/SOURCES.txt` & `postgresql-integration-test-0.0.2/postgresql_integration_test.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 postgresql_integration_test/__init__.py
+postgresql_integration_test/attributes.py
 postgresql_integration_test/exceptions.py
 postgresql_integration_test/helpers.py
 postgresql_integration_test/log.py
 postgresql_integration_test/postgresql.py
 postgresql_integration_test/settings.py
 postgresql_integration_test/version.py
 postgresql_integration_test.egg-info/PKG-INFO
```

### Comparing `postgresql-integration-test-0.0.1/pyproject.toml` & `postgresql-integration-test-0.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 dynamic = ["version", "readme"]
 authors = [{name = "Jason Camp", email = "me@jason.camp"},{name = "Ian Meyer", email = "k@imeyer.io"}]
 license = {text = "Apache"}
 description = "postgresql-integration-test is a python module that creates a temporary PostgreSQL instance to use for testing your application."
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12"
 ]
 
 dependencies = [
     "psycopg2-binary >= 2.9.9",
     "pyyaml >= 6.0.1",
 ]
```

### Comparing `postgresql-integration-test-0.0.1/tests/test_helpers.py` & `postgresql-integration-test-0.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.1/tests/test_integration.py` & `postgresql-integration-test-0.0.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.1/tests/test_log.py` & `postgresql-integration-test-0.0.2/tests/test_log.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.1/tests/test_pgsql.py` & `postgresql-integration-test-0.0.2/tests/test_pgsql.py`

 * *Files identical despite different names*

### Comparing `postgresql-integration-test-0.0.1/tests/test_settings.py` & `postgresql-integration-test-0.0.2/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 import functools
 
-from postgresql_integration_test.postgresql import PostgreSQL
+from postgresql_integration_test import PostgreSQL
 
 
 @pytest.fixture
 def pgsql_connect(autouse=True):
     return PostgreSQL()
```

