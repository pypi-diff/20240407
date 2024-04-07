# Comparing `tmp/tko-0.3.8.tar.gz` & `tmp/tko-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.3.8.tar", last modified: Sat Apr  6 02:09:36 2024, max compression
+gzip compressed data, was "tko-0.3.9.tar", last modified: Sun Apr  7 03:39:13 2024, max compression
```

## Comparing `tko-0.3.8.tar` & `tko-0.3.9.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 02:09:36.627798 tko-0.3.8/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.8/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.8/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-06 02:09:36.627798 tko-0.3.8/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.3.8/Readme.md
--rw-r--r--   0 lion      (1000) lion      (1000)     3245 2024-04-06 01:46:34.000000 tko-0.3.8/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.8/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-06 02:09:36.627798 tko-0.3.8/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.3.8/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 02:09:33.914465 tko-0.3.8/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 02:09:36.614465 tko-0.3.8/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-06 00:50:25.000000 tko-0.3.8/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9417 2024-04-05 15:52:20.000000 tko-0.3.8/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8001 2024-04-05 15:51:48.000000 tko-0.3.8/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.3.8/src/tko/basic.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.8/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7688 2024-04-06 01:44:59.000000 tko-0.3.8/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:50:45.000000 tko-0.3.8/src/tko/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.8/src/tko/format.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.8/src/tko/guide.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.3.8/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.8/src/tko/pattern.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.8/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.8/src/tko/settings.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3928 2024-04-06 02:07:31.000000 tko-0.3.8/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.3.8/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.3.8/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 02:09:36.624465 tko-0.3.8/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-06 02:09:33.000000 tko-0.3.8/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      554 2024-04-06 02:09:33.000000 tko-0.3.8/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-06 02:09:33.000000 tko-0.3.8/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-06 02:09:33.000000 tko-0.3.8/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-06 02:09:33.000000 tko-0.3.8/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-06 02:09:33.000000 tko-0.3.8/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:13.133334 tko-0.3.9/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.9/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.9/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-07 03:39:13.133334 tko-0.3.9/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.3.9/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     3315 2024-04-07 03:37:46.000000 tko-0.3.9/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.9/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-07 03:39:13.133334 tko-0.3.9/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.3.9/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:13.120001 tko-0.3.9/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:13.130001 tko-0.3.9/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-07 03:39:08.000000 tko-0.3.9/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9417 2024-04-05 15:52:20.000000 tko-0.3.9/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6485 2024-04-07 03:36:24.000000 tko-0.3.9/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.3.9/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.9/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7688 2024-04-06 01:44:59.000000 tko-0.3.9/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.9/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.9/src/tko/guide.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.3.9/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.9/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.9/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.9/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3928 2024-04-06 02:07:31.000000 tko-0.3.9/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.3.9/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.3.9/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:13.133334 tko-0.3.9/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-07 03:39:13.000000 tko-0.3.9/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      536 2024-04-07 03:39:13.000000 tko-0.3.9/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-07 03:39:13.000000 tko-0.3.9/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-07 03:39:13.000000 tko-0.3.9/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-07 03:39:13.000000 tko-0.3.9/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-07 03:39:13.000000 tko-0.3.9/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.3.8/LICENSE` & `tko-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/PKG-INFO` & `tko-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.8
+Version: 0.3.9
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.8/Readme.md` & `tko-0.3.9/Readme.md`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/changelog.md` & `tko-0.3.9/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+- 0.3.8
+  - fix: filter mode calling filter command from feno package
 - 0.3.7
   - fix: filter mode with empty files
   - fix: action class to poo mode
   - fix: remove auto select entry point for java and typescript
   - fix: remove download keep and required from config to use drafts only
 - 0.3.6
   - add compact mode to run
```

### Comparing `tko-0.3.8/setup.py` & `tko-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/__main__.py` & `tko-0.3.9/src/tko/__main__.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/actions.py` & `tko-0.3.9/src/tko/actions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from typing import List, Optional
 import os
 import shutil
