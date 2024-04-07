# Comparing `tmp/obsidown-0.1.4.tar.gz` & `tmp/obsidown-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsidown-0.1.4.tar", max compression
+gzip compressed data, was "obsidown-0.2.0.tar", max compression
```

## Comparing `obsidown-0.1.4.tar` & `obsidown-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2024-04-06 10:38:39.046856 obsidown-0.1.4/LICENSE
--rw-r--r--   0        0        0     1608 2024-04-06 10:38:39.046856 obsidown-0.1.4/README.md
--rw-r--r--   0        0        0      128 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/__init__.py
--rw-r--r--   0        0        0      338 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/__main__.py
--rw-r--r--   0        0        0      605 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/config.py
--rw-r--r--   0        0        0     4929 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/main.py
--rw-r--r--   0        0        0     1202 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/base.py
--rw-r--r--   0        0        0     6627 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/citations.py
--rw-r--r--   0        0        0     1235 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/dispatch.py
--rw-r--r--   0        0        0     1043 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/link_convert.py
--rw-r--r--   0        0        0      560 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/math_convert.py
--rw-r--r--   0        0        0      601 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/remove_after_string.py
--rw-r--r--   0        0        0     1197 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/update_frontmatter.py
--rw-r--r--   0        0        0      692 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/operations/write_file.py
--rw-r--r--   0        0        0     4246 2024-04-06 10:38:39.046856 obsidown-0.1.4/obsidown/utils.py
--rw-r--r--   0        0        0     2264 2024-04-06 10:38:39.046856 obsidown-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 obsidown-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-07 21:47:29.458471 obsidown-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1608 2024-04-07 21:47:29.458471 obsidown-0.2.0/README.md
+-rw-r--r--   0        0        0      128 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/__init__.py
+-rw-r--r--   0        0        0      338 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/__main__.py
+-rw-r--r--   0        0        0      686 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/config.py
+-rw-r--r--   0        0        0     5427 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/main.py
+-rw-r--r--   0        0        0     1202 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/base.py
+-rw-r--r--   0        0        0     6670 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/citations.py
+-rw-r--r--   0        0        0     1235 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/dispatch.py
+-rw-r--r--   0        0        0     1043 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/link_convert.py
+-rw-r--r--   0        0        0      560 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/math_convert.py
+-rw-r--r--   0        0        0      601 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/remove_after_string.py
+-rw-r--r--   0        0        0     1845 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/update_frontmatter.py
+-rw-r--r--   0        0        0      692 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/operations/write_file.py
+-rw-r--r--   0        0        0     4257 2024-04-07 21:47:29.458471 obsidown-0.2.0/obsidown/utils.py
+-rw-r--r--   0        0        0     2264 2024-04-07 21:47:29.458471 obsidown-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 obsidown-0.2.0/PKG-INFO
```

### Comparing `obsidown-0.1.4/LICENSE` & `obsidown-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.4/README.md` & `obsidown-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.4/obsidown/config.py` & `obsidown-0.2.0/obsidown/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 class SourcesList(BaseModel):
     paths: list[str]
     images: list[str]
 
 
 class Destination(BaseModel):
-    base: str  # URL base
+    base: str  # URL base o fthe files
     path: str  # where to store the files
     images: str  # where to store the images
+    images_path: str  # where to store the images in the filesystem
     filesystem: str  # the location of the processed files
 
 
 class Operation(BaseModel):
     name: str
     options: dict
```

### Comparing `obsidown-0.1.4/obsidown/main.py` & `obsidown-0.2.0/obsidown/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Iterable
 import yaml
 import os
-import frontmatter
 
 from obsidown.config import Config
 from obsidown.operations.base import MdFile, _load_contents
 from obsidown.operations.dispatch import dispatch
 from . import utils
 
 
@@ -49,27 +48,39 @@
                 operation.name, config, not_cited_refs, **operation.options
             )
             md_file = operation(md_file)
 
     # Now write the images on the filesystem
     save_images(image_refs, images, config)
 
