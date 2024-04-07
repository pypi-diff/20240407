# Comparing `tmp/psychrochart-0.9.2.tar.gz` & `tmp/psychrochart-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.9.2.tar", max compression
+gzip compressed data, was "psychrochart-0.9.3.tar", max compression
```

## Comparing `psychrochart-0.9.2.tar` & `psychrochart-0.9.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11899 2023-07-30 10:32:10.109106 psychrochart-0.9.2/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-07-30 10:32:10.109106 psychrochart-0.9.2/LICENSE
--rw-r--r--   0        0        0     7883 2023-07-30 10:32:10.109106 psychrochart-0.9.2/README.md
--rw-r--r--   0        0        0      739 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/__init__.py
--rw-r--r--   0        0        0      336 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/__main__.py
--rw-r--r--   0        0        0    15292 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart.py
--rw-r--r--   0        0        0     2231 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_entities.py
--rw-r--r--   0        0        0     2157 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3097 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    15847 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chartdata.py
--rw-r--r--   0        0        0    18332 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/chartzones.py
--rw-r--r--   0        0        0        0 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/__init__.py
--rw-r--r--   0        0        0     3298 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/annots.py
--rw-r--r--   0        0        0     1246 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/base.py
--rw-r--r--   0        0        0     8674 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/config.py
--rw-r--r--   0        0        0     3945 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/curves.py
--rw-r--r--   0        0        0     5844 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/parsers.py
--rw-r--r--   0        0        0     2079 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/styles.py
--rw-r--r--   0        0        0     1924 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/models/validators.py
--rw-r--r--   0        0        0    16203 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/plot_logic.py
--rw-r--r--   0        0        0     8135 2023-07-30 10:32:10.121106 psychrochart-0.9.2/psychrochart/process_logic.py
--rw-r--r--   0        0        0     4631 2023-07-30 10:32:10.125106 psychrochart-0.9.2/psychrochart/util.py
--rw-r--r--   0        0        0     2271 2023-07-30 10:32:10.125106 psychrochart-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     9266 1970-01-01 00:00:00.000000 psychrochart-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    12511 2023-09-30 13:36:01.499213 psychrochart-0.9.3/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-09-30 13:36:01.499213 psychrochart-0.9.3/LICENSE
+-rw-r--r--   0        0        0     8573 2023-09-30 13:36:01.499213 psychrochart-0.9.3/README.md
+-rw-r--r--   0        0        0      739 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/__main__.py
+-rw-r--r--   0        0        0    15292 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart.py
+-rw-r--r--   0        0        0     2231 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart_entities.py
+-rw-r--r--   0        0        0     2157 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3457 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    17420 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chartdata.py
+-rw-r--r--   0        0        0    18585 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/chartzones.py
+-rw-r--r--   0        0        0        0 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     3298 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     1246 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/base.py
+-rw-r--r--   0        0        0     9272 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/config.py
+-rw-r--r--   0        0        0     4014 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5836 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     2704 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1924 2023-09-30 13:36:01.515213 psychrochart-0.9.3/psychrochart/models/validators.py
+-rw-r--r--   0        0        0    16316 2023-09-30 13:36:01.519213 psychrochart-0.9.3/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     8488 2023-09-30 13:36:01.519213 psychrochart-0.9.3/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     4631 2023-09-30 13:36:01.519213 psychrochart-0.9.3/psychrochart/util.py
+-rw-r--r--   0        0        0     2271 2023-09-30 13:36:01.519213 psychrochart-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     9956 1970-01-01 00:00:00.000000 psychrochart-0.9.3/PKG-INFO
```

### Comparing `psychrochart-0.9.2/CHANGELOG.md` & `psychrochart-0.9.3/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.9.3] - ✨ Add customizable annotations - 2023-09-30
+
+From @tadashiorigami in #44, thanks!
+
+##### Changes
+
+- ✨ Add styling for annotations (labeled curves in the chart), customizing their **font-size, color, and bbox style**.
+- 🔧 Support negative `constant_h_labels_loc` settings, to strech the constant h line to the left inside the saturated area, giving the chart an aspect closer to the popular ASHRAE chart.
+- ✅ Add unit test with example from @tadashiorigami, with styled annotations with bbox and hack for negative constant_h_labels_loc
+- 📦️ Bump version and update matplotlib to 3.8.0
+
 ## [0.9.2] - 🐛 Fix install with new pydantic v2 - 2023-07-30
 
 ##### Changes
 
 - 🎨 lint: pre-commit autoupdate
 - 📦️ env: Bump patch version and fix deps with pydantic version < v2, and enabling new Python 3.12
 - 📝 Update CHANGELOG
```

### Comparing `psychrochart-0.9.2/LICENSE` & `psychrochart-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/README.md` & `psychrochart-0.9.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -147,14 +147,34 @@
         "with_constant_rh": True,
         "constant_rh_curves": [25, 50, 75],
         "constant_rh_labels": [25, 50, 75],
         "with_constant_v": False,
         "with_constant_h": False,
         "with_constant_wet_temp": False,
         "with_zones": False
+    },
+    "constant_v_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":7,
+        "bbox": dict(boxstyle="square,pad=-0.2", color=[1, 1, 1, 0.9], lw=0.5)
+    },
+    "constant_h_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":6,
+        "bbox": dict(boxstyle="square,pad=-0.1", color=[1, 1, 1, 0.9], lw=0.5)
+    },
+    "constant_wet_temp_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":7,
+        "bbox": dict(boxstyle="square,pad=0", color=[1, 1, 1, 0.9], lw=0.5)
+    },
+    "constant_rh_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":7,
+        "bbox": dict(boxstyle="square,pad=0", color=[1, 1, 1, 0.9], lw=0.5)
     }
 }
 
 chart_custom_2 = PsychroChart.create(custom_style)
 chart_custom_2.plot()
 ```
```

