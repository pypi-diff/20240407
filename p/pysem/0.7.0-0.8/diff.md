# Comparing `tmp/pysem-0.7.0.tar.gz` & `tmp/pysem-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysem-0.7.0.tar", last modified: Fri Apr 14 07:33:48 2023, max compression
+gzip compressed data, was "pysem-0.8.tar", last modified: Sun Apr  7 20:02:11 2024, max compression
```

## Comparing `pysem-0.7.0.tar` & `pysem-0.8.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.804971 pysem-0.7.0/
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1063 2021-02-26 22:10:43.000000 pysem-0.7.0/LICENSE
--rw-r--r--   0 mattis    (1000) mattis    (1000)       60 2021-02-26 22:10:43.000000 pysem-0.7.0/MANIFEST.in
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1896 2023-04-14 07:33:48.804971 pysem-0.7.0/PKG-INFO
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1165 2023-04-14 07:29:29.000000 pysem-0.7.0/README.md
--rw-r--r--   0 mattis    (1000) mattis    (1000)      403 2023-04-14 07:33:48.804971 pysem-0.7.0/setup.cfg
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1279 2023-04-14 07:27:47.000000 pysem-0.7.0/setup.py
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.801638 pysem-0.7.0/src/
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.801638 pysem-0.7.0/src/pysem/
--rw-r--r--   0 mattis    (1000) mattis    (1000)       91 2023-04-14 07:29:47.000000 pysem-0.7.0/src/pysem/__init__.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)        0 2022-05-23 11:11:52.000000 pysem-0.7.0/src/pysem/cli.py
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.804971 pysem-0.7.0/src/pysem/data/
--rw-r--r--   0 mattis    (1000) mattis    (1000)   857513 2023-04-14 07:27:15.000000 pysem-0.7.0/src/pysem/data/concepticon.zip
--rw-r--r--   0 mattis    (1000) mattis    (1000)   204330 2021-02-26 22:10:43.000000 pysem-0.7.0/src/pysem/data/sense.csv
--rw-r--r--   0 mattis    (1000) mattis    (1000)      546 2021-05-03 15:22:28.000000 pysem-0.7.0/src/pysem/data.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)    12242 2023-04-14 07:30:25.000000 pysem-0.7.0/src/pysem/glosses.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)     2722 2022-11-29 09:09:24.000000 pysem-0.7.0/src/pysem/main.py
--rw-r--r--   0 mattis    (1000) mattis    (1000)     2171 2021-05-03 17:22:50.000000 pysem-0.7.0/src/pysem/sense.py
-drwxr-xr-x   0 mattis    (1000) mattis    (1000)        0 2023-04-14 07:33:48.804971 pysem-0.7.0/src/pysem.egg-info/
--rw-r--r--   0 mattis    (1000) mattis    (1000)     1896 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/PKG-INFO
--rw-r--r--   0 mattis    (1000) mattis    (1000)      451 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/SOURCES.txt
--rw-r--r--   0 mattis    (1000) mattis    (1000)        1 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/dependency_links.txt
--rw-r--r--   0 mattis    (1000) mattis    (1000)       20 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/entry_points.txt
--rw-r--r--   0 mattis    (1000) mattis    (1000)        1 2021-05-03 17:25:48.000000 pysem-0.7.0/src/pysem.egg-info/not-zip-safe
--rw-r--r--   0 mattis    (1000) mattis    (1000)       95 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/requires.txt
--rw-r--r--   0 mattis    (1000) mattis    (1000)        6 2023-04-14 07:33:48.000000 pysem-0.7.0/src/pysem.egg-info/top_level.txt
+drwxr-xr-x   0 mattis    (1000) users      (985)        0 2024-04-07 20:02:11.712786 pysem-0.8/
+-rw-r--r--   0 mattis    (1000) users      (985)     1063 2021-06-02 01:37:24.000000 pysem-0.8/LICENSE
+-rw-r--r--   0 mattis    (1000) users      (985)       60 2021-06-02 01:37:24.000000 pysem-0.8/MANIFEST.in
+-rw-r--r--   0 mattis    (1000) users      (985)     2258 2024-04-07 20:02:11.712786 pysem-0.8/PKG-INFO
+-rw-r--r--   0 mattis    (1000) users      (985)     1202 2024-04-07 19:58:32.000000 pysem-0.8/README.md
+-rw-r--r--   0 mattis    (1000) users      (985)      403 2024-04-07 20:02:11.712786 pysem-0.8/setup.cfg
+-rw-r--r--   0 mattis    (1000) users      (985)     1303 2024-04-07 19:58:51.000000 pysem-0.8/setup.py
+drwxr-xr-x   0 mattis    (1000) users      (985)        0 2024-04-07 20:02:11.689452 pysem-0.8/src/
+drwxr-xr-x   0 mattis    (1000) users      (985)        0 2024-04-07 20:02:11.696119 pysem-0.8/src/pysem/
+-rw-r--r--   0 mattis    (1000) users      (985)       91 2024-04-07 19:58:45.000000 pysem-0.8/src/pysem/__init__.py
+-rw-r--r--   0 mattis    (1000) users      (985)        0 2022-07-10 07:58:59.000000 pysem-0.8/src/pysem/cli.py
+drwxr-xr-x   0 mattis    (1000) users      (985)        0 2024-04-07 20:02:11.709452 pysem-0.8/src/pysem/data/
+-rw-r--r--   0 mattis    (1000) users      (985)   867333 2024-04-07 19:55:04.000000 pysem-0.8/src/pysem/data/concepticon.zip
+-rw-r--r--   0 mattis    (1000) users      (985)   204330 2021-06-02 01:37:24.000000 pysem-0.8/src/pysem/data/sense.csv
+-rw-r--r--   0 mattis    (1000) users      (985)      546 2021-06-02 01:37:24.000000 pysem-0.8/src/pysem/data.py
+-rw-r--r--   0 mattis    (1000) users      (985)    12389 2024-04-07 20:00:18.000000 pysem-0.8/src/pysem/glosses.py
+-rw-r--r--   0 mattis    (1000) users      (985)     2722 2022-12-02 04:30:49.000000 pysem-0.8/src/pysem/main.py
+-rw-r--r--   0 mattis    (1000) users      (985)     2171 2021-06-02 01:37:24.000000 pysem-0.8/src/pysem/sense.py
+drwxr-xr-x   0 mattis    (1000) users      (985)        0 2024-04-07 20:02:11.709452 pysem-0.8/src/pysem.egg-info/
+-rw-r--r--   0 mattis    (1000) users      (985)     2258 2024-04-07 20:02:11.000000 pysem-0.8/src/pysem.egg-info/PKG-INFO
+-rw-r--r--   0 mattis    (1000) users      (985)      457 2024-04-07 20:02:11.000000 pysem-0.8/src/pysem.egg-info/SOURCES.txt
+-rw-r--r--   0 mattis    (1000) users      (985)        1 2024-04-07 20:02:11.000000 pysem-0.8/src/pysem.egg-info/dependency_links.txt
+-rw-r--r--   0 mattis    (1000) users      (985)        1 2021-06-02 18:22:23.000000 pysem-0.8/src/pysem.egg-info/not-zip-safe
+-rw-r--r--   0 mattis    (1000) users      (985)      100 2024-04-07 20:02:11.000000 pysem-0.8/src/pysem.egg-info/requires.txt
+-rw-r--r--   0 mattis    (1000) users      (985)        6 2024-04-07 20:02:11.000000 pysem-0.8/src/pysem.egg-info/top_level.txt
+drwxr-xr-x   0 mattis    (1000) users      (985)        0 2024-04-07 20:02:11.709452 pysem-0.8/tests/
+-rw-r--r--   0 mattis    (1000) users      (985)     2492 2021-06-13 09:36:05.000000 pysem-0.8/tests/test_glosses.py
+-rw-r--r--   0 mattis    (1000) users      (985)      410 2021-06-02 01:37:24.000000 pysem-0.8/tests/test_sense.py
```

### Comparing `pysem-0.7.0/LICENSE` & `pysem-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pysem-0.7.0/PKG-INFO` & `pysem-0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 Metadata-Version: 2.1
 Name: pysem
