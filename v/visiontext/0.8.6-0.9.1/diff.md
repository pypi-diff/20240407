# Comparing `tmp/visiontext-0.8.6.tar.gz` & `tmp/visiontext-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visiontext-0.8.6.tar", last modified: Mon Jan 22 09:46:04 2024, max compression
+gzip compressed data, was "visiontext-0.9.1.tar", last modified: Mon Jan 22 09:47:35 2024, max compression
```

## Comparing `visiontext-0.8.6.tar` & `visiontext-0.9.1.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.305893 visiontext-0.8.6/
--rw-------   0 gings    (14999) lmb-mit   (1061)    11339 2024-01-22 09:09:20.000000 visiontext-0.8.6/LICENSE
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2726 2024-01-22 09:46:04.305893 visiontext-0.8.6/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)     1411 2024-01-22 09:45:45.000000 visiontext-0.8.6/README.md
--rw-------   0 gings    (14999) lmb-mit   (1061)     2768 2024-01-22 09:09:20.000000 visiontext-0.8.6/pyproject.toml
--rw-------   0 gings    (14999) lmb-mit   (1061)      218 2024-01-22 09:45:45.000000 visiontext-0.8.6/requirements.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       38 2024-01-22 09:46:04.309893 visiontext-0.8.6/setup.cfg
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.181891 visiontext-0.8.6/src/
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.245892 visiontext-0.8.6/src/visiontext/
--rw-------   0 gings    (14999) lmb-mit   (1061)       51 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      120 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/__main__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     7839 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/bboxes.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2123 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/cacheutils.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5630 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/colormaps.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.265892 visiontext-0.8.6/src/visiontext/datasets/
--rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/datasets/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1228 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/distutils.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1601 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/font.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6413 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/htmltools.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     5483 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/images.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2930 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/imports.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.277892 visiontext-0.8.6/src/visiontext/iotools/
--rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/iotools/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2861 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/iotools/feature_compression.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      568 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/iotools/lmdbext.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4511 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/iotools/tar_indexer.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     9157 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/iotools/tar_lookup.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      220 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/mathutils.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.289893 visiontext-0.8.6/src/visiontext/nlp/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      238 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/nlp/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     6113 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/nlp/lemmatizer.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     4460 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/nlp/nltktools.py
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)      418 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/nlp/regextools.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2801 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/pandatools.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      334 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/plots.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.293893 visiontext-0.8.6/src/visiontext/profiling/
--rw-------   0 gings    (14999) lmb-mit   (1061)      179 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/profiling/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      790 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/profiling/code_profiler.py
--rw-------   0 gings    (14999) lmb-mit   (1061)    10180 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/profiling/hardware_profiler.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      199 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/profiling.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.297893 visiontext-0.8.6/src/visiontext/run/
--rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/run/__init__.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     1578 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/run/profile_gpu.py
--rw-------   0 gings    (14999) lmb-mit   (1061)      589 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/spacytools.py
--rw-------   0 gings    (14999) lmb-mit   (1061)     2957 2024-01-22 09:45:45.000000 visiontext-0.8.6/src/visiontext/visualize.py
-drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:46:04.301893 visiontext-0.8.6/src/visiontext.egg-info/
--rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2726 2024-01-22 09:46:04.000000 visiontext-0.8.6/src/visiontext.egg-info/PKG-INFO
--rw-------   0 gings    (14999) lmb-mit   (1061)     1248 2024-01-22 09:46:04.000000 visiontext-0.8.6/src/visiontext.egg-info/SOURCES.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2024-01-22 09:46:04.000000 visiontext-0.8.6/src/visiontext.egg-info/dependency_links.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)      139 2024-01-22 09:46:04.000000 visiontext-0.8.6/src/visiontext.egg-info/requires.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)       11 2024-01-22 09:46:04.000000 visiontext-0.8.6/src/visiontext.egg-info/top_level.txt
--rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-10-29 14:26:59.000000 visiontext-0.8.6/src/visiontext.egg-info/zip-safe
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.139645 visiontext-0.9.1/
+-rw-------   0 gings    (14999) lmb-mit   (1061)    11339 2024-01-22 09:09:20.000000 visiontext-0.9.1/LICENSE
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2726 2024-01-22 09:47:35.139645 visiontext-0.9.1/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1411 2024-01-22 09:47:15.000000 visiontext-0.9.1/README.md
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2768 2024-01-22 09:09:20.000000 visiontext-0.9.1/pyproject.toml
+-rw-------   0 gings    (14999) lmb-mit   (1061)      218 2024-01-22 09:47:15.000000 visiontext-0.9.1/requirements.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       38 2024-01-22 09:47:35.139645 visiontext-0.9.1/setup.cfg
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.007642 visiontext-0.9.1/src/
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.067644 visiontext-0.9.1/src/visiontext/
+-rw-------   0 gings    (14999) lmb-mit   (1061)       51 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      120 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/__main__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     7839 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/bboxes.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2123 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/cacheutils.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5630 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/colormaps.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.091644 visiontext-0.9.1/src/visiontext/datasets/
+-rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/datasets/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1228 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/distutils.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1601 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/font.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6413 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/htmltools.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     5483 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/images.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2930 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/imports.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.103644 visiontext-0.9.1/src/visiontext/iotools/
+-rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/iotools/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2861 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/iotools/feature_compression.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      568 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/iotools/lmdbext.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4511 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/iotools/tar_indexer.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     9157 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/iotools/tar_lookup.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      220 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/mathutils.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.115645 visiontext-0.9.1/src/visiontext/nlp/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      238 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/nlp/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     6113 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/nlp/lemmatizer.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     4460 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/nlp/nltktools.py
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)      418 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/nlp/regextools.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2801 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/pandatools.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      334 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/plots.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.123645 visiontext-0.9.1/src/visiontext/profiling/
+-rw-------   0 gings    (14999) lmb-mit   (1061)      179 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/profiling/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      790 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/profiling/code_profiler.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)    10180 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/profiling/hardware_profiler.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      199 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/profiling.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.131645 visiontext-0.9.1/src/visiontext/run/
+-rw-------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/run/__init__.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1578 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/run/profile_gpu.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)      589 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/spacytools.py
+-rw-------   0 gings    (14999) lmb-mit   (1061)     2957 2024-01-22 09:47:15.000000 visiontext-0.9.1/src/visiontext/visualize.py
+drwx------   0 gings    (14999) lmb-mit   (1061)        0 2024-01-22 09:47:35.135645 visiontext-0.9.1/src/visiontext.egg-info/
+-rw-r--r--   0 gings    (14999) lmb-mit   (1061)     2726 2024-01-22 09:47:34.000000 visiontext-0.9.1/src/visiontext.egg-info/PKG-INFO
+-rw-------   0 gings    (14999) lmb-mit   (1061)     1248 2024-01-22 09:47:34.000000 visiontext-0.9.1/src/visiontext.egg-info/SOURCES.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2024-01-22 09:47:34.000000 visiontext-0.9.1/src/visiontext.egg-info/dependency_links.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)      139 2024-01-22 09:47:34.000000 visiontext-0.9.1/src/visiontext.egg-info/requires.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)       11 2024-01-22 09:47:34.000000 visiontext-0.9.1/src/visiontext.egg-info/top_level.txt
+-rw-------   0 gings    (14999) lmb-mit   (1061)        1 2023-10-29 14:26:59.000000 visiontext-0.9.1/src/visiontext.egg-info/zip-safe
```

### Comparing `visiontext-0.8.6/LICENSE` & `visiontext-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/PKG-INFO` & `visiontext-0.9.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visiontext
-Version: 0.8.6
+Version: 0.9.1
 Summary: Utilities for deep learning on multimodal data.
 Author: simonging
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/visiontext
 Keywords: python,jupyter,notebook,lab,ipython,html,pandas,matplotlib,pytorch,numpy
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: visiontext Version: 0.8.6 Summary: Utilities for
+Metadata-Version: 2.1 Name: visiontext Version: 0.9.1 Summary: Utilities for
 deep learning on multimodal data. Author: simonging License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/visiontext Keywords:
 python,jupyter,notebook,lab,ipython,html,pandas,matplotlib,pytorch,numpy
 Platform: any Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `visiontext-0.8.6/README.md` & `visiontext-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/pyproject.toml` & `visiontext-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/bboxes.py` & `visiontext-0.9.1/src/visiontext/bboxes.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/cacheutils.py` & `visiontext-0.9.1/src/visiontext/cacheutils.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/colormaps.py` & `visiontext-0.9.1/src/visiontext/colormaps.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/distutils.py` & `visiontext-0.9.1/src/visiontext/distutils.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/font.py` & `visiontext-0.9.1/src/visiontext/font.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/htmltools.py` & `visiontext-0.9.1/src/visiontext/htmltools.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/images.py` & `visiontext-0.9.1/src/visiontext/images.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/imports.py` & `visiontext-0.9.1/src/visiontext/imports.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/iotools/feature_compression.py` & `visiontext-0.9.1/src/visiontext/iotools/feature_compression.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/iotools/lmdbext.py` & `visiontext-0.9.1/src/visiontext/iotools/lmdbext.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/iotools/tar_indexer.py` & `visiontext-0.9.1/src/visiontext/iotools/tar_indexer.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/iotools/tar_lookup.py` & `visiontext-0.9.1/src/visiontext/iotools/tar_lookup.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/nlp/lemmatizer.py` & `visiontext-0.9.1/src/visiontext/nlp/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/nlp/nltktools.py` & `visiontext-0.9.1/src/visiontext/nlp/nltktools.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/pandatools.py` & `visiontext-0.9.1/src/visiontext/pandatools.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/profiling/code_profiler.py` & `visiontext-0.9.1/src/visiontext/profiling/code_profiler.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/profiling/hardware_profiler.py` & `visiontext-0.9.1/src/visiontext/profiling/hardware_profiler.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/run/profile_gpu.py` & `visiontext-0.9.1/src/visiontext/run/profile_gpu.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/spacytools.py` & `visiontext-0.9.1/src/visiontext/spacytools.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext/visualize.py` & `visiontext-0.9.1/src/visiontext/visualize.py`

 * *Files identical despite different names*

### Comparing `visiontext-0.8.6/src/visiontext.egg-info/PKG-INFO` & `visiontext-0.9.1/src/visiontext.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visiontext
-Version: 0.8.6
+Version: 0.9.1
 Summary: Utilities for deep learning on multimodal data.
 Author: simonging
 License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/visiontext
 Keywords: python,jupyter,notebook,lab,ipython,html,pandas,matplotlib,pytorch,numpy
 Platform: any
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: visiontext Version: 0.8.6 Summary: Utilities for
+Metadata-Version: 2.1 Name: visiontext Version: 0.9.1 Summary: Utilities for
 deep learning on multimodal data. Author: simonging License: Apache-2.0
 Project-URL: Project-URL, https://github.com/simonging/visiontext Keywords:
 python,jupyter,notebook,lab,ipython,html,pandas,matplotlib,pytorch,numpy
 Platform: any Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `visiontext-0.8.6/src/visiontext.egg-info/SOURCES.txt` & `visiontext-0.9.1/src/visiontext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

