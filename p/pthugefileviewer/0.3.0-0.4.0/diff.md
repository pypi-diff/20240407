# Comparing `tmp/pthugefileviewer-0.3.0.tar.gz` & `tmp/pthugefileviewer-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pthugefileviewer-0.3.0.tar", last modified: Sat Apr  6 19:32:55 2024, max compression
+gzip compressed data, was "pthugefileviewer-0.4.0.tar", last modified: Sun Apr  7 21:32:45 2024, max compression
```

## Comparing `pthugefileviewer-0.3.0.tar` & `pthugefileviewer-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:32:55.059162 pthugefileviewer-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-06 19:32:55.059162 pthugefileviewer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:32:55.059162 pthugefileviewer-0.3.0/pthugefileviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-06 19:32:55.000000 pthugefileviewer-0.3.0/pthugefileviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-06 19:32:55.000000 pthugefileviewer-0.3.0/pthugefileviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:32:55.000000 pthugefileviewer-0.3.0/pthugefileviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 19:32:55.000000 pthugefileviewer-0.3.0/pthugefileviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 19:32:55.000000 pthugefileviewer-0.3.0/pthugefileviewer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-06 19:32:55.059162 pthugefileviewer-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:32:55.055162 pthugefileviewer-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:32:55.055162 pthugefileviewer-0.3.0/src/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     8456 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/src/bin/hfv-regexbuild
--rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/src/bin/hfv-view
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:32:55.055162 pthugefileviewer-0.3.0/src/pthugefileviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/src/pthugefileviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/src/pthugefileviewer/hugefilevieweruicontrol.py
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/src/pthugefileviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:32:55.059162 pthugefileviewer-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-06 19:32:48.000000 pthugefileviewer-0.3.0/tests/test_hfv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 21:32:45.000000 pthugefileviewer-0.4.0/pthugefileviewer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.833603 pthugefileviewer-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.833603 pthugefileviewer-0.4.0/src/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9968 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/bin/hfv-regexbuild
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1895 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/bin/hfv-view
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/src/pthugefileviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/pthugefileviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6411 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/pthugefileviewer/hugefilevieweruicontrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/src/pthugefileviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:32:45.837603 pthugefileviewer-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7341 2024-04-07 21:32:38.000000 pthugefileviewer-0.4.0/tests/test_hfv.py
```

### Comparing `pthugefileviewer-0.3.0/LICENSE` & `pthugefileviewer-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.3.0/PKG-INFO` & `pthugefileviewer-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.3.0
+Version: 0.4.0
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.3.0/README.md` & `pthugefileviewer-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.3.0/pthugefileviewer.egg-info/PKG-INFO` & `pthugefileviewer-0.4.0/pthugefileviewer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pthugefileviewer
-Version: 0.3.0
+Version: 0.4.0
 Summary: Huge file viewer control for prompt-toolkit
 Home-page: http://github.com/lpenz/pthugefileviewer
 Author: "Leandro Lisboa Penz"
 Author-email: "lpenz@lpenz.org"
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

### Comparing `pthugefileviewer-0.3.0/setup.cfg` & `pthugefileviewer-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pthugefileviewer
-version = 0.3.0
+version = 0.4.0
 description = Huge file viewer control for prompt-toolkit
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = "Leandro Lisboa Penz"
 author_email = "lpenz@lpenz.org"
