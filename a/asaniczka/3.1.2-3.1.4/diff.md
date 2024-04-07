# Comparing `tmp/asaniczka-3.1.2.tar.gz` & `tmp/asaniczka-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asaniczka-3.1.2.tar", last modified: Sat Apr  6 08:21:21 2024, max compression
+gzip compressed data, was "asaniczka-3.1.4.tar", last modified: Sun Apr  7 08:41:26 2024, max compression
```

## Comparing `asaniczka-3.1.2.tar` & `asaniczka-3.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:21:21.269658 asaniczka-3.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:21:21.269658 asaniczka-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-06 08:21:16.000000 asaniczka-3.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:21:21.269658 asaniczka-3.1.2/asaniczka/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 08:21:16.000000 asaniczka-3.1.2/asaniczka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-04-06 08:21:16.000000 asaniczka-3.1.2/asaniczka/db_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    34509 2024-04-06 08:21:16.000000 asaniczka-3.1.2/asaniczka/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-04-06 08:21:16.000000 asaniczka-3.1.2/asaniczka/scrape_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 08:21:21.269658 asaniczka-3.1.2/asaniczka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-06 08:21:21.000000 asaniczka-3.1.2/asaniczka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-06 08:21:21.000000 asaniczka-3.1.2/asaniczka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 08:21:21.000000 asaniczka-3.1.2/asaniczka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-06 08:21:21.000000 asaniczka-3.1.2/asaniczka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 08:21:21.000000 asaniczka-3.1.2/asaniczka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-06 08:21:16.000000 asaniczka-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 08:21:21.269658 asaniczka-3.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:41:26.823071 asaniczka-3.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-07 08:41:26.823071 asaniczka-3.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-07 08:41:22.000000 asaniczka-3.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:41:26.823071 asaniczka-3.1.4/asaniczka/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-07 08:41:22.000000 asaniczka-3.1.4/asaniczka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24084 2024-04-07 08:41:22.000000 asaniczka-3.1.4/asaniczka/db_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34505 2024-04-07 08:41:22.000000 asaniczka-3.1.4/asaniczka/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14168 2024-04-07 08:41:22.000000 asaniczka-3.1.4/asaniczka/scrape_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:41:26.823071 asaniczka-3.1.4/asaniczka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-04-07 08:41:26.000000 asaniczka-3.1.4/asaniczka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 08:41:26.000000 asaniczka-3.1.4/asaniczka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:41:26.000000 asaniczka-3.1.4/asaniczka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-07 08:41:26.000000 asaniczka-3.1.4/asaniczka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 08:41:26.000000 asaniczka-3.1.4/asaniczka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-07 08:41:22.000000 asaniczka-3.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 08:41:26.823071 asaniczka-3.1.4/setup.cfg
```

### Comparing `asaniczka-3.1.2/PKG-INFO` & `asaniczka-3.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaniczka
-Version: 3.1.2
+Version: 3.1.4
 Summary: All my commonly used fuctions
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/asaniczka_pip
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `asaniczka-3.1.2/README.md` & `asaniczka-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `asaniczka-3.1.2/asaniczka/db_tools.py` & `asaniczka-3.1.4/asaniczka/db_tools.py`

 * *Files identical despite different names*

### Comparing `asaniczka-3.1.2/asaniczka/main.py` & `asaniczka-3.1.4/asaniczka/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -512,19 +512,19 @@
                 response = helper_get_request_no_proxy(
                     url, headers=headers, timeout=timeout, session=session
                 )
         # pylint: disable=broad-except
         except Exception as error:
             if logger:
                 if logger_level_debug:
-                    logger.debug("Failed to POST request. %s", format_error(error))
+                    logger.debug("Failed to GET request. %s", format_error(error))
                 else:
-                    logger.warning("Failed to POST request. %s", format_error(error))
+                    logger.warning("Failed to GET request. %s", format_error(error))
             else:
