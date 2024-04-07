# Comparing `tmp/csv2db-1.6.0.tar.gz` & `tmp/csv2db-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv2db-1.6.0.tar", last modified: Sat Nov  4 17:42:18 2023, max compression
+gzip compressed data, was "csv2db-1.6.1.tar", last modified: Sun Apr  7 01:58:23 2024, max compression
```

## Comparing `csv2db-1.6.0.tar` & `csv2db-1.6.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 17:42:18.761048 csv2db-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-11-04 17:42:10.000000 csv2db-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2023-11-04 17:42:18.761048 csv2db-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15827 2023-11-04 17:42:10.000000 csv2db-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2023-11-04 17:42:10.000000 csv2db-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-04 17:42:18.761048 csv2db-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 17:42:18.757048 csv2db-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 17:42:18.757048 csv2db-1.6.0/src/csv2db/
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-11-04 17:42:10.000000 csv2db-1.6.0/src/csv2db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2023-11-04 17:42:10.000000 csv2db-1.6.0/src/csv2db/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-11-04 17:42:10.000000 csv2db-1.6.0/src/csv2db/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12367 2023-11-04 17:42:10.000000 csv2db-1.6.0/src/csv2db/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 17:42:18.757048 csv2db-1.6.0/src/csv2db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2023-11-04 17:42:18.000000 csv2db-1.6.0/src/csv2db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      535 2023-11-04 17:42:18.000000 csv2db-1.6.0/src/csv2db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-04 17:42:18.000000 csv2db-1.6.0/src/csv2db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-04 17:42:18.000000 csv2db-1.6.0/src/csv2db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-11-04 17:42:18.000000 csv2db-1.6.0/src/csv2db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-04 17:42:18.000000 csv2db-1.6.0/src/csv2db.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)    24202 2023-11-04 17:42:10.000000 csv2db-1.6.0/src/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-04 17:42:18.761048 csv2db-1.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2023-11-04 17:42:10.000000 csv2db-1.6.0/test/tests_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)    15399 2023-11-04 17:42:10.000000 csv2db-1.6.0/test/tests_loading.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-11-04 17:42:10.000000 csv2db-1.6.0/test/tests_loading_db2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-11-04 17:42:10.000000 csv2db-1.6.0/test/tests_loading_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2023-11-04 17:42:10.000000 csv2db-1.6.0/test/tests_loading_oracle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-11-04 17:42:10.000000 csv2db-1.6.0/test/tests_loading_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-11-04 17:42:10.000000 csv2db-1.6.0/test/tests_loading_sqlserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:58:23.161880 csv2db-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 01:58:16.000000 csv2db-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17725 2024-04-07 01:58:23.161880 csv2db-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16448 2024-04-07 01:58:16.000000 csv2db-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-04-07 01:58:16.000000 csv2db-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 01:58:23.161880 csv2db-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:58:23.157880 csv2db-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:58:23.157880 csv2db-1.6.1/src/csv2db/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-07 01:58:16.000000 csv2db-1.6.1/src/csv2db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-07 01:58:16.000000 csv2db-1.6.1/src/csv2db/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-07 01:58:16.000000 csv2db-1.6.1/src/csv2db/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12294 2024-04-07 01:58:16.000000 csv2db-1.6.1/src/csv2db/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:58:23.161880 csv2db-1.6.1/src/csv2db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17725 2024-04-07 01:58:23.000000 csv2db-1.6.1/src/csv2db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-07 01:58:23.000000 csv2db-1.6.1/src/csv2db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 01:58:23.000000 csv2db-1.6.1/src/csv2db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-07 01:58:23.000000 csv2db-1.6.1/src/csv2db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-07 01:58:23.000000 csv2db-1.6.1/src/csv2db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 01:58:23.000000 csv2db-1.6.1/src/csv2db.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24202 2024-04-07 01:58:16.000000 csv2db-1.6.1/src/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 01:58:23.157880 csv2db-1.6.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-07 01:58:16.000000 csv2db-1.6.1/test/tests_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15399 2024-04-07 01:58:16.000000 csv2db-1.6.1/test/tests_loading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-07 01:58:16.000000 csv2db-1.6.1/test/tests_loading_db2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-07 01:58:16.000000 csv2db-1.6.1/test/tests_loading_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-07 01:58:16.000000 csv2db-1.6.1/test/tests_loading_oracle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 01:58:16.000000 csv2db-1.6.1/test/tests_loading_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 01:58:16.000000 csv2db-1.6.1/test/tests_loading_sqlserver.py
```

### Comparing `csv2db-1.6.0/LICENSE` & `csv2db-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/PKG-INFO` & `csv2db-1.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv2db
-Version: 1.6.0
+Version: 1.6.1
 Summary: The CSV to database command line loader.
 Author: Gerald Venzl
 Maintainer: Gerald Venzl
 Project-URL: Documentation, https://github.com/csv2db/csv2db/wiki
 Project-URL: Homepage, https://csv2db.github.io/
 Project-URL: Issues, https://github.com/csv2db/csv2db/issues
 Project-URL: Source, https://github.com/csv2db/csv2db
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: oracledb>=1.1.1
+Requires-Dist: oracledb>=2.0.0
 Requires-Dist: mysql-connector-python>=8.0.13
