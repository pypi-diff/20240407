# Comparing `tmp/yowasp_wavedrom-3.5.0.5-py3-none-any.whl.zip` & `tmp/yowasp_wavedrom-3.5.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 40676 bytes, number of entries: 7
--rw-r--r--  2.0 unx      893 b- defN 24-Apr-05 02:01 yowasp_wavedrom/__init__.py
--rw-r--r--  2.0 unx   392666 b- defN 24-Apr-05 02:01 yowasp_wavedrom/bundle.js
--rw-r--r--  2.0 unx     3125 b- defN 24-Apr-05 02:02 yowasp_wavedrom-3.5.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 02:02 yowasp_wavedrom-3.5.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       62 b- defN 24-Apr-05 02:02 yowasp_wavedrom-3.5.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-05 02:02 yowasp_wavedrom-3.5.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      610 b- defN 24-Apr-05 02:02 yowasp_wavedrom-3.5.0.5.dist-info/RECORD
-7 files, 397464 bytes uncompressed, 39582 bytes compressed:  90.0%
+Zip file size: 40673 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      904 b- defN 24-Apr-07 07:07 yowasp_wavedrom/__init__.py
+-rw-r--r--  2.0 unx   392666 b- defN 24-Apr-07 07:07 yowasp_wavedrom/bundle.js
+-rw-r--r--  2.0 unx     3125 b- defN 24-Apr-07 07:07 yowasp_wavedrom-3.5.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 07:07 yowasp_wavedrom-3.5.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       62 b- defN 24-Apr-07 07:07 yowasp_wavedrom-3.5.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 24-Apr-07 07:07 yowasp_wavedrom-3.5.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      610 b- defN 24-Apr-07 07:07 yowasp_wavedrom-3.5.0.6.dist-info/RECORD
+7 files, 397475 bytes uncompressed, 39579 bytes compressed:  90.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: yowasp_wavedrom/__init__.py
 Comment: 
 
 Filename: yowasp_wavedrom/bundle.js
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.5.dist-info/METADATA
+Filename: yowasp_wavedrom-3.5.0.6.dist-info/METADATA
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.5.dist-info/WHEEL
+Filename: yowasp_wavedrom-3.5.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.5.dist-info/entry_points.txt
+Filename: yowasp_wavedrom-3.5.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.5.dist-info/top_level.txt
+Filename: yowasp_wavedrom-3.5.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: yowasp_wavedrom-3.5.0.5.dist-info/RECORD
+Filename: yowasp_wavedrom-3.5.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yowasp_wavedrom/__init__.py

```diff
@@ -1,14 +1,14 @@
 import sys
 import json
 import pathlib
 import quickjs
 try:
     import importlib.resources as importlib_resources
-    importlib_resources.files()
+    importlib_resources.files(__package__)
 except (ImportError, AttributeError):
     import importlib_resources
 
 
 def render(source):
     ctx = quickjs.Context()
     ctx.set("module", ctx.globalThis)
```

## Comparing `yowasp_wavedrom-3.5.0.5.dist-info/METADATA` & `yowasp_wavedrom-3.5.0.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yowasp-wavedrom
-Version: 3.5.0.5
+Version: 3.5.0.6
 Summary: WaveDrom generates diagrams for digital waveforms, bit fields, and simple combinational circuits
 Author-email: Catherine <whitequark@whitequark.org>
 License: MIT
 Project-URL: Homepage, https://yowasp.org/
 Project-URL: Source Code, https://github.com/YoWASP/wavedrom
 Project-URL: Bug Tracker, https://github.com/YoWASP/wavedrom/issues
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `yowasp_wavedrom-3.5.0.5.dist-info/RECORD` & `yowasp_wavedrom-3.5.0.6.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-yowasp_wavedrom/__init__.py,sha256=vVCyIlhFJodRLauOOJPiw7TzPQJwaAlH5MXPmECYT1Y,893
+yowasp_wavedrom/__init__.py,sha256=xzEXA9ZmV8f7EBToJ0nghMoyt_PbhjZZe2H4jRvx7Cs,904
 yowasp_wavedrom/bundle.js,sha256=rAsoqZhCJxhC2a3u5h3bnRnGvrpNRzTT38B5FMSPywc,392666
-yowasp_wavedrom-3.5.0.5.dist-info/METADATA,sha256=Uo7l0sD2LQjJ2cmdt2ZTBGroK0NugzXPmWvfOaW_AS8,3125
-yowasp_wavedrom-3.5.0.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-yowasp_wavedrom-3.5.0.5.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
-yowasp_wavedrom-3.5.0.5.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
-yowasp_wavedrom-3.5.0.5.dist-info/RECORD,,
+yowasp_wavedrom-3.5.0.6.dist-info/METADATA,sha256=4XI1QOnNuHhmn_RWrlps7uKNRdDIqwID7dTfw8SHlsc,3125
+yowasp_wavedrom-3.5.0.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+yowasp_wavedrom-3.5.0.6.dist-info/entry_points.txt,sha256=f1-Gv--EFDS68WqclOQZE7t_68tohm_3PCSOMxvxMRk,62
+yowasp_wavedrom-3.5.0.6.dist-info/top_level.txt,sha256=JtrHpwT3JTQeRyno78VqmBKi_sqTqNPqpjW2KixTsrE,16
+yowasp_wavedrom-3.5.0.6.dist-info/RECORD,,
```

