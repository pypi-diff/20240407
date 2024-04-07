# Comparing `tmp/notional-0.8.0.tar.gz` & `tmp/notional-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notional-0.8.0.tar", max compression
+gzip compressed data, was "notional-0.8.1.tar", max compression
```

## Comparing `notional-0.8.0.tar` & `notional-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1071 2021-09-20 19:35:00.000000 notional-0.8.0/LICENSE
--rw-r--r--   0        0        0     2357 2023-01-05 14:29:43.601551 notional-0.8.0/README.md
--rw-r--r--   0        0        0     1017 2023-03-29 12:56:53.385450 notional-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      368 2023-03-18 01:40:46.522873 notional-0.8.0/src/notional/__init__.py
--rw-r--r--   0        0        0      294 2023-03-17 13:04:42.774343 notional-0.8.0/src/notional/__main__.py
--rw-r--r--   0        0        0    22382 2023-03-29 12:56:53.385768 notional-0.8.0/src/notional/blocks.py
--rw-r--r--   0        0        0     9915 2023-01-16 16:50:53.239668 notional-0.8.0/src/notional/core.py
--rw-r--r--   0        0        0     4844 2023-01-03 22:37:30.143172 notional-0.8.0/src/notional/iterator.py
--rw-r--r--   0        0        0    13489 2023-01-16 16:51:01.327922 notional-0.8.0/src/notional/orm.py
--rw-r--r--   0        0        0    18556 2023-02-02 03:53:57.054782 notional-0.8.0/src/notional/parser.py
--rw-r--r--   0        0        0    10053 2023-02-02 03:53:57.055203 notional-0.8.0/src/notional/query.py
--rw-r--r--   0        0        0     7266 2022-12-31 15:49:40.747142 notional-0.8.0/src/notional/schema.py
--rw-r--r--   0        0        0    17950 2023-03-18 01:40:46.523290 notional-0.8.0/src/notional/session.py
--rw-r--r--   0        0        0     9682 2023-02-04 02:33:49.661287 notional-0.8.0/src/notional/text.py
--rw-r--r--   0        0        0    30793 2023-02-02 03:53:57.056928 notional-0.8.0/src/notional/types.py
--rw-r--r--   0        0        0     1374 2022-12-31 15:49:40.748917 notional-0.8.0/src/notional/user.py
--rw-r--r--   0        0        0     1299 2023-02-02 03:53:57.057536 notional-0.8.0/src/notional/util.py
--rw-r--r--   0        0        0     1697 2023-03-19 04:03:23.147593 notional-0.8.0/src/notional/version.py
--rw-r--r--   0        0        0     3266 1970-01-01 00:00:00.000000 notional-0.8.0/setup.py
--rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 notional-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-09-20 19:35:00.000000 notional-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2357 2023-01-05 14:29:43.601551 notional-0.8.1/README.md
+-rw-r--r--   0        0        0     1559 2024-04-07 02:00:02.886877 notional-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      368 2023-08-02 03:16:34.247660 notional-0.8.1/src/notional/__init__.py
+-rw-r--r--   0        0        0      294 2023-03-17 13:04:42.774343 notional-0.8.1/src/notional/__main__.py
+-rw-r--r--   0        0        0    22381 2024-04-07 01:59:59.936119 notional-0.8.1/src/notional/blocks.py
+-rw-r--r--   0        0        0     9915 2024-04-07 01:59:59.936964 notional-0.8.1/src/notional/core.py
+-rw-r--r--   0        0        0     4844 2024-04-07 01:59:59.937794 notional-0.8.1/src/notional/iterator.py
+-rw-r--r--   0        0        0    13452 2024-04-07 01:59:59.938521 notional-0.8.1/src/notional/orm.py
+-rw-r--r--   0        0        0    18566 2023-12-27 15:42:54.107393 notional-0.8.1/src/notional/parser.py
+-rw-r--r--   0        0        0    10053 2024-04-07 01:59:59.939658 notional-0.8.1/src/notional/query.py
+-rw-r--r--   0        0        0     7943 2024-04-07 01:59:59.940353 notional-0.8.1/src/notional/schema.py
+-rw-r--r--   0        0        0    17930 2024-04-07 01:59:59.941235 notional-0.8.1/src/notional/session.py
+-rw-r--r--   0        0        0     9580 2024-04-07 02:00:02.887260 notional-0.8.1/src/notional/text.py
+-rw-r--r--   0        0        0    30793 2024-04-07 01:59:59.942819 notional-0.8.1/src/notional/types.py
+-rw-r--r--   0        0        0     1374 2024-04-07 01:59:59.943721 notional-0.8.1/src/notional/user.py
+-rw-r--r--   0        0        0     1299 2024-04-07 01:59:59.944620 notional-0.8.1/src/notional/util.py
+-rw-r--r--   0        0        0     1697 2023-03-19 04:03:23.147593 notional-0.8.1/src/notional/version.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 notional-0.8.1/PKG-INFO
```

### Comparing `notional-0.8.0/LICENSE` & `notional-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/README.md` & `notional-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/src/notional/blocks.py` & `notional-0.8.1/src/notional/blocks.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 class TextBlock(Block, ABC):
     """A standard text block object in Notion."""
 
     # text blocks have a nested object with 'type' name and a 'rich_text' child
 
     @property
     def __text__(self):
