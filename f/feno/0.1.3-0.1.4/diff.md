# Comparing `tmp/feno-0.1.3.tar.gz` & `tmp/feno-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.1.3.tar", last modified: Sat Apr  6 20:51:25 2024, max compression
+gzip compressed data, was "feno-0.1.4.tar", last modified: Sun Apr  7 03:39:54 2024, max compression
```

## Comparing `feno-0.1.3.tar` & `feno-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.126670 feno-0.1.3/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.3/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.3/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-06 20:51:25.126670 feno-0.1.3/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.3/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      630 2024-04-06 20:40:49.000000 feno-0.1.3/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.3/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-06 20:51:25.130003 feno-0.1.3/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.3/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.096670 feno-0.1.3/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.116670 feno-0.1.3/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-06 20:40:16.000000 feno-0.1.3/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2003 2024-04-04 23:51:34.000000 feno-0.1.3/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5188 2024-04-04 23:50:56.000000 feno-0.1.3/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.3/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.3/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.3/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5382 2024-04-03 18:14:31.000000 feno-0.1.3/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.3/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.3/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.3/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.3/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    11201 2024-04-04 23:37:02.000000 feno-0.1.3/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.3/src/feno/remote_md.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1375 2024-04-04 23:31:11.000000 feno-0.1.3/src/feno/tree.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-06 20:51:25.126670 feno-0.1.3/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-06 20:51:25.000000 feno-0.1.3/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.480001 feno-0.1.4/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.4/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.4/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 03:39:54.480001 feno-0.1.4/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.4/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      727 2024-04-07 00:21:27.000000 feno-0.1.4/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.4/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-07 03:39:54.480001 feno-0.1.4/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.4/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.463334 feno-0.1.4/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.476668 feno-0.1.4/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-06 22:35:14.000000 feno-0.1.4/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2191 2024-04-07 02:05:33.000000 feno-0.1.4/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5211 2024-04-07 02:09:04.000000 feno-0.1.4/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.4/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.4/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.4/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8883 2024-04-07 02:50:05.000000 feno-0.1.4/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.4/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.4/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.4/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.4/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    12742 2024-04-07 02:08:10.000000 feno-0.1.4/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.4/src/feno/remote_md.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.480001 feno-0.1.4/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.1.3/LICENSE` & `feno-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/PKG-INFO` & `feno-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.3
+Version: 0.1.4
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.3/README.md` & `feno-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/setup.py` & `feno-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno/__main__.py` & `feno-0.1.4/src/feno/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,52 +10,59 @@
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('targets', metavar='T', type=str, nargs='*', help='folders')
     parser.add_argument("--check", "-c", action="store_true", help="Check if the file needs to be rebuilt")
     parser.add_argument("--version", "-v", action="store_true", help="Prints the version")
 
     parser.add_argument("--brief", "-b", action="store_true", help="Brief mode")
-    parser.add_argument("--erase", "-e", action="store_true", help="Erase .html and .tio temp files")
-    parser.add_argument("--remote", "-r", action="store_true", help="Search for remote.cfg file and create absolute links")
+
     parser.add_argument("--tko", "-t", action="store_true", help="Insert tko preamble")
+    parser.add_argument("--remote", "-r", action="store_true", help="Search for remote.cfg file and create absolute links")
+    parser.add_argument("--erase", "-e", action="store_true", help="Erase .html and .tio temp files")
+
+    parser.add_argument("--full", "-f", action="store_true", help="Full mode - equivalent to -tre")
     
 
     args = parser.parse_args()
     Log.set_verbose(not args.brief)
+    if args.full:
+        args.tko = True
+        args.remote = True
+        args.erase = True
     
     if args.version:
         print(__version__)
         sys.exit(0)
 
     if len(args.targets) == 0:
         print("fail: No targets specified")
         exit(1)
 
     for target in args.targets:
         hook = os.path.basename(os.path.abspath(target))
 
         actions = Actions(target, args.remote, args.tko)
         Log.resume(hook, end=": [ ")
-        Log.verbose(hook, end=" ")
+        Log.verbose(hook)
 
         if not actions.validate():
             continue
 
         actions.load_title()
         actions.create_cache()
         actions.update_markdown()
 
         if not args.check or actions.need_rebuild():
             actions.recreate_cache() # erase .cache
             actions.copy_drafts()
+            actions.run_local_sh()
             actions.update_markdown() # se os drafts tiverem mudado o markdown precisa ser atualizado
             actions.remote_md()
             actions.html()
             actions.build_cases()
-            actions.run_local_sh()
             actions.init_vpl()
             actions.create_mapi()
             actions.clean(args.erase)
 
         Log.resume("]")