+    # Don't know if index page is needed
     # Now create index pages
-    index_frontmatter = {
-        "layout": "page",
-        "title": "Notes",
-        "permalink": "/notes",
-        "tags": "italian",
-    }
-    index_content = "Here you can find the categories of all the notes on the site: \n"
-    index_content += create_table_contents(files, config)
-    with open(
-        os.path.join(config.output.filesystem, config.output.path, "index.md"), "w"
-    ) as f:
-        f.write(frontmatter.dumps(frontmatter.Post(index_content, **index_frontmatter)))
+
+
+#     index_frontmatter = {
+#         "title": "Notes",
+#     }
+#     index_content = "Follow the RSS feed of my notes:"
+#     index_content += """
+# <a href="/notes/index.xml" title="RSS" aria-label="RSS">
+#     <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"
+#     stroke-linecap="round" stroke-linejoin="round" height="23">
+#     <path d="M4 11a9 9 0 0 1 9 9" />
+#     <path d="M4 4a16 16 0 0 1 16 16" />
+#     <circle cx="5" cy="19" r="1" />
+#     </svg>
+# </a>
+# \n
+# """
+#     index_content += "Here you can find the categories of all the notes on the site: \n"
+# index_content += create_table_contents(files, config)
+# with open(
+#     os.path.join(config.output.filesystem, config.output.path, "index.md"), "w"
+# ) as f:
+#     f.write(frontmatter.dumps(frontmatter.Post(index_content, **index_frontmatter)))
 
 
 def save_images(image_refs: Iterable[str], images: list[str], config: Config):
     """Saves the images in the correct directory."""
     for image in image_refs:
         image_local_path = None
         for img in images:
@@ -80,21 +91,22 @@
             print(f"Image {image} not found in the filesystem")
             continue
 
         # This is to make sure we don't get any overlapping images!
         # Another solution is to change the name of the image...
         dirname = os.path.dirname(image)
         output_dir = os.path.join(
-            config.output.filesystem, config.output.images, dirname
+            config.output.filesystem, config.output.images_path, dirname
         )
         if not os.path.exists(output_dir):
             os.makedirs(output_dir)
 
         with open(
-            os.path.join(config.output.filesystem, config.output.images, image), "wb"
+            os.path.join(config.output.filesystem, config.output.images_path, image),
+            "wb",
         ) as f:
             with open(image_local_path, "rb") as i:
                 f.write(i.read())
 
 
 def create_table_contents(files: list[str], config: Config) -> str:
     """Creates the table of contents for the index page."""
@@ -109,20 +121,22 @@
             os.path.basename(os.path.dirname(file)).replace("-", " ").title()
         )
         if current_category not in categories:
             categories[current_category] = f"- [{no_extension}]({target})\n"
         else:
             categories[current_category] += f"- [{no_extension}]({target})\n"
 
-    index_content = "## Table of Contents\n"
-    for category in categories:
-        index_content += f"- [{category}](#{utils.to_kebab_case(category)})\n"
-    index_content += "\n\n"
+    # index_content = "## Table of Contents\n"
+    # for category in categories:
+    #     index_content += f"- [{category}](#{utils.to_kebab_case(category)})\n"
+    # index_content += "\n\n"
+
+    index_content = ""
 
-    for category, content in categories.items():
+    for category, content in sorted(categories.items(), key=lambda x: x[0]):
         index_content += f"## {category}\n"
         index_content += content + "\n\n"
 
     return index_content
 
 
 def load_images(filepath: str) -> list[str]:
```

### Comparing `obsidown-0.1.4/obsidown/operations/base.py` & `obsidown-0.2.0/obsidown/operations/base.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.4/obsidown/operations/citations.py` & `obsidown-0.2.0/obsidown/operations/citations.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
         new_contents = re.sub(
             r"\[\[@([^\]]+?)(\|([^\]]+))?\]\]",
             convert_to_citation,
             new_contents,
         )
 
         # Should add config to see if needs to add a section of references at the end
