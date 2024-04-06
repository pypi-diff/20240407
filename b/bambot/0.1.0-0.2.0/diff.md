# Comparing `tmp/bambot-0.1.0.tar.gz` & `tmp/bambot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambot-0.1.0.tar", last modified: Sat Apr  6 20:37:03 2024, max compression
+gzip compressed data, was "bambot-0.2.0.tar", last modified: Sat Apr  6 23:07:18 2024, max compression
```

## Comparing `bambot-0.1.0.tar` & `bambot-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 20:37:03.922438 bambot-0.1.0/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1161 2024-04-06 20:37:03.922232 bambot-0.1.0/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      261 2024-04-06 20:04:16.000000 bambot-0.1.0/README.md
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 20:37:03.921351 bambot-0.1.0/bambot/
--rw-r--r--   0 spencerkinney   (501) staff       (20)       21 2024-04-06 20:30:19.000000 bambot-0.1.0/bambot/__init__.py
--rw-r--r--   0 spencerkinney   (501) staff       (20)      352 2024-04-06 20:30:24.000000 bambot-0.1.0/bambot/core.py
-drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 20:37:03.922046 bambot-0.1.0/bambot.egg-info/
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1161 2024-04-06 20:37:03.000000 bambot-0.1.0/bambot.egg-info/PKG-INFO
--rw-r--r--   0 spencerkinney   (501) staff       (20)      172 2024-04-06 20:37:03.000000 bambot-0.1.0/bambot.egg-info/SOURCES.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-06 20:37:03.000000 bambot-0.1.0/bambot.egg-info/dependency_links.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-06 20:37:03.000000 bambot-0.1.0/bambot.egg-info/top_level.txt
--rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-06 20:37:03.922473 bambot-0.1.0/setup.cfg
--rw-r--r--   0 spencerkinney   (501) staff       (20)     1126 2024-04-06 20:16:49.000000 bambot-0.1.0/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:07:18.462557 bambot-0.2.0/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1185 2024-04-06 23:07:18.462289 bambot-0.2.0/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      261 2024-04-06 20:04:16.000000 bambot-0.2.0/README.md
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:07:18.460659 bambot-0.2.0/bambot/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       21 2024-04-06 20:30:19.000000 bambot-0.2.0/bambot/__init__.py
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     2952 2024-04-06 22:52:43.000000 bambot-0.2.0/bambot/core.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:07:18.461990 bambot-0.2.0/bambot.egg-info/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1185 2024-04-06 23:07:18.000000 bambot-0.2.0/bambot.egg-info/PKG-INFO
+-rw-r--r--   0 spencerkinney   (501) staff       (20)      215 2024-04-06 23:07:18.000000 bambot-0.2.0/bambot.egg-info/SOURCES.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        1 2024-04-06 23:07:18.000000 bambot-0.2.0/bambot.egg-info/dependency_links.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        9 2024-04-06 23:07:18.000000 bambot-0.2.0/bambot.egg-info/requires.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)        7 2024-04-06 23:07:18.000000 bambot-0.2.0/bambot.egg-info/top_level.txt
+-rw-r--r--   0 spencerkinney   (501) staff       (20)       38 2024-04-06 23:07:18.462595 bambot-0.2.0/setup.cfg
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1130 2024-04-06 23:04:42.000000 bambot-0.2.0/setup.py
+drwxr-xr-x   0 spencerkinney   (501) staff       (20)        0 2024-04-06 23:07:18.461671 bambot-0.2.0/tests/
+-rw-r--r--   0 spencerkinney   (501) staff       (20)     1737 2024-04-06 22:55:58.000000 bambot-0.2.0/tests/test.py
```

### Comparing `bambot-0.1.0/PKG-INFO` & `bambot-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package for interfacing with Bam foundational AI models.
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp.
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
 # Bambot
 
 Bambot is a Python package for interfacing with Bam foundational AI models which simplifies the process of integrating advanced data capabilities into your apps.
 
 ## Installation
```

### Comparing `bambot-0.1.0/bambot.egg-info/PKG-INFO` & `bambot-0.2.0/bambot.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambot
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Python package for interfacing with Bam foundational AI models.
 Home-page: https://github.com/BamCorp/bambot
 Author: Bam Corp.
 Author-email: spencer@bam.bot
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6, <4
 Description-Content-Type: text/markdown
+Requires-Dist: requests
 
 # Bambot
 
 Bambot is a Python package for interfacing with Bam foundational AI models which simplifies the process of integrating advanced data capabilities into your apps.
 
 ## Installation
```

### Comparing `bambot-0.1.0/setup.py` & `bambot-0.2.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # setup.py
 from setuptools import setup, find_packages
 
 setup(
     name='bambot',
-    version='0.1.0',
+    version='0.2.0',
     author='Bam Corp.',
     author_email='spencer@bam.bot',
     description='A Python package for interfacing with Bam foundational AI models.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/BamCorp/bambot',
     packages=find_packages(),
     install_requires=[
-        # deps
+        "requests"
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
```