```

### Comparing `feno-0.1.3/src/feno/actions.py` & `feno-0.1.4/src/feno/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .jsontools import JsonVPL
 from .check import Check
 from .remote_md import RemoteMd, Title, RemoteCfg
 from .html import HTML
 from .cases import Cases
 from .log import Log
-from .tree import Tree
 from .mdpp import Mdpp
+from .filter import DeepFilter
 
 from typing import Optional
 import subprocess
 import os
 import shutil
 
 def norm_join(*args):
@@ -54,15 +54,15 @@
         shutil.rmtree(self.cache)
         os.makedirs(self.cache)
         return self
     
     def need_rebuild(self):
         if Check.need_rebuild(self.source_dir, self.target):
             Log.resume("Changes ", end="")
-            Log.verbose(f"    Changes in {self.source_dir}")
+            Log.verbose(f"  Changes in {self.source_dir}")
             return True
             
         Log.verbose("")
         return False
     
     def remote_md(self):
         cfg = RemoteCfg()
@@ -70,70 +70,71 @@
         if self.make_remote:
             cfg_path = RemoteCfg.search_cfg_path(self.source_dir)
             if cfg_path is None:
                 print("\n    fail: no remote.cfg found in the parent folders")
                 print("\n    fail: proceeding without make absolute links")
             else:
                 found = True
-                Log.verbose(f"    remote.cfg: {cfg_path}")
+                Log.verbose(f"  remote.cfg: {cfg_path}")
                 cfg.read(cfg_path)
         RemoteMd.run(cfg, self.source_readme, self.remote_readme, self.hook, self.insert_tko_preamble)
         if self.make_remote and found:
             Log.resume("AbsoluteMd ", end="")
-        Log.verbose(f"    RemoteFile: {self.remote_readme}")
+        Log.verbose(f"  RemoteFile: {self.remote_readme}")
     
     # uses pandoc to generate html from markdown
     def html(self):
         title = Title.extract_title(self.source_readme)
         HTML.generate_html_with_pandoc(title, self.remote_readme, self.target_html, True)
         Log.resume("HTML ", end="")
-        Log.verbose(f"    HTML  file: {self.target_html}")
+        Log.verbose(f"  HTML  file: {self.target_html}")
 
     # uses tko to generate cases file
     def build_cases(self):
         Cases.run(self.cases, self.source_readme, self.source_dir)
         Log.resume("Cases ", end="")
-        Log.verbose(f"    Cases file: {self.cases}")
+        Log.verbose(f"  Cases file: {self.cases}")
 
     def copy_drafts(self):
         source_src = norm_join(self.source_dir, "src")
         if os.path.isdir(source_src):
             Log.resume("Drafts ", end="")
-            Log.verbose(f"    Drafts dir: {source_src}")
-            Tree.deep_filter_copy(source_src, self.cache_src, 5)
+            Log.verbose(f"  Drafts dir: {source_src}")
+            filter = DeepFilter().set_indent(4)
+            filter.copy(source_src, self.cache_src, 5)
 
     def run_local_sh(self):
         local_sh = norm_join(self.source_dir, "local.sh")
         actual_chdir = os.getcwd()
         if os.path.isfile(local_sh):
+            Log.verbose(f"  Execute local.sh")
             os.chdir(self.source_dir)
             subprocess.run("bash local.sh", shell=True)
             os.chdir(actual_chdir)
             Log.resume("Local.sh ", end="")
-            Log.verbose(f"    local.sh executed")
 
     def init_vpl(self):
         self.vpl = JsonVPL(self.title, open(self.target_html).read())
         self.vpl.set_cases(self.cases)
         if self.vpl.load_config_json(self.config_json, self.source_dir):
             Log.resume("Required ", end="")
-            Log.verbose(f"    CfgVplJson: {self.config_json}")
+            Log.verbose(f"  CfgVplJson: {self.config_json}")
         if self.vpl.load_drafts(self.cache_src):
             Log.resume("Drafts ", end="")
 
     def create_mapi(self):
         open(self.mapi_json, "w").write(str(self.vpl) + "\n")
         Log.resume("Mapi ", end="")
-        Log.verbose(f"    Mapi  file: {self.mapi_json}")
+        Log.verbose(f"  Mapi  file: {self.mapi_json}")
 
     def clean(self, erase: bool):
         if erase:
             Log.resume("Cleaning ", end="")
-            Log.verbose("    Cleaning  : html and cases files")
+            Log.verbose("  Cleaning  : html and cases files")
             os.remove(self.cases)
             os.remove(self.target_html)
 
     # run mdpp script on source readme
     def update_markdown(self):
         if Mdpp.update_file(self.source_readme):
             Log.resume("Mdpp ", end="")
