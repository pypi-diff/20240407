# Comparing `tmp/unicodedata_reader-1.3.0.tar.gz` & `tmp/unicodedata_reader-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata_reader-1.3.0.tar", max compression
+gzip compressed data, was "unicodedata_reader-1.3.1.tar", max compression
```

## Comparing `unicodedata_reader-1.3.0.tar` & `unicodedata_reader-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/LICENSE
--rw-r--r--   0        0        0     3120 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/README.md
--rw-r--r--   0        0        0      648 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4829 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4360 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/compressor.py
--rw-r--r--   0        0        0      982 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/east_asian_width.py
--rwxr-xr-x   0        0        0     1220 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    14674 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      558 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      671 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     4537 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/reader.py
--rw-r--r--   0        0        0     2160 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/set.py
--rwxr-xr-x   0        0        0      996 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 07:50:32.999719 unicodedata_reader-1.3.1/LICENSE
+-rw-r--r--   0        0        0     3114 2024-04-07 07:50:32.999719 unicodedata_reader-1.3.1/README.md
+-rw-r--r--   0        0        0      648 2024-04-07 07:50:32.999719 unicodedata_reader-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4829 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    14759 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     4537 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2156 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-07 07:50:33.003719 unicodedata_reader-1.3.1/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.1/PKG-INFO
```

### Comparing `unicodedata_reader-1.3.0/LICENSE` & `unicodedata_reader-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/README.md` & `unicodedata_reader-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 ## Python
 
 ```python
 import unicodedata_reader
 
 reader = unicodedata_reader.UnicodeDataReader.default
 lb = reader.line_break()
-print(lb.value(0x41))
+print(lb[0x41])
 ```
 The example above prints `AL`,
 the [Line_Break property] value for U+0041.
 Please also see [line_break_test.py] for more usages.
 
 [line_break_test.py]: https://github.com/kojiishi/unicodedata-reader/blob/main/tests/line_break_test.py
```

### Comparing `unicodedata_reader-1.3.0/pyproject.toml` & `unicodedata_reader-1.3.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "1.3.0"
+version = "1.3.1"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/__main__.py` & `unicodedata_reader-1.3.1/unicodedata_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-1.3.1/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/cli.py` & `unicodedata_reader-1.3.1/unicodedata_reader/cli.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/compressor.py` & `unicodedata_reader-1.3.1/unicodedata_reader/compressor.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/east_asian_width.py` & `unicodedata_reader-1.3.1/unicodedata_reader/east_asian_width.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/emoji.py` & `unicodedata_reader-1.3.1/unicodedata_reader/emoji.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/entry.py` & `unicodedata_reader-1.3.1/unicodedata_reader/entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,14 +214,17 @@
         self._ensure_multi_iterable()
         return self._entries.__iter__()
 
     def __len__(self):
         self._ensure_multi_iterable()
         return len(self._entries)
 
+    def __getitem__(self, code: int) -> Any:
+        return self.value(code)
+
     def missing_value(self, code: int):
         if self._missing_entries:
             # `_missing_entries` can overlap, iterate all entries.
             for entry in self._missing_entries:
                 if entry.is_in_range(code):
                     return entry.value
         return None
@@ -247,15 +250,15 @@
         self._entries = UnicodeDataEntry.from_values(values)
 
     def unicodes(self) -> Iterable[int]:
         """Returns a list of Unicode code points defined in this entries."""
         self._ensure_multi_iterable()
         return itertools.chain(*(e.range() for e in self._entries))
 
-    def value(self, code: int):
+    def value(self, code: int) -> Any:
         """Returns the value for the given code point."""
         self._ensure_multi_iterable()
         for entry in self._entries:
             if code < entry.min:
                 return self.missing_value(code)
             if code <= entry.max:
                 return entry.value
```

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/general_category.py` & `unicodedata_reader-1.3.1/unicodedata_reader/general_category.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/line_break.py` & `unicodedata_reader-1.3.1/unicodedata_reader/line_break.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/reader.py` & `unicodedata_reader-1.3.1/unicodedata_reader/reader.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/set.py` & `unicodedata_reader-1.3.1/unicodedata_reader/set.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     def __init__(self,
                  entries: UnicodeDataEntries = None,
                  pred: Callable[[Any], bool] = None) -> None:
         self.set = set()  # type: Set[int]
         if entries:
             self.add_entries(entries, pred)
 
-    def __contains__(self, code_point: int) -> bool:
+    def contains(self, code_point: int) -> bool:
         return code_point in self.set
 
     def __iter__(self) -> Iterable[int]:
         return self.set.__iter__()
 
     def __isub__(self, other: 'Set') -> 'Set':
         self.set -= other.set
```

### Comparing `unicodedata_reader-1.3.0/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-1.3.1/unicodedata_reader/vertical_orientation.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.0/PKG-INFO` & `unicodedata_reader-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 1.3.0
+Version: 1.3.1
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
@@ -64,15 +64,15 @@
 ## Python
 
 ```python
 import unicodedata_reader
 
 reader = unicodedata_reader.UnicodeDataReader.default
 lb = reader.line_break()
-print(lb.value(0x41))
+print(lb[0x41])
 ```
 The example above prints `AL`,
 the [Line_Break property] value for U+0041.
 Please also see [line_break_test.py] for more usages.
 
 [line_break_test.py]: https://github.com/kojiishi/unicodedata-reader/blob/main/tests/line_break_test.py
```

