# Comparing `tmp/unicodedata_reader-1.3.2.tar.gz` & `tmp/unicodedata_reader-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata_reader-1.3.2.tar", max compression
+gzip compressed data, was "unicodedata_reader-1.3.3.tar", max compression
```

## Comparing `unicodedata_reader-1.3.2.tar` & `unicodedata_reader-1.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/LICENSE
--rw-r--r--   0        0        0     3114 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/README.md
--rw-r--r--   0        0        0      648 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4829 2024-04-07 08:15:58.653200 unicodedata_reader-1.3.2/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4360 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/compressor.py
--rw-r--r--   0        0        0      982 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/east_asian_width.py
--rwxr-xr-x   0        0        0     1220 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    14759 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      558 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      671 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     4537 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/reader.py
--rw-r--r--   0        0        0     2160 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/set.py
--rwxr-xr-x   0        0        0      996 2024-04-07 08:15:58.657200 unicodedata_reader-1.3.2/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/LICENSE
+-rw-r--r--   0        0        0     3114 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/README.md
+-rw-r--r--   0        0        0      648 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4829 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    14679 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     5090 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2019 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-07 09:50:04.348447 unicodedata_reader-1.3.3/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3858 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.3/PKG-INFO
```

### Comparing `unicodedata_reader-1.3.2/LICENSE` & `unicodedata_reader-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/README.md` & `unicodedata_reader-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/pyproject.toml` & `unicodedata_reader-1.3.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "1.3.2"
+version = "1.3.3"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
```

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/__main__.py` & `unicodedata_reader-1.3.3/unicodedata_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-1.3.3/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/cli.py` & `unicodedata_reader-1.3.3/unicodedata_reader/cli.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/compressor.py` & `unicodedata_reader-1.3.3/unicodedata_reader/compressor.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/east_asian_width.py` & `unicodedata_reader-1.3.3/unicodedata_reader/east_asian_width.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/emoji.py` & `unicodedata_reader-1.3.3/unicodedata_reader/emoji.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/entry.py` & `unicodedata_reader-1.3.3/unicodedata_reader/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
-from typing import Set
 from typing import Union
 from typing import Tuple
 
 _logger = logging.getLogger('UnicodeDataEntry')
 
 
 def u_hex(value):
@@ -269,28 +268,27 @@
         """Returns an `Iterable` of `UnicodeDataEntry` for the given `pred`."""
         return (entry for entry in self if pred(entry.value))
 
     def codes_for(self, pred: Callable[[Any], bool]) -> Iterable[int]:
         """Returns an `Iterable` of Unicode code points for the given `pred`."""
         return itertools.chain(*(e.range() for e in self.filter(pred)))
 
-    def add_to_set(self, pred: Callable[[Any], bool], set: Set[int]) -> None:
+    def add_to_set(self, pred: Callable[[Any], bool], set: set) -> None:
         """Add values `pred` returns `True` to `set[int]`."""
         for code in self.codes_for(pred):
             set.add(code)
 
-    def remove_from_set(self, pred: Callable[[Any], bool],
-                        set: Set[int]) -> None:
+    def remove_from_set(self, pred: Callable[[Any], bool], set: set) -> None:
         """Remove values `pred` returns `True` from `set[int]`."""
         for code in self.codes_for(pred):
             set.discard(code)
 
-    def to_set(self, pred: Callable[[Any], bool]) -> Set[int]:
+    def to_set(self, pred: Callable[[Any], bool]) -> set:
         """Returns a `set[int]` of values `pred` returns `True`."""
-        s = set()  # type: set[int]
+        s = set()
         self.add_to_set(pred, s)
         return s
 
     def values_for_code(self) -> Iterable[Any]:
         """Returns a list of values whose index is the Unicode code point.
 
         The list includes missing values,
```

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/general_category.py` & `unicodedata_reader-1.3.3/unicodedata_reader/general_category.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/line_break.py` & `unicodedata_reader-1.3.3/unicodedata_reader/line_break.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/reader.py` & `unicodedata_reader-1.3.3/unicodedata_reader/reader.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,14 +26,30 @@
 
     def __init__(
         self,
         url_template: str = 'https://www.unicode.org/Public/UNIDATA/{0}.txt'
     ) -> None:
         self.url_template = url_template
 
+    class Context(object):
+        """This class changes `UnicodeDataReader.default` while in the context,
+        and restores when exit."""
+
+        def __init__(self, reader: 'UnicodeDataReader') -> None:
+            self.reader = reader
+
+        def __enter__(self):
+            self.saved_default = UnicodeDataReader.default
+            UnicodeDataReader.default = self.reader
+            return self.reader
+
+        def __exit__(self, exc_type, exc_val, exc_tb):
+            UnicodeDataReader.default = self.saved_default
+            return None
+
     def bidi_brackets(self) -> UnicodeDataEntries:
         name = 'BidiBrackets'
         lines = self.read_lines(name)
         return UnicodeBidiBracketsDataEntries(name=name, lines=lines)
 
     def blocks(self) -> UnicodeDataEntries:
         name = 'Blocks'
```

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/set.py` & `unicodedata_reader-1.3.3/unicodedata_reader/set.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any
 from typing import Callable
 from typing import Iterable
-from typing import Set
+from typing import Optional
 
 from unicodedata_reader.entry import *
 from unicodedata_reader.reader import *
 
 
 class Set(object):
     """A simple wrapper of a `set` of Unicode code points."""
 
     def __init__(self,
-                 entries: UnicodeDataEntries = None,
-                 pred: Callable[[Any], bool] = None) -> None:
-        self.set = set()  # type: Set[int]
+                 entries: Optional[UnicodeDataEntries] = None,
+                 pred: Optional[Callable[[Any], bool]] = None) -> None:
+        self.set = set()
         if entries:
             self.add_entries(entries, pred)
 
     def __contains__(self, code_point: int) -> bool:
         return code_point in self.set
 
     def __iter__(self) -> Iterable[int]:
@@ -42,29 +42,25 @@
         self.set.discard(code)
 
     def add_entries(self, entries: UnicodeDataEntries, pred: Callable[[Any],
                                                                       bool]):
         entries.add_to_set(pred, self.set)
 
     @staticmethod
-    def east_asian_width(
-            value: str,
-            reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
+    def east_asian_width(value: str) -> 'Set':
+        reader = UnicodeDataReader.default
         return Set(reader.east_asian_width(), lambda v: v == value)
 
     @staticmethod
-    def general_category(
-            value: str,
-            reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
+    def general_category(value: str) -> 'Set':
+        reader = UnicodeDataReader.default
         return Set(reader.general_category(), lambda v: v.startswith(value))
 
     @staticmethod
-    def scripts(
-            value: str,
-            reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
+    def scripts(value: str) -> 'Set':
+        reader = UnicodeDataReader.default
         return Set(reader.scripts(), lambda v: v == value)
 
     @staticmethod
-    def script_extensions(
-            value: str,
-            reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
+    def script_extensions(value: str) -> 'Set':
+        reader = UnicodeDataReader.default
         return Set(reader.script_extensions(), lambda v: value in v)
```

### Comparing `unicodedata_reader-1.3.2/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-1.3.3/unicodedata_reader/vertical_orientation.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.3.2/PKG-INFO` & `unicodedata_reader-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 1.3.2
+Version: 1.3.3
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

