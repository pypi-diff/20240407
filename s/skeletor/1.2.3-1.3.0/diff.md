# Comparing `tmp/skeletor-1.2.3.tar.gz` & `tmp/skeletor-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skeletor-1.2.3.tar", last modified: Wed Nov  9 15:15:13 2022, max compression
+gzip compressed data, was "skeletor-1.3.0.tar", last modified: Sun Apr  7 14:08:29 2024, max compression
```

## Comparing `skeletor-1.2.3.tar` & `skeletor-1.3.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (116)    35126 2022-11-09 15:15:10.000000 skeletor-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       97 2022-11-09 15:15:10.000000 skeletor-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5611 2022-11-09 15:15:13.000000 skeletor-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4571 2022-11-09 15:15:10.000000 skeletor-1.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-09 15:15:13.000000 skeletor-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1787 2022-11-09 15:15:10.000000 skeletor-1.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor/
--rw-r--r--   0 runner    (1001) docker     (116)    11162 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor/data/
--rw-r--r--   0 runner    (1001) docker     (116)   534422 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/data/722817260.obj
--rw-r--r--   0 runner    (1001) docker     (116)      399 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/data/README.md
--rw-r--r--   0 runner    (1001) docker     (116)     2027 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor/post/
--rw-r--r--   0 runner    (1001) docker     (116)     1623 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    20378 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/post/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (116)    13040 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/post/radiusextraction.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor/pre/
--rw-r--r--   0 runner    (1001) docker     (116)     1651 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11194 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/pre/meshcontraction.py
--rw-r--r--   0 runner    (1001) docker     (116)     9621 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/pre/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor/pre/templates/
--rw-r--r--   0 runner    (1001) docker     (116)     1182 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/pre/templates/blender_decimate.py.template
--rw-r--r--   0 runner    (1001) docker     (116)     1147 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/pre/templates/blender_remesh.py.template
--rw-r--r--   0 runner    (1001) docker     (116)    12987 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/pre/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor/skeletonize/
--rw-r--r--   0 runner    (1001) docker     (116)     2855 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8744 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    15176 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/edge_collapse.py
--rw-r--r--   0 runner    (1001) docker     (116)    11538 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/tangent_ball.py
--rw-r--r--   0 runner    (1001) docker     (116)     8212 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/teasar.py
--rw-r--r--   0 runner    (1001) docker     (116)    13982 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     7314 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/vertex_cluster.py
--rw-r--r--   0 runner    (1001) docker     (116)    11932 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/skeletonize/wave.py
--rw-r--r--   0 runner    (1001) docker     (116)     2387 2022-11-09 15:15:10.000000 skeletor-1.2.3/skeletor/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5611 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      918 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      134 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2022-11-09 15:15:13.000000 skeletor-1.2.3/skeletor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.354135 skeletor-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35126 2024-04-07 14:08:27.000000 skeletor-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-07 14:08:27.000000 skeletor-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-07 14:08:29.354135 skeletor-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-07 14:08:27.000000 skeletor-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:08:29.354135 skeletor-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-07 14:08:27.000000 skeletor-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.350135 skeletor-1.3.0/skeletor/
+-rw-r--r--   0 runner    (1001) docker     (127)    11738 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.350135 skeletor-1.3.0/skeletor/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   534422 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/data/722817260.obj
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.354135 skeletor-1.3.0/skeletor/post/
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24877 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/post/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13040 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/post/radiusextraction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.354135 skeletor-1.3.0/skeletor/pre/
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11482 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/pre/meshcontraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/pre/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.354135 skeletor-1.3.0/skeletor/pre/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/pre/templates/blender_decimate.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/pre/templates/blender_remesh.py.template
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/pre/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.354135 skeletor-1.3.0/skeletor/skeletonize/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15176 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/edge_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11538 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/tangent_ball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8212 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/teasar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13982 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/vertex_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/skeletonize/wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-07 14:08:27.000000 skeletor-1.3.0/skeletor/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.354135 skeletor-1.3.0/skeletor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5880 2024-04-07 14:08:29.000000 skeletor-1.3.0/skeletor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-07 14:08:29.000000 skeletor-1.3.0/skeletor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:08:29.000000 skeletor-1.3.0/skeletor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:08:29.000000 skeletor-1.3.0/skeletor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-07 14:08:29.000000 skeletor-1.3.0/skeletor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 14:08:29.000000 skeletor-1.3.0/skeletor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:08:29.354135 skeletor-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-07 14:08:27.000000 skeletor-1.3.0/tests/test_skeletor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `skeletor-1.2.3/LICENSE` & `skeletor-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/PKG-INFO` & `skeletor-1.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletor
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python 3 library to extract skeletons from 3D meshes
 Home-page: https://github.com/navis-org/skeletor
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://navis-org.github.io/skeletor/
 Project-URL: Source, https://github.com/navis-org/skeletor
@@ -17,14 +17,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.16.0
+Requires-Dist: trimesh>=2.38.0
+Requires-Dist: tqdm>=4.50.0
+Requires-Dist: scipy>=1.3.0
+Requires-Dist: pandas>=0.24.2
+Requires-Dist: networkx>=2.4
+Requires-Dist: scikit-learn>=0.23
+Requires-Dist: igraph>=0.8
+Requires-Dist: ncollpyde>=0.14.0
 
 [![Generic badge](https://img.shields.io/badge/Github-pages-green)](https://navis-org.github.io/skeletor/) [![Tests](https://github.com/navis-org/skeletor/actions/workflows/test-package.yml/badge.svg)](https://github.com/navis-org/skeletor/actions/workflows/test-package.yml) [![DOI](https://zenodo.org/badge/153085435.svg)](https://zenodo.org/badge/latestdoi/153085435)
 
 # Skeletor
 Unlike its [namesake](https://en.wikipedia.org/wiki/Skeletor), this Python 3
 library does not (yet) seek to conquer Eternia but to turn meshes into skeletons.
```

