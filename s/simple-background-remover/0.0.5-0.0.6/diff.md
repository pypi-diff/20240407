# Comparing `tmp/simple_background_remover-0.0.5.tar.gz` & `tmp/simple_background_remover-0.0.6.tar.gz`

## Comparing `simple_background_remover-0.0.5.tar` & `simple_background_remover-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/src/simple_background_remover/__init__.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/src/simple_background_remover/color_helper.py
--rw-r--r--   0        0        0     4161 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/src/simple_background_remover/simple_background_remover.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/LICENSE
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/README.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 simple_background_remover-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0   351776 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/demos/Apple-0.2.png
+-rw-r--r--   0        0        0    63996 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/demos/Apple.jpg
+-rw-r--r--   0        0        0   195567 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/demos/Shirt-0.094.png
+-rw-r--r--   0        0        0    49497 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/demos/Shirt.jpg
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/src/simple_background_remover/__init__.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/src/simple_background_remover/color_helper.py
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/src/simple_background_remover/simple_background_remover.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/LICENSE
+-rw-r--r--   0        0        0     3560 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 simple_background_remover-0.0.6/PKG-INFO
```

### Comparing `simple_background_remover-0.0.5/.github/workflows/python-publish.yml` & `simple_background_remover-0.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.5/src/simple_background_remover/color_helper.py` & `simple_background_remover-0.0.6/src/simple_background_remover/color_helper.py`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.5/src/simple_background_remover/simple_background_remover.py` & `simple_background_remover-0.0.6/src/simple_background_remover/simple_background_remover.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     for pixel_data in image_data:
         if helper.is_close_to_background(pixel_data[0], pixel_data[1], pixel_data[2]):
             new_data.append(helper.TRANSPARENT_COLOR)
         else:
             new_data.append(pixel_data)
 
     image.putdata(new_data)
-    file_name = f'{output_filename}-{round(helper.get_wiggle_room(), 3)}.png'
+    file_name = f'{output_filename}.png'
     image.save(file_name, "PNG")
     print(f'Image saved: \'{file_name}\'')
             
 
 def __get_determined_background_color(image: Image.Image) -> tuple[int, int, int]:
     """
     Determines the solid background color of an image by looking at
```

### Comparing `simple_background_remover-0.0.5/.gitignore` & `simple_background_remover-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.5/LICENSE` & `simple_background_remover-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.5/README.md` & `simple_background_remover-0.0.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 # simple_background_remover
 This library is meant to be a quick and dirty background remover for simple images with solid(ish) background colors. Basically, a green screen. It does not have any sort of 'foreground detection'; it simply transparent-ifies pixels which are similar to the provided (or determined) background color.
 
 The processed files automatically get saved as PNGs.
 
+#### Installation
+This library is [available on PyPi](https://pypi.org/project/simple-background-remover/) and can be installed with `python -m pip install simple_background_remover`.
+
 #### Usage
 ```python
-from simple_background_remover import remove_background
+from simple_background_remover import *
+
+simple_background_remover.remove_background(input_filename='images/myPhoto.jpg',
+                                            output_filename='images/processed/myPhoto', # Note no file extension
+                                            wiggle_room=0.15, 
+                                            background_color=(0, 0, 0))
 
+# Alternatively
+from simple_background_remover.simple_background_remover import remove_background
 remove_background(input_filename='images/myPhoto.jpg',
-                  output_filename='images/processed/myPhoto', 
+                  output_filename='images/processed/myPhoto', # Note no file extension
                   wiggle_room=0.15, 
                   background_color=(0, 0, 0))
 ```
 
 #### wiggle_room
 `wiggle_room` is an optional parameter between 0 and 1. It determines how similar a pixels color can be to the background color and still be considered 'background'. For example, a value of 0.2 means that pixels can be +/- 20% similar to the background color and still be considered background pixels, and therefore made transparents. Note: This 20% range is applied to the R, G, and B value of the background color, so it's not perfect. Ideally it would use [redmean/Euclidean distance](https://en.wikipedia.org/wiki/Color_difference) like the auto-generated `wiggle_room` (more on that below) uses.
 
 If wiggle_room is not passed/left as `None`, the wiggle room will be auto-determined by roughly calculating the contrast between the average foreground and background color. The larger the contrast (i.e. foreground black, background white), the higher `wiggle_room` can be. The smaller the constrast (i.e. foreground black, background dark gray), the lower `wiggle_room` must be, otherwise you risk accidentally transparent-ifying foreground pixels.
 
 #### background_color
 `background_color` is an optional parameter for the background color of the image (passed as an RGB color, as `tuple[int, int, int]` -- i.e. (0, 0, 0) for white). If not passed `background_color` will be estimated based on the average color of the top left 5% of the image. Ideally this could be flexible for the caller in the future. 
 
 #### Examples
- - To do: post some images
+ - See the demos folder for some examples. The Shirt was done with auto wiggle room and background determination, and worked almost perfectly. The Apple has some bleed over. The library originally tried a wiggle room of ~0.37, but there was way too much bleed over, so I manually set it to 0.2
 
 ---
 ## Todo
 Lots more can be done to improve this repo. 
  - General clean up -- I wrote this pretty quickly and many places could be cleaned up/refactored
+ - Add print statements if argument passed into `remove_background`
  - Validation on user inputs
  - Improvements on the auto determination of background color and wiggle room
    - Could use the redmean to determine the closeness to background per pixel instead of doing +/- wiggle room -- although may be very slow
    - Allow user to pass in which corner to read background from
```

### Comparing `simple_background_remover-0.0.5/pyproject.toml` & `simple_background_remover-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple_background_remover"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="oversizedcanoe" },
 ]
 description = "A quick and dirty background remover for simple images with solid(ish) background colors."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_background_remover-0.0.5/PKG-INFO` & `simple_background_remover-0.0.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simple_background_remover
