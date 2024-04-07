# Comparing `tmp/unicodedata_reader-1.2.0.tar.gz` & `tmp/unicodedata_reader-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicodedata_reader-1.2.0.tar", max compression
+gzip compressed data, was "unicodedata_reader-1.3.0.tar", max compression
```

## Comparing `unicodedata_reader-1.2.0.tar` & `unicodedata_reader-1.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/LICENSE
--rw-r--r--   0        0        0     3120 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/README.md
--rw-r--r--   0        0        0      678 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      107 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/__init__.py
--rw-r--r--   0        0        0     1101 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/__main__.py
--rwxr-xr-x   0        0        0     1310 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/bidi_brackets.py
--rw-r--r--   0        0        0     4829 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/cli.py
--rwxr-xr-x   0        0        0     4360 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/compressor.py
--rw-r--r--   0        0        0      982 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/east_asian_width.py
--rwxr-xr-x   0        0        0     1220 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/emoji.py
--rw-r--r--   0        0        0    13464 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/entry.py
--rwxr-xr-x   0        0        0      558 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/general_category.py
--rwxr-xr-x   0        0        0      671 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/line_break.py
--rw-r--r--   0        0        0     4537 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/reader.py
--rw-r--r--   0        0        0     2255 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/set.py
--rwxr-xr-x   0        0        0      996 2024-04-06 21:24:14.719304 unicodedata_reader-1.2.0/unicodedata_reader/vertical_orientation.py
--rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3120 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/README.md
+-rw-r--r--   0        0        0      648 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      107 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/__init__.py
+-rw-r--r--   0        0        0     1101 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/__main__.py
+-rwxr-xr-x   0        0        0     1310 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/bidi_brackets.py
+-rw-r--r--   0        0        0     4829 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/cli.py
+-rwxr-xr-x   0        0        0     4360 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/compressor.py
+-rw-r--r--   0        0        0      982 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/east_asian_width.py
+-rwxr-xr-x   0        0        0     1220 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/emoji.py
+-rw-r--r--   0        0        0    14674 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/entry.py
+-rwxr-xr-x   0        0        0      558 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/general_category.py
+-rwxr-xr-x   0        0        0      671 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/line_break.py
+-rw-r--r--   0        0        0     4537 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/reader.py
+-rw-r--r--   0        0        0     2160 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/set.py
+-rwxr-xr-x   0        0        0      996 2024-04-07 07:32:47.616115 unicodedata_reader-1.3.0/unicodedata_reader/vertical_orientation.py
+-rw-r--r--   0        0        0     3864 1970-01-01 00:00:00.000000 unicodedata_reader-1.3.0/PKG-INFO
```

### Comparing `unicodedata_reader-1.2.0/LICENSE` & `unicodedata_reader-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/README.md` & `unicodedata_reader-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/pyproject.toml` & `unicodedata_reader-1.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "unicodedata-reader"
-version = "1.2.0"
+version = "1.3.0"
 description = ""
 authors = ["Koji Ishii <kojii@chromium.org>"]
 readme = "README.md"
 repository = "https://github.com/kojiishi/unicodedata-reader"
 license = "Apache-2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 platformdirs = ">=2.2,<5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
-pytype = {version = "*", python = "<3.10"}
+pytype = "*"
 tox = "^4.14.2"
 yapf = "^0.40.2"
 
 [tool.poetry.scripts]
 unicodedata-reader = 'unicodedata_reader.__main__:main'
 
 [tool.pytest.ini_options]