### Comparing `skeletor-1.2.3/README.md` & `skeletor-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/setup.py` & `skeletor-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/__init__.py` & `skeletor-1.3.0/skeletor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 # Getting started
 
 A skeletonization pipeline typically consists of:
 
 1. Some pre-processing of the mesh (e.g. fixing some potential errors like
    degenerate faces, unreferenced vertices, etc.)
 2. The skeletonization itself
-3. Some post-processing of the skeleton (e.g. adding radius information)
+3. Some post-processing of the skeleton (e.g. adding radius information, smoothing, etc.)
 
 ------
 
 Here is a complete list of available functions:
 
 | function                                    | description                                                 |
 | ------------------------------------------- | ----------------------------------------------------------- |
@@ -80,27 +80,31 @@
 | `skeletor.skeletonize.by_vertex_clusters()` | very fast but needs mesh to be contracted (see above)       |
 | `skeletor.skeletonize.by_edge_collapse()`   | presented in [1] but never got this to work well            |
 | `skeletor.skeletonize.by_teasar()`          | very fast and robust, works on mesh surface                 |
 | `skeletor.skeletonize.by_tangent_ball()`    | very fast, best on smooth meshes                            |
 | **postprocessing**                          |                                                             |
 | `skeletor.post.clean_up()`                  | fix some potential errors in the skeleton                   |
 | `skeletor.post.radii()`                     | add radius information using various method                 |
+| `skeletor.post.smooth()`                    | smooth the skeleton                                         |
+| `skeletor.post.remove_bristles()`           | remove single-node bristles from the skeleton               |
+| `skeletor.post.despike()`                   | smooth out jumps in the skeleton                            |
 
 ------
 
 See docstrings of the respective functions for details.
 
 A pipeline might look like this:
 
  1. `skeletor.pre.fix_mesh()` to fix the mesh
  2. `skeletor.pre.simplify()` to simplify the mesh
  3. `skeletor.pre.contract()` to contract the mesh [1]
