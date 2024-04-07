# Comparing `tmp/ColdTOFU-0.1.2.tar.gz` & `tmp/ColdTOFU-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ColdTOFU-0.1.2.tar", last modified: Thu Apr  4 03:58:38 2024, max compression
+gzip compressed data, was "ColdTOFU-0.1.3.tar", last modified: Sun Apr  7 04:09:18 2024, max compression
```

## Comparing `ColdTOFU-0.1.2.tar` & `ColdTOFU-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.486283 ColdTOFU-0.1.2/
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.483953 ColdTOFU-0.1.2/ColdTOFU/
--rw-r--r--   0 chetan     (501) staff       (20)   325120 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/ATSIFIO64.dll
--rw-r--r--   0 chetan     (501) staff       (20)    13142 2024-04-04 03:48:17.000000 ColdTOFU-0.1.2/ColdTOFU/AndorSifReader.py
--rw-r--r--   0 chetan     (501) staff       (20)      732 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/Helvetica_bright.mplstyle
--rw-r--r--   0 chetan     (501) staff       (20)    26925 2024-04-04 03:32:07.000000 ColdTOFU-0.1.2/ColdTOFU/Images.py
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.485679 ColdTOFU-0.1.2/ColdTOFU/Physics/
--rw-r--r--   0 chetan     (501) staff       (20)      143 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/__init__.py
--rw-r--r--   0 chetan     (501) staff       (20)     1863 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/allenDeviation.py
--rw-r--r--   0 chetan     (501) staff       (20)     3050 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/basisMatrices.py
--rw-r--r--   0 chetan     (501) staff       (20)     1125 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/beams.py
--rw-r--r--   0 chetan     (501) staff       (20)     1449 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/createAndDestroy.py
--rw-r--r--   0 chetan     (501) staff       (20)     4291 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/Physics/spinInDickeBasis.py
--rw-r--r--   0 chetan     (501) staff       (20)      224 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/__init__.py
--rw-r--r--   0 chetan     (501) staff       (20)    17659 2023-12-21 06:19:43.000000 ColdTOFU-0.1.2/ColdTOFU/fits.py
--rw-r--r--   0 chetan     (501) staff       (20)     1332 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/jupyterTools.py
--rw-r--r--   0 chetan     (501) staff       (20)     6439 2023-12-21 06:19:42.000000 ColdTOFU-0.1.2/ColdTOFU/numberOfAtoms.py
--rw-r--r--   0 chetan     (501) staff       (20)     2700 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/picoMatTools.py
--rw-r--r--   0 chetan     (501) staff       (20)      153 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/rcParams.json
--rw-r--r--   0 chetan     (501) staff       (20)      856 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/scientific_serif.mplstyle
--rw-r--r--   0 chetan     (501) staff       (20)     2694 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/ColdTOFU/sigma.py
--rw-r--r--   0 chetan     (501) staff       (20)    10352 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/ColdTOFU/spectrum.py
-drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-04 03:58:38.485929 ColdTOFU-0.1.2/ColdTOFU.egg-info/
--rw-r--r--   0 chetan     (501) staff       (20)      973 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/PKG-INFO
--rw-r--r--   0 chetan     (501) staff       (20)      695 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/SOURCES.txt
--rw-r--r--   0 chetan     (501) staff       (20)        1 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/dependency_links.txt
--rw-r--r--   0 chetan     (501) staff       (20)        9 2024-04-04 03:58:38.000000 ColdTOFU-0.1.2/ColdTOFU.egg-info/top_level.txt
--rw-r--r--   0 chetan     (501) staff       (20)     1068 2023-09-04 06:19:38.000000 ColdTOFU-0.1.2/LICENCE
--rw-r--r--   0 chetan     (501) staff       (20)       74 2023-12-21 06:19:46.000000 ColdTOFU-0.1.2/MANIFEST.in
--rw-r--r--   0 chetan     (501) staff       (20)      973 2024-04-04 03:58:38.486216 ColdTOFU-0.1.2/PKG-INFO
--rw-r--r--   0 chetan     (501) staff       (20)      508 2023-12-21 05:51:00.000000 ColdTOFU-0.1.2/README.md
--rw-r--r--   0 chetan     (501) staff       (20)      231 2024-04-04 03:58:00.000000 ColdTOFU-0.1.2/pyproject.toml
--rw-r--r--   0 chetan     (501) staff       (20)      656 2024-04-04 03:58:38.486564 ColdTOFU-0.1.2/setup.cfg
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-07 04:09:18.494607 ColdTOFU-0.1.3/
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-07 04:09:18.492402 ColdTOFU-0.1.3/ColdTOFU/
+-rw-r--r--   0 chetan     (501) staff       (20)   325120 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/ATSIFIO64.dll
+-rw-r--r--   0 chetan     (501) staff       (20)    13142 2024-04-04 03:48:17.000000 ColdTOFU-0.1.3/ColdTOFU/AndorSifReader.py
+-rw-r--r--   0 chetan     (501) staff       (20)      732 2023-12-21 05:51:00.000000 ColdTOFU-0.1.3/ColdTOFU/Helvetica_bright.mplstyle
+-rw-r--r--   0 chetan     (501) staff       (20)    26943 2024-04-05 08:06:25.000000 ColdTOFU-0.1.3/ColdTOFU/Images.py
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-07 04:09:18.494008 ColdTOFU-0.1.3/ColdTOFU/Physics/
+-rw-r--r--   0 chetan     (501) staff       (20)      143 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/Physics/__init__.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1863 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/Physics/allenDeviation.py
+-rw-r--r--   0 chetan     (501) staff       (20)     3050 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/Physics/basisMatrices.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1125 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/Physics/beams.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1449 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/Physics/createAndDestroy.py
+-rw-r--r--   0 chetan     (501) staff       (20)     4291 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/Physics/spinInDickeBasis.py
+-rw-r--r--   0 chetan     (501) staff       (20)      224 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/__init__.py
+-rw-r--r--   0 chetan     (501) staff       (20)    17659 2023-12-21 06:19:43.000000 ColdTOFU-0.1.3/ColdTOFU/fits.py
+-rw-r--r--   0 chetan     (501) staff       (20)     1332 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/jupyterTools.py
+-rw-r--r--   0 chetan     (501) staff       (20)     6439 2023-12-21 06:19:42.000000 ColdTOFU-0.1.3/ColdTOFU/numberOfAtoms.py
+-rw-r--r--   0 chetan     (501) staff       (20)     2700 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/picoMatTools.py
+-rw-r--r--   0 chetan     (501) staff       (20)      153 2023-12-21 05:51:00.000000 ColdTOFU-0.1.3/ColdTOFU/rcParams.json
+-rw-r--r--   0 chetan     (501) staff       (20)      856 2023-12-21 05:51:00.000000 ColdTOFU-0.1.3/ColdTOFU/scientific_serif.mplstyle
+-rw-r--r--   0 chetan     (501) staff       (20)     2694 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/ColdTOFU/sigma.py
+-rw-r--r--   0 chetan     (501) staff       (20)    10352 2023-12-21 05:51:00.000000 ColdTOFU-0.1.3/ColdTOFU/spectrum.py
+drwxr-xr-x   0 chetan     (501) staff       (20)        0 2024-04-07 04:09:18.494264 ColdTOFU-0.1.3/ColdTOFU.egg-info/
+-rw-r--r--   0 chetan     (501) staff       (20)      973 2024-04-07 04:09:18.000000 ColdTOFU-0.1.3/ColdTOFU.egg-info/PKG-INFO
+-rw-r--r--   0 chetan     (501) staff       (20)      695 2024-04-07 04:09:18.000000 ColdTOFU-0.1.3/ColdTOFU.egg-info/SOURCES.txt
+-rw-r--r--   0 chetan     (501) staff       (20)        1 2024-04-07 04:09:18.000000 ColdTOFU-0.1.3/ColdTOFU.egg-info/dependency_links.txt
+-rw-r--r--   0 chetan     (501) staff       (20)        9 2024-04-07 04:09:18.000000 ColdTOFU-0.1.3/ColdTOFU.egg-info/top_level.txt
+-rw-r--r--   0 chetan     (501) staff       (20)     1068 2023-09-04 06:19:38.000000 ColdTOFU-0.1.3/LICENCE
+-rw-r--r--   0 chetan     (501) staff       (20)       74 2023-12-21 06:19:46.000000 ColdTOFU-0.1.3/MANIFEST.in
+-rw-r--r--   0 chetan     (501) staff       (20)      973 2024-04-07 04:09:18.494528 ColdTOFU-0.1.3/PKG-INFO
+-rw-r--r--   0 chetan     (501) staff       (20)      508 2023-12-21 05:51:00.000000 ColdTOFU-0.1.3/README.md
+-rw-r--r--   0 chetan     (501) staff       (20)      231 2024-04-05 03:47:06.000000 ColdTOFU-0.1.3/pyproject.toml
+-rw-r--r--   0 chetan     (501) staff       (20)      656 2024-04-07 04:09:18.494896 ColdTOFU-0.1.3/setup.cfg
```

### Comparing `ColdTOFU-0.1.2/ColdTOFU/ATSIFIO64.dll` & `ColdTOFU-0.1.3/ColdTOFU/ATSIFIO64.dll`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/AndorSifReader.py` & `ColdTOFU-0.1.3/ColdTOFU/AndorSifReader.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/Helvetica_bright.mplstyle` & `ColdTOFU-0.1.3/ColdTOFU/Helvetica_bright.mplstyle`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/Images.py` & `ColdTOFU-0.1.3/ColdTOFU/Images.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         averagedOD: ndarray, OD of the averaged signal with averaging on superloop
         averagedOD2: ndarray, OD of the averaged signal with averaging on loop
     """
     def __init__(self, filePath):
         self.filePath = filePath
         self.ext = os.path.splitext(filePath)[1]
         if self.ext == '.tif':
-            self.im = Image.open(filePath)
+            self.im = Image.open(filePath, formats=['TIFF'])
             self.tags = self.im.tag.named()
         elif self.ext == '.sif':
             if sys.platform.startswith('win'):
                 from .AndorSifReader import AndorSifFile
                 self.im = AndorSifFile(filePath).signal
                 self.tags = self.im.props
                 self.frames = self.im.data
```

### Comparing `ColdTOFU-0.1.2/ColdTOFU/Physics/allenDeviation.py` & `ColdTOFU-0.1.3/ColdTOFU/Physics/allenDeviation.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/Physics/basisMatrices.py` & `ColdTOFU-0.1.3/ColdTOFU/Physics/basisMatrices.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/Physics/beams.py` & `ColdTOFU-0.1.3/ColdTOFU/Physics/beams.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/Physics/createAndDestroy.py` & `ColdTOFU-0.1.3/ColdTOFU/Physics/createAndDestroy.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/Physics/spinInDickeBasis.py` & `ColdTOFU-0.1.3/ColdTOFU/Physics/spinInDickeBasis.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/fits.py` & `ColdTOFU-0.1.3/ColdTOFU/fits.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/jupyterTools.py` & `ColdTOFU-0.1.3/ColdTOFU/jupyterTools.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/numberOfAtoms.py` & `ColdTOFU-0.1.3/ColdTOFU/numberOfAtoms.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/picoMatTools.py` & `ColdTOFU-0.1.3/ColdTOFU/picoMatTools.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/scientific_serif.mplstyle` & `ColdTOFU-0.1.3/ColdTOFU/scientific_serif.mplstyle`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/sigma.py` & `ColdTOFU-0.1.3/ColdTOFU/sigma.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU/spectrum.py` & `ColdTOFU-0.1.3/ColdTOFU/spectrum.py`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/ColdTOFU.egg-info/PKG-INFO` & `ColdTOFU-0.1.3/ColdTOFU.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColdTOFU
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cold Atoms Time-of-Flight Utilities
 Home-page: https://github.com/chetanmadasu/TOFU
 Author: Chetan Sriram Madasu
 Author-email: chetan.madasu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ColdTOFU-0.1.2/ColdTOFU.egg-info/SOURCES.txt` & `ColdTOFU-0.1.3/ColdTOFU.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/LICENCE` & `ColdTOFU-0.1.3/LICENCE`

 * *Files identical despite different names*

### Comparing `ColdTOFU-0.1.2/PKG-INFO` & `ColdTOFU-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ColdTOFU
-Version: 0.1.2
+Version: 0.1.3
 Summary: Cold Atoms Time-of-Flight Utilities
 Home-page: https://github.com/chetanmadasu/TOFU
 Author: Chetan Sriram Madasu
 Author-email: chetan.madasu@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ColdTOFU-0.1.2/setup.cfg` & `ColdTOFU-0.1.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ColdTOFU
-version = 0.1.2
+version = 0.1.3
 author = Chetan Sriram Madasu
 author_email = chetan.madasu@gmail.com
 description = Cold Atoms Time-of-Flight Utilities
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chetanmadasu/TOFU
 license = MIT License
```