```

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/__main__.py` & `unicodedata_reader-1.3.0/unicodedata_reader/__main__.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/bidi_brackets.py` & `unicodedata_reader-1.3.0/unicodedata_reader/bidi_brackets.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/cli.py` & `unicodedata_reader-1.3.0/unicodedata_reader/cli.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/compressor.py` & `unicodedata_reader-1.3.0/unicodedata_reader/compressor.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/east_asian_width.py` & `unicodedata_reader-1.3.0/unicodedata_reader/east_asian_width.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/emoji.py` & `unicodedata_reader-1.3.0/unicodedata_reader/emoji.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/entry.py` & `unicodedata_reader-1.3.0/unicodedata_reader/entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import enum
 import itertools
 import logging
 import re
 import types
 from typing import Any
+from typing import Callable
 from typing import Dict
 from typing import Iterable
 from typing import List
 from typing import Optional
 from typing import Sequence
+from typing import Set
 from typing import Union
 from typing import Tuple
 
 _logger = logging.getLogger('UnicodeDataEntry')
 
 
 def u_hex(value):
@@ -255,14 +257,40 @@
         for entry in self._entries:
             if code < entry.min:
                 return self.missing_value(code)
             if code <= entry.max:
                 return entry.value
         return self.missing_value(code)
 
+    def filter(self, pred: Callable[[Any],
+                                    bool]) -> Iterable[UnicodeDataEntry]:
+        """Returns an `Iterable` of `UnicodeDataEntry` for the given `pred`."""
+        return (entry for entry in self if pred(entry.value))
+
+    def codes_for(self, pred: Callable[[Any], bool]) -> Iterable[int]:
+        """Returns an `Iterable` of Unicode code points for the given `pred`."""
+        return itertools.chain(*(e.range() for e in self.filter(pred)))
+
+    def add_to_set(self, pred: Callable[[Any], bool], set: Set[int]) -> None:
+        """Add values `pred` returns `True` to `set[int]`."""
+        for code in self.codes_for(pred):
+            set.add(code)
+
+    def remove_from_set(self, pred: Callable[[Any], bool],
+                        set: Set[int]) -> None:
+        """Remove values `pred` returns `True` from `set[int]`."""
+        for code in self.codes_for(pred):
+            set.discard(code)
+
+    def to_set(self, pred: Callable[[Any], bool]) -> Set[int]:
+        """Returns a `set[int]` of values `pred` returns `True`."""
+        s = set()  # type: set[int]
+        self.add_to_set(pred, s)
+        return s
+
     def values_for_code(self) -> Iterable[Any]:
         """Returns a list of values whose index is the Unicode code point.
 
         The list includes missing values,
         so that `tuple(values_for_code())[code]` is equal to `value(code)`.
         """
         self._ensure_multi_iterable()
```

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/general_category.py` & `unicodedata_reader-1.3.0/unicodedata_reader/general_category.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/line_break.py` & `unicodedata_reader-1.3.0/unicodedata_reader/line_break.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/reader.py` & `unicodedata_reader-1.3.0/unicodedata_reader/reader.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/set.py` & `unicodedata_reader-1.3.0/unicodedata_reader/set.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from typing import Any
 from typing import Callable
 from typing import Iterable
+from typing import Set
 
 from unicodedata_reader.entry import *
 from unicodedata_reader.reader import *
 
 
 class Set(object):
-    """A simple set of Unicode code points."""
+    """A simple wrapper of a `set` of Unicode code points."""
 
-    def __init__(self) -> None:
-        self.set = set()  # type: set[int]
+    def __init__(self,
+                 entries: UnicodeDataEntries = None,
+                 pred: Callable[[Any], bool] = None) -> None:
+        self.set = set()  # type: Set[int]
+        if entries:
+            self.add_entries(entries, pred)
 
     def __contains__(self, code_point: int) -> bool:
         return code_point in self.set
 
     def __iter__(self) -> Iterable[int]:
         return self.set.__iter__()
 
@@ -34,44 +39,32 @@
         self.set.add(code)
 
     def remove(self, code: int) -> None:
         self.set.discard(code)
 
     def add_entries(self, entries: UnicodeDataEntries, pred: Callable[[Any],
                                                                       bool]):
-        for entry in entries:
-            if pred(entry.value):
-                for code in entry.range():
-                    self.set.add(code)
+        entries.add_to_set(pred, self.set)
 
     @staticmethod
     def east_asian_width(
             value: str,
             reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
-        set = Set()
-        set.add_entries(reader.east_asian_width(), lambda v: v == value)
-        return set
+        return Set(reader.east_asian_width(), lambda v: v == value)
 
     @staticmethod
     def general_category(
             value: str,
             reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
-        set = Set()
-        set.add_entries(reader.general_category(),
-                        lambda v: v.startswith(value))
-        return set
+        return Set(reader.general_category(), lambda v: v.startswith(value))
 
     @staticmethod
     def scripts(
             value: str,
             reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
-        set = Set()
-        set.add_entries(reader.scripts(), lambda v: v == value)
-        return set
+        return Set(reader.scripts(), lambda v: v == value)
 
     @staticmethod
     def script_extensions(
             value: str,
             reader: UnicodeDataReader = UnicodeDataReader.default) -> 'Set':
-        set = Set()
-        set.add_entries(reader.script_extensions(), lambda v: value in v)
-        return set
+        return Set(reader.script_extensions(), lambda v: value in v)
```

### Comparing `unicodedata_reader-1.2.0/unicodedata_reader/vertical_orientation.py` & `unicodedata_reader-1.3.0/unicodedata_reader/vertical_orientation.py`

 * *Files identical despite different names*

### Comparing `unicodedata_reader-1.2.0/PKG-INFO` & `unicodedata_reader-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicodedata-reader
-Version: 1.2.0
+Version: 1.3.0
 Summary: 
 Home-page: https://github.com/kojiishi/unicodedata-reader
 License: Apache-2.0
 Author: Koji Ishii
 Author-email: kojii@chromium.org
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
```

