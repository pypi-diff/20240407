# Comparing `tmp/CINOSUM-1.0.4.tar.gz` & `tmp/CINOSUM-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CINOSUM-1.0.4.tar", last modified: Sat Apr  6 10:50:48 2024, max compression
+gzip compressed data, was "CINOSUM-1.0.5.tar", last modified: Sun Apr  7 06:29:23 2024, max compression
```

## Comparing `CINOSUM-1.0.4.tar` & `CINOSUM-1.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 10:50:48.815473 CINOSUM-1.0.4/
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 10:50:48.815473 CINOSUM-1.0.4/CINOSUM.egg-info/
--rw-r--r--   0 lhy       (1003) lhy       (1003)      441 2024-04-06 10:50:48.000000 CINOSUM-1.0.4/CINOSUM.egg-info/PKG-INFO
--rw-rw-r--   0 lhy       (1003) lhy       (1003)      312 2024-04-06 10:50:48.000000 CINOSUM-1.0.4/CINOSUM.egg-info/SOURCES.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        1 2024-04-06 10:50:48.000000 CINOSUM-1.0.4/CINOSUM.egg-info/dependency_links.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-06 10:50:48.000000 CINOSUM-1.0.4/CINOSUM.egg-info/requires.txt
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        7 2024-04-06 10:50:48.000000 CINOSUM-1.0.4/CINOSUM.egg-info/top_level.txt
--rw-r--r--   0 lhy       (1003) lhy       (1003)      441 2024-04-06 10:50:48.815473 CINOSUM-1.0.4/PKG-INFO
-drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-06 10:50:48.815473 CINOSUM-1.0.4/models/
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     4507 2024-04-06 03:29:14.000000 CINOSUM-1.0.4/models/CINOSUM.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:12:32.000000 CINOSUM-1.0.4/models/__init__.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     4814 2024-04-06 03:16:15.000000 CINOSUM-1.0.4/models/encoder.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)    12903 2024-04-06 03:05:07.000000 CINOSUM-1.0.4/models/generate.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     3951 2024-04-06 03:16:07.000000 CINOSUM-1.0.4/models/model_builder.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     8340 2024-03-26 02:05:37.000000 CINOSUM-1.0.4/models/neural.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     9649 2024-04-06 03:05:18.000000 CINOSUM-1.0.4/models/optimizers.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)     3886 2024-04-01 13:19:09.000000 CINOSUM-1.0.4/models/rnn.py
--rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-06 10:50:48.815473 CINOSUM-1.0.4/setup.cfg
--rw-rw-r--   0 lhy       (1003) lhy       (1003)      588 2024-04-06 10:50:04.000000 CINOSUM-1.0.4/setup.py
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-07 06:29:23.640673 CINOSUM-1.0.5/
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-07 06:29:23.548673 CINOSUM-1.0.5/CINOSUM.egg-info/
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      343 2024-04-07 06:29:23.000000 CINOSUM-1.0.5/CINOSUM.egg-info/PKG-INFO
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      312 2024-04-07 06:29:23.000000 CINOSUM-1.0.5/CINOSUM.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        1 2024-04-07 06:29:23.000000 CINOSUM-1.0.5/CINOSUM.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-07 06:29:23.000000 CINOSUM-1.0.5/CINOSUM.egg-info/requires.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        7 2024-04-07 06:29:23.000000 CINOSUM-1.0.5/CINOSUM.egg-info/top_level.txt
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      343 2024-04-07 06:29:23.640673 CINOSUM-1.0.5/PKG-INFO
+drwxrwxr-x   0 lhy       (1003) lhy       (1003)        0 2024-04-07 06:29:23.624673 CINOSUM-1.0.5/models/
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     4507 2024-04-06 03:29:14.000000 CINOSUM-1.0.5/models/CINOSUM.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)        0 2024-04-06 03:12:32.000000 CINOSUM-1.0.5/models/__init__.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     4814 2024-04-06 03:16:15.000000 CINOSUM-1.0.5/models/encoder.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)    12903 2024-04-06 03:05:07.000000 CINOSUM-1.0.5/models/generate.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     3951 2024-04-06 03:16:07.000000 CINOSUM-1.0.5/models/model_builder.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     8340 2024-03-26 02:05:37.000000 CINOSUM-1.0.5/models/neural.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     9649 2024-04-06 03:05:18.000000 CINOSUM-1.0.5/models/optimizers.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)     3886 2024-04-01 13:19:09.000000 CINOSUM-1.0.5/models/rnn.py
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)       38 2024-04-07 06:29:23.640673 CINOSUM-1.0.5/setup.cfg
+-rw-rw-r--   0 lhy       (1003) lhy       (1003)      588 2024-04-07 06:27:25.000000 CINOSUM-1.0.5/setup.py
```

### Comparing `CINOSUM-1.0.4/models/CINOSUM.py` & `CINOSUM-1.0.5/models/CINOSUM.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.4/models/encoder.py` & `CINOSUM-1.0.5/models/encoder.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.4/models/generate.py` & `CINOSUM-1.0.5/models/generate.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.4/models/model_builder.py` & `CINOSUM-1.0.5/models/model_builder.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.4/models/neural.py` & `CINOSUM-1.0.5/models/neural.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.4/models/optimizers.py` & `CINOSUM-1.0.5/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.4/models/rnn.py` & `CINOSUM-1.0.5/models/rnn.py`

 * *Files identical despite different names*

### Comparing `CINOSUM-1.0.4/setup.py` & `CINOSUM-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='CINOSUM',
-    version='1.0.4',
+    version='1.0.5',
     description='Chinese Minority Extractive Multi-language summarization project',
     author='HaoYu Luo',
     author_email='506685820@qq.com',
     packages=find_packages(),
     install_requires=[
         'torch',
         'numpy',
```

