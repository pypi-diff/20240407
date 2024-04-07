# Comparing `tmp/yaml-to-markdown-0.1.1712383579.tar.gz` & `tmp/yaml-to-markdown-0.1.1712460996.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaml-to-markdown-0.1.1712383579.tar", last modified: Sat Apr  6 06:06:19 2024, max compression
+gzip compressed data, was "yaml-to-markdown-0.1.1712460996.tar", last modified: Sun Apr  7 03:36:37 2024, max compression
```

## Comparing `yaml-to-markdown-0.1.1712383579.tar` & `yaml-to-markdown-0.1.1712460996.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:06:19.932060 yaml-to-markdown-0.1.1712383579/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-06 06:06:19.932060 yaml-to-markdown-0.1.1712383579/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 06:06:19.932060 yaml-to-markdown-0.1.1712383579/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:06:19.928060 yaml-to-markdown-0.1.1712383579/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:06:19.932060 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/convert_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/md_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/md_converter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-06 06:05:23.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/utils_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 06:06:19.932060 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-06 06:06:19.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-06 06:06:19.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 06:06:19.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-06 06:06:19.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-06 06:06:19.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 06:06:19.000000 yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:36:37.039859 yaml-to-markdown-0.1.1712460996/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-07 03:36:37.039859 yaml-to-markdown-0.1.1712460996/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-07 03:36:37.039859 yaml-to-markdown-0.1.1712460996/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:36:37.035859 yaml-to-markdown-0.1.1712460996/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:36:37.039859 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/convert_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/md_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8067 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/md_converter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 03:35:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:36:37.039859 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-07 03:36:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-07 03:36:37.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:36:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 03:36:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-07 03:36:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 03:36:36.000000 yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/top_level.txt
```

### Comparing `yaml-to-markdown-0.1.1712383579/LICENSE` & `yaml-to-markdown-0.1.1712460996/LICENSE`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712383579/PKG-INFO` & `yaml-to-markdown-0.1.1712460996/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712383579
+Version: 0.1.1712460996
 Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `yaml-to-markdown-0.1.1712383579/README.md` & `yaml-to-markdown-0.1.1712460996/README.md`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712383579/setup.py` & `yaml-to-markdown-0.1.1712460996/setup.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/convert.py` & `yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/convert.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/convert_test.py` & `yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/convert_test.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/md_converter.py` & `yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/md_converter.py`

 * *Files identical despite different names*

### Comparing `yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown/md_converter_test.py` & `yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown/md_converter_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,33 @@
             == """##
 | Section1 |
 | --- |
 | data1 |
 """
         )
 
+    def test_process_list_of_list(self) -> None:
+        output_writer = StringIO()
+        md_converter = MDConverter()
+        data = [["list1 data1", "list1 data2"], ["list2 data1", "list2 data2"]]
+
+        md_converter.convert(data, output_writer)
+        output = output_writer.getvalue()
+
+        assert (
+            output
+            == """##
+* list1 data1
+* list1 data2
+* list2 data1
+* list2 data2
+
+"""
+        )
+
     def test_process_section_with_str(self) -> None:
         output_writer = StringIO()
         md_converter = MDConverter()
         data = {"section1": "data1"}
 
         md_converter.convert(data, output_writer)
         output = output_writer.getvalue()
```

### Comparing `yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/PKG-INFO` & `yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaml-to-markdown
-Version: 0.1.1712383579
+Version: 0.1.1712460996
 Summary: Converts a YAML/JSON file or python Dict/List to a Markdown file
 Home-page: https://anevis.github.io/yaml-to-markdown/
 Author: anevis
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click==8.1.7
```

### Comparing `yaml-to-markdown-0.1.1712383579/src/yaml_to_markdown.egg-info/SOURCES.txt` & `yaml-to-markdown-0.1.1712460996/src/yaml_to_markdown.egg-info/SOURCES.txt`

 * *Files identical despite different names*

