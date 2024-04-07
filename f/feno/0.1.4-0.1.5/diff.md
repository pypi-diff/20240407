# Comparing `tmp/feno-0.1.4.tar.gz` & `tmp/feno-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.1.4.tar", last modified: Sun Apr  7 03:39:54 2024, max compression
+gzip compressed data, was "feno-0.1.5.tar", last modified: Sun Apr  7 04:09:47 2024, max compression
```

## Comparing `feno-0.1.4.tar` & `feno-0.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.480001 feno-0.1.4/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.4/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.4/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 03:39:54.480001 feno-0.1.4/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.4/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      727 2024-04-07 00:21:27.000000 feno-0.1.4/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.4/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-07 03:39:54.480001 feno-0.1.4/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.4/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.463334 feno-0.1.4/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.476668 feno-0.1.4/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-06 22:35:14.000000 feno-0.1.4/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2191 2024-04-07 02:05:33.000000 feno-0.1.4/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5211 2024-04-07 02:09:04.000000 feno-0.1.4/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.4/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.4/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.4/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8883 2024-04-07 02:50:05.000000 feno-0.1.4/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.4/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.4/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.4/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.4/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    12742 2024-04-07 02:08:10.000000 feno-0.1.4/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.4/src/feno/remote_md.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 03:39:54.480001 feno-0.1.4/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-07 03:39:54.000000 feno-0.1.4/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.410005 feno-0.1.5/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.1.5/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.1.5/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 04:09:47.410005 feno-0.1.5/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     1471 2024-04-05 00:38:35.000000 feno-0.1.5/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      763 2024-04-07 04:08:40.000000 feno-0.1.5/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      306 2024-04-04 23:06:44.000000 feno-0.1.5/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-07 04:09:47.410005 feno-0.1.5/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.1.5/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.396671 feno-0.1.5/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.406671 feno-0.1.5/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-07 04:09:33.000000 feno-0.1.5/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2191 2024-04-07 02:05:33.000000 feno-0.1.5/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5211 2024-04-07 02:09:04.000000 feno-0.1.5/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.1.5/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.1.5/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.1.5/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8883 2024-04-07 02:50:05.000000 feno-0.1.5/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8925 2024-04-06 20:37:55.000000 feno-0.1.5/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.1.5/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3503 2024-04-05 00:31:13.000000 feno-0.1.5/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.1.5/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11661 2024-04-07 04:06:10.000000 feno-0.1.5/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4976 2024-04-04 23:15:36.000000 feno-0.1.5/src/feno/remote_md.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-07 04:09:47.410005 feno-0.1.5/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     2324 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      525 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       51 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-07 04:09:47.000000 feno-0.1.5/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.1.4/LICENSE` & `feno-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/PKG-INFO` & `feno-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.4
+Version: 0.1.5
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.4/README.md` & `feno-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/changelog.md` & `feno-0.1.5/changelog.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Changelog
 
+- 0.1.5
+  - fix: erro no mdpp links
 - 0.1.4
   - adicionado modo recursivo no filter
   - adicionando opcoes de clean, quiet no filter
 - 0.1.3
   - removendo link para css que gerava arquivos html diferentes
 - 0.1.1
   - apenas adiciona no drafts arquivos gerados
```

### Comparing `feno-0.1.4/setup.py` & `feno-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/__main__.py` & `feno-0.1.5/src/feno/__main__.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/actions.py` & `feno-0.1.5/src/feno/actions.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/cases.py` & `feno-0.1.5/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/check.py` & `feno-0.1.5/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/css_style.py` & `feno-0.1.5/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/filter.py` & `feno-0.1.5/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/html.py` & `feno-0.1.5/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/indexer.py` & `feno-0.1.5/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/jsontools.py` & `feno-0.1.5/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno/mdpp.py` & `feno-0.1.5/src/feno/mdpp.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,75 +103,44 @@
         else:
             subst = r"<!-- toch -->\n<!-- toch -->"
         return re.sub(regex, subst, content, 0, re.MULTILINE | re.DOTALL)
 
 class Links:
 
     @staticmethod