-Requires-Dist: psycopg-binary>=3.1.9
+Requires-Dist: psycopg[binary]>=3.1.9
 Requires-Dist: pymssql>=2.1.4
 
 ```
                   ___       ____  
   ___________   _|__ \ ____/ / /_ 
  / ___/ ___/ | / /_/ // __  / __ \
 / /__(__  )| |/ / __// /_/ / /_/ /
@@ -53,34 +53,34 @@
 which is usually much easier once the data is in the database rather than in the CSV files.
 
 `csv2db` is capable of scanning all CSV file headers at once and generate a `CREATE TABLE` statement with all the column names present.
 This is particularly useful if the format of the CSV files has changed over time or because you want to load different CSV file types into the same database table.
 
 # Usage
 
-```console
+```bash
 $ ./csv2db -h
 usage: csv2db [-h] {generate,gen,load,lo} ...
 
 The CSV to database command line loader.
-Version: 1.6.0
+Version: 1.6.1
 (c) Gerald Venzl
 
 positional arguments:
   {generate,gen,load,lo}
     generate (gen)      Prints a CREATE TABLE SQL statement to create the
                         table and columns based on the header row of the CSV
                         file(s).
     load (lo)           Loads the data from the CSV file(s) into the database.
 
 options:
   -h, --help            show this help message and exit
 ```
 
-```console
+```bash
 $ ./csv2db generate -h
 usage: csv2db generate [-h] [-f FILE] [-e ENCODING] [-v] [--debug]
                        [-o {oracle,mysql,postgres,sqlserver,db2}] [-t TABLE]
                        [-c COLUMN_TYPE] [-s SEPARATOR] [-q QUOTE]
                        [--case-insensitive-identifiers] [--quote-identifiers]
 
 options:
@@ -105,15 +105,15 @@
                         The quote character on which a string won't be split.
   --case-insensitive-identifiers
                         If set, all identifiers will be upper-cased.
   --quote-identifiers   If set, all table and column identifiers will be
                         quoted.
 ```
 
-```console
+```bash
 $ ./csv2db load -h
 usage: csv2db load [-h] [-f FILE] [-e ENCODING] [-v] [--debug] -t TABLE
                    [-o {oracle,mysql,postgres,sqlserver,db2}] -u USER
                    [-p PASSWORD] [-m HOST] [-n PORT] [-d DBNAME] [-b BATCH]
                    [-s SEPARATOR] [-q QUOTE] [-a] [--truncate] [-i] [-l]
                    [--case-insensitive-identifiers] [--quote-identifiers]
 
@@ -164,30 +164,30 @@
 
 # How to use csv2db
 
 ## Loading CSV files into the database
 
 `csv2db` can load plain text csv files as well as compressed csv files in `.zip` or `.gz` format without having to uncompress them first.
 
-```console
+```bash
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv -t citibikes -u csv_data -p csv_data -d ORCLPDB1
 
 Loading file test/resources/201811-citibike-tripdata.csv
 File loaded.
 
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv.gz -t citibikes -u csv_data -p csv_data -d ORCLPDB1
 
 Loading file test/resources/201811-citibike-tripdata.csv.gz
 File loaded.
 
 ```
 
 `csv2db` `--verbose` option will provide verbose output.
 
-```console
+```bash
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 1 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -196,15 +196,15 @@
 Closing database connection.
 ```
 
 `csv2db` can load multiple files at once, using either wildcard characters (e.g. data*.csv.zip) or by passing on the folder containing CSV files.
 
 ***Note:** String including wildcard characters have to be enclosed in `""`*
 
-```console
+```bash
 $ ./csv2db load -f "test/resources/201811-citibike-tripdata.*" -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 3 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -219,15 +219,15 @@
 Loading file test/resources/201811-citibike-tripdata.csv.zip
 10 rows loaded.
 File loaded.
 
 Closing database connection.
 ```
 
