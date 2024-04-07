# Comparing `tmp/btc_embedded-24.1.2.tar.gz` & `tmp/btc_embedded-24.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btc_embedded-24.1.2.tar", last modified: Fri Apr  5 09:21:34 2024, max compression
+gzip compressed data, was "btc_embedded-24.1.3.tar", last modified: Sun Apr  7 08:01:20 2024, max compression
```

## Comparing `btc_embedded-24.1.2.tar` & `btc_embedded-24.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 09:21:34.440331 btc_embedded-24.1.2/
--rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/LICENSE.txt
--rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/MANIFEST.in
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 09:21:34.440416 btc_embedded-24.1.2/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/README.md
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 09:21:34.439574 btc_embedded-24.1.2/btc_embedded/
--rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/btc_embedded/__init__.py
--rw-r--r--   0 thabok     (501) staff       (20)    21322 2024-04-05 09:18:51.000000 btc_embedded-24.1.2/btc_embedded/api.py
--rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/btc_embedded/btc_config.yml
--rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/btc_embedded/btc_summary_report.template
--rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.2/btc_embedded/config.py
--rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/btc_embedded/reporting.py
--rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.2/btc_embedded/util.py
-drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-05 09:21:34.440218 btc_embedded-24.1.2/btc_embedded.egg-info/
--rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-05 09:21:34.000000 btc_embedded-24.1.2/btc_embedded.egg-info/PKG-INFO
--rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-05 09:21:34.000000 btc_embedded-24.1.2/btc_embedded.egg-info/SOURCES.txt
--rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-05 09:21:34.000000 btc_embedded-24.1.2/btc_embedded.egg-info/dependency_links.txt
--rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-05 09:21:34.000000 btc_embedded-24.1.2/btc_embedded.egg-info/requires.txt
--rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-05 09:21:34.000000 btc_embedded-24.1.2/btc_embedded.egg-info/top_level.txt
--rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-05 09:21:34.440619 btc_embedded-24.1.2/setup.cfg
--rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-05 09:17:15.000000 btc_embedded-24.1.2/setup.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-07 08:01:20.042389 btc_embedded-24.1.3/
+-rw-r--r--   0 thabok     (501) staff       (20)     1079 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/LICENSE.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       76 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/MANIFEST.in
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-07 08:01:20.042464 btc_embedded-24.1.3/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)     1791 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/README.md
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-07 08:01:20.041504 btc_embedded-24.1.3/btc_embedded/
+-rw-r--r--   0 thabok     (501) staff       (20)      357 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/__init__.py
+-rw-r--r--   0 thabok     (501) staff       (20)    21391 2024-04-07 08:00:27.000000 btc_embedded-24.1.3/btc_embedded/api.py
+-rw-r--r--   0 thabok     (501) staff       (20)     2068 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/btc_config.yml
+-rw-r--r--   0 thabok     (501) staff       (20)    35498 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/btc_summary_report.template
+-rw-r--r--   0 thabok     (501) staff       (20)     3670 2024-01-24 10:47:06.000000 btc_embedded-24.1.3/btc_embedded/config.py
+-rw-r--r--   0 thabok     (501) staff       (20)     4499 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/reporting.py
+-rw-r--r--   0 thabok     (501) staff       (20)     1866 2024-01-16 13:29:56.000000 btc_embedded-24.1.3/btc_embedded/util.py
+drwxr-xr-x   0 thabok     (501) staff       (20)        0 2024-04-07 08:01:20.042254 btc_embedded-24.1.3/btc_embedded.egg-info/
+-rw-r--r--   0 thabok     (501) staff       (20)      818 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/PKG-INFO
+-rw-r--r--   0 thabok     (501) staff       (20)      415 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/SOURCES.txt
+-rw-r--r--   0 thabok     (501) staff       (20)        1 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/dependency_links.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       16 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/requires.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       13 2024-04-07 08:01:20.000000 btc_embedded-24.1.3/btc_embedded.egg-info/top_level.txt
+-rw-r--r--   0 thabok     (501) staff       (20)       79 2024-04-07 08:01:20.042695 btc_embedded-24.1.3/setup.cfg
+-rw-r--r--   0 thabok     (501) staff       (20)      976 2024-04-07 08:00:31.000000 btc_embedded-24.1.3/setup.py
```

### Comparing `btc_embedded-24.1.2/LICENSE.txt` & `btc_embedded-24.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.2/PKG-INFO` & `btc_embedded-24.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc_embedded
-Version: 24.1.2
+Version: 24.1.3
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.2/README.md` & `btc_embedded-24.1.3/README.md`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.2/btc_embedded/api.py` & `btc_embedded-24.1.3/btc_embedded/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,22 +120,23 @@
 
     def print_messages(self, search_string=None, severity=None):
         """Prints all messages since the last profile create/profile load.
         Optional filters are available:
         
         - severity: INFO, WARNING, ERROR or CRITICAL
         - search_string: only prints messages that contain the given string"""
-        path = f"/message-markers/{self.message_marker_date}/messages"
-        if search_string: path += '?search-string=' + search_string
-        if severity: path += ('&' if search_string else '?') + f"severity={severity}"
-        messages = self.get(path)
-        messages.sort(key=lambda msg: datetime.strptime(msg['date'], DATE_FORMAT))
-        for msg in messages:
-            print(f"[{msg['severity']}] {msg['message']}" + (f" (Hint: {msg['hint']})" if 'hint' in msg and msg['hint'] else ""))
-        print("\n")
+        if self.message_marker_date:
+            path = f"/message-markers/{self.message_marker_date}/messages"
+            if search_string: path += '?search-string=' + search_string
+            if severity: path += ('&' if search_string else '?') + f"severity={severity}"
+            messages = self.get(path)
+            messages.sort(key=lambda msg: datetime.strptime(msg['date'], DATE_FORMAT))
+            for msg in messages:
+                print(f"[{msg['severity']}] {msg['message']}" + (f" (Hint: {msg['hint']})" if 'hint' in msg and msg['hint'] else ""))
+            print("\n")
 
     # - - - - - - - - - - - - - - - - - - - - 
     #   DEPRICATED PUBLIC FUNCTIONS
     # - - - - - - - - - - - - - - - - - - - - 
 
     # Performs a get request on the given url extension
     def get_req(self, urlappendix, message=None):
```

