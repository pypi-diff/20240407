# Comparing `tmp/tkutils-1.1.1.tar.gz` & `tmp/tkutils-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkutils-1.1.1.tar", max compression
+gzip compressed data, was "tkutils-1.1.2.tar", max compression
```

## Comparing `tkutils-1.1.1.tar` & `tkutils-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rwxr-xr-x   0        0        0     2817 2023-04-22 21:02:45.313791 tkutils-1.1.1/README.md
--rwxr-xr-x   0        0        0      752 2023-04-22 21:26:35.451151 tkutils-1.1.1/pyproject.toml
--rwxr-xr-x   0        0        0     3571 2023-04-22 21:26:38.075873 tkutils-1.1.1/src/tkutils/__init__.py
--rwxr-xr-x   0        0        0      101 2022-12-22 16:54:42.632637 tkutils-1.1.1/src/tkutils/__main__.py
--rwxr-xr-x   0        0        0       22 2023-04-22 21:26:38.077458 tkutils-1.1.1/src/tkutils/__version__.py
--rwxr-xr-x   0        0        0     9327 2023-04-22 21:02:45.584732 tkutils-1.1.1/src/tkutils/grid_layout.py
--rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.645734 tkutils-1.1.1/src/tkutils/helpers/__init__.py
--rwxr-xr-x   0        0        0     4316 2023-04-22 21:02:45.586456 tkutils-1.1.1/src/tkutils/helpers/event_provider.py
--rwxr-xr-x   0        0        0     5290 2023-04-22 21:02:45.603352 tkutils-1.1.1/src/tkutils/helpers/keysym.py
--rwxr-xr-x   0        0        0    10200 2023-04-22 21:22:04.762277 tkutils-1.1.1/src/tkutils/images.py
--rwxr-xr-x   0        0        0       37 2022-12-22 16:54:42.728682 tkutils-1.1.1/src/tkutils/menu_builder/__init__.py
--rwxr-xr-x   0        0        0     2261 2023-04-22 21:02:45.611159 tkutils-1.1.1/src/tkutils/menu_builder/bases.py
--rwxr-xr-x   0        0        0     5047 2023-04-22 21:02:45.638271 tkutils-1.1.1/src/tkutils/menu_builder/menu_builder.py
--rwxr-xr-x   0        0        0     8300 2023-04-22 21:02:45.643707 tkutils-1.1.1/src/tkutils/menu_builder/menu_builder_options.py
--rwxr-xr-x   0        0        0      220 2022-12-22 16:54:42.802957 tkutils-1.1.1/src/tkutils/two_way_binding/__init__.py
--rwxr-xr-x   0        0        0    28483 2023-04-22 21:02:45.645441 tkutils-1.1.1/src/tkutils/two_way_binding/binder.py
--rwxr-xr-x   0        0        0    13926 2023-04-22 21:02:45.646758 tkutils-1.1.1/src/tkutils/two_way_binding/binding_descriptor.py
--rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.814650 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/__init__.py
--rwxr-xr-x   0        0        0     9282 2023-04-22 21:09:36.221905 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_binder_config.py
--rwxr-xr-x   0        0        0    10709 2023-04-22 21:02:45.672479 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configuration.py
--rwxr-xr-x   0        0        0     3174 2023-04-22 21:15:09.528146 tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py
--rwxr-xr-x   0        0        0      565 2022-12-22 16:54:42.850410 tkutils-1.1.1/src/tkutils/two_way_binding/errors.py
--rwxr-xr-x   0        0        0       55 2022-12-22 16:54:42.863360 tkutils-1.1.1/src/tkutils/utilities/__init__.py
--rwxr-xr-x   0        0        0    12657 2022-12-22 16:54:42.896203 tkutils-1.1.1/src/tkutils/utilities/singleton_namespace.py
--rw-r--r--   0        0        0     3570 1970-01-01 00:00:00.000000 tkutils-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2817 2024-04-07 13:33:10.088201 tkutils-1.1.2/README.md
+-rw-r--r--   0        0        0      717 2024-04-07 13:33:17.156408 tkutils-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3571 2024-04-07 13:33:10.092201 tkutils-1.1.2/src/tkutils/__init__.py
+-rwxr-xr-x   0        0        0      101 2022-12-22 16:54:42.632637 tkutils-1.1.2/src/tkutils/__main__.py
+-rw-r--r--   0        0        0       22 2024-04-07 13:33:10.092201 tkutils-1.1.2/src/tkutils/__version__.py
+-rwxr-xr-x   0        0        0     9327 2023-04-22 21:02:45.584732 tkutils-1.1.2/src/tkutils/grid_layout.py
+-rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.645734 tkutils-1.1.2/src/tkutils/helpers/__init__.py
+-rwxr-xr-x   0        0        0     4316 2023-04-22 21:02:45.586456 tkutils-1.1.2/src/tkutils/helpers/event_provider.py
+-rwxr-xr-x   0        0        0     5290 2023-04-22 21:02:45.603352 tkutils-1.1.2/src/tkutils/helpers/keysym.py
+-rwxr-xr-x   0        0        0    10200 2023-04-22 21:26:49.261380 tkutils-1.1.2/src/tkutils/images.py
+-rwxr-xr-x   0        0        0       37 2022-12-22 16:54:42.728682 tkutils-1.1.2/src/tkutils/menu_builder/__init__.py
+-rwxr-xr-x   0        0        0     2261 2023-04-22 21:02:45.611159 tkutils-1.1.2/src/tkutils/menu_builder/bases.py
+-rwxr-xr-x   0        0        0     5047 2023-04-22 21:02:45.638271 tkutils-1.1.2/src/tkutils/menu_builder/menu_builder.py
+-rwxr-xr-x   0        0        0     8300 2023-04-22 21:02:45.643707 tkutils-1.1.2/src/tkutils/menu_builder/menu_builder_options.py
+-rwxr-xr-x   0        0        0      220 2022-12-22 16:54:42.802957 tkutils-1.1.2/src/tkutils/two_way_binding/__init__.py
+-rwxr-xr-x   0        0        0    28483 2023-04-22 21:02:45.645441 tkutils-1.1.2/src/tkutils/two_way_binding/binder.py
+-rwxr-xr-x   0        0        0    13926 2023-04-22 21:02:45.646758 tkutils-1.1.2/src/tkutils/two_way_binding/binding_descriptor.py
+-rwxr-xr-x   0        0        0        0 2022-12-22 16:54:42.814650 tkutils-1.1.2/src/tkutils/two_way_binding/configuration/__init__.py
+-rwxr-xr-x   0        0        0     9282 2023-04-22 21:09:36.221905 tkutils-1.1.2/src/tkutils/two_way_binding/configuration/_binder_config.py
+-rwxr-xr-x   0        0        0    10709 2023-04-22 21:02:45.672479 tkutils-1.1.2/src/tkutils/two_way_binding/configuration/_configuration.py
+-rwxr-xr-x   0        0        0     3174 2023-04-22 21:26:49.262561 tkutils-1.1.2/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py
+-rwxr-xr-x   0        0        0      565 2022-12-22 16:54:42.850410 tkutils-1.1.2/src/tkutils/two_way_binding/errors.py
+-rwxr-xr-x   0        0        0       55 2022-12-22 16:54:42.863360 tkutils-1.1.2/src/tkutils/utilities/__init__.py
+-rwxr-xr-x   0        0        0    12657 2022-12-22 16:54:42.896203 tkutils-1.1.2/src/tkutils/utilities/singleton_namespace.py
+-rw-r--r--   0        0        0     3496 1970-01-01 00:00:00.000000 tkutils-1.1.2/PKG-INFO
```

### Comparing `tkutils-1.1.1/README.md` & `tkutils-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Welcome to TkUtils
 
 `tkutils` is a package offering some additional logic and syntactic sugar when using `tkinter`.
 The main goal is to fill some gaps of tkinter, which might make it very annoying to use.
 
