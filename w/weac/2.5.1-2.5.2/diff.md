# Comparing `tmp/weac-2.5.1.tar.gz` & `tmp/weac-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weac-2.5.1.tar", last modified: Thu Apr  4 12:40:05 2024, max compression
+gzip compressed data, was "weac-2.5.2.tar", last modified: Sun Apr  7 11:07:26 2024, max compression
```

## Comparing `weac-2.5.1.tar` & `weac-2.5.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.962766 weac-2.5.1/
--rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-04 12:39:52.000000 weac-2.5.1/CITATION.cff
--rw-r--r--   0 runner     (501) staff       (20)      129 2024-04-04 12:39:52.000000 weac-2.5.1/LICENSE
--rw-r--r--   0 runner     (501) staff       (20)       39 2024-04-04 12:39:52.000000 weac-2.5.1/MANIFEST.in
--rw-r--r--   0 runner     (501) staff       (20)    17289 2024-04-04 12:40:05.962499 weac-2.5.1/PKG-INFO
--rw-r--r--   0 runner     (501) staff       (20)    16462 2024-04-04 12:39:52.000000 weac-2.5.1/README.md
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.950802 weac-2.5.1/build/
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.961659 weac-2.5.1/build/weac.egg-info/
--rw-r--r--   0 runner     (501) staff       (20)      266 2024-04-04 12:40:05.000000 weac-2.5.1/build/weac.egg-info/SOURCES.txt
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.958370 weac-2.5.1/img/
--rw-r--r--   0 runner     (501) staff       (20)    70202 2024-04-04 12:39:52.000000 weac-2.5.1/img/bc.png
--rw-r--r--   0 runner     (501) staff       (20)    17056 2024-04-04 12:39:52.000000 weac-2.5.1/img/layering.png
--rw-r--r--   0 runner     (501) staff       (20)    82279 2024-04-04 12:39:52.000000 weac-2.5.1/img/logo.png
--rw-r--r--   0 runner     (501) staff       (20)    37795 2024-04-04 12:39:52.000000 weac-2.5.1/img/model.png
--rw-r--r--   0 runner     (501) staff       (20)    69175 2024-04-04 12:39:52.000000 weac-2.5.1/img/profiles.png
--rw-r--r--   0 runner     (501) staff       (20)    30453 2024-04-04 12:39:52.000000 weac-2.5.1/img/systems.png
--rw-r--r--   0 runner     (501) staff       (20)      184 2024-04-04 12:39:52.000000 weac-2.5.1/pyproject.toml
--rw-r--r--   0 runner     (501) staff       (20)      988 2024-04-04 12:40:05.963817 weac-2.5.1/setup.cfg
-drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-04 12:40:05.961254 weac-2.5.1/weac/
--rw-r--r--   0 runner     (501) staff       (20)      359 2024-04-04 12:39:52.000000 weac-2.5.1/weac/__init__.py
--rw-r--r--   0 runner     (501) staff       (20)    22476 2024-04-04 12:39:52.000000 weac-2.5.1/weac/eigensystem.py
--rw-r--r--   0 runner     (501) staff       (20)     1980 2024-04-04 12:39:52.000000 weac-2.5.1/weac/inverse.py
--rwxr-xr-x   0 runner     (501) staff       (20)     2064 2024-04-04 12:39:52.000000 weac-2.5.1/weac/layered.py
--rw-r--r--   0 runner     (501) staff       (20)    70269 2024-04-04 12:39:52.000000 weac-2.5.1/weac/mixins.py
--rw-r--r--   0 runner     (501) staff       (20)    20705 2024-04-04 12:39:52.000000 weac-2.5.1/weac/plot.py
--rw-r--r--   0 runner     (501) staff       (20)     9605 2024-04-04 12:39:52.000000 weac-2.5.1/weac/tools.py
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-07 11:07:26.048859 weac-2.5.2/
+-rw-r--r--   0 runner     (501) staff       (20)     1589 2024-04-07 11:07:06.000000 weac-2.5.2/CITATION.cff
+-rw-r--r--   0 runner     (501) staff       (20)      129 2024-04-07 11:07:06.000000 weac-2.5.2/LICENSE
+-rw-r--r--   0 runner     (501) staff       (20)       39 2024-04-07 11:07:06.000000 weac-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner     (501) staff       (20)    17629 2024-04-07 11:07:26.048579 weac-2.5.2/PKG-INFO
+-rw-r--r--   0 runner     (501) staff       (20)    16802 2024-04-07 11:07:06.000000 weac-2.5.2/README.md
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-07 11:07:26.035620 weac-2.5.2/build/
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-07 11:07:26.047572 weac-2.5.2/build/weac.egg-info/
+-rw-r--r--   0 runner     (501) staff       (20)      266 2024-04-07 11:07:26.000000 weac-2.5.2/build/weac.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-07 11:07:26.043063 weac-2.5.2/img/
+-rw-r--r--   0 runner     (501) staff       (20)    70202 2024-04-07 11:07:06.000000 weac-2.5.2/img/bc.png
+-rw-r--r--   0 runner     (501) staff       (20)    17056 2024-04-07 11:07:06.000000 weac-2.5.2/img/layering.png
+-rw-r--r--   0 runner     (501) staff       (20)    82279 2024-04-07 11:07:06.000000 weac-2.5.2/img/logo.png
+-rw-r--r--   0 runner     (501) staff       (20)    37795 2024-04-07 11:07:06.000000 weac-2.5.2/img/model.png
+-rw-r--r--   0 runner     (501) staff       (20)    69175 2024-04-07 11:07:06.000000 weac-2.5.2/img/profiles.png
+-rw-r--r--   0 runner     (501) staff       (20)    30453 2024-04-07 11:07:06.000000 weac-2.5.2/img/systems.png
+-rw-r--r--   0 runner     (501) staff       (20)      184 2024-04-07 11:07:06.000000 weac-2.5.2/pyproject.toml
+-rw-r--r--   0 runner     (501) staff       (20)      988 2024-04-07 11:07:26.049910 weac-2.5.2/setup.cfg
+drwxr-xr-x   0 runner     (501) staff       (20)        0 2024-04-07 11:07:26.047075 weac-2.5.2/weac/
+-rw-r--r--   0 runner     (501) staff       (20)      359 2024-04-07 11:07:06.000000 weac-2.5.2/weac/__init__.py
+-rw-r--r--   0 runner     (501) staff       (20)    22476 2024-04-07 11:07:06.000000 weac-2.5.2/weac/eigensystem.py
+-rw-r--r--   0 runner     (501) staff       (20)     1980 2024-04-07 11:07:06.000000 weac-2.5.2/weac/inverse.py
+-rwxr-xr-x   0 runner     (501) staff       (20)     2064 2024-04-07 11:07:06.000000 weac-2.5.2/weac/layered.py
+-rw-r--r--   0 runner     (501) staff       (20)    70269 2024-04-07 11:07:06.000000 weac-2.5.2/weac/mixins.py
+-rw-r--r--   0 runner     (501) staff       (20)    20705 2024-04-07 11:07:06.000000 weac-2.5.2/weac/plot.py
+-rw-r--r--   0 runner     (501) staff       (20)     9961 2024-04-07 11:07:06.000000 weac-2.5.2/weac/tools.py
```

### Comparing `weac-2.5.1/CITATION.cff` & `weac-2.5.2/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 authors:
 - family-names: "Rosendahl"
   given-names: "Philipp Laurens"
   orcid: "https://orcid.org/0000-0002-6587-875X"
 - family-names: "Weissgraeber"
   given-names: "Philipp"
   orcid: "https://orcid.org/0000-0001-8320-8672"