### Comparing `psychrochart-0.9.2/psychrochart/__init__.py` & `psychrochart-0.9.3/psychrochart/__init__.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/chart.py` & `psychrochart-0.9.3/psychrochart/chart.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/chart_entities.py` & `psychrochart-0.9.3/psychrochart/chart_entities.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.9.3/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.9.3/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.9.3/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8505275974025974%*

 * *Differences: {"'chart_params'": "{'constant_rh_curves': {delete: [10, 8, 6, 5, 4, 2, 0]}, 'constant_rh_labels': "*

 * *                   "[], 'constant_v_step': 0.04, 'range_vol_m3_kg': {insert: [(0, 0.86)], delete: "*

 * *                   "[0]}, 'constant_v_labels': [], 'constant_h_step': 40, 'range_h': [20, 120], "*

 * *                   "'constant_h_labels': [], 'range_wet_temp': {insert: [(1, 35)], delete: [1]}, "*

 * *                   "'constant_wet_temp_labels': {delete: [7, 5, 3, 1, 0]}, 'constant_temp_step': "*

 * *                […]*

```diff
@@ -1,93 +1,51 @@
 {
     "chart_params": {
-        "constant_h_label": "Constant enthalpy",
-        "constant_h_labels": [
-            5,
-            25,
-            50,
-            75,
-            100,
-            125
-        ],
-        "constant_h_labels_loc": 1,
-        "constant_h_step": 5,
-        "constant_humid_label": "Absolute humidity",
-        "constant_humid_label_include_limits": true,
-        "constant_humid_label_step": 2,
-        "constant_humid_step": 1,
+        "constant_h_labels": [],
+        "constant_h_step": 40,
+        "constant_humid_label_include_limits": false,
+        "constant_humid_label_step": 10,
+        "constant_humid_step": 10,
         "constant_rh_curves": [
-            10,
             20,
-            30,
             40,
-            45,
-            50,
-            55,
             60,
-            70,
-            80,
-            90
-        ],
-        "constant_rh_label": "Constant relative humidity",
-        "constant_rh_labels": [
-            20,
-            30,
-            40,
-            50,
-            60,
-            70,
             80
         ],
-        "constant_rh_labels_loc": 0.85,
-        "constant_temp_label": "Dry bulb temperature",
-        "constant_temp_label_include_limits": true,
-        "constant_temp_label_step": 5,
-        "constant_temp_step": 1,
-        "constant_v_label": "Constant specific volume",
-        "constant_v_labels": [
-            0.8,
-            0.9,
-            0.96
-        ],
-        "constant_v_labels_loc": 1,
-        "constant_v_step": 0.02,
-        "constant_wet_temp_label": "Constant wet bulb temperature",
+        "constant_rh_labels": [],
+        "constant_temp_label_include_limits": false,
+        "constant_temp_label_step": 15,
+        "constant_temp_step": 5,
+        "constant_v_labels": [],
+        "constant_v_step": 0.04,
         "constant_wet_temp_labels": [
-            0,
-            5,
             10,
-            15,
             20,
-            25,
-            30,
-            35
+            30
         ],
-        "constant_wet_temp_labels_loc": 0.05,
         "constant_wet_temp_step": 5,
         "range_h": [
-            5,
-            155
+            20,
+            120
         ],
         "range_vol_m3_kg": [
-            0.78,
+            0.86,
             0.98
         ],
         "range_wet_temp": [
             -10,
-            40
+            35
         ],
         "with_constant_dry_temp": true,
         "with_constant_h": true,
-        "with_constant_humidity": true,
+        "with_constant_humidity": false,
         "with_constant_rh": true,
         "with_constant_v": true,
         "with_constant_wet_temp": true,
-        "with_zones": true,
-        "zones": []
+        "with_zones": false
     },
     "constant_dry_temp": {
         "color": [
             0.855,
             0.145,
             0.114
         ],
@@ -96,16 +54,16 @@
     },
     "constant_h": {
         "color": [
             0.251,
             0,
             0.502
         ],
-        "linestyle": "--",
-        "linewidth": 1
+        "linestyle": "-",
+        "linewidth": 2
     },
     "constant_humidity": {
         "color": [
             0,
             0.125,
             0.376
         ],
@@ -114,119 +72,118 @@
     },
     "constant_rh": {
         "color": [
             0,
             0.498,
             1
         ],
-        "linestyle": "-.",
-        "linewidth": 1
+        "linestyle": "-",
+        "linewidth": 2
     },
     "constant_v": {
         "color": [
             0,
             0.502,
             0.337
         ],
-        "linestyle": "--",
-        "linewidth": 1
+        "linestyle": "-",
+        "linewidth": 2
     },
     "constant_wet_temp": {
         "color": [
             0.498,
             0.875,
             1
         ],
-        "linestyle": "-.",
+        "linestyle": "-",
         "linewidth": 1
     },
     "figure": {
-        "dpi": 150,
         "figsize": [
             16,
-            9
+            10
         ],
-        "fontsize": 10,
         "partial_axis": true,
         "position": [
-            0.025,
-            0.075,
-            0.925,
-            0.875
+            0,
+            0,
+            1,
+            1
         ],
-        "title": "Psychrometric Chart",
+        "title": null,
         "x_axis": {
             "color": [
-                0.2,
-                0.2,
-                0.2
+                0.855,
+                0.145,
+                0.114
             ],
             "linestyle": "-",
             "linewidth": 2
         },
         "x_axis_labels": {
             "color": [
-                0.2,
-                0.2,
-                0.2
+                0.855,
+                0.145,
+                0.114
             ],
-            "fontsize": 9
+            "fontsize": 11
         },
         "x_axis_ticks": {
             "color": [
-                0.2,
-                0.2,
-                0.2
+                0.855,
+                0.145,
+                0.114
             ],
-            "direction": "out"
+            "direction": "in",
+            "pad": -20
         },
-        "x_label": "Dry-bulb temperature, $\u00b0C$",
+        "x_label": "Dry-bulb temperature ($\u00b0C$)",
         "y_axis": {
             "color": [
-                0.3,
-                0.3,
-                0.3
+                0,
+                0.125,
+                0.376
             ],
             "linestyle": "-",
             "linewidth": 2
         },
         "y_axis_labels": {
             "color": [
-                0.3,
-                0.3,
-                0.3
+                0,
+                0.125,
+                0.376
             ],
-            "fontsize": 8
+            "fontsize": 10
         },
         "y_axis_ticks": {
             "color": [
-                0.3,
-                0.3,
-                0.3
+                0,
+                0.125,
+                0.376
             ],
-            "direction": "out"
+            "direction": "in",
+            "pad": -20
         },
-        "y_label": "Humidity ratio $w, g_w / kg_{da}$"
+        "y_label": "Humidity ratio ($g_w / kg_{da}$)"
     },
     "limits": {
-        "altitude_m": 0,
-        "pressure_kpa": null,
+        "altitude_m": 550,
         "range_humidity_g_kg": [
             0,
-            40
+            25
         ],
         "range_temp_c": [
-            0,
-            50
+            10,
+            40
         ],
-        "step_temp": 1
+        "step_temp": 0.25
     },
     "saturation": {
         "color": [
             0.855,
-            0.004,
-            0.278
+            0.145,
+            0.114
         ],
         "linestyle": "-",
-        "linewidth": 3
+        "linewidth": 5
     }
 }
```

### Comparing `psychrochart-0.9.2/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.9.3/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.9.3/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.9.3/psychrochart/chart_styles/default_chart_config.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6075197124304267%*

 * *Differences: {"'chart_params'": "{'constant_rh_curves': {insert: [(0, 10), (2, 30), (4, 45), (5, 50), (6, 55), "*

 * *                   "(8, 70), (10, 90)]}, 'constant_rh_labels': [20, 30, 40, 50, 60, 70, 80], "*

 * *                   "'constant_v_step': 0.02, 'range_vol_m3_kg': {insert: [(0, 0.78)], delete: "*

 * *                   "[0]}, 'constant_v_labels': [0.8, 0.9, 0.96], 'constant_h_step': 5, 'range_h': "*

 * *                   "[5, 155], 'constant_h_labels': [5, 25, 50, 75, 100, 125], 'range_wet_temp': "*

 * *                   "{in […]*

```diff
@@ -1,51 +1,93 @@
 {
     "chart_params": {
-        "constant_h_labels": [],
-        "constant_h_step": 40,
-        "constant_humid_label_include_limits": false,
-        "constant_humid_label_step": 10,
-        "constant_humid_step": 10,
+        "constant_h_label": "Constant enthalpy",
+        "constant_h_labels": [
+            5,
+            25,
+            50,
+            75,
+            100,
+            125
+        ],
+        "constant_h_labels_loc": 1,
+        "constant_h_step": 5,
+        "constant_humid_label": "Absolute humidity",
+        "constant_humid_label_include_limits": true,
+        "constant_humid_label_step": 2,
+        "constant_humid_step": 1,
         "constant_rh_curves": [
+            10,
+            20,
+            30,
+            40,
+            45,
+            50,
+            55,
+            60,
+            70,
+            80,
+            90
+        ],
+        "constant_rh_label": "Constant relative humidity",
+        "constant_rh_labels": [
             20,
+            30,
             40,
+            50,
             60,
+            70,
             80
         ],
-        "constant_rh_labels": [],
-        "constant_temp_label_include_limits": false,
-        "constant_temp_label_step": 15,
-        "constant_temp_step": 5,
-        "constant_v_labels": [],
-        "constant_v_step": 0.04,
+        "constant_rh_labels_loc": 0.85,
+        "constant_temp_label": "Dry bulb temperature",
+        "constant_temp_label_include_limits": true,
+        "constant_temp_label_step": 5,
+        "constant_temp_step": 1,
+        "constant_v_label": "Constant specific volume",
+        "constant_v_labels": [
+            0.8,
+            0.9,
+            0.96
+        ],
+        "constant_v_labels_loc": 1,
+        "constant_v_step": 0.02,
+        "constant_wet_temp_label": "Constant wet bulb temperature",
         "constant_wet_temp_labels": [
+            0,
+            5,
             10,
+            15,
             20,
-            30
+            25,
+            30,
+            35
         ],
+        "constant_wet_temp_labels_loc": 0.05,
         "constant_wet_temp_step": 5,
         "range_h": [
-            20,
-            120
+            5,
+            155
         ],
         "range_vol_m3_kg": [
-            0.86,
+            0.78,
             0.98
         ],
         "range_wet_temp": [
             -10,
-            35
+            40
         ],
         "with_constant_dry_temp": true,
         "with_constant_h": true,
-        "with_constant_humidity": false,
+        "with_constant_humidity": true,
         "with_constant_rh": true,
         "with_constant_v": true,
         "with_constant_wet_temp": true,
-        "with_zones": false
+        "with_zones": true,
+        "zones": []
     },
     "constant_dry_temp": {
         "color": [
             0.855,
             0.145,
             0.114
         ],
@@ -54,16 +96,21 @@
     },
     "constant_h": {
         "color": [
             0.251,
             0,
             0.502
         ],
-        "linestyle": "-",
-        "linewidth": 2
+        "linestyle": "--",
+        "linewidth": 1
+    },
+    "constant_h_annotation": {
+        "bbox": {},
+        "color": null,
+        "fontsize": 10
     },
     "constant_humidity": {
         "color": [
             0,
             0.125,
             0.376
         ],
@@ -72,118 +119,134 @@
     },
     "constant_rh": {
         "color": [
             0,
             0.498,
             1
         ],
-        "linestyle": "-",
-        "linewidth": 2
+        "linestyle": "-.",
+        "linewidth": 1
+    },
+    "constant_rh_annotation": {
+        "bbox": {},
+        "color": null,
+        "fontsize": 10
     },
     "constant_v": {
         "color": [
             0,
             0.502,
             0.337
         ],
-        "linestyle": "-",
-        "linewidth": 2
+        "linestyle": "--",
+        "linewidth": 1
+    },
+    "constant_v_annotation": {
+        "bbox": {},
+        "color": null,
+        "fontsize": 10
     },
     "constant_wet_temp": {
         "color": [
             0.498,
             0.875,
             1
         ],
-        "linestyle": "-",
+        "linestyle": "-.",
         "linewidth": 1
     },
+    "constant_wet_temp_annotation": {
+        "bbox": {},
+        "color": null,
+        "fontsize": 10
+    },
     "figure": {
+        "dpi": 150,
         "figsize": [
             16,
-            10
+            9
         ],
+        "fontsize": 10,
         "partial_axis": true,
         "position": [
-            0,
-            0,
-            1,
-            1
+            0.025,
+            0.075,
+            0.925,
+            0.875
         ],
-        "title": null,
+        "title": "Psychrometric Chart",
         "x_axis": {
             "color": [
-                0.855,
-                0.145,
-                0.114
+                0.2,
+                0.2,
+                0.2
             ],
             "linestyle": "-",
             "linewidth": 2
         },
         "x_axis_labels": {
             "color": [
-                0.855,
-                0.145,
-                0.114
+                0.2,
+                0.2,
+                0.2
             ],
-            "fontsize": 11
+            "fontsize": 9
         },
         "x_axis_ticks": {
             "color": [
-                0.855,
-                0.145,
-                0.114
+                0.2,
+                0.2,
+                0.2
             ],
-            "direction": "in",
-            "pad": -20
+            "direction": "out"
         },
-        "x_label": "Dry-bulb temperature ($\u00b0C$)",
+        "x_label": "Dry-bulb temperature, $\u00b0C$",
         "y_axis": {
             "color": [
-                0,
-                0.125,
-                0.376
+                0.3,
+                0.3,
+                0.3
             ],
             "linestyle": "-",
             "linewidth": 2
         },
         "y_axis_labels": {
             "color": [
-                0,
-                0.125,
-                0.376
+                0.3,
+                0.3,
+                0.3
             ],
-            "fontsize": 10
+            "fontsize": 8
         },
         "y_axis_ticks": {
             "color": [
-                0,
-                0.125,
-                0.376
+                0.3,
+                0.3,
+                0.3
             ],
-            "direction": "in",
-            "pad": -20
+            "direction": "out"
         },
-        "y_label": "Humidity ratio ($g_w / kg_{da}$)"
+        "y_label": "Humidity ratio $w, g_w / kg_{da}$"
     },
     "limits": {
-        "altitude_m": 550,
+        "altitude_m": 0,
+        "pressure_kpa": null,
         "range_humidity_g_kg": [
             0,
-            25
+            40
         ],
         "range_temp_c": [
-            10,
-            40
+            0,
+            50
         ],
-        "step_temp": 0.25
+        "step_temp": 1
     },
     "saturation": {
         "color": [
             0.855,
-            0.145,
-            0.114
+            0.004,
+            0.278
         ],
         "linestyle": "-",
-        "linewidth": 5
+        "linewidth": 3
     }
 }
```

### Comparing `psychrochart-0.9.2/psychrochart/chartdata.py` & `psychrochart-0.9.3/psychrochart/chartdata.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     GetTWetBulbFromHumRatio,
     GetVapPresFromHumRatio,
     isIP,
 )
 from scipy.interpolate import interp1d
 
 from psychrochart.models.curves import PsychroCurve, PsychroCurves
-from psychrochart.models.styles import CurveStyle
+from psychrochart.models.styles import AnnotationStyle, CurveStyle
 from psychrochart.util import solve_curves_with_iteration
 
 f_vec_hum_ratio_from_vap_press = np.vectorize(GetHumRatioFromVapPres)
 f_vec_moist_air_enthalpy = np.vectorize(GetMoistAirEnthalpy)
 f_vec_moist_air_volume = np.vectorize(GetMoistAirVolume)
 f_vec_dew_point_from_vap_press = np.vectorize(GetTDewPointFromVapPres)
 f_vec_dry_temp_from_enthalpy = np.vectorize(GetTDryBulbFromEnthalpyAndHumRatio)
@@ -113,14 +113,15 @@
     pressure: float,
     rh_perc_values: list[int],
     *,
     style: CurveStyle,
     rh_label_values: list[int] | None = None,
     label_loc: float = 0.0,
     family_label: str | None = None,
+    annotation_style: AnnotationStyle | None = None,
 ) -> PsychroCurves:
     """Generate curves of constant relative humidity for the chart."""
     rh_values = sorted(rh for rh in rh_perc_values if 0 <= rh <= 100)
     temps_ct_rh = np.arange(dbt_min, dbt_max + temp_step, temp_step)
     curves_ct_rh = [
         gen_points_in_constant_relative_humidity(temps_ct_rh, rh, pressure)
         for rh in rh_values
@@ -132,14 +133,15 @@
                 x_data=temps_ct_rh,
                 y_data=curve_ct_rh,
                 style=style,
                 type_curve="constant_rh_data",
                 label_loc=label_loc,
                 label=f"RH {rh:g} %" if rh in rh_label_values else None,
                 internal_value=float(rh),
+                annotation_style=annotation_style,
             )
             for rh, curve_ct_rh in zip(rh_values, curves_ct_rh)
         ],
         family_label=family_label,
     )
 
 
