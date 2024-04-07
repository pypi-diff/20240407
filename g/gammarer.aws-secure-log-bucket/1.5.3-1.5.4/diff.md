# Comparing `tmp/gammarer.aws-secure-log-bucket-1.5.3.tar.gz` & `tmp/gammarer.aws-secure-log-bucket-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-log-bucket-1.5.3.tar", last modified: Sun Mar 31 18:22:20 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-log-bucket-1.5.4.tar", last modified: Sun Apr  7 18:22:24 2024, max compression
```

## Comparing `gammarer.aws-secure-log-bucket-1.5.3.tar` & `gammarer.aws-secure-log-bucket-1.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:22:20.655442 gammarer.aws-secure-log-bucket-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-31 18:22:20.655442 gammarer.aws-secure-log-bucket-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 18:22:20.655442 gammarer.aws-secure-log-bucket-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:22:20.651442 gammarer.aws-secure-log-bucket-1.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:22:20.651442 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:22:20.655442 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:22:20.655442 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24436 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:22:20.655442 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-31 18:22:20.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-31 18:22:20.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:22:20.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-31 18:22:20.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 18:22:20.000000 gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.088228 gammarer.aws-secure-log-bucket-1.5.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.088228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (127)    13209 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24438 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:22:09.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:22:24.092228 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 18:22:24.000000 gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/LICENSE` & `gammarer.aws-secure-log-bucket-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/PKG-INFO` & `gammarer.aws-secure-log-bucket-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-log-bucket
-Version: 1.5.3
+Version: 1.5.4
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarer/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/README.md` & `gammarer.aws-secure-log-bucket-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/setup.py` & `gammarer.aws-secure-log-bucket-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-log-bucket",
-    "version": "1.5.3",
+    "version": "1.5.4",
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_log_bucket",
         "gammarer.aws_secure_log_bucket._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_log_bucket._jsii": [
-            "aws-secure-log-bucket@1.5.3.jsii.tgz"
+            "aws-secure-log-bucket@1.5.4.jsii.tgz"
         ],
         "gammarer.aws_secure_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/__init__.py` & `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py` & `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer/aws_secure_log_bucket/_jsii/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import constructs._jsii
 import gammarer.aws_secure_bucket._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-log-bucket",
-    "1.5.3",
+    "1.5.4",
     __name__[0:-6],
-    "aws-secure-log-bucket@1.5.3.jsii.tgz",
+    "aws-secure-log-bucket@1.5.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO` & `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-log-bucket
-Version: 1.5.3
+Version: 1.5.4
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/gammarer/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-log-bucket-1.5.3/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt` & `gammarer.aws-secure-log-bucket-1.5.4/src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_log_bucket.egg-info/SOURCES.txt
 src/gammarer.aws_secure_log_bucket.egg-info/dependency_links.txt
 src/gammarer.aws_secure_log_bucket.egg-info/requires.txt
 src/gammarer.aws_secure_log_bucket.egg-info/top_level.txt
 src/gammarer/aws_secure_log_bucket/__init__.py
 src/gammarer/aws_secure_log_bucket/py.typed
 src/gammarer/aws_secure_log_bucket/_jsii/__init__.py
-src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.3.jsii.tgz
+src/gammarer/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@1.5.4.jsii.tgz
```

