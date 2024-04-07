# Comparing `tmp/thothglyph_doc-0.2.0.tar.gz` & `tmp/thothglyph_doc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thothglyph_doc-0.2.0.tar", max compression
+gzip compressed data, was "thothglyph_doc-0.2.1.tar", max compression
```

## Comparing `thothglyph_doc-0.2.0.tar` & `thothglyph_doc-0.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1065 2022-10-23 13:24:34.663758 thothglyph_doc-0.2.0/LICENSE
--rw-r--r--   0        0        0      809 2023-09-03 08:22:53.916534 thothglyph_doc-0.2.0/README.md
--rw-r--r--   0        0        0      697 2023-09-03 08:22:53.916534 thothglyph_doc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-09-03 08:22:53.924535 thothglyph_doc-0.2.0/thothglyph/__init__.py
--rw-r--r--   0        0        0        0 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/app/__init__.py
--rw-r--r--   0        0        0     2500 2023-09-03 08:22:53.924535 thothglyph_doc-0.2.0/thothglyph/app/converter.py
--rw-r--r--   0        0        0     3115 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/data/tglyph.svg
--rw-r--r--   0        0        0     7412 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/data/tglyph_256.png
--rw-r--r--   0        0        0     1651 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/data/tglyph_64.png
--rw-r--r--   0        0        0       43 2023-09-03 08:22:53.924535 thothglyph_doc-0.2.0/thothglyph/error.py
--rw-r--r--   0        0        0     3064 2023-03-21 22:03:58.063084 thothglyph_doc-0.2.0/thothglyph/ext/blockdiag.py
--rw-r--r--   0        0        0     1164 2023-03-21 22:03:58.063084 thothglyph_doc-0.2.0/thothglyph/ext/graphviz.py
--rw-r--r--   0        0        0     2243 2022-10-30 22:30:03.141640 thothglyph_doc-0.2.0/thothglyph/ext/math.py
--rw-r--r--   0        0        0       74 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/ext/mermaid.py
--rw-r--r--   0        0        0       74 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/ext/plantuml.py
--rw-r--r--   0        0        0     1277 2023-03-21 22:03:58.063084 thothglyph_doc-0.2.0/thothglyph/ext/wavedrom.py
--rw-r--r--   0        0        0      580 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/node/logging.py
--rw-r--r--   0        0        0    17076 2023-03-29 17:17:41.872183 thothglyph_doc-0.2.0/thothglyph/node/nd.py
--rw-r--r--   0        0        0      311 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/reader/__init__.py
--rw-r--r--   0        0        0    26011 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/reader/md.py
--rw-r--r--   0        0        0     7344 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/reader/reader.py
--rw-r--r--   0        0        0    45257 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/reader/tglyph.py
--rw-r--r--   0        0        0     1557 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/template/common/check_dis.pdf
--rw-r--r--   0        0        0      627 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/template/common/check_dis.svg
--rw-r--r--   0        0        0     1597 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/template/common/check_en.pdf
--rw-r--r--   0        0        0      748 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/template/common/check_en.svg
--rw-r--r--   0        0        0     1638 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/template/common/check_im.pdf
--rw-r--r--   0        0        0      735 2022-10-23 13:56:14.057389 thothglyph_doc-0.2.0/thothglyph/template/common/check_im.svg
--rw-r--r--   0        0        0    52673 2022-10-30 22:30:03.141640 thothglyph_doc-0.2.0/thothglyph/template/docx/default/style.docx
--rw-r--r--   0        0        0     4840 2023-03-29 17:17:41.876183 thothglyph_doc-0.2.0/thothglyph/template/html/default/index.html
--rw-r--r--   0        0        0     3723 2023-03-29 17:17:41.876183 thothglyph_doc-0.2.0/thothglyph/template/html/preview/index.html
--rw-r--r--   0        0        0     6793 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/template/latex/default/document-ja.tex
--rw-r--r--   0        0        0      363 2023-09-03 08:22:53.928535 thothglyph_doc-0.2.0/thothglyph/writer/__init__.py
--rw-r--r--   0        0        0    18936 2023-09-03 08:22:53.932535 thothglyph_doc-0.2.0/thothglyph/writer/docx.py
--rw-r--r--   0        0        0    16304 2023-09-03 08:22:53.932535 thothglyph_doc-0.2.0/thothglyph/writer/html.py
--rw-r--r--   0        0        0    18211 2023-09-03 08:22:53.932535 thothglyph_doc-0.2.0/thothglyph/writer/latex.py
--rw-r--r--   0        0        0     4530 2023-09-03 08:22:53.932535 thothglyph_doc-0.2.0/thothglyph/writer/pdf.py
--rw-r--r--   0        0        0     5363 2023-09-03 08:22:53.932535 thothglyph_doc-0.2.0/thothglyph/writer/writer.py
--rw-r--r--   0        0        0     1502 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-09-03 08:30:24.832210 thothglyph_doc-0.2.1/LICENSE
+-rw-r--r--   0        0        0      813 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.1/README.md
+-rw-r--r--   0        0        0      697 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-07 14:47:55.090699 thothglyph_doc-0.2.1/thothglyph/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/app/__init__.py
+-rw-r--r--   0        0        0     2500 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/app/converter.py
+-rw-r--r--   0        0        0     3115 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/data/tglyph.svg
+-rw-r--r--   0        0        0     7412 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/data/tglyph_256.png
+-rw-r--r--   0        0        0     1651 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/data/tglyph_64.png
+-rw-r--r--   0        0        0       43 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/error.py
+-rw-r--r--   0        0        0     3064 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/blockdiag.py
+-rw-r--r--   0        0        0     1164 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/graphviz.py
+-rw-r--r--   0        0        0     2243 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/math.py
+-rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/mermaid.py
+-rw-r--r--   0        0        0       74 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/plantuml.py
+-rw-r--r--   0        0        0     1277 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/ext/wavedrom.py
+-rw-r--r--   0        0        0      580 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/node/logging.py
+-rw-r--r--   0        0        0    17076 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/node/nd.py
+-rw-r--r--   0        0        0      311 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/reader/__init__.py
+-rw-r--r--   0        0        0    26011 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/reader/md.py
+-rw-r--r--   0        0        0     7344 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/reader/reader.py
+-rw-r--r--   0        0        0    45290 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.1/thothglyph/reader/tglyph.py
+-rw-r--r--   0        0        0     1557 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.pdf
+-rw-r--r--   0        0        0      627 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.svg
+-rw-r--r--   0        0        0     1597 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_en.pdf
+-rw-r--r--   0        0        0      748 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_en.svg
+-rw-r--r--   0        0        0     1638 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_im.pdf
+-rw-r--r--   0        0        0      735 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/common/check_im.svg
+-rw-r--r--   0        0        0    52673 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/docx/default/style.docx
+-rw-r--r--   0        0        0     5439 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.1/thothglyph/template/html/default/index.html
+-rw-r--r--   0        0        0     4322 2024-04-07 14:47:55.094699 thothglyph_doc-0.2.1/thothglyph/template/html/preview/index.html
+-rw-r--r--   0        0        0     6793 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/template/latex/default/document-ja.tex
+-rw-r--r--   0        0        0      363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/__init__.py
+-rw-r--r--   0        0        0    18936 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/docx.py
+-rw-r--r--   0        0        0    16304 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/html.py
+-rw-r--r--   0        0        0    18211 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/latex.py
+-rw-r--r--   0        0        0     4530 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/pdf.py
+-rw-r--r--   0        0        0     5363 2023-09-03 08:30:24.836210 thothglyph_doc-0.2.1/thothglyph/writer/writer.py
+-rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 thothglyph_doc-0.2.1/PKG-INFO
```

### Comparing `thothglyph_doc-0.2.0/LICENSE` & `thothglyph_doc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/pyproject.toml` & `thothglyph_doc-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thothglyph-doc"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Documentation converter and language for Engineers"
 authors = ["nakandev <nakandev.s@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "thothglyph" },
 ]
