# Comparing `tmp/sldc-cytomine-2.4.0.tar.gz` & `tmp/sldc-cytomine-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sldc-cytomine-2.4.0.tar", last modified: Thu Feb 29 16:45:47 2024, max compression
+gzip compressed data, was "sldc-cytomine-2.5.0.tar", last modified: Sun Apr  7 13:25:05 2024, max compression
```

## Comparing `sldc-cytomine-2.4.0.tar` & `sldc-cytomine-2.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:45:47.977373 sldc-cytomine-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-29 16:45:47.977373 sldc-cytomine-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 16:45:47.977373 sldc-cytomine-2.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:45:47.977373 sldc-cytomine-2.4.0/sldc_cytomine/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/sldc_cytomine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/sldc_cytomine/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/sldc_cytomine/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/sldc_cytomine/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/sldc_cytomine/tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-02-29 16:45:37.000000 sldc-cytomine-2.4.0/sldc_cytomine/tile_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 16:45:47.977373 sldc-cytomine-2.4.0/sldc_cytomine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-02-29 16:45:47.000000 sldc-cytomine-2.4.0/sldc_cytomine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-29 16:45:47.000000 sldc-cytomine-2.4.0/sldc_cytomine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 16:45:47.000000 sldc-cytomine-2.4.0/sldc_cytomine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 16:45:47.000000 sldc-cytomine-2.4.0/sldc_cytomine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-02-29 16:45:47.000000 sldc-cytomine-2.4.0/sldc_cytomine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:25:05.939796 sldc-cytomine-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-07 13:25:05.939796 sldc-cytomine-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 13:25:05.939796 sldc-cytomine-2.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:25:05.939796 sldc-cytomine-2.5.0/sldc_cytomine/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/sldc_cytomine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/sldc_cytomine/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/sldc_cytomine/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/sldc_cytomine/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/sldc_cytomine/tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-07 13:25:01.000000 sldc-cytomine-2.5.0/sldc_cytomine/tile_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:25:05.939796 sldc-cytomine-2.5.0/sldc_cytomine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-07 13:25:05.000000 sldc-cytomine-2.5.0/sldc_cytomine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-07 13:25:05.000000 sldc-cytomine-2.5.0/sldc_cytomine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:25:05.000000 sldc-cytomine-2.5.0/sldc_cytomine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-07 13:25:05.000000 sldc-cytomine-2.5.0/sldc_cytomine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 13:25:05.000000 sldc-cytomine-2.5.0/sldc_cytomine.egg-info/top_level.txt
```

### Comparing `sldc-cytomine-2.4.0/PKG-INFO` & `sldc-cytomine-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sldc-cytomine
-Version: 2.4.0
+Version: 2.5.0
 Summary: Cytomine-SLDC, a SLDC binding to Cytomine
 Home-page: https://github.com/waliens/sldc
 Author: Romain Mormont
 Author-email: romain.mormont@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