-            Log.verbose(f"    Mdpp updading")
+            Log.verbose(f"  Mdpp updading")
```

### Comparing `feno-0.1.3/src/feno/cases.py` & `feno-0.1.4/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno/check.py` & `feno-0.1.4/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno/css_style.py` & `feno-0.1.4/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno/filter.py` & `feno-0.1.4/src/feno/filter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import enum
 import os
 import argparse
 from typing import Tuple
+import shutil
 
 from .__init__ import __version__
 
 # modes
 # == RAW
 # ++ CUT
 # -- DEL
@@ -114,49 +115,149 @@
                 output.append(line)
         return "\n".join(output)
     
     def process(self, content: str) -> str:
         content = LegacyFilter(self.filename).process(content)
         return self.__process(content)
 
+def clean_com(target: str, content: str) -> str:
+    com = get_comment(target)
+    lines = content.split("\n")
+    output = [line for line in lines if not line.lstrip().startswith(com)]
+    return "\n".join(output)
+
+class DeepFilter:
+    extensions = [".md", ".c", ".cpp", ".h", ".hpp", ".py", ".java", ".js", ".ts", ".hs", ".txt"]
+
+    def __init__(self):
+        self.cheat_mode = False
+        self.quiet_mode = False
+        self.indent = ""
+    
+    def print(self, *args, **kwargs):
+        if not self.quiet_mode:
+            print(" " * self.indent, end="")
+            print(*args, **kwargs)
+
+    def set_indent(self, prefix: str):
+        self.indent = prefix
+        return self
+
+    def set_quiet(self, value):
+        self.quiet_mode = (value == True)
+        return self
+    
+    def set_cheat(self, value):
+        self.cheat_mode = (value == True)
+        return self
+
+    def copy(self, source, destiny, deep: int):
+        # print("debug", source, destiny, deep)
+        if deep == 0:
+            return
+        if os.path.isdir(source):
+            chain = source.split(os.sep)
+            if len(chain) > 1 and chain[-1].startswith("."):
+                return
+            if not os.path.isdir(destiny):
+                os.makedirs(destiny)
+            for file in sorted(os.listdir(source)):
+                self.copy(os.path.join(source, file), os.path.join(destiny, file), deep - 1)
+        else:
+            filename = os.path.basename(source)
+
+            if not any([filename.endswith(ext) for ext in self.extensions]):
+                return
+            content = open(source, "r").read()
+
+            processed = Filter(filename).process(content)
+
+            if self.cheat_mode:
+                if processed != content:
+                    cleaned = clean_com(source, content)
+                    with open(destiny, "w") as f:
+                        f.write(cleaned)
+            elif processed != "":
+                with open(destiny, "w") as f:
+                    f.write(processed)
+            
+
+            line = ""
+            if self.cheat_mode:
+                if processed != content:
+                    line += "(cleaned ): "
+                else:
+                    line += "(disabled): "
+            else:
+                if processed == "":
+                    line += "(disabled): "
+                elif processed != content:
+                    line += "(filtered): "
+                else:
+                    line += "(        ): "
+            line += destiny
 
+            self.print(line)
 
 def open_file(path): 
         if os.path.isfile(path):
             with open(path) as f:
                 file_content = f.read()
                 return True, file_content
         print("Warning: File", path, "not found")
         return False, "" 
 
 
-def rmcom(target: str, content: str) -> str:
-    com = get_comment(target)
-    lines = content.split("\n")
-    output = [line for line in lines if not line.lstrip().startswith(com)]
-    return "\n".join(output)
+
 
 def main():
     parser = argparse.ArgumentParser()
-    parser.add_argument('file', type=str, help='file to process')
+    parser.add_argument('target', type=str, help='file or folder to process')
     parser.add_argument('-u', '--update', action="store_true", help='update source file')
-    parser.add_argument('-r', '--rmcom', action="store_true", help='rm comments')
-    parser.add_argument('-o', '--output', type=str, help='output file')
+    parser.add_argument('-c', '--cheat', action="store_true", help='recursive cheat mode cleaning comments on students files')
+    parser.add_argument('-o', '--output', type=str, help='output target')
     parser.add_argument("-v", '--version', action="store_true", help='print version')
+    parser.add_argument("-r", "--recursive", action="store_true", help="recursive mode")
+    parser.add_argument("-f", "--force", action="store_true", help="force mode")
+    parser.add_argument("-q", "--quiet", action="store_true", help="quiet mode")
+    parser.add_argument("-i", "--indent", type=int, default=0, help="indent using spaces")
+
     args = parser.parse_args()
 
     if args.version:
         print(__version__)
         exit()
 