- 4. `skeletor.skeletonize.vertex_clusters()` to generate a skeleton
+ 4. `skeletor.skeletonize.by_vertex_clusters()` to generate a skeleton
  5. `skeletor.post.clean_up()` to clean up some potential issues with the skeleton
- 6. `skeletor.post.radii()` to extract radii either by k-nearest neighbours or ray-casting
+ 6. `skeletor.post.smooth()` to smooth the skeleton
+ 7. `skeletor.post.radii()` to extract radii either by k-nearest neighbours or ray-casting
 
 In my experience there is no one-size-fits-all. You will have to play around to
 find the right approach and parameters to get nice skeletons for your meshes.
 If you need help just open an [issue](https://github.com/navis-org/skeletor/issues).
 
 Also check out the Gotchas below!
 
@@ -190,15 +194,15 @@
 
 ```Python
 >>> import skeletor as sk
 >>> # Load the example mesh that ships with skeletor
 >>> mesh = sk.example_mesh()
 >>> # Alternatively use trimesh to load/construct your own mesh:
 >>> # import trimesh as tm
->>> # mesh = tm.Trimesh(vertices, faces) 
+>>> # mesh = tm.Trimesh(vertices, faces)
 >>> # mesh = tm.load_mesh('some/mesh.obj')
 >>> # Run some general clean-up (see docstring for details)
 >>> fixed = sk.pre.fix_mesh(mesh, remove_disconnected=5, inplace=False)
 >>> # Contract mesh to 10% (0.1) of original volume
 >>> cont = sk.pre.contract(fixed, epsilon=0.1)
 >>> # Skeletonize
 >>> skel = sk.skeletonize.by_vertex_clusters(cont, sampling_dist=100)
@@ -213,17 +217,20 @@
 
 - while this is a general purpose library, my personal focus is on neurons and
   this has certainly influenced things like default parameter values and certain
   post-processing steps
 - meshes need to be triangular (we are using `trimesh`)
 - use `sk.pre.simplify` if your mesh is very complex (half a million vertices is
   where things start getting sluggish)
-- a good mesh contraction is often half the battle
+- a good mesh contraction is often half the battle but it can be tricky to get
+  to work
 - if the mesh consists of multiple disconnected pieces the skeleton will
   likewise be fragmented (i.e. will have multiple roots)
+- it's often a good idea to fix issues with the skeleton in postprocessing rather
+  than trying to get the skeletonization to be perfect
 
 # Benchmarks
 
 <img src="https://github.com/navis-org/skeletor/raw/master/benchmarks/benchmark_2.png" alt="skeletor_benchmark" width="100%"/>
 
 [Benchmarks](https://github.com/navis-org/skeletor/blob/master/benchmarks/skeletor_benchmark.ipynb)
 were run on a 2018 MacBook Pro (2.2 GHz Core i7, 32Gb memory) with optional
@@ -252,16 +259,16 @@
 # Top-level functions and classes
 At top-level we only expose `example_mesh()` and the `Skeleton` class (which
 you probably won't ever need to touch manually). Everything else is neatly
 tucked away into submodules (see side-bar or above table).
 
 """
 
-__version__ = "1.2.3"
-__version_vector__ = (1, 2, 3)
+__version__ = "1.3.0"
+__version_vector__ = (1, 3, 0)
 
 from . import skeletonize
 from . import pre
 from . import post
 
 from .skeletonize.base import Skeleton
 from .data import example_mesh
```

### Comparing `skeletor-1.2.3/skeletor/data/722817260.obj` & `skeletor-1.3.0/skeletor/data/722817260.obj`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/data/__init__.py` & `skeletor-1.3.0/skeletor/data/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/post/__init__.py` & `skeletor-1.3.0/skeletor/post/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,20 +25,27 @@
 
 `skeletor.post.clean_up` can help you solve some potential issues:
 
 - skeleton nodes (vertices) that outside or right on the surface instead of
   centered inside the mesh
 - superfluous "hairs" on otherwise straight bits
 
+`skeletor.post.smooth` will smooth out the skeleton.
+
+`skeletor.post.despike` can help you remove spikes in the skeleton where
+single nodes are out of aligment.
+
+`skeletor.post.remove_bristles` will remove bristles from the skeleton.
+
 ### Computing radius information
 
 Only `skeletor.skeletonize.by_wavefront()` provides radii off the bat. For all
 other methods, you might want to run `skeletor.post.radii` can help you
 (re-)generate radius information for the skeletons.
 
 """
 
 from .radiusextraction import radii
-from .postprocessing import clean_up
+from .postprocessing import clean_up, smooth, despike, remove_bristles
 
 __docformat__ = "numpy"
-__all__ = ['radii', 'clean_up']
+__all__ = ["radii", "clean_up", "smooth", "despike", "remove_bristles"]
```

### Comparing `skeletor-1.2.3/skeletor/post/postprocessing.py` & `skeletor-1.3.0/skeletor/post/postprocessing.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,38 +84,37 @@
 
     # Recenter vertices
     _ = recenter_vertices(s, mesh, inplace=True)
 
     return s
 
 
-def remove_hairs(s, mesh=None, inplace=False):
-    """Remove "hairs" that sometimes occurr along the backbone.
+def remove_bristles(s, mesh=None, los_only=False, inplace=False):
+    """Remove "bristles" that sometimes occurr along the backbone.
 
-    Works by finding terminal twigs that consist of only a single node. We will
-    then remove those that are within line of sight of their parent.
-
-    Note that this is currently not used for clean up as it does not work very
-    well: removes as many correct hairs as genuine small branches.
+    Works by finding terminal twigs that consist of only a single node.
 
     Parameters
     ----------
     s :         skeletor.Skeleton
                 Skeleton to clean up.
     mesh :      trimesh.Trimesh, optional
                 Original mesh (e.g. before contraction). If not provided will
                 use the mesh associated with ``s``.
+    los_only :  bool
+                If True, will only remove bristles that are in line of sight of
+                their parent. If False, will remove all single-node bristles.
     inplace :   bool
                 If False will make and return a copy of the skeleton. If True,
                 will modify the `s` inplace.
 
     Returns
     -------
-    SWC :       pandas.DataFrame
-                SWC with line-of-sight twigs removed.
+    s :         skeletor.Skeleton
+                Skeleton with single-node twigs removed.
 
     """
     if isinstance(mesh, type(None)):
         mesh = s.mesh
 
     # Make a copy of the skeleton
     if not inplace:
@@ -128,35 +127,38 @@
     # Find terminal twigs
     twigs = s.swc[~s.swc.node_id.isin(s.swc.parent_id)]
     twigs = twigs[twigs.parent_id.isin(bp)]
 
     if twigs.empty:
         return s
 
-    # Initialize ncollpyde Volume
-    coll = ncollpyde.Volume(mesh.vertices, mesh.faces, validate=False)
-
-    # Remove twigs that aren't inside the volume
-    twigs = twigs[coll.contains(twigs[['x', 'y', 'z']].values)]
-
-    # Generate rays between all pairs and their parents
-    sources = twigs[['x', 'y', 'z']].values
-    targets = s.swc.set_index('node_id').loc[twigs.parent_id,
-                                             ['x', 'y', 'z']].values
-
-    # Get intersections: `ix` points to index of line segment; `loc` is the
-    #  x/y/z coordinate of the intersection and `is_backface` is True if
-    # intersection happened at the inside of a mesh
-    ix, loc, is_backface = coll.intersections(sources, targets)
-
-    # Find pairs of twigs with no intersection - i.e. with line of sight
-    los = ~np.isin(np.arange(sources.shape[0]), ix)
-
-    # To remove: have line of sight
-    to_remove = twigs[los]
+    if los_only:
+        # Initialize ncollpyde Volume
+        coll = ncollpyde.Volume(mesh.vertices, mesh.faces, validate=False)
+
+        # Remove twigs that aren't inside the volume
+        twigs = twigs[coll.contains(twigs[['x', 'y', 'z']].values)]
+
+        # Generate rays between all pairs and their parents
+        sources = twigs[['x', 'y', 'z']].values
+        targets = s.swc.set_index('node_id').loc[twigs.parent_id,
+                                                ['x', 'y', 'z']].values
+
+        # Get intersections: `ix` points to index of line segment; `loc` is the
+        #  x/y/z coordinate of the intersection and `is_backface` is True if
+        # intersection happened at the inside of a mesh
+        ix, loc, is_backface = coll.intersections(sources, targets)
+
+        # Find pairs of twigs with no intersection - i.e. with line of sight
+        los = ~np.isin(np.arange(sources.shape[0]), ix)
+
+        # To remove: have line of sight
+        to_remove = twigs[los]
+    else:
+        to_remove = twigs
 
     s.swc = s.swc[~s.swc.node_id.isin(to_remove.node_id)].copy()
 
     # Update the mesh map
     mesh_map = getattr(s, 'mesh_map', None)
     if not isinstance(mesh_map, type(None)):
         for t in to_remove.itertuples():
@@ -188,16 +190,16 @@
                 Original mesh.
     inplace :   bool
                 If False will make and return a copy of the skeleton. If True,
                 will modify the `s` inplace.
 
     Returns
     -------
-    SWC :       pandas.DataFrame
-                SWC with line-of-sight twigs removed.
+    s :         skeletor.Skeleton
+                Skeleton with vertices recentered.
 
     """
     if isinstance(mesh, type(None)):
         mesh = s.mesh
 
     # Copy skeleton
     if not inplace:
@@ -337,16 +339,16 @@
                 of the longest edge in skeleton as limit.
     inplace :   bool
                 If False will make and return a copy of the skeleton. If True,
                 will modify the `s` inplace.
 
     Returns
     -------
-    SWC :       pandas.DataFrame
-                SWC with line-of-sight twigs removed.
+    s :         skeletor.Skeleton
+                Skeleton with line-of-sight twigs removed.
 
     """
     # Make a copy of the SWC
     if not inplace:
         s = s.copy()
 
     # Add distance to parents
@@ -462,15 +464,15 @@
                 theta = more pruning.
     inplace :   bool
                 If False will make and return a copy of the skeleton. If True,
                 will modify the `s` inplace.
 
     Returns
     -------
-    SWC :       pandas.DataFrame
+    s :         skeletor.Skeleton
                 SWC with parallel twigs removed.
 
     """
     assert isinstance(theta, numbers.Number), "theta must be a number"
     assert 0 <= theta <= 1, "theta must be between 0 and 1"
 
     # Work on a copy of the SWC table
@@ -543,7 +545,138 @@
             for t in to_remove.itertuples():
                 mesh_map[mesh_map == t.node_id] = t.parent_id
 
         # Reindex nodes
         s.reindex(inplace=True)
 
     return s
+
+def smooth(s,
+           window: int = 3,
+           to_smooth: list = ['x', 'y', 'z'],
+           inplace: bool = False):
+    """Smooth skeleton using rolling windows.
+
+    Parameters
+    ----------
+    s :             skeletor.Skeleton
+                    Skeleton to be processed.
+    window :        int, optional
+                    Size (N observations) of the rolling window in number of
+                    nodes.
+    to_smooth :     list
+                    Columns of the node table to smooth. Should work with any
+                    numeric column (e.g. 'radius').
+    inplace :       bool
+                    If False will make and return a copy of the skeleton. If
+                    True, will modify the `s` inplace.
+
+    Returns
+    -------
+    s :             skeletor.Skeleton
+                    Skeleton with smoothed node table.
+
+    """
+    if not inplace:
+        s = s.copy()
+
+    # Prepare nodes (add parent_dist for later, set index)
+    nodes = s.swc.set_index('node_id', inplace=False).copy()
+
+    to_smooth = np.array(to_smooth)
+    miss = to_smooth[~np.isin(to_smooth, nodes.columns)]
+    if len(miss):
+        raise ValueError(f'Column(s) not found in node table: {miss}')
+
+    # Go over each segment and smooth
+    for seg in s.get_segments():
+        # Get this segment's parent distances and get cumsum
+        this_co = nodes.loc[seg, to_smooth]
+
+        interp = this_co.rolling(window, min_periods=1).mean()
+
+        nodes.loc[seg, to_smooth] = interp.values
+
+    # Reassign nodes
+    s.swc = nodes.reset_index(drop=False, inplace=False)
+
+    return s
+
+def despike(s,
+            sigma = 5,
+            max_spike_length = 1,
+            inplace = False,
+            reverse = False):
+    r"""Remove spikes in skeleton.
+
+    For each node A, the euclidean distance to its next successor (parent)
+    B and that node's successor C (i.e A->B->C) is computed. If
+    :math:`\\frac{dist(A,B)}{dist(A,C)}>sigma`, node B is considered a spike
+    and realigned between A and C.
+
+    Parameters
+    ----------
+    x :                 skeletor.Skeleton
+                        Skeleton to be processed.
+    sigma :             float | int, optional
+                        Threshold for spike detection. Smaller sigma = more
+                        aggressive spike detection.
+    max_spike_length :  int, optional
+                        Determines how long (# of nodes) a spike can be.
+    inplace :           bool, optional
+                        If False, a copy of the neuron is returned.
+    reverse :           bool, optional
+                        If True, will **also** walk the segments from proximal
+                        to distal. Use this to catch spikes on e.g. terminal
+                        nodes.
+
+    Returns
+    -------
+    s                   skeletor.Skeleton
+                        Despiked neuron.
+
+    """
+    if not inplace:
+        s = s.copy()
+
+    # Index nodes table by node ID
+    this_nodes = s.swc.set_index('node_id', inplace=False)
+
+    segments = s.get_segments()
+    segs_to_walk = segments
+
+    if reverse:
+        segs_to_walk += segs_to_walk[::-1]
+
+    # For each spike length do -> do this in reverse to correct the long
+    # spikes first
+    for l in list(range(1, max_spike_length + 1))[::-1]:
+        # Go over all segments
+        for seg in segs_to_walk:
+            # Get nodes A, B and C of this segment
+            this_A = this_nodes.loc[seg[:-l - 1]]
+            this_B = this_nodes.loc[seg[l:-1]]
+            this_C = this_nodes.loc[seg[l + 1:]]
+
+            # Get coordinates
+            A = this_A[['x', 'y', 'z']].values
+            B = this_B[['x', 'y', 'z']].values
+            C = this_C[['x', 'y', 'z']].values
+
+            # Calculate euclidian distances A->B and A->C
+            dist_AB = np.linalg.norm(A - B, axis=1)
+            dist_AC = np.linalg.norm(A - C, axis=1)
+
+            # Get the spikes
+            spikes_ix = np.where(np.divide(dist_AB, dist_AC, where=dist_AC != 0) > sigma)[0]
+            spikes = this_B.iloc[spikes_ix]
+
+            if not spikes.empty:
+                # Interpolate new position(s) between A and C
+                new_positions = A[spikes_ix] + (C[spikes_ix] - A[spikes_ix]) / 2
+
+                this_nodes.loc[spikes.index, ['x', 'y', 'z']] = new_positions
+
+    # Reassign node table
+    s.swc = this_nodes.reset_index(drop=False, inplace=False)
+
+    return s
```

### Comparing `skeletor-1.2.3/skeletor/post/radiusextraction.py` & `skeletor-1.3.0/skeletor/post/radiusextraction.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/pre/__init__.py` & `skeletor-1.3.0/skeletor/pre/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/pre/meshcontraction.py` & `skeletor-1.3.0/skeletor/pre/meshcontraction.py`

 * *Files 9% similar despite different names*

```diff
@@ -161,19 +161,25 @@
                   "{rate_fmt}, epsilon {postfix[2]:.2g}")
     with tqdm(total=100,
               bar_format=bar_format,
               disable=progress is False,
               postfix=[1, iter_lim, 1]) as pbar:
         for i in range(iter_lim):
             # Get Laplace weights
+
             if operator == 'cotangent':
                 L = laplacian_cotangent(dm, normalized=True)
             else:
                 L = laplacian_umbrella(dm)
-
+            """
+            import robust_laplacian
+            L, M_ = robust_laplacian.mesh_laplacian(np.array(dm.vertices),
+                                                    np.array(dm.faces),
+                                                    mollify_factor=1e-3)
+            """
             V = getMeshVPos(dm)
             A = sp.sparse.vstack([WL.dot(L), WH])
             b = np.vstack((zeros, WH.dot(V)))
 
             cpts = np.zeros((n, 3))
             for j in range(3):
                 """
```

### Comparing `skeletor-1.2.3/skeletor/pre/preprocessing.py` & `skeletor-1.3.0/skeletor/pre/preprocessing.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/pre/templates/blender_decimate.py.template` & `skeletor-1.3.0/skeletor/pre/templates/blender_decimate.py.template`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/pre/templates/blender_remesh.py.template` & `skeletor-1.3.0/skeletor/pre/templates/blender_remesh.py.template`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/pre/utils.py` & `skeletor-1.3.0/skeletor/pre/utils.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/skeletonize/__init__.py` & `skeletor-1.3.0/skeletor/skeletonize/__init__.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/skeletonize/base.py` & `skeletor-1.3.0/skeletor/skeletonize/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -161,18 +161,83 @@
         nodes = self.swc.loc[not_root]
         parents = self.swc.set_index('node_id').loc[self.swc.loc[not_root, 'parent_id'].values]
 
         dists = nodes[['x', 'y', 'z']].values - parents[['x', 'y', 'z']].values
         dists = np.sqrt((dists ** 2).sum(axis=1))
 
         G = nx.DiGraph()
+        G.add_nodes_from(self.swc.node_id.values)
         G.add_weighted_edges_from(zip(nodes.node_id.values, nodes.parent_id.values, dists))
 
         return G
 
+    def get_segments(self,
+                     weight = 'weight',
+                     return_lengths = False):
+        """Generate a list of linear segments while maximizing segment lengths.
+
+        Parameters
+        ----------
+        weight :    'weight' | None, optional
+                    If ``"weight"`` use physical, geodesic length to determine
+                    segment length. If ``None`` use number of nodes (faster).
+        return_lengths : bool
+                    If True, also return lengths of segments according to ``weight``.
+
+        Returns
+        -------
+        segments :  list
+                    Segments as list of lists containing node IDs. List is
+                    sorted by segment lengths.
+        lengths :   list
+                    Length for each segment according to ``weight``. Only provided
+                    if `return_lengths` is True.
+
+        """
+        assert weight in ('weight', None), f'Unable to use weight "{weight}"'
+
+        # Get graph representation
+        G = self.get_graph()
+
+        # Get distances to root
+        dists = {}
+        for root in self.swc[self.swc.parent_id < 0].node_id.values:
+            dists.update(nx.shortest_path_length(G, target=root, weight=weight))
+
+        # Sort leaf nodes
+        endNodeIDs = self.leafs[self.leafs.parent_id >= 0].node_id.values
+        endNodeIDs = sorted(endNodeIDs, key=lambda x: dists.get(x, 0), reverse=True)
+
+        seen: set = set()
+        sequences = []
+        for nodeID in endNodeIDs:
+            sequence = [nodeID]
+            parents = list(G.successors(nodeID))
+            while True:
+                if not parents:
+                    break
+                parentID = parents[0]
+                sequence.append(parentID)
+                if parentID in seen:
+                    break
+                seen.add(parentID)
+                parents = list(G.successors(parentID))
+
+            if len(sequence) > 1:
+                sequences.append(sequence)
+
+        # Sort sequences by length
+        lengths = [dists[s[0]] - dists[s[-1]] for s in sequences]
+        sequences = [x for _, x in sorted(zip(lengths, sequences), reverse=True)]
+
+        if return_lengths:
+            return sequences, sorted(lengths, reverse=True)
+        else:
+            return sequences
+
     def save_swc(self, filepath):
         """Save skeleton in SWC format.
 
         Parameters
         ----------
         filepath :      path-like
                         Filepath to save SWC to.
```

### Comparing `skeletor-1.2.3/skeletor/skeletonize/edge_collapse.py` & `skeletor-1.3.0/skeletor/skeletonize/edge_collapse.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/skeletonize/tangent_ball.py` & `skeletor-1.3.0/skeletor/skeletonize/tangent_ball.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/skeletonize/teasar.py` & `skeletor-1.3.0/skeletor/skeletonize/teasar.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/skeletonize/utils.py` & `skeletor-1.3.0/skeletor/skeletonize/utils.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/skeletonize/vertex_cluster.py` & `skeletor-1.3.0/skeletor/skeletonize/vertex_cluster.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/skeletonize/wave.py` & `skeletor-1.3.0/skeletor/skeletonize/wave.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor/utilities.py` & `skeletor-1.3.0/skeletor/utilities.py`

 * *Files identical despite different names*

### Comparing `skeletor-1.2.3/skeletor.egg-info/PKG-INFO` & `skeletor-1.3.0/skeletor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletor
-Version: 1.2.3
+Version: 1.3.0
 Summary: Python 3 library to extract skeletons from 3D meshes
 Home-page: https://github.com/navis-org/skeletor
 Author: Philipp Schlegel
 Author-email: pms70@cam.ac.uk
 License: GNU GPL V3
 Project-URL: Documentation, https://navis-org.github.io/skeletor/
 Project-URL: Source, https://github.com/navis-org/skeletor
@@ -17,14 +17,23 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: numpy>=1.16.0
+Requires-Dist: trimesh>=2.38.0
+Requires-Dist: tqdm>=4.50.0
+Requires-Dist: scipy>=1.3.0
+Requires-Dist: pandas>=0.24.2
+Requires-Dist: networkx>=2.4
+Requires-Dist: scikit-learn>=0.23
+Requires-Dist: igraph>=0.8
+Requires-Dist: ncollpyde>=0.14.0
 
 [![Generic badge](https://img.shields.io/badge/Github-pages-green)](https://navis-org.github.io/skeletor/) [![Tests](https://github.com/navis-org/skeletor/actions/workflows/test-package.yml/badge.svg)](https://github.com/navis-org/skeletor/actions/workflows/test-package.yml) [![DOI](https://zenodo.org/badge/153085435.svg)](https://zenodo.org/badge/latestdoi/153085435)
 
 # Skeletor
 Unlike its [namesake](https://en.wikipedia.org/wiki/Skeletor), this Python 3
 library does not (yet) seek to conquer Eternia but to turn meshes into skeletons.
```

### Comparing `skeletor-1.2.3/skeletor.egg-info/SOURCES.txt` & `skeletor-1.3.0/skeletor.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -25,8 +25,9 @@
 skeletor/skeletonize/__init__.py
 skeletor/skeletonize/base.py
 skeletor/skeletonize/edge_collapse.py
 skeletor/skeletonize/tangent_ball.py
 skeletor/skeletonize/teasar.py
 skeletor/skeletonize/utils.py
 skeletor/skeletonize/vertex_cluster.py
-skeletor/skeletonize/wave.py
+skeletor/skeletonize/wave.py
+tests/test_skeletor.py
```