-        """Provide short-hand access to the nested text content in this block."""
+        """Provide shorthand access to the nested text content in this block."""
 
         return self("rich_text")
 
     @classmethod
     def __compose__(cls, *text):
         """Compose a `TextBlock` from the given text items."""
```

### Comparing `notional-0.8.0/src/notional/core.py` & `notional-0.8.1/src/notional/core.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/src/notional/iterator.py` & `notional-0.8.1/src/notional/iterator.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/src/notional/orm.py` & `notional-0.8.1/src/notional/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 There are two primary constructs in this module that enable custom type definitions
 in Notional: `Property()` and `connected_page()`.
 """
 
 import logging
 from typing import Union
 
-from emoji import emojize
+from emoji import emojize, is_emoji
 
 from .blocks import Page
 from .schema import PropertyObject, RichText
-from .text import is_emoji, make_safe_python_name
+from .text import make_safe_python_name
 from .types import DatabaseRef, EmojiObject, ExternalFile, PropertyValue
 
 logger = logging.getLogger(__name__)
 
 
 class ConnectedProperty:
     """Contains the information and methods needed for a connected property.
@@ -77,17 +77,17 @@
 
         # TODO raise instead?
         if self.page_data is None:
             return None
 
         try:
             prop = self.page_data[self.name]
-        except AttributeError:
+        except AttributeError as err:
             if self.default == ...:
-                raise AttributeError(f"Missing property: {self.name}")
+                raise err
             return self.default
 
         if not isinstance(prop, self.value_type):
             raise TypeError("Type mismatch")
 
         if hasattr(prop, "Value"):
             return prop.Value
@@ -404,15 +404,15 @@
     :param source_db: if provided, the returned class will use the ID and schema of
       this object to initialize the connected page
 
     :param schema: if provided, the returned class will contain properties according
       to the schema provided; defaults to `None`
 
     :param cls: the returned class will inherit from the given class, which must be a