@@ -147,14 +149,15 @@
     w_humidity_ratio_min: float,
     temp: float,
     pressure: float,
     *,
     style: CurveStyle,
     type_curve: str | None = None,
     reverse: bool = False,
+    annotation_style: AnnotationStyle | None = None,
 ) -> PsychroCurve:
     """Generate vertical line (constant dry bulb temp) up to saturation."""
     w_max = _factor_out_w() * GetHumRatioFromVapPres(
         GetSatVapPres(temp), pressure
     )
     if reverse:
         path_y = [w_max, w_humidity_ratio_min]
@@ -162,63 +165,68 @@
         path_y = [w_humidity_ratio_min, w_max]
     return PsychroCurve(
         x_data=np.array([temp, temp]),
         y_data=np.array(path_y),
         style=style,
         type_curve=type_curve,
         internal_value=temp,
+        annotation_style=annotation_style,
     )
 
 
 def make_constant_dry_bulb_v_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     temps_vl: np.ndarray,
     *,
     style: CurveStyle,
     family_label: str | None = None,
+    annotation_style: AnnotationStyle | None = None,
 ) -> PsychroCurves:
     """Generate curves of constant dry bulb temperature (vertical)."""
     w_max_vec = _get_humid_ratio_in_saturation(temps_vl, pressure)
     return PsychroCurves(
         curves=[
             PsychroCurve(
                 x_data=np.array([temp, temp]),
                 y_data=np.array([w_humidity_ratio_min, w_max]),
                 style=style,
                 type_curve="constant_dry_temp_data",
                 internal_value=temp,
+                annotation_style=annotation_style,
             )
             for temp, w_max in zip(temps_vl, w_max_vec)
         ],
         family_label=family_label,
     )
 
 
 def make_constant_humidity_ratio_h_lines(
     dbt_max: float,
     pressure: float,
     ws_hl: np.ndarray,
     *,
     style: CurveStyle,
     family_label: str | None = None,
+    annotation_style: AnnotationStyle | None = None,
 ) -> PsychroCurves:
     """Generate curves of constant absolute humidity (horizontal)."""
     arr_hum_ratios = np.array(ws_hl) / _factor_out_w()
     dew_points = f_vec_dew_point_from_vap_press(
         dbt_max, f_vec_vap_press_from_hum_ratio(arr_hum_ratios, pressure)
     )
     return PsychroCurves(
         curves=[
             PsychroCurve(
                 x_data=np.array([t_dp, dbt_max]),
                 y_data=np.array([w, w]),
                 style=style,
                 type_curve="constant_humidity_data",
                 internal_value=w,
+                annotation_style=annotation_style,
             )
             for w, t_dp in zip(ws_hl, dew_points)
         ],
         family_label=family_label,
     )
 
 
