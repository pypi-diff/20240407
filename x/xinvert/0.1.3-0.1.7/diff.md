# Comparing `tmp/xinvert-0.1.3.tar.gz` & `tmp/xinvert-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xinvert-0.1.3.tar", last modified: Tue Aug 15 21:19:05 2023, max compression
+gzip compressed data, was "xinvert-0.1.7.tar", last modified: Sun Apr  7 09:34:52 2024, max compression
```

## Comparing `xinvert-0.1.3.tar` & `xinvert-0.1.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 21:19:05.041029 xinvert-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-15 21:18:52.000000 xinvert-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-08-15 21:19:05.041029 xinvert-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-08-15 21:18:52.000000 xinvert-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-15 21:19:05.045029 xinvert-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-15 21:18:52.000000 xinvert-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 21:19:05.041029 xinvert-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_3DOcean.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_AnimateConverge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_Bretherton.py
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_Eliassen.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_FDs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_Fofonoff.py
--rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_Geopotential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_GillMatsuno.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_HeldSuarezModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_Ishida.py
--rw-r--r--   0 runner    (1001) docker     (123)    11670 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_LLC4320Poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_MG.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_MunkWBC.py
--rw-r--r--   0 runner    (1001) docker     (123)    11897 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_OmegaEq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_OptArg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_Poisson.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_QGPV.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_RefStateSWM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_StommelArons.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_StommelWBC.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-15 21:18:52.000000 xinvert-0.1.3/tests/test_trace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 21:19:05.041029 xinvert-0.1.3/xinvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-08-15 21:18:52.000000 xinvert-0.1.3/xinvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    79443 2023-08-15 21:18:52.000000 xinvert-0.1.3/xinvert/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    20440 2023-08-15 21:18:52.000000 xinvert-0.1.3/xinvert/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    27428 2023-08-15 21:18:52.000000 xinvert-0.1.3/xinvert/finitediffs.py
--rw-r--r--   0 runner    (1001) docker     (123)    68730 2023-08-15 21:18:52.000000 xinvert-0.1.3/xinvert/numbas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-15 21:18:52.000000 xinvert-0.1.3/xinvert/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-15 21:19:05.041029 xinvert-0.1.3/xinvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-08-15 21:19:05.000000 xinvert-0.1.3/xinvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-15 21:19:05.000000 xinvert-0.1.3/xinvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-15 21:19:05.000000 xinvert-0.1.3/xinvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-15 21:19:05.000000 xinvert-0.1.3/xinvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-15 21:19:05.000000 xinvert-0.1.3/xinvert.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:34:52.477184 xinvert-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-07 09:34:48.000000 xinvert-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-07 09:34:52.477184 xinvert-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-07 09:34:48.000000 xinvert-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 09:34:52.477184 xinvert-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-07 09:34:48.000000 xinvert-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:34:52.477184 xinvert-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_3DOcean.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_AnimateConverge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_Bretherton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_Eliassen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_FDs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_Fofonoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10831 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_Geopotential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_GillMatsuno.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_HeldSuarezModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_Ishida.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_LLC4320Poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_MG.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_MunkWBC.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_OmegaEq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_OptArg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_Poisson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6531 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_QGPV.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_RefStateSWM.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_StommelArons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_StommelWBC.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-07 09:34:48.000000 xinvert-0.1.7/tests/test_trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:34:52.477184 xinvert-0.1.7/xinvert/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-07 09:34:48.000000 xinvert-0.1.7/xinvert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82342 2024-04-07 09:34:48.000000 xinvert-0.1.7/xinvert/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20481 2024-04-07 09:34:48.000000 xinvert-0.1.7/xinvert/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27645 2024-04-07 09:34:48.000000 xinvert-0.1.7/xinvert/finitediffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68730 2024-04-07 09:34:48.000000 xinvert-0.1.7/xinvert/numbas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-07 09:34:48.000000 xinvert-0.1.7/xinvert/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 09:34:52.477184 xinvert-0.1.7/xinvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2024-04-07 09:34:52.000000 xinvert-0.1.7/xinvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-07 09:34:52.000000 xinvert-0.1.7/xinvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 09:34:52.000000 xinvert-0.1.7/xinvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 09:34:52.000000 xinvert-0.1.7/xinvert.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-07 09:34:52.000000 xinvert-0.1.7/xinvert.egg-info/top_level.txt
```

### Comparing `xinvert-0.1.3/LICENSE` & `xinvert-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/PKG-INFO` & `xinvert-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: xinvert
-Version: 0.1.3
+Version: 0.1.7
 Summary: Invert geofluid problems based on xarray, using SOR iteration
 Home-page: https://github.com/miniufo/xinvert
 Author: miniufo
 Author-email: miniufo@163.com
 License: MIT
 Keywords: invert inversion atmosphere ocean SOR successive-overrelaxation-iteration
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: xarray
+Requires-Dist: dask
+Requires-Dist: numba
 
 # xinvert
 
 [![DOI](https://zenodo.org/badge/323045845.svg)](https://zenodo.org/badge/latestdoi/323045845)
 ![GitHub](https://img.shields.io/github/license/miniufo/xinvert)
 [![Documentation Status](https://readthedocs.org/projects/xinvert/badge/?version=latest)](https://xinvert.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/xinvert.svg)](https://badge.fury.io/py/xinvert)
 ![Workflow](https://github.com/miniufo/xinvert/actions/workflows/python-publish.yml/badge.svg)
 [![pytest](https://github.com/miniufo/xinvert/actions/workflows/tests.yml/badge.svg)](https://github.com/miniufo/xinvert/actions/workflows/tests.yml)
 [![Build Status](https://app.travis-ci.com/miniufo/xinvert.svg?branch=master)](https://app.travis-ci.com/miniufo/xinvert)
+[![status](https://joss.theoj.org/papers/1fc4ac8f98c0778516971880727a3a94/status.svg)](https://joss.theoj.org/papers/1fc4ac8f98c0778516971880727a3a94)
+
 
 ![animate plot](https://raw.githubusercontent.com/miniufo/xinvert/master/pics/animateConverge.gif)
 
 
 ## 1. Introduction
 Researches on meteorology and oceanography usually encounter [inversion problems](https://doi.org/10.1017/CBO9780511629570) that need to be solved numerically.  One of the classical inversion problem is to solve Poisson equation for a streamfunction $\psi$ given the vertical component of vorticity $\zeta$ and proper boundary conditions.
 
@@ -32,15 +38,15 @@
 
 Nowadays [`xarray`](http://xarray.pydata.org/en/stable/) becomes a popular data structure commonly used in [Big Data Geoscience](https://pangeo.io/).  Since the whole 4D data, as well as the coordinate information, are all combined into [`xarray`](http://xarray.pydata.org/en/stable/), solving the inversion problem become quite straightforward and the only input would be just one [`xarray.DataArray`](http://xarray.pydata.org/en/stable/) of vorticity.  Inversion on the spherical earth, like some meteorological problems, could utilize the spherical harmonics like [windspharm](https://github.com/ajdawson/windspharm), which would be more efficient using FFT than SOR used here.  However, in the case of ocean, SOR method is definitely a better choice in the presence of irregular land/sea mask.
 
 More importantly, this could be generalized into a numerical solver for elliptical equation using [SOR](https://mathworld.wolfram.com/SuccessiveOverrelaxationMethod.html) method, with spatially-varying coefficients.  Various popular inversion problems in geofluid dynamics will be illustrated as examples.
 
 One problem with SOR is that the speed of iteration using **explicit loops in Python** will be **e-x-t-r-e-m-e-l-y ... s-l-o-w**!  A very suitable solution here is to use [`numba`](https://numba.pydata.org/).  We may try our best to speed things up using more hardwares (possibly GPU).
 
-Classical problems include Gill-Matsuno model, Stommel-Munk model, QG omega model, PV inversion model, Swayer-Eliassen balance model...  A complete list of the classical inversion problems can be found at [this notebook](./docs/source/notebooks/Introduction.ipynb).
+Classical problems include Gill-Matsuno model, Stommel-Munk model, QG omega model, PV inversion model, Swayer-Eliassen balance model...  A complete list of the classical inversion problems can be found at [this notebook](./docs/source/notebooks/00_Introduction.ipynb).
 
 Why `xinvert`?
 
 - **Thinking and coding in equations:** User APIs are very close to the equations: unknowns are on the LHS of `=`, whereas the known forcings are on its RHS;
 - **Genearlize all the steady-state problems:** All the known steady-state problems in geophysical fluid dynamics can be easily adapted to fit the solvers;
 - **Very short parameter list:** Passing a single `xarray` forcing is enough for the inversion.  Coordinates information is already encapsulated.
 - **Flexible model parameters:** Model paramters can be either a constant, or varying with a specific dimension (like Coriolis $f$), or fully varying with space and time, due to the use of `xarray`'s broadcasting capability;
@@ -88,7 +94,28 @@
 # output has 1 more dimension (iter) than input, which could be animated over.
 # Here 40 frames and loop 1 per frame (final state is after 40 iterations) is used.
 psi = animate_iteration(invert_Poisson, vor, iParams=iParams,
                         loop_per_frame=1, max_frames=40)
 ```
 
 See the animation at the top.
+
+
+
+## 5 Cite
+
+If you use the package in research, teaching, or other activities, we would be grateful
+if you mention `xinvert` and cite our paper in JOSS:
+
+```bibtex
+@article{Qian2023,
+    doi = {10.21105/joss.05510},
+    url = {https://doi.org/10.21105/joss.05510},
+    year = {2023},
+    publisher = {The Open Journal},
+    volume = {8},
+    number = {89},
+    pages = {5510},
+    author = {Yu-Kun Qian},
+    title = {xinvert: A Python package for inversion problems in geophysical fluid dynamics}, journal = {Journal of Open Source Software}
+}
+```
```

### Comparing `xinvert-0.1.3/README.md` & `xinvert-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![DOI](https://zenodo.org/badge/323045845.svg)](https://zenodo.org/badge/latestdoi/323045845)
 ![GitHub](https://img.shields.io/github/license/miniufo/xinvert)
 [![Documentation Status](https://readthedocs.org/projects/xinvert/badge/?version=latest)](https://xinvert.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/xinvert.svg)](https://badge.fury.io/py/xinvert)
 ![Workflow](https://github.com/miniufo/xinvert/actions/workflows/python-publish.yml/badge.svg)
 [![pytest](https://github.com/miniufo/xinvert/actions/workflows/tests.yml/badge.svg)](https://github.com/miniufo/xinvert/actions/workflows/tests.yml)
 [![Build Status](https://app.travis-ci.com/miniufo/xinvert.svg?branch=master)](https://app.travis-ci.com/miniufo/xinvert)
+[![status](https://joss.theoj.org/papers/1fc4ac8f98c0778516971880727a3a94/status.svg)](https://joss.theoj.org/papers/1fc4ac8f98c0778516971880727a3a94)
+
 
 ![animate plot](https://raw.githubusercontent.com/miniufo/xinvert/master/pics/animateConverge.gif)
 
 
 ## 1. Introduction
 Researches on meteorology and oceanography usually encounter [inversion problems](https://doi.org/10.1017/CBO9780511629570) that need to be solved numerically.  One of the classical inversion problem is to solve Poisson equation for a streamfunction $\psi$ given the vertical component of vorticity $\zeta$ and proper boundary conditions.
 
@@ -18,15 +20,15 @@
 
 Nowadays [`xarray`](http://xarray.pydata.org/en/stable/) becomes a popular data structure commonly used in [Big Data Geoscience](https://pangeo.io/).  Since the whole 4D data, as well as the coordinate information, are all combined into [`xarray`](http://xarray.pydata.org/en/stable/), solving the inversion problem become quite straightforward and the only input would be just one [`xarray.DataArray`](http://xarray.pydata.org/en/stable/) of vorticity.  Inversion on the spherical earth, like some meteorological problems, could utilize the spherical harmonics like [windspharm](https://github.com/ajdawson/windspharm), which would be more efficient using FFT than SOR used here.  However, in the case of ocean, SOR method is definitely a better choice in the presence of irregular land/sea mask.
 
 More importantly, this could be generalized into a numerical solver for elliptical equation using [SOR](https://mathworld.wolfram.com/SuccessiveOverrelaxationMethod.html) method, with spatially-varying coefficients.  Various popular inversion problems in geofluid dynamics will be illustrated as examples.
 
 One problem with SOR is that the speed of iteration using **explicit loops in Python** will be **e-x-t-r-e-m-e-l-y ... s-l-o-w**!  A very suitable solution here is to use [`numba`](https://numba.pydata.org/).  We may try our best to speed things up using more hardwares (possibly GPU).
 
-Classical problems include Gill-Matsuno model, Stommel-Munk model, QG omega model, PV inversion model, Swayer-Eliassen balance model...  A complete list of the classical inversion problems can be found at [this notebook](./docs/source/notebooks/Introduction.ipynb).
+Classical problems include Gill-Matsuno model, Stommel-Munk model, QG omega model, PV inversion model, Swayer-Eliassen balance model...  A complete list of the classical inversion problems can be found at [this notebook](./docs/source/notebooks/00_Introduction.ipynb).
 
 Why `xinvert`?
 
 - **Thinking and coding in equations:** User APIs are very close to the equations: unknowns are on the LHS of `=`, whereas the known forcings are on its RHS;
 - **Genearlize all the steady-state problems:** All the known steady-state problems in geophysical fluid dynamics can be easily adapted to fit the solvers;
 - **Very short parameter list:** Passing a single `xarray` forcing is enough for the inversion.  Coordinates information is already encapsulated.
 - **Flexible model parameters:** Model paramters can be either a constant, or varying with a specific dimension (like Coriolis $f$), or fully varying with space and time, due to the use of `xarray`'s broadcasting capability;
@@ -73,8 +75,29 @@
 
 # output has 1 more dimension (iter) than input, which could be animated over.
 # Here 40 frames and loop 1 per frame (final state is after 40 iterations) is used.
 psi = animate_iteration(invert_Poisson, vor, iParams=iParams,
                         loop_per_frame=1, max_frames=40)
 ```
 
-See the animation at the top.
+See the animation at the top.
+
+
+
+## 5 Cite
+
+If you use the package in research, teaching, or other activities, we would be grateful
+if you mention `xinvert` and cite our paper in JOSS:
+
+```bibtex
+@article{Qian2023,
+    doi = {10.21105/joss.05510},
+    url = {https://doi.org/10.21105/joss.05510},
+    year = {2023},
+    publisher = {The Open Journal},
+    volume = {8},
+    number = {89},
+    pages = {5510},
+    author = {Yu-Kun Qian},
+    title = {xinvert: A Python package for inversion problems in geophysical fluid dynamics}, journal = {Journal of Open Source Software}
+}
+```
```

### Comparing `xinvert-0.1.3/setup.py` & `xinvert-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_3DOcean.py` & `xinvert-0.1.7/tests/test_3DOcean.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_AnimateConverge.py` & `xinvert-0.1.7/tests/test_AnimateConverge.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_Bretherton.py` & `xinvert-0.1.7/tests/test_Bretherton.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_Eliassen.py` & `xinvert-0.1.7/tests/test_Eliassen.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_FDs.py` & `xinvert-0.1.7/tests/test_FDs.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_Fofonoff.py` & `xinvert-0.1.7/tests/test_Fofonoff.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_Geopotential.py` & `xinvert-0.1.7/tests/test_Geopotential.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_GillMatsuno.py` & `xinvert-0.1.7/tests/test_GillMatsuno.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_HeldSuarezModel.py` & `xinvert-0.1.7/tests/test_HeldSuarezModel.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_Ishida.py` & `xinvert-0.1.7/tests/test_Ishida.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_LLC4320Poisson.py` & `xinvert-0.1.7/tests/test_LLC4320Poisson.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_MG.py` & `xinvert-0.1.7/tests/test_MG.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_MunkWBC.py` & `xinvert-0.1.7/tests/test_MunkWBC.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_OmegaEq.py` & `xinvert-0.1.7/tests/test_OmegaEq.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_OptArg.py` & `xinvert-0.1.7/tests/test_OptArg.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_Poisson.py` & `xinvert-0.1.7/tests/test_Poisson.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_QGPV.py` & `xinvert-0.1.7/tests/test_QGPV.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_RefStateSWM.py` & `xinvert-0.1.7/tests/test_RefStateSWM.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_StommelArons.py` & `xinvert-0.1.7/tests/test_StommelArons.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_StommelWBC.py` & `xinvert-0.1.7/tests/test_StommelWBC.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/tests/test_trace.py` & `xinvert-0.1.7/tests/test_trace.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/xinvert/__init__.py` & `xinvert-0.1.7/xinvert/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,8 +27,8 @@
                   invert_3DOcean, \
                   animate_iteration, cal_flow
                   
 from .utils import loop_noncore
 
 from .finitediffs import FiniteDiff, deriv, deriv2, padBCs
 
-__version__ = "0.1.3"
+__version__ = "0.1.7"
```

### Comparing `xinvert-0.1.3/xinvert/apps.py` & `xinvert-0.1.7/xinvert/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 
 @author: MiniUFO
 Copyright 2018. All rights reserved. Use is subject to license terms.
 """
 import numpy as np
 import xarray as xr
 import copy
-from .utils import _R_earth, _omega, _undeftmp, _g, _deg2m, loop_noncore
+from .utils import loop_noncore
 from .core import inv_standard3D, inv_standard2D, inv_standard1D,\
                   inv_general3D, inv_general2D,\
                   inv_general2D_bih, inv_standard2D_test
 
 
+# default undefined value
+_undeftmp = -9.99e8
+
 ###### default invert parameters. ######
 default_iParams = copy.deepcopy({
     # boundary conditions for the 2D slice
     # if 3D, should be ['fixed', 'fixed', 'fixed']
     'BCs'      : ['fixed', 'fixed'],
     # undefined value in the array
     'undef'    : np.nan,
@@ -46,14 +49,18 @@
     'R'      : 5e-5 , # linear drag coefficient in Stommel-Munk model
     'depth'  : 100  , # depth of the ocean or mixed layer in Stommel-Munk model
     'rho0'   : 1027 , # constant density of seawater in Stommel-Munk model
     'ang0'   : 2e5  , # background angular momentum
     'lambda' : 1e-8 , # used in Bretherton-Haidvogel model
     'c0'     : 8e-9 , # for Fofonoff model
     'c1'     : 8e-5 , # for Fofonoff model
+    
+    'Rearth' : 6371200.0, # Radius of Earth
+    'Omega'  : 7.292e-5 , # angular speed of Earth's rotation
+    'g'      : 9.80665  , # gravitational acceleration
 })
 
 
 
 """
 Application functions
 """
@@ -86,15 +93,15 @@
     
     Returns
     -------
     xarray.DataArray
         Results of the SOR inversion.
     """
     return __template(__coeffs_Poisson, inv_standard2D, 2, F, dims, coords,
-                      icbc, [], mParams, iParams)
+                      icbc, ['g', 'Omega', 'Rearth'], mParams, iParams)
 
 
 
 def invert_RefState(PV, dims, coords='z-lat', icbc=None,
                     mParams=default_mParams, iParams=default_iParams):
     r"""PV inversion for a balanced symmetric vortex.
 
@@ -131,15 +138,15 @@
     
     Returns
     -------
     xarray.DataArray
         Results (angular momentum Λ) of the SOR inversion.
     """
     return __template(__coeffs_RefState, inv_standard2D, 2, PV, dims, coords,
-                      icbc, ['Ang0', 'Gamma'], mParams, iParams)
+                      icbc, ['Ang0', 'Gamma', 'g', 'Omega', 'Rearth'], mParams, iParams)
 
 
 def invert_RefStateSWM(Q, dims, coords='lat', icbc=None,
                        mParams=default_mParams, iParams=default_iParams):
     r"""(PV) inversion for a steady state of shallow-water model.
 
     The balanced symmetric vortex equation is given as:
@@ -183,15 +190,15 @@
     
     Returns
     -------
     xarray.DataArray
         Results (angular momentum Λ) of the SOR inversion.
     """
     return __template(__coeffs_RefStateSWM, inv_standard1D, 1, Q, dims, coords,
-                      icbc, ['M0', 'C0'], mParams, iParams)
+                      icbc, ['M0', 'C0', 'g', 'Rearth', 'Omega'], mParams, iParams)
 
 
 def invert_PV2D(PV, dims, coords='z-lat', icbc=None,
                 mParams=default_mParams, iParams=default_iParams):
     r"""Inverting the QG PV equation.
 
     The QG PV equation is given as:
@@ -236,15 +243,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (QG streamfunction) of the SOR inversion.
     """
     return __template(__coeffs_PV2D, inv_standard2D, 2, PV, dims, coords,
-                      icbc, ['f0', 'beta', 'N2'], mParams, iParams)
+                      icbc, ['f0', 'beta', 'N2', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_Eliassen(F, dims, coords='z-lat', icbc=None,
                     mParams=default_mParams, iParams=default_iParams):
     r"""Inverting the Eliassen balanced vortex model.
 
     The Eliassen model is given as:
@@ -285,15 +293,15 @@
     
     Returns
     -------
     xarray.DataArray
         Results of the SOR inversion.
     """
     return __template(__coeffs_Eliassen, inv_standard2D, 2, F, dims, coords,
-                      icbc, ['A', 'B', 'C'], mParams, iParams)
+                      icbc, ['A', 'B', 'C', 'g', 'Omega', 'Rearth'], mParams, iParams)
 
 
 def invert_GillMatsuno(Q, dims, coords='lat-lon', icbc=None, 
                        mParams=default_mParams, iParams=default_iParams):
     r"""Inverting Gill-Matsuno model.
 
     The Gill-Matsuno model is given as:
@@ -332,15 +340,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (mass distribution) of the SOR inversion.
     """
     return __template(__coeffs_GillMatsuno, inv_general2D, 2, Q, dims, coords,
-                      icbc, ['f0', 'beta', 'epsilon', 'Phi'], mParams, iParams)
+                      icbc, ['f0', 'beta', 'epsilon', 'Phi', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_GillMatsuno_test(Q, dims, coords='lat-lon', icbc=None, 
                        mParams=default_mParams, iParams=default_iParams):
     r"""Inverting Gill-Matsuno model (test use only).
 
     The Gill-Matsuno model is given as:
@@ -379,15 +388,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (mass distribution) of the SOR inversion.
     """
     return __template(__coeffs_GillMatsuno_test, inv_standard2D_test, 2, Q, dims, coords,
-                      icbc, ['f0', 'beta', 'epsilon', 'Phi'], mParams, iParams)
+                      icbc, ['f0', 'beta', 'epsilon', 'Phi', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_Stommel(curl, dims, coords='lat-lon', icbc=None,
                    mParams=default_mParams, iParams=default_iParams):
     r"""Inverting Stommel model.
 
     The Stommel model is given as:
@@ -424,15 +434,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (streamfunction) of the SOR inversion.
     """
     return __template(__coeffs_Stommel, inv_general2D, 2, curl, dims, coords,
-                      icbc, ['beta', 'R', 'D', 'rho0'], mParams, iParams)
+                      icbc, ['beta', 'R', 'D', 'rho0', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_Stommel_test(curl, dims, coords='lat-lon', icbc=None,
                    mParams=default_mParams, iParams=default_iParams):
     r"""Inverting Stommel model (test used only).
 
     The Stommel model is given as:
@@ -469,15 +480,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (streamfunction) of the SOR inversion.
     """
     return __template(__coeffs_Stommel_test, inv_standard2D_test, 2, curl, dims, coords,
-                      icbc, ['beta', 'R', 'D', 'rho0'], mParams, iParams)
+                      icbc, ['beta', 'R', 'D', 'rho0', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_StommelMunk(curl, dims, coords='lat-lon', icbc=None,
                        mParams=default_mParams, iParams=default_iParams):
     r"""Inverting Stommel-Munk model.
 
     The Stommel-Munk model is given as:
@@ -516,15 +528,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results of the SOR inversion.
     """
     return __template(__coeffs_StommelMunk, inv_general2D_bih, 2, curl, dims, coords,
-                      icbc, ['A4', 'beta', 'R', 'D', 'rho0'], mParams, iParams)
+                      icbc, ['A4', 'beta', 'R', 'D', 'rho0', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_StommelArons(Q, dims, coords='lat-lon', icbc=None, 
                         mParams=default_mParams, iParams=default_iParams):
     r"""Inverting Stommel-Arons model.
 
     The Stommel-Arons model is given as:
@@ -562,15 +575,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (mass distribution) of the SOR inversion.
     """
     return __template(__coeffs_StommelArons, inv_general2D, 2, Q, dims, coords,
-                      icbc, ['f0', 'beta', 'epsilon'], mParams, iParams)
+                      icbc, ['f0', 'beta', 'epsilon', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_geostrophic(lapPhi, dims, coords='lat-lon', icbc=None,
                        mParams=default_mParams, iParams=default_iParams):
     r"""Inverting the geostrophic balance model.
 
     The geostrophic balance model is given as:
@@ -605,15 +619,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (geostrophic streamfunction) of the SOR inversion.
     """
     return __template(__coeffs_geostrophic, inv_standard2D, 2, lapPhi, dims, coords,
-                      icbc, ['f0', 'beta'], mParams, iParams)
+                      icbc, ['f0', 'beta', 'Omega', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_BrethertonHaidvogel(h, dims, coords='cartesian', icbc=None,
                                mParams=default_mParams, iParams=default_iParams):
     r"""Inverting the Bretherton-Haiduogel model.
 
     The Bretherton-Haiduogel model is given as:
@@ -649,15 +664,16 @@
         
     Returns
     -------
     xarray.DataArray
         Results (geostrophic streamfunction) of the SOR inversion.
     """
     return __template(__coeffs_Bretherton, inv_standard2D_test, 2, h, dims, coords,
-                      icbc, ['f0', 'beta', 'D', 'lambda'], mParams, iParams)
+                      icbc, ['f0', 'beta', 'D', 'lambda', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_Fofonoff(F, dims, coords='cartesian', icbc=None,
                     mParams=default_mParams, iParams=default_iParams):
     r"""Inverting the Fofonoff (1954) model.
 
     The equation is given as:
@@ -693,22 +709,23 @@
     
     Returns
     -------
     xarray.DataArray
         Results of the SOR inversion.
     """
     return __template(__coeffs_Fofonoff, inv_standard2D_test, 2, F, dims, coords,
-                      icbc, ['c0', 'c1', 'f0', 'beta'], mParams, iParams)
+                      icbc, ['c0', 'c1', 'f0', 'beta', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_omega(F, dims, coords='lat-lon', icbc=None,
                  mParams=default_mParams, iParams=default_iParams):
-    r"""Inverting the Omega equation.
+    r"""Inverting the omega equation.
 
-    The Omega equation is given as:
+    The omega equation is given as:
 
     .. math::
 
         \frac{f^2}{N^2}\frac{\partial^2 \omega}{\partial z^2} +
         \frac{\partial^2 \omega}{\partial y^2} +
         \frac{\partial^2 \omega}{\partial x^2} = \frac{F}{N^2}
 
@@ -755,16 +772,17 @@
         
         if np.isnan(mParams['N2'][1:]).any():
             raise Exception('nan in coefficient A')
         
         if (mParams['N2'][1:]<=0).any():
             raise Exception('unstable stratification in coefficient A')
     
-    return __template(__coeffs_Omega, inv_standard3D, 3, F, dims, coords,
-                      icbc, ['f0', 'beta', 'N2'], mParams, iParams)
+    return __template(__coeffs_omega, inv_standard3D, 3, F, dims, coords,
+                      icbc, ['f0', 'beta', 'N2', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 def invert_3DOcean(F, dims, coords='lat-lon', icbc=None,
                    mParams=default_mParams, iParams=default_iParams):
     r"""Inverting 3D ocean flow.
 
     The 3D ocean flow equation is given as:
@@ -816,15 +834,16 @@
         if np.isnan(mParams['N2'][1:]).any():
             raise Exception('nan in coefficient A')
         
         if (mParams['N2'][1:]<=0).any():
             raise Exception('unstable stratification in coefficient A')
     
     return __template(__coeffs_3DOcean, inv_general3D, 3, F, dims, coords,
-                      icbc, ['f0', 'beta', 'epsilon', 'N2', 'k'], mParams, iParams)
+                      icbc, ['f0', 'beta', 'epsilon', 'N2', 'k', 'g', 'Omega', 'Rearth'],
+                      mParams, iParams)
 
 
 
 """
 Some high-level functions are based on application functions
 """
 def animate_iteration(app_name, F, dims, coords='lat-lon', icbc=None,
@@ -875,83 +894,87 @@
     dimLen = len(dims)
     
     iParams = __update(default_iParams, iParams)
     
     if   app_name == 'poisson':
         coef_func = __coeffs_Poisson
         invt_func = inv_standard2D
-        validMPs  = []
+        validMPs  = ['g', 'Omega', 'Rearth']
         
     elif app_name == 'pv2d':
         coef_func = __coeffs_PV2D
         invt_func = inv_standard2D
-        validMPs  = ['f0', 'beta', 'N2']
+        validMPs  = ['f0', 'beta', 'N2', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'geostrophic':
         coef_func = __coeffs_geostrophic
         invt_func = inv_standard2D
-        validMPs  = ['f0', 'beta']
+        validMPs  = ['f0', 'beta', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'gillmatsuno':
         coef_func = __coeffs_GillMatsuno
         invt_func = inv_general2D
-        validMPs  = ['f0', 'beta', 'epsilon', 'Phi']
+        validMPs  = ['f0', 'beta', 'epsilon', 'Phi', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'eliassen':
         coef_func = __coeffs_Eliassen
         invt_func = inv_standard2D
-        validMPs  = ['A', 'B', 'C']
+        validMPs  = ['A', 'B', 'C', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'stommel':
         coef_func = __coeffs_Stommel
         invt_func = inv_general2D_bih
-        validMPs  = ['beta', 'R', 'D', 'rho0']
+        validMPs  = ['beta', 'R', 'D', 'rho0', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'stommelmunk':
         coef_func = __coeffs_StommelMunk
         invt_func = inv_general2D_bih
-        validMPs  = ['A4', 'beta', 'R', 'D', 'rho0']
+        validMPs  = ['A4', 'beta', 'R', 'D', 'rho0', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'refstate':
         coef_func = __coeffs_RefState
         invt_func = inv_standard2D
-        validMPs  = ['Ang0', 'Gamma']
+        validMPs  = ['Ang0', 'Gamma', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'brethertonhaidvogel':
         coef_func = __coeffs_Bretherton
         invt_func = inv_standard2D_test
-        validMPs  = ['f0', 'beta', 'D', 'lambda']
+        validMPs  = ['f0', 'beta', 'D', 'lambda', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'fofonoff':
         coef_func = __coeffs_Fofonoff
         invt_func = inv_standard2D_test
-        validMPs  = ['c0', 'c1', 'f0', 'beta']
+        validMPs  = ['c0', 'c1', 'f0', 'beta', 'g', 'Omega', 'Rearth']
         
     elif app_name == 'omega':
-        coef_func = __coeffs_Omega
+        coef_func = __coeffs_omega
         invt_func = inv_standard3D
-        validMPs  = ['f0', 'beta', 'N2']
+        validMPs  = ['f0', 'beta', 'N2', 'g', 'Omega', 'Rearth']
         
     elif app_name == '3Docean':
-        coef_func = __coeffs_Omega
+        coef_func = __coeffs_omega
         invt_func = inv_standard3D
-        validMPs  = ['f0', 'beta', 'N2', 'epsilon', 'k']
+        validMPs  = ['f0', 'beta', 'N2', 'epsilon', 'k', 'g', 'Omega', 'Rearth']
     else:
         raise Exception('unsupported problem: '+app_name+', should be one of:\n'+
                         "'Poisson'\n'PV2D'\n'GillMatsuno'\n'Eliassen'\n"+
                         "'geostrophic'\n'StommelMunk'\n'RefState'\n'omega'")
     
+    mParams = __update(default_mParams, mParams, validMPs)
+    
     ######  1. calculating the coefficients  ######
     maskF, initS, coeffs = coef_func(F, dims, coords, mParams, iParams, icbc)
     
     ######  2. calculating the parameters  ######
     if dimLen == 2:
-        ps = __cal_params2D(maskF[dims[0]], maskF[dims[1]], coords)
+        ps = __cal_params2D(maskF[dims[0]], maskF[dims[1]], coords,
+                            Rearth=mParams['Rearth'])
     elif dimLen == 3:
-        ps = __cal_params3D(maskF[dims[0]], maskF[dims[1]], maskF[dims[2]], coords)
+        ps = __cal_params3D(maskF[dims[0]], maskF[dims[1]], maskF[dims[2]], coords,
+                            Rearth=mParams['Rearth'])
     else:
         raise Exception('dimension length should be one of [2, 3]')
     
     iParams = __update(ps, iParams)
     
     if iParams['debug']:
         __print_params(iParams)
@@ -1062,15 +1085,15 @@
         
         o_guess = o_guess.interp_like(frs[0])
         o_guess = xr.where(np.isnan(o_guess), 0, o_guess) # maskout nan
     
     return o_guess, fs, os
 
 
-def _invert_Omega_MG(force, S, dims, BCs=['fixed', 'fixed', 'fixed'],
+def _invert_omega_MG(force, S, dims, BCs=['fixed', 'fixed', 'fixed'],
                     coords='latlon', f0=None, beta=None,
                     undef=np.nan, mxLoop=5000, tolerance=1e-6,
                     optArg=None, printInfo=True, debug=False,
                     icbc=None, ratio=4, gridNo=3):
     from utils.XarrayUtils import coarsen
     
     ratios = [10, 6, 3, 1]
@@ -1097,15 +1120,15 @@
         if ratio == 1:
             break
         
         o_guess = o_guess.interp_like(fs[i+1])
         o_guess = xr.where(np.isnan(o_guess), 0, o_guess) # maskout nan
         
         # # iteration over fine grid from the coarse initial guess
-        # o = invert_OmegaEquation(force, S, dims=dims, BCs=BCs, coords=coords,
+        # o = invert_omegaEquation(force, S, dims=dims, BCs=BCs, coords=coords,
         #                          f0=f0, beta=beta, undef=undef, mxLoop=mxLoop/50,
         #                          tolerance=tolerance, optArg=optArg, debug=debug,
         #                          printInfo=printInfo, icbc=o_guess)
     
     return o_guess, fs, os
 
 
@@ -1203,34 +1226,37 @@
             
         else:
             raise Exception('unsupported coords ' + coords +
                             ', should be [lat-lon, z-lat, z-lon, cartesian]')
     
     else: # GillMatsuno case
         mParams = __update(default_mParams, mParams,
-                           ['f0', 'beta', 'epsilon', 'Phi'])
+                           ['f0', 'beta', 'epsilon', 'Phi', 'Omega', 'Rearth'])
         
-        eps  = mParams['epsilon']
-        f0   = mParams['f0']
-        beta = mParams['beta']
+        eps    = mParams['epsilon']
+        f0     = mParams['f0']
+        beta   = mParams['beta']
+        Omega  = mParams['Omega']
+        Rearth = mParams['Rearth']
         
         if coords.lower() == 'lat-lon':
             lats = np.deg2rad(S[dims[0]])
             cosLat = np.cos(lats)
             sinLat = np.sin(lats)
             
-            f = 2.0 * _omega * sinLat
+            f = 2.0 * Omega * sinLat
+            deg2m = np.deg2rad(1.0) * Rearth
             
             coef1 = eps / (eps**2.0 + f**2.0)
             coef2 = f   / (eps**2.0 + f**2.0)
             
-            c1 = - coef1 * S.differentiate(dims[1]) / _deg2m / cosLat \
-                 - coef2 * S.differentiate(dims[0]) / _deg2m
-            c2 = - coef1 * S.differentiate(dims[0]) / _deg2m \
-                 + coef2 * S.differentiate(dims[1]) / _deg2m / cosLat
+            c1 = - coef1 * S.differentiate(dims[1]) / deg2m / cosLat \
+                 - coef2 * S.differentiate(dims[0]) / deg2m
+            c2 = - coef1 * S.differentiate(dims[0]) / deg2m \
+                 + coef2 * S.differentiate(dims[1]) / deg2m / cosLat
         elif coords.lower() == 'cartesian':
             ydef = S[dims[0]]
             f = f0 + beta * ydef
             
             coef1 = eps / (eps**2.0 + f**2.0)
             coef2 = f   / (eps**2.0 + f**2.0)
             
@@ -1290,19 +1316,22 @@
     mParams = __update(default_mParams, mParams, validParams)
     
     ######  1. calculating the coefficients  ######
     maskF, initS, coeffs = coef_func(F, dims, coords, mParams, iParams, icbc)
     
     ######  2. calculating the parameters  ######
     if dimLen == 1:
-        ps = __cal_params1D(maskF[dims[0]], coords)
+        ps = __cal_params1D(maskF[dims[0]], coords,
+                            Rearth=mParams['Rearth'])
     elif dimLen == 2:
-        ps = __cal_params2D(maskF[dims[0]], maskF[dims[1]], coords)
+        ps = __cal_params2D(maskF[dims[0]], maskF[dims[1]], coords,
+                            Rearth=mParams['Rearth'])
     elif dimLen == 3:
-        ps = __cal_params3D(maskF[dims[0]], maskF[dims[1]], maskF[dims[2]], coords)
+        ps = __cal_params3D(maskF[dims[0]], maskF[dims[1]], maskF[dims[2]], coords,
+                            Rearth=mParams['Rearth'])
     else:
         raise Exception('dimension length should be one of [2, 3]')
         
     iParams = __update(ps, iParams)
     
     if iParams['debug']:
         __print_params(iParams)
@@ -1360,45 +1389,49 @@
                         ', should be in [lat-lon, z-lat, z-lon, cartesian]')
     
     return F, initS, (A, B, C)
 
 
 def __coeffs_RefState(Q, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for reference state."""
-    angM  = mParams['angM']
+    ang0  = mParams['ang0']
     Gamma = mParams['Gamma']
+    g     = mParams['g']
     
     maskF, initS, zero = __mask_FS(Q, dims, iParams, icbc)
 
     if coords.lower() == 'z-lat': # dims[0] is θ, dims[1] is lat
         lats = np.deg2rad(maskF[dims[1]])
         sinL = np.sin(lats)
         
         A = zero + sinL
         B = zero
-        C = zero + Gamma * _g / Q / maskF[dims[1]]
+        C = zero + Gamma * g / Q / maskF[dims[1]]
         F = maskF.where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[0] is θ, dims[1] is r
-        A = zero + 2.0 * angM / maskF[dims[1]]**3.0
+        A = zero + 2.0 * ang0 / maskF[dims[1]]**3.0
         B = zero
-        C = zero + Gamma * _g / Q / maskF[dims[1]]
+        C = zero + Gamma * g / Q / maskF[dims[1]]
         F = maskF.where(maskF!=_undeftmp, _undeftmp)
 
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [z-lat, cartesian]')
     
     return F, initS, (A, B, C)
 
 
 def __coeffs_RefStateSWM(Q, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for reference state of a shallow-water model."""
-    M0 = mParams['M0']
-    C0 = mParams['C0']
+    M0     = mParams['M0']
+    C0     = mParams['C0']
+    g      = mParams['g']
+    Rearth = mParams['Rearth']
+    Omega  = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(Q, dims, iParams, icbc)
     
     import numba as nb
     
     @nb.jit(nopython=True, cache=False)
     def diff_2nd(M, cosH, delY):
@@ -1414,30 +1447,30 @@
         return re
     
     if coords.lower() == 'lat': # dims[0] is θ, dims[1] is lat
         lats = np.deg2rad(maskF[dims[0]])
         cosG = np.cos(lats)
         cosH = np.cos((lats+lats.shift({dims[0]:1}))/2.0) # shift half grid
         sinG = np.sin(lats)
-        asin = _R_earth * sinG
-        acos = _R_earth * cosG
+        asin = Rearth * sinG
+        acos = Rearth * cosG
         
         acos = xr.where(acos<0, -acos*0.1, acos) # ensure positive 0 at poles
         
         diff = xr.apply_ufunc(diff_2nd, M0, cosH,
-                              np.abs(lats[0]-lats[1])*_R_earth,
+                              np.abs(lats[0]-lats[1]) * Rearth,
                               dask='parallelized',
                               vectorize=True,
                               input_core_dims=[[dims[0]], [dims[0]], []],
                               output_core_dims=[[dims[0]]])
         
         A = zero + 1.0 / cosH
-        B = zero - C0 * maskF * asin  / (np.pi * _g * acos**3.0)
-        F = zero - (asin * C0**2.0 / (2.0 * np.pi * _g * acos**3.0)) + \
-                   (2.0 * np.pi * _omega**2.0 * asin * acos) / _g - diff
+        B = zero - C0 * maskF * asin  / (np.pi * g* acos**3.0)
+        F = zero - (asin * C0**2.0 / (2.0 * np.pi * g* acos**3.0)) + \
+                   (2.0 * np.pi * Omega**2.0 * asin * acos) / g - diff
     
     elif coords.lower() == 'cartesian': # dims[0] is θ, dims[1] is r
         raise Exception('not supported for cartesian coordinates')
 
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [z-lat, cartesian]')
@@ -1449,15 +1482,15 @@
     """Calculating coefficients for QG PV equation."""
     f0 = mParams['f0']
     N2 = mParams['N2']
     
     maskF, initS, zero = __mask_FS(PV, dims, iParams, icbc)
 
     if coords.lower() == 'z-lat': # dims[0] is p, dims[1] is lat
-        A = zero + f0**2 / N2
+        A = zero + f0**2 / N2  # should use f(lat)
         B = zero
         C = zero + 1
         F = maskF.where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[0] is p, dims[1] is r
         A = zero + f0**2 / N2
         B = zero
@@ -1494,38 +1527,40 @@
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [z-lat, cartesian]')
     
     return F, initS, (A, B, C)
 
 
-def __coeffs_GillMatsuno(Q, dims, coords, mParam, iParams, icbc):
+def __coeffs_GillMatsuno(Q, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Gill-Matsuno model."""
-    Phi     = mParam['Phi' ]
-    epsilon = mParam['epsilon']
-    f0      = mParam['f0'  ]
-    beta    = mParam['beta']
+    Phi     = mParams['Phi' ]
+    epsilon = mParams['epsilon']
+    f0      = mParams['f0'  ]
+    beta    = mParams['beta']
+    Omega   = mParams['Omega']
+    Rearth  = mParams['Rearth']
     
     maskF, initS, zero = __mask_FS(Q, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(Q[dims[0]])
         cosL = np.cos(lats)
         
-        f = 2.0 * _omega * np.sin(lats)
+        f = 2.0 * Omega * np.sin(lats)
         
         c1 = epsilon / (epsilon**2. + f**2.)
         c2 = f       / (epsilon**2. + f**2.)
-        const = _R_earth / 180. * np.pi
+        deg2m = Rearth / 180. * np.pi
         
         A = zero + c1 * Phi
         B = zero
         C = zero + c1 * Phi / cosL**2.
-        D = zero + Phi *(c1.differentiate(dims[0]) / const + c1*np.tan(lats)/_R_earth)
-        E = zero - Phi * c2.differentiate(dims[0]) / const / cosL
+        D = zero + Phi *(c1.differentiate(dims[0]) / deg2m + c1*np.tan(lats)/Rearth)
+        E = zero - Phi * c2.differentiate(dims[0]) / deg2m / cosL
         F = zero - epsilon
         G = maskF.where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[0] is y, dims[1] is x
         ydef = Q[dims[0]]
         f    = f0 + beta * ydef
         
@@ -1543,30 +1578,31 @@
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [lat-lon, cartesian]')
     
     return G, initS, (A, B, C, D, E, F)
 
 
-def __coeffs_GillMatsuno_test(Q, dims, coords, mParam, iParams, icbc):
+def __coeffs_GillMatsuno_test(Q, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Gill-Matsuno model."""
-    Phi     = mParam['Phi' ]
-    epsilon = mParam['epsilon']
-    f0      = mParam['f0'  ]
-    beta    = mParam['beta']
+    Phi     = mParams['Phi' ]
+    epsilon = mParams['epsilon']
+    f0      = mParams['f0'  ]
+    beta    = mParams['beta']
+    Omega   = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(Q, dims, iParams, icbc)
 
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(Q[dims[0]])
         cosG = np.cos(lats)
         cosH = np.cos((lats+lats.shift({dims[0]:1}))/2.)
         
-        fG = 2. * _omega * np.sin(lats)
-        fH = 2. * _omega * np.sin((lats+lats.shift({dims[0]:1}))/2.)
+        fG = 2. * Omega * np.sin(lats)
+        fH = 2. * Omega * np.sin((lats+lats.shift({dims[0]:1}))/2.)
         
         c1G = epsilon / (epsilon**2. + fG**2.)
         c1H = epsilon / (epsilon**2. + fH**2.)
         c2G = fG      / (epsilon**2. + fG**2.)
         
         A = zero + c1H * Phi * cosH
         B = zero - c2G * Phi
@@ -1594,32 +1630,34 @@
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [lat-lon, cartesian]')
     
     return F, initS, (A, B, C, D, E)
 
 
-def __coeffs_Stommel(curl, dims, coords, mParam, iParams, icbc):
+def __coeffs_Stommel(curl, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Stommel model."""
-    beta = mParam['beta']
-    R    = mParam['R'   ]
-    depth= mParam['D'   ]
-    rho0 = mParam['rho0']
+    beta   = mParams['beta']
+    R      = mParams['R'   ]
+    depth  = mParams['D'   ]
+    rho0   = mParams['rho0']
+    Rearth = mParams['Rearth']
+    Omega  = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(curl, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(curl[dims[0]])
         cosL = np.cos(lats)
         
         A = zero - R / depth
         B = zero
         C = zero - R / depth / cosL**2.
         D = zero
-        E = zero - 2. * _omega / _R_earth
+        E = zero - 2. * Omega / Rearth
         F = zero
         G = (-maskF / depth / rho0).where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[0] is θ, dims[1] is r
         A = zero - R / depth
         B = zero
         C = zero - R / depth
@@ -1631,29 +1669,30 @@
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [lat-lon, z-lat, z-lon, cartesian]')
     
     return G, initS, (A, B, C, D, E, F)
 
 
-def __coeffs_Stommel_test(curl, dims, coords, mParam, iParams, icbc):
+def __coeffs_Stommel_test(curl, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Stommel model."""
-    f0   = mParam['f0'  ]
-    beta = mParam['beta']
-    R    = mParam['R'   ]
-    depth= mParam['D'   ]
-    rho0 = mParam['rho0']
+    f0    = mParams['f0'  ]
+    beta  = mParams['beta']
+    R     = mParams['R'   ]
+    depth = mParams['D'   ]
+    rho0  = mParams['rho0']
+    Omega = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(curl, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(curl[dims[0]])
         cosG = np.cos(lats)
         cosH = np.cos((lats+lats.shift({dims[0]:1}))/2.)
-        f    = 2. * _omega * np.sin(lats)
+        f    = 2. * Omega * np.sin(lats)
         
         A = zero - R / depth * cosH
         B = zero - f
         C = zero + f
         D = zero - R / depth / cosG
         E = zero
         F = (-maskF / depth / rho0 * cosG).where(maskF!=_undeftmp, _undeftmp)
@@ -1674,34 +1713,36 @@
                         ', should be in [lat-lon, z-lat, z-lon, cartesian]')
     
     return F, initS, (A, B, C, D, E)
 
 
 def __coeffs_StommelMunk(curl, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Stommel-Munk model."""
-    beta = mParams['beta']
-    A4   = mParams['A4'  ]
-    R    = mParams['R'   ]
-    depth= mParams['D'   ]
-    rho0 = mParams['rho0']
+    beta   = mParams['beta']
+    A4     = mParams['A4'  ]
+    R      = mParams['R'   ]
+    depth  = mParams['D'   ]
+    rho0   = mParams['rho0']
+    Omega  = mParams['Omega']
+    Rearth = mParams['Rearth']
     
     maskF, initS, zero = __mask_FS(curl, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(curl[dims[0]])
         cosL = np.cos(lats)
         
         A = zero + A4
         B = zero
         C = zero + A4 / cosL**2.
         D = zero - R / depth
         E = zero
         F = zero - R / depth / cosL**2.
         G = zero
-        H = zero - 2. * _omega / _R_earth
+        H = zero - 2. * Omega / Rearth
         I = zero
         J = (-maskF / depth / rho0).where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[0] is y, dims[1] is x
         A = zero + A4
         B = zero
         C = zero + A4
@@ -1716,37 +1757,39 @@
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [lat-lon, cartesian]')
     
     return J, initS, (A, B, C, D, E, F, G, H, I)
 
 
-def __coeffs_StommelArons(Q, dims, coords, mParam, iParams, icbc):
+def __coeffs_StommelArons(Q, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Stommel-Arons model."""
-    epsilon = mParam['epsilon']
-    f0      = mParam['f0']
-    beta    = mParam['beta']
+    epsilon = mParams['epsilon']
+    f0      = mParams['f0']
+    beta    = mParams['beta']
+    Omega   = mParams['Omega']
+    Rearth  = mParams['Rearth']
     
     maskF, initS, zero = __mask_FS(Q, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(Q[dims[0]])
         cosL = np.cos(lats)
         
-        f = 2.0 * _omega * np.sin(lats)
+        f = 2.0 * Omega * np.sin(lats)
         
         c1 = epsilon / (epsilon**2. + f**2.)
         c2 = f       / (epsilon**2. + f**2.)
-        const = _R_earth / 180. * np.pi
+        deg2m = Rearth / 180. * np.pi
         
         A = zero + c1
         B = zero
         C = zero + c1 / cosL**2.
-        D = zero + (c1.differentiate(dims[0]) / const + c1*np.tan(lats)/_R_earth)
-        E = zero - c2.differentiate(dims[0]) / const / cosL
+        D = zero + (c1.differentiate(dims[0]) / deg2m + c1*np.tan(lats)/Rearth)
+        E = zero - c2.differentiate(dims[0]) / deg2m / cosL
         F = zero
         G = maskF.where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[0] is y, dims[1] is x
         ydef = Q[dims[0]]
         f    = f0 + beta * ydef
         
@@ -1766,29 +1809,30 @@
                         ', should be in [lat-lon, cartesian]')
     
     return G, initS, (A, B, C, D, E, F)
 
 
 def __coeffs_geostrophic(lapPhi, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for geostrophic equation."""
-    f0   = mParams['f0']
-    beta = mParams['beta']
+    f0    = mParams['f0']
+    beta  = mParams['beta']
+    Omega = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(lapPhi, dims, iParams, icbc)
 
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(maskF[dims[0]])
         
         sinG = np.sin(lats)
         sinH = np.sin((lats+lats.shift({dims[0]:1}))/2.)
         cosG = np.cos(lats)
         cosH = np.cos((lats+lats.shift({dims[0]:1}))/2.)
         
-        fH = 2. * _omega * sinH
-        fG = 2. * _omega * sinG
+        fH = 2. * Omega * sinH
+        fG = 2. * Omega * sinG
         
         # regulation for near-zero f
         fH = xr.where(np.abs(fH)<2e-05, fH*1.5, fH)
         fG = xr.where(np.abs(fG)<2e-05, fG*1.5, fG)
         
         A = zero + fH * cosH
         B = zero
@@ -1810,26 +1854,27 @@
                         ', should be in [lat-lon, cartesian]')
     
     return F, initS, (A, B, C)
 
 
 def __coeffs_Bretherton(h, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Bretherton-Haiduogel equation."""
-    f0   = mParams['f0']
-    beta = mParams['beta']
-    depth= mParams['D']
-    lamb = mParams['lambda']
+    f0    = mParams['f0']
+    beta  = mParams['beta']
+    depth = mParams['D']
+    lamb  = mParams['lambda']
+    Omega = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(h, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(maskF[dims[0]])
         cosG = np.cos(lats)
         cosH = np.cos((lats+lats.shift({dims[0]:1}))/2.0) # shift half grid
-        f    = 2. * _omega * np.sin(lats)
+        f    = 2. * Omega * np.sin(lats)
         
         A = zero + cosH
         B = zero
         C = zero
         D = zero + 1.0 / cosG
         E = zero - lamb * depth * cosG
         F = (-maskF*f/depth * cosG).where(maskF!=_undeftmp, _undeftmp)
@@ -1850,26 +1895,27 @@
                         ', should be in [lat-lon, cartesian]')
     
     return F, initS, (A, B, C, D, E)
 
 
 def __coeffs_Fofonoff(f, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for Bretherton-Haiduogel equation."""
-    f0   = mParams['f0']
-    beta = mParams['beta']
-    c0   = mParams['c0']
-    c1   = mParams['c1']
+    f0    = mParams['f0']
+    beta  = mParams['beta']
+    c0    = mParams['c0']
+    c1    = mParams['c1']
+    Omega = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(f, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[0] is lat, dims[1] is lon
         lats = np.deg2rad(maskF[dims[0]])
         cosG = np.cos(lats)
         cosH = np.cos((lats+lats.shift({dims[0]:1}))/2.0) # shift half grid
-        f    = 2. * _omega * np.sin(lats)
+        f    = 2. * Omega * np.sin(lats)
         
         A = zero + cosH
         B = zero
         C = zero
         D = zero + 1.0 / cosG
         E = zero - c0 * cosG
         F = ((zero + c1 - f) * cosG).where(maskF!=_undeftmp, _undeftmp)
@@ -1888,29 +1934,30 @@
     else:
         raise Exception('unsupported coords ' + coords +
                         ', should be in [lat-lon, cartesian]')
     
     return F, initS, (A, B, C, D, E)
 
 
-def __coeffs_Omega(force, dims, coords, mParams, iParams, icbc):
+def __coeffs_omega(force, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for QG omega equation."""
-    f0   = mParams['f0']
-    beta = mParams['beta']
-    N2   = mParams['N2']
+    f0    = mParams['f0']
+    beta  = mParams['beta']
+    N2    = mParams['N2']
+    Omega = mParams['Omega']
     
     maskF, initS, zero = __mask_FS(force, dims, iParams, icbc)
 
     if coords.lower() == 'lat-lon': # dims[1] is lat, dims[2] is lon
         lats = np.deg2rad(force[dims[1]])
         
         cosH = np.cos((lats+lats.shift({dims[1]:1}))/2.)
         cosG = np.cos(lats)
         
-        f = 2. * _omega * np.sin(lats)
+        f = 2. * Omega * np.sin(lats)
         
         A = zero + f**2 * cosG
         B = zero + N2*cosH
         C = zero + N2/cosG
         F = (maskF * cosG).where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[1] is y, dims[2] is x
@@ -1933,44 +1980,47 @@
 def __coeffs_3DOcean(force, dims, coords, mParams, iParams, icbc):
     """Calculating coefficients for 3D ocean model."""
     f0      = mParams['f0']
     beta    = mParams['beta']
     epsilon = mParams['epsilon']
     N2      = mParams['N2']
     k       = mParams['k']
+    Omega   = mParams['Omega']
+    Rearth  = mParams['Rearth']
     
     maskF, initS, zero = __mask_FS(force, dims, iParams, icbc)
     
     if coords.lower() == 'lat-lon': # dims[1] is lat, dims[2] is lon
         lats = np.deg2rad(force[dims[1]])
         cosL = np.cos(lats)
         
-        f = 2. * _omega * np.sin(lats)
+        f = 2. * Omega * np.sin(lats)
         
         c1 = epsilon / (epsilon**2. + f**2.)
         c2 = f       / (epsilon**2. + f**2.)
         c3 = maskF[dims[0]] - maskF[dims[0]] + k / N2
-        const = _R_earth / 180. * np.pi
+        deg2m = Rearth / 180. * np.pi
         
         A = zero + c3
         B = zero + c1
         C = zero + c1 / cosL**2.
         D = zero + c3.differentiate(dims[0])
-        E = zero +(c1.differentiate(dims[1]) / const - c1*np.tan(lats)/_R_earth)
-        F = zero - c2.differentiate(dims[1]) / const / cosL
+        E = zero +(c1.differentiate(dims[1]) / deg2m - c1*np.tan(lats)/Rearth)
+        F = zero - c2.differentiate(dims[1]) / deg2m / cosL
         G = zero
         H = maskF.where(maskF!=_undeftmp, _undeftmp)
     
     elif coords.lower() == 'cartesian': # dims[1] is y, dims[2] is x
         ydef = force[dims[1]]
         f = f0 + beta * ydef
         
         c1 = epsilon / (epsilon**2. + f**2.)
         c2 = f       / (epsilon**2. + f**2.)
         c3 = maskF[dims[0]] - maskF[dims[0]] + k / N2
+        const = 1 # check this
         
         A = zero + c3
         B = zero + c1
         C = zero + c1
         D = zero + c3.differentiate(dims[0])
         E = zero + c1.differentiate(dims[1]) / const
         F = zero - c2.differentiate(dims[1]) / const
@@ -2030,15 +2080,16 @@
         
         initS = xr.where(mask, icbc, 0)
     
     # loaded initS because dask cannot be modified
     return maskF, initS.load(), zero
 
 
-def __cal_params3D(dim3_var, dim2_var, dim1_var, coords, debug=False):
+def __cal_params3D(dim3_var, dim2_var, dim1_var, coords,
+                   Rearth=default_mParams['Rearth'], debug=False):
     r"""Pre-calculate some parameters needed in SOR for the 3D cases.
 
     Parameters
     ----------
     dim3_var: xarray.DataArray
         Dimension variable of third dimension (e.g., lev).
     dim2_var: xarray.DataArray
@@ -2055,18 +2106,21 @@
     """
     gc3  = len(dim3_var)
     gc2  = len(dim2_var)
     gc1  = len(dim1_var)
     del3 = dim3_var.diff(dim3_var.name).values[0] # assumed uniform
     del2 = dim2_var.diff(dim2_var.name).values[0] # assumed uniform
     del1 = dim1_var.diff(dim1_var.name).values[0] # assumed uniform
+    __uniform_interval(dim3_var, del3)
+    __uniform_interval(dim2_var, del2)
+    __uniform_interval(dim1_var, del1)
     
     if coords.lower() == 'lat-lon':
-        del2 = np.deg2rad(del2) * _R_earth # convert lat to m
-        del1 = np.deg2rad(del1) * _R_earth # convert lon to m
+        del2 = np.deg2rad(del2) * Rearth # convert lat to m
+        del1 = np.deg2rad(del1) * Rearth # convert lon to m
     elif coords.lower() == 'cartesian':
         pass
     else:
         raise Exception('unsupported coords for 3D case: ' + coords +
                         ', should be in [\'lat-lon\', \'cartesian\']')
     
     ratio1    = del1 / del2
@@ -2109,15 +2163,15 @@
                                 #   [0] overflow or not
                                 #   [1] tolerance
                                 #   [2] loop count
     
     return re
 
 
-def __cal_params2D(dim2_var, dim1_var, coords):
+def __cal_params2D(dim2_var, dim1_var, coords, Rearth=default_mParams['Rearth']):
     r"""Pre-calculate some parameters needed in SOR.
 
     Parameters
     ----------
     dim2_var: xarray.DataArray
         Dimension variable of second dimension (e.g., lat).
     dim1_var: xarray.DataArray
@@ -2130,22 +2184,24 @@
     re: dict
         Pre-calculated parameters.
     """
     gc2  = len(dim2_var)
     gc1  = len(dim1_var)
     del2 = dim2_var.diff(dim2_var.name).values[0] # assumed uniform
     del1 = dim1_var.diff(dim1_var.name).values[0] # assumed uniform
+    __uniform_interval(dim2_var, del2)
+    __uniform_interval(dim1_var, del1)
     
     if coords.lower() == 'lat-lon':
-        del2 = np.deg2rad(del2) * _R_earth # convert lat to m
-        del1 = np.deg2rad(del1) * _R_earth # convert lon to m
+        del2 = np.deg2rad(del2) * Rearth # convert lat to m
+        del1 = np.deg2rad(del1) * Rearth # convert lon to m
     elif coords.lower() == 'z-lat':
-        del1 = np.deg2rad(del1) * _R_earth # convert lat to m
+        del1 = np.deg2rad(del1) * Rearth # convert lat to m
     elif coords.lower() == 'z-lon':
-        del1 = np.deg2rad(del1) * _R_earth # convert lon to m
+        del1 = np.deg2rad(del1) * Rearth # convert lon to m
     elif coords.lower() == 'cartesian':
         pass
     else:
         raise Exception('unsupported coords for 2D case: ' + coords +
                         ', should be [lat-lon, cartesian]')
     
     ratio    = del1 / del2
@@ -2178,15 +2234,15 @@
                                #   [0] overflow or not
                                #   [1] tolerance
                                #   [2] loop count
     
     return re
 
 
-def __cal_params1D(dim1_var, coords):
+def __cal_params1D(dim1_var, coords, Rearth=default_mParams['Rearth']):
     r"""Pre-calculate some parameters needed in SOR.
 
     Parameters
     ----------
     dim1_var: xarray.DataArray
         Dimension variable of first  dimension (e.g., lon).
     debug: boolean
@@ -2195,17 +2251,18 @@
     Returns
     -------
     re: dict
         Pre-calculated parameters.
     """
     gc1  = len(dim1_var)
     del1 = dim1_var.diff(dim1_var.name).values[0] # assumed uniform
+    __uniform_interval(dim1_var, del1)
     
     if coords.lower() == 'lat':
-        del1 = np.deg2rad(del1) * _R_earth # convert lon to m
+        del1 = np.deg2rad(del1) * Rearth # convert lon to m
     else:
         raise Exception('unsupported coords for 2D case: ' + coords +
                         ', should be [lat-lon, cartesian]')
     
     del1Sqr = del1 ** 2.0
     epsilon = np.sin(np.pi/(2.0*gc1+2.0))**2
     optArg  = 2.0 / (1.0 + np.sqrt((2.0 - epsilon) * epsilon))
@@ -2230,20 +2287,25 @@
     """Update default invert parameters with user-defined ones."""
     
     if valid is not None and users != default:
         for k, v in users.items():
             if k not in valid:
                 raise Exception(f'mParams[\'{k}\'] is not used, valid are {valid}')
     
+    default_cp = copy.deepcopy(default)
+    
     for k, v in users.items():
         if v is not None:
-            default[k] = v
+            default_cp[k] = v
     
-    return default
+    return default_cp
 
+def __uniform_interval(coord1D, value):
+    if not np.isclose(coord1D.diff(coord1D.name), value).all():
+        raise Exception(f'coordinate {coord1D.name} is non-uniform:\n{coord1D}')
 
 def __print_params(params):
     """Print parameters for debugging."""
     if 'ratio' in params:
         print('dim grids  : ',
               params['gc2'], params['gc1'])
         print('dim intervs: ',
```

### Comparing `xinvert-0.1.3/xinvert/core.py` & `xinvert-0.1.7/xinvert/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 
 @author: MiniUFO
 Copyright 2018. All rights reserved. Use is subject to license terms.
 """
 from .numbas import invert_standard_3D, invert_standard_2D, invert_standard_1D,\
                     invert_general_3D, invert_general_2D, \
                     invert_general_bih_2D, invert_standard_2D_test
-from .utils import loop_noncore, _undeftmp
+from .utils import loop_noncore
+
+
+# default undefined value
+_undeftmp = -9.99e8
 
 """
 Below are the core methods of xinvert
 """
 def inv_standard3D(A, B, C, F, S, dims, iParams):
     r"""Inverting a 3D volume of elliptic equation in a standard form.
```

### Comparing `xinvert-0.1.3/xinvert/finitediffs.py` & `xinvert-0.1.7/xinvert/finitediffs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 @author: MiniUFO
 Copyright 2018. All rights reserved. Use is subject to license terms.
 """
 #%%
 import numpy as np
 import xarray as xr
-from .utils import _deg2m, _R_earth
 
 
 class FiniteDiff(object):
     """
     This class wrap some basic finite-difference operators supported for
     Cartesian coordinates (coords='cartesian') or latitude/longitude
     coordinates (coords='lat/lon'), using centered different scheme.
@@ -36,14 +35,16 @@
         points along 'X' dimension; or BCs={'Z': ('fixed','reflect')} for fixed
         left BC and reflected right BC.  Left indicates lower indices along 'X'.
     fill: float or dict
         Fill value if BCs are fixed.  A typical example can be:
         {'Z':(1,2), 'Y':(0,0), 'X':(1,0)}
     coords: {'lat-lon', 'cartesian'}
         Types of coords.  Should be one of ['lat-lon', 'cartesian'].
+    R: float
+        Radius of Earth.
     
     Methods
     -------
     grad(scalar)
         3D gradient.
     divg(vector)
         3D divergence.
@@ -58,15 +59,15 @@
     shear_strain(vector)
         Shear strain.
     deformation_rate(vector)
         Deformation rate.
     Okubo_Weiss(vector)
         Okubo Weiss parameter.
     """
-    def __init__(self, dim_mapping, BCs='extend', coords='lat-lon', fill=0):
+    def __init__(self, dim_mapping, BCs='extend', coords='lat-lon', fill=0, R=6371200.0):
         """Construct a FiniteDiff instance given dimension mapping
         
         Parameters
         ----------
         dim_mapping: dict
             Mapping 4D coordinates into ['T', 'Z', 'Y', 'X']. A typical case is:
                 {'T':'time', 'Z':'lev', 'Y':'lat', 'X':'lon'}.
@@ -83,14 +84,16 @@
             * 'extrapolate': pad with extrapolated value. (NOT implemented). 1st
               derivative equals the first inner point. 2nd derivative is exactly zero.
         coords: str
             Types of coords.  Should be one of ['lat-lon', 'cartesian'].
         fills: float or dict
             Fill value if BCs are fixed.  A typical example can be:
                 {'Z':(1,2), 'Y':(0,0), 'X':(1,0)}
+        R: float
+            Radius of Earth.
         """
         # Align dims and BCs with default one ('extend').
         if BCs is None:
             BCs = {}
             for dim in dim_mapping:
                 BCs[dim] = ('extend', 'extend')
         
@@ -124,14 +127,15 @@
                 if not dim in fill:
                     fill[dim] = (0, 0)
         
         self.dmap   = dim_mapping
         self.BCs    = BCs
         self.fill   = fill
         self.coords = coords
+        self.R      = R
         
         if coords not in ['lat-lon', 'cartesian']:
             raise Exception('unsupported coords: ' + coords +
                             ', should be one of [\'lat-lon\', \'cartesian\']')
     
     
     def __repr__(self):
@@ -176,21 +180,21 @@
         llc  = self.coords == 'lat-lon'
         re   = []
         
         for dim in dims:
             dimName = self.dmap[dim]
             
             if dim == 'Y' and llc:
-                scale = _deg2m
+                scale = np.pi * self.R / 180.0 # deg2m
             elif dim == 'X' and llc:
                 if 'Y' in self.dmap and self.dmap['Y'] in v.dims:
                     cos = np.cos(np.deg2rad(v[self.dmap['Y']]))
                 else:
                     cos = 1
-                scale = _deg2m * cos
+                scale = np.pi * self.R / 180.0 * cos # deg2m
             else:
                 scale = 1
             
             grd = deriv(v, dimName, BCs[dim], fill, scale)
             
             # if llc and dim == 'X' and 'Y' in self.dmap:
             #     grd = grd.where(np.abs(grd[self.dmap['Y']])!=90, other=0)
@@ -250,23 +254,23 @@
         
         for comp, dim in zip(vector, dims):
             dimName = self.dmap[dim]
             
             if llc and dim == 'Y':
                 # weight cos(lat)
                 cos = np.cos(np.deg2rad(comp[self.dmap['Y']]))
-                scale = _deg2m * cos
+                scale = np.pi * self.R / 180.0 * cos
                 tmp = comp * cos
             elif llc and dim == 'X':
                 # weight cos(lat)
                 if 'Y' in self.dmap and self.dmap['Y'] in vector[0].dims:
                     cos = np.cos(np.deg2rad(comp[self.dmap['Y']]))
                 else:
                     cos = 1
-                scale = _deg2m * cos
+                scale = np.pi * self.R / 180.0 * cos
                 tmp = comp
             else:
                 scale = 1
                 tmp = comp
             
             div = deriv(tmp, dimName, BCs[dim], fill, scale)
             
@@ -329,15 +333,15 @@
                     break
             
             if dims['Y'] in tmp.dims:
                 cos = np.cos(np.deg2rad(tmp[dims['Y']]))
             else:
                 cos = 1
                 
-            scale = _deg2m * cos
+            scale = np.deg2rad(1.0) * self.R * cos
         else:
             scale = 1.0
         
         vors = []
         for comp in components:
             if comp == 'i': # wy - vz
                 t  = w * cos if llc else w # weighted by cos(lat)
@@ -410,19 +414,19 @@
         for dim in dims:
             if llc and dim in ['X', 'Y']:
                 dimN  = dmap['Y']
                 latR  = np.deg2rad(v[dimN])
                 cosL  = np.cos(latR)
                 
                 if dim == 'Y':
-                    scale  = _deg2m
+                    scale  = np.pi * self.R / 180.0
                     metric = -deriv(v, dmap['Y'], BCs['Y'], fill['Y'],
-                                    scale) * np.tan(latR) / _R_earth
+                                    scale) * np.tan(latR) / self.R
                 else:
-                    scale = _deg2m * cosL
+                    scale = np.pi * self.R / 180.0 * cosL
                     metric = 0
             else:
                 scale = 1.0
                 metric = 0
             
             re.append(deriv2(v, dmap[dim], BCs[dim], fill[dim], scale) + metric)
```

### Comparing `xinvert-0.1.3/xinvert/numbas.py` & `xinvert-0.1.7/xinvert/numbas.py`

 * *Files identical despite different names*

### Comparing `xinvert-0.1.3/xinvert/utils.py` & `xinvert-0.1.7/xinvert/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,14 @@
 # -*- coding: utf-8 -*-
 """
 Created on 2021.01.03
 
 @author: MiniUFO
 Copyright 2018. All rights reserved. Use is subject to license terms.
 """
-#%%
-import numpy as np
-
-
-_R_earth = 6371200.0 # consistent with GrADS
-_omega = 7.292e-5    # angular speed of the earth rotation
-_g = 9.80665         # gravitational acceleration
-_undeftmp = -9.99e8  # default undefined value
-_deg2m = np.pi * _R_earth / 180.0
-
-_latlon = ['lat', 'latitude' , 'lats', 'yc', 'y',
-           'lon', 'longitude', 'long', 'xc', 'x']
 
 
 def loop_noncore(data, dims=None):
     """Loop over the non-core dimensions using generator.
 
     The non-core dimensions are given outside the list in `dims`.
```

### Comparing `xinvert-0.1.3/xinvert.egg-info/PKG-INFO` & `xinvert-0.1.7/xinvert.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 Metadata-Version: 2.1
 Name: xinvert
-Version: 0.1.3
+Version: 0.1.7
 Summary: Invert geofluid problems based on xarray, using SOR iteration
 Home-page: https://github.com/miniufo/xinvert
 Author: miniufo
 Author-email: miniufo@163.com
 License: MIT
 Keywords: invert inversion atmosphere ocean SOR successive-overrelaxation-iteration
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy
+Requires-Dist: xarray
+Requires-Dist: dask
+Requires-Dist: numba
 
 # xinvert
 
 [![DOI](https://zenodo.org/badge/323045845.svg)](https://zenodo.org/badge/latestdoi/323045845)
 ![GitHub](https://img.shields.io/github/license/miniufo/xinvert)
 [![Documentation Status](https://readthedocs.org/projects/xinvert/badge/?version=latest)](https://xinvert.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/xinvert.svg)](https://badge.fury.io/py/xinvert)
 ![Workflow](https://github.com/miniufo/xinvert/actions/workflows/python-publish.yml/badge.svg)
 [![pytest](https://github.com/miniufo/xinvert/actions/workflows/tests.yml/badge.svg)](https://github.com/miniufo/xinvert/actions/workflows/tests.yml)
 [![Build Status](https://app.travis-ci.com/miniufo/xinvert.svg?branch=master)](https://app.travis-ci.com/miniufo/xinvert)
+[![status](https://joss.theoj.org/papers/1fc4ac8f98c0778516971880727a3a94/status.svg)](https://joss.theoj.org/papers/1fc4ac8f98c0778516971880727a3a94)
+
 
 ![animate plot](https://raw.githubusercontent.com/miniufo/xinvert/master/pics/animateConverge.gif)
 
 
 ## 1. Introduction
 Researches on meteorology and oceanography usually encounter [inversion problems](https://doi.org/10.1017/CBO9780511629570) that need to be solved numerically.  One of the classical inversion problem is to solve Poisson equation for a streamfunction $\psi$ given the vertical component of vorticity $\zeta$ and proper boundary conditions.
 
@@ -32,15 +38,15 @@
 
 Nowadays [`xarray`](http://xarray.pydata.org/en/stable/) becomes a popular data structure commonly used in [Big Data Geoscience](https://pangeo.io/).  Since the whole 4D data, as well as the coordinate information, are all combined into [`xarray`](http://xarray.pydata.org/en/stable/), solving the inversion problem become quite straightforward and the only input would be just one [`xarray.DataArray`](http://xarray.pydata.org/en/stable/) of vorticity.  Inversion on the spherical earth, like some meteorological problems, could utilize the spherical harmonics like [windspharm](https://github.com/ajdawson/windspharm), which would be more efficient using FFT than SOR used here.  However, in the case of ocean, SOR method is definitely a better choice in the presence of irregular land/sea mask.
 
 More importantly, this could be generalized into a numerical solver for elliptical equation using [SOR](https://mathworld.wolfram.com/SuccessiveOverrelaxationMethod.html) method, with spatially-varying coefficients.  Various popular inversion problems in geofluid dynamics will be illustrated as examples.
 
 One problem with SOR is that the speed of iteration using **explicit loops in Python** will be **e-x-t-r-e-m-e-l-y ... s-l-o-w**!  A very suitable solution here is to use [`numba`](https://numba.pydata.org/).  We may try our best to speed things up using more hardwares (possibly GPU).
 
-Classical problems include Gill-Matsuno model, Stommel-Munk model, QG omega model, PV inversion model, Swayer-Eliassen balance model...  A complete list of the classical inversion problems can be found at [this notebook](./docs/source/notebooks/Introduction.ipynb).
+Classical problems include Gill-Matsuno model, Stommel-Munk model, QG omega model, PV inversion model, Swayer-Eliassen balance model...  A complete list of the classical inversion problems can be found at [this notebook](./docs/source/notebooks/00_Introduction.ipynb).
 
 Why `xinvert`?
 
 - **Thinking and coding in equations:** User APIs are very close to the equations: unknowns are on the LHS of `=`, whereas the known forcings are on its RHS;
 - **Genearlize all the steady-state problems:** All the known steady-state problems in geophysical fluid dynamics can be easily adapted to fit the solvers;
 - **Very short parameter list:** Passing a single `xarray` forcing is enough for the inversion.  Coordinates information is already encapsulated.
 - **Flexible model parameters:** Model paramters can be either a constant, or varying with a specific dimension (like Coriolis $f$), or fully varying with space and time, due to the use of `xarray`'s broadcasting capability;
@@ -88,7 +94,28 @@
 # output has 1 more dimension (iter) than input, which could be animated over.
 # Here 40 frames and loop 1 per frame (final state is after 40 iterations) is used.
 psi = animate_iteration(invert_Poisson, vor, iParams=iParams,
                         loop_per_frame=1, max_frames=40)
 ```
 
 See the animation at the top.
+
+
+
+## 5 Cite
+
+If you use the package in research, teaching, or other activities, we would be grateful
+if you mention `xinvert` and cite our paper in JOSS:
+
+```bibtex
+@article{Qian2023,
+    doi = {10.21105/joss.05510},
+    url = {https://doi.org/10.21105/joss.05510},
+    year = {2023},
+    publisher = {The Open Journal},
+    volume = {8},
+    number = {89},
+    pages = {5510},
+    author = {Yu-Kun Qian},
+    title = {xinvert: A Python package for inversion problems in geophysical fluid dynamics}, journal = {Journal of Open Source Software}
+}
+```
```

### Comparing `xinvert-0.1.3/xinvert.egg-info/SOURCES.txt` & `xinvert-0.1.7/xinvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

