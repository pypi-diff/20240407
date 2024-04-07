# Comparing `tmp/msgraphhelper-0.2.0.tar.gz` & `tmp/msgraphhelper-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgraphhelper-0.2.0.tar", last modified: Mon Apr  1 17:23:10 2024, max compression
+gzip compressed data, was "msgraphhelper-0.3.0.tar", last modified: Sun Apr  7 18:34:36 2024, max compression
```

## Comparing `msgraphhelper-0.2.0.tar` & `msgraphhelper-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.438072 msgraphhelper-0.2.0/msgraphhelper/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/odata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/msgraphhelper/url.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/msgraphhelper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 17:23:10.000000 msgraphhelper-0.2.0/msgraphhelper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 17:23:10.442072 msgraphhelper-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/test/test_odata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-01 17:23:06.000000 msgraphhelper-0.2.0/test/test_url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:34:36.845193 msgraphhelper-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-07 18:34:36.841193 msgraphhelper-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11464 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:34:36.841193 msgraphhelper-0.3.0/msgraphhelper/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/msgraphhelper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10629 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/msgraphhelper/odata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/msgraphhelper/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/msgraphhelper/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/msgraphhelper/url.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:34:36.841193 msgraphhelper-0.3.0/msgraphhelper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12550 2024-04-07 18:34:36.000000 msgraphhelper-0.3.0/msgraphhelper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-07 18:34:36.000000 msgraphhelper-0.3.0/msgraphhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:34:36.000000 msgraphhelper-0.3.0/msgraphhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-07 18:34:36.000000 msgraphhelper-0.3.0/msgraphhelper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 18:34:36.000000 msgraphhelper-0.3.0/msgraphhelper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:34:36.845193 msgraphhelper-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:34:36.841193 msgraphhelper-0.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/test/test_odata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-07 18:34:32.000000 msgraphhelper-0.3.0/test/test_url.py
```

### Comparing `msgraphhelper-0.2.0/LICENSE` & `msgraphhelper-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.2.0/PKG-INFO` & `msgraphhelper-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphhelper
-Version: 0.2.0
+Version: 0.3.0
 Summary: Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions
 Author-email: Giles Antonio Radford <moof@metamoof.net>
 Project-URL: Homepage, https://github.com/metamoof/msgraphhelper
 Project-URL: Issues, https://github.com/metamoof/msgraphhelper/issues
 Keywords: azure-functions,ms-graph,graph,suscription,Webhooks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `msgraphhelper-0.2.0/README.md` & `msgraphhelper-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.2.0/msgraphhelper/odata.py` & `msgraphhelper-0.3.0/msgraphhelper/odata.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,7 +305,18 @@
         for response in responses:
             resptext = response.text
             # remove random UTF8 BOMs that BC can add if response is a number
             resptext = resptext.replace("\ufeff", "")
             for resp in json.loads(resptext)["responses"]:
                 self[resp["id"]] = resp
         return super().__init__()
+
+    def errors(self) -> dict:
+        """
+        Get all the responses that returned an error
+
+        :return: A dictionary of all the responses that returned an error
+        :rtype: dict
+        """
+        return dict(
+            (key, value) for key, value in self.items() if value["status"] >= 300
+        )
```

### Comparing `msgraphhelper-0.2.0/msgraphhelper/session.py` & `msgraphhelper-0.3.0/msgraphhelper/session.py`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.2.0/msgraphhelper/subscriptions.py` & `msgraphhelper-0.3.0/msgraphhelper/subscriptions.py`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.2.0/msgraphhelper/url.py` & `msgraphhelper-0.3.0/msgraphhelper/url.py`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.2.0/msgraphhelper.egg-info/PKG-INFO` & `msgraphhelper-0.3.0/msgraphhelper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgraphhelper
-Version: 0.2.0
+Version: 0.3.0
 Summary: Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions
 Author-email: Giles Antonio Radford <moof@metamoof.net>
 Project-URL: Homepage, https://github.com/metamoof/msgraphhelper
 Project-URL: Issues, https://github.com/metamoof/msgraphhelper/issues
 Keywords: azure-functions,ms-graph,graph,suscription,Webhooks
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `msgraphhelper-0.2.0/pyproject.toml` & `msgraphhelper-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msgraphhelper"
-version = "0.2.0"
+version = "0.3.0"
 description = "Handle MS Graph Change Notifications in a Pythonic manner in Azure Functions"
 readme = "README.md"
 authors = [{ name = "Giles Antonio Radford", email = "moof@metamoof.net" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `msgraphhelper-0.2.0/test/test_odata.py` & `msgraphhelper-0.3.0/test/test_odata.py`

 * *Files identical despite different names*

### Comparing `msgraphhelper-0.2.0/test/test_url.py` & `msgraphhelper-0.3.0/test/test_url.py`

 * *Files identical despite different names*