-version: 2.5.1
+version: 2.5.2
 date-released: 2021-12-30
 identifiers:
   - description: Collection of archived snapshots of all versions of WEAC
     type: doi
     value: 10.5281/zenodo.5773113
   - description: Release v2.4 for the analysis of slope-normal and vertical PST boundary conditions
     type: doi
```

### Comparing `weac-2.5.1/PKG-INFO` & `weac-2.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weac
-Version: 2.5.1
+Version: 2.5.2
 Summary: Weak layer anticrack nucleation model
 Home-page: https://github.com/2phi/weac
 Author: 2phi GbR
 Author-email: mail@2phi.de
 License: Proprietary
 Project-URL: Demo, https://github.com/2phi/weac/blob/main/demo/demo.ipynb
 Project-URL: Documentation, https://2phi.github.io/weac
@@ -209,23 +209,33 @@
 ```
 
 <!-- ROADMAP -->
 ## Roadmap
 
 See the [open issues](https://github.com/2phi/weac/issues) for a list of proposed features and known issues.
 
-### v2.6
+### v3.0
+
+- [ ] New mathematical foundation to improve the weak-layer representation
+- [ ] Complex terrain through the addition of out-of-plane tilt
+- [ ] Up, down, and cross-slope cracks
+
+### v2.7
 - [ ] Finite fracture mechanics implementation for layered snow covers
 
-### v2.5
+### v2.6
 - [ ] Implement anistropic weak layer
 - [ ] Add demo gif
 
 ## Release history
 
+### v2.5
+- Analyze slab touchdown in PST experiments by setting `touchdown=True`
+- Completely redesigned and significantly improved API documentation
+
 ### v2.4
 - Choose between slope-normal (`'-pst'`, `'pst-'`) or vertial (`'-vpst'`, `'vpst-'`) PST boundary conditions
 
 ### v2.3
 - Stress plots on deformed contours
 - PSTs now account for slab touchdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: weac Version: 2.5.1 Summary: Weak layer anticrack
+Metadata-Version: 2.1 Name: weac Version: 2.5.2 Summary: Weak layer anticrack
 nucleation model Home-page: https://github.com/2phi/weac Author: 2phi GbR
 Author-email: mail@2phi.de License: Proprietary Project-URL: Demo, https://
 github.com/2phi/weac/blob/main/demo/demo.ipynb Project-URL: Documentation,
 https://2phi.github.io/weac Project-URL: Issues and feature requests, https://
 github.com/2phi/weac/issues Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Scientific/Engineering Requires-Python:
@@ -89,41 +89,46 @@
 Plot weak-layer stresses (using only x-coordinates of bedded segments, xwl)
 weac.plot.stresses(skier, x=xwl, z=z, **segments) ``` Compute output quantities
 for exporting or plotting. ```python # Slab deflections (using x-coordinates of
 all segments, xsl) x_cm, w_um = skier.get_slab_deflection(x=xsl, z=z,
 unit='um') # Weak-layer shear stress (using only x-coordinates of bedded
 segments, xwl) x_cm, tau_kPa = skier.get_weaklayer_shearstress(x=xwl, z=z,
 unit='kPa') ``` ## Roadmap See the [open issues](https://github.com/2phi/weac/