-Online version of the help documentation: http://frederic.zinelli.gitlab.io/tkutils/
+Online version of the help documentation: http://frederic-zinelli.gitlab.io/tkutils/
 
 
 
 ## Features
 
 
-### Additional logic: two-way binding, with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
+### Additional logic: two-way binding, with [`Binder`](http://frederic-zinelli.gitlab.io/tkutils/binder/binder_overview/)
 
-The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
+The [`Binder`](http://frederic-zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
 binding reactivity between widgets and underlying object properties from the model/logic layer
 of the application.
 
 Several advantages come with this:
 
 * Changes of bound properties in the model layer are cascading in the GUI automatically.
 * The model layer of the application becomes (finally) totally independent from the presentation
@@ -24,39 +24,39 @@
   think about its integration with `tkinter` itself.
 
 
 
 ### Syntactic sugar
 
 
-#### [`GridLayout`](http://frederic.zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)
+#### [`GridLayout`](http://frederic-zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)
 
 A grid layout manager which is abstracting away all the naughty `widget.grid(...)` calls and
 rows/columns grid configuration. Positioning widgets in the grid and controlling their "spanning"
 becomes very easy, without extra typing.
 
 
-#### [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
+#### [`MenuBuilder`](http://frederic-zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
 
 A helper to build menus and to abstract away all the technicalities encountered when creating menus through
-`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
+`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic-zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
 
 
-#### [`Event`](http://frederic.zinelli.gitlab.io/tkutils/event/)
+#### [`Event`](http://frederic-zinelli.gitlab.io/tkutils/event/)
 
 A utility to build event strings with auto-completion/IDE suggestions support.
 
 
-#### [`KeySym`](http://frederic.zinelli.gitlab.io/tkutils/key_sym/)
+#### [`KeySym`](http://frederic-zinelli.gitlab.io/tkutils/key_sym/)
 
 A utility to get all keysym information with auto-completion/IDE suggestions (providing string,
 keycode and keysym_num values).
 
 
-#### [`images`](http://frederic.zinelli.gitlab.io/tkutils/images/images/)
+#### [`images`](http://frederic-zinelli.gitlab.io/tkutils/images/images/)
 
 Various factories related to images to:
 
 * Simplify and reduce the typing needed,
 * Handle file conversions automatically,
 * Register automatically the image object on the host for the user (to avoid garbage collection).
 
@@ -80,9 +80,9 @@
 
 * Using an archive file (with the appropriate version number):
 
 ```bash
 pip install tkutils.1.0.2.tar.gz
 ```
 
-* Cloning the [GitLab repository](https://gitlab.com/frederic.zinelli/tkutils).
+* Cloning the [GitLab repository](https://gitlab.com/frederic-zinelli/tkutils).
```

### Comparing `tkutils-1.1.1/pyproject.toml` & `tkutils-1.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 [tool.poetry]
 name = "tkutils"
-version = "1.1.1"
+version = "1.1.2"
 description = "Python tkinter utilities."
 authors = ["Frédéric Zinelli <frederic.zinelli@gmail.com>"]
-license = "FreeBSD"
 readme = "README.md"
-repository = "https://gitlab.com/frederic.zinelli/tkutils"
-homepage = "http://frederic.zinelli.gitlab.io/tkutils/"
+repository = "https://gitlab.com/frederic-zinelli/tkutils"
+homepage = "http://frederic-zinelli.gitlab.io/tkutils/"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-Pillow = "^9.3.0"
-typing-extensions = "^4.4.0"
+Pillow = "^9.3"
+typing-extensions = "^4.4"
 
 [tool.poetry.group.dev.dependencies]
-pylint = "^2.15.6"
-pytest = "^7.2.0"
-mkdocs = "^1.4.2"
-mkdocs-material = "^8.5.11"
-mkdocstrings = {version = "^0.19.0", extras = ["python"] }
+pylint = "^2.15"
+pytest = "^7.2"
+mkdocs = "^1.4"
+mkdocs-material = "^8.5"
+mkdocstrings = {version = "^0.19", extras = ["python"] }
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 essai = "project_debug:routing"
```

### Comparing `tkutils-1.1.1/src/tkutils/__init__.py` & `tkutils-1.1.2/src/tkutils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 # Welcome to TkUtils
 
 `tkutils` is a package offering some additional logic and syntactic sugar when using `tkinter`.
 The main goal is to fill some gaps of tkinter, which might make it very annoying to use.
 
-Online version of the help documentation: http://frederic.zinelli.gitlab.io/tkutils/
+Online version of the help documentation: http://frederic-zinelli.gitlab.io/tkutils/
 
 
 
 ## Features
 
 
-### Additional logic: two-way binding, with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
+### Additional logic: two-way binding, with [`Binder`](http://frederic-zinelli.gitlab.io/tkutils/binder/binder_overview/)
 
-The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
+The [`Binder`](http://frederic-zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
 binding reactivity between widgets and underlying object properties from the model/logic layer
 of the application.
 
 Several advantages come with this:
 
 * Changes of bound properties in the model layer are cascading in the GUI automatically.
 * The model layer of the application becomes (finally) totally independent from the presentation
@@ -25,39 +25,39 @@
   think about its integration with `tkinter` itself.
 
 
 
 ### Syntactic sugar
 
 
-#### [`GridLayout`](http://frederic.zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)
+#### [`GridLayout`](http://frederic-zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)
 
 A grid layout manager which is abstracting away all the naughty `widget.grid(...)` calls and
 rows/columns grid configuration. Positioning widgets in the grid and controlling their "spanning"
 becomes very easy, without extra typing.
 
 
-#### [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
+#### [`MenuBuilder`](http://frederic-zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
 
 A helper to build menus and to abstract away all the technicalities encountered when creating menus through
-`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
+`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic-zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
 
 
-#### [`Event`](http://frederic.zinelli.gitlab.io/tkutils/event/)
+#### [`Event`](http://frederic-zinelli.gitlab.io/tkutils/event/)
 
 A utility to build event strings with auto-completion/IDE suggestions support.
 
 
-#### [`KeySym`](http://frederic.zinelli.gitlab.io/tkutils/key_sym/)
+#### [`KeySym`](http://frederic-zinelli.gitlab.io/tkutils/key_sym/)
 
 A utility to get all keysym information with auto-completion/IDE suggestions (providing string,
 keycode and keysym_num values).
 
 
-#### [`images`](http://frederic.zinelli.gitlab.io/tkutils/images/images/)
+#### [`images`](http://frederic-zinelli.gitlab.io/tkutils/images/images/)
 
 Various factories related to images to:
 
 * Simplify and reduce the typing needed,
 * Handle file conversions automatically,
 * Register automatically the image object on the host for the user (to avoid garbage collection).
 
@@ -81,15 +81,15 @@
 
 * Using an archive file (with the appropriate version number):
 
 ```bash
 pip install tkutils.1.0.2.tar.gz
 ```
 
-* Cloning the [GitLab repository](https://gitlab.com/frederic.zinelli/tkutils).
+* Cloning the [GitLab repository](https://gitlab.com/frederic-zinelli/tkutils).
 
 
 """
 
 from .helpers.event_provider import Event, EventStr
 from .helpers.keysym import KeySym
 from .grid_layout import GridLayout
```

### Comparing `tkutils-1.1.1/src/tkutils/grid_layout.py` & `tkutils-1.1.2/src/tkutils/grid_layout.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/helpers/event_provider.py` & `tkutils-1.1.2/src/tkutils/helpers/event_provider.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/helpers/keysym.py` & `tkutils-1.1.2/src/tkutils/helpers/keysym.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/images.py` & `tkutils-1.1.2/src/tkutils/images.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/menu_builder/bases.py` & `tkutils-1.1.2/src/tkutils/menu_builder/bases.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/menu_builder/menu_builder.py` & `tkutils-1.1.2/src/tkutils/menu_builder/menu_builder.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/menu_builder/menu_builder_options.py` & `tkutils-1.1.2/src/tkutils/menu_builder/menu_builder_options.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/two_way_binding/binder.py` & `tkutils-1.1.2/src/tkutils/two_way_binding/binder.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/two_way_binding/binding_descriptor.py` & `tkutils-1.1.2/src/tkutils/two_way_binding/binding_descriptor.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_binder_config.py` & `tkutils-1.1.2/src/tkutils/two_way_binding/configuration/_binder_config.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configuration.py` & `tkutils-1.1.2/src/tkutils/two_way_binding/configuration/_configuration.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py` & `tkutils-1.1.2/src/tkutils/two_way_binding/configuration/_configurer_image_factory.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/two_way_binding/errors.py` & `tkutils-1.1.2/src/tkutils/two_way_binding/errors.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/src/tkutils/utilities/singleton_namespace.py` & `tkutils-1.1.2/src/tkutils/utilities/singleton_namespace.py`

 * *Files identical despite different names*

### Comparing `tkutils-1.1.1/PKG-INFO` & `tkutils-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 Metadata-Version: 2.1
 Name: tkutils
-Version: 1.1.1
+Version: 1.1.2
 Summary: Python tkinter utilities.
-Home-page: http://frederic.zinelli.gitlab.io/tkutils/
-License: FreeBSD
+Home-page: http://frederic-zinelli.gitlab.io/tkutils/
 Author: Frédéric Zinelli
 Author-email: frederic.zinelli@gmail.com
 Requires-Python: >=3.8,<4.0
-Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: Pillow (>=9.3.0,<10.0.0)
-Requires-Dist: typing-extensions (>=4.4.0,<5.0.0)
-Project-URL: Repository, https://gitlab.com/frederic.zinelli/tkutils
+Requires-Dist: Pillow (>=9.3,<10.0)
+Requires-Dist: typing-extensions (>=4.4,<5.0)
+Project-URL: Repository, https://gitlab.com/frederic-zinelli/tkutils
 Description-Content-Type: text/markdown
 
 # Welcome to TkUtils
 
 `tkutils` is a package offering some additional logic and syntactic sugar when using `tkinter`.
 The main goal is to fill some gaps of tkinter, which might make it very annoying to use.
 
-Online version of the help documentation: http://frederic.zinelli.gitlab.io/tkutils/
+Online version of the help documentation: http://frederic-zinelli.gitlab.io/tkutils/
 
 
 
 ## Features
 
 
-### Additional logic: two-way binding, with [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/)
+### Additional logic: two-way binding, with [`Binder`](http://frederic-zinelli.gitlab.io/tkutils/binder/binder_overview/)
 
-The [`Binder`](http://frederic.zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
+The [`Binder`](http://frederic-zinelli.gitlab.io/tkutils/binder/binder_overview/) class is  to setup a transparent two-way
 binding reactivity between widgets and underlying object properties from the model/logic layer
 of the application.
 
 Several advantages come with this:
 
 * Changes of bound properties in the model layer are cascading in the GUI automatically.
 * The model layer of the application becomes (finally) totally independent from the presentation
@@ -44,39 +42,39 @@
   think about its integration with `tkinter` itself.
 
 
 
 ### Syntactic sugar
 
 
-#### [`GridLayout`](http://frederic.zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)
+#### [`GridLayout`](http://frederic-zinelli.gitlab.io/tkutils/grid_layout/grid_layout/)
 
 A grid layout manager which is abstracting away all the naughty `widget.grid(...)` calls and
 rows/columns grid configuration. Positioning widgets in the grid and controlling their "spanning"
 becomes very easy, without extra typing.
 
 
-#### [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
+#### [`MenuBuilder`](http://frederic-zinelli.gitlab.io/tkutils/menu_builder/menu_builder/)
 
 A helper to build menus and to abstract away all the technicalities encountered when creating menus through
-`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic.zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
+`tkinter`, which quickly make the declarations very unclear. Using the [`MenuBuilder`](http://frederic-zinelli.gitlab.io/tkutils/menu_builder/menu_builder/), the actual `Menu` hierarchy becomes very obvious: "what you see is what you get".
 
 
-#### [`Event`](http://frederic.zinelli.gitlab.io/tkutils/event/)
+#### [`Event`](http://frederic-zinelli.gitlab.io/tkutils/event/)
 
 A utility to build event strings with auto-completion/IDE suggestions support.
 
 
-#### [`KeySym`](http://frederic.zinelli.gitlab.io/tkutils/key_sym/)
+#### [`KeySym`](http://frederic-zinelli.gitlab.io/tkutils/key_sym/)
 
 A utility to get all keysym information with auto-completion/IDE suggestions (providing string,
 keycode and keysym_num values).
 
 
-#### [`images`](http://frederic.zinelli.gitlab.io/tkutils/images/images/)
+#### [`images`](http://frederic-zinelli.gitlab.io/tkutils/images/images/)
 
 Various factories related to images to:
 
 * Simplify and reduce the typing needed,
 * Handle file conversions automatically,
 * Register automatically the image object on the host for the user (to avoid garbage collection).
 
@@ -100,10 +98,10 @@
 
 * Using an archive file (with the appropriate version number):
 
 ```bash
 pip install tkutils.1.0.2.tar.gz
 ```
 
-* Cloning the [GitLab repository](https://gitlab.com/frederic.zinelli/tkutils).
+* Cloning the [GitLab repository](https://gitlab.com/frederic-zinelli/tkutils).
```