-```console
+```bash
 $ ./csv2db load -f test/resources -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 3 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -325,50 +325,50 @@
 The idea is to have a staging table that data can be loaded into first and then figure out the correct data types for each column.
 
 # Installation
 
 You can install `csv2db` either by installing it as a Python package,
 which will automatically install all dependencies except the Db2 driver (as this one is still in Beta status)
 
-```console
+```bash
 $ python3 -m pip install csv2db
 $ csv2db
 ```
 
 or cloning this Git repository
 
-```console
+```bash
 $ git clone https://github.com/csv2db/csv2db
 ```
 
 or by downloading one of the releases
 
-```console
+```bash
 $ LOCATION=$(curl -s https://api.github.com/repos/csv2db/csv2db/releases/latest | grep "tag_name" | awk '{print "https://github.com/csv2db/csv2db/archive/" substr($2, 2, length($2)-3) ".zip"}') ; curl -L -o csv2db.zip $LOCATION
 $ unzip csv2db.zip
 $ cd csv2db*
 $ ./csv2db
 ```
     
 In order for `csv2db` to work the appropriate database driver or drivers need to be installed.
 This installation is done automatically when installing `csv2db` as a Python package (`pip install csv2db`).
 The following drivers are being used, and are all available on [pypi.org](https://pypi.org/):
 
-* Oracle: [oracledb](https://pypi.org/project/oracledb/) version 1.1.1+
+* Oracle: [oracledb](https://pypi.org/project/oracledb/) version 2.0.0+
 * MySQL: [mysql-connector-python](https://pypi.org/project/mysql-connector-python/) version 8.0.13+
-* PostgreSQL: [psycopg-binary](https://pypi.org/project/psycopg-binary/) version 3.1.9+
+* PostgreSQL: [psycopg[binary]](https://pypi.org/project/psycopg-binary/) version 3.1.9+
 * SQL Server: [pymssql](https://pypi.org/project/pymssql/) version 2.1.4+
 * DB2: [ibm-db](https://pypi.org/project/ibm-db/) version 2.0.9+
 
 You can install any of these drivers via `pip`:
 
-```console
+```bash
 $ python3 -m pip install oracledb
 $ python3 -m pip install mysql-connector-python
-$ python3 -m pip install psycopg-binary
+$ python3 -m pip install psycopg[binary]
 $ python3 -m pip install pymssql
 $ python3 -m pip install ibm-db
 ```
 
 For more instruction on how to install the driver(s) on your environment,
 please see the documentation of the individual driver or refer to the
 [csv2db Installation Guide](https://github.com/csv2db/csv2db/wiki/Installation-Guide).
@@ -384,14 +384,36 @@
 Following that core design goal, `csv2db` will most likely never provide many database-specific options or parameters for the end-user to set,
 it will not deal with explicit data type or character set conversion or globalization support that some databases offer.
 If a user requires any of these features or more, he or she should look for one of the already existing ETL tools out there.
 
 Simply put, `csv2db` does not do much more than taking rows from a delimited file and execute `INSERT INTO` statements with the values of these rows.
 It is there to help users to get the contents of a file into a database table quickly where the data can then be further processed.
 
+## Using the `csv2db` Docker image
+`csv2db` is also offered as a Docker image, making the usage of `csv2db` quick and easy without requiring any install.
+
+To run `csv2db`, simply invoke the `docker|podman run` command, for example:
+
+```bash
+# quick test the image
+podman run --rm csv2db --help
+```
+
+To load data, bind the folder containing the input files as a Docker volume:
+```bash
+podman run --rm -v <input files folder>:/input/ csv2db load -f /input/<input file(s)> ...
+```
+
+For example:
+```bash
+podman run --rm -v $HOME/input_files:/input csv2db \
+  load -f /input/201811-citibike-tripdata.csv -t citibikes \
+  -u db_user -p db_pass -d my_db
+```
+
 ## Exit codes
 `csv2db` returns following exit codes:  
 
 | Exit code             | Value | Meaning                                                                                          |
 |-----------------------|:-----:|--------------------------------------------------------------------------------------------------|
 | `SUCCESS`             |   0   | Successful execution of the program.                                                             |
 | `GENERIC_ERROR`       |   1   | A generic error occurred.                                                                        |
@@ -403,15 +425,15 @@
 `csv2db` is capable of color coded output and will do so by default (except on Windows).  
 <span style="color:yellow">Debug output is yellow.</span>  
 <span style="color:red">Error output is red.</span>  
 This can be deactivated by setting the `$NO_COLOR` environment variable. For more details on `$NO_COLOR` see https://no-color.org/
 
 # LICENSE
 
-	Copyright 2023 Gerald Venzl
+	Copyright 2024 Gerald Venzl
 	
 	Licensed under the Apache License, Version 2.0 (the "License");
 	you may not use this file except in compliance with the License.
 	You may obtain a copy of the License at
 	
 	    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `csv2db-1.6.0/README.md` & `csv2db-1.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,34 +21,34 @@
 which is usually much easier once the data is in the database rather than in the CSV files.
 
 `csv2db` is capable of scanning all CSV file headers at once and generate a `CREATE TABLE` statement with all the column names present.
 This is particularly useful if the format of the CSV files has changed over time or because you want to load different CSV file types into the same database table.
 
 # Usage
 
-```console
+```bash
 $ ./csv2db -h
 usage: csv2db [-h] {generate,gen,load,lo} ...
 
 The CSV to database command line loader.
-Version: 1.6.0
+Version: 1.6.1
 (c) Gerald Venzl
 
 positional arguments:
   {generate,gen,load,lo}
     generate (gen)      Prints a CREATE TABLE SQL statement to create the
                         table and columns based on the header row of the CSV
                         file(s).
     load (lo)           Loads the data from the CSV file(s) into the database.
 
 options:
   -h, --help            show this help message and exit
 ```
 
-```console
+```bash
 $ ./csv2db generate -h
 usage: csv2db generate [-h] [-f FILE] [-e ENCODING] [-v] [--debug]
                        [-o {oracle,mysql,postgres,sqlserver,db2}] [-t TABLE]
                        [-c COLUMN_TYPE] [-s SEPARATOR] [-q QUOTE]
                        [--case-insensitive-identifiers] [--quote-identifiers]
 
 options:
@@ -73,15 +73,15 @@
                         The quote character on which a string won't be split.
   --case-insensitive-identifiers
                         If set, all identifiers will be upper-cased.
   --quote-identifiers   If set, all table and column identifiers will be
                         quoted.
 ```
 
-```console
+```bash
 $ ./csv2db load -h
 usage: csv2db load [-h] [-f FILE] [-e ENCODING] [-v] [--debug] -t TABLE
                    [-o {oracle,mysql,postgres,sqlserver,db2}] -u USER
                    [-p PASSWORD] [-m HOST] [-n PORT] [-d DBNAME] [-b BATCH]
                    [-s SEPARATOR] [-q QUOTE] [-a] [--truncate] [-i] [-l]
                    [--case-insensitive-identifiers] [--quote-identifiers]
 
@@ -132,30 +132,30 @@
 
 # How to use csv2db
 
 ## Loading CSV files into the database
 
 `csv2db` can load plain text csv files as well as compressed csv files in `.zip` or `.gz` format without having to uncompress them first.
 
-```console
+```bash
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv -t citibikes -u csv_data -p csv_data -d ORCLPDB1
 
 Loading file test/resources/201811-citibike-tripdata.csv
 File loaded.
 
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv.gz -t citibikes -u csv_data -p csv_data -d ORCLPDB1
 
 Loading file test/resources/201811-citibike-tripdata.csv.gz
 File loaded.
 
 ```
 
 `csv2db` `--verbose` option will provide verbose output.
 
-```console
+```bash
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 1 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -164,15 +164,15 @@
 Closing database connection.
 ```
 
 `csv2db` can load multiple files at once, using either wildcard characters (e.g. data*.csv.zip) or by passing on the folder containing CSV files.
 
 ***Note:** String including wildcard characters have to be enclosed in `""`*
 
-```console
+```bash
 $ ./csv2db load -f "test/resources/201811-citibike-tripdata.*" -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 3 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -187,15 +187,15 @@
 Loading file test/resources/201811-citibike-tripdata.csv.zip
 10 rows loaded.
 File loaded.
 
 Closing database connection.
 ```
 
-```console
+```bash
 $ ./csv2db load -f test/resources -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 3 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -293,50 +293,50 @@
 The idea is to have a staging table that data can be loaded into first and then figure out the correct data types for each column.
 
 # Installation
 
 You can install `csv2db` either by installing it as a Python package,
 which will automatically install all dependencies except the Db2 driver (as this one is still in Beta status)
 
-```console
+```bash
 $ python3 -m pip install csv2db
 $ csv2db
 ```
 
 or cloning this Git repository
 
-```console
+```bash
 $ git clone https://github.com/csv2db/csv2db
 ```
 
 or by downloading one of the releases
 
-```console
+```bash
 $ LOCATION=$(curl -s https://api.github.com/repos/csv2db/csv2db/releases/latest | grep "tag_name" | awk '{print "https://github.com/csv2db/csv2db/archive/" substr($2, 2, length($2)-3) ".zip"}') ; curl -L -o csv2db.zip $LOCATION
 $ unzip csv2db.zip
 $ cd csv2db*
 $ ./csv2db
 ```
     
 In order for `csv2db` to work the appropriate database driver or drivers need to be installed.
 This installation is done automatically when installing `csv2db` as a Python package (`pip install csv2db`).
 The following drivers are being used, and are all available on [pypi.org](https://pypi.org/):
 
-* Oracle: [oracledb](https://pypi.org/project/oracledb/) version 1.1.1+
+* Oracle: [oracledb](https://pypi.org/project/oracledb/) version 2.0.0+
 * MySQL: [mysql-connector-python](https://pypi.org/project/mysql-connector-python/) version 8.0.13+
-* PostgreSQL: [psycopg-binary](https://pypi.org/project/psycopg-binary/) version 3.1.9+
+* PostgreSQL: [psycopg[binary]](https://pypi.org/project/psycopg-binary/) version 3.1.9+
 * SQL Server: [pymssql](https://pypi.org/project/pymssql/) version 2.1.4+
 * DB2: [ibm-db](https://pypi.org/project/ibm-db/) version 2.0.9+
 
 You can install any of these drivers via `pip`:
 
-```console
+```bash
 $ python3 -m pip install oracledb
 $ python3 -m pip install mysql-connector-python
-$ python3 -m pip install psycopg-binary
+$ python3 -m pip install psycopg[binary]
 $ python3 -m pip install pymssql
 $ python3 -m pip install ibm-db
 ```
 
 For more instruction on how to install the driver(s) on your environment,
 please see the documentation of the individual driver or refer to the
 [csv2db Installation Guide](https://github.com/csv2db/csv2db/wiki/Installation-Guide).
@@ -352,14 +352,36 @@
 Following that core design goal, `csv2db` will most likely never provide many database-specific options or parameters for the end-user to set,
 it will not deal with explicit data type or character set conversion or globalization support that some databases offer.
 If a user requires any of these features or more, he or she should look for one of the already existing ETL tools out there.
 
 Simply put, `csv2db` does not do much more than taking rows from a delimited file and execute `INSERT INTO` statements with the values of these rows.
 It is there to help users to get the contents of a file into a database table quickly where the data can then be further processed.
 
+## Using the `csv2db` Docker image
+`csv2db` is also offered as a Docker image, making the usage of `csv2db` quick and easy without requiring any install.
+
+To run `csv2db`, simply invoke the `docker|podman run` command, for example:
+
+```bash
+# quick test the image
+podman run --rm csv2db --help
+```
+
+To load data, bind the folder containing the input files as a Docker volume:
+```bash
+podman run --rm -v <input files folder>:/input/ csv2db load -f /input/<input file(s)> ...
+```
+
+For example:
+```bash
+podman run --rm -v $HOME/input_files:/input csv2db \
+  load -f /input/201811-citibike-tripdata.csv -t citibikes \
+  -u db_user -p db_pass -d my_db
+```
+
 ## Exit codes
 `csv2db` returns following exit codes:  
 
 | Exit code             | Value | Meaning                                                                                          |
 |-----------------------|:-----:|--------------------------------------------------------------------------------------------------|
 | `SUCCESS`             |   0   | Successful execution of the program.                                                             |
 | `GENERIC_ERROR`       |   1   | A generic error occurred.                                                                        |
@@ -371,15 +393,15 @@
 `csv2db` is capable of color coded output and will do so by default (except on Windows).  
 <span style="color:yellow">Debug output is yellow.</span>  
 <span style="color:red">Error output is red.</span>  
 This can be deactivated by setting the `$NO_COLOR` environment variable. For more details on `$NO_COLOR` see https://no-color.org/
 
 # LICENSE
 
-	Copyright 2023 Gerald Venzl
+	Copyright 2024 Gerald Venzl
 	
 	Licensed under the Apache License, Version 2.0 (the "License");
 	you may not use this file except in compliance with the License.
 	You may obtain a copy of the License at
 	
 	    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `csv2db-1.6.0/pyproject.toml` & `csv2db-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # Since: October, 2023
 # Author: gvenzl
 # Name: pyproject.toml
 # Description: The project file
 #
-# Copyright 2019 Gerald Venzl
+# Copyright 2023 Gerald Venzl
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "csv2db"
-version = "1.6.0"
+version = "1.6.1"
 description = "The CSV to database command line loader."
 authors = [{ name="Gerald Venzl" }]
 maintainers = [{ name="Gerald Venzl" }]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -44,17 +44,17 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Database",
     "Topic :: Utilities",
 ]
 requires-python = ">=3.8"
 dependencies = [
-        "oracledb >= 1.1.1",
+        "oracledb >= 2.0.0",
         "mysql-connector-python >= 8.0.13",
-        "psycopg-binary >= 3.1.9",
+        "psycopg[binary] >= 3.1.9",
         "pymssql >= 2.1.4",
 ]
 
 [project.scripts]
 csv2db = "main:entrypoint"
 
 [project.urls]
```

### Comparing `csv2db-1.6.0/src/csv2db/__init__.py` & `csv2db-1.6.1/src/csv2db/__init__.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/src/csv2db/config.py` & `csv2db-1.6.1/src/csv2db/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-version = "1.6.0"
+version = "1.6.1"
 
 verbose = False
 debug = False
 direct_path = False
 batch_size = 10000
 conn = None
 table_name = ""
```

### Comparing `csv2db-1.6.0/src/csv2db/constants.py` & `csv2db-1.6.1/src/csv2db/constants.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/src/csv2db/functions.py` & `csv2db-1.6.1/src/csv2db/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,16 +226,15 @@
     """
 
     try:
         if db_type is DBType.ORACLE:
             import oracledb
             conn = oracledb.connect(user=user,
                                     password=password,
-                                    dsn=host + ":" + port + "/" + db_name,
-                                    encoding="UTF-8", nencoding="UTF-8")
+                                    dsn=host + ":" + port + "/" + db_name)
         elif db_type is DBType.MYSQL:
             import mysql.connector
             conn = mysql.connector.connect(
                                        user=user,
                                        password=password,
                                        host=host,
                                        port=int(port),
```

### Comparing `csv2db-1.6.0/src/csv2db.egg-info/PKG-INFO` & `csv2db-1.6.1/src/csv2db.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv2db
-Version: 1.6.0
+Version: 1.6.1
 Summary: The CSV to database command line loader.
 Author: Gerald Venzl
 Maintainer: Gerald Venzl
 Project-URL: Documentation, https://github.com/csv2db/csv2db/wiki
 Project-URL: Homepage, https://csv2db.github.io/
 Project-URL: Issues, https://github.com/csv2db/csv2db/issues
 Project-URL: Source, https://github.com/csv2db/csv2db
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: oracledb>=1.1.1
+Requires-Dist: oracledb>=2.0.0
 Requires-Dist: mysql-connector-python>=8.0.13
-Requires-Dist: psycopg-binary>=3.1.9
+Requires-Dist: psycopg[binary]>=3.1.9
 Requires-Dist: pymssql>=2.1.4
 
 ```
                   ___       ____  
   ___________   _|__ \ ____/ / /_ 
  / ___/ ___/ | / /_/ // __  / __ \
 / /__(__  )| |/ / __// /_/ / /_/ /
@@ -53,34 +53,34 @@
 which is usually much easier once the data is in the database rather than in the CSV files.
 
 `csv2db` is capable of scanning all CSV file headers at once and generate a `CREATE TABLE` statement with all the column names present.
 This is particularly useful if the format of the CSV files has changed over time or because you want to load different CSV file types into the same database table.
 
 # Usage
 
-```console
+```bash
 $ ./csv2db -h
 usage: csv2db [-h] {generate,gen,load,lo} ...
 
 The CSV to database command line loader.
-Version: 1.6.0
+Version: 1.6.1
 (c) Gerald Venzl
 
 positional arguments:
   {generate,gen,load,lo}
     generate (gen)      Prints a CREATE TABLE SQL statement to create the
                         table and columns based on the header row of the CSV
                         file(s).
     load (lo)           Loads the data from the CSV file(s) into the database.
 
 options:
   -h, --help            show this help message and exit
 ```
 
-```console
+```bash
 $ ./csv2db generate -h
 usage: csv2db generate [-h] [-f FILE] [-e ENCODING] [-v] [--debug]
                        [-o {oracle,mysql,postgres,sqlserver,db2}] [-t TABLE]
                        [-c COLUMN_TYPE] [-s SEPARATOR] [-q QUOTE]
                        [--case-insensitive-identifiers] [--quote-identifiers]
 
 options:
@@ -105,15 +105,15 @@
                         The quote character on which a string won't be split.
   --case-insensitive-identifiers
                         If set, all identifiers will be upper-cased.
   --quote-identifiers   If set, all table and column identifiers will be
                         quoted.
 ```
 
-```console
+```bash
 $ ./csv2db load -h
 usage: csv2db load [-h] [-f FILE] [-e ENCODING] [-v] [--debug] -t TABLE
                    [-o {oracle,mysql,postgres,sqlserver,db2}] -u USER
                    [-p PASSWORD] [-m HOST] [-n PORT] [-d DBNAME] [-b BATCH]
                    [-s SEPARATOR] [-q QUOTE] [-a] [--truncate] [-i] [-l]
                    [--case-insensitive-identifiers] [--quote-identifiers]
 
@@ -164,30 +164,30 @@
 
 # How to use csv2db
 
 ## Loading CSV files into the database
 
 `csv2db` can load plain text csv files as well as compressed csv files in `.zip` or `.gz` format without having to uncompress them first.
 
-```console
+```bash
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv -t citibikes -u csv_data -p csv_data -d ORCLPDB1
 
 Loading file test/resources/201811-citibike-tripdata.csv
 File loaded.
 
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv.gz -t citibikes -u csv_data -p csv_data -d ORCLPDB1
 
 Loading file test/resources/201811-citibike-tripdata.csv.gz
 File loaded.
 
 ```
 
 `csv2db` `--verbose` option will provide verbose output.
 
-```console
+```bash
 $ ./csv2db load -f test/resources/201811-citibike-tripdata.csv -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 1 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -196,15 +196,15 @@
 Closing database connection.
 ```
 
 `csv2db` can load multiple files at once, using either wildcard characters (e.g. data*.csv.zip) or by passing on the folder containing CSV files.
 
 ***Note:** String including wildcard characters have to be enclosed in `""`*
 
-```console
+```bash
 $ ./csv2db load -f "test/resources/201811-citibike-tripdata.*" -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 3 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -219,15 +219,15 @@
 Loading file test/resources/201811-citibike-tripdata.csv.zip
 10 rows loaded.
 File loaded.
 
 Closing database connection.
 ```
 
-```console
+```bash
 $ ./csv2db load -f test/resources -t citibikes -u csv_data -p csv_data -d ORCLPDB1 --verbose
 Finding file(s).
 Found 3 file(s).
 Establishing database connection.
 
 Loading file test/resources/201811-citibike-tripdata.csv
 16 rows loaded.
@@ -325,50 +325,50 @@
 The idea is to have a staging table that data can be loaded into first and then figure out the correct data types for each column.
 
 # Installation
 
 You can install `csv2db` either by installing it as a Python package,
 which will automatically install all dependencies except the Db2 driver (as this one is still in Beta status)
 
-```console
+```bash
 $ python3 -m pip install csv2db
 $ csv2db
 ```
 
 or cloning this Git repository
 
-```console
+```bash
 $ git clone https://github.com/csv2db/csv2db
 ```
 
 or by downloading one of the releases
 
-```console
+```bash
 $ LOCATION=$(curl -s https://api.github.com/repos/csv2db/csv2db/releases/latest | grep "tag_name" | awk '{print "https://github.com/csv2db/csv2db/archive/" substr($2, 2, length($2)-3) ".zip"}') ; curl -L -o csv2db.zip $LOCATION
 $ unzip csv2db.zip
 $ cd csv2db*
 $ ./csv2db
 ```
     
 In order for `csv2db` to work the appropriate database driver or drivers need to be installed.
 This installation is done automatically when installing `csv2db` as a Python package (`pip install csv2db`).
 The following drivers are being used, and are all available on [pypi.org](https://pypi.org/):
 
-* Oracle: [oracledb](https://pypi.org/project/oracledb/) version 1.1.1+
+* Oracle: [oracledb](https://pypi.org/project/oracledb/) version 2.0.0+
 * MySQL: [mysql-connector-python](https://pypi.org/project/mysql-connector-python/) version 8.0.13+
-* PostgreSQL: [psycopg-binary](https://pypi.org/project/psycopg-binary/) version 3.1.9+
+* PostgreSQL: [psycopg[binary]](https://pypi.org/project/psycopg-binary/) version 3.1.9+
 * SQL Server: [pymssql](https://pypi.org/project/pymssql/) version 2.1.4+
 * DB2: [ibm-db](https://pypi.org/project/ibm-db/) version 2.0.9+
 
 You can install any of these drivers via `pip`:
 
-```console
+```bash
 $ python3 -m pip install oracledb
 $ python3 -m pip install mysql-connector-python
-$ python3 -m pip install psycopg-binary
+$ python3 -m pip install psycopg[binary]
 $ python3 -m pip install pymssql
 $ python3 -m pip install ibm-db
 ```
 
 For more instruction on how to install the driver(s) on your environment,
 please see the documentation of the individual driver or refer to the
 [csv2db Installation Guide](https://github.com/csv2db/csv2db/wiki/Installation-Guide).
@@ -384,14 +384,36 @@
 Following that core design goal, `csv2db` will most likely never provide many database-specific options or parameters for the end-user to set,
 it will not deal with explicit data type or character set conversion or globalization support that some databases offer.
 If a user requires any of these features or more, he or she should look for one of the already existing ETL tools out there.
 
 Simply put, `csv2db` does not do much more than taking rows from a delimited file and execute `INSERT INTO` statements with the values of these rows.
 It is there to help users to get the contents of a file into a database table quickly where the data can then be further processed.
 
+## Using the `csv2db` Docker image
+`csv2db` is also offered as a Docker image, making the usage of `csv2db` quick and easy without requiring any install.
+
+To run `csv2db`, simply invoke the `docker|podman run` command, for example:
+
+```bash
+# quick test the image
+podman run --rm csv2db --help
+```
+
+To load data, bind the folder containing the input files as a Docker volume:
+```bash
+podman run --rm -v <input files folder>:/input/ csv2db load -f /input/<input file(s)> ...
+```
+
+For example:
+```bash
+podman run --rm -v $HOME/input_files:/input csv2db \
+  load -f /input/201811-citibike-tripdata.csv -t citibikes \
+  -u db_user -p db_pass -d my_db
+```
+
 ## Exit codes
 `csv2db` returns following exit codes:  
 
 | Exit code             | Value | Meaning                                                                                          |
 |-----------------------|:-----:|--------------------------------------------------------------------------------------------------|
 | `SUCCESS`             |   0   | Successful execution of the program.                                                             |
 | `GENERIC_ERROR`       |   1   | A generic error occurred.                                                                        |
@@ -403,15 +425,15 @@
 `csv2db` is capable of color coded output and will do so by default (except on Windows).  
 <span style="color:yellow">Debug output is yellow.</span>  
 <span style="color:red">Error output is red.</span>  
 This can be deactivated by setting the `$NO_COLOR` environment variable. For more details on `$NO_COLOR` see https://no-color.org/
 
 # LICENSE
 
-	Copyright 2023 Gerald Venzl
+	Copyright 2024 Gerald Venzl
 	
 	Licensed under the Apache License, Version 2.0 (the "License");
 	you may not use this file except in compliance with the License.
 	You may obtain a copy of the License at
 	
 	    http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `csv2db-1.6.0/src/csv2db.egg-info/SOURCES.txt` & `csv2db-1.6.1/src/csv2db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/src/main.py` & `csv2db-1.6.1/src/main.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/test/tests_functional.py` & `csv2db-1.6.1/test/tests_functional.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/test/tests_loading.py` & `csv2db-1.6.1/test/tests_loading.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/test/tests_loading_db2.py` & `csv2db-1.6.1/test/tests_loading_db2.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/test/tests_loading_mysql.py` & `csv2db-1.6.1/test/tests_loading_mysql.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/test/tests_loading_oracle.py` & `csv2db-1.6.1/test/tests_loading_oracle.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/test/tests_loading_postgres.py` & `csv2db-1.6.1/test/tests_loading_postgres.py`

 * *Files identical despite different names*

### Comparing `csv2db-1.6.0/test/tests_loading_sqlserver.py` & `csv2db-1.6.1/test/tests_loading_sqlserver.py`

 * *Files identical despite different names*