-issues) for a list of proposed features and known issues. ### v2.6 - [ ] Finite
-fracture mechanics implementation for layered snow covers ### v2.5 - [ ]
-Implement anistropic weak layer - [ ] Add demo gif ## Release history ### v2.4
-- Choose between slope-normal (`'-pst'`, `'pst-'`) or vertial (`'-vpst'`,
-`'vpst-'`) PST boundary conditions ### v2.3 - Stress plots on deformed contours
-- PSTs now account for slab touchdown ### v2.2 - Sign of inclination `phi`
-consistent with the coordinate system (positive counterclockwise) - Dimension
-arguments to field-quantity methods added - Improved aspect ratio of profile
-views and contour plots - Improved plot labels - Convenience methods for the
-export of weak-layer stresses and slab deformations provided - Wrapper for
-(re)calculation of the fundamental system added - Now allows for distributed
-surface loads ### v2.1 - Consistent use of coordinate system with downward
-pointing z-axis - Consitent top-to-bottom numbering of slab layers -
-Implementation of PSTs cut from either left or right side ### v2.0 - Completely
-rewritten in ð Python - Coupled bending-extension ODE solver implemented -
-Stress analysis of arbitrarily layered snow slabs - FEM validation of -
-displacements - weak-layer stresses - energy release rates in weak layers -
-Documentation - Demo and examples ### v1.0 - Written in ð MATLAB -
-Deformation analysis of homogeneous snow labs - Weak-layer stress prediction -
-Energy release rates of cracks in weak layers - Finite fracture mechanics
-implementation - Prediction of anticrack nucleation ## How to contribute 1.
-Fork the project 2. Create your feature branch (`git checkout -b feature/
-amazingfeature`) 3. Commit your changes (`git commit -m 'Add some amazing
-feature'`) 4. Push to the branch (`git push origin feature/amazingfeature`) 5.
-Open a pull request ## Workflows [![Publish Python ð releases ð¦ to PyPI ]
-(https://github.com/2phi/weac/actions/workflows/release.yml/badge.svg)](https:/
-/github.com/2phi/weac/actions/workflows/release.yml)
+issues) for a list of proposed features and known issues. ### v3.0 - [ ] New
+mathematical foundation to improve the weak-layer representation - [ ] Complex
+terrain through the addition of out-of-plane tilt - [ ] Up, down, and cross-
+slope cracks ### v2.7 - [ ] Finite fracture mechanics implementation for
+layered snow covers ### v2.6 - [ ] Implement anistropic weak layer - [ ] Add
+demo gif ## Release history ### v2.5 - Analyze slab touchdown in PST
+experiments by setting `touchdown=True` - Completely redesigned and
+significantly improved API documentation ### v2.4 - Choose between slope-normal
+(`'-pst'`, `'pst-'`) or vertial (`'-vpst'`, `'vpst-'`) PST boundary conditions
+### v2.3 - Stress plots on deformed contours - PSTs now account for slab
+touchdown ### v2.2 - Sign of inclination `phi` consistent with the coordinate
+system (positive counterclockwise) - Dimension arguments to field-quantity
+methods added - Improved aspect ratio of profile views and contour plots -
+Improved plot labels - Convenience methods for the export of weak-layer
+stresses and slab deformations provided - Wrapper for (re)calculation of the
+fundamental system added - Now allows for distributed surface loads ### v2.1 -
+Consistent use of coordinate system with downward pointing z-axis - Consitent
+top-to-bottom numbering of slab layers - Implementation of PSTs cut from either
+left or right side ### v2.0 - Completely rewritten in ð Python - Coupled
+bending-extension ODE solver implemented - Stress analysis of arbitrarily
+layered snow slabs - FEM validation of - displacements - weak-layer stresses -
+energy release rates in weak layers - Documentation - Demo and examples ###
+v1.0 - Written in ð MATLAB - Deformation analysis of homogeneous snow labs -
+Weak-layer stress prediction - Energy release rates of cracks in weak layers -
+Finite fracture mechanics implementation - Prediction of anticrack nucleation
+## How to contribute 1. Fork the project 2. Create your feature branch (`git
+checkout -b feature/amazingfeature`) 3. Commit your changes (`git commit -
+m 'Add some amazing feature'`) 4. Push to the branch (`git push origin feature/
+amazingfeature`) 5. Open a pull request ## Workflows [![Publish Python ð
+releases ð¦ to PyPI ](https://github.com/2phi/weac/actions/workflows/
+release.yml/badge.svg)](https://github.com/2phi/weac/actions/workflows/
+release.yml)
 [![Build and publish Sphinx ðª¬ documentation ](https://github.com/2phi/weac/
 actions/workflows/docs.yml/badge.svg)](https://github.com/2phi/weac/actions/
 workflows/docs.yml) ## License Copyright 2phi GbR, 2020-2024. We currently do
 not offer an open-source license. Please contact us for private licensing
 options. ## Contact E-mail: mail@2phi.de Â· Web: https://2phi.de Â· Project
 Link: [https://github.com/2phi/weac](https://github.com/2phi/weac) Â· Project
 DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://dx.doi.org/10.5281/
```