### Comparing `btc_embedded-24.1.2/btc_embedded/btc_config.yml` & `btc_embedded-24.1.3/btc_embedded/btc_config.yml`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.2/btc_embedded/btc_summary_report.template` & `btc_embedded-24.1.3/btc_embedded/btc_summary_report.template`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.2/btc_embedded/config.py` & `btc_embedded-24.1.3/btc_embedded/config.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.2/btc_embedded/reporting.py` & `btc_embedded-24.1.3/btc_embedded/reporting.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.2/btc_embedded/util.py` & `btc_embedded-24.1.3/btc_embedded/util.py`

 * *Files identical despite different names*

### Comparing `btc_embedded-24.1.2/btc_embedded.egg-info/PKG-INFO` & `btc_embedded-24.1.3/btc_embedded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btc-embedded
-Version: 24.1.2
+Version: 24.1.3
 Summary: API wrapper for BTC EmbeddedPlatform 23.3p0 REST API
 Home-page: https://github.com/btc-embedded/btc-embedded
 Author: Thabo Krick
 Author-email: thabo.krick@btc-embedded.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `btc_embedded-24.1.2/setup.py` & `btc_embedded-24.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='btc_embedded',
-    version='24.1.2',
+    version='24.1.3',
     packages=['btc_embedded'],
     include_package_data=True,
     license='MIT',
     description='API wrapper for BTC EmbeddedPlatform 23.3p0 REST API',
     author='Thabo Krick',
     author_email='thabo.krick@btc-embedded.com',
     url='https://github.com/btc-embedded/btc-embedded',
```

