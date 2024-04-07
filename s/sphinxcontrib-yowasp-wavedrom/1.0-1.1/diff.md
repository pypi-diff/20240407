# Comparing `tmp/sphinxcontrib_yowasp_wavedrom-1.0-py3-none-any.whl.zip` & `tmp/sphinxcontrib_yowasp_wavedrom-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 4619 bytes, number of entries: 5
--rw-r--r--  2.0 unx     3186 b- defN 16-Jan-01 00:00 sphinxcontrib/yowasp_wavedrom.py
--rw-r--r--  2.0 unx     2737 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.0.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     1089 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.0.dist-info/licenses/LICENSE.txt
-?rw-------  2.0 unx      477 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.0.dist-info/RECORD
-5 files, 7594 bytes uncompressed, 3723 bytes compressed:  51.0%
+Zip file size: 4824 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     3687 b- defN 16-Jan-01 00:00 sphinxcontrib/yowasp_wavedrom.py
+-rw-r--r--  2.0 unx     2737 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1089 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.1.dist-info/licenses/LICENSE.txt
+?rw-------  2.0 unx      477 b- defN 16-Jan-01 00:00 sphinxcontrib_yowasp_wavedrom-1.1.dist-info/RECORD
+5 files, 8095 bytes uncompressed, 3928 bytes compressed:  51.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: sphinxcontrib/yowasp_wavedrom.py
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.0.dist-info/METADATA
+Filename: sphinxcontrib_yowasp_wavedrom-1.1.dist-info/METADATA
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.0.dist-info/WHEEL
+Filename: sphinxcontrib_yowasp_wavedrom-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.0.dist-info/licenses/LICENSE.txt
+Filename: sphinxcontrib_yowasp_wavedrom-1.1.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: sphinxcontrib_yowasp_wavedrom-1.0.dist-info/RECORD
+Filename: sphinxcontrib_yowasp_wavedrom-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sphinxcontrib/yowasp_wavedrom.py

```diff
@@ -1,13 +1,14 @@
 import re
 import json
-from pathlib import Path
+from pathlib import Path, PosixPath
 from docutils.parsers.rst import Directive
 from docutils import nodes
 import sphinx.application
+import sphinx.writers.html5
 import yowasp_wavedrom
 
 
 class WaveDromDirective(Directive):
     required_arguments = 1
     has_content = True
 
@@ -36,15 +37,15 @@
         return [node]
 
 
 class wavedrom_diagram(nodes.General, nodes.Inline, nodes.Element):
     pass
 
 
-def html_visit_wavedrom_diagram(self, node):
+def html_visit_wavedrom_diagram(self: sphinx.writers.html5.HTML5Translator, node: wavedrom_diagram):
     basename: str = node["name"]
     wavedrom_loc: str = node["loc"]
     wavedrom_src: dict = node["src"]
 
     # Adjust diagram configuration according to builder configuration.
     wavedrom_src_config = wavedrom_src.setdefault("config", {})
     if "signal" in wavedrom_src:
@@ -61,15 +62,23 @@
             f'</em>')
         raise nodes.SkipNode
     
     # Write the SVG to output directory. This is necessary because inlining it into the HTML has
     # significantly different behavior: duplicate IDs result in broken rendering, text can be
     # selected, media queries can't be overridden with a `color-scheme` CSS attribute for themes
     # that have a dark/light toggle via JS, etc.
-    pathname = Path(self.builder.outdir) / self.builder.imagedir / f'{basename}.svg'
+    pathname = Path(self.builder.outdir).joinpath(
+        # Note that for documents in subdirectories, the image directory is placed within that
+        # subdirectory. The other option would be to use enough `../` to locate the top-level
+        # image directory; using leading `/` in the `<img>` tag isn't feasible since that would
+        # break on `file:///` URLs.
+        PosixPath(self.builder.current_docname).parent,
+        self.builder.imagedir,
+        f'{basename}.svg'
+    )
     pathname.parent.mkdir(parents=True, exist_ok=True)
     pathname.write_text(wavedrom_svg)
 
     # Reference the SVG in the HTML document.
     self.body.append(f'<img src="{self.builder.imagedir}/{basename}.svg" '
         f'alt="{self.encode(node["src"])}">')
     raise nodes.SkipNode
```

## Comparing `sphinxcontrib_yowasp_wavedrom-1.0.dist-info/METADATA` & `sphinxcontrib_yowasp_wavedrom-1.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-yowasp-wavedrom
-Version: 1.0
+Version: 1.1
 Summary: A Sphinx extension for embedding WaveDrom diagrams
 Author-Email: Catherine <whitequark@whitequark.org>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: ~=3.8
 Requires-Dist: importlib_resources; python_version < "3.9"
 Requires-Dist: Sphinx~=7.1
-Requires-Dist: yowasp_wavedrom>=3.5.0.5
+Requires-Dist: yowasp-wavedrom>=3.5.0.6
 Description-Content-Type: text/markdown
 
 sphinxcontrib-yowasp-wavedrom
 =============================
 
 This [Sphinx] extension allows embedding [WaveDrom] waveform, bitfield, and circuit diagrams into Sphinx documents.
```

## Comparing `sphinxcontrib_yowasp_wavedrom-1.0.dist-info/licenses/LICENSE.txt` & `sphinxcontrib_yowasp_wavedrom-1.1.dist-info/licenses/LICENSE.txt`

 * *Files identical despite different names*

