# Comparing `tmp/jo3mnist-0.0.3.tar.gz` & `tmp/jo3mnist-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jo3mnist-0.0.3.tar", last modified: Wed Dec 13 11:01:13 2023, max compression
+gzip compressed data, was "jo3mnist-0.0.4.tar", last modified: Sun Apr  7 08:56:07 2024, max compression
```

## Comparing `jo3mnist-0.0.3.tar` & `jo3mnist-0.0.4.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2023-12-13 11:01:13.687250 jo3mnist-0.0.3/
--rw-r--r--   0 gum       (1001) gum       (1001)     1069 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/LICENSE
--rw-r--r--   0 gum       (1001) gum       (1001)      983 2023-12-13 11:01:13.687250 jo3mnist-0.0.3/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)      391 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/README.md
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2023-12-13 11:01:13.683916 jo3mnist-0.0.3/jo3mnist/
--rw-r--r--   0 gum       (1001) gum       (1001)       94 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/jo3mnist/__init__.py
--rw-r--r--   0 gum       (1001) gum       (1001)     6946 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/jo3mnist/__main__.py
--rw-r--r--   0 gum       (1001) gum       (1001)      882 2023-12-13 10:51:39.000000 jo3mnist-0.0.3/jo3mnist/data.py
--rw-r--r--   0 gum       (1001) gum       (1001)     4528 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/jo3mnist/equinox.py
--rw-r--r--   0 gum       (1001) gum       (1001)      703 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/jo3mnist/vis.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2023-12-13 11:01:13.687250 jo3mnist-0.0.3/jo3mnist.egg-info/
--rw-r--r--   0 gum       (1001) gum       (1001)      983 2023-12-13 11:01:13.000000 jo3mnist-0.0.3/jo3mnist.egg-info/PKG-INFO
--rw-r--r--   0 gum       (1001) gum       (1001)      394 2023-12-13 11:01:13.000000 jo3mnist-0.0.3/jo3mnist.egg-info/SOURCES.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        1 2023-12-13 11:01:13.000000 jo3mnist-0.0.3/jo3mnist.egg-info/dependency_links.txt
--rw-r--r--   0 gum       (1001) gum       (1001)       67 2023-12-13 11:01:13.000000 jo3mnist-0.0.3/jo3mnist.egg-info/requires.txt
--rw-r--r--   0 gum       (1001) gum       (1001)        9 2023-12-13 11:01:13.000000 jo3mnist-0.0.3/jo3mnist.egg-info/top_level.txt
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2023-12-13 11:01:13.687250 jo3mnist-0.0.3/mnist/
--rw-r--r--   0 gum       (1001) gum       (1001)       94 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/mnist/__init__.py
--rw-r--r--   0 gum       (1001) gum       (1001)     6946 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/mnist/__main__.py
--rw-r--r--   0 gum       (1001) gum       (1001)      882 2023-12-13 10:51:39.000000 jo3mnist-0.0.3/mnist/data.py
--rw-r--r--   0 gum       (1001) gum       (1001)     4528 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/mnist/equinox.py
--rw-r--r--   0 gum       (1001) gum       (1001)      703 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/mnist/vis.py
--rw-r--r--   0 gum       (1001) gum       (1001)     1004 2023-12-13 10:52:35.000000 jo3mnist-0.0.3/pyproject.toml
--rw-r--r--   0 gum       (1001) gum       (1001)       38 2023-12-13 11:01:13.687250 jo3mnist-0.0.3/setup.cfg
--rw-r--r--   0 gum       (1001) gum       (1001)       61 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/setup.py
-drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2023-12-13 11:01:13.687250 jo3mnist-0.0.3/tests/
--rw-r--r--   0 gum       (1001) gum       (1001)      396 2023-11-17 14:26:17.000000 jo3mnist-0.0.3/tests/test_main.py
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/
+-rw-r--r--   0 gum       (1001) gum       (1001)     1069 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/LICENSE
+-rw-r--r--   0 gum       (1001) gum       (1001)     1012 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/PKG-INFO
+-rw-r--r--   0 gum       (1001) gum       (1001)      391 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/README.md
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.174342 jo3mnist-0.0.4/jo3mnist/
+-rw-r--r--   0 gum       (1001) gum       (1001)       86 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/jo3mnist/__init__.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     6946 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/jo3mnist/__main__.py
+-rw-r--r--   0 gum       (1001) gum       (1001)      883 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/jo3mnist/data.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     4528 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/jo3mnist/equinox.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     3608 2024-04-07 08:53:42.000000 jo3mnist-0.0.4/jo3mnist/tiny_imagenet.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     1211 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/jo3mnist/vis.py
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/jo3mnist.egg-info/
+-rw-r--r--   0 gum       (1001) gum       (1001)     1012 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/PKG-INFO
+-rw-r--r--   0 gum       (1001) gum       (1001)      420 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/SOURCES.txt
+-rw-r--r--   0 gum       (1001) gum       (1001)        1 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/dependency_links.txt
+-rw-r--r--   0 gum       (1001) gum       (1001)       81 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/requires.txt
+-rw-r--r--   0 gum       (1001) gum       (1001)        9 2024-04-07 08:56:07.000000 jo3mnist-0.0.4/jo3mnist.egg-info/top_level.txt
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/mnist/
+-rw-r--r--   0 gum       (1001) gum       (1001)       86 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/mnist/__init__.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     6946 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/mnist/__main__.py
+-rw-r--r--   0 gum       (1001) gum       (1001)      883 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/mnist/data.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     4528 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/mnist/equinox.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     1211 2024-01-14 11:00:33.000000 jo3mnist-0.0.4/mnist/vis.py
+-rw-r--r--   0 gum       (1001) gum       (1001)     1025 2024-04-07 08:55:33.000000 jo3mnist-0.0.4/pyproject.toml
+-rw-r--r--   0 gum       (1001) gum       (1001)       38 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/setup.cfg
+-rw-r--r--   0 gum       (1001) gum       (1001)       61 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/setup.py
+drwxr-xr-x   0 gum       (1001) gum       (1001)        0 2024-04-07 08:56:07.177675 jo3mnist-0.0.4/tests/
+-rw-r--r--   0 gum       (1001) gum       (1001)      396 2023-11-17 14:26:17.000000 jo3mnist-0.0.4/tests/test_main.py
```

### Comparing `jo3mnist-0.0.3/LICENSE` & `jo3mnist-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.3/PKG-INFO` & `jo3mnist-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: jo3mnist
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/mnist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: equinox
 Requires-Dist: jax
 Requires-Dist: jaxtyping
 Requires-Dist: numpy
 Requires-Dist: pillow