@@ -246,18 +254,20 @@
 def make_constant_enthalpy_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     enthalpy_values: np.ndarray,
     *,
     saturation_curve: PsychroCurve,
     style: CurveStyle,
+    delta_t: float,
     h_label_values: list[float] | None = None,
     label_loc: float = 0.0,
     family_label: str | None = None,
     dbt_min_seen: float | None = None,
+    annotation_style: AnnotationStyle | None = None,
 ) -> PsychroCurves | None:
     """Generate curves of constant enthalpy for the chart."""
     h_in_sat = (
         f_vec_moist_air_enthalpy(
             saturation_curve.x_data, saturation_curve.y_data / _factor_out_w()
         )
         / _factor_out_h()
@@ -300,34 +310,65 @@
         lambda x: GetMoistAirEnthalpy(
             x, GetHumRatioFromVapPres(GetSatVapPres(x), pressure)
         )
         / _factor_out_h(),
     )
     w_in_sat = _get_humid_ratio_in_saturation(t_sat_points, pressure)
 
-    return PsychroCurves(
-        curves=[
+    curves = [
+        PsychroCurve(
+            x_data=np.array([t_sat, t_max]),
+            y_data=np.array([w_sat, w_humidity_ratio_min]),
+            style=style,
+            type_curve="constant_h_data",
+            label_loc=label_loc,
+            label=(
+                _make_enthalpy_label(h)
+                if isinstance(h_label_values, list)
+                and round(h, 3) in h_label_values
+                else None
+            ),
+            internal_value=round(h, 3),
+            annotation_style=annotation_style,
+        )
+        for t_sat, w_sat, t_max, h in zip(
+            t_sat_points, w_in_sat, temps_max_constant_h, h_objective
+        )
+    ]
+
+    if label_loc < 0:
+        style.linestyle = "--"
+        curves += [
             PsychroCurve(
-                x_data=np.array([t_sat, t_max]),
-                y_data=np.array([w_sat, w_humidity_ratio_min]),
+                x_data=np.array([t_sat + (delta_t * label_loc), t_sat]),
+                y_data=np.array(
+                    [
+                        w_sat
+                        + (delta_t * label_loc)
+                        * (w_humidity_ratio_min - w_sat)
+                        / (t_max - t_sat),
+                        w_sat,
+                    ]
+                ),
                 style=style,
                 type_curve="constant_h_data",
-                label_loc=label_loc,
-                label=(
-                    _make_enthalpy_label(h)
-                    if isinstance(h_label_values, list)
-                    and round(h, 3) in h_label_values
-                    else None
-                ),
                 internal_value=round(h, 3),
             )
-            for t_sat, w_sat, t_max, h in zip(
-                t_sat_points, w_in_sat, temps_max_constant_h, h_objective
+            for t_sat, w_sat, t_max, h, curve in zip(
+                t_sat_points,
+                w_in_sat,
+                temps_max_constant_h,
+                h_objective,
+                curves,
             )
-        ],
+            if curve.label is not None
+        ]
+
+    return PsychroCurves(
+        curves=curves,
         family_label=family_label,
     )
 
 
 def make_constant_specific_volume_lines(
     w_humidity_ratio_min: float,
     pressure: float,
@@ -335,14 +376,15 @@
     *,
     saturation_curve: PsychroCurve,
     style: CurveStyle,
     v_label_values: list[float] | None = None,
     label_loc: float = 0.0,
     family_label: str | None = None,
     dbt_min_seen: float | None = None,
+    annotation_style: AnnotationStyle | None = None,
 ) -> PsychroCurves | None:
     """Generate curves of constant specific volume for the chart."""
     v_in_sat = f_vec_moist_air_volume(
         saturation_curve.x_data,
         saturation_curve.y_data / _factor_out_w(),
         pressure,
     )
@@ -396,14 +438,15 @@
                 label=(
                     _make_vol_label(vol)
                     if isinstance(v_label_values, list)
                     and round(vol, 3) in v_label_values
                     else None
                 ),
                 internal_value=round(vol, 3),
+                annotation_style=annotation_style,
             )
             for t_sat, w_sat, t_max, vol in zip(
                 t_sat_points, w_in_sat, temps_max_constant_v, v_objective
             )
         ],
         family_label=family_label,
     )
