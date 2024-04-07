# Comparing `tmp/py4phi-0.9.0.tar.gz` & `tmp/py4phi-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4phi-0.9.0.tar", last modified: Sun Apr  7 20:25:07 2024, max compression
+gzip compressed data, was "py4phi-0.9.1.tar", last modified: Sun Apr  7 20:48:09 2024, max compression
```

## Comparing `py4phi-0.9.0.tar` & `py4phi-0.9.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.840988 py4phi-0.9.0/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    11357 2024-04-07 09:44:34.000000 py4phi-0.9.0/LICENSE
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1873 2024-04-07 10:07:22.000000 py4phi-0.9.0/NOTICE
--rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    21742 2024-04-07 20:25:07.840988 py4phi-0.9.0/PKG-INFO
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     7409 2024-04-07 20:14:44.000000 py4phi-0.9.0/README.md
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.832988 py4phi-0.9.0/cli/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-0.9.0/cli/__init__.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.832988 py4phi-0.9.0/cli/analytics/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-30 22:00:06.000000 py4phi-0.9.0/cli/analytics/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3764 2024-03-31 13:04:23.000000 py4phi-0.9.0/cli/analytics/feature_selection.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3725 2024-03-31 13:04:23.000000 py4phi-0.9.0/cli/analytics/principal_component_analysis.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      497 2024-03-31 13:04:23.000000 py4phi-0.9.0/cli/cli_main.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4512 2024-03-31 13:04:23.000000 py4phi-0.9.0/cli/descriptions.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.832988 py4phi-0.9.0/cli/encryption/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-0.9.0/cli/encryption/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8938 2024-04-07 09:05:07.000000 py4phi-0.9.0/cli/encryption/encryption.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1807 2024-03-30 22:00:06.000000 py4phi-0.9.0/cli/encryption/model_encryption.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-03-30 22:00:06.000000 py4phi-0.9.0/cli/utils.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.836988 py4phi-0.9.0/py4phi/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       78 2024-04-04 21:26:02.000000 py4phi-0.9.0/py4phi/__init__.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.836988 py4phi-0.9.0/py4phi/_encryption/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 08:44:07.000000 py4phi-0.9.0/py4phi/_encryption/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4530 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/_encryption/_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3248 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/_encryption/_model_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1903 2024-04-04 20:31:34.000000 py4phi-0.9.0/py4phi/_encryption/_pandas_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2154 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/_encryption/_polars_encryptor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2385 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/_encryption/_pyspark_encryptor.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.836988 py4phi-0.9.0/py4phi/analytics/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-27 20:27:56.000000 py4phi-0.9.0/py4phi/analytics/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      386 2024-03-30 16:13:27.000000 py4phi-0.9.0/py4phi/analytics/base_analytics.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     7134 2024-04-03 20:50:33.000000 py4phi-0.9.0/py4phi/analytics/feature_selection.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8868 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/analytics/principal_component_analysis.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4619 2024-04-04 20:31:34.000000 py4phi-0.9.0/py4phi/config_processor.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      680 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/consts.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    16943 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/controller.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4470 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/core.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.840988 py4phi-0.9.0/py4phi/dataset_handlers/
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-04 14:14:53.000000 py4phi-0.9.0/py4phi/dataset_handlers/__init__.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     6097 2024-03-27 20:27:56.000000 py4phi-0.9.0/py4phi/dataset_handlers/base_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3117 2024-04-04 20:31:34.000000 py4phi-0.9.0/py4phi/dataset_handlers/pandas_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3084 2024-04-04 20:31:34.000000 py4phi-0.9.0/py4phi/dataset_handlers/polars_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4235 2024-04-04 20:31:34.000000 py4phi-0.9.0/py4phi/dataset_handlers/pyspark_dataset_handler.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3636 2024-04-02 21:42:25.000000 py4phi-0.9.0/py4phi/dataset_handlers/pyspark_write_utils.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      553 2024-02-24 17:29:06.000000 py4phi-0.9.0/py4phi/log4j.properties
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      371 2024-04-07 09:05:07.000000 py4phi-0.9.0/py4phi/logger_setup.py
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      648 2024-03-27 20:27:56.000000 py4phi-0.9.0/py4phi/utils.py
-drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:25:07.840988 py4phi-0.9.0/py4phi.egg-info/
--rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    21742 2024-04-07 20:25:07.000000 py4phi-0.9.0/py4phi.egg-info/PKG-INFO
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1303 2024-04-07 20:25:07.000000 py4phi-0.9.0/py4phi.egg-info/SOURCES.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        1 2024-04-07 20:25:07.000000 py4phi-0.9.0/py4phi.egg-info/dependency_links.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       45 2024-04-07 20:25:07.000000 py4phi-0.9.0/py4phi.egg-info/entry_points.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-04-07 20:25:07.000000 py4phi-0.9.0/py4phi.egg-info/requires.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       11 2024-04-07 20:25:07.000000 py4phi-0.9.0/py4phi.egg-info/top_level.txt
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1417 2024-04-07 20:14:44.000000 py4phi-0.9.0/pyproject.toml
--rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       38 2024-04-07 20:25:07.840988 py4phi-0.9.0/setup.cfg
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    11357 2024-04-07 09:44:34.000000 py4phi-0.9.1/LICENSE
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1873 2024-04-07 10:07:22.000000 py4phi-0.9.1/NOTICE
+-rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    21919 2024-04-07 20:48:09.236741 py4phi-0.9.1/PKG-INFO
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     7409 2024-04-07 20:28:28.000000 py4phi-0.9.1/README.md
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/cli/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-0.9.1/cli/__init__.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/cli/analytics/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-30 22:00:06.000000 py4phi-0.9.1/cli/analytics/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3764 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/analytics/feature_selection.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3725 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/analytics/principal_component_analysis.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      497 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/cli_main.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4512 2024-03-31 13:04:23.000000 py4phi-0.9.1/cli/descriptions.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/cli/encryption/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-23 22:09:20.000000 py4phi-0.9.1/cli/encryption/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8938 2024-04-07 09:05:07.000000 py4phi-0.9.1/cli/encryption/encryption.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1807 2024-03-30 22:00:06.000000 py4phi-0.9.1/cli/encryption/model_encryption.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-03-30 22:00:06.000000 py4phi-0.9.1/cli/utils.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.232740 py4phi-0.9.1/py4phi/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       78 2024-04-04 21:26:02.000000 py4phi-0.9.1/py4phi/__init__.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi/_encryption/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 08:44:07.000000 py4phi-0.9.1/py4phi/_encryption/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4530 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3248 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_model_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1903 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/_encryption/_pandas_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2154 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_polars_encryptor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     2385 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/_encryption/_pyspark_encryptor.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi/analytics/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-03-27 20:27:56.000000 py4phi-0.9.1/py4phi/analytics/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      386 2024-03-30 16:13:27.000000 py4phi-0.9.1/py4phi/analytics/base_analytics.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     7134 2024-04-03 20:50:33.000000 py4phi-0.9.1/py4phi/analytics/feature_selection.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     8868 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/analytics/principal_component_analysis.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4619 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/config_processor.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      680 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/consts.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)    16943 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/controller.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4470 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/core.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi/dataset_handlers/
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        0 2024-02-04 14:14:53.000000 py4phi-0.9.1/py4phi/dataset_handlers/__init__.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     6097 2024-03-27 20:27:56.000000 py4phi-0.9.1/py4phi/dataset_handlers/base_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3117 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/dataset_handlers/pandas_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3084 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/dataset_handlers/polars_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     4235 2024-04-04 20:31:34.000000 py4phi-0.9.1/py4phi/dataset_handlers/pyspark_dataset_handler.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     3636 2024-04-02 21:42:25.000000 py4phi-0.9.1/py4phi/dataset_handlers/pyspark_write_utils.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      553 2024-02-24 17:29:06.000000 py4phi-0.9.1/py4phi/log4j.properties
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      371 2024-04-07 09:05:07.000000 py4phi-0.9.1/py4phi/logger_setup.py
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      648 2024-03-27 20:27:56.000000 py4phi-0.9.1/py4phi/utils.py
+drwxrwxr-x   0 volodymyr  (1000) volodymyr  (1000)        0 2024-04-07 20:48:09.236741 py4phi-0.9.1/py4phi.egg-info/
+-rw-r--r--   0 volodymyr  (1000) volodymyr  (1000)    21919 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/PKG-INFO
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1303 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/SOURCES.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)        1 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/dependency_links.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       45 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/entry_points.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)      325 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/requires.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       11 2024-04-07 20:48:09.000000 py4phi-0.9.1/py4phi.egg-info/top_level.txt
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)     1573 2024-04-07 20:47:52.000000 py4phi-0.9.1/pyproject.toml
+-rw-rw-r--   0 volodymyr  (1000) volodymyr  (1000)       38 2024-04-07 20:48:09.236741 py4phi-0.9.1/setup.cfg
```

### Comparing `py4phi-0.9.0/LICENSE` & `py4phi-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/NOTICE` & `py4phi-0.9.1/NOTICE`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/PKG-INFO` & `py4phi-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4phi
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for encryption/decryption and analysis of sensitive data.
 Author-email: Volodymyr Kiriushyn <zalorderon3331@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,18 @@
 Project-URL: repository, https://github.com/volodymyrkir/py4phi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Topic :: Security
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: iniconfig>=2.0.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: pluggy>=1.3.0
```

