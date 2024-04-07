# Comparing `tmp/unicodedata_reader-1.3.3.tar.gz` & `tmp/unicodedata_reader-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata_reader-1.3.3.tar", max compression
+gzip compressed data, was "unicodedata_reader-1.3.4.tar", max compression
```

## Comparing `unicodedata_reader-1.3.3.tar` & `unicodedata_reader-1.3.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/LICENSE
--rw-r--r--   0        0        0     3114 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/README.md
--rw-r--r--   0        0        0      648 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4829 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4360 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/compressor.py
--rw-r--r--   0        0        0      982 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/east_asian_width.py
--rwxr-xr-x   0        0        0     1220 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    14679 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      558 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      671 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     5090 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/reader.py
--rw-r--r--   0        0        0     2019 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/set.py
--rwxr-xr-x   0        0        0      996 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 12:47:39.472876 unicodedata_reader-1.3.4/LICENSE
+-rw-r--r--   0        0        0     3114 2024-04-07 12:47:39.472876 unicodedata_reader-1.3.4/README.md
+-rw-r--r--   0        0        0      648 2024-04-07 12:47:39.472876 unicodedata_reader-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4829 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    14771 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     5090 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2019 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-07 12:47:39.476876 unicodedata_reader-1.3.4/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.4/PKG-INFO
```

### Comparing `unicodedata_reader-1.3.3/LICENSE` & `unicodedata_reader-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/README.md` & `unicodedata_reader-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/pyproject.toml` & `unicodedata_reader-1.3.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "1.3.3"
+version = "1.3.4"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/__main__.py` & `unicodedata_reader-1.3.4/unicodedata_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-1.3.4/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/cli.py` & `unicodedata_reader-1.3.4/unicodedata_reader/cli.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/compressor.py` & `unicodedata_reader-1.3.4/unicodedata_reader/compressor.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/east_asian_width.py` & `unicodedata_reader-1.3.4/unicodedata_reader/east_asian_width.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/emoji.py` & `unicodedata_reader-1.3.4/unicodedata_reader/emoji.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/entry.py` & `unicodedata_reader-1.3.4/unicodedata_reader/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from typing import Sequence
 from typing import Union
 from typing import Tuple
 
 _logger = logging.getLogger('UnicodeDataEntry')
 
 
-def u_hex(value):
+def u_hex(value: int) -> str:
     return f'{value:04X}'
 
 
 def u_enc(c, encoding):
     code = 0
     for byte in c.encode(encoding, 'ignore'):
         code = code * 256 + byte
@@ -75,24 +75,32 @@
 
     def range(self):
         return range(self.min, self.max + 1)
 
     def is_in_range(self, code: int) -> bool:
         return code >= self.min and code <= self.max
 
+    @staticmethod
+    def to_codes(entries: Iterable['UnicodeDataEntry']):
+        return itertools.chain(*(e.range() for e in entries))
+
     @property
     def count(self):
         self.assert_range()
         return self.max - self.min + 1
 
-    def range_as_str(self):
+    def range_as_str(self, converter: Callable[[int], str] = u_hex):
         self.assert_range()
+        min = converter(self.min)
         if self.min == self.max:
-            return u_hex(self.min)
-        return f'{u_hex(self.min)}..{u_hex(self.max)}'
+            return min
+        max = converter(self.max)
+        if min == max:
+            return min
+        return f'{min}..{max}'
 
     def to_str(self, separator: str = ';'):
         return separator.join((self.range_as_str(), str(self.value)))
 
     def __str__(self):
         return self.to_str()
 
@@ -264,26 +272,22 @@
         return self.missing_value(code)
 
     def filter(self, pred: Callable[[Any],
                                     bool]) -> Iterable[UnicodeDataEntry]:
         """Returns an `Iterable` of `UnicodeDataEntry` for the given `pred`."""
         return (entry for entry in self if pred(entry.value))
 
-    def codes_for(self, pred: Callable[[Any], bool]) -> Iterable[int]:
-        """Returns an `Iterable` of Unicode code points for the given `pred`."""
-        return itertools.chain(*(e.range() for e in self.filter(pred)))
-
     def add_to_set(self, pred: Callable[[Any], bool], set: set) -> None:
         """Add values `pred` returns `True` to `set[int]`."""
-        for code in self.codes_for(pred):
+        for code in UnicodeDataEntry.to_codes(self.filter(pred)):
             set.add(code)
 
     def remove_from_set(self, pred: Callable[[Any], bool], set: set) -> None:
         """Remove values `pred` returns `True` from `set[int]`."""
-        for code in self.codes_for(pred):
+        for code in UnicodeDataEntry.to_codes(self.filter(pred)):
             set.discard(code)
 
     def to_set(self, pred: Callable[[Any], bool]) -> set:
         """Returns a `set[int]` of values `pred` returns `True`."""
         s = set()
         self.add_to_set(pred, s)
         return s
```

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/general_category.py` & `unicodedata_reader-1.3.4/unicodedata_reader/general_category.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/line_break.py` & `unicodedata_reader-1.3.4/unicodedata_reader/line_break.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/reader.py` & `unicodedata_reader-1.3.4/unicodedata_reader/reader.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/set.py` & `unicodedata_reader-1.3.4/unicodedata_reader/set.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-1.3.4/unicodedata_reader/vertical_orientation.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.3/PKG-INFO` & `unicodedata_reader-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 1.3.3
+Version: 1.3.4
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

