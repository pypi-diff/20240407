# Comparing `tmp/pytubefix-5.0rc2.tar.gz` & `tmp/pytubefix-5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytubefix-5.0rc2.tar", last modified: Wed Apr  3 14:49:16 2024, max compression
+gzip compressed data, was "pytubefix-5.1rc1.tar", last modified: Sun Apr  7 03:26:41 2024, max compression
```

## Comparing `pytubefix-5.0rc2.tar` & `pytubefix-5.1rc1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 14:49:16.556474 pytubefix-5.0rc2/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1101 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/LICENSE
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       18 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/MANIFEST.in
--rw-r--r--   0 estoque   (1000) estoque   (1000)     4506 2024-04-03 14:49:16.556474 pytubefix-5.0rc2/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3174 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/README.md
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1524 2024-04-03 14:48:19.000000 pytubefix-5.0rc2/pyproject.toml
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 14:49:16.548474 pytubefix-5.0rc2/pytubefix/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      614 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    20098 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6595 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/captions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1121 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/chapters.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5645 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/cipher.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    17032 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      786 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/colors.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 14:49:16.552474 pytubefix-5.0rc2/pytubefix/contrib/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        0 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/contrib/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    19995 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/contrib/channel.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14600 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/contrib/playlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    11048 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/contrib/search.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     4115 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18319 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/extract.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     9944 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/helpers.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    17414 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/innertube.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     4311 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/itags.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    41663 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/jsinterp.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1483 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/metadata.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      478 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/monostate.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5960 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/parser.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14289 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/query.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     8817 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/request.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    14818 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/pytubefix/streams.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-03 14:47:15.000000 pytubefix-5.0rc2/pytubefix/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 14:49:16.556474 pytubefix-5.0rc2/pytubefix.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     4506 2024-04-03 14:49:16.000000 pytubefix-5.0rc2/pytubefix.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1029 2024-04-03 14:49:16.000000 pytubefix-5.0rc2/pytubefix.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-03 14:49:16.000000 pytubefix-5.0rc2/pytubefix.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       49 2024-04-03 14:49:16.000000 pytubefix-5.0rc2/pytubefix.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       10 2024-04-03 14:49:16.000000 pytubefix-5.0rc2/pytubefix.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-03 14:49:16.556474 pytubefix-5.0rc2/setup.cfg
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 14:49:16.556474 pytubefix-5.0rc2/tests/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6579 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_captions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1360 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_cipher.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18009 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3626 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2963 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_extract.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     5060 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_helpers.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      279 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_itags.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1939 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_main.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      501 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_metadata.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1412 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_parser.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     6172 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_query.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1882 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_request.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    13661 2024-04-03 14:44:53.000000 pytubefix-5.0rc2/tests/test_streams.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-07 03:26:41.784804 pytubefix-5.1rc1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1101 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/LICENSE
+-rw-rw-r--   0 juan      (1000) juan      (1000)       18 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/MANIFEST.in
+-rw-r--r--   0 juan      (1000) juan      (1000)     4506 2024-04-07 03:26:41.784804 pytubefix-5.1rc1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3174 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/README.md
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1524 2024-04-07 03:25:29.000000 pytubefix-5.1rc1/pyproject.toml
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-07 03:26:41.780804 pytubefix-5.1rc1/pytubefix/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      614 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    20098 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6595 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1358 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/chapters.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5645 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17032 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      786 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/colors.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-07 03:26:41.780804 pytubefix-5.1rc1/pytubefix/contrib/
+-rw-rw-r--   0 juan      (1000) juan      (1000)        0 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/contrib/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    19995 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/contrib/channel.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14600 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/contrib/playlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    11072 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/contrib/search.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4115 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18319 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     9944 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    17414 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/innertube.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     4311 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    41663 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/jsinterp.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1483 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      478 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/monostate.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5960 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14289 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     8817 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    14818 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/pytubefix/streams.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       75 2024-04-07 03:24:41.000000 pytubefix-5.1rc1/pytubefix/version.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-07 03:26:41.784804 pytubefix-5.1rc1/pytubefix.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     4506 2024-04-07 03:26:41.000000 pytubefix-5.1rc1/pytubefix.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1029 2024-04-07 03:26:41.000000 pytubefix-5.1rc1/pytubefix.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-04-07 03:26:41.000000 pytubefix-5.1rc1/pytubefix.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       49 2024-04-07 03:26:41.000000 pytubefix-5.1rc1/pytubefix.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       10 2024-04-07 03:26:41.000000 pytubefix-5.1rc1/pytubefix.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-04-07 03:26:41.784804 pytubefix-5.1rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-04-07 03:26:41.784804 pytubefix-5.1rc1/tests/
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6579 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_captions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1360 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_cipher.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18009 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3626 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2963 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_extract.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     5060 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_helpers.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      279 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_itags.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1939 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_main.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      501 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_metadata.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1412 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_parser.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     6172 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_query.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1882 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_request.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    13661 2024-04-07 02:15:15.000000 pytubefix-5.1rc1/tests/test_streams.py
```

### Comparing `pytubefix-5.0rc2/LICENSE` & `pytubefix-5.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/PKG-INFO` & `pytubefix-5.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.0rc2
+Version: 5.1rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.0rc2 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.1rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.0rc2/README.md` & `pytubefix-5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pyproject.toml` & `pytubefix-5.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytubefix"
-version = "5.0-rc2"
+version = "5.1-rc1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python3 library for downloading YouTube Videos."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT license"}
```

### Comparing `pytubefix-5.0rc2/pytubefix/__init__.py` & `pytubefix-5.1rc1/pytubefix/__init__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/__main__.py` & `pytubefix-5.1rc1/pytubefix/__main__.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/captions.py` & `pytubefix-5.1rc1/pytubefix/captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/chapters.py` & `pytubefix-5.1rc1/pytubefix/chapters.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,30 @@
+# Native python imports
 from datetime import timedelta