### Comparing `weac-2.5.1/README.md` & `weac-2.5.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -185,23 +185,33 @@
 ```
 
 <!-- ROADMAP -->
 ## Roadmap
 
 See the [open issues](https://github.com/2phi/weac/issues) for a list of proposed features and known issues.
 
-### v2.6
+### v3.0
+
+- [ ] New mathematical foundation to improve the weak-layer representation
+- [ ] Complex terrain through the addition of out-of-plane tilt
+- [ ] Up, down, and cross-slope cracks
+
+### v2.7
 - [ ] Finite fracture mechanics implementation for layered snow covers
 
-### v2.5
+### v2.6
 - [ ] Implement anistropic weak layer
 - [ ] Add demo gif
 
 ## Release history
 
+### v2.5
+- Analyze slab touchdown in PST experiments by setting `touchdown=True`
+- Completely redesigned and significantly improved API documentation
+
 ### v2.4
 - Choose between slope-normal (`'-pst'`, `'pst-'`) or vertial (`'-vpst'`, `'vpst-'`) PST boundary conditions
 
 ### v2.3
 - Stress plots on deformed contours
 - PSTs now account for slab touchdown
```

#### html2text {}

```diff
@@ -78,41 +78,46 @@
 Plot weak-layer stresses (using only x-coordinates of bedded segments, xwl)
 weac.plot.stresses(skier, x=xwl, z=z, **segments) ``` Compute output quantities
 for exporting or plotting. ```python # Slab deflections (using x-coordinates of
 all segments, xsl) x_cm, w_um = skier.get_slab_deflection(x=xsl, z=z,
 unit='um') # Weak-layer shear stress (using only x-coordinates of bedded
 segments, xwl) x_cm, tau_kPa = skier.get_weaklayer_shearstress(x=xwl, z=z,
 unit='kPa') ``` ## Roadmap See the [open issues](https://github.com/2phi/weac/