-      sublass of `ConnectedPage`; defaults to `ConnectedPage`
+      subclass of `ConnectedPage`; defaults to `ConnectedPage`
     """
 
     if cls is None:
         cls = ConnectedPage
 
     elif not issubclass(cls, ConnectedPage):
         raise ValueError("'cls' must subclass ConnectedPage")
```

### Comparing `notional-0.8.0/src/notional/parser.py` & `notional-0.8.1/src/notional/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 
     def _process(self, reader):
         # build the schema based on the first row
 
         try:
             header = next(reader)
         except StopIteration:
-            raise ValueError("Invalid CSV: empty data")
+            raise ValueError("Invalid CSV: empty data") from None
 
         if self._has_header:
             self._build_schema(*header)
 
         else:
             cols = [str(num) for num in range(len(header))]
             self._build_schema(*cols)
```

### Comparing `notional-0.8.0/src/notional/query.py` & `notional-0.8.1/src/notional/query.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/src/notional/schema.py` & `notional-0.8.1/src/notional/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,51 @@
 """Objects representing a database schema."""
 
 from enum import Enum
 from typing import Any, List, Optional
 from uuid import UUID
 
+import pydantic
+
 from .core import GenericObject, TypedObject
 from .text import Color
 
 
 class Function(str, Enum):
     """Standard aggregation functions."""
 
-    COUNT_ALL = "count_all"
+    COUNT = "count"
     COUNT_VALUES = "count_values"
-    COUNT_UNIQUE_VALUES = "count_unique_values"
-    COUNT_EMPTY = "count_empty"
-    COUNT_NOT_EMPTY = "count_not_empty"
+    COUNT_PER_GROUP = "count_per_group"
+
+    EMPTY = "empty"
+    NOT_EMPTY = "not_empty"
+
+    CHECKED = "checked"
+    UNCHECKED = "unchecked"
 
     PERCENT_EMPTY = "percent_empty"
     PERCENT_NOT_EMPTY = "percent_not_empty"
+    PERCENT_CHECKED = "percent_checked"
+    PERCENT_PER_GROUP = "percent_per_group"
 
     AVERAGE = "average"
     MIN = "min"
     MAX = "max"
     MEDIAN = "median"
     RANGE = "range"
     SUM = "sum"
 
+    DATE_RANGE = "date_range"
     EARLIEST_DATE = "earliest_date"
     LATEST_DATE = "latest_date"
 
     SHOW_ORIGINAL = "show_original"
+    SHOW_UNIQUE = "show_unique"
+    UNIQUE = "unique"
 
 
 class NumberFormat(str, Enum):
     """Available number formats in Notion."""
 
     NUMBER = "number"
     NUMBER_WITH_COMMAS = "number_with_commas"
@@ -97,14 +108,20 @@
 
 class Number(PropertyObject, type="number"):
     """Defines the number configuration for a database property."""
 
     class _NestedData(GenericObject):
         format: NumberFormat = NumberFormat.NUMBER
 
+        # leads to better error messages, see
+        # https://github.com/pydantic/pydantic/issues/355
+        @pydantic.validator("format", pre=True)
+        def validate_enum_field(cls, field: str):
+            return NumberFormat(field)
+
     number: _NestedData = _NestedData()
 
     @classmethod
     def __compose__(cls, format):
         """Create a `Number` object with the expected format."""
         return cls(number=cls._NestedData(format=format))
 
@@ -239,22 +256,28 @@
     relation: PropertyRelation = PropertyRelation()
 
 
 class Rollup(PropertyObject, type="rollup"):
     """Defines the rollup configuration for a database property."""
 
     class _NestedData(GenericObject):
-        function: Function = Function.COUNT_ALL
+        function: Function = Function.COUNT
 
         relation_property_name: Optional[str] = None
         relation_property_id: Optional[str] = None
 
         rollup_property_name: Optional[str] = None
         rollup_property_id: Optional[str] = None
 
+        # leads to better error messages, see
+        # https://github.com/pydantic/pydantic/issues/355
+        @pydantic.validator("function", pre=True)
+        def validate_enum_field(cls, field: str):
+            return Function(field)
+
     rollup: _NestedData = _NestedData()
 
 
 class CreatedTime(PropertyObject, type="created_time"):
     """Defines the created-time configuration for a database property."""
 
     created_time: Any = {}
```

### Comparing `notional-0.8.0/src/notional/session.py` & `notional-0.8.1/src/notional/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     """Raised when there are issues with the Notion session."""
 
     def __init__(self, message):
         """Initialize the `SessionError` with a supplied message.."""
         super().__init__(message)
 
 
-class Session(object):
+class Session:
     """An active session with the Notion SDK."""
 
     def __init__(self, **kwargs):
         """Initialize the `Session` object and the endpoints.
 
         `kwargs` will be passed direction to the Notion SDK Client.  For more details,
         see the (full docs)[https://ramnes.github.io/notion-sdk-py/reference/client/].
@@ -93,15 +93,15 @@
 
         if error is not None:
             raise SessionError(error)
 
         return True
 
 
-class Endpoint(object):
+class Endpoint:
     """Notional wrapper for the API endpoints."""
 
     def __init__(self, session: Session):
         """Initialize the `Endpoint` for the supplied session."""
         self.session = session
 
 
@@ -370,15 +370,15 @@
 
         def __call__(self):
             """Return the underlying endpoint in the Notion SDK."""
             return self.session.client.pages.properties
 
         # https://developers.notion.com/reference/retrieve-a-page-property
         def retrieve(self, page_id, property_id):
-            """Return the Property on a specific page Page with the given ID."""
+            """Return the Property on a specific Page with the given ID."""
 
             logger.info("Retrieving property :: %s [%s]", property_id, page_id)
 
             data = self().retrieve(page_id, property_id)
 
             # TODO should PropertyListItem return an iterator instead?
             return parse_obj_as(Union[PropertyItem, PropertyItemList], obj=data)
@@ -492,15 +492,15 @@
         }
 
         data = self().update(page.id.hex, properties=props)
 
         return page.refresh(**data)
 
     def set(self, page, cover=False, icon=False, archived=None):