+    if args.cheat:
+        args.recursive = True
+
+    if args.recursive:
+        if args.output is None:
+            print("Error: output is required in recursive mode")
+            exit()
+        if not os.path.isdir(args.target):
+            print("Error: target must be a folder in recursive mode")
+            exit()
+        if os.path.exists(args.output):
+            if not args.force:
+                print("Error: output folder already exists")
+                exit()
+            else:
+                shutil.rmtree(args.output)
+                os.makedirs(args.output)
+
+        deep_filter = DeepFilter().set_cheat(args.cheat).set_quiet(args.quiet).set_indent(args.indent)
+        deep_filter.copy(args.target, args.output, 10)
+        exit()
+
     success, content = open_file(args.file)
     if success:
 
-        if args.rmcom:
-            content = rmcom(args.file, content)
+        if args.cheat:
+            content = clean_com(args.file, content)
         else:
             content = Filter(args.file).process(content)
 
         if args.output:
             if os.path.isfile(args.output):
                 old = open(args.output).read()
                 if old != content:
```

### Comparing `feno-0.1.3/src/feno/html.py` & `feno-0.1.4/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno/indexer.py` & `feno-0.1.4/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno/jsontools.py` & `feno-0.1.4/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno/mdpp.py` & `feno-0.1.4/src/feno/mdpp.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,51 @@
         if action == Action.RUN:
             new_toc = TocMaker.execute_toch(content)
             subst = r"<!-- toch -->\n" + new_toc + r"\n<!-- toch -->"
         else:
             subst = r"<!-- toch -->\n<!-- toch -->"
         return re.sub(regex, subst, content, 0, re.MULTILINE | re.DOTALL)
 
+class Links:
+
+    @staticmethod
+    def load_links(target):
+        origin = target
+        output = ""
+        if os.path.isdir(origin):
+            # create a markdown list os links with all files under .cache/src
+            entries = sorted(os.listdir(origin))
+            for lang in entries:
+                output += "- " + lang + "\n"
+                for file in sorted(os.listdir(os.path.join(origin, lang))):
+                    output += "  - [" + file + "](" + target + "/" + lang + "/" + file + ")\n"
+        return output
+
+    @staticmethod
+    def execute(path, content: str, action: Action = Action.RUN) -> str:
+        regex = r"<!-- links (\S*?) -->\n(.*?)<!-- links -->"
+        matches = re.finditer(regex, content, re.MULTILINE | re.DOTALL)
+        
+        # replace content of group 2 with load_links of group 1 for each match
+        for match in matches:
+            target = match.group(1)
+            lregex = r"<!-- links " + target + r" -->\n(.*?)<!-- links -->"
+            if action == Action.RUN:
+                path = os.path.dirname(path)
+                target = os.path.join(path, target)
+                new_links = Links.load_links(target)
+                subst = r"<!-- links " + target + r" -->\n" + new_links + r"<!-- links -->"
+            else:
+                subst = r"<!-- links " + target + r" -->\n<!-- links -->"
+            content = re.sub(lregex, subst, content, 0, re.MULTILINE | re.DOTALL)
+
+        return content
+            
+
+
 class Drafts:
 
     @staticmethod
     def load_drafts(readme_path):
         folder = os.path.dirname(readme_path)
         origin = os.path.join(folder, ".cache/lang")
         output = ""
@@ -283,14 +320,15 @@
         updated = original
         updated_toc = Toc.execute(updated, action)
         updated_toc = Toch.execute(updated_toc, action)
         if updated != updated_toc:
             updated = updated_toc
         updated = Load.execute(updated, target_dir, action)
         updated = Drafts.execute(target, updated, action)
+        updated = Links.execute(target, updated, action)
         Save.execute(updated)
         
         if updated != original:
             with open(path, "w") as f:
                 f.write(updated)
                 hook = os.path.abspath(path).split(os.sep)[-2]
                 return True
```

### Comparing `feno-0.1.3/src/feno/remote_md.py` & `feno-0.1.4/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.3/src/feno.egg-info/PKG-INFO` & `feno-0.1.4/src/feno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.3
+Version: 0.1.4
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.3/src/feno.egg-info/SOURCES.txt` & `feno-0.1.4/src/feno.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -14,14 +14,13 @@
 src/feno/filter.py
 src/feno/html.py
 src/feno/indexer.py
 src/feno/jsontools.py
 src/feno/log.py
 src/feno/mdpp.py
 src/feno/remote_md.py
-src/feno/tree.py
 src/feno.egg-info/PKG-INFO
 src/feno.egg-info/SOURCES.txt
 src/feno.egg-info/dependency_links.txt
 src/feno.egg-info/entry_points.txt
 src/feno.egg-info/requires.txt
 src/feno.egg-info/top_level.txt
```