-Version: 0.0.5
+Version: 0.0.6
 Summary: A quick and dirty background remover for simple images with solid(ish) background colors.
 Project-URL: Homepage, https://github.com/oversizedcanoe/simple_background_remover 
 Author: oversizedcanoe
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -13,36 +13,47 @@
 Description-Content-Type: text/markdown
 
 # simple_background_remover
 This library is meant to be a quick and dirty background remover for simple images with solid(ish) background colors. Basically, a green screen. It does not have any sort of 'foreground detection'; it simply transparent-ifies pixels which are similar to the provided (or determined) background color.
 
 The processed files automatically get saved as PNGs.
 
+#### Installation
+This library is [available on PyPi](https://pypi.org/project/simple-background-remover/) and can be installed with `python -m pip install simple_background_remover`.
+
 #### Usage
 ```python
-from simple_background_remover import remove_background
+from simple_background_remover import *
+
+simple_background_remover.remove_background(input_filename='images/myPhoto.jpg',
+                                            output_filename='images/processed/myPhoto', # Note no file extension
+                                            wiggle_room=0.15, 
+                                            background_color=(0, 0, 0))
 
+# Alternatively
+from simple_background_remover.simple_background_remover import remove_background
 remove_background(input_filename='images/myPhoto.jpg',
-                  output_filename='images/processed/myPhoto', 
+                  output_filename='images/processed/myPhoto', # Note no file extension
                   wiggle_room=0.15, 
                   background_color=(0, 0, 0))
 ```
 
 #### wiggle_room
 `wiggle_room` is an optional parameter between 0 and 1. It determines how similar a pixels color can be to the background color and still be considered 'background'. For example, a value of 0.2 means that pixels can be +/- 20% similar to the background color and still be considered background pixels, and therefore made transparents. Note: This 20% range is applied to the R, G, and B value of the background color, so it's not perfect. Ideally it would use [redmean/Euclidean distance](https://en.wikipedia.org/wiki/Color_difference) like the auto-generated `wiggle_room` (more on that below) uses.
 
 If wiggle_room is not passed/left as `None`, the wiggle room will be auto-determined by roughly calculating the contrast between the average foreground and background color. The larger the contrast (i.e. foreground black, background white), the higher `wiggle_room` can be. The smaller the constrast (i.e. foreground black, background dark gray), the lower `wiggle_room` must be, otherwise you risk accidentally transparent-ifying foreground pixels.
 
 #### background_color
 `background_color` is an optional parameter for the background color of the image (passed as an RGB color, as `tuple[int, int, int]` -- i.e. (0, 0, 0) for white). If not passed `background_color` will be estimated based on the average color of the top left 5% of the image. Ideally this could be flexible for the caller in the future. 
 
 #### Examples
- - To do: post some images
+ - See the demos folder for some examples. The Shirt was done with auto wiggle room and background determination, and worked almost perfectly. The Apple has some bleed over. The library originally tried a wiggle room of ~0.37, but there was way too much bleed over, so I manually set it to 0.2
 
 ---
 ## Todo
 Lots more can be done to improve this repo. 
  - General clean up -- I wrote this pretty quickly and many places could be cleaned up/refactored
+ - Add print statements if argument passed into `remove_background`
  - Validation on user inputs
  - Improvements on the auto determination of background color and wiggle room
    - Could use the redmean to determine the closeness to background per pixel instead of doing +/- wiggle room -- although may be very slow
    - Allow user to pass in which corner to read background from
```

