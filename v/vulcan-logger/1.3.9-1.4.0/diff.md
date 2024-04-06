# Comparing `tmp/vulcan-logger-1.3.9.tar.gz` & `tmp/vulcan-logger-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-logger-1.3.9.tar", last modified: Sat Apr  6 21:11:36 2024, max compression
+gzip compressed data, was "vulcan-logger-1.4.0.tar", last modified: Sat Apr  6 21:54:21 2024, max compression
```

## Comparing `vulcan-logger-1.3.9.tar` & `vulcan-logger-1.4.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:11:36.348425 vulcan-logger-1.3.9/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-06 21:11:36.348425 vulcan-logger-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 21:11:36.348425 vulcan-logger-1.3.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:11:36.344425 vulcan-logger-1.3.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/tests/test_encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5513 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/tests/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:11:36.348425 vulcan-logger-1.3.9/vulcan_logger/
--rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/vulcan_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/vulcan_logger/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/vulcan_logger/encoder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4152 2024-04-06 21:11:27.000000 vulcan-logger-1.3.9/vulcan_logger/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:11:36.348425 vulcan-logger-1.3.9/vulcan_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-06 21:11:36.000000 vulcan-logger-1.3.9/vulcan_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 21:11:36.000000 vulcan-logger-1.3.9/vulcan_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 21:11:36.000000 vulcan-logger-1.3.9/vulcan_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 21:11:36.000000 vulcan-logger-1.3.9/vulcan_logger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 21:11:36.000000 vulcan-logger-1.3.9/vulcan_logger.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:54:21.107793 vulcan-logger-1.4.0/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1070 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-06 21:54:21.107793 vulcan-logger-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 21:54:21.107793 vulcan-logger-1.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      400 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:54:21.103793 vulcan-logger-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/tests/test_encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5513 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/tests/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:54:21.107793 vulcan-logger-1.4.0/vulcan_logger/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       41 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/vulcan_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3677 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/vulcan_logger/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1529 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/vulcan_logger/encoder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4152 2024-04-06 21:54:13.000000 vulcan-logger-1.4.0/vulcan_logger/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 21:54:21.107793 vulcan-logger-1.4.0/vulcan_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4463 2024-04-06 21:54:21.000000 vulcan-logger-1.4.0/vulcan_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-06 21:54:21.000000 vulcan-logger-1.4.0/vulcan_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 21:54:21.000000 vulcan-logger-1.4.0/vulcan_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 21:54:21.000000 vulcan-logger-1.4.0/vulcan_logger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 21:54:21.000000 vulcan-logger-1.4.0/vulcan_logger.egg-info/top_level.txt
```

### Comparing `vulcan-logger-1.3.9/LICENSE` & `vulcan-logger-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.9/PKG-INFO` & `vulcan-logger-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.9
+Version: 1.4.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

### Comparing `vulcan-logger-1.3.9/tests/test_decorator.py` & `vulcan-logger-1.4.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.9/tests/test_encoder.py` & `vulcan-logger-1.4.0/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.9/tests/test_logger.py` & `vulcan-logger-1.4.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.9/vulcan_logger/decorator.py` & `vulcan-logger-1.4.0/vulcan_logger/decorator.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.9/vulcan_logger/encoder.py` & `vulcan-logger-1.4.0/vulcan_logger/encoder.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.9/vulcan_logger/logger.py` & `vulcan-logger-1.4.0/vulcan_logger/logger.py`

 * *Files identical despite different names*

### Comparing `vulcan-logger-1.3.9/vulcan_logger.egg-info/PKG-INFO` & `vulcan-logger-1.4.0/vulcan_logger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-logger
-Version: 1.3.9
+Version: 1.4.0
 Summary: A logging utility package with colored logs.
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: coloredlogs
 
 # Vulcan Logger
 Vulcan Logger is a Python package that provides a customizable logging utility with support for automatic inclusion of caller's filename and line number in logs. It aims to simplify logging in Python applications by offering features such as log level configuration, colored logs, and conditional logging.
```

