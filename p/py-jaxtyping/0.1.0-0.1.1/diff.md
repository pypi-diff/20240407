# Comparing `tmp/py-jaxtyping-0.1.0.tar.gz` & `tmp/py-jaxtyping-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-jaxtyping-0.1.0.tar", last modified: Sun Apr  7 09:14:40 2024, max compression
+gzip compressed data, was "py-jaxtyping-0.1.1.tar", last modified: Sun Apr  7 09:17:59 2024, max compression
```

## Comparing `py-jaxtyping-0.1.0.tar` & `py-jaxtyping-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:14:40.101790 py-jaxtyping-0.1.0/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1046 2024-04-07 09:14:40.101790 py-jaxtyping-0.1.0/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      712 2024-04-07 08:56:34.000000 py-jaxtyping-0.1.0/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-04-07 07:53:41.000000 py-jaxtyping-0.1.0/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-07 09:14:40.101790 py-jaxtyping-0.1.0/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:14:40.091790 py-jaxtyping-0.1.0/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:14:40.091790 py-jaxtyping-0.1.0/src/py_jaxtyping/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      806 2024-04-07 09:14:13.000000 py-jaxtyping-0.1.0/src/py_jaxtyping/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2339 2024-04-07 09:13:41.000000 py-jaxtyping-0.1.0/src/py_jaxtyping/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:14:40.101790 py-jaxtyping-0.1.0/src/py_jaxtyping.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1046 2024-04-07 09:14:40.000000 py-jaxtyping-0.1.0/src/py_jaxtyping.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      277 2024-04-07 09:14:40.000000 py-jaxtyping-0.1.0/src/py_jaxtyping.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-07 09:14:40.000000 py-jaxtyping-0.1.0/src/py_jaxtyping.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-07 09:14:40.000000 py-jaxtyping-0.1.0/src/py_jaxtyping.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-07 09:14:40.000000 py-jaxtyping-0.1.0/src/py_jaxtyping.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1213 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      879 2024-04-07 09:17:09.000000 py-jaxtyping-0.1.1/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-04-07 09:17:57.000000 py-jaxtyping-0.1.1/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/src/py_jaxtyping/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      967 2024-04-07 09:17:42.000000 py-jaxtyping-0.1.1/src/py_jaxtyping/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2339 2024-04-07 09:13:41.000000 py-jaxtyping-0.1.1/src/py_jaxtyping/main.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1213 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      277 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/top_level.txt
```

### Comparing `py-jaxtyping-0.1.0/PKG-INFO` & `py-jaxtyping-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jaxtyping
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pydantic support for Jaxtyping array annotations
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: numpy
@@ -17,22 +17,25 @@
   
 Instead of `Int[np.ndarray, 'B 256 64 3']`, do `PyArray[Int, int, 'B 256 64 3']`
 
 You can use it with `jaxtyping` as normal, but also it will:
 - Serialize to nested lists
 - Validate the correct shape and datatypes from serialized lists
 
+**With `pydantic`, make sure to use `model_config = ConfigDict(arbitrary_types_allowed=True)`**
+
 ### Example
 ```
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from py_jaxtyping import PyArray
 from jaxtyping import Int
 import numpy as np
 
 class Sample(BaseModel):
+  model_config = ConfigDict(arbitrary_types_allowed=True)
   img: PyArray[Int, int, "W H 3"]
   label: str
 
 Sample.model_validate({
   'img': np.ones((256, 64, 3)),
   'label': 'car'
 })
```

### Comparing `py-jaxtyping-0.1.0/README.md` & `py-jaxtyping-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,22 +6,25 @@
   
 Instead of `Int[np.ndarray, 'B 256 64 3']`, do `PyArray[Int, int, 'B 256 64 3']`
 
 You can use it with `jaxtyping` as normal, but also it will:
 - Serialize to nested lists
 - Validate the correct shape and datatypes from serialized lists
 
+**With `pydantic`, make sure to use `model_config = ConfigDict(arbitrary_types_allowed=True)`**
+
 ### Example
 ```
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from py_jaxtyping import PyArray
 from jaxtyping import Int
 import numpy as np
 
 class Sample(BaseModel):
+  model_config = ConfigDict(arbitrary_types_allowed=True)
   img: PyArray[Int, int, "W H 3"]
   label: str
 
 Sample.model_validate({
   'img': np.ones((256, 64, 3)),
   'label': 'car'
 })
```

### Comparing `py-jaxtyping-0.1.0/pyproject.toml` & `py-jaxtyping-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-jaxtyping"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pydantic support for Jaxtyping array annotations"
 dependencies = [
   "pydantic", "numpy"
 ]
```

### Comparing `py-jaxtyping-0.1.0/src/py_jaxtyping/main.py` & `py-jaxtyping-0.1.1/src/py_jaxtyping/main.py`

 * *Files identical despite different names*

### Comparing `py-jaxtyping-0.1.0/src/py_jaxtyping.egg-info/PKG-INFO` & `py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jaxtyping
-Version: 0.1.0
+Version: 0.1.1
 Summary: Pydantic support for Jaxtyping array annotations
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: numpy
@@ -17,22 +17,25 @@
   
 Instead of `Int[np.ndarray, 'B 256 64 3']`, do `PyArray[Int, int, 'B 256 64 3']`
 
 You can use it with `jaxtyping` as normal, but also it will:
 - Serialize to nested lists
 - Validate the correct shape and datatypes from serialized lists
 
+**With `pydantic`, make sure to use `model_config = ConfigDict(arbitrary_types_allowed=True)`**
+
 ### Example
 ```
-from pydantic import BaseModel
+from pydantic import BaseModel, ConfigDict
 from py_jaxtyping import PyArray
 from jaxtyping import Int
 import numpy as np
 
 class Sample(BaseModel):
+  model_config = ConfigDict(arbitrary_types_allowed=True)
   img: PyArray[Int, int, "W H 3"]
   label: str
 
 Sample.model_validate({
   'img': np.ones((256, 64, 3)),
   'label': 'car'
 })
```