@@ -417,14 +460,15 @@
     pressure: float,
     wbt_values: np.ndarray,
     *,
     style: CurveStyle,
     wbt_label_values: list[float] | None = None,
     label_loc: float = 0.0,
     family_label: str | None = None,
+    annotation_style: AnnotationStyle | None = None,
 ) -> PsychroCurves | None:
     """Generate curves of constant wet bulb temperature for the chart."""
     wt_min = GetTWetBulbFromHumRatio(
         dry_bulb_temp_min, w_humidity_ratio_min / _factor_out_w(), pressure
     )
     if -0.75 < wt_min < 0.0:  # slope change zone
         wt_min = 0
@@ -491,11 +535,12 @@
             label=(
                 _make_temp_label(wbt)
                 if isinstance(wbt_label_values, list)
                 and round(wbt, 3) in wbt_label_values
                 else None
             ),
             internal_value=wbt,
+            annotation_style=annotation_style,
         )
         curves.append(c)
 
     return PsychroCurves(curves=curves, family_label=family_label)
```

### Comparing `psychrochart-0.9.2/psychrochart/chartzones.py` & `psychrochart-0.9.3/psychrochart/chartzones.py`

 * *Files 5% similar despite different names*

```diff
@@ -190,14 +190,15 @@
     return PsychroCurve(
         x_data=np.array(dbt_points),
         y_data=np.array(w_points),
         style=zone.style,
         type_curve=zone.zone_type,
         label=zone.label,
         internal_value=random_internal_value() if zone.label is None else None,
+        annotation_style=zone.annotation_style,
     )
 
 
 def _make_zone_delimited_by_enthalpy_and_rh(
     zone: ChartZone,
     pressure: float,
     *,
@@ -206,25 +207,27 @@
     dbt_max: float,
     w_min: float,
     w_max: float,
 ) -> PsychroCurve | None:
     assert zone.zone_type == "enthalpy-rh"
     h_min, h_max = zone.points_x
     rh_min, rh_max = zone.points_y
