# Comparing `tmp/feynmodel-0.0.5.tar.gz` & `tmp/feynmodel-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feynmodel-0.0.5.tar", max compression
+gzip compressed data, was "feynmodel-0.0.6.tar", max compression
```

## Comparing `feynmodel-0.0.5.tar` & `feynmodel-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-03-31 17:10:08.000771 feynmodel-0.0.5/LICENSE
--rw-r--r--   0        0        0     2374 2024-03-31 17:10:08.000771 feynmodel-0.0.5/README.md
--rw-r--r--   0        0        0      176 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/__init__.py
--rw-r--r--   0        0        0      336 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/coupling.py
--rw-r--r--   0        0        0      284 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/coupling_order.py
--rw-r--r--   0        0        0      447 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/decay.py
--rw-r--r--   0        0        0     7475 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/feyn_model.py
--rw-r--r--   0        0        0      340 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/form_factor.py
--rw-r--r--   0        0        0      383 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/function.py
--rw-r--r--   0        0        0        0 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/interface/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/interface/feynarts.py
--rw-r--r--   0        0        0     2859 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/interface/qgraf.py
--rw-r--r--   0        0        0     5250 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/interface/ufo.py
--rw-r--r--   0        0        0      354 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/lorentz.py
--rw-r--r--   0        0        0        0 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/model/__init__.py
--rw-r--r--   0        0        0      277 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/model/mssm.py
--rw-r--r--   0        0        0      248 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/model/sm.py
--rw-r--r--   0        0        0      689 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/parameter.py
--rw-r--r--   0        0        0     3252 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/particle.py
--rw-r--r--   0        0        0     1313 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/ufo_base_class.py
--rw-r--r--   0        0        0      777 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/util.py
--rw-r--r--   0        0        0      563 2024-03-31 17:10:08.000771 feynmodel-0.0.5/feynmodel/vertex.py
--rw-r--r--   0        0        0     1937 2024-03-31 17:10:08.924775 feynmodel-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 feynmodel-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-07 09:11:26.980291 feynmodel-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2374 2024-04-07 09:11:26.980291 feynmodel-0.0.6/README.md
+-rw-r--r--   0        0        0      176 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/__init__.py
+-rw-r--r--   0        0        0      336 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/coupling.py
+-rw-r--r--   0        0        0      284 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/coupling_order.py
+-rw-r--r--   0        0        0      447 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/decay.py
+-rw-r--r--   0        0        0     7475 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/feyn_model.py
+-rw-r--r--   0        0        0      340 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/form_factor.py
+-rw-r--r--   0        0        0      383 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/function.py
+-rw-r--r--   0        0        0        0 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/interface/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 09:11:26.980291 feynmodel-0.0.6/feynmodel/interface/feynarts.py
+-rw-r--r--   0        0        0     3166 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/interface/qgraf.py
+-rw-r--r--   0        0        0     5250 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/interface/ufo.py
+-rw-r--r--   0        0        0      354 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/lorentz.py
+-rw-r--r--   0        0        0        0 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/model/__init__.py
+-rw-r--r--   0        0        0      277 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/model/mssm.py
+-rw-r--r--   0        0        0      248 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/model/sm.py
+-rw-r--r--   0        0        0      689 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/parameter.py
+-rw-r--r--   0        0        0     3252 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/particle.py
+-rw-r--r--   0        0        0     1313 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/ufo_base_class.py
+-rw-r--r--   0        0        0      777 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/util.py
+-rw-r--r--   0        0        0      563 2024-04-07 09:11:26.984292 feynmodel-0.0.6/feynmodel/vertex.py
+-rw-r--r--   0        0        0     1937 2024-04-07 09:11:27.852296 feynmodel-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3222 1970-01-01 00:00:00.000000 feynmodel-0.0.6/PKG-INFO
```

### Comparing `feynmodel-0.0.5/LICENSE` & `feynmodel-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/README.md` & `feynmodel-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/feynmodel/feyn_model.py` & `feynmodel-0.0.6/feynmodel/feyn_model.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/feynmodel/interface/qgraf.py` & `feynmodel-0.0.6/feynmodel/interface/qgraf.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Convert a feynmodel to a qgraf model
 # return the qgraf model as string
 
+from typing import Optional
+
 from feynmodel.feyn_model import FeynModel
 from feynmodel.particle import Particle
 from feynmodel.util import get_name
 from feynmodel.vertex import Vertex
 
 
 def get_particle_name(particle, use_pdg_names=False, anti=False):
@@ -20,16 +22,27 @@
     else:
         if anti:
             return particle.antiname
         else:
             return particle.name
 
 
+def pdg_id_to_qgraf_name(
+    feynmodel: FeynModel, pdg_id: int, use_pdg_names: bool = False
+) -> Optional[str]:
+    for p in feynmodel.particles:
+        if p.pdg_code == pdg_id:
+            return get_particle_name(p, use_pdg_names)
+    return None
+
+
 def feynmodel_to_qgraf(
-    feynmodel: FeynModel, use_pdg_names=False, include_antiparticles=False
+    feynmodel: FeynModel,
+    use_pdg_names: bool = False,
+    include_antiparticles: bool = False,
 ):
     return_string = ""
     return_string + "* Particles\n"
     for p in feynmodel.particles:
         if include_antiparticles or p.pdg_code > 0:
             stat = ["-", "+", "+", "-", "+"][p.spin + 1]
             name = get_particle_name(p, use_pdg_names)
```

### Comparing `feynmodel-0.0.5/feynmodel/interface/ufo.py` & `feynmodel-0.0.6/feynmodel/interface/ufo.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/feynmodel/parameter.py` & `feynmodel-0.0.6/feynmodel/parameter.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/feynmodel/particle.py` & `feynmodel-0.0.6/feynmodel/particle.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/feynmodel/ufo_base_class.py` & `feynmodel-0.0.6/feynmodel/ufo_base_class.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/feynmodel/util.py` & `feynmodel-0.0.6/feynmodel/util.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/feynmodel/vertex.py` & `feynmodel-0.0.6/feynmodel/vertex.py`

 * *Files identical despite different names*

### Comparing `feynmodel-0.0.5/pyproject.toml` & `feynmodel-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "feynmodel"
-version = "0.0.5"
+version = "0.0.6"
 description = "Models for constructing Feynman diagrams"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/feynmodel"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `feynmodel-0.0.5/PKG-INFO` & `feynmodel-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feynmodel
-Version: 0.0.5
+Version: 0.0.6
 Summary: Models for constructing Feynman diagrams
 Home-page: https://github.com/APN-Pucky/feynmodel
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

