# Comparing `tmp/avro.py-2024.3.31.tar.gz` & `tmp/avro.py-2024.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avro.py-2024.3.31.tar", last modified: Sun Mar 31 16:11:26 2024, max compression
+gzip compressed data, was "avro.py-2024.4.7.tar", last modified: Sun Apr  7 06:59:50 2024, max compression
```

## Comparing `avro.py-2024.3.31.tar` & `avro.py-2024.4.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:11:26.464514 avro.py-2024.3.31/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-31 16:11:22.000000 avro.py-2024.3.31/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-31 16:11:22.000000 avro.py-2024.3.31/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-31 16:11:26.464514 avro.py-2024.3.31/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-03-31 16:11:22.000000 avro.py-2024.3.31/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:11:26.460514 avro.py-2024.3.31/avro/
--rwxr-xr-x   0 runner    (1001) docker     (127)      275 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/cli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      799 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    12937 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:11:26.460514 avro.py-2024.3.31/avro/resources/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/resources/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:11:26.460514 avro.py-2024.3.31/avro/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      576 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/utils/count.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2389 2024-03-31 16:11:22.000000 avro.py-2024.3.31/avro/utils/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:11:26.460514 avro.py-2024.3.31/avro.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-03-31 16:11:26.000000 avro.py-2024.3.31/avro.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-31 16:11:26.000000 avro.py-2024.3.31/avro.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 16:11:26.000000 avro.py-2024.3.31/avro.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-31 16:11:26.000000 avro.py-2024.3.31/avro.py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-31 16:11:26.000000 avro.py-2024.3.31/avro.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-31 16:11:26.000000 avro.py-2024.3.31/avro.py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-31 16:11:22.000000 avro.py-2024.3.31/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 16:11:26.464514 avro.py-2024.3.31/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1785 2024-03-31 16:11:22.000000 avro.py-2024.3.31/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 16:11:26.460514 avro.py-2024.3.31/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5589 2024-03-31 16:11:22.000000 avro.py-2024.3.31/tests/test_main.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1051 2024-03-31 16:11:22.000000 avro.py-2024.3.31/tests/test_utils_count.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3923 2024-03-31 16:11:22.000000 avro.py-2024.3.31/tests/test_utils_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-07 06:59:46.000000 avro.py-2024.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-07 06:59:46.000000 avro.py-2024.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-07 06:59:50.337261 avro.py-2024.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-07 06:59:46.000000 avro.py-2024.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      274 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      799 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12937 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39017 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/resources/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      576 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/count.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2389 2024-04-07 06:59:46.000000 avro.py-2024.4.7/avro/utils/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/avro.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 06:59:50.000000 avro.py-2024.4.7/avro.py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 06:59:46.000000 avro.py-2024.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:59:50.337261 avro.py-2024.4.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1804 2024-04-07 06:59:46.000000 avro.py-2024.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:59:50.337261 avro.py-2024.4.7/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5589 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_main.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1051 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_utils_count.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3923 2024-04-07 06:59:46.000000 avro.py-2024.4.7/tests/test_utils_validate.py
```

### Comparing `avro.py-2024.3.31/LICENSE` & `avro.py-2024.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/PKG-INFO` & `avro.py-2024.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2024.3.31
+Version: 2024.4.7
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,phonetics,avro,avro phonetic,bangla,bengali,bengali phonetics,transliteration
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cli
 Requires-Dist: click>=8.0.0; extra == "cli"
+Requires-Dist: pyclip>=0.7.0; extra == "cli"
 
 
 <!-- SPDX-License-Identifier: MIT -->
 
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
@@ -106,15 +107,15 @@
 ```python
 # Reversing back!
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 ```
 
 ---
 
-## 🔖 Command Line Usgae
+## 🔖 Command Line Usage
 
 Alternatively, instead of using avro.py from within your Python project, you can also use it as a simple,
 tiny command-line interface for easy parsing and reversing of text.
 
 ```sh
 # Installing the package.
 $ pip install avro.py[cli]
@@ -128,14 +129,19 @@
 
 # Parsing some text.
 $ avro parse "tumi onek bhalO!"
 $ avro parse --bijoy "amio kharap na, taina?"  # (bijoy keyboard format)
 
 # Reversing.
 $ avro reverse "তাই তো!"
+
+# Using additional flags to ease workflow.
+$ avro parse --from-clip  # (fetching input from clipboard)
+$ avro parse "asolei!" --copy  # (copying output to clipboard)
+$ avro parse --from-clip --copy  # (clipboard input -> output)
 ```
 
 <br>
 
 ## 🛠️ Contributing
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
```

### Comparing `avro.py-2024.3.31/README.md` & `avro.py-2024.4.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ```python
 # Reversing back!
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 ```
 
 ---
 