+    delta_t = dbt_max - dbt_min
     dbt_min_use = _adjust_temp_range_for_enthalpy(
         (h_min, h_max), (dbt_min, dbt_max), pressure, step_temp
     )
     h_lines = make_constant_enthalpy_lines(
         w_min,
         pressure,
         np.array([h_min, h_max]),
         saturation_curve=make_saturation_line(
             dbt_min_use, dbt_max, step_temp, pressure
         ),
         style=CurveStyle(),
+        delta_t=delta_t,
     )
     if not _valid_zone_delimiter_on_plot_limits(
         zone, h_lines, dbt_min, dbt_max, w_min, w_max
     ):
         return None
 
     rh_lines = make_constant_relative_humidity_lines(
@@ -273,14 +276,15 @@
     return PsychroCurve(
         x_data=np.array(temps_zone),
         y_data=np.array(abs_humid),
         style=zone.style,
         type_curve=zone.zone_type,
         label=zone.label,
         internal_value=random_internal_value() if zone.label is None else None,
+        annotation_style=zone.annotation_style,
     )
 
 
 def _make_zone_delimited_by_volume_and_rh(
     zone: ChartZone,
     pressure: float,
     *,
@@ -359,14 +363,15 @@
         return PsychroCurve(
             x_data=np.array([dbt_1, dbt_2]),
             y_data=np.array([w_1, w_2]),
             style=zone.style,
             type_curve=zone.zone_type,
             label=zone.label,
             internal_value=w_2,
+            annotation_style=zone.annotation_style,
         )
 
     # build path clockwise starting in left bottom corner
     path_x, path_y = [], []
     if saturation.y_data[0] < w_1:  # saturation cuts lower w value
         idx_start = (saturation.y_data > w_1).argmax()
         t_start, t_end = (
@@ -436,14 +441,15 @@
     return PsychroCurve(
         x_data=np.array(path_x),
         y_data=np.array(path_y),
         style=zone.style,
         type_curve=zone.zone_type,
         label=zone.label,
         internal_value=w_2,
+        annotation_style=zone.annotation_style,
     )
 
 
 def make_zone_curve(
     zone_conf: ChartZone,
     *,
     pressure: float,
```

### Comparing `psychrochart-0.9.2/psychrochart/models/annots.py` & `psychrochart-0.9.3/psychrochart/models/annots.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/models/base.py` & `psychrochart-0.9.3/psychrochart/models/base.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/models/config.py` & `psychrochart-0.9.3/psychrochart/models/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Literal
 
 from pydantic import Extra, Field, root_validator
 
 from psychrochart.models.styles import (
+    AnnotationStyle,
     BaseConfig,
     CurveStyle,
     LabelStyle,
     TickStyle,
     ZoneStyle,
 )
 
@@ -34,14 +35,15 @@
 _DEFAULT_STYLE_WET_TEMP = CurveStyle(color=[0.498, 0.875, 1.0], linestyle="-.")
 _DEFAULT_STYLE_DRY_TEMP = CurveStyle(
     color=[0.855, 0.145, 0.114], linewidth=0.75, linestyle=":"
 )
 _DEFAULT_STYLE_HUMID = CurveStyle(
     color=[0.0, 0.125, 0.376], linewidth=0.75, linestyle=":"
 )
+_DEFAULT_STYLE_CURVES_ANNOTATION = AnnotationStyle(fontsize=10)
 
 ZoneKind = Literal[
     "dbt-rh", "xy-points", "enthalpy-rh", "volume-rh", "dbt-wmax"
 ]
 
 
 class ChartFigure(BaseConfig):
@@ -81,14 +83,15 @@
     """Pydantic model for styled fixed areas on the psychrochart."""
 
     points_x: list[float]
     points_y: list[float]
     label: str | None = Field(default=None)
     zone_type: ZoneKind = Field(default="xy-points")
     style: ZoneStyle = Field(default_factory=ZoneStyle)
+    annotation_style: AnnotationStyle = Field(default_factory=AnnotationStyle)
 
     @root_validator
     def _validate_zone_definition(cls, values):
         shape = len(values["points_x"]), len(values["points_y"])
         if shape[0] < 2 or shape[1] < 2 or shape[0] != shape[1]:
             raise ValueError(f"Invalid shape: {shape}")
         if values["zone_type"] != "xy-points" and (
@@ -127,15 +130,15 @@
     constant_v_labels_loc: float = Field(default=1.0)
 
     with_constant_h: bool = Field(default=True)
     constant_h_label: str | None = Field(default="Constant enthalpy")
     constant_h_step: float = Field(default=5)
     range_h: tuple[float, float] = Field(default=_DEFAULT_RANGE_ENTALPHY)
     constant_h_labels: list[float] = Field(default=_DEFAULT_CONSTANT_H_LABELS)
-    constant_h_labels_loc: float = Field(default=1.0)
+    constant_h_labels_loc: float = Field(default=1)
 
     with_constant_wet_temp: bool = Field(default=True)
     constant_wet_temp_label: str | None = Field(
         default="Constant wet bulb temperature"
     )
     constant_wet_temp_step: float = Field(default=5)
     range_wet_temp: tuple[float, float] = Field(
@@ -178,14 +181,26 @@
     saturation: CurveStyle = Field(default=_DEFAULT_STYLE_SAT)
     constant_rh: CurveStyle = Field(default=_DEFAULT_STYLE_RH)
     constant_v: CurveStyle = Field(default=_DEFAULT_STYLE_V)
     constant_h: CurveStyle = Field(default=_DEFAULT_STYLE_H)
     constant_wet_temp: CurveStyle = Field(default=_DEFAULT_STYLE_WET_TEMP)
     constant_dry_temp: CurveStyle = Field(default=_DEFAULT_STYLE_DRY_TEMP)
     constant_humidity: CurveStyle = Field(default=_DEFAULT_STYLE_HUMID)
+    constant_v_annotation: AnnotationStyle = Field(
+        default=_DEFAULT_STYLE_CURVES_ANNOTATION
+    )
+    constant_h_annotation: AnnotationStyle = Field(
+        default=_DEFAULT_STYLE_CURVES_ANNOTATION
+    )
+    constant_wet_temp_annotation: AnnotationStyle = Field(
+        default=_DEFAULT_STYLE_CURVES_ANNOTATION
+    )
+    constant_rh_annotation: AnnotationStyle = Field(
+        default=_DEFAULT_STYLE_CURVES_ANNOTATION
+    )
 
     chart_params: ChartParams = Field(default_factory=ChartParams)
 
     class Config:
         extra = Extra.ignore
 
     @property
```

### Comparing `psychrochart-0.9.2/psychrochart/models/curves.py` & `psychrochart-0.9.3/psychrochart/models/curves.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import AbstractSet, Any, Mapping
 
 import numpy as np
 from pydantic import BaseModel, Field, root_validator
 
-from psychrochart.models.styles import CurveStyle, ZoneStyle
+from psychrochart.models.styles import AnnotationStyle, CurveStyle, ZoneStyle
 from psychrochart.models.validators import parse_curve_arrays
 
 
 class PsychroCurve(BaseModel):
     """Pydantic model to store a psychrometric curve for plotting."""
 
     x_data: np.ndarray
     y_data: np.ndarray
     style: ZoneStyle | CurveStyle
     type_curve: str | None = None
     label: str | None = None
     label_loc: float = 0.75
     internal_value: float | None = None
+    annotation_style: AnnotationStyle | None = None
 
     class Config:
         arbitrary_types_allowed = True
         json_encoders = {np.ndarray: lambda x: x.tolist()}
 
     @root_validator(pre=True)
     def _parse_curve_data(cls, values):
```

### Comparing `psychrochart-0.9.2/psychrochart/models/parsers.py` & `psychrochart-0.9.3/psychrochart/models/parsers.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,51 +11,51 @@
     ChartPoint,
     ChartSeries,
     ConvexGroupTuple,
 )
 from psychrochart.models.config import ChartConfig, ChartZones, DEFAULT_ZONES
 
 PATH_STYLES = Path(__file__).absolute().parents[1] / "chart_styles"
-DEFAULT_CHART_CONFIG_FILE = str(PATH_STYLES / "default_chart_config.json")
-ASHRAE_CHART_CONFIG_FILE = str(PATH_STYLES / "ashrae_chart_style.json")
-ASHRAE_IP_CHART_CONFIG_FILE = str(PATH_STYLES / "ashrae_ip_chart_style.json")
-INTERIOR_CHART_CONFIG_FILE = str(PATH_STYLES / "interior_chart_style.json")
-MINIMAL_CHART_CONFIG_FILE = str(PATH_STYLES / "minimal_chart_style.json")
-DEFAULT_ZONES_FILE = str(PATH_STYLES / "default_comfort_zones.json")
+DEFAULT_CHART_CONFIG_FILE = PATH_STYLES / "default_chart_config.json"
+ASHRAE_CHART_CONFIG_FILE = PATH_STYLES / "ashrae_chart_style.json"
+ASHRAE_IP_CHART_CONFIG_FILE = PATH_STYLES / "ashrae_ip_chart_style.json"
+INTERIOR_CHART_CONFIG_FILE = PATH_STYLES / "interior_chart_style.json"
+MINIMAL_CHART_CONFIG_FILE = PATH_STYLES / "minimal_chart_style.json"
+DEFAULT_ZONES_FILE = PATH_STYLES / "default_comfort_zones.json"
 
 STYLES = {
     "ashrae": ASHRAE_CHART_CONFIG_FILE,
     "ashrae_ip": ASHRAE_IP_CHART_CONFIG_FILE,
     "default": DEFAULT_CHART_CONFIG_FILE,
     "interior": INTERIOR_CHART_CONFIG_FILE,
     "minimal": MINIMAL_CHART_CONFIG_FILE,
 }
 
 T = TypeVar("T", bound=BaseModel)
 
 
 def obj_loader(
     data_cls: Type[T],
-    data: T | dict[str, Any] | str | None = None,
+    data: T | dict[str, Any] | str | Path | None = None,
     default_obj: T | None = None,
 ) -> T:
     """Load pydantic model from disk, or raw, with optional defaults."""
     if data is None:
         return default_obj if default_obj is not None else data_cls()
     if isinstance(data, data_cls):
         return data
     if isinstance(data, str) and data in STYLES:
         return data_cls.parse_file(STYLES[data])
-    if isinstance(data, str):
+    if isinstance(data, (str, Path)):
         return data_cls.parse_file(data)
     return data_cls(**data)
 
 
 def load_config(
-    config: ChartConfig | dict[str, Any] | str | None = None
+    config: ChartConfig | dict[str, Any] | Path | str | None = None
 ) -> ChartConfig:
     """Load the plot params for the psychrometric chart."""
     return obj_loader(ChartConfig, config)
 
 
 def load_zones(
     zones: ChartZones | dict[str, Any] | str | None = None
```

### Comparing `psychrochart-0.9.2/psychrochart/models/styles.py` & `psychrochart-0.9.3/psychrochart/models/styles.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any
+
 from pydantic import Extra, Field, root_validator, validator
 
 from psychrochart.models.base import BaseConfig
 from psychrochart.models.validators import parse_color, reduce_field_abrs
 
 
 class CurveStyle(BaseConfig):
@@ -33,14 +35,33 @@
         extra = Extra.allow
 
     @validator("color", pre=True, always=True)
     def _color_arr(cls, v, values):
         return parse_color(v)
 
 
+class AnnotationStyle(BaseConfig):
+    """Container for matplotlib styling of curve annotations."""
+
+    color: list[float] | None = None
+    fontsize: int | float = Field(default=9)
+    bbox: dict[str, Any] = Field(default_factory=dict)
+
+    class Config:
+        extra = Extra.allow
+
+    @validator("color", pre=True, always=True)
+    def _color_arr(cls, v, values):
+        return parse_color(v) if v else None
+
+    def export_style(self) -> dict[str, Any]:
+        """Get enabled styling kwargs for curve annotation."""
+        return {key: value for key, value in self.dict().items() if value}
+
+
 class TickStyle(BaseConfig):
     """Container for matplotlib tick axes styling."""
 
     direction: str = Field(default="out")
     color: list[float] = Field(default=[0.2, 0.2, 0.2])
 
     class Config:
```

### Comparing `psychrochart-0.9.2/psychrochart/models/validators.py` & `psychrochart-0.9.3/psychrochart/models/validators.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/psychrochart/plot_logic.py` & `psychrochart-0.9.3/psychrochart/plot_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,16 +102,17 @@
         text_style["ha"] = "center"
 
     text_style["color"] = mod_color(curve.style.color, -25)
     if ha is not None:
         text_style["ha"] = ha
     if va is not None:
         text_style["va"] = va
-    if params:
-        text_style.update(params)
+
+    if curve.annotation_style is not None:
+        text_style.update(curve.annotation_style.export_style())
 
     return _annotate_label(ax, label, text_x, text_y, rotation, text_style)
 
 
 def plot_curve(
     curve: PsychroCurve, ax: Axes, label_prefix: str | None = None
 ) -> dict[str, Artist]:
@@ -169,16 +170,18 @@
             text_x = 0.5 * (bbox_p.x0 + bbox_p.x1)
             text_y = 0.5 * (bbox_p.y0 + bbox_p.y1)
             style_params = {
                 "ha": "center",
                 "va": "center",
                 "backgroundcolor": [1, 1, 1, 0.4],
             }
+
             assert isinstance(curve.style, ZoneStyle)
-            style_params["color"] = mod_color(curve.style.edgecolor, -25)
+            if curve.annotation_style is not None:
+                style_params.update(curve.annotation_style.export_style())
             reg_artist(
                 "label_" + gid_zone,
                 _annotate_label(
                     ax, curve.label, text_x, text_y, 0, style_params
                 ),
                 artists,
             )
```

### Comparing `psychrochart-0.9.2/psychrochart/process_logic.py` & `psychrochart-0.9.3/psychrochart/process_logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,32 +118,36 @@
             config.limits.step_temp,
             chart.pressure,
             rh_perc_values=rh_values,
             rh_label_values=config.chart_params.constant_rh_labels,
             style=config.constant_rh,
             label_loc=config.chart_params.constant_rh_labels_loc,
             family_label=config.chart_params.constant_rh_label,
+            annotation_style=config.constant_rh_annotation,
         )
     else:
         chart.constant_rh_data = None
 
     # Constant enthalpy lines:
     if config.chart_params.with_constant_h:
         step = config.chart_params.constant_h_step
         start, end = config.chart_params.range_h
+        delta_t = config.limits.range_temp_c[1] - config.limits.range_temp_c[0]
         chart.constant_h_data = make_constant_enthalpy_lines(
             config.w_min,
             chart.pressure,
             enthalpy_values=np.arange(start, end, step),
+            delta_t=delta_t,
             h_label_values=config.chart_params.constant_h_labels,
             style=config.constant_h,
             label_loc=config.chart_params.constant_h_labels_loc,
             family_label=config.chart_params.constant_h_label,
             saturation_curve=chart.saturation,
             dbt_min_seen=dbt_min_seen,
+            annotation_style=config.constant_h_annotation,
         )
     else:
         chart.constant_h_data = None
 
     # Constant specific volume lines:
     if config.chart_params.with_constant_v:
         step = config.chart_params.constant_v_step
@@ -154,14 +158,15 @@
             vol_values=np.arange(start, end, step),
             v_label_values=config.chart_params.constant_v_labels,
             style=config.constant_v,
             label_loc=config.chart_params.constant_v_labels_loc,
             family_label=config.chart_params.constant_v_label,
             saturation_curve=chart.saturation,
             dbt_min_seen=dbt_min_seen,
+            annotation_style=config.constant_v_annotation,
         )
     else:
         chart.constant_v_data = None
 
     # Constant wet bulb temperature lines:
     if config.chart_params.with_constant_wet_temp:
         step = config.chart_params.constant_wet_temp_step
@@ -173,14 +178,15 @@
             config.w_max,
             chart.pressure,
             wbt_values=np.arange(start, end, step),
             wbt_label_values=config.chart_params.constant_wet_temp_labels,
             style=config.constant_wet_temp,
             label_loc=config.chart_params.constant_wet_temp_labels_loc,
             family_label=config.chart_params.constant_wet_temp_label,
+            annotation_style=config.constant_wet_temp_annotation,
         )
     else:
         chart.constant_wbt_data = None
 
 
 def _gen_chart_zones(config: ChartConfig, chart: PsychroChartModel) -> None:
     # regen all zones
```

### Comparing `psychrochart-0.9.2/psychrochart/util.py` & `psychrochart-0.9.3/psychrochart/util.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.9.2/pyproject.toml` & `psychrochart-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 log_level = "INFO"
 log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.9.2"
+version = "0.9.3"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `psychrochart-0.9.2/PKG-INFO` & `psychrochart-0.9.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.10,<3.13
@@ -179,14 +179,34 @@
         "with_constant_rh": True,
         "constant_rh_curves": [25, 50, 75],
         "constant_rh_labels": [25, 50, 75],
         "with_constant_v": False,
         "with_constant_h": False,
         "with_constant_wet_temp": False,
         "with_zones": False
+    },
+    "constant_v_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":7,
+        "bbox": dict(boxstyle="square,pad=-0.2", color=[1, 1, 1, 0.9], lw=0.5)
+    },
+    "constant_h_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":6,
+        "bbox": dict(boxstyle="square,pad=-0.1", color=[1, 1, 1, 0.9], lw=0.5)
+    },
+    "constant_wet_temp_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":7,
+        "bbox": dict(boxstyle="square,pad=0", color=[1, 1, 1, 0.9], lw=0.5)
+    },
+    "constant_rh_annotation": {
+        "color":[0.2, 0.2, 0.2],
+        "fontsize":7,
+        "bbox": dict(boxstyle="square,pad=0", color=[1, 1, 1, 0.9], lw=0.5)
     }
 }
 
 chart_custom_2 = PsychroChart.create(custom_style)
 chart_custom_2.plot()
 ```
```

