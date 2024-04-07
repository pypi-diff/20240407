# Comparing `tmp/specnn4pde-0.0.3.tar.gz` & `tmp/specnn4pde-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specnn4pde-0.0.3.tar", last modified: Wed Apr  3 08:29:05 2024, max compression
+gzip compressed data, was "specnn4pde-0.0.4.tar", last modified: Sun Apr  7 02:45:18 2024, max compression
```

## Comparing `specnn4pde-0.0.3.tar` & `specnn4pde-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:29:05.764980 specnn4pde-0.0.3/
--rw-rw-rw-   0        0        0     1091 2024-04-03 06:49:12.000000 specnn4pde-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2716 2024-04-03 08:29:05.764980 specnn4pde-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1654 2024-04-03 06:39:13.000000 specnn4pde-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 08:29:05.766407 specnn4pde-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1709 2024-04-03 08:28:54.000000 specnn4pde-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:29:05.749855 specnn4pde-0.0.3/specnn4pde/
--rw-rw-rw-   0        0        0        0 2023-11-10 02:06:30.000000 specnn4pde-0.0.3/specnn4pde/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-03-15 09:39:53.000000 specnn4pde-0.0.3/specnn4pde/linalg.py
--rw-rw-rw-   0        0        0    12133 2024-04-03 03:41:58.000000 specnn4pde-0.0.3/specnn4pde/npde.py
--rw-rw-rw-   0        0        0    16254 2024-04-03 05:24:24.000000 specnn4pde-0.0.3/specnn4pde/spectral.py
--rw-rw-rw-   0        0        0     6621 2024-03-20 02:37:42.000000 specnn4pde-0.0.3/specnn4pde/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:29:05.763983 specnn4pde-0.0.3/specnn4pde.egg-info/
--rw-rw-rw-   0        0        0     2716 2024-04-03 08:29:05.000000 specnn4pde-0.0.3/specnn4pde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-03 08:29:05.000000 specnn4pde-0.0.3/specnn4pde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:29:05.000000 specnn4pde-0.0.3/specnn4pde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-03 08:29:05.000000 specnn4pde-0.0.3/specnn4pde.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 08:29:05.000000 specnn4pde-0.0.3/specnn4pde.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 02:45:18.077203 specnn4pde-0.0.4/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 06:49:12.000000 specnn4pde-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2716 2024-04-07 02:45:18.076205 specnn4pde-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1654 2024-04-05 03:16:54.000000 specnn4pde-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 02:45:18.078200 specnn4pde-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1709 2024-04-07 02:45:06.000000 specnn4pde-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:45:18.061191 specnn4pde-0.0.4/specnn4pde/
+-rw-rw-rw-   0        0        0       37 2024-04-05 03:16:25.000000 specnn4pde-0.0.4/specnn4pde/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-03-15 09:39:53.000000 specnn4pde-0.0.4/specnn4pde/linalg.py
+-rw-rw-rw-   0        0        0     9192 2024-04-06 15:04:07.000000 specnn4pde-0.0.4/specnn4pde/nn.py
+-rw-rw-rw-   0        0        0    12133 2024-04-03 03:41:58.000000 specnn4pde-0.0.4/specnn4pde/npde.py
+-rw-rw-rw-   0        0        0    16238 2024-04-04 03:16:10.000000 specnn4pde-0.0.4/specnn4pde/spectral.py
+-rw-rw-rw-   0        0        0     6621 2024-03-20 02:37:42.000000 specnn4pde-0.0.4/specnn4pde/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:45:18.075204 specnn4pde-0.0.4/specnn4pde.egg-info/
+-rw-rw-rw-   0        0        0     2716 2024-04-07 02:45:17.000000 specnn4pde-0.0.4/specnn4pde.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2024-04-07 02:45:18.000000 specnn4pde-0.0.4/specnn4pde.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:45:17.000000 specnn4pde-0.0.4/specnn4pde.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-07 02:45:17.000000 specnn4pde-0.0.4/specnn4pde.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 02:45:17.000000 specnn4pde-0.0.4/specnn4pde.egg-info/top_level.txt
```

### Comparing `specnn4pde-0.0.3/LICENSE` & `specnn4pde-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.3/PKG-INFO` & `specnn4pde-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specnn4pde
-Version: 0.0.3
+Version: 0.0.4
 Summary: Solving partial differential equations using spectral methods and neural networks.
 Home-page: https://github.com/mxweng/specnn4pde
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 Requires-Dist: sympy
 
 # SpecNN4PDE
 SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
 - `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
 - `linalg`: This module primarily focuses on numerical algebra methods.
-- `tools`: A collection of utility functions for system and package information retrieval, time measurement, etc.
+- `utils`: A collection of utility functions for system and package information retrieval, time measurement, etc.
 - `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 
 This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
 When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
