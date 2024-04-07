# Comparing `tmp/vigor-0.1.1.tar.gz` & `tmp/vigor-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vigor-0.1.1.tar", last modified: Wed May 11 06:22:40 2022, max compression
+gzip compressed data, was "vigor-0.1.2.tar", last modified: Sun Apr  7 21:56:10 2024, max compression
```

## Comparing `vigor-0.1.1.tar` & `vigor-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 ryanl      (502) staff       (20)        0 2022-05-11 06:22:40.747689 vigor-0.1.1/
--rw-r--r--   0 ryanl      (502) staff       (20)     1074 2022-03-29 07:15:10.000000 vigor-0.1.1/LICENSE
--rw-r--r--   0 ryanl      (502) staff       (20)     1114 2022-05-11 06:22:40.747575 vigor-0.1.1/PKG-INFO
--rw-r--r--   0 ryanl      (502) staff       (20)      400 2022-03-29 07:40:27.000000 vigor-0.1.1/README.md
--rw-r--r--   0 ryanl      (502) staff       (20)       38 2022-05-11 06:22:40.747727 vigor-0.1.1/setup.cfg
--rw-r--r--   0 ryanl      (502) staff       (20)     1150 2022-05-11 06:21:57.000000 vigor-0.1.1/setup.py
-drwxr-xr-x   0 ryanl      (502) staff       (20)        0 2022-05-11 06:22:40.747034 vigor-0.1.1/vigor/
--rw-r--r--   0 ryanl      (502) staff       (20)      228 2022-05-11 06:22:08.000000 vigor-0.1.1/vigor/__init__.py
--rw-r--r--   0 ryanl      (502) staff       (20)       71 2022-03-29 07:48:03.000000 vigor-0.1.1/vigor/__main__.py
--rw-r--r--   0 ryanl      (502) staff       (20)     2421 2022-05-11 06:17:07.000000 vigor-0.1.1/vigor/utils.py
-drwxr-xr-x   0 ryanl      (502) staff       (20)        0 2022-05-11 06:22:40.747430 vigor-0.1.1/vigor.egg-info/
--rw-r--r--   0 ryanl      (502) staff       (20)     1114 2022-05-11 06:22:40.000000 vigor-0.1.1/vigor.egg-info/PKG-INFO
--rw-r--r--   0 ryanl      (502) staff       (20)      193 2022-05-11 06:22:40.000000 vigor-0.1.1/vigor.egg-info/SOURCES.txt
--rw-r--r--   0 ryanl      (502) staff       (20)        1 2022-05-11 06:22:40.000000 vigor-0.1.1/vigor.egg-info/dependency_links.txt
--rw-r--r--   0 ryanl      (502) staff       (20)        6 2022-05-11 06:22:40.000000 vigor-0.1.1/vigor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:56:10.234719 vigor-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 21:56:00.000000 vigor-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-07 21:56:10.234719 vigor-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-07 21:56:00.000000 vigor-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:56:10.234719 vigor-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-07 21:56:00.000000 vigor-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:56:10.230719 vigor-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-07 21:56:00.000000 vigor-0.1.2/tests/test_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:56:10.234719 vigor-0.1.2/vigor/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-07 21:56:00.000000 vigor-0.1.2/vigor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 21:56:00.000000 vigor-0.1.2/vigor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 21:56:00.000000 vigor-0.1.2/vigor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:56:10.234719 vigor-0.1.2/vigor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-04-07 21:56:10.000000 vigor-0.1.2/vigor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-07 21:56:10.000000 vigor-0.1.2/vigor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:56:10.000000 vigor-0.1.2/vigor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 21:56:10.000000 vigor-0.1.2/vigor.egg-info/top_level.txt
```

### Comparing `vigor-0.1.1/LICENSE` & `vigor-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vigor-0.1.1/PKG-INFO` & `vigor-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: vigor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of semi-random, semi-useful Python scripts and CLI tools.
 Home-page: https://github.com/RyanLiu6/vigor
 Author: Ryan Liu
 Author-email: ryan@ryanliu6.xyz
 License: MIT
-Description: # vigor
-        
-        <!-- [![pypi](https://img.shields.io/pypi/v/vigor.svg)](https://pypi.python.org/pypi/vigor)
-        [![versions](https://img.shields.io/pypi/pyversions/vigor.svg)](https://github.com/ryanliu6/vigor) -->
-        [![license](https://img.shields.io/github/license/ryanliu6/vigor.svg)](https://github.com/ryanliu6/vigor/blob/main/LICENSE)
-        
-        A collection of semi-random, semi-useful Python scripts and CLI tools.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+# vigor
+
+<!-- [![pypi](https://img.shields.io/pypi/v/vigor.svg)](https://pypi.python.org/pypi/vigor)
+[![versions](https://img.shields.io/pypi/pyversions/vigor.svg)](https://github.com/ryanliu6/vigor) -->
+[![license](https://img.shields.io/github/license/ryanliu6/vigor.svg)](https://github.com/ryanliu6/vigor/blob/main/LICENSE)
+
+A collection of semi-random, semi-useful Python scripts and CLI tools.
```

### Comparing `vigor-0.1.1/setup.py` & `vigor-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     text_type = type(u"")
     with io.open(filename, mode="r", encoding='utf-8') as fd:
         return re.sub(text_type(r':[a-z]+:`~?(.*?)`'), text_type(r'``\1``'), fd.read())
 
 
 setup(
     name="vigor",
-    version="0.1.1",
+    version="0.1.2",
     url="https://github.com/RyanLiu6/vigor",
     license='MIT',
 
     author="Ryan Liu",
     author_email="ryan@ryanliu6.xyz",
 
     description="A collection of semi-random, semi-useful Python scripts and CLI tools.",
```

### Comparing `vigor-0.1.1/vigor.egg-info/PKG-INFO` & `vigor-0.1.2/vigor.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: vigor
-Version: 0.1.1
+Version: 0.1.2
 Summary: A collection of semi-random, semi-useful Python scripts and CLI tools.
 Home-page: https://github.com/RyanLiu6/vigor
 Author: Ryan Liu
 Author-email: ryan@ryanliu6.xyz
 License: MIT
-Description: # vigor
-        
-        <!-- [![pypi](https://img.shields.io/pypi/v/vigor.svg)](https://pypi.python.org/pypi/vigor)
-        [![versions](https://img.shields.io/pypi/pyversions/vigor.svg)](https://github.com/ryanliu6/vigor) -->
-        [![license](https://img.shields.io/github/license/ryanliu6/vigor.svg)](https://github.com/ryanliu6/vigor/blob/main/LICENSE)
-        
-        A collection of semi-random, semi-useful Python scripts and CLI tools.
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+License-File: LICENSE
+
+# vigor
+
+<!-- [![pypi](https://img.shields.io/pypi/v/vigor.svg)](https://pypi.python.org/pypi/vigor)
+[![versions](https://img.shields.io/pypi/pyversions/vigor.svg)](https://github.com/ryanliu6/vigor) -->
+[![license](https://img.shields.io/github/license/ryanliu6/vigor.svg)](https://github.com/ryanliu6/vigor/blob/main/LICENSE)
+
+A collection of semi-random, semi-useful Python scripts and CLI tools.
```

