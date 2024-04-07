# Comparing `tmp/dynamicpy-1.2.2.tar.gz` & `tmp/dynamicpy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamicpy-1.2.2.tar", max compression
+gzip compressed data, was "dynamicpy-1.3.0.tar", max compression
```

## Comparing `dynamicpy-1.2.2.tar` & `dynamicpy-1.3.0.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-04-02 13:19:20.126349 dynamicpy-1.2.2/LICENCE
--rw-r--r--   0        0        0     3276 2024-04-02 13:19:20.126349 dynamicpy-1.2.2/README.md
--rw-r--r--   0        0        0      610 2024-04-02 13:19:20.126349 dynamicpy-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1128 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/__init__.py
--rw-r--r--   0        0        0     3932 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/dependencies.py
--rw-r--r--   0        0        0     1056 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/errors.py
--rw-r--r--   0        0        0     7195 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/loader.py
--rw-r--r--   0        0        0     5604 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/utils.py
--rw-r--r--   0        0        0     2658 2024-04-02 13:19:37.238289 dynamicpy-1.2.2/src/dynamicpy/widgets.py
--rw-r--r--   0        0        0     4083 1970-01-01 00:00:00.000000 dynamicpy-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-07 13:50:53.420399 dynamicpy-1.3.0/LICENCE
+-rw-r--r--   0        0        0     4437 2024-04-07 13:50:53.420399 dynamicpy-1.3.0/README.md
+-rw-r--r--   0        0        0      610 2024-04-07 13:50:53.420399 dynamicpy-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1195 2024-04-07 13:51:14.668564 dynamicpy-1.3.0/src/dynamicpy/__init__.py
+-rw-r--r--   0        0        0     3932 2024-04-07 13:51:14.668564 dynamicpy-1.3.0/src/dynamicpy/dependencies.py
+-rw-r--r--   0        0        0     1056 2024-04-07 13:51:14.664564 dynamicpy-1.3.0/src/dynamicpy/errors.py
+-rw-r--r--   0        0        0     7195 2024-04-07 13:51:14.664564 dynamicpy-1.3.0/src/dynamicpy/loader.py
+-rw-r--r--   0        0        0     6622 2024-04-07 13:51:14.664564 dynamicpy-1.3.0/src/dynamicpy/model.py
+-rw-r--r--   0        0        0     5604 2024-04-07 13:51:14.668564 dynamicpy-1.3.0/src/dynamicpy/utils.py
+-rw-r--r--   0        0        0     2658 2024-04-07 13:51:14.664564 dynamicpy-1.3.0/src/dynamicpy/widgets.py
+-rw-r--r--   0        0        0     5244 1970-01-01 00:00:00.000000 dynamicpy-1.3.0/PKG-INFO
```

### Comparing `dynamicpy-1.2.2/LICENCE` & `dynamicpy-1.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.2/pyproject.toml` & `dynamicpy-1.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dynamicpy"
-version = "1.2.2"
+version = "1.3.0"
 description = "A python module for dynamically interacting with objects to improve expandability."
 authors = ["NimajnebEC <nimajnebec@users.noreply.github.com>"]
 repository = "https://github.com/NimajnebEC/dynamicpy"
 packages = [{ include = "dynamicpy", from = "src" }]
 readme = "README.md"
 license = "MIT"
```

### Comparing `dynamicpy-1.2.2/src/dynamicpy/__init__.py` & `dynamicpy-1.3.0/src/dynamicpy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """
 A python module for dynamically interacting with objects to improve expandability.
 
 https://github.com/NimajnebEC/dynamicpy
 """
 
 
-__version__ = "1.2.2"
+__version__ = "1.3.0"
 __author__ = "NimajnebEC <nimajnebec@users.noreply.github.com>"
 
 from dynamicpy.dependencies import DependencyLibrary
 from dynamicpy.errors import (
     DependencyNotFoundError,
     DuplicateDependencyError,
     DynamicPyError,
     InjectDependenciesError,
     NoForeignModulesError,
     NoParentError,
 )
 from dynamicpy.loader import DynamicLoader