-## 🔖 Command Line Usgae
+## 🔖 Command Line Usage
 
 Alternatively, instead of using avro.py from within your Python project, you can also use it as a simple,
 tiny command-line interface for easy parsing and reversing of text.
 
 ```sh
 # Installing the package.
 $ pip install avro.py[cli]
@@ -103,14 +103,19 @@
 
 # Parsing some text.
 $ avro parse "tumi onek bhalO!"
 $ avro parse --bijoy "amio kharap na, taina?"  # (bijoy keyboard format)
 
 # Reversing.
 $ avro reverse "তাই তো!"
+
+# Using additional flags to ease workflow.
+$ avro parse --from-clip  # (fetching input from clipboard)
+$ avro parse "asolei!" --copy  # (copying output to clipboard)
+$ avro parse --from-clip --copy  # (clipboard input -> output)
 ```
 
 <br>
 
 ## 🛠️ Contributing
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
```

### Comparing `avro.py-2024.3.31/avro/config.py` & `avro.py-2024.4.7/avro/config.py`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/avro/main.py` & `avro.py-2024.4.7/avro/main.py`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/avro/resources/dictionary.py` & `avro.py-2024.4.7/avro/resources/dictionary.py`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/avro/utils/count.py` & `avro.py-2024.4.7/avro/utils/count.py`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/avro/utils/validate.py` & `avro.py-2024.4.7/avro/utils/validate.py`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/avro.py.egg-info/PKG-INFO` & `avro.py-2024.4.7/avro.py.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avro.py
-Version: 2024.3.31
+Version: 2024.4.7
 Summary: A modern Pythonic implementation of Avro Phonetic.
 Home-page: https://github.com/hitblast/avro.py
 Author: HitBlast
 Author-email: hitblastlive@gmail.com
 License: MIT
 Keywords: python,phonetics,avro,avro phonetic,bangla,bengali,bengali phonetics,transliteration
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: cli
 Requires-Dist: click>=8.0.0; extra == "cli"
+Requires-Dist: pyclip>=0.7.0; extra == "cli"
 
 
 <!-- SPDX-License-Identifier: MIT -->
 
 <div align="center">
 
 # <img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" height="40px"/> avro.py
@@ -106,15 +107,15 @@
 ```python
 # Reversing back!
 reversed_text = avro.reverse('আমার সোনার বাংলা।')
 ```
 
 ---
 
-## 🔖 Command Line Usgae
+## 🔖 Command Line Usage
 
 Alternatively, instead of using avro.py from within your Python project, you can also use it as a simple,
 tiny command-line interface for easy parsing and reversing of text.
 
 ```sh
 # Installing the package.
 $ pip install avro.py[cli]
@@ -128,14 +129,19 @@
 
 # Parsing some text.
 $ avro parse "tumi onek bhalO!"
 $ avro parse --bijoy "amio kharap na, taina?"  # (bijoy keyboard format)
 
 # Reversing.
 $ avro reverse "তাই তো!"
+
+# Using additional flags to ease workflow.
+$ avro parse --from-clip  # (fetching input from clipboard)
+$ avro parse "asolei!" --copy  # (copying output to clipboard)
+$ avro parse --from-clip --copy  # (clipboard input -> output)
 ```
 
 <br>
 
 ## 🛠️ Contributing
 
 :octocat: *Fork -> Do your changes -> Send a Pull Request, it's that easy!* <br>
```

### Comparing `avro.py-2024.3.31/setup.py` & `avro.py-2024.4.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
     extras_require={
-        'cli': ['click>=8.0.0'],
+        'cli': ['click>=8.0.0', 'pyclip >= 0.7.0'],
     },
     entry_points={
         'console_scripts': [
             'avro=avro.cli:main',
         ],
     },
 )
```

### Comparing `avro.py-2024.3.31/tests/test_main.py` & `avro.py-2024.4.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/tests/test_utils_count.py` & `avro.py-2024.4.7/tests/test_utils_count.py`

 * *Files identical despite different names*

### Comparing `avro.py-2024.3.31/tests/test_utils_validate.py` & `avro.py-2024.4.7/tests/test_utils_validate.py`

 * *Files identical despite different names*

