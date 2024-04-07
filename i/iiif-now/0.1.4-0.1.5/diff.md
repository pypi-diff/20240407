# Comparing `tmp/iiif_now-0.1.4.tar.gz` & `tmp/iiif_now-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iiif_now-0.1.4.tar", max compression
+gzip compressed data, was "iiif_now-0.1.5.tar", max compression
```

## Comparing `iiif_now-0.1.4.tar` & `iiif_now-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0      545 2024-04-05 18:46:31.521092 iiif_now-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     1157 2024-04-05 18:50:34.024138 iiif_now-0.1.4/README.md
--rw-r--r--   0        0        0      165 2024-04-03 22:15:54.969000 iiif_now-0.1.4/iiif_now/__init__.py
--rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.4/iiif_now/csvreader/__init__.py
--rw-r--r--   0        0        0     4520 2024-04-03 14:47:09.996938 iiif_now-0.1.4/iiif_now/csvreader/csvreader.py
--rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.4/iiif_now/datacanvas/__init__.py
--rw-r--r--   0        0        0     2033 2024-04-03 15:22:16.528962 iiif_now-0.1.4/iiif_now/datacanvas/datacanvas.py
--rw-r--r--   0        0        0      975 2024-04-02 23:02:06.414380 iiif_now-0.1.4/iiif_now/iiifnow.py
--rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.4/iiif_now/manifest/__init__.py
--rw-r--r--   0        0        0     6065 2024-04-05 18:45:21.332298 iiif_now-0.1.4/iiif_now/manifest/manifest.py
--rw-r--r--   0        0        0       30 2024-04-02 22:30:01.682517 iiif_now-0.1.4/iiif_now/navplace/__init__.py
--rw-r--r--   0        0        0     2418 2024-04-05 13:28:21.220416 iiif_now-0.1.4/iiif_now/navplace/navplace.py
--rw-r--r--   0        0        0       32 2024-04-03 22:15:54.948804 iiif_now-0.1.4/iiif_now/thumbnail/__init__.py
--rw-r--r--   0        0        0     1041 2024-04-03 22:38:50.485206 iiif_now-0.1.4/iiif_now/thumbnail/thumbnail.py
--rw-r--r--   0        0        0      593 2024-04-04 12:22:12.705733 iiif_now-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 iiif_now-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      726 2024-04-07 18:50:37.872348 iiif_now-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1157 2024-04-05 18:50:34.024138 iiif_now-0.1.5/README.md
+-rw-r--r--   0        0        0      232 2024-04-07 18:00:50.703436 iiif_now-0.1.5/iiif_now/__init__.py
+-rw-r--r--   0        0        0       33 2024-03-31 14:34:26.835751 iiif_now-0.1.5/iiif_now/csvreader/__init__.py
+-rw-r--r--   0        0        0     4520 2024-04-03 14:47:09.996938 iiif_now-0.1.5/iiif_now/csvreader/csvreader.py
+-rw-r--r--   0        0        0       34 2024-03-31 14:35:09.074716 iiif_now-0.1.5/iiif_now/datacanvas/__init__.py
+-rw-r--r--   0        0        0     2033 2024-04-03 15:22:16.528962 iiif_now-0.1.5/iiif_now/datacanvas/datacanvas.py
+-rw-r--r--   0        0        0       30 2024-04-07 16:37:09.970415 iiif_now-0.1.5/iiif_now/homepage/__init__.py
+-rw-r--r--   0        0        0      549 2024-04-07 16:57:23.725069 iiif_now-0.1.5/iiif_now/homepage/homepage.py
+-rw-r--r--   0        0        0      975 2024-04-02 23:02:06.414380 iiif_now-0.1.5/iiif_now/iiifnow.py
+-rw-r--r--   0        0        0       32 2024-03-31 23:06:07.096746 iiif_now-0.1.5/iiif_now/manifest/__init__.py
+-rw-r--r--   0        0        0     6653 2024-04-07 18:14:46.600465 iiif_now-0.1.5/iiif_now/manifest/manifest.py
+-rw-r--r--   0        0        0       30 2024-04-02 22:30:01.682517 iiif_now-0.1.5/iiif_now/navplace/__init__.py
+-rw-r--r--   0        0        0     2418 2024-04-05 13:28:21.220416 iiif_now-0.1.5/iiif_now/navplace/navplace.py
+-rw-r--r--   0        0        0       35 2024-04-07 18:00:50.724180 iiif_now-0.1.5/iiif_now/study_guide/__init__.py
+-rw-r--r--   0        0        0      810 2024-04-07 18:15:16.623561 iiif_now-0.1.5/iiif_now/study_guide/study_guide.py
+-rw-r--r--   0        0        0       32 2024-04-03 22:15:54.948804 iiif_now-0.1.5/iiif_now/thumbnail/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-03 22:38:50.485206 iiif_now-0.1.5/iiif_now/thumbnail/thumbnail.py
+-rw-r--r--   0        0        0      619 2024-04-07 16:55:53.125028 iiif_now-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2852 1970-01-01 00:00:00.000000 iiif_now-0.1.5/PKG-INFO
```

### Comparing `iiif_now-0.1.4/README.md` & `iiif_now-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.4/iiif_now/csvreader/csvreader.py` & `iiif_now-0.1.5/iiif_now/csvreader/csvreader.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.4/iiif_now/datacanvas/datacanvas.py` & `iiif_now-0.1.5/iiif_now/datacanvas/datacanvas.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.4/iiif_now/iiifnow.py` & `iiif_now-0.1.5/iiif_now/iiifnow.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.4/iiif_now/manifest/manifest.py` & `iiif_now-0.1.5/iiif_now/manifest/manifest.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from iiif_prezi3 import Manifest, config, KeyValueString, load_bundled_extensions, AnnotationPage, Annotation, ResourceItem
 import requests
 import json
