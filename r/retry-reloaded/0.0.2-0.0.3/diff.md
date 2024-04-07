# Comparing `tmp/retry-reloaded-0.0.2.tar.gz` & `tmp/retry-reloaded-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry-reloaded-0.0.2.tar", last modified: Wed Apr  3 16:43:01 2024, max compression
+gzip compressed data, was "retry-reloaded-0.0.3.tar", last modified: Sun Apr  7 16:14:33 2024, max compression
```

## Comparing `retry-reloaded-0.0.2.tar` & `retry-reloaded-0.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.414313 retry-reloaded-0.0.2/retry/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/retry_reloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_retry_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.112636 retry-reloaded-0.0.3/retry_reloaded/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/retry_reloaded/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/retry_reloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 16:14:33.000000 retry-reloaded-0.0.3/retry_reloaded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:14:33.116637 retry-reloaded-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2007 2024-04-07 16:14:25.000000 retry-reloaded-0.0.3/tests/test_retry_args.py
```

### Comparing `retry-reloaded-0.0.2/LICENSE` & `retry-reloaded-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.2/PKG-INFO` & `retry-reloaded-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,16 +19,16 @@
 ## Install
 `pip install retry-reloaded`
 
 ## Features:
 
 - **Exception Handling**: Retry based on specific exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
-- **Timeout**: Specify the maximum time to spend on retries. Timeout check happens right before retry execution of the wrapped function.
-- **Deadline**: Define a deadline for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
+- **Timeout**: Specify the maximum time in seconds to spend on retries. Timeout check happens right before retry execution of the wrapped function.
+- **Deadline**: Define a deadline in seconds for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
 - **Retry Callback**: Execute a callback function between retry attempts.
 - **Successful Retry Callback**: Perform an action after a successful retry.
 - **Failure Callback**: Define a callback function after failing all retries.
 - **Logging control**: Define which logger (or no logger) to use for logging retries and exceptions.
 
 ## API
@@ -38,15 +38,15 @@
 - Backoff strategies: `FixedBackOff`, `LinearBackOff`, `ExponentialBackOff`, `RandomUniformBackOff`
 
 
 ## Examples
 
 ```python
 # public API
-from retry import (
+from retry_reloaded import (
     retry,
     callback_factory,
     CallbackFactory,
     FixedBackOff,
     LinearBackOff,
     ExponentialBackOff,
     RandomUniformBackOff,
```

### Comparing `retry-reloaded-0.0.2/README.md` & `retry-reloaded-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 ## Install
 `pip install retry-reloaded`
 
 ## Features:
 
 - **Exception Handling**: Retry based on specific exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
-- **Timeout**: Specify the maximum time to spend on retries. Timeout check happens right before retry execution of the wrapped function.
-- **Deadline**: Define a deadline for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
+- **Timeout**: Specify the maximum time in seconds to spend on retries. Timeout check happens right before retry execution of the wrapped function.
+- **Deadline**: Define a deadline in seconds for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
 - **Retry Callback**: Execute a callback function between retry attempts.
 - **Successful Retry Callback**: Perform an action after a successful retry.
 - **Failure Callback**: Define a callback function after failing all retries.
 - **Logging control**: Define which logger (or no logger) to use for logging retries and exceptions.
 
 ## API
@@ -24,15 +24,15 @@
 - Backoff strategies: `FixedBackOff`, `LinearBackOff`, `ExponentialBackOff`, `RandomUniformBackOff`
 
 
 ## Examples
 
 ```python
 # public API
-from retry import (
+from retry_reloaded import (
     retry,
     callback_factory,
     CallbackFactory,
     FixedBackOff,
     LinearBackOff,
     ExponentialBackOff,
     RandomUniformBackOff,
```

### Comparing `retry-reloaded-0.0.2/retry/__init__.py` & `retry-reloaded-0.0.3/retry_reloaded/__init__.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.2/retry/_exceptions.py` & `retry-reloaded-0.0.3/retry_reloaded/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.2/retry/_logging.py` & `retry-reloaded-0.0.3/retry_reloaded/_logging.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.2/retry/_validate.py` & `retry-reloaded-0.0.3/retry_reloaded/_validate.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.2/retry/backoff.py` & `retry-reloaded-0.0.3/retry_reloaded/backoff.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.2/retry/callback.py` & `retry-reloaded-0.0.3/retry_reloaded/callback.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.2/retry/retry.py` & `retry-reloaded-0.0.3/retry_reloaded/retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     Decorator that adds retry functionality to a function.
 
     Parameters:
         exceptions (Tuple[Type[Exception]], optional): A tuple of exception types that should trigger a retry.
             Defaults to (Exception,), meaning any exception will trigger a retry.
         max_retries (int, optional): The maximum number of retry attempts. Defaults to None (unlimited retries).
         backoff (BackOff, optional): The backoff strategy to use between retry attempts.
