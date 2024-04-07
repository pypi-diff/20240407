# Comparing `tmp/py-jaxtyping-0.1.1.tar.gz` & `tmp/py-jaxtyping-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-jaxtyping-0.1.1.tar", last modified: Sun Apr  7 09:17:59 2024, max compression
+gzip compressed data, was "py-jaxtyping-0.1.2.tar", last modified: Sun Apr  7 09:59:29 2024, max compression
```

## Comparing `py-jaxtyping-0.1.1.tar` & `py-jaxtyping-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1213 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      879 2024-04-07 09:17:09.000000 py-jaxtyping-0.1.1/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-04-07 09:17:57.000000 py-jaxtyping-0.1.1/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/src/py_jaxtyping/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      967 2024-04-07 09:17:42.000000 py-jaxtyping-0.1.1/src/py_jaxtyping/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2339 2024-04-07 09:13:41.000000 py-jaxtyping-0.1.1/src/py_jaxtyping/main.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:17:59.851787 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1213 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      277 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-07 09:17:59.000000 py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:59:29.491792 py-jaxtyping-0.1.2/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-07 09:59:29.481792 py-jaxtyping-0.1.2/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      782 2024-04-07 09:59:23.000000 py-jaxtyping-0.1.2/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      558 2024-04-07 09:59:27.000000 py-jaxtyping-0.1.2/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-07 09:59:29.491792 py-jaxtyping-0.1.2/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:59:29.481792 py-jaxtyping-0.1.2/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:59:29.481792 py-jaxtyping-0.1.2/src/py_jaxtyping/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      848 2024-04-07 09:59:12.000000 py-jaxtyping-0.1.2/src/py_jaxtyping/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1356 2024-04-07 09:58:46.000000 py-jaxtyping-0.1.2/src/py_jaxtyping/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1601 2024-04-07 09:57:49.000000 py-jaxtyping-0.1.2/src/py_jaxtyping/schemas.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-07 09:59:29.481792 py-jaxtyping-0.1.2/src/py_jaxtyping.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1116 2024-04-07 09:59:29.000000 py-jaxtyping-0.1.2/src/py_jaxtyping.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      305 2024-04-07 09:59:29.000000 py-jaxtyping-0.1.2/src/py_jaxtyping.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-07 09:59:29.000000 py-jaxtyping-0.1.2/src/py_jaxtyping.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       15 2024-04-07 09:59:29.000000 py-jaxtyping-0.1.2/src/py_jaxtyping.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       13 2024-04-07 09:59:29.000000 py-jaxtyping-0.1.2/src/py_jaxtyping.egg-info/top_level.txt
```

### Comparing `py-jaxtyping-0.1.1/PKG-INFO` & `py-jaxtyping-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jaxtyping
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pydantic support for Jaxtyping array annotations
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: numpy
@@ -17,16 +17,14 @@
   
 Instead of `Int[np.ndarray, 'B 256 64 3']`, do `PyArray[Int, int, 'B 256 64 3']`
 
 You can use it with `jaxtyping` as normal, but also it will:
 - Serialize to nested lists
 - Validate the correct shape and datatypes from serialized lists
 
-**With `pydantic`, make sure to use `model_config = ConfigDict(arbitrary_types_allowed=True)`**
-
 ### Example
 ```
 from pydantic import BaseModel, ConfigDict
 from py_jaxtyping import PyArray
 from jaxtyping import Int
 import numpy as np
```

### Comparing `py-jaxtyping-0.1.1/README.md` & `py-jaxtyping-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -6,16 +6,14 @@
   
 Instead of `Int[np.ndarray, 'B 256 64 3']`, do `PyArray[Int, int, 'B 256 64 3']`
 
 You can use it with `jaxtyping` as normal, but also it will:
 - Serialize to nested lists
 - Validate the correct shape and datatypes from serialized lists
 