+from iiif_now.homepage import HomePage
 from iiif_now.navplace import NavPlace
+from iiif_now.study_guide import StudyGuide
 from iiif_now.thumbnail import Thumbnail
 
 
 class ANManifest:
     def __init__(
             self,
             manifest_data,
@@ -24,32 +26,43 @@
         self.manifest = self.__build_manifest()
         self.extensions = load_bundled_extensions(
             extensions=extensions
         )
 
     def __build_manifest(self):
         # @Todo: Clean up this method.  It's a mess and doing too much.
+        homepage = HomePage(
+            self.manifest_data['manifest_title'] if self.manifest_data['manifest_title'] != "" else "Untitled"
+        ).body
+        rendering = StudyGuide(self.manifest_data['metadata']['Artist']).body
+        rights = "http://rightsstatements.org/vocab/InC/1.0/"
         if self.features:
             navplace_data = NavPlace(
                 self.features,
                 self.manifest_bucket,
                 self.manifest_data['manifest_title'] if self.manifest_data['manifest_title'] != "" else "Untitled"
             ).features
             manifest = Manifest(
                 id=f"{self.manifest_bucket}{self.manifest_data['id']}.json",
                 label=self.manifest_data['manifest_title'] if self.manifest_data['manifest_title'] != "" else "Untitled",
                 metadata=self.metadata,
-                navPlace={"features": navplace_data}
+                navPlace={"features": navplace_data},
+                homepage=[homepage],
+                rights=rights,
+                rendering=rendering
             )
         else:
             manifest = Manifest(
                 id=f"{self.manifest_bucket}{self.manifest_data['id']}.json",
                 label=self.manifest_data['manifest_title'] if self.manifest_data[
                                                                   'manifest_title'] != "" else "Untitled",
-                metadata=self.metadata
+                metadata=self.metadata,
+                homepage=[homepage],
+                rights=rights,
+                rendering=rendering
             )
         for canvas in self.manifest_data['canvases']:
             thumbnail = Thumbnail(f"{self.image_server_path}{canvas['thumbnail']}").get()
             if canvas['type'] == 'Image':
                 try:
                     # @Todo: Protect anno page and annotation
                     manifest.make_canvas_from_iiif(
```

### Comparing `iiif_now-0.1.4/iiif_now/navplace/navplace.py` & `iiif_now-0.1.5/iiif_now/navplace/navplace.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.4/iiif_now/thumbnail/thumbnail.py` & `iiif_now-0.1.5/iiif_now/thumbnail/thumbnail.py`

 * *Files identical despite different names*

### Comparing `iiif_now-0.1.4/pyproject.toml` & `iiif_now-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "iiif-now"
-version = "0.1.4"
+version = "0.1.5"
 description = "IIIF Manifest Generator for Abolition Now project"
 authors = ["Mark Baggett <mbagget1@utk.edu>"]
 license = "WTFPL"
 readme = ["README.md", "CHANGELOG.md"]
 repository = "https://github.com/abolition-now/iiif_now/"
 
 [tool.poetry.dependencies]
 python = "^3.8 || ^3.9 || ^3.10 || ^3.11 || ^3.12"
 requests = "^2.31.0"
 iiif-prezi3 = "^1.2.1"
 pyyaml = "^6.0.1"
 click = "^8.1.7"
 tqdm = "^4.66.2"
+python-slugify = "^8.0.4"
 
 [tool.poetry.scripts]
 iiifnow = "iiif_now.iiifnow:cli"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `iiif_now-0.1.4/PKG-INFO` & `iiif_now-0.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iiif-now
-Version: 0.1.4
+Version: 0.1.5
 Summary: IIIF Manifest Generator for Abolition Now project
 Home-page: https://github.com/abolition-now/iiif_now/
 License: WTFPL
 Author: Mark Baggett
 Author-email: mbagget1@utk.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: iiif-prezi3 (>=1.2.1,<2.0.0)
+Requires-Dist: python-slugify (>=8.0.4,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tqdm (>=4.66.2,<5.0.0)
 Project-URL: Repository, https://github.com/abolition-now/iiif_now/
 Description-Content-Type: text/markdown
 
 # IIIF Now
@@ -54,23 +55,31 @@
 ## Usage
 
 ```bash
 iiifnow use config.yml
 ```
 # Changes
 
+## [0.1.5] - 2024-04-07
+
+### Features
+
+* Added `homepage` to manifest.
+* Added `rights` to manifest.
+* Initialized `StudyGuide` as something that may be rendered from a manifest.
+
 ## [0.1.4] - 2024-04-05
 
 ### Features
 
 * Canvases now have metadata.
 
 ### Bug Fixes
 
-* Thumbnails: Both video an image canvases get thumbnails.
+* Thumbnails: Both video and image canvases get thumbnails.
 * navPlace: If location unknown, print error and pass.
 
 ### Minor Changes
 
 * Manifests: Got rid of all hard-coded URIs.
 
 ## [0.1.3] - 2024-04-03
```