-            Defaults to FixedBackOff(base_delay=0).
+            Defaults to FixedBackOff(base_delay=0) with base_delay referring to seconds.
         timeout (float, optional): The maximum time (in seconds) to spend on retries. Defaults to None (no timeout).
             Timeout check happens right before retry execution of the wrapped function.
         deadline (float, optional): The deadline (in seconds) for retries. Defaults to None (no deadline).
             Deadline check happens right after the retry execution of the wrapped function.
         logger (logging.Logger, optional): The logger instance to use for logging retry attempts. Defaults to retry_logger.
         log_retry_traceback (bool, optional): Whether to log the traceback of exceptions triggering retries.
             Defaults to False.
```

### Comparing `retry-reloaded-0.0.2/retry_reloaded.egg-info/PKG-INFO` & `retry-reloaded-0.0.3/retry_reloaded.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,16 +19,16 @@
 ## Install
 `pip install retry-reloaded`
 
 ## Features:
 
 - **Exception Handling**: Retry based on specific exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
-- **Timeout**: Specify the maximum time to spend on retries. Timeout check happens right before retry execution of the wrapped function.
-- **Deadline**: Define a deadline for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
+- **Timeout**: Specify the maximum time in seconds to spend on retries. Timeout check happens right before retry execution of the wrapped function.
+- **Deadline**: Define a deadline in seconds for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
 - **Retry Callback**: Execute a callback function between retry attempts.
 - **Successful Retry Callback**: Perform an action after a successful retry.
 - **Failure Callback**: Define a callback function after failing all retries.
 - **Logging control**: Define which logger (or no logger) to use for logging retries and exceptions.
 
 ## API
@@ -38,15 +38,15 @@
 - Backoff strategies: `FixedBackOff`, `LinearBackOff`, `ExponentialBackOff`, `RandomUniformBackOff`
 
 
 ## Examples
 
 ```python
 # public API
-from retry import (
+from retry_reloaded import (
     retry,
     callback_factory,
     CallbackFactory,
     FixedBackOff,
     LinearBackOff,
     ExponentialBackOff,
     RandomUniformBackOff,
```

### Comparing `retry-reloaded-0.0.2/setup.py` & `retry-reloaded-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="retry-reloaded",
-    version="0.0.2",
+    version="0.0.3",
     description="A simple Python library for retrying functions \
         with various backoff and callback strategies.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/chrisK824/retry",
     author="Chris Karvouniaris",
     author_email="christos.karvouniaris247@gmail.com",
```

### Comparing `retry-reloaded-0.0.2/tests/test_backoff.py` & `retry-reloaded-0.0.3/tests/test_backoff.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from retry.backoff import (
+from retry_reloaded.backoff import (
     FixedBackOff,
     LinearBackOff,
     RandomUniformBackOff,
     ExponentialBackOff,
 )
 import pytest
```

### Comparing `retry-reloaded-0.0.2/tests/test_callback.py` & `retry-reloaded-0.0.3/tests/test_callback.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from retry.callback import CallbackFactory, callback_factory
+from retry_reloaded.callback import CallbackFactory, callback_factory
 import pytest
 
 
 def test_CallbackFactory_callable_function():
     def dummy_func():
         pass
```

### Comparing `retry-reloaded-0.0.2/tests/test_retry.py` & `retry-reloaded-0.0.3/tests/test_retry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 from time import sleep
-from retry.retry import retry
-from retry._exceptions import (
+from retry_reloaded import retry
+from retry_reloaded._exceptions import (
     MaxRetriesException,
     RetriesTimeoutException,
     RetriesDeadlineException
 )
-from retry.backoff import FixedBackOff
+from retry_reloaded.backoff import FixedBackOff
 
 
 def test_successful_execution():
     retries = 0
 
     @retry(max_retries=3)
     def successful_function():
```

### Comparing `retry-reloaded-0.0.2/tests/test_retry_args.py` & `retry-reloaded-0.0.3/tests/test_retry_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import pytest
-from retry.retry import retry
+from retry_reloaded import retry
 
 
 def test_valid_arguments():
     @retry()
     def valid_function():
         return "Valid function"
```