### Comparing `py4phi-0.9.0/README.md` & `py4phi-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/cli/analytics/feature_selection.py` & `py4phi-0.9.1/cli/analytics/feature_selection.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/cli/analytics/principal_component_analysis.py` & `py4phi-0.9.1/cli/analytics/principal_component_analysis.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/cli/descriptions.py` & `py4phi-0.9.1/cli/descriptions.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/cli/encryption/encryption.py` & `py4phi-0.9.1/cli/encryption/encryption.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/cli/encryption/model_encryption.py` & `py4phi-0.9.1/cli/encryption/model_encryption.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/_encryption/_encryptor.py` & `py4phi-0.9.1/py4phi/_encryption/_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/_encryption/_model_encryptor.py` & `py4phi-0.9.1/py4phi/_encryption/_model_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/_encryption/_pandas_encryptor.py` & `py4phi-0.9.1/py4phi/_encryption/_pandas_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/_encryption/_polars_encryptor.py` & `py4phi-0.9.1/py4phi/_encryption/_polars_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/_encryption/_pyspark_encryptor.py` & `py4phi-0.9.1/py4phi/_encryption/_pyspark_encryptor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/analytics/feature_selection.py` & `py4phi-0.9.1/py4phi/analytics/feature_selection.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/analytics/principal_component_analysis.py` & `py4phi-0.9.1/py4phi/analytics/principal_component_analysis.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/config_processor.py` & `py4phi-0.9.1/py4phi/config_processor.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/consts.py` & `py4phi-0.9.1/py4phi/consts.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/controller.py` & `py4phi-0.9.1/py4phi/controller.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/core.py` & `py4phi-0.9.1/py4phi/core.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/dataset_handlers/base_dataset_handler.py` & `py4phi-0.9.1/py4phi/dataset_handlers/base_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/dataset_handlers/pandas_dataset_handler.py` & `py4phi-0.9.1/py4phi/dataset_handlers/pandas_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/dataset_handlers/polars_dataset_handler.py` & `py4phi-0.9.1/py4phi/dataset_handlers/polars_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/dataset_handlers/pyspark_dataset_handler.py` & `py4phi-0.9.1/py4phi/dataset_handlers/pyspark_dataset_handler.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/dataset_handlers/pyspark_write_utils.py` & `py4phi-0.9.1/py4phi/dataset_handlers/pyspark_write_utils.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/log4j.properties` & `py4phi-0.9.1/py4phi/log4j.properties`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi/utils.py` & `py4phi-0.9.1/py4phi/utils.py`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/py4phi.egg-info/PKG-INFO` & `py4phi-0.9.1/py4phi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py4phi
-Version: 0.9.0
+Version: 0.9.1
 Summary: A library for encryption/decryption and analysis of sensitive data.
 Author-email: Volodymyr Kiriushyn <zalorderon3331@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -208,14 +208,18 @@
 Project-URL: repository, https://github.com/volodymyrkir/py4phi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Healthcare Industry
+Classifier: Topic :: Security
+Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 Requires-Dist: iniconfig>=2.0.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: pluggy>=1.3.0
```

### Comparing `py4phi-0.9.0/py4phi.egg-info/SOURCES.txt` & `py4phi-0.9.1/py4phi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py4phi-0.9.0/pyproject.toml` & `py4phi-0.9.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,24 +5,28 @@
 [tool.setuptools.packages.find]
 include = ["py4phi*", "cli*"]
 
 [project]
 name="py4phi"
 requires-python = ">=3.10"
 license={file="LICENSE"}
-version = "0.9.0"
+version = "0.9.1"
 description="A library for encryption/decryption and analysis of sensitive data."
 readme = "README.md"
 classifiers=[
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: Healthcare Industry",
+    "Topic :: Security",
+    "Topic :: Scientific/Engineering"
 ]
 
 authors = [
   {name = "Volodymyr Kiriushyn", email = "zalorderon3331@gmail.com" }
 ]
 dependencies = [
     "iniconfig>=2.0.0",
```