+import subprocess
 
 from .wdir import Wdir
 from .basic import DiffMode, ExecutionResult, CompilerError, Param, Unit
 from .diff import Diff
 from .format import Colored, Color, Report, symbols
 from .writer import Writer
 from .solver import Solver
 from .runner import Runner
-from .filter import Filter
 
 
 class Execution:
 
     def __init__(self):
         pass
 
@@ -29,63 +29,25 @@
             return ExecutionResult.SUCCESS
         return ExecutionResult.WRONG_OUTPUT
 
 
 class FilterMode:
 
     @staticmethod
-    def deep_filter_copy(source, destiny):
-        if os.path.isdir(source):
-            chain = source.split(os.sep)
-            if len(chain) > 1 and chain[-1].startswith("."):
-                return
-            if not os.path.isdir(destiny):
-                os.makedirs(destiny)
-            for file in sorted(os.listdir(source)):
-                FilterMode.deep_filter_copy(os.path.join(source, file), os.path.join(destiny, file))
-        else:
-            filename = os.path.basename(source)
-            text_extensions = [".md", ".c", ".cpp", ".h", ".hpp", ".py", ".java", ".js", ".ts", ".hs"]
-
-            if not any([filename.endswith(ext) for ext in text_extensions]):
-                return
-            
-            content = open(source, "r").read()
-            processed = Filter(filename).process(content)
-            if processed != "":
-                with open(destiny, "w") as f:
-                    f.write(processed)
-            
-            line = "";
-            if processed != content:
-                if processed == "":
-                    line += "(disabled): "
-                else:
-                    line += "(filtered): "
-            else:
-                line += "(        ): "
-            line += destiny
-            print(line)
-
-    @staticmethod
     def deep_copy_and_change_dir():
         # path to ~/.tko_filter
         filter_path = os.path.join(os.path.expanduser("~"), ".tko_filter")
-        try:
-            if not os.path.isdir(filter_path):
-                os.makedirs(filter_path)
-            else:
-                # force remove  non empty dir
-                shutil.rmtree(filter_path)
-                os.makedirs(filter_path)
-        except FileExistsError as e:
-            print("fail: Dir " + filter_path + " could not be created.")
-            print("fail: verify your permissions, or if there is a file with the same name.")
-        
-        FilterMode.deep_filter_copy(".", filter_path)
+
+        # verify if filter command is available
+        if shutil.which("filter") is None:
+            print("ERROR: filter command not found")
+            print("Install feno with 'pip install feno'")
+            exit(1)
+
+        subprocess.run(["filter", "-rf", ".", "-o", filter_path])
 
         os.chdir(filter_path)
 
 
 class Run:
 
     def __init__(self, target_list: List[str], exec_cmd: Optional[str], param: Param.Basic):
```

### Comparing `tko-0.3.8/src/tko/basic.py` & `tko-0.3.9/src/tko/basic.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/diff.py` & `tko-0.3.9/src/tko/diff.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/down.py` & `tko-0.3.9/src/tko/down.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/format.py` & `tko-0.3.9/src/tko/format.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/guide.py` & `tko-0.3.9/src/tko/guide.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/loader.py` & `tko-0.3.9/src/tko/loader.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/pattern.py` & `tko-0.3.9/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/runner.py` & `tko-0.3.9/src/tko/runner.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/settings.py` & `tko-0.3.9/src/tko/settings.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/solver.py` & `tko-0.3.9/src/tko/solver.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/wdir.py` & `tko-0.3.9/src/tko/wdir.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko/writer.py` & `tko-0.3.9/src/tko/writer.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.8/src/tko.egg-info/PKG-INFO` & `tko-0.3.9/src/tko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.8
+Version: 0.3.9
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.8/src/tko.egg-info/SOURCES.txt` & `tko-0.3.9/src/tko.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 setup.py
 src/tko/__init__.py
 src/tko/__main__.py
 src/tko/actions.py
 src/tko/basic.py
 src/tko/diff.py
 src/tko/down.py
-src/tko/filter.py
 src/tko/format.py
 src/tko/guide.py
 src/tko/loader.py
 src/tko/pattern.py
 src/tko/runner.py
 src/tko/settings.py
 src/tko/solver.py
```

