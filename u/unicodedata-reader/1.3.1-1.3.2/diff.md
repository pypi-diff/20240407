# Comparing `tmp/unicodedata_reader-1.3.1.tar.gz` & `tmp/unicodedata_reader-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata_reader-1.3.1.tar", max compression
+gzip compressed data, was "unicodedata_reader-1.3.2.tar", max compression
```

## Comparing `unicodedata_reader-1.3.1.tar` & `unicodedata_reader-1.3.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-07 07:50:32.999719 unicodedata_reader-1.3.1/LICENSE
--rw-r--r--   0        0        0     3114 2024-04-07 07:50:32.999719 unicodedata_reader-1.3.1/README.md
--rw-r--r--   0        0        0      648 2024-04-07 07:50:32.999719 unicodedata_reader-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4829 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4360 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/compressor.py
--rw-r--r--   0        0        0      982 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/east_asian_width.py
--rwxr-xr-x   0        0        0     1220 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    14759 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      558 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      671 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     4537 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/reader.py
--rw-r--r--   0        0        0     2156 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/set.py
--rwxr-xr-x   0        0        0      996 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/LICENSE
+-rw-r--r--   0        0        0     3114 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/README.md
+-rw-r--r--   0        0        0      648 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4829 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    14759 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     4537 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2160 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.2/PKG-INFO
```

### Comparing `unicodedata_reader-1.3.1/LICENSE` & `unicodedata_reader-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/README.md` & `unicodedata_reader-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/pyproject.toml` & `unicodedata_reader-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "1.3.1"
+version = "1.3.2"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/__main__.py` & `unicodedata_reader-1.3.2/unicodedata_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-1.3.2/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/cli.py` & `unicodedata_reader-1.3.2/unicodedata_reader/cli.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/compressor.py` & `unicodedata_reader-1.3.2/unicodedata_reader/compressor.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/east_asian_width.py` & `unicodedata_reader-1.3.2/unicodedata_reader/east_asian_width.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/emoji.py` & `unicodedata_reader-1.3.2/unicodedata_reader/emoji.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/entry.py` & `unicodedata_reader-1.3.2/unicodedata_reader/entry.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/general_category.py` & `unicodedata_reader-1.3.2/unicodedata_reader/general_category.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/line_break.py` & `unicodedata_reader-1.3.2/unicodedata_reader/line_break.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/reader.py` & `unicodedata_reader-1.3.2/unicodedata_reader/reader.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/set.py` & `unicodedata_reader-1.3.2/unicodedata_reader/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self,
                  entries: UnicodeDataEntries = None,
                  pred: Callable[[Any], bool] = None) -> None:
         self.set = set()  # type: Set[int]
         if entries:
             self.add_entries(entries, pred)
 
-    def contains(self, code_point: int) -> bool:
+    def __contains__(self, code_point: int) -> bool:
         return code_point in self.set
 
     def __iter__(self) -> Iterable[int]:
         return self.set.__iter__()
 
     def __isub__(self, other: 'Set') -> 'Set':
         self.set -= other.set
```

### Comparing `unicodedata_reader-1.3.1/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-1.3.2/unicodedata_reader/vertical_orientation.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.1/PKG-INFO` & `unicodedata_reader-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 1.3.1
+Version: 1.3.2
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

