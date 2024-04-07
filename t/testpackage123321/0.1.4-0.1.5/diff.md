# Comparing `tmp/testpackage123321-0.1.4.tar.gz` & `tmp/testpackage123321-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testpackage123321-0.1.4.tar", last modified: Sun Apr  7 08:28:21 2024, max compression
+gzip compressed data, was "testpackage123321-0.1.5.tar", last modified: Sun Apr  7 09:03:39 2024, max compression
```

## Comparing `testpackage123321-0.1.4.tar` & `testpackage123321-0.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 08:28:21.734149 testpackage123321-0.1.4/
--rw-rw-rw-   0        0        0     1091 2024-04-05 17:39:08.000000 testpackage123321-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     2879 2024-04-07 08:28:21.731150 testpackage123321-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2017 2024-04-05 17:39:08.000000 testpackage123321-0.1.4/README.md
--rw-rw-rw-   0        0        0       42 2024-04-07 08:28:21.735150 testpackage123321-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1282 2024-04-07 08:28:07.000000 testpackage123321-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:28:21.668599 testpackage123321-0.1.4/testpackage/
--rw-rw-rw-   0        0        0        0 2024-04-05 17:39:08.000000 testpackage123321-0.1.4/testpackage/__init__.py
--rw-rw-rw-   0        0        0      588 2024-04-07 08:16:44.000000 testpackage123321-0.1.4/testpackage/check_version.py
--rw-rw-rw-   0        0        0      814 2024-04-07 08:16:32.000000 testpackage123321-0.1.4/testpackage/document_extractor.py
--rw-rw-rw-   0        0        0     2030 2024-04-06 07:02:12.000000 testpackage123321-0.1.4/testpackage/evaluation_question_generator.py
--rw-rw-rw-   0        0        0     5089 2024-04-07 08:13:56.000000 testpackage123321-0.1.4/testpackage/hub.py
--rw-rw-rw-   0        0        0     2634 2024-04-07 08:12:34.000000 testpackage123321-0.1.4/testpackage/library_exceptions.py
--rw-rw-rw-   0        0        0     5040 2024-04-06 06:20:12.000000 testpackage123321-0.1.4/testpackage/text_chunker.py
--rw-rw-rw-   0        0        0     2081 2024-04-06 06:19:36.000000 testpackage123321-0.1.4/testpackage/text_cleaner.py
--rw-rw-rw-   0        0        0     2691 2024-04-06 05:40:03.000000 testpackage123321-0.1.4/testpackage/text_utils.py
--rw-rw-rw-   0        0        0     5184 2024-04-07 08:20:26.000000 testpackage123321-0.1.4/testpackage/tru_lens_evaluator.py
-drwxrwxrwx   0        0        0        0 2024-04-07 08:28:21.728151 testpackage123321-0.1.4/testpackage123321.egg-info/
--rw-rw-rw-   0        0        0     2879 2024-04-07 08:28:21.000000 testpackage123321-0.1.4/testpackage123321.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      575 2024-04-07 08:28:21.000000 testpackage123321-0.1.4/testpackage123321.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 08:28:21.000000 testpackage123321-0.1.4/testpackage123321.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-04-07 08:28:21.000000 testpackage123321-0.1.4/testpackage123321.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      135 2024-04-07 08:28:21.000000 testpackage123321-0.1.4/testpackage123321.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-07 08:28:21.000000 testpackage123321-0.1.4/testpackage123321.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 09:03:39.241223 testpackage123321-0.1.5/
+-rw-rw-rw-   0        0        0     1091 2024-04-05 17:39:08.000000 testpackage123321-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0     2879 2024-04-07 09:03:39.238121 testpackage123321-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2017 2024-04-05 17:39:08.000000 testpackage123321-0.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 09:03:39.242228 testpackage123321-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1292 2024-04-07 09:03:25.000000 testpackage123321-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:03:39.168999 testpackage123321-0.1.5/testpackage/
+-rw-rw-rw-   0        0        0        0 2024-04-05 17:39:08.000000 testpackage123321-0.1.5/testpackage/__init__.py
+-rw-rw-rw-   0        0        0      588 2024-04-07 08:16:44.000000 testpackage123321-0.1.5/testpackage/check_version.py
+-rw-rw-rw-   0        0        0      814 2024-04-07 08:16:32.000000 testpackage123321-0.1.5/testpackage/document_extractor.py
+-rw-rw-rw-   0        0        0     2030 2024-04-06 07:02:12.000000 testpackage123321-0.1.5/testpackage/evaluation_question_generator.py
+-rw-rw-rw-   0        0        0     5089 2024-04-07 08:13:56.000000 testpackage123321-0.1.5/testpackage/hub.py
+-rw-rw-rw-   0        0        0     2634 2024-04-07 08:12:34.000000 testpackage123321-0.1.5/testpackage/library_exceptions.py
+-rw-rw-rw-   0        0        0     5040 2024-04-06 06:20:12.000000 testpackage123321-0.1.5/testpackage/text_chunker.py
+-rw-rw-rw-   0        0        0     2081 2024-04-06 06:19:36.000000 testpackage123321-0.1.5/testpackage/text_cleaner.py
+-rw-rw-rw-   0        0        0     2691 2024-04-06 05:40:03.000000 testpackage123321-0.1.5/testpackage/text_utils.py
+-rw-rw-rw-   0        0        0     5184 2024-04-07 08:20:26.000000 testpackage123321-0.1.5/testpackage/tru_lens_evaluator.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:03:39.236078 testpackage123321-0.1.5/testpackage123321.egg-info/
+-rw-rw-rw-   0        0        0     2879 2024-04-07 09:03:38.000000 testpackage123321-0.1.5/testpackage123321.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      575 2024-04-07 09:03:38.000000 testpackage123321-0.1.5/testpackage123321.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 09:03:38.000000 testpackage123321-0.1.5/testpackage123321.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2024-04-07 09:03:38.000000 testpackage123321-0.1.5/testpackage123321.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      135 2024-04-07 09:03:38.000000 testpackage123321-0.1.5/testpackage123321.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-07 09:03:38.000000 testpackage123321-0.1.5/testpackage123321.egg-info/top_level.txt
```

### Comparing `testpackage123321-0.1.4/LICENSE` & `testpackage123321-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/PKG-INFO` & `testpackage123321-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpackage123321
-Version: 0.1.4
+Version: 0.1.5
 Summary: This library is to search the best parameters across different steps of the RAG process.
 Home-page: https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit
 Author: Ankit
 Author-email: a.baliyan008@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `testpackage123321-0.1.4/README.md` & `testpackage123321-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/setup.py` & `testpackage123321-0.1.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testpackage123321',
-    version='0.1.4', # all versions prior to launch will go into 0.0.1.--
+    version='0.1.5', # all versions prior to launch will go into 0.0.1.--
     packages=find_packages(),
     license='MIT',
     description='This library is to search the best parameters across different steps of the RAG process.',
     entry_points={
         'console_scripts': [
-            'check_version = test_RAG_X.check_version:main',  # Replace with your script path
+            'check_version = testpackage.check_version:check_version',  # Replace with your script path
         ]
     },
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Ankit',
     author_email='a.baliyan008@gmail.com',
     url='https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit',
```