### Comparing `sldc-cytomine-2.4.0/setup.py` & `sldc-cytomine-2.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-__version__ = "v2.4.0"
+__version__ = "v2.5.0"
 
 setup(
     name="sldc-cytomine",
     version=__version__,
     description="Cytomine-SLDC, a SLDC binding to Cytomine",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `sldc-cytomine-2.4.0/sldc_cytomine/autodetect.py` & `sldc-cytomine-2.5.0/sldc_cytomine/autodetect.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.4.0/sldc_cytomine/dump.py` & `sldc-cytomine-2.5.0/sldc_cytomine/dump.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.4.0/sldc_cytomine/image.py` & `sldc-cytomine-2.5.0/sldc_cytomine/image.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.4.0/sldc_cytomine/tile.py` & `sldc-cytomine-2.5.0/sldc_cytomine/tile.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   """An abstract tile implementation that downloads the tile from a server and caches it in a local folder"""
   def __init__(self, working_path, parent, offset, width, height, tile_identifier=None, polygon_mask=None):
     Tile.__init__(self, parent, offset, width, height, tile_identifier=tile_identifier, polygon_mask=polygon_mask)
     self._working_path = working_path
 
   @abstractmethod
   def download_tile_image(self):
-    pass      
+    pass
 
   @property
   def cache_filename(self):
     image_instance = self.base_image.image_instance
     x, y, width, height = self.abs_offset_x, self.abs_offset_y, self.width, self.height
     zoom = self.base_image.zoom_level
     cache_filename_format = "{id}-{zoom}-{x}-{y}-{w}-{h}.png"
@@ -101,21 +101,41 @@
       raise TypeError(f"CytominePims tile should be used in conjunction with CytomineSlide only (as base image), found `{type(slide)}`")
     iip_topology = TileTopology(slide, None, max_width=256, max_height=256, overlap=0)
     col_tile = self.abs_offset_x // 256
     row_tile = self.abs_offset_y // 256
     tile_index = col_tile + row_tile * iip_topology.tile_horizontal_count
     _slice = slide.slice_instance
     zoom = self.base_image.image_instance.zoom - slide.zoom_level
+
     return Cytomine.get_instance().download_file(f"{_slice.imageServerUrl}/image/{_slice.path}/normalized-tile/zoom/{zoom}/ti/{tile_index}.jpg", self.cache_filepath, False, payload={
       "z_slices": "0",
       "timepoints": "0",
       "channels": "0,1,2",
       "colormaps": "#f00,#0f0,#00f",
     })
 
+class CytominePims20241Tile(CytomineDownloadableTile):
+  """Tile fetch using the PIMS CE/EET2024.1 """
+  def download_tile_image(self):
+    slide = self.base_image
+    if not isinstance(slide, CytomineSlide):
+      raise TypeError(f"CytominePims tile should be used in conjunction with CytomineSlide only (as base image), found `{type(slide)}`")
+    col_tile = self.abs_offset_x // 256
+    row_tile = self.abs_offset_y // 256
+    _slice = slide.slice_instance
+    zoom = self.base_image.image_instance.zoom - slide.zoom_level
+
+    return Cytomine.get_instance().download_file(f"sliceinstance/{_slice.id}/normalized-tile/zoom/{zoom}/tx/{col_tile}/ty/{row_tile}.jpg", self.cache_filepath, False, payload={
+    "z_slices": "0",
+    "timepoints": "0",
+    "channels": "0,1,2",
+    "colormaps": "#f00,#0f0,#00f",
+    })
+    # Not compatible with 2024.1, rather use
+
 
 class CytomineWindowTile(CytomineDownloadableTile):
   """Tiling using the window service"""
   def download_tile_image(self):
     return self.base_image.image_instance.window(
       x=self.abs_offset_x,
       y=self.abs_offset_y,
@@ -169,15 +189,15 @@
 
   def _iip_window(self):
     left_margin = self.abs_offset_x % 256
     top_margin = self.abs_offset_y % 256
     right_margin = 256 - (self.abs_offset_x + self.width) % 256
     bottom_margin = 256 - (self.abs_offset_y + self.height) % 256
     margins = [top_margin, left_margin, bottom_margin, right_margin]
-     
+
     offset = self.abs_offset_x - left_margin, self.abs_offset_y - top_margin
     width = self.width + left_margin + right_margin
     height = self.height + top_margin + bottom_margin
     window = self.base_image.window(offset=offset, max_width=width, max_height=height)
 
     return window, offset, (width, height), margins
 
@@ -201,12 +221,12 @@
 
   def fetch_subtiles(self):
     """fetch underlying tiles without loading them into memory"""
     from sldc_cytomine.tile_builder import CytomineGenericTileBuilder
     window, _, _, _ = self._iip_window()
     builder = CytomineGenericTileBuilder(self._tile_class, self._working_path)
     topology = TileTopology(window, builder, max_width=256, max_height=256, overlap=0)
-    
+
     def download_tile(tile: CytomineDownloadableTile):
       return tile.download_tile_image()
 
-    _ = parallel.generic_download(list(topology), download_tile, n_workers=self._n_jobs)
+    _ = parallel.generic_download(list(topology), download_tile, n_workers=self._n_jobs)
```

### Comparing `sldc-cytomine-2.4.0/sldc_cytomine/tile_builder.py` & `sldc-cytomine-2.5.0/sldc_cytomine/tile_builder.py`

 * *Files identical despite different names*

### Comparing `sldc-cytomine-2.4.0/sldc_cytomine.egg-info/PKG-INFO` & `sldc-cytomine-2.5.0/sldc_cytomine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sldc-cytomine
-Version: 2.4.0
+Version: 2.5.0
 Summary: Cytomine-SLDC, a SLDC binding to Cytomine
 Home-page: https://github.com/waliens/sldc
 Author: Romain Mormont
 Author-email: romain.mormont@gmail.com
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
```