-        new_contents += "\n\n# References\n\n"
+        if len(citation_key_set) != 0:
+            new_contents += "\n\n# References\n\n"
         for i, key in enumerate(citation_key_set):
             entry = self.bib[key]
             new_contents += f"[{i+1}] {self._format_long_citation(entry)}\n\n"
 
         return MdFile(
             metadata=file.metadata,
             contents=new_contents,
```

### Comparing `obsidown-0.1.4/obsidown/operations/dispatch.py` & `obsidown-0.2.0/obsidown/operations/dispatch.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.4/obsidown/operations/link_convert.py` & `obsidown-0.2.0/obsidown/operations/link_convert.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def __call__(self, file: MdFile) -> MdFile:
         """Converts the links from the notes into the correct format for the markdown files."""
 
         contents = utils.convert_external_links(file.contents)
         if len(file.references) > 0:
             contents = utils.filter_link(contents, self.not_cited_refs)
             contents = utils.convert_images(contents, "/" + self.config.output.images)
-            contents = utils.convert_links(contents, "/" + self.config.output.path)
+            contents = utils.convert_links(contents, "/" + self.config.output.base)
         contents = utils.convert_links(contents)
 
         return MdFile(
             metadata=file.metadata,
             contents=contents,
             references=file.references,
             filename=file.filename,
```

### Comparing `obsidown-0.1.4/obsidown/operations/math_convert.py` & `obsidown-0.2.0/obsidown/operations/math_convert.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.4/obsidown/operations/remove_after_string.py` & `obsidown-0.2.0/obsidown/operations/remove_after_string.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.4/obsidown/operations/write_file.py` & `obsidown-0.2.0/obsidown/operations/write_file.py`

 * *Files identical despite different names*

### Comparing `obsidown-0.1.4/obsidown/utils.py` & `obsidown-0.2.0/obsidown/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,21 +49,21 @@
     "[https://google.com](https://google.com)"
     >>> convert_external_links("[https://google.com](https://google.com)")
     "[https://google.com](https://google.com)"
     """
 
     # Questo regex è un po' fragile, ma è difficile da fare, dovresti avere lookahead infinito!
     return re.sub(
-        r"(?<!\[)(https?:\/\/[^\s\]\(\)]+)(?!(\)|[a-z]|\.|[0-9]|[A-Z]|\/|_|-|=|\?|&|~))",
+        r"(?<!\[)(https?:\/\/[^\s\]\(\)]+)(?!(\)|[a-z]|\.|[0-9]|[A-Z]|\/|_|,|-|=|\?|&|~|#|%|:))",
         r"[\1](\1)",
         page,
     )
 
 
-def convert_links(page: str, base: str = ""):
+def convert_links(page: str, base: str = ""):  #
     """Convert the links to the markdown format.
     # Warning: this assumes images to be links to!
 
     Example
     -------
     >>> convert_links("hello [[world]]", "https://google.com")
     "hello [world](https://google.com/world)"
```

### Comparing `obsidown-0.1.4/pyproject.toml` & `obsidown-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "obsidown"
-version = "0.1.4"
+version = "0.2.0"
 description = "A quick way to convert obsidian markdown docs to markdown static pages"
 authors = ["Angelo 'Flecart' Huang <xuanqiang.huang@studio.unibo.it>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 homepage = "https://pypi.org/project/obsidown/"
 repository = "https://github.com/flecart/obsidown"
 classifiers = [
```

### Comparing `obsidown-0.1.4/PKG-INFO` & `obsidown-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsidown
-Version: 0.1.4
+Version: 0.2.0
 Summary: A quick way to convert obsidian markdown docs to markdown static pages
 Home-page: https://pypi.org/project/obsidown/
 License: GPL-3.0-only
 Author: Angelo 'Flecart' Huang
 Author-email: xuanqiang.huang@studio.unibo.it
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

