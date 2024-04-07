# Comparing `tmp/pytector-0.0.6.tar.gz` & `tmp/pytector-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytector-0.0.6.tar", last modified: Sun Apr  7 03:37:23 2024, max compression
+gzip compressed data, was "pytector-0.0.7.tar", last modified: Sun Apr  7 03:48:48 2024, max compression
```

## Comparing `pytector-0.0.6.tar` & `pytector-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.877598 pytector-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 03:35:15.000000 pytector-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 03:35:15.000000 pytector-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-07 03:37:23.877598 pytector-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-07 03:35:15.000000 pytector-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.873598 pytector-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-07 03:35:15.000000 pytector-0.0.6/docs/PromptInjectionDetector.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:37:23.877598 pytector-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-07 03:35:15.000000 pytector-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.873598 pytector-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.873598 pytector-0.0.6/src/pytector/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 03:35:15.000000 pytector-0.0.6/src/pytector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-07 03:35:15.000000 pytector-0.0.6/src/pytector/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.877598 pytector-0.0.6/src/pytector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.877598 pytector-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-07 03:35:15.000000 pytector-0.0.6/tests/test_pytector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:48:48.114430 pytector-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 03:46:26.000000 pytector-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 03:46:26.000000 pytector-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-07 03:48:48.110430 pytector-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-07 03:46:26.000000 pytector-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:48:48.110430 pytector-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-07 03:46:26.000000 pytector-0.0.7/docs/PromptInjectionDetector.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:48:48.114430 pytector-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-07 03:46:26.000000 pytector-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:48:48.106430 pytector-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:48:48.110430 pytector-0.0.7/src/pytector/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 03:46:26.000000 pytector-0.0.7/src/pytector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-07 03:46:26.000000 pytector-0.0.7/src/pytector/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:48:48.110430 pytector-0.0.7/src/pytector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2957 2024-04-07 03:48:48.000000 pytector-0.0.7/src/pytector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 03:48:48.000000 pytector-0.0.7/src/pytector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:48:48.000000 pytector-0.0.7/src/pytector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 03:48:48.000000 pytector-0.0.7/src/pytector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 03:48:48.000000 pytector-0.0.7/src/pytector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:48:48.110430 pytector-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-07 03:46:26.000000 pytector-0.0.7/tests/test_pytector.py
```

### Comparing `pytector-0.0.6/LICENSE` & `pytector-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pytector-0.0.6/PKG-INFO` & `pytector-0.0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytector
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for detecting prompt injections in text using Open-Source LLMs.
 Home-page: https://github.com/MaxMLang/pytector
 Author: Max Melchior Lang
 Author-email: langmaxmelchior@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,19 @@
 License-File: LICENSE
 Requires-Dist: transformers>=4.0.0
 Requires-Dist: validators
 Requires-Dist: torch
 
 # Pytector
 
+![Workflow Status](https://img.shields.io/github/workflow/status/MaxMLang/pytector/CI)
+![Python Version](https://img.shields.io/badge/python-3.9+-blue.svg)
+![License](https://img.shields.io/github/license/MaxMLang/pytector)
+![Issues](https://img.shields.io/github/issues/MaxMLang/pytector)
+![Pull Requests](https://img.shields.io/github/issues-pr/MaxMLang/pytector)
 Pytector is a Python package designed to detect prompt injection in text inputs using state-of-the-art machine learning models from the transformers library.
 
 ## Disclaimer
 
 The Pytector package is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.
 Pytector is still a prototype and cannot provide 100% protection against prompt injection attacks!
```

### Comparing `pytector-0.0.6/docs/PromptInjectionDetector.md` & `pytector-0.0.7/docs/PromptInjectionDetector.md`

 * *Files identical despite different names*

### Comparing `pytector-0.0.6/setup.py` & `pytector-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytector',
-    version='0.0.6',
+    version='0.0.7',
     author='Max Melchior Lang',
     author_email='langmaxmelchior@gmail.com',
     description='A package for detecting prompt injections in text using Open-Source LLMs.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/MaxMLang/pytector',
     package_dir={'': 'src'},
```

### Comparing `pytector-0.0.6/src/pytector/detector.py` & `pytector-0.0.7/src/pytector/detector.py`

 * *Files identical despite different names*

### Comparing `pytector-0.0.6/src/pytector.egg-info/PKG-INFO` & `pytector-0.0.7/src/pytector.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytector
-Version: 0.0.6
+Version: 0.0.7
 Summary: A package for detecting prompt injections in text using Open-Source LLMs.
 Home-page: https://github.com/MaxMLang/pytector
 Author: Max Melchior Lang
 Author-email: langmaxmelchior@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,14 +13,19 @@
 License-File: LICENSE
 Requires-Dist: transformers>=4.0.0
 Requires-Dist: validators
 Requires-Dist: torch
 
 # Pytector
 
+![Workflow Status](https://img.shields.io/github/workflow/status/MaxMLang/pytector/CI)
+![Python Version](https://img.shields.io/badge/python-3.9+-blue.svg)
+![License](https://img.shields.io/github/license/MaxMLang/pytector)
+![Issues](https://img.shields.io/github/issues/MaxMLang/pytector)
+![Pull Requests](https://img.shields.io/github/issues-pr/MaxMLang/pytector)
 Pytector is a Python package designed to detect prompt injection in text inputs using state-of-the-art machine learning models from the transformers library.
 
 ## Disclaimer
 
 The Pytector package is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages, or other liability, whether in an action of contract, tort or otherwise, arising from, out of, or in connection with the software or the use or other dealings in the software.
 Pytector is still a prototype and cannot provide 100% protection against prompt injection attacks!
```

### Comparing `pytector-0.0.6/tests/test_pytector.py` & `pytector-0.0.7/tests/test_pytector.py`

 * *Files identical despite different names*

