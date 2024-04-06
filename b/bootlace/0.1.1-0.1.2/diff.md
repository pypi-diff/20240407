# Comparing `tmp/bootlace-0.1.1.tar.gz` & `tmp/bootlace-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Mar 27 03:07:45 2024, max compression
+gzip compressed data, last modified: Sat Apr  6 22:06:50 2024, max compression
```

## Comparing `bootlace-0.1.1.tar` & `bootlace-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,79 @@
--rw-r--r--   0        0        0      247 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/__about__.py
--rw-r--r--   0        0        0      340 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/__init__.py
--rw-r--r--   0        0        0      411 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/_version.py
--rw-r--r--   0        0        0     8751 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/breadcrumbs.py
--rw-r--r--   0        0        0     1130 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/icon.py
--rw-r--r--   0        0        0      465 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/image.py
--rw-r--r--   0        0        0     1968 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/links.py
--rw-r--r--   0        0        0        0 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/py.typed
--rw-r--r--   0        0        0      669 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/size.py
--rw-r--r--   0        0        0     1217 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/style.py
--rw-r--r--   0        0        0     6892 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/util.py
--rw-r--r--   0        0        0        0 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/forms/__init__.py
--rw-r--r--   0        0        0     3037 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/forms/fields.py
--rw-r--r--   0        0        0      661 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/forms/widgets.py
--rw-r--r--   0        0        0     1571 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/forms/templates/bootlace/_form.html
--rw-r--r--   0        0        0      109 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/nav/__init__.py
--rw-r--r--   0        0        0     3972 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/nav/bar.py
--rw-r--r--   0        0        0     3518 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/nav/core.py
--rw-r--r--   0        0        0      427 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/nav/elements.py
--rw-r--r--   0        0        0     2475 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/nav/nav.py
--rw-r--r--   0        0        0      253 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/table/__init__.py
--rw-r--r--   0        0        0     4469 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/table/base.py
--rw-r--r--   0        0        0     2056 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/table/columns.py
--rw-r--r--   0        0        0       67 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/testing/__init__.py
--rw-r--r--   0        0        0     4910 2024-03-27 03:07:45.000000 bootlace-0.1.1/src/bootlace/testing/html.py
--rw-r--r--   0        0        0     1222 2024-03-27 03:07:45.000000 bootlace-0.1.1/.gitignore
--rw-r--r--   0        0        0     1096 2024-03-27 03:07:45.000000 bootlace-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0      478 2024-03-27 03:07:45.000000 bootlace-0.1.1/README.md
--rw-r--r--   0        0        0     2522 2024-03-27 03:07:45.000000 bootlace-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1323 2024-03-27 03:07:45.000000 bootlace-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      247 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/__about__.py
+-rw-r--r--   0        0        0      384 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/__init__.py
+-rw-r--r--   0        0        0      411 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/_version.py
+-rw-r--r--   0        0        0     8751 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/breadcrumbs.py
+-rw-r--r--   0        0        0     1447 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/extension.py
+-rw-r--r--   0        0        0     1139 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/icon.py
+-rw-r--r--   0        0        0      465 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/image.py
+-rw-r--r--   0        0        0     1968 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/links.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/py.typed
+-rw-r--r--   0        0        0      669 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/size.py
+-rw-r--r--   0        0        0     1217 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/style.py
+-rw-r--r--   0        0        0     6892 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/util.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/forms/__init__.py
+-rw-r--r--   0        0        0     3037 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/forms/fields.py
+-rw-r--r--   0        0        0      661 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/forms/widgets.py
+-rw-r--r--   0        0        0     1571 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/forms/templates/bootlace/_form.html
+-rw-r--r--   0        0        0      109 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/nav/__init__.py
+-rw-r--r--   0        0        0     3972 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/nav/bar.py
+-rw-r--r--   0        0        0     3518 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/nav/core.py
+-rw-r--r--   0        0        0      427 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/nav/elements.py
+-rw-r--r--   0        0        0     2475 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/nav/nav.py
+-rw-r--r--   0        0        0    70330 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203179 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51796 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115988 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70404 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203183 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51871 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116065 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12066 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129328 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10127 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51370 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12059 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129343 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10199 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63944 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107824 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267492 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85353 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180382 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107692 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267433 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85282 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180218 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   280814 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.css
+-rw-r--r--   0        0        0   679012 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232949 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589162 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280393 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   678857 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   233056 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   588696 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0    88585 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    47188 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/icons/bootstrap-icons.json
+-rw-r--r--   0        0        0   211136 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   972584 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/icons/bootstrap-icons.svg
+-rw-r--r--   0        0        0   207731 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444287 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80664 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   331887 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135747 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305153 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    74155 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222463 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145313 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.js
+-rw-r--r--   0        0        0   306321 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60578 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220351 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/static/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0      253 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/table/__init__.py
+-rw-r--r--   0        0        0     4469 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/table/base.py
+-rw-r--r--   0        0        0     2056 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/table/columns.py
+-rw-r--r--   0        0        0       67 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/testing/__init__.py
+-rw-r--r--   0        0        0     4910 2024-04-06 22:06:50.000000 bootlace-0.1.2/src/bootlace/testing/html.py
+-rw-r--r--   0        0        0     1222 2024-04-06 22:06:50.000000 bootlace-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1096 2024-04-06 22:06:50.000000 bootlace-0.1.2/LICENSE.txt
+-rw-r--r--   0        0        0      478 2024-04-06 22:06:50.000000 bootlace-0.1.2/README.md
+-rw-r--r--   0        0        0     2545 2024-04-06 22:06:50.000000 bootlace-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1323 2024-04-06 22:06:50.000000 bootlace-0.1.2/PKG-INFO
```

### Comparing `bootlace-0.1.1/src/bootlace/breadcrumbs.py` & `bootlace-0.1.2/src/bootlace/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/icon.py` & `bootlace-0.1.2/src/bootlace/icon.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 class Icon:
     """A Bootstrap icon
 
     This class supports the :func:`as_tag` protocol to display itself.
     """
 
     #: Endpoint name for getting the Bootstrap Icon SVG file