-Version: 0.7.0
+Version: 0.8
 Summary: Python library for manipulating semantic data in linguistics
 Home-page: https://github.com/lingpy/pysem
 Author: Johann-Mattis List
-Author-email: list@shh.mpg.de
+Author-email: mattis.list@uni-passau.de
 License: MIT
 Keywords: data
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: clldutils>=3.5
+Requires-Dist: csvw
+Requires-Dist: attrs>=20
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest>=4.3; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: coverage>=4.2; extra == "test"
 
 # PySem: Pysen library for handling semantic data in linguistics
 
-* **Current Version**: 0.7
-* **Concepticon Version**: [3.1.0](https://doi.org/10.5281/zenodo.7777629)
+* **Current Version**: 0.8
+* **Concepticon Version**: [3.2.0](https://doi.org/10.5281/zenodo.7298022)
  
 ## Usage Examples
 
 Retrieve the sense data assembled by S. A. Starostin in the STARLING software package and search for similar words:
 
 ```python
 >>> from pysem.sense import Sense
@@ -47,10 +56,8 @@
 >>> from pysem import to_concepticon
 >>> to_concepticon([{"gloss": "Fuß", pos: "noun"}], language="de"}])
 {'Fuß': [['1301', 'FOOT', 'noun', 19]]}
 ```
 
 ## How to Cite
 
-> List, Johann-Mattis (2023): PySeM. A Python library for handling semantic data in linguistics. Version 0.7 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
-
-
+> List, Johann-Mattis (2024): PySeM. A Python library for handling semantic data in linguistics [Software, Version 0.8]. With contributions by Johannes Englisch. URL: https://pypi.org/project/pysem, Passau: MCL Chair at the University of Passau.
```

### Comparing `pysem-0.7.0/setup.py` & `pysem-0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='pysem',
-    version='0.7.0',
+    version='0.8',
     license='MIT',
     description='Python library for manipulating semantic data in linguistics',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
     ],
     author='Johann-Mattis List',
-    author_email='list@shh.mpg.de',
+    author_email='mattis.list@uni-passau.de',
     url='https://github.com/lingpy/pysem',
     keywords='data',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     include_package_data=True,
     zip_safe=False,
     platforms='any',
     python_requires='>=3.5',
     install_requires=[
         'clldutils>=3.5',
+        'csvw',
         "attrs>=20"
     ],
     extras_require={
         'dev': ['black', 'wheel', 'twine'],
         'test': [
             'pytest>=4.3',
             'pytest-cov',
```

### Comparing `pysem-0.7.0/src/pysem/data/sense.csv` & `pysem-0.8/src/pysem/data/sense.csv`

 * *Files identical despite different names*

### Comparing `pysem-0.7.0/src/pysem/data.py` & `pysem-0.8/src/pysem/data.py`

 * *Files identical despite different names*

### Comparing `pysem-0.7.0/src/pysem/glosses.py` & `pysem-0.8/src/pysem/glosses.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,15 +284,15 @@
     splitter=",|;|:|/| or | OR ",
     marker='?!"¨:;,»«´“”*+-',
     brackets_open="([{（<",
     brackets_close=")]}）>",
     mappings=MAPPINGS,
 ):
     """
-    Map a given concept list to Concepticon (Version 3.1.0).
+    Map a given concept list to Concepticon (Version 3.2.0).
     """
     matches = {}
     for concept in concepts:
         gloss, pos = concept.get(gloss_ref), concept.get(pos_ref, "")
         if gloss:
             glosses = parse_gloss(
                 gloss,
@@ -334,17 +334,19 @@
                             row[1],
                             row[2],
                             row[3],
                             g.similarity(Gloss.from_string(text, pos=row[3])),
                         )
                     ]
 
+            # using a dictionary (key -> True) instead of a set because sets
+            # don't guarantee a stable element order.
             results = sorted(
-                set(results),
-                key=lambda x: (x[-1], 1 if g.pos == x[-2] else 0, x[-3]),
+                {row: True for row in results},
+                key=lambda x: (x[-1], 1 if pos == x[-2] else 0, x[-3]),
                 reverse=True,
             )[:max_matches]
             matches[gloss] = []
             for result in results:
                 matches[gloss] += [[result[0], result[1], result[3], result[4]]]
         else:
             raise ValueError("no glosses could be found")
```

### Comparing `pysem-0.7.0/src/pysem/main.py` & `pysem-0.8/src/pysem/main.py`

 * *Files identical despite different names*

### Comparing `pysem-0.7.0/src/pysem/sense.py` & `pysem-0.8/src/pysem/sense.py`

 * *Files identical despite different names*

### Comparing `pysem-0.7.0/src/pysem.egg-info/PKG-INFO` & `pysem-0.8/src/pysem.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 Metadata-Version: 2.1
 Name: pysem
-Version: 0.7.0
+Version: 0.8
 Summary: Python library for manipulating semantic data in linguistics
 Home-page: https://github.com/lingpy/pysem
 Author: Johann-Mattis List
-Author-email: list@shh.mpg.de
+Author-email: mattis.list@uni-passau.de
 License: MIT
 Keywords: data
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: clldutils>=3.5
+Requires-Dist: csvw
+Requires-Dist: attrs>=20
 Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: wheel; extra == "dev"
+Requires-Dist: twine; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: pytest>=4.3; extra == "test"
+Requires-Dist: pytest-cov; extra == "test"
+Requires-Dist: coverage>=4.2; extra == "test"
 
 # PySem: Pysen library for handling semantic data in linguistics
 
-* **Current Version**: 0.7
-* **Concepticon Version**: [3.1.0](https://doi.org/10.5281/zenodo.7777629)
+* **Current Version**: 0.8
+* **Concepticon Version**: [3.2.0](https://doi.org/10.5281/zenodo.7298022)
  
 ## Usage Examples
 
 Retrieve the sense data assembled by S. A. Starostin in the STARLING software package and search for similar words:
 
 ```python
 >>> from pysem.sense import Sense
@@ -47,10 +56,8 @@
 >>> from pysem import to_concepticon
 >>> to_concepticon([{"gloss": "Fuß", pos: "noun"}], language="de"}])
 {'Fuß': [['1301', 'FOOT', 'noun', 19]]}
 ```
 
 ## How to Cite
 
-> List, Johann-Mattis (2023): PySeM. A Python library for handling semantic data in linguistics. Version 0.7 URL: https://github.com/lingpy/pysem/, Leipzig: Max Planck Institute for Evolutionary Anthropology.
-
-
+> List, Johann-Mattis (2024): PySeM. A Python library for handling semantic data in linguistics [Software, Version 0.8]. With contributions by Johannes Englisch. URL: https://pypi.org/project/pysem, Passau: MCL Chair at the University of Passau.
```

