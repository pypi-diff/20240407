# Comparing `tmp/html_text_color-0.0.8.tar.gz` & `tmp/html_text_color-0.0.9.tar.gz`

## Comparing `html_text_color-0.0.8.tar` & `html_text_color-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 html_text_color-0.0.8/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 html_text_color-0.0.8/html_text_color/__init__.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 html_text_color-0.0.8/html_text_color/create_colored.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 html_text_color-0.0.8/html_text_color/test.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_multiple.html
--rw-r--r--   0        0        0    51463 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_multiple.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_single.html
--rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_single.svg
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_tokens.html
--rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.8/test_outputs/test_tokens.svg
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 html_text_color-0.0.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 html_text_color-0.0.8/LICENSE
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 html_text_color-0.0.8/README.md
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 html_text_color-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 html_text_color-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 html_text_color-0.0.9/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 html_text_color-0.0.9/html_text_color/__init__.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 html_text_color-0.0.9/html_text_color/create_colored.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 html_text_color-0.0.9/html_text_color/test.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 html_text_color-0.0.9/html_text_color/util.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 html_text_color-0.0.9/test_outputs/test_multiple.html
+-rw-r--r--   0        0        0    51463 2020-02-02 00:00:00.000000 html_text_color-0.0.9/test_outputs/test_multiple.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.9/test_outputs/test_single.html
+-rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.9/test_outputs/test_single.svg
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 html_text_color-0.0.9/test_outputs/test_tokens.html
+-rw-r--r--   0        0        0    23110 2020-02-02 00:00:00.000000 html_text_color-0.0.9/test_outputs/test_tokens.svg
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 html_text_color-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 html_text_color-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 html_text_color-0.0.9/README.md
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 html_text_color-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 html_text_color-0.0.9/PKG-INFO
```

### Comparing `html_text_color-0.0.8/.github/workflows/publish_to_pypi.yml` & `html_text_color-0.0.9/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/html_text_color/create_colored.py` & `html_text_color-0.0.9/html_text_color/create_colored.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from xml.etree import ElementTree as ET
 from xml.etree.ElementTree import ParseError
 import numpy as np
 from matplotlib import colormaps
 import re
+from html_text_color.util import convert_to_ranks
 
 replacements = {"▁": " ", "<0x0A>": "<br/>", "Ġ": " ", "\n": "<br>"}
 stupid_color = re.compile(r"^[rgb]{,3}$")
 
 
 def process_color_nums(color_nums, normalize=True, color_order=None, mn=None, mx=None):
     color_nums = np.array(color_nums)
@@ -38,16 +39,20 @@
         assert color_nums.shape[1] == 1, f"Invalid color_order {color_order}"
         cmap = colormaps.get_cmap(color_order)
         for i, n in enumerate(color_nums[:, 0]):
             out[i] = np.array(cmap(n)[:3]) * 255
     return out
 
 
-def from_text(tokens, color_nums, normalize=True, color_order=None, beautify=True):
+def from_text(
+    tokens, color_nums, normalize=True, color_order=None, beautify=True, ranked=False
+):
     tokens = tokens.copy()
+    if ranked:
+        color_nums = convert_to_ranks(color_nums)
     if type(tokens[0]) == list:
         mn = min(min(x) for x in color_nums)
         mx = max(max(x) for x in color_nums)
         color_nums = [
             process_color_nums(cn, normalize, color_order, mn=mn, mx=mx)
             for cn in color_nums
         ]
@@ -92,13 +97,14 @@
 def from_ids(
     ids,
     tokenizer,
     color_nums,
     normalize=True,
     color_order=None,
     beautify=True,
+    ranked=False,
 ):
     if isinstance(ids[0], list):
         tokens = [tokenizer.convert_ids_to_tokens(i) for i in ids]
     else:
         tokens = tokenizer.convert_ids_to_tokens(ids)
-    return from_text(tokens, color_nums, normalize, color_order, beautify)
+    return from_text(tokens, color_nums, normalize, color_order, beautify, ranked)
```

### Comparing `html_text_color-0.0.8/html_text_color/test.py` & `html_text_color-0.0.9/html_text_color/test.py`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/test_outputs/test_multiple.html` & `html_text_color-0.0.9/test_outputs/test_multiple.html`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/test_outputs/test_multiple.svg` & `html_text_color-0.0.9/test_outputs/test_multiple.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/test_outputs/test_single.svg` & `html_text_color-0.0.9/test_outputs/test_single.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/test_outputs/test_tokens.svg` & `html_text_color-0.0.9/test_outputs/test_tokens.svg`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/LICENSE` & `html_text_color-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/README.md` & `html_text_color-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/pyproject.toml` & `html_text_color-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `html_text_color-0.0.8/PKG-INFO` & `html_text_color-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: html_text_color
-Version: 0.0.8
+Version: 0.0.9
 Summary: Visualize number vector on text using colored html
 Author-email: Yannik Keller <yannik@kelnet.de>
 License: MIT License
 License-File: LICENSE
 Keywords: HTML,Language Model,color,text,visualization
 Requires-Python: >=3.6
 Requires-Dist: matplotlib
```