```

### Comparing `thothglyph_doc-0.2.0/thothglyph/app/converter.py` & `thothglyph_doc-0.2.1/thothglyph/app/converter.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/data/tglyph.svg` & `thothglyph_doc-0.2.1/thothglyph/data/tglyph.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/data/tglyph_256.png` & `thothglyph_doc-0.2.1/thothglyph/data/tglyph_256.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/data/tglyph_64.png` & `thothglyph_doc-0.2.1/thothglyph/data/tglyph_64.png`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/ext/blockdiag.py` & `thothglyph_doc-0.2.1/thothglyph/ext/blockdiag.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/ext/graphviz.py` & `thothglyph_doc-0.2.1/thothglyph/ext/graphviz.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/ext/math.py` & `thothglyph_doc-0.2.1/thothglyph/ext/math.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/ext/wavedrom.py` & `thothglyph_doc-0.2.1/thothglyph/ext/wavedrom.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/node/logging.py` & `thothglyph_doc-0.2.1/thothglyph/node/logging.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/node/nd.py` & `thothglyph_doc-0.2.1/thothglyph/node/nd.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/reader/md.py` & `thothglyph_doc-0.2.1/thothglyph/reader/md.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/reader/reader.py` & `thothglyph_doc-0.2.1/thothglyph/reader/reader.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/reader/tglyph.py` & `thothglyph_doc-0.2.1/thothglyph/reader/tglyph.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,20 +41,20 @@
         'PREPROCESSED_LINE': r'^⑇$',
         'SECTION_TITLE_LINE': r' *((?:▮+)|(?:▯+))([*+]?) +([^⟦]+) *(?:⟦([^⟧]*)⟧)?',
         'TOC_LINE': r' *¤toc(?:⟦([^⟧]*)⟧)?⸨([^⸩]*)⸩ *$',
         'FIGURE_LINE': r' *¤figure(?:⟦([^⟧]*)⟧)?⸨([^⸩]*)⸩ *$',
         'TABLE_LINE': r'^ *\|.+\| *$',
         'LISTTABLE_BEGIN_LINE': r'^ *\|=== *(?:⟦([^⟧]*)⟧)? *$',
         'LISTTABLE_END_LINE': r'^ *===\| *$',
-        'FOOTNOTE_LIST_SYMBOL': r' *•\[\^(.+)\] +',
-        'REFERENCE_LIST_SYMBOL': r' *•\[\#(.+)\] +',
-        'CHECK_LIST_SYMBOL': r' *(•+)(\[[ x-]\]) +',
-        'BULLET_LIST_SYMBOL': r' *(•+) +',
-        'ORDERED_LIST_SYMBOL': r' *(꓾+) +',
-        'DESC_LIST_SYMBOL': r' *(ᛝ+)([^ᛝ]+)ᛝ(?: +)?',
+        'FOOTNOTE_LIST_SYMBOL': r' *•\[\^(.+)\](?: +|$)',
+        'REFERENCE_LIST_SYMBOL': r' *•\[\#(.+)\](?: +|$)',
+        'CHECK_LIST_SYMBOL': r' *(•+)(\[[ x-]\])(?: +|$)',
+        'BULLET_LIST_SYMBOL': r' *(•+)(?: +|$)',
+        'ORDERED_LIST_SYMBOL': r' *(꓾+)(?: +|$)',
+        'DESC_LIST_SYMBOL': r' *(ᛝ+)([^ᛝ]+)ᛝ(?: +|$)',
         'LIST_TERMINATOR_SYMBOL': r' *(◃+) *$',
         'CUSTOM_LINE': r'( *)¤¤¤(.*)',
         'CODE_LINE': r'( *)⸌⸌⸌(.*)',
         'QUOTE_SYMBOL': r'^ *> ',
         'HR_LINE': r'^ *(?:(={4,})|(-{4,}))$',
         'BREAK_LINE': r' *↲',
         'STR_LINE': r'.+',
@@ -509,15 +509,15 @@
             'BULLET_LIST_SYMBOL': nd.BulletListBlockNode,
             'ORDERED_LIST_SYMBOL': nd.OrderedListBlockNode,
             'DESC_LIST_SYMBOL': nd.DescriptionListBlockNode,
             'CHECK_LIST_SYMBOL': nd.CheckListBlockNode,
         }
         if token.key in table:
             listblock = table[token.key]()
-            m = re.match(r' *([•꓾ᛝ]+)([^ ]*)( +)', token.value)
+            m = re.match(r' *([•꓾ᛝ]+)([^ ]*)( +|$)', token.value)
             assert m
             listblock.level = len(m.group(1))
             listblock.indent = len(m.group(0))
             return listblock
         lineno = token.line + 1
         msg = 'Not list symbol.'
         msg = f'{self.reader.path}:{lineno}: {msg}'
```

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/common/check_dis.pdf` & `thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/common/check_dis.svg` & `thothglyph_doc-0.2.1/thothglyph/template/common/check_dis.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/common/check_en.pdf` & `thothglyph_doc-0.2.1/thothglyph/template/common/check_en.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/common/check_en.svg` & `thothglyph_doc-0.2.1/thothglyph/template/common/check_en.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/common/check_im.pdf` & `thothglyph_doc-0.2.1/thothglyph/template/common/check_im.pdf`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/common/check_im.svg` & `thothglyph_doc-0.2.1/thothglyph/template/common/check_im.svg`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/docx/default/style.docx` & `thothglyph_doc-0.2.1/thothglyph/template/docx/default/style.docx`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/html/default/index.html` & `thothglyph_doc-0.2.1/thothglyph/template/html/default/index.html`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,29 @@
 pre code {font-size: medium; border: 0px; padding: 0px;}
 code {background: #f8f8f8; border: 1px solid #ddd; padding: 5px 3px 0 3px; font-family: courier, monospace;}
 var {font-style: normal; font-family: courier, monospace; font-weight: bold;}
 kbd {background: #f8f8f8; border: 1px solid #ddd; border-radius: 3px; padding: 0px 3px 0 3px; font-family: sans-serif;}
 span.menu {background: #f8f8f8; border: 1px solid #ddd; padding: 0px 3px 0 3px; font-family: sans-serif;}
 a {color: #14d; text-decoration: none;}
 a:active, a:hover {text-decoration: underline;}
+@media (prefers-color-scheme: dark) {
+body {background-color: #000; color: #fff;}
+#header {background: #000; border-bottom: 2px solid #444;}
+#sidebar {background: #000; border-right: 2px solid #444;}
+h1 {border-bottom: 4px solid #444;}
+h2 {border-bottom: 2px solid #444;}
+blockquote {border-left: 4px solid #444;}
+table th {background: #222;}
+table th,td {border: 1px solid #888;}
+pre {border: 1px solid #444; background: #111;}
+code {border: 1px solid #444; background: #111;}
+kbd {background: #111; border: 1px solid #333;}
+span.menu {background: #111; border: 1px solid #333;}
+a {color: #48f;}
+}
 </style>
 <!-- <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/github-markdown-css@3.0.1/github-markdown.min.css"> -->
 <!-- Custom Extention: MathJax -->
 <!-- <script type="text/javascript" id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script> -->
 <!-- Custom Extention: WaveDrom -->
 <!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/wavedrom/2.6.8/skins/default.js" type="text/javascript"></script> -->
 <!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/wavedrom/2.6.8/wavedrom.min.js" type="text/javascript"></script> -->
```

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/html/preview/index.html` & `thothglyph_doc-0.2.1/thothglyph/template/html/preview/index.html`

 * *Files 15% similar despite different names*

```diff
@@ -45,14 +45,29 @@
 pre code {font-size: medium; border: 0px; padding: 0px;}
 code {background: #f8f8f8; border: 1px solid #ddd; padding: 5px 3px 0 3px; font-family: courier, monospace;}
 var {font-style: normal; font-family: courier, monospace; font-weight: bold;}
 kbd {background: #f8f8f8; border: 1px solid #ddd; border-radius: 3px; padding: 0px 3px 0 3px; font-family: sans-serif;}
 span.menu {background: #f8f8f8; border: 1px solid #ddd; padding: 0px 3px 0 3px; font-family: sans-serif;}
 a {color: #14d; text-decoration: none;}
 a:active, a:hover {text-decoration: underline;}
+@media (prefers-color-scheme: dark) {
+body {background-color: #000; color: #fff;}
+#header {background: #000; border-bottom: 2px solid #444;}
+#sidebar {background: #000; border-right: 2px solid #444;}
+h1 {border-bottom: 4px solid #444;}
+h2 {border-bottom: 2px solid #444;}
+blockquote {border-left: 4px solid #444;}
+table th {background: #222;}
+table th,td {border: 1px solid #888;}
+pre {border: 1px solid #444; background: #111;}
+code {border: 1px solid #444; background: #111;}
+kbd {background: #111; border: 1px solid #333;}
+span.menu {background: #111; border: 1px solid #333;}
+a {color: #48f;}
+}
 </style>
 <!-- <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/github-markdown-css@3.0.1/github-markdown.min.css"> -->
 <!-- Custom Extention: MathJax -->
 <!-- <script type="text/javascript" id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-chtml.js"></script> -->
 <!-- Custom Extention: WaveDrom -->
 <!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/wavedrom/2.6.8/skins/default.js" type="text/javascript"></script> -->
 <!-- <script src="https://cdnjs.cloudflare.com/ajax/libs/wavedrom/2.6.8/wavedrom.min.js" type="text/javascript"></script> -->
```

### Comparing `thothglyph_doc-0.2.0/thothglyph/template/latex/default/document-ja.tex` & `thothglyph_doc-0.2.1/thothglyph/template/latex/default/document-ja.tex`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/writer/docx.py` & `thothglyph_doc-0.2.1/thothglyph/writer/docx.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/writer/html.py` & `thothglyph_doc-0.2.1/thothglyph/writer/html.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/writer/latex.py` & `thothglyph_doc-0.2.1/thothglyph/writer/latex.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/writer/pdf.py` & `thothglyph_doc-0.2.1/thothglyph/writer/pdf.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/thothglyph/writer/writer.py` & `thothglyph_doc-0.2.1/thothglyph/writer/writer.py`

 * *Files identical despite different names*

### Comparing `thothglyph_doc-0.2.0/PKG-INFO` & `thothglyph_doc-0.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thothglyph-doc
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Documentation converter and language for Engineers
 License: MIT
 Author: nakandev
 Author-email: nakandev.s@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -66,10 +66,10 @@
 
 ## Languages
 
 See [documents](https://thothglyph-doc.readthedocs.io/en/latest/index.html)
 
 ## Tools
 
-* [vim-thothglyph](https://github.com/nakandev/vim-thothglyph)
-* [vscode-thothglyph](https://github.com/nakandev/vscode-thothglyph)
+* [vim-thothglyph](https://github.com/thothglyph/vim-thothglyph)
+* [vscode-thothglyph](https://github.com/thothglyph/vscode-thothglyph)
```

