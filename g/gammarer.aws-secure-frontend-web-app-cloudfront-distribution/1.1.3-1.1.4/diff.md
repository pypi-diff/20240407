# Comparing `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3.tar.gz` & `tmp/gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3.tar", last modified: Sun Mar 31 18:21:15 2024, max compression
+gzip compressed data, was "gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4.tar", last modified: Sun Apr  7 18:21:17 2024, max compression
```

## Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3.tar` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:15.467528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-31 18:21:15.467528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 18:21:15.467528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:15.463528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:15.467528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:15.467528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:15.467528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22231 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.1.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:21:01.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:21:15.467528 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-31 18:21:15.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-31 18:21:15.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:21:15.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-31 18:21:15.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-31 18:21:15.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2110 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.628636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:21:03.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:21:17.624636 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 18:21:17.000000 gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/LICENSE` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 1.1.3
+Version: 1.1.4
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/README.md` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/setup.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarer.aws-secure-frontend-web-app-cloudfront-distribution",
-    "version": "1.1.3",
+    "version": "1.1.4",
     "description": "AWS CloudFront distribution for frontend web app (spa) optimized.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution",
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii"
     ],
     "package_data": {
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution._jsii": [
-            "aws-secure-frontend-web-app-cloudfront-distribution@1.1.3.jsii.tgz"
+            "aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz"
         ],
         "gammarer.aws_secure_frontend_web_app_cloudfront_distribution": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 from typeguard import check_type
 
 import aws_cdk._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarer/aws-secure-frontend-web-app-cloudfront-distribution",
-    "1.1.3",
+    "1.1.4",
     __name__[0:-6],
-    "aws-secure-frontend-web-app-cloudfront-distribution@1.1.3.jsii.tgz",
+    "aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarer.aws-secure-frontend-web-app-cloudfront-distribution
-Version: 1.1.3
+Version: 1.1.4
 Summary: AWS CloudFront distribution for frontend web app (spa) optimized.
 Home-page: https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarer/aws-secure-frontend-web-app-cloudfront-distribution.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.3/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt` & `gammarer.aws-secure-frontend-web-app-cloudfront-distribution-1.1.4/src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/SOURCES.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/dependency_links.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/requires.txt
 src/gammarer.aws_secure_frontend_web_app_cloudfront_distribution.egg-info/top_level.txt
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/__init__.py
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/py.typed
 src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/__init__.py
-src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.1.3.jsii.tgz
+src/gammarer/aws_secure_frontend_web_app_cloudfront_distribution/_jsii/aws-secure-frontend-web-app-cloudfront-distribution@1.1.4.jsii.tgz
```