-issues) for a list of proposed features and known issues. ### v2.6 - [ ] Finite
-fracture mechanics implementation for layered snow covers ### v2.5 - [ ]
-Implement anistropic weak layer - [ ] Add demo gif ## Release history ### v2.4
-- Choose between slope-normal (`'-pst'`, `'pst-'`) or vertial (`'-vpst'`,
-`'vpst-'`) PST boundary conditions ### v2.3 - Stress plots on deformed contours
-- PSTs now account for slab touchdown ### v2.2 - Sign of inclination `phi`
-consistent with the coordinate system (positive counterclockwise) - Dimension
-arguments to field-quantity methods added - Improved aspect ratio of profile
-views and contour plots - Improved plot labels - Convenience methods for the
-export of weak-layer stresses and slab deformations provided - Wrapper for
-(re)calculation of the fundamental system added - Now allows for distributed
-surface loads ### v2.1 - Consistent use of coordinate system with downward
-pointing z-axis - Consitent top-to-bottom numbering of slab layers -
-Implementation of PSTs cut from either left or right side ### v2.0 - Completely
-rewritten in ð Python - Coupled bending-extension ODE solver implemented -
-Stress analysis of arbitrarily layered snow slabs - FEM validation of -
-displacements - weak-layer stresses - energy release rates in weak layers -
-Documentation - Demo and examples ### v1.0 - Written in ð MATLAB -
-Deformation analysis of homogeneous snow labs - Weak-layer stress prediction -
-Energy release rates of cracks in weak layers - Finite fracture mechanics
-implementation - Prediction of anticrack nucleation ## How to contribute 1.
-Fork the project 2. Create your feature branch (`git checkout -b feature/
-amazingfeature`) 3. Commit your changes (`git commit -m 'Add some amazing
-feature'`) 4. Push to the branch (`git push origin feature/amazingfeature`) 5.
-Open a pull request ## Workflows [![Publish Python ð releases ð¦ to PyPI ]
-(https://github.com/2phi/weac/actions/workflows/release.yml/badge.svg)](https:/
-/github.com/2phi/weac/actions/workflows/release.yml)
+issues) for a list of proposed features and known issues. ### v3.0 - [ ] New
+mathematical foundation to improve the weak-layer representation - [ ] Complex
+terrain through the addition of out-of-plane tilt - [ ] Up, down, and cross-
+slope cracks ### v2.7 - [ ] Finite fracture mechanics implementation for
+layered snow covers ### v2.6 - [ ] Implement anistropic weak layer - [ ] Add
+demo gif ## Release history ### v2.5 - Analyze slab touchdown in PST
+experiments by setting `touchdown=True` - Completely redesigned and
+significantly improved API documentation ### v2.4 - Choose between slope-normal
+(`'-pst'`, `'pst-'`) or vertial (`'-vpst'`, `'vpst-'`) PST boundary conditions
+### v2.3 - Stress plots on deformed contours - PSTs now account for slab
+touchdown ### v2.2 - Sign of inclination `phi` consistent with the coordinate
+system (positive counterclockwise) - Dimension arguments to field-quantity
+methods added - Improved aspect ratio of profile views and contour plots -
+Improved plot labels - Convenience methods for the export of weak-layer
+stresses and slab deformations provided - Wrapper for (re)calculation of the
+fundamental system added - Now allows for distributed surface loads ### v2.1 -
+Consistent use of coordinate system with downward pointing z-axis - Consitent
+top-to-bottom numbering of slab layers - Implementation of PSTs cut from either
+left or right side ### v2.0 - Completely rewritten in ð Python - Coupled
+bending-extension ODE solver implemented - Stress analysis of arbitrarily
+layered snow slabs - FEM validation of - displacements - weak-layer stresses -
+energy release rates in weak layers - Documentation - Demo and examples ###
+v1.0 - Written in ð MATLAB - Deformation analysis of homogeneous snow labs -
+Weak-layer stress prediction - Energy release rates of cracks in weak layers -
+Finite fracture mechanics implementation - Prediction of anticrack nucleation
+## How to contribute 1. Fork the project 2. Create your feature branch (`git
+checkout -b feature/amazingfeature`) 3. Commit your changes (`git commit -
+m 'Add some amazing feature'`) 4. Push to the branch (`git push origin feature/
+amazingfeature`) 5. Open a pull request ## Workflows [![Publish Python ð
+releases ð¦ to PyPI ](https://github.com/2phi/weac/actions/workflows/
+release.yml/badge.svg)](https://github.com/2phi/weac/actions/workflows/
+release.yml)
 [![Build and publish Sphinx ðª¬ documentation ](https://github.com/2phi/weac/
 actions/workflows/docs.yml/badge.svg)](https://github.com/2phi/weac/actions/
 workflows/docs.yml) ## License Copyright 2phi GbR, 2020-2024. We currently do
 not offer an open-source license. Please contact us for private licensing
 options. ## Contact E-mail: mail@2phi.de Â· Web: https://2phi.de Â· Project
 Link: [https://github.com/2phi/weac](https://github.com/2phi/weac) Â· Project
 DOI: [http://dx.doi.org/10.5281/zenodo.5773113](http://dx.doi.org/10.5281/
```