-from dataclasses import dataclass
+from typing import List
 
 
-@dataclass
 class ChapterThumbnail:
     """Container for chapter thumbnails."""
-    width: int
-    height: int
-    url: str
+
+    def __init__(self, width: int, height: int, url: str):
+        self.width = width
+        self.height = height
+        self.url = url
+
+    def __repr__(self):
+        return f'<pytubefix.chapters.ChapterThumbnail: width={self.width}, height={self.height}, url={self.url}>'
 
 
 class Chapter:
     """Container for chapters tracks."""
     title: str
     start_seconds: int
     duration: int  # in seconds
-    thumbnails: list[ChapterThumbnail]
+    thumbnails: List[ChapterThumbnail]
 
     def __init__(self, chapter_data: dict, duration: int):
         data = chapter_data['chapterRenderer']
 
         self.title = data['title']['simpleText']
         self.start_seconds = int(data['timeRangeStartMillis'] / 1000)
         self.duration = duration
```

### Comparing `pytubefix-5.0rc2/pytubefix/cipher.py` & `pytubefix-5.1rc1/pytubefix/cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/cli.py` & `pytubefix-5.1rc1/pytubefix/cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/colors.py` & `pytubefix-5.1rc1/pytubefix/colors.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/contrib/channel.py` & `pytubefix-5.1rc1/pytubefix/contrib/channel.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/contrib/playlist.py` & `pytubefix-5.1rc1/pytubefix/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/contrib/search.py` & `pytubefix-5.1rc1/pytubefix/contrib/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Module for interacting with YouTube search."""
 # Native python imports
 import logging
+from typing import List
 
 # Local imports
 from pytubefix import YouTube, Channel, Playlist
 from pytubefix.helpers import deprecated
 from pytubefix.innertube import InnerTube
 
 logger = logging.getLogger(__name__)
@@ -42,15 +43,15 @@
         if self._completion_suggestions:
             return self._completion_suggestions
         if self.results:
             self._completion_suggestions = self._initial_results['refinements']
         return self._completion_suggestions
 
     @property
-    def videos(self) -> list[YouTube]:
+    def videos(self) -> List[YouTube]:
         """Returns the search result videos.
 
         On first call, will generate and return the first set of results.
         Additional results can be generated using ``.get_next_results()``.
 
         :rtype: list[YouTube]
         :returns:
@@ -63,15 +64,15 @@
             self._results['shorts'] = results['shorts']
             self._results['playlist'] = results['playlist']
             self._results['channel'] = results['channel']
 
         return [items for items in self._results['videos']]
 
     @property