+Requires-Dist: opencv-python
 Requires-Dist: optax
 Requires-Dist: torch
 Requires-Dist: torchvision
 Provides-Extra: demo
 
 # README
```

### Comparing `jo3mnist-0.0.3/jo3mnist/__main__.py` & `jo3mnist-0.0.4/jo3mnist/__main__.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.3/jo3mnist/data.py` & `jo3mnist-0.0.4/jo3mnist/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #! /usr/bin/env python3
 # vim:fenc=utf-8
 
 from pathlib import Path
+
 import torchvision
 from torch.utils.data import DataLoader
 
 
 def load(path=Path("./res/MNIST"), batch_size=64, shuffle=True):
     normalise_data = torchvision.transforms.Compose(
         [
```

### Comparing `jo3mnist-0.0.3/jo3mnist/equinox.py` & `jo3mnist-0.0.4/jo3mnist/equinox.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.3/jo3mnist.egg-info/PKG-INFO` & `jo3mnist-0.0.4/jo3mnist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: jo3mnist
-Version: 0.0.3
+Version: 0.0.4
 Author-email: Jochem Hölscher <a.fake@e.mail>
 Project-URL: homepage, https://github.com/JJJHolscher/mnist
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: equinox
 Requires-Dist: jax
 Requires-Dist: jaxtyping
 Requires-Dist: numpy
 Requires-Dist: pillow
+Requires-Dist: opencv-python
 Requires-Dist: optax
 Requires-Dist: torch
 Requires-Dist: torchvision
 Provides-Extra: demo
 
 # README
```

### Comparing `jo3mnist-0.0.3/mnist/__main__.py` & `jo3mnist-0.0.4/mnist/__main__.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.3/mnist/data.py` & `jo3mnist-0.0.4/mnist/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #! /usr/bin/env python3
 # vim:fenc=utf-8
 
 from pathlib import Path
+
 import torchvision
 from torch.utils.data import DataLoader
 
 
 def load(path=Path("./res/MNIST"), batch_size=64, shuffle=True):
     normalise_data = torchvision.transforms.Compose(
         [
```

### Comparing `jo3mnist-0.0.3/mnist/equinox.py` & `jo3mnist-0.0.4/mnist/equinox.py`

 * *Files identical despite different names*

### Comparing `jo3mnist-0.0.3/pyproject.toml` & `jo3mnist-0.0.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 
 [project]
 name = "jo3mnist"
-version = "0.0.3" # TODO; automatically update versions by looking at git
+version = "0.0.4" # TODO; automatically update versions by looking at git
 description = ""
 dependencies = [
     "equinox",
     "jax",
     "jaxtyping",
     "numpy",
     "pillow",
+    "opencv-python",
     "optax",
     "torch",
     "torchvision"
 ]
 dynamic = ["readme"]
 requires-python = ">=3.11"
 classifiers = [
```