```

### Comparing `pthugefileviewer-0.3.0/src/bin/hfv-regexbuild` & `pthugefileviewer-0.4.0/src/bin/hfv-regexbuild`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python3
 """
 A console regular expression builder
 """
 
 import argparse
+import itertools
 import os
 import re
 from typing import Optional
 
 import pthugefileviewer
 from prompt_toolkit import Application
 from prompt_toolkit.application import get_app
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.document import Document
 from prompt_toolkit.formatted_text import StyleAndTextTuples
 from prompt_toolkit.key_binding import KeyBindings
 from prompt_toolkit.key_binding.bindings.focus import focus_next
 from prompt_toolkit.key_binding.key_processor import KeyPressEvent
 from prompt_toolkit.layout.containers import Container, HSplit, Window
-from prompt_toolkit.layout.controls import BufferControl
+from prompt_toolkit.layout.controls import BufferControl, FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.layout.processors import (
     Processor,
     Transformation,
     TransformationInput,
 )
 from prompt_toolkit.layout.utils import explode_text_fragments
@@ -136,16 +137,22 @@
             return Transformation(fragments)
         fragments = explode_text_fragments(fragments)
         fragments[pos] = ("class:regex.error", fragments[pos][1])
         return Transformation(fragments)
 
 
 class RegexWidget:
-    def __init__(self, fileview: FileviewWidget, initial_regex_str: str = ""):
+    def __init__(
+        self,
+        fileview: FileviewWidget,
+        statuswidget: "StatusWidget",
+        initial_regex_str: str = "",
+    ):
         self.fileview = fileview
+        self.statuswidget = statuswidget
         self.regex_str = initial_regex_str
         self.buffer = Buffer(
             document=Document(text=self.regex_str),
             multiline=True,
             on_text_changed=self.regex_changed,
         )
         self.control = BufferControl(
@@ -163,43 +170,82 @@
         else:
             self.frame.title = [("class:title.unfocused", "Regular expression")]
         return ""
 
     def regex_changed(self, buf: Buffer) -> None:
         try:
             regex = re.compile(bytes(buf.document.text, "utf-8"), re.S)
-        except re.error:
+        except re.error as e:
             self.fileview.control.use_regex(None)
+            self.statuswidget.error(e.msg)
             return
+        self.statuswidget.reset()
         self.fileview.control.use_regex(regex)
 
     def __pt_container__(self) -> Container:
         return self.window
 
 
+class StatusWidget:
+    def __init__(self) -> None:
+        self.default: StyleAndTextTuples = list(
+            itertools.chain.from_iterable(
+                [
+                    ("class:status.key", f"{key} "),
+                    ("class:status.descr", f"{descr}    "),
+                ]
+                for key, descr in [
+                    (" TAB", "switch panes"),
+                    ("F3", "search next"),
+                    ("^Up", ""),
+                    ("^Dn", ""),
+                    ("^PgUp", ""),
+                    ("^PgDn", ""),
+                    ("^D", "exit"),
+                ]
+            )
+        )
+        self.control = FormattedTextControl(text=self.default)
+        self.window = Window(self.control, height=1, style="class:status.ok")
+
+    def error(self, msg: str) -> None:
+        self.window.style = "class:status.error"
+        self.control.text = f" Regex error: {msg}"
+
+    def reset(self) -> None:
+        self.window.style = "class:status.ok"
+        self.control.text = self.default
+
+
 def regexbuilder_run(
     filename: os.PathLike[str], initial_regex_str: Optional[str] = None
 ) -> None:
+    statuswidget = StatusWidget()
     fileview = FileviewWidget(filename)
-    regexwidget = RegexWidget(fileview, initial_regex_str or "")
+    regexwidget = RegexWidget(fileview, statuswidget, initial_regex_str or "")
     root_container = HSplit(
         [
             fileview.frame,
             regexwidget.frame,
+            statuswidget.window,
         ]
     )
     layout = Layout(root_container)
     layout.focus(regexwidget.window)
     style = Style.from_dict(
         {
             "match": "bold fg:white bg:green",
             "oldmatch": "fg:gray bg:darkgreen",
             "title.focused": "reverse",
             "title.unfocused": "",
             "regex.error": "fg:white bg:red",
+            "status.ok": "bg:#222222",
+            "status.key": "fg:white",
+            "status.descr": "fg:gray",
+            "status.error": "bg:red fg:white bold",
         }
     )
     kb = KeyBindings()
     app: Application[None] = Application(
         layout=layout,
         key_bindings=kb,
         full_screen=True,
```

### Comparing `pthugefileviewer-0.3.0/src/bin/hfv-view` & `pthugefileviewer-0.4.0/src/bin/hfv-view`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.3.0/src/pthugefileviewer/hugefilevieweruicontrol.py` & `pthugefileviewer-0.4.0/src/pthugefileviewer/hugefilevieweruicontrol.py`

 * *Files identical despite different names*

### Comparing `pthugefileviewer-0.3.0/tests/test_hfv.py` & `pthugefileviewer-0.4.0/tests/test_hfv.py`

 * *Files identical despite different names*