-        """Set specific page attributes (such as cover, icon, etc) on the server.
+        """Set specific page attributes (such as cover, icon, etc.) on the server.
 
         `page` may be any suitable `PageRef` type.
 
         To remove an attribute, set its value to None.
         """
 
         page_id = PageRef[page].page_id
```

### Comparing `notional-0.8.0/src/notional/text.py` & `notional-0.8.1/src/notional/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 """Utilities for working text, markdown & Rich Text in Notion."""
 
 import re
 from copy import deepcopy
 from enum import Enum
 from typing import Optional
 
-from emoji import EMOJI_DATA
-
 from .core import GenericObject, TypedObject
 
 # this might be a place to capture other utilities for working with markdown, text
 # rich text, etc...  the challenge is not importing types due to a circular ref.
 
 
 # the max text size according to the Notion API is 2000 characters...
@@ -45,19 +43,14 @@
 
 
 def markdown(*rtf):
     """Return text as markdown from the list of RichText objects."""
     return "".join(str(text) for text in rtf if text)
 
 
-def is_emoji(text):
-    """Check if text is a single emoji."""
-    return text in EMOJI_DATA
-
-
 def chunky(text, length=MAX_TEXT_OBJECT_SIZE):
     """Break the given `text` into chunks of at most `length` size."""
     return (text[idx : idx + length] for idx in range(0, len(text), length))
 
 
 def text_blocks(text: str):
     """Convert the given plain text into an array of TextObject's.
@@ -243,19 +236,19 @@
         elif self.plain_text is None or len(self.plain_text) == 0:
             text = f"({self.href})"
         else:
             text = f"[{self.plain_text}]({self.href})"
 
         if self.annotations:
             if self.annotations.bold:
-                text = f"*{text}*"
-            if self.annotations.italic:
                 text = f"**{text}**"
+            if self.annotations.italic:
+                text = f"*{text}*"
             if self.annotations.underline:
-                text = f"_{text}_"
+                text = f"<u>{text}</u>"
             if self.annotations.strikethrough:
                 text = f"~{text}~"
             if self.annotations.code:
                 text = f"`{text}`"
 
         return text
 
@@ -375,14 +368,15 @@
     SASS = "sass"
     SCALA = "scala"
     SCHEME = "scheme"
     SCSS = "scss"
     SHELL = "shell"
     SQL = "sql"
     SWIFT = "swift"
+    TOML = "toml"
     TYPESCRIPT = "typescript"
     VB_NET = "vb.net"
     VERILOG = "verilog"
     VHDL = "vhdl"
     VISUAL_BASIC = "visual basic"
     WEBASSEMBLY = "webassembly"
     XML = "xml"
```

### Comparing `notional-0.8.0/src/notional/types.py` & `notional-0.8.1/src/notional/types.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/src/notional/user.py` & `notional-0.8.1/src/notional/user.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/src/notional/util.py` & `notional-0.8.1/src/notional/util.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/src/notional/version.py` & `notional-0.8.1/src/notional/version.py`

 * *Files identical despite different names*

### Comparing `notional-0.8.0/PKG-INFO` & `notional-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: notional
-Version: 0.8.0
+Version: 0.8.1
 Summary: A high-level interface for the Notion SDK.
 Home-page: https://github.com/jheddings/notional/
 License: MIT
 Author: Jason Heddings
 Author-email: jheddings@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: emoji (>=2.2.0,<3.0.0)
+Requires-Dist: emoji (>=2.11.0,<3.0.0)
 Requires-Dist: html5lib (>=1.1,<2.0)
-Requires-Dist: notion-client (>=2.0.0,<3.0.0)
-Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
+Requires-Dist: notion-client (>=2.2.1,<3.0.0)
+Requires-Dist: pydantic (>=1.10.15,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Project-URL: Documentation, https://jheddings.github.io/notional/
 Project-URL: Repository, https://github.com/jheddings/notional/
 Description-Content-Type: text/markdown
 
 # notional #
 
 [![PyPI](https://img.shields.io/pypi/v/notional.svg)](https://pypi.org/project/notional)
```