### Comparing `weac-2.5.1/img/bc.png` & `weac-2.5.2/img/bc.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/img/layering.png` & `weac-2.5.2/img/layering.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/img/logo.png` & `weac-2.5.2/img/logo.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/img/model.png` & `weac-2.5.2/img/model.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/img/profiles.png` & `weac-2.5.2/img/profiles.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/img/systems.png` & `weac-2.5.2/img/systems.png`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/setup.cfg` & `weac-2.5.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weac
-version = 2.5.1
+version = 2.5.2
 author = 2phi GbR
 author_email = mail@2phi.de
 description = Weak layer anticrack nucleation model
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/2phi/weac
 project_urls =
```

### Comparing `weac-2.5.1/weac/eigensystem.py` & `weac-2.5.2/weac/eigensystem.py`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/weac/inverse.py` & `weac-2.5.2/weac/inverse.py`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/weac/layered.py` & `weac-2.5.2/weac/layered.py`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/weac/mixins.py` & `weac-2.5.2/weac/mixins.py`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/weac/plot.py` & `weac-2.5.2/weac/plot.py`

 * *Files identical despite different names*

### Comparing `weac-2.5.1/weac/tools.py` & `weac-2.5.2/weac/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,14 +280,17 @@
     phi : float, optional
         Inclination of the slab (°). Default is 0.
         
     Returns
     -------
     first_contact : float
         Cut length at first contact (mm).
+    full_contact : float
+        Cut length at which the slab comes into full contact (more than
+        a singular point) with the base layer (mm).
     steady_state : float
         Steady-state touchdown distance (mm).
     """
     # Check if layering is defined
     layers = layers if layers else [[240, 200], ]
 
     # Initialize model with user input
@@ -298,14 +301,19 @@
     touchdown.set_beam_properties(layers=layers, C0=C0, C1=C1, update=True)
 
     # Assemble very long dummy PST to compute crack length where the slab
     # first comes in contact with base layer after weak-layer collapse
     touchdown.calc_segments(L=1e5, a=0, phi=phi)
     first_contact = touchdown.calc_a1()
 
+    # Compute ut length at which the slab comes into full contact (more
+    # than a singular point) with the base layer
+    full_contact = touchdown.calc_a2()
+
     # Compute steady-state touchdown distance in a dummy PST with a cut
     # of 5 times the first contact distance
     touchdown.calc_segments(L=1e5, a=5*first_contact, phi=phi)
     steady_state = touchdown.calc_lC()
 
-    # Return first-contact cut length and steady-state touchdown distance (mm)
-    return first_contact, steady_state
+    # Return first-contact cut length, full-contact cut length,
+    # and steady-state touchdown distance (mm)
+    return first_contact, full_contact, steady_state
```