-**With `pydantic`, make sure to use `model_config = ConfigDict(arbitrary_types_allowed=True)`**
-
 ### Example
 ```
 from pydantic import BaseModel, ConfigDict
 from py_jaxtyping import PyArray
 from jaxtyping import Int
 import numpy as np
```

### Comparing `py-jaxtyping-0.1.1/pyproject.toml` & `py-jaxtyping-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-jaxtyping"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Pydantic support for Jaxtyping array annotations"
 dependencies = [
   "pydantic", "numpy"
 ]
```

### Comparing `py-jaxtyping-0.1.1/src/py_jaxtyping/main.py` & `py-jaxtyping-0.1.2/src/py_jaxtyping/schemas.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from typing import Annotated, Any, Unpack, Literal, TypedDict, TypeVar
-from pydantic import AfterValidator, PlainSerializer, WithJsonSchema
 from pydantic_core import CoreSchema
-from pydantic_core.core_schema import no_info_after_validator_function
-import numpy as np
 
 class SchemaKeys(TypedDict):
   array: str
   dtype: str
   items: str
   minItems: str
   maxItems: str
@@ -22,14 +19,18 @@
   match dims:
     case [dim] if str(dim).isdecimal():
       d = int(dim)
       return {
         'type': keys['array'], keys['items']: array_schema([], **keys),
         keys['minItems']: d, keys['maxItems']: d
       }
+    case [dim]:
+      return {
+        'type': keys['array'], keys['items']: array_schema([], **keys),
+      }
     case [dim, *ds] if str(dim).isdecimal():
       d = int(dim)
       return {
         'type': keys['array'], keys['items']: array_schema(ds, **keys),
         keys['minItems']: d, keys['maxItems']: d
       }
     case [dim, *ds]:
@@ -46,37 +47,8 @@
     minItems='minItems', maxItems='maxItems'
   )
 
 def core_schema(dims: list, dtype: Literal['int', 'float', 'bool'] = 'int') -> CoreSchema:
   return array_schema(
     dims, array='list', dtype=dtype, items='items_schema',
     minItems='min_length', maxItems='max_length'
-  ) # type: ignore
-
-
-class PyArray:
-  """A `jaxtyping` array that can be used with pydantic
-  
-  Instead of:
-  >>> Int[np.ndarray, 'B 256 64 3']
-  do:
-  >>> PyArray[Int, 'B 256 64 3']
-
-  You can use it with `jaxtyping` as normal, but also
-
-  ```
-  class WithArray(BaseModel):
-    arr: PyArray[Int, 'B 256 64 3']
-  ```
-
-  And it will:
-  - Serialize to nested lists
-  - Validate the correct shape and datatypes from serialized lists
-  """
-  def __class_getitem__(cls, params: tuple[type, str]):
-    DType, dims = params
-    return Annotated[
-      DType[np.ndarray, dims],
-      AfterValidator(np.array),
-      PlainSerializer(lambda arr: arr.tolist()),
-      WithJsonSchema(json_schema(dims.split(' ')))
-    ]
+  ) # type: ignore
```

### Comparing `py-jaxtyping-0.1.1/src/py_jaxtyping.egg-info/PKG-INFO` & `py-jaxtyping-0.1.2/src/py_jaxtyping.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-jaxtyping
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pydantic support for Jaxtyping array annotations
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/REPO.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: numpy
@@ -17,16 +17,14 @@
   
 Instead of `Int[np.ndarray, 'B 256 64 3']`, do `PyArray[Int, int, 'B 256 64 3']`
 
 You can use it with `jaxtyping` as normal, but also it will:
 - Serialize to nested lists
 - Validate the correct shape and datatypes from serialized lists
 
-**With `pydantic`, make sure to use `model_config = ConfigDict(arbitrary_types_allowed=True)`**
-
 ### Example
 ```
 from pydantic import BaseModel, ConfigDict
 from py_jaxtyping import PyArray
 from jaxtyping import Int
 import numpy as np
```