-    def shorts(self) -> list[YouTube]:
+    def shorts(self) -> List[YouTube]:
         """Returns the search result shorts.
 
         On first call, will generate and return the first set of results.
         Additional results can be generated using ``.get_next_results()``.
 
         :rtype: list[YouTube]
         :returns:
@@ -84,15 +85,15 @@
             self._results['shorts'] = results['shorts']
             self._results['playlist'] = results['playlist']
             self._results['channel'] = results['channel']
 
         return [items for items in self._results['shorts']]
 
     @property
-    def playlist(self) -> list[Playlist]:
+    def playlist(self) -> List[Playlist]:
         """Returns the search result playlist.
 
         On first call, will generate and return the first set of results.
         Additional results can be generated using ``.get_next_results()``.
 
         :rtype: list[Playlist]
         :returns:
@@ -105,15 +106,15 @@
             self._results['shorts'] = results['shorts']
             self._results['playlist'] = results['playlist']
             self._results['channel'] = results['channel']
 
         return [items for items in self._results['playlist']]
 
     @property
-    def channel(self) -> list[Channel]:
+    def channel(self) -> List[Channel]:
         """Returns the search result channel.
 
         On first call, will generate and return the first set of results.
         Additional results can be generated using ``.get_next_results()``.
 
         :rtype: list[Channel]
         :returns:
```

### Comparing `pytubefix-5.0rc2/pytubefix/exceptions.py` & `pytubefix-5.1rc1/pytubefix/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/extract.py` & `pytubefix-5.1rc1/pytubefix/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     try:
         regex_search(r"og:restrictions:age", watch_html, group=0)
     except RegexMatchError:
         return False
     return True
 
 
-def playability_status(watch_html: str) -> tuple[str, str]:
+def playability_status(watch_html: str) -> Tuple[Any, Any]:
     """Return the playability status and status explanation of a video.
 
     For example, a video may have a status of LOGIN_REQUIRED, and an explanation
     of "This is a private video. Please sign in to verify that you may see it."
 
     This explanation is what gets incorporated into the media player overlay.
```

### Comparing `pytubefix-5.0rc2/pytubefix/helpers.py` & `pytubefix-5.1rc1/pytubefix/helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/innertube.py` & `pytubefix-5.1rc1/pytubefix/innertube.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/itags.py` & `pytubefix-5.1rc1/pytubefix/itags.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/jsinterp.py` & `pytubefix-5.1rc1/pytubefix/jsinterp.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/metadata.py` & `pytubefix-5.1rc1/pytubefix/metadata.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/parser.py` & `pytubefix-5.1rc1/pytubefix/parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/query.py` & `pytubefix-5.1rc1/pytubefix/query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/request.py` & `pytubefix-5.1rc1/pytubefix/request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix/streams.py` & `pytubefix-5.1rc1/pytubefix/streams.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/pytubefix.egg-info/PKG-INFO` & `pytubefix-5.1rc1/pytubefix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytubefix
-Version: 5.0rc2
+Version: 5.1rc1
 Summary: Python3 library for downloading YouTube Videos.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: MIT license
 Project-URL: Homepage, https://github.com/juanbindez/pytubefix
 Project-URL: Bug Reports, https://github.com/juanbindez/pytubefix/issues
 Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytubefix Version: 5.0rc2 Summary: Python3 library
+Metadata-Version: 2.1 Name: pytubefix Version: 5.1rc1 Summary: Python3 library
 for downloading YouTube Videos. Author-email: Juan Bindez
 gmail.com> License: MIT license Project-URL: Homepage, https://github.com/
 juanbindez/pytubefix Project-URL: Bug Reports, https://github.com/juanbindez/
 pytubefix/issues Project-URL: Read the Docs, http://pytubefix.readthedocs.io/
 Keywords: youtube,download,video,stream Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pytubefix-5.0rc2/pytubefix.egg-info/SOURCES.txt` & `pytubefix-5.1rc1/pytubefix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_captions.py` & `pytubefix-5.1rc1/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_cipher.py` & `pytubefix-5.1rc1/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_cli.py` & `pytubefix-5.1rc1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_exceptions.py` & `pytubefix-5.1rc1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_extract.py` & `pytubefix-5.1rc1/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_helpers.py` & `pytubefix-5.1rc1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_main.py` & `pytubefix-5.1rc1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_parser.py` & `pytubefix-5.1rc1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_query.py` & `pytubefix-5.1rc1/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_request.py` & `pytubefix-5.1rc1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytubefix-5.0rc2/tests/test_streams.py` & `pytubefix-5.1rc1/tests/test_streams.py`

 * *Files identical despite different names*

