# Comparing `tmp/climush-0.0.2.tar.gz` & `tmp/climush-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climush-0.0.2.tar", last modified: Sun Apr  7 02:38:13 2024, max compression
+gzip compressed data, was "climush-0.0.3.tar", last modified: Sun Apr  7 02:48:51 2024, max compression
```

## Comparing `climush-0.0.2.tar` & `climush-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 02:38:13.906727 climush-0.0.2/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     2112 2024-04-07 02:38:13.906476 climush-0.0.2/PKG-INFO
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.2/README.md
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 02:38:13.905188 climush-0.0.2/climush/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      142 2024-04-07 02:14:17.000000 climush-0.0.2/climush/__init__.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.2/climush/binfo_old.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    64710 2024-04-04 05:28:28.000000 climush-0.0.2/climush/bioinfo.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.2/climush/config.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     1125 2024-03-12 03:14:02.000000 climush-0.0.2/climush/constants.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)    43925 2024-03-21 06:50:22.000000 climush-0.0.2/climush/utilities.py
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.2/climush/viz.py
-drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 02:38:13.906228 climush-0.0.2/climush.egg-info/
--rw-r--r--   0 carolyndelevich   (501) staff       (20)     2112 2024-04-07 02:38:13.000000 climush-0.0.2/climush.egg-info/PKG-INFO
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      313 2024-04-07 02:38:13.000000 climush-0.0.2/climush.egg-info/SOURCES.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)        1 2024-04-07 02:38:13.000000 climush-0.0.2/climush.egg-info/dependency_links.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)       42 2024-04-07 02:38:13.000000 climush-0.0.2/climush.egg-info/requires.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)        8 2024-04-07 02:38:13.000000 climush-0.0.2/climush.egg-info/top_level.txt
--rw-r--r--   0 carolyndelevich   (501) staff       (20)      913 2024-04-07 02:35:42.000000 climush-0.0.2/pyproject.toml
--rw-r--r--   0 carolyndelevich   (501) staff       (20)       38 2024-04-07 02:38:13.906771 climush-0.0.2/setup.cfg
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 02:48:51.179782 climush-0.0.3/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     2112 2024-04-07 02:48:51.179480 climush-0.0.3/PKG-INFO
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     1234 2024-04-04 09:14:41.000000 climush-0.0.3/README.md
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 02:48:51.178079 climush-0.0.3/climush/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      152 2024-04-07 02:45:45.000000 climush-0.0.3/climush/__init__.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    24466 2024-02-03 09:44:16.000000 climush-0.0.3/climush/binfo_old.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    64710 2024-04-04 05:28:28.000000 climush-0.0.3/climush/bioinfo.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      380 2024-04-07 02:13:39.000000 climush-0.0.3/climush/config.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     1125 2024-03-12 03:14:02.000000 climush-0.0.3/climush/constants.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)    43925 2024-03-21 06:50:22.000000 climush-0.0.3/climush/utilities.py
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     5770 2024-02-23 04:02:34.000000 climush-0.0.3/climush/viz.py
+drwxr-xr-x   0 carolyndelevich   (501) staff       (20)        0 2024-04-07 02:48:51.179207 climush-0.0.3/climush.egg-info/
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)     2112 2024-04-07 02:48:51.000000 climush-0.0.3/climush.egg-info/PKG-INFO
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      313 2024-04-07 02:48:51.000000 climush-0.0.3/climush.egg-info/SOURCES.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)        1 2024-04-07 02:48:51.000000 climush-0.0.3/climush.egg-info/dependency_links.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)       42 2024-04-07 02:48:51.000000 climush-0.0.3/climush.egg-info/requires.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)        8 2024-04-07 02:48:51.000000 climush-0.0.3/climush.egg-info/top_level.txt
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)      914 2024-04-07 02:48:28.000000 climush-0.0.3/pyproject.toml
+-rw-r--r--   0 carolyndelevich   (501) staff       (20)       38 2024-04-07 02:48:51.179836 climush-0.0.3/setup.cfg
```

### Comparing `climush-0.0.2/PKG-INFO` & `climush-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `climush-0.0.2/README.md` & `climush-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `climush-0.0.2/climush/binfo_old.py` & `climush-0.0.3/climush/binfo_old.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.2/climush/bioinfo.py` & `climush-0.0.3/climush/bioinfo.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.2/climush/constants.py` & `climush-0.0.3/climush/constants.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.2/climush/utilities.py` & `climush-0.0.3/climush/utilities.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.2/climush/viz.py` & `climush-0.0.3/climush/viz.py`

 * *Files identical despite different names*

### Comparing `climush-0.0.2/climush.egg-info/PKG-INFO` & `climush-0.0.3/climush.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climush
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools to run the CliMush bioinformatics pipeline.
 Author-email: Carolyn Delevich <cdelevic@uoregon.edu>
 Project-URL: Homepage, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline
 Project-URL: Repository, https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package
 Project-URL: Issues, https://github.com/cdelevich/climush/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `climush-0.0.2/pyproject.toml` & `climush-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'climush'
-version = '0.0.2'
+version = '0.0.3'
 authors = [
     { name='Carolyn Delevich', email='cdelevic@uoregon.edu' }]
 description = 'Tools to run the CliMush bioinformatics pipeline.'
 readme = 'README.md'
 classifiers = [
     'Programming Language :: Python :: 3',
     'License :: OSI Approved :: MIT License',
@@ -19,14 +19,14 @@
 requires-python = ">=3.10"
 dependencies = [
     'pandas',
     'scipy',
     'numpy',
     'matplotlib',
     'seaborn',
-    'Bio'
+    'Bio',
 ]
 
 [project.urls]
 Homepage = 'https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline'
 Repository = 'https://github.com/cdelevich/climush/tree/main/bioinformatics-pipeline/climush_py-package'
 Issues = 'https://github.com/cdelevich/climush/issues'
```

