# Comparing `tmp/PygameToolsBox-1.0.8.tar.gz` & `tmp/PygameToolsBox-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.0.8.tar", last modified: Sat Apr  6 19:52:25 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.0.9.tar", last modified: Sat Apr  6 19:59:33 2024, max compression
```

## Comparing `PygameToolsBox-1.0.8.tar` & `PygameToolsBox-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 19:52:25.105299 PygameToolsBox-1.0.8/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     3749 2024-04-06 19:52:25.102993 PygameToolsBox-1.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 19:52:25.063366 PygameToolsBox-1.0.8/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-04-06 19:52:11.000000 PygameToolsBox-1.0.8/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     5025 2024-04-06 19:48:59.000000 PygameToolsBox-1.0.8/PygameToolsBox/animated_object.py
--rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.8/PygameToolsBox/mask_image.py
--rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.8/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.0.8/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-04-06 19:52:25.091991 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     3749 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-04-06 19:52:25.000000 PygameToolsBox-1.0.8/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3143 2024-04-06 19:50:04.000000 PygameToolsBox-1.0.8/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 19:52:25.105805 PygameToolsBox-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-06 19:59:33.634513 PygameToolsBox-1.0.9/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     3749 2024-04-06 19:59:33.631013 PygameToolsBox-1.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 19:59:33.603013 PygameToolsBox-1.0.9/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-06 19:59:11.000000 PygameToolsBox-1.0.9/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     5057 2024-04-06 19:58:03.000000 PygameToolsBox-1.0.9/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.9/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.9/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3696 2024-04-06 19:08:25.000000 PygameToolsBox-1.0.9/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-06 19:59:33.630013 PygameToolsBox-1.0.9/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     3749 2024-04-06 19:59:33.000000 PygameToolsBox-1.0.9/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-06 19:59:33.000000 PygameToolsBox-1.0.9/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 19:59:33.000000 PygameToolsBox-1.0.9/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-06 19:59:33.000000 PygameToolsBox-1.0.9/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-06 19:59:33.000000 PygameToolsBox-1.0.9/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3143 2024-04-06 19:50:04.000000 PygameToolsBox-1.0.9/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-06 19:59:33.634513 PygameToolsBox-1.0.9/setup.cfg
```

### Comparing `PygameToolsBox-1.0.8/LICENSE` & `PygameToolsBox-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.8/PKG-INFO` & `PygameToolsBox-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.8/PygameToolsBox/animated_object.py` & `PygameToolsBox-1.0.9/PygameToolsBox/animated_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 class AnimatedObject:
     def __init__(self, images: [Surface], cooling: int):
         """
         Automate animation of game object, You can specify different action to object and switch
         between these actions to switch animation sequence.
-        :param images: All the image nedded for the object
+        :param images: All the image needed for the object
         :param cooling: Frames spacing between switching image
         """
         self.images = [MaskImage(i) for i in images]
         self._actions = dict[str, ActionSequence]()
         self._current_action: ActionSequence | None = None
         self._current_image = self.images[0]
         self.cooling = cooling
@@ -120,21 +120,21 @@
             self._current_image = None
 
     def is_collide_with(self, other: MaskImage):
         """
         :param other: The other object (sprite) to test collision
         :return: True if the object is colliding with another object else return False
         """
-        self._current_image.rect.center = self._pos
+        self._current_image.rect.center = (self._pos.x, self.pos.y)
         if self._current_image and pygame.sprite.collide_rect(self._current_image, other):
             if pygame.sprite.collide_mask(self._current_image, other):
                 return True
         return False
 
     def draw(self, win: Surface):
         """
         Display object to the screen
         :param win: Surface to draw
         """
         if self._current_image:
-            self._current_image.rect.center = self._pos
+            self._current_image.rect.center = (self._pos.x, self.pos.y)
             win.blit(self._current_image.image, self._current_image.rect)
```

### Comparing `PygameToolsBox-1.0.8/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.0.9/PygameToolsBox/parallax_bg.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.8/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.0.9/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.8/PygameToolsBox.egg-info/PKG-INFO` & `PygameToolsBox-1.0.9/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.8
+Version: 1.0.9
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.8/README.md` & `PygameToolsBox-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.8/pyproject.toml` & `PygameToolsBox-1.0.9/pyproject.toml`

 * *Files identical despite different names*

