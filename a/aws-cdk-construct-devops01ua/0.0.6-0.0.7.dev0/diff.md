# Comparing `tmp/aws_cdk_construct_devops01ua-0.0.6.tar.gz` & `tmp/aws_cdk_construct_devops01ua-0.0.7.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_cdk_construct_devops01ua-0.0.6.tar", last modified: Sat Apr  6 20:27:57 2024, max compression
+gzip compressed data, was "aws_cdk_construct_devops01ua-0.0.7.dev0.tar", last modified: Sun Apr  7 17:07:57 2024, max compression
```

## Comparing `aws_cdk_construct_devops01ua-0.0.6.tar` & `aws_cdk_construct_devops01ua-0.0.7.dev0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-06 20:27:57.157731 aws_cdk_construct_devops01ua-0.0.6/
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)     1579 2024-04-06 20:27:57.156907 aws_cdk_construct_devops01ua-0.0.6/PKG-INFO
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)      898 2024-04-02 15:34:46.000000 aws_cdk_construct_devops01ua-0.0.6/README.md
-drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-06 20:27:57.134742 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua/
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)        0 2024-04-06 19:51:22.000000 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua/__init__.py
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)     2185 2024-04-06 19:51:22.000000 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua/constructs.py
-drwxr-xr-x   0 ahrechanychenko   (501) staff       (20)        0 2024-04-06 20:27:57.155342 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua.egg-info/
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)     1579 2024-04-06 20:27:56.000000 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua.egg-info/PKG-INFO
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)      361 2024-04-06 20:27:56.000000 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua.egg-info/SOURCES.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)        1 2024-04-06 20:27:56.000000 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua.egg-info/dependency_links.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)       38 2024-04-06 20:27:56.000000 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua.egg-info/requires.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)       29 2024-04-06 20:27:56.000000 aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua.egg-info/top_level.txt
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)       38 2024-04-06 20:27:57.157804 aws_cdk_construct_devops01ua-0.0.6/setup.cfg
--rw-r--r--   0 ahrechanychenko   (501) staff       (20)      953 2024-04-06 20:27:11.000000 aws_cdk_construct_devops01ua-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:07:57.931609 aws_cdk_construct_devops01ua-0.0.7.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-07 17:07:57.931609 aws_cdk_construct_devops01ua-0.0.7.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-07 17:07:50.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:07:57.927609 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 17:07:50.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-07 17:07:50.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua/constructs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 17:07:57.927609 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-07 17:07:57.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-07 17:07:57.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 17:07:57.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 17:07:57.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 17:07:57.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 17:07:57.931609 aws_cdk_construct_devops01ua-0.0.7.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-07 17:07:50.000000 aws_cdk_construct_devops01ua-0.0.7.dev0/setup.py
```

### Comparing `aws_cdk_construct_devops01ua-0.0.6/PKG-INFO` & `aws_cdk_construct_devops01ua-0.0.7.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_cdk_construct_devops01ua
-Version: 0.0.6
+Version: 0.0.7.dev0
 Summary: Sample of custom AWS CDK construct for demo purposes
 Author: Artem Hrechanychenko
 Author-email: devops01ua@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aws_cdk_construct_devops01ua-0.0.6/README.md` & `aws_cdk_construct_devops01ua-0.0.7.dev0/README.md`

 * *Files identical despite different names*

### Comparing `aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua/constructs.py` & `aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua/constructs.py`

 * *Files identical despite different names*

### Comparing `aws_cdk_construct_devops01ua-0.0.6/aws_cdk_construct_devops01ua.egg-info/PKG-INFO` & `aws_cdk_construct_devops01ua-0.0.7.dev0/aws_cdk_construct_devops01ua.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_cdk_construct_devops01ua
-Version: 0.0.6
+Version: 0.0.7.dev0
 Summary: Sample of custom AWS CDK construct for demo purposes
 Author: Artem Hrechanychenko
 Author-email: devops01ua@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `aws_cdk_construct_devops01ua-0.0.6/setup.py` & `aws_cdk_construct_devops01ua-0.0.7.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aws_cdk_construct_devops01ua',  # Replace with your package name
-    version='0.0.6',  # Replace with your package version
+    version='0.0.7-dev',  # Replace with your package version
     author='Artem Hrechanychenko',
     author_email='devops01ua@gmail.com',
     description='Sample of custom AWS CDK construct for demo purposes',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```