-    def load_links(target):
-        origin = target
+    def load_links(readme_dir, filter_dir):
+        origin = os.path.join(readme_dir, filter_dir)
         output = ""
         if os.path.isdir(origin):
             # create a markdown list os links with all files under .cache/src
             entries = sorted(os.listdir(origin))
             for lang in entries:
                 output += "- " + lang + "\n"
                 for file in sorted(os.listdir(os.path.join(origin, lang))):
-                    output += "  - [" + file + "](" + target + "/" + lang + "/" + file + ")\n"
+                    output += "  - [" + file + "](" + filter_dir + "/" + lang + "/" + file + ")\n"
         return output
 
     @staticmethod
     def execute(path, content: str, action: Action = Action.RUN) -> str:
         regex = r"<!-- links (\S*?) -->\n(.*?)<!-- links -->"
         matches = re.finditer(regex, content, re.MULTILINE | re.DOTALL)
         
         # replace content of group 2 with load_links of group 1 for each match
         for match in matches:
-            target = match.group(1)
-            lregex = r"<!-- links " + target + r" -->\n(.*?)<!-- links -->"
+            filter_dir = match.group(1)
+            lregex = r"<!-- links " + filter_dir + r" -->\n(.*?)<!-- links -->"
             if action == Action.RUN:
-                path = os.path.dirname(path)
-                target = os.path.join(path, target)
-                new_links = Links.load_links(target)
-                subst = r"<!-- links " + target + r" -->\n" + new_links + r"<!-- links -->"
+                readme_dir = os.path.normpath(os.path.dirname(path))
+                new_links = Links.load_links(readme_dir, filter_dir)
+                subst = r"<!-- links " + filter_dir + r" -->\n" + new_links + r"<!-- links -->"
             else:
-                subst = r"<!-- links " + target + r" -->\n<!-- links -->"
+                subst = r"<!-- links " + filter_dir + r" -->\n<!-- links -->"
             content = re.sub(lregex, subst, content, 0, re.MULTILINE | re.DOTALL)
 
         return content
-            
-
-
-class Drafts:
-
-    @staticmethod
-    def load_drafts(readme_path):
-        folder = os.path.dirname(readme_path)
-        origin = os.path.join(folder, ".cache/lang")
-        output = ""
-        if os.path.isdir(origin):
-            # create a markdown list os links with all files under .cache/src
-            entries = sorted(os.listdir(origin))
-            for lang in entries:
-                output += "- " + lang + "\n"
-                for file in sorted(os.listdir(os.path.join(origin, lang))):
-                    output += "  - [" + file + "](.cache/lang/" + lang + "/" + file + ")\n"
-
-        return output
-
-
-    @staticmethod
-    def execute(path, content: str, action: Action = Action.RUN) -> str:
-        regex = r"<!-- draft -->\n(.*?)<!-- draft -->"
-        if action == Action.RUN:
-            new_draft = Drafts.load_drafts(path)
-            subst = r"<!-- draft -->\n" + new_draft + r"\n<!-- draft -->"
-        else:
-            subst = r"<!-- draft -->\n<!-- draft -->"
-        return re.sub(regex, subst, content, 0, re.MULTILINE | re.DOTALL)
 
 class Load:
 
     @staticmethod
     def extract_between_tags(content, tag):
         regex = r"\[\[" + tag + r"\]\].*?^(.*)^[\S ]*\[\[" + tag + r"\]\]"
         matches = re.finditer(regex, content, re.MULTILINE | re.DOTALL)
@@ -319,15 +288,14 @@
             return False
         updated = original
         updated_toc = Toc.execute(updated, action)
         updated_toc = Toch.execute(updated_toc, action)
         if updated != updated_toc:
             updated = updated_toc
         updated = Load.execute(updated, target_dir, action)
-        updated = Drafts.execute(target, updated, action)
         updated = Links.execute(target, updated, action)
         Save.execute(updated)
         
         if updated != original:
             with open(path, "w") as f:
                 f.write(updated)
                 hook = os.path.abspath(path).split(os.sep)[-2]
```

### Comparing `feno-0.1.4/src/feno/remote_md.py` & `feno-0.1.5/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.1.4/src/feno.egg-info/PKG-INFO` & `feno-0.1.5/src/feno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.1.4
+Version: 0.1.5
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.1.4/src/feno.egg-info/SOURCES.txt` & `feno-0.1.5/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

