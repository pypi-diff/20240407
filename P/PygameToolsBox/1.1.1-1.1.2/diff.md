# Comparing `tmp/PygameToolsBox-1.1.1.tar.gz` & `tmp/PygameToolsBox-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.1.1.tar", last modified: Sun Apr  7 02:53:45 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.1.2.tar", last modified: Sun Apr  7 03:14:21 2024, max compression
```

## Comparing `PygameToolsBox-1.1.1.tar` & `PygameToolsBox-1.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 02:53:45.774608 PygameToolsBox-1.1.1/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     3681 2024-04-07 02:53:45.772615 PygameToolsBox-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-07 02:53:45.746602 PygameToolsBox-1.1.1/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-07 02:52:58.000000 PygameToolsBox-1.1.1/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     4477 2024-04-07 02:51:57.000000 PygameToolsBox-1.1.1/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      517 2024-04-07 01:29:10.000000 PygameToolsBox-1.1.1/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 PygameToolsBox-1.1.1/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.1.1/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-07 02:53:45.771620 PygameToolsBox-1.1.1/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3681 2024-04-07 02:53:45.000000 PygameToolsBox-1.1.1/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-07 02:53:45.000000 PygameToolsBox-1.1.1/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 02:53:45.000000 PygameToolsBox-1.1.1/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 02:53:45.000000 PygameToolsBox-1.1.1/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-07 02:53:45.000000 PygameToolsBox-1.1.1/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3075 2024-04-07 02:29:42.000000 PygameToolsBox-1.1.1/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 02:53:45.774608 PygameToolsBox-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 03:14:21.826459 PygameToolsBox-1.1.2/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3681 2024-04-07 03:14:21.825456 PygameToolsBox-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 03:14:21.801462 PygameToolsBox-1.1.2/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-07 03:11:58.000000 PygameToolsBox-1.1.2/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     4439 2024-04-07 03:12:15.000000 PygameToolsBox-1.1.2/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      517 2024-04-07 01:29:10.000000 PygameToolsBox-1.1.2/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2838 2024-04-07 02:00:30.000000 PygameToolsBox-1.1.2/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.1.2/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-07 03:14:21.824470 PygameToolsBox-1.1.2/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3681 2024-04-07 03:14:21.000000 PygameToolsBox-1.1.2/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-07 03:14:21.000000 PygameToolsBox-1.1.2/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 03:14:21.000000 PygameToolsBox-1.1.2/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-07 03:14:21.000000 PygameToolsBox-1.1.2/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-07 03:14:21.000000 PygameToolsBox-1.1.2/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3075 2024-04-07 02:29:42.000000 PygameToolsBox-1.1.2/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 03:14:21.827456 PygameToolsBox-1.1.2/setup.cfg
```

### Comparing `PygameToolsBox-1.1.1/LICENSE` & `PygameToolsBox-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.1/PKG-INFO` & `PygameToolsBox-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.1.1/PygameToolsBox/animated_object.py` & `PygameToolsBox-1.1.2/PygameToolsBox/animated_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,21 +105,19 @@
 
     def get_action(self) -> str | None:
         """
         :return: Action currently set otherwise return None
         """
         return self._current_action.name if self._current_action else None
 
-    def update(self, pos: Rect):
+    def update(self):
         """
         Call every frame for adjust animation and object position
         :param pos: New position for the sprite
         """
-        self.rect = pos
-
         if self._cool_down > 0:
             self._cool_down -= 1
             return
 
         self._cool_down = self._cooling
         self._image_index = self._current_action.get_next()
```

### Comparing `PygameToolsBox-1.1.1/PygameToolsBox/mask_image.py` & `PygameToolsBox-1.1.2/PygameToolsBox/mask_image.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.1/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.1.2/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.1/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.1.2/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.1/PygameToolsBox.egg-info/PKG-INFO` & `PygameToolsBox-1.1.2/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.1.1
+Version: 1.1.2
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.1.1/README.md` & `PygameToolsBox-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.1.1/pyproject.toml` & `PygameToolsBox-1.1.2/pyproject.toml`

 * *Files identical despite different names*