### Comparing `testpackage123321-0.1.4/testpackage/check_version.py` & `testpackage123321-0.1.5/testpackage/check_version.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/document_extractor.py` & `testpackage123321-0.1.5/testpackage/document_extractor.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/evaluation_question_generator.py` & `testpackage123321-0.1.5/testpackage/evaluation_question_generator.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/hub.py` & `testpackage123321-0.1.5/testpackage/hub.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/library_exceptions.py` & `testpackage123321-0.1.5/testpackage/library_exceptions.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/text_chunker.py` & `testpackage123321-0.1.5/testpackage/text_chunker.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/text_cleaner.py` & `testpackage123321-0.1.5/testpackage/text_cleaner.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/text_utils.py` & `testpackage123321-0.1.5/testpackage/text_utils.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage/tru_lens_evaluator.py` & `testpackage123321-0.1.5/testpackage/tru_lens_evaluator.py`

 * *Files identical despite different names*

### Comparing `testpackage123321-0.1.4/testpackage123321.egg-info/PKG-INFO` & `testpackage123321-0.1.5/testpackage123321.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testpackage123321
-Version: 0.1.4
+Version: 0.1.5
 Summary: This library is to search the best parameters across different steps of the RAG process.
 Home-page: https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit
 Author: Ankit
 Author-email: a.baliyan008@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `testpackage123321-0.1.4/testpackage123321.egg-info/SOURCES.txt` & `testpackage123321-0.1.5/testpackage123321.egg-info/SOURCES.txt`

 * *Files identical despite different names*

