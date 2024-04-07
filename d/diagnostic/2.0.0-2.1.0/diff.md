# Comparing `tmp/diagnostic-2.0.0.tar.gz` & `tmp/diagnostic-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagnostic-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "diagnostic-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `diagnostic-2.0.0.tar` & `diagnostic-2.1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1080 2023-07-28 11:21:27.518573 diagnostic-2.0.0/LICENSE
--rw-r--r--   0        0        0      911 2023-07-30 12:59:54.451840 diagnostic-2.0.0/README.md
--rw-r--r--   0        0        0     1235 2023-09-10 16:21:37.915275 diagnostic-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      288 2023-09-10 16:33:10.407798 diagnostic-2.0.0/src/diagnostic/__init__.py
--rw-r--r--   0        0        0     8860 2023-09-10 16:21:37.916175 diagnostic-2.0.0/src/diagnostic/_base.py
--rw-r--r--   0        0        0     7424 2023-09-10 16:21:37.916606 diagnostic-2.0.0/src/diagnostic/_check_docs.py
--rw-r--r--   0        0        0     1110 2023-07-30 12:59:54.459211 diagnostic-2.0.0/src/diagnostic/_concrete.py
--rw-r--r--   0        0        0     7215 2023-09-10 16:21:37.917046 diagnostic-2.0.0/src/diagnostic/_parsers.py
--rw-r--r--   0        0        0      174 2023-09-10 15:26:24.566415 diagnostic-2.0.0/src/diagnostic/check-docs.py
--rw-r--r--   0        0        0        0 2023-09-10 16:21:37.917092 diagnostic-2.0.0/src/diagnostic/py.typed
--rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 diagnostic-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-07-28 11:21:27.518573 diagnostic-2.1.0/LICENSE
+-rw-r--r--   0        0        0      911 2023-07-30 12:59:54.451840 diagnostic-2.1.0/README.md
+-rw-r--r--   0        0        0     1235 2023-09-10 16:21:37.915275 diagnostic-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      288 2024-04-07 17:37:48.478937 diagnostic-2.1.0/src/diagnostic/__init__.py
+-rw-r--r--   0        0        0     8860 2023-09-10 16:21:37.916175 diagnostic-2.1.0/src/diagnostic/_base.py
+-rw-r--r--   0        0        0     7479 2023-09-23 09:00:55.459453 diagnostic-2.1.0/src/diagnostic/_check_docs.py
+-rw-r--r--   0        0        0     1110 2023-07-30 12:59:54.459211 diagnostic-2.1.0/src/diagnostic/_concrete.py
+-rw-r--r--   0        0        0     7215 2024-04-07 17:10:16.569491 diagnostic-2.1.0/src/diagnostic/_parsers.py
+-rw-r--r--   0        0        0      174 2023-09-10 15:26:24.566415 diagnostic-2.1.0/src/diagnostic/check-docs.py
+-rw-r--r--   0        0        0        0 2023-09-10 16:21:37.917092 diagnostic-2.1.0/src/diagnostic/py.typed
+-rw-r--r--   0        0        0     1967 1970-01-01 00:00:00.000000 diagnostic-2.1.0/PKG-INFO
```

### Comparing `diagnostic-2.0.0/LICENSE` & `diagnostic-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `diagnostic-2.0.0/README.md` & `diagnostic-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `diagnostic-2.0.0/pyproject.toml` & `diagnostic-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `diagnostic-2.0.0/src/diagnostic/_base.py` & `diagnostic-2.1.0/src/diagnostic/_base.py`

 * *Files identical despite different names*

### Comparing `diagnostic-2.0.0/src/diagnostic/_check_docs.py` & `diagnostic-2.1.0/src/diagnostic/_check_docs.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 import argparse
 import sys
 from pathlib import Path
 from typing import Any, Callable, Iterable, Sequence, TypeVar
 
 import rich
+import rich.text
 import rich.traceback
 from rich.markup import escape
 
 from . import DiagnosticError
 from ._parsers import find_code_headings_in_document, find_codes_in_sources
 
 rich.traceback.install(show_locals=True)
@@ -91,15 +92,15 @@
         _format_to_lines(
             extra_codes,
             doc_codes,
             kind="extra",
             fallback_filename=str(docs_index),
         ),
     ]
-    causes = list(filter(None, sections))
+    causes = [rich.text.Text.from_markup(lines) for lines in sections if lines]
 
     if undocumented_codes and extra_codes:
         code = "undocumented-and-extra-codes"
         message = "Found undocumented and extra codes!"
     elif undocumented_codes:
         code = "undocumented-codes"
         message = "Found undocumented codes!"
```

### Comparing `diagnostic-2.0.0/src/diagnostic/_concrete.py` & `diagnostic-2.1.0/src/diagnostic/_concrete.py`

 * *Files identical despite different names*

### Comparing `diagnostic-2.0.0/src/diagnostic/_parsers.py` & `diagnostic-2.1.0/src/diagnostic/_parsers.py`

 * *Files identical despite different names*

### Comparing `diagnostic-2.0.0/PKG-INFO` & `diagnostic-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagnostic
-Version: 2.0.0
+Version: 2.1.0
 Summary: Present errors that contain causes better understand what happened.
 Author-email: Pradyun Gedam <mail@pradyunsg.me>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