-    endpoint: ClassVar[str] = "static"
+    endpoint: ClassVar[str] = "bootlace.static"
 
     #: Filename for the Bootstrap Icon SVG file
     filename: ClassVar[str] = "icons/bootstrap-icons.svg"
 
     #: Name of the icon
     name: str
```

### Comparing `bootlace-0.1.1/src/bootlace/links.py` & `bootlace-0.1.2/src/bootlace/links.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/size.py` & `bootlace-0.1.2/src/bootlace/size.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/style.py` & `bootlace-0.1.2/src/bootlace/style.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/util.py` & `bootlace-0.1.2/src/bootlace/util.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/forms/fields.py` & `bootlace-0.1.2/src/bootlace/forms/fields.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/forms/widgets.py` & `bootlace-0.1.2/src/bootlace/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/forms/templates/bootlace/_form.html` & `bootlace-0.1.2/src/bootlace/forms/templates/bootlace/_form.html`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/nav/bar.py` & `bootlace-0.1.2/src/bootlace/nav/bar.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/nav/core.py` & `bootlace-0.1.2/src/bootlace/nav/core.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/nav/nav.py` & `bootlace-0.1.2/src/bootlace/nav/nav.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/table/base.py` & `bootlace-0.1.2/src/bootlace/table/base.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/table/columns.py` & `bootlace-0.1.2/src/bootlace/table/columns.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/src/bootlace/testing/html.py` & `bootlace-0.1.2/src/bootlace/testing/html.py`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/.gitignore` & `bootlace-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/LICENSE.txt` & `bootlace-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bootlace-0.1.1/pyproject.toml` & `bootlace-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,16 @@
   "def __hash__",
   "if TYPE_CHECKING:",
   "if __name__ == .__main__.:",
   "raise AssertionError",
   "raise NotImplementedError",
   "if 0:",
   "except BaseException:",
-  ": \\.\\.\\.",
+  "\\.\\.\\.",
+  "if app is not None:",
 ]
 omit = ["src/bootlace/_version.py", "src/bootlace/testing/*"]
 
 
 [tool.black]
 line-length = 120
```

### Comparing `bootlace-0.1.1/PKG-INFO` & `bootlace-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bootlace
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pythonic Bootstrap Utilities
 Project-URL: Documentation, https://github.com/alexrudy/bootlace#readme
 Project-URL: Issues, https://github.com/alexrudy/bootlace/issues
 Project-URL: Source, https://github.com/alexrudy/bootlace
 Author-email: Alex Rudy <github@alexrudy.net>
 License-Expression: MIT
 License-File: LICENSE.txt
```