```

### Comparing `specnn4pde-0.0.3/README.md` & `specnn4pde-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SpecNN4PDE
 SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
 - `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
 - `linalg`: This module primarily focuses on numerical algebra methods.
-- `tools`: A collection of utility functions for system and package information retrieval, time measurement, etc.
+- `utils`: A collection of utility functions for system and package information retrieval, time measurement, etc.
 - `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 
 This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
 When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
```

### Comparing `specnn4pde-0.0.3/setup.py` & `specnn4pde-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.command import install_data
 from setuptools import setup, find_packages
 
 setup(
     name='specnn4pde',  # package name
-    version='0.0.3',  # version
+    version='0.0.4',  # version
     author='MXWeng',  # author name
     author_email='2431141461@qq.com',  # author email
     description='Solving partial differential equations using spectral methods and neural networks.',  # short description
     long_description=open('README.md').read(),  # long description, usually your README
     long_description_content_type='text/markdown',  # format of the long description, 'text/markdown' if it's Markdown
     url='https://github.com/mxweng/specnn4pde',  # project homepage
     packages=find_packages(),  # automatically discover all packages
```

### Comparing `specnn4pde-0.0.3/specnn4pde/linalg.py` & `specnn4pde-0.0.4/specnn4pde/linalg.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.3/specnn4pde/npde.py` & `specnn4pde-0.0.4/specnn4pde/npde.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.3/specnn4pde/spectral.py` & `specnn4pde-0.0.4/specnn4pde/spectral.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,15 +385,15 @@
 
 def glue1D(interval, Ncell, D, r, w, end_pts = False):
     """
     Glue the differential matrix D, Gauss points r, and quadrature weights w on each cell together.
 
     Parameters
     ----------
-    interval : list or tuple, length 2
+    interval : (2,) array_like
         The left and right edge of the domain.
     Ncell : int
         The number of cells.
     D, r, w : ndarray
         The differential matrix, Gauss points, and quadrature weights on the reference cell [-1, 1],
         which can be generated by `spectral.Jacobi_Gauss`, `spectral.Jacobi_Gauss_Lobatto`.
     end_pts : bool, optional
@@ -430,15 +430,15 @@
 
 def glue_pts_1D(interval, Ncell, r, end_pts = False):
     """
     Glue the points r on each cell together.
 
     Parameters
     ----------
-    interval : list or tuple, length 2
+    interval : (2,) array_like
         The left and right edge of the domain.
     Ncell : int
         The number of cells.
     r : ndarray
         The collocation points on the reference cell [-1, 1],
     end_pts : bool, optional
         Whether the end points -1, 1 are included in r or not. The default is False.
```

### Comparing `specnn4pde-0.0.3/specnn4pde/tools.py` & `specnn4pde-0.0.4/specnn4pde/utils.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.3/specnn4pde.egg-info/PKG-INFO` & `specnn4pde-0.0.4/specnn4pde.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specnn4pde
-Version: 0.0.3
+Version: 0.0.4
 Summary: Solving partial differential equations using spectral methods and neural networks.
 Home-page: https://github.com/mxweng/specnn4pde
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,15 +28,15 @@
 Requires-Dist: sympy
 
 # SpecNN4PDE
 SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
 - `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
 - `linalg`: This module primarily focuses on numerical algebra methods.
-- `tools`: A collection of utility functions for system and package information retrieval, time measurement, etc.
+- `utils`: A collection of utility functions for system and package information retrieval, time measurement, etc.
 - `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
 
 This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
 When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
```