-                print("Failed to POST request. %s", format_error(error))
+                print("Failed to GET request. %s", format_error(error))
 
             retries += 1
             continue
 
         if response.status_code == 200:
             # do the okay things
             content = response.text
@@ -696,22 +696,22 @@
     logger_level_debug: Optional[bool] = False,
     proxy: Union[str, None] = None,
     retry_count: int = 5,
     retry_sleep_time: int = 5,
     timeout: int = 45,
 ) -> str | None:
     """
-    Makes a basic HTTP POST request to the given URL.
+    Makes a basic HTTP GET request to the given URL.
 
     ### Responsibility:
-    - Make a POST request to a URL with options for handling exceptions, logging, proxies, payload, and session usage.
+    - Make a GET request to a URL with options for handling exceptions, logging, proxies, payload, and session usage.
     - Retry the request multiple times and raise an error if unsuccessful after specified retries.
 
     ### Args:
-    - `url`: The URL to make the POST request.
+    - `url`: The URL to make the GET request.
     - `headers`: The headers to be included in the request.
     - `payload`: The data to be sent in the request body.
     - `silence_exceptions`: Will not raise any exceptions if set to True.
     - `logger`: The logger instance to log warnings.
     - `logger_level_debug`: Whether to log warnings at debug level.
     - `proxy`: Proxy to use for the request.
     - `retry_count`: Number of times to retry the request.
@@ -888,22 +888,22 @@
             break
 
         # if not okay, then start logging and retrying
         if logger:
             # if logger level is said to be debug, do debug, otherwise it's a warning
             if logger_level_debug:
                 logger.debug(
-                    "Failed to get request. \
+                    "Failed to POST request. \
                     Status code %d, Response text: %s",
                     response.status_code,
                     format_error(response.text),
                 )
             else:
                 logger.warning(
-                    "Failed to get request. \
+                    "Failed to POST request. \
                     Status code %d, Response text: %s",
                     response.status_code,
                     format_error(response.text),
                 )
 
         if (
             response.status_code == 420
```

### Comparing `asaniczka-3.1.2/asaniczka/scrape_helper.py` & `asaniczka-3.1.4/asaniczka/scrape_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
             result = future.result()
             if result:
                 working_proxies.append(result)
 
     return working_proxies
 
 
-def download_proxies(url: str) -> list[Proxy]:
+def download_proxies(url: str, validate=True) -> list[Proxy]:
     """
     Downloads the proxies from your webshare live url
     """
 
     if not url:
         raise ValueError("No URL provided")
 
@@ -438,13 +438,17 @@
 
     response = asaniczka.get_request(url, timeout=5)
 
     if not response:
         raise ValueError("URL didn't recieve any data")
 
     lines = response.split("\n")
-    lines = [line.strip() for line in lines]
+    lines = [line.strip() for line in lines if ":" in line]
     proxies = [Proxy(line, ProxyProvider.WEBSHARE) for line in lines]
 
-    working_proxies = validate_proxies(proxies)
-    print("You have ", len(working_proxies), " working proxies!")
+    if validate:
+        working_proxies = validate_proxies(proxies)
+        print("You have ", len(working_proxies), " working proxies!")
+    else:
+        working_proxies = proxies
+
     return working_proxies
```

### Comparing `asaniczka-3.1.2/asaniczka.egg-info/PKG-INFO` & `asaniczka-3.1.4/asaniczka.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asaniczka
-Version: 3.1.2
+Version: 3.1.4
 Summary: All my commonly used fuctions
 Author-email: Asaniczka <asaniczka@gmail.com>
 Maintainer-email: Asaniczka <asaniczka@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/asaniczka/asaniczka_pip
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `asaniczka-3.1.2/pyproject.toml` & `asaniczka-3.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools >= 61.0', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "asaniczka"
-version = "3.1.2"
+version = "3.1.4"
 description = "All my commonly used fuctions"
 readme = "README.md"
 dependencies = [
   "pytz>=2022.1",
   "requests>=2.0",
   "playwright>=1.0.0",
   "tqdm>=4.0.0",
```

