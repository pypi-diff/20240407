# Comparing `tmp/genflowly-lambda-utils-0.0.3.tar.gz` & `tmp/genflowly-lambda-utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genflowly-lambda-utils-0.0.3.tar", last modified: Sat Apr  6 01:07:40 2024, max compression
+gzip compressed data, was "genflowly-lambda-utils-0.0.4.tar", last modified: Sun Apr  7 14:46:39 2024, max compression
```

## Comparing `genflowly-lambda-utils-0.0.3.tar` & `genflowly-lambda-utils-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-06 01:07:40.000000 genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:40.654190 genflowly-lambda-utils-0.0.3/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_dynamodb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_s3_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_secrets_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_sns_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_sqs_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/aws_step_functions_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/contants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-06 01:07:14.000000 genflowly-lambda-utils-0.0.3/utils/jwt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 14:46:39.000000 genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:39.905788 genflowly-lambda-utils-0.0.4/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_dynamodb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_s3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_secrets_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_sns_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_sqs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/aws_step_functions_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/contants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/hashing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-04-07 14:46:13.000000 genflowly-lambda-utils-0.0.4/utils/jwt_utils.py
```

### Comparing `genflowly-lambda-utils-0.0.3/PKG-INFO` & `genflowly-lambda-utils-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly-lambda-utils-0.0.3/README.md` & `genflowly-lambda-utils-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/PKG-INFO` & `genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genflowly-lambda-utils
-Version: 0.0.3
+Version: 0.0.4
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: aiosignal
 Requires-Dist: async-timeout
 Requires-Dist: attrs
 Requires-Dist: bardapi
 Requires-Dist: boto3
```

### Comparing `genflowly-lambda-utils-0.0.3/genflowly_lambda_utils.egg-info/requires.txt` & `genflowly-lambda-utils-0.0.4/genflowly_lambda_utils.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.3/setup.py` & `genflowly-lambda-utils-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="genflowly-lambda-utils",
-    version="0.0.3",
+    version="0.0.4",
     packages=find_packages(),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     install_requires=[
         "aiohttp",
         "aiosignal",
         "async-timeout",
```

### Comparing `genflowly-lambda-utils-0.0.3/utils/aws_dynamodb_utils.py` & `genflowly-lambda-utils-0.0.4/utils/aws_dynamodb_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.3/utils/aws_secrets_utils.py` & `genflowly-lambda-utils-0.0.4/utils/aws_secrets_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.3/utils/aws_sns_utils.py` & `genflowly-lambda-utils-0.0.4/utils/aws_sns_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.3/utils/aws_step_functions_utils.py` & `genflowly-lambda-utils-0.0.4/utils/aws_step_functions_utils.py`

 * *Files identical despite different names*

### Comparing `genflowly-lambda-utils-0.0.3/utils/jwt_utils.py` & `genflowly-lambda-utils-0.0.4/utils/jwt_utils.py`

 * *Files identical despite different names*

