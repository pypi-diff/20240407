# Comparing `tmp/pytector-0.0.5.tar.gz` & `tmp/pytector-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytector-0.0.5.tar", last modified: Sun Apr  7 03:06:19 2024, max compression
+gzip compressed data, was "pytector-0.0.6.tar", last modified: Sun Apr  7 03:37:23 2024, max compression
```

## Comparing `pytector-0.0.5.tar` & `pytector-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:06:19.281909 pytector-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 03:06:13.000000 pytector-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 03:06:13.000000 pytector-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-07 03:06:19.281909 pytector-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-07 03:06:13.000000 pytector-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:06:19.277909 pytector-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-07 03:06:13.000000 pytector-0.0.5/docs/PromptInjectionDetector.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:06:19.281909 pytector-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-07 03:06:13.000000 pytector-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:06:19.277909 pytector-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:06:19.277909 pytector-0.0.5/src/pytector/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 03:06:13.000000 pytector-0.0.5/src/pytector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-07 03:06:13.000000 pytector-0.0.5/src/pytector/detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:06:19.281909 pytector-0.0.5/src/pytector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-07 03:06:19.000000 pytector-0.0.5/src/pytector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 03:06:19.000000 pytector-0.0.5/src/pytector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:06:19.000000 pytector-0.0.5/src/pytector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 03:06:19.000000 pytector-0.0.5/src/pytector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 03:06:19.000000 pytector-0.0.5/src/pytector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:06:19.281909 pytector-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-04-07 03:06:13.000000 pytector-0.0.5/tests/test_pytector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.877598 pytector-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-07 03:35:15.000000 pytector-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-07 03:35:15.000000 pytector-0.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-07 03:37:23.877598 pytector-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-07 03:35:15.000000 pytector-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.873598 pytector-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-07 03:35:15.000000 pytector-0.0.6/docs/PromptInjectionDetector.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:37:23.877598 pytector-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-07 03:35:15.000000 pytector-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.873598 pytector-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.873598 pytector-0.0.6/src/pytector/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 03:35:15.000000 pytector-0.0.6/src/pytector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-07 03:35:15.000000 pytector-0.0.6/src/pytector/detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.877598 pytector-0.0.6/src/pytector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 03:37:23.000000 pytector-0.0.6/src/pytector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:37:23.877598 pytector-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-07 03:35:15.000000 pytector-0.0.6/tests/test_pytector.py
```

### Comparing `pytector-0.0.5/LICENSE` & `pytector-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytector-0.0.5/PKG-INFO` & `pytector-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytector
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for detecting prompt injections in text using Open-Source LLMs.
 Home-page: https://github.com/MaxMLang/pytector
 Author: Max Melchior Lang
 Author-email: langmaxmelchior@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,23 +27,29 @@
 ## Features
 
 - Detect prompt injections with pre-trained models.
 - Support for multiple models including DeBERTa, DistilBERT, and ONNX versions.
 - Easy-to-use interface with customizable threshold settings.
 
 ## Installation
+Via PIP
+```bash
+pip install pytector
+```
 
 Install Pytector directly from the source code:
 
 ```bash
 git clone https://github.com/MaxMLang/pytector.git
 cd pytector
 pip install .
 ```
 
+
+
 ## Usage
 
 To use Pytector, you can import the `PromptInjectionDetector` class and create an instance with a pre-defined model or a custom model URL.
 
 ```python
 import pytector
```

### Comparing `pytector-0.0.5/README.md` & `pytector-0.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,23 +10,29 @@
 ## Features
 
 - Detect prompt injections with pre-trained models.
 - Support for multiple models including DeBERTa, DistilBERT, and ONNX versions.
 - Easy-to-use interface with customizable threshold settings.
 
 ## Installation
+Via PIP
+```bash
+pip install pytector
+```
 
 Install Pytector directly from the source code:
 
 ```bash
 git clone https://github.com/MaxMLang/pytector.git
 cd pytector
 pip install .
 ```
 
+
+
 ## Usage
 
 To use Pytector, you can import the `PromptInjectionDetector` class and create an instance with a pre-defined model or a custom model URL.
 
 ```python
 import pytector
```

### Comparing `pytector-0.0.5/docs/PromptInjectionDetector.md` & `pytector-0.0.6/docs/PromptInjectionDetector.md`

 * *Files identical despite different names*

### Comparing `pytector-0.0.5/setup.py` & `pytector-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='pytector',
-    version='0.0.5',
+    version='0.0.6',
     author='Max Melchior Lang',
     author_email='langmaxmelchior@gmail.com',
     description='A package for detecting prompt injections in text using Open-Source LLMs.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/MaxMLang/pytector',
     package_dir={'': 'src'},
```

### Comparing `pytector-0.0.5/src/pytector/detector.py` & `pytector-0.0.6/src/pytector/detector.py`

 * *Files identical despite different names*

### Comparing `pytector-0.0.5/src/pytector.egg-info/PKG-INFO` & `pytector-0.0.6/src/pytector.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytector
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package for detecting prompt injections in text using Open-Source LLMs.
 Home-page: https://github.com/MaxMLang/pytector
 Author: Max Melchior Lang
 Author-email: langmaxmelchior@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -27,23 +27,29 @@
 ## Features
 
 - Detect prompt injections with pre-trained models.
 - Support for multiple models including DeBERTa, DistilBERT, and ONNX versions.
 - Easy-to-use interface with customizable threshold settings.
 
 ## Installation
+Via PIP
+```bash
+pip install pytector
+```
 
 Install Pytector directly from the source code:
 
 ```bash
 git clone https://github.com/MaxMLang/pytector.git
 cd pytector
 pip install .
 ```
 
+
+
 ## Usage
 
 To use Pytector, you can import the `PromptInjectionDetector` class and create an instance with a pre-defined model or a custom model URL.
 
 ```python
 import pytector
```

### Comparing `pytector-0.0.5/tests/test_pytector.py` & `pytector-0.0.6/tests/test_pytector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
+import validators
+import transformers
 from src import pytector
 
-
 class TestPromptInjectionDetector(unittest.TestCase):
 
     def test_initialization_with_predefined_model(self):
         """Test initialization with a predefined model."""
         detector = pytector.PromptInjectionDetector(model_name_or_url="deberta")
         self.assertIsInstance(detector, pytector.PromptInjectionDetector)
```