+from dynamicpy.model import Model, field
 from dynamicpy.utils import (
     ConstructorProtocol,
     functionify,
     get_foreign_module,
     get_module,
     get_module_parent,
     get_stack_module_up,
@@ -42,8 +43,10 @@
     "get_stack_module_up",
     "get_module",
     "is_package",
     "DependencyNotFoundError",
     "DuplicateDependencyError",
     "InjectDependenciesError",
     "BaseWidget",
+    "Model",
+    "field",
 )
```

### Comparing `dynamicpy-1.2.2/src/dynamicpy/dependencies.py` & `dynamicpy-1.3.0/src/dynamicpy/dependencies.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.2/src/dynamicpy/errors.py` & `dynamicpy-1.3.0/src/dynamicpy/errors.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.2/src/dynamicpy/loader.py` & `dynamicpy-1.3.0/src/dynamicpy/loader.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.2/src/dynamicpy/utils.py` & `dynamicpy-1.3.0/src/dynamicpy/utils.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.2/src/dynamicpy/widgets.py` & `dynamicpy-1.3.0/src/dynamicpy/widgets.py`

 * *Files identical despite different names*

### Comparing `dynamicpy-1.2.2/PKG-INFO` & `dynamicpy-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,17 @@
-Metadata-Version: 2.1
-Name: dynamicpy
-Version: 1.2.2
-Summary: A python module for dynamically interacting with objects to improve expandability.
-Home-page: https://github.com/NimajnebEC/dynamicpy
-License: MIT
-Author: NimajnebEC
-Author-email: nimajnebec@users.noreply.github.com
-Requires-Python: >=3.8,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: typeguard (>=4.0.0,<5.0.0)
-Project-URL: Repository, https://github.com/NimajnebEC/dynamicpy
-Description-Content-Type: text/markdown
-
 # DynamicPy <!-- omit from toc -->
 
 A python module for dynamically interacting with objects to improve expandability.
 
 ### Features
 
 - [Dynamic Loader](#dynamic-loader)
 - [Dependency Library](#dependency-library)
 - [Widgets](#widgets)
+- [Models](#models)
 
 ## Dynamic Loader
 
 The `DynamicLoader` class allows for the dynamic import of modules and the scraping of their globals.
 
 To provide functionality with the scraped globals you must register a handler using the `register_handler` method or the `handler` decorator. Both methods take an optional `selector` parameter which is a predicate to determine wether the handler should be called.
 
@@ -117,7 +98,50 @@
 loader = DynamicLoader()
 
 @loader.widget_handler(ExampleWidget)
 def widget_handler(widget: ExampleWidget):
     widget.callback("Hello World!")  # prints "Hello World!"
 ```
 
+## Models
+
+DynamicPy provides its own system similar to [dataclasses](https://docs.python.org/3/library/dataclasses.html) called models which are designed to aid in data validation and type hinting. A model can be defined by simply extending the `dynamicpy.Model` class and specifying fields. These fields can be populated using the model's constructor.
+
+```py
+from dynamicpy import Model
+
+class User(Model):
+    gid: int
+    name: str
+    avatar: str
+
+User(guid=123, name="John Doe", avatar="https://bit.ly/3J73JHU")
+```
+
+Behaviour can be further configured using the `dynamicpy.field` function.
+
+```py
+from dynamicpy import Model, field
+
+class User(Model):
+    gid: int = field(cast=int)
+    name: str = field(default="Unnamed")
+    avatar: str = "https://bit.ly/3J73JHU" # default alternative
+
+User(guid="123")
+```
+
+Models will also recursively load types with a `from_dict` classmethod (including other models).
+
+```py
+from dynamicpy import Model
+
+class User(Model):
+    gid: int
+    name: str
+
+class Post(Model):
+    title: str
+    author: User
+
+Post.from_dict({"title": "Lorem Ipsum", "author": {"gid": 123, "name": "John Doe"}})
+```
```

