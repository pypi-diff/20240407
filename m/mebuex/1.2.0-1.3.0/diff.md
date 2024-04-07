# Comparing `tmp/mebuex-1.2.0.tar.gz` & `tmp/mebuex-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mebuex-1.2.0.tar", last modified: Fri Dec 29 20:42:34 2023, max compression
+gzip compressed data, was "mebuex-1.3.0.tar", last modified: Sun Apr  7 09:06:49 2024, max compression
```

## Comparing `mebuex-1.2.0.tar` & `mebuex-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-12-29 20:42:34.099845 mebuex-1.2.0/
--rw-r--r--   0 phd       (1000) phd       (1000)     1056 2022-07-13 11:17:33.000000 mebuex-1.2.0/LICENSE
--rw-r--r--   0 phd       (1000) phd       (1000)     4357 2023-12-29 20:42:34.099845 mebuex-1.2.0/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)     3593 2023-12-29 20:41:04.000000 mebuex-1.2.0/README.md
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-12-29 20:42:34.099845 mebuex-1.2.0/mebuex/
--rw-r--r--   0 phd       (1000) phd       (1000)      213 2022-07-13 11:31:24.000000 mebuex-1.2.0/mebuex/__init__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     5018 2023-12-29 18:33:29.000000 mebuex-1.2.0/mebuex/build_ext.py
--rw-r--r--   0 phd       (1000) phd       (1000)      799 2022-07-13 13:28:44.000000 mebuex-1.2.0/mebuex/extension.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-12-29 20:42:34.099845 mebuex-1.2.0/mebuex/scripts/
--rw-r--r--   0 phd       (1000) phd       (1000)      190 2023-12-29 19:50:02.000000 mebuex-1.2.0/mebuex/scripts/__init__.py
--rw-r--r--   0 phd       (1000) phd       (1000)     2173 2023-12-29 20:30:11.000000 mebuex-1.2.0/mebuex/scripts/gravelspoon.py
-drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2023-12-29 20:42:34.099845 mebuex-1.2.0/mebuex.egg-info/
--rw-r--r--   0 phd       (1000) phd       (1000)     4357 2023-12-29 20:42:34.000000 mebuex-1.2.0/mebuex.egg-info/PKG-INFO
--rw-r--r--   0 phd       (1000) phd       (1000)      330 2023-12-29 20:42:34.000000 mebuex-1.2.0/mebuex.egg-info/SOURCES.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        1 2023-12-29 20:42:34.000000 mebuex-1.2.0/mebuex.egg-info/dependency_links.txt
--rw-r--r--   0 phd       (1000) phd       (1000)       65 2023-12-29 20:42:34.000000 mebuex-1.2.0/mebuex.egg-info/entry_points.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        6 2023-12-29 20:42:34.000000 mebuex-1.2.0/mebuex.egg-info/requires.txt
--rw-r--r--   0 phd       (1000) phd       (1000)        7 2023-12-29 20:42:34.000000 mebuex-1.2.0/mebuex.egg-info/top_level.txt
--rw-r--r--   0 phd       (1000) phd       (1000)      914 2023-12-29 20:07:28.000000 mebuex-1.2.0/pyproject.toml
--rw-r--r--   0 phd       (1000) phd       (1000)       38 2023-12-29 20:42:34.099845 mebuex-1.2.0/setup.cfg
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-07 09:06:49.307089 mebuex-1.3.0/
+-rw-r--r--   0 phd       (1000) phd       (1000)     1056 2022-07-13 11:17:33.000000 mebuex-1.3.0/LICENSE
+-rw-r--r--   0 phd       (1000) phd       (1000)     4647 2024-04-07 09:06:49.307089 mebuex-1.3.0/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)     3883 2024-04-07 08:43:19.000000 mebuex-1.3.0/README.md
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-07 09:06:49.307089 mebuex-1.3.0/mebuex/
+-rw-r--r--   0 phd       (1000) phd       (1000)      213 2022-07-13 11:31:24.000000 mebuex-1.3.0/mebuex/__init__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     5162 2024-04-07 08:41:41.000000 mebuex-1.3.0/mebuex/build_ext.py
+-rw-r--r--   0 phd       (1000) phd       (1000)      938 2024-04-07 08:41:28.000000 mebuex-1.3.0/mebuex/extension.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-07 09:06:49.307089 mebuex-1.3.0/mebuex/scripts/
+-rw-r--r--   0 phd       (1000) phd       (1000)      190 2023-12-29 19:50:02.000000 mebuex-1.3.0/mebuex/scripts/__init__.py
+-rw-r--r--   0 phd       (1000) phd       (1000)     2173 2023-12-29 20:30:11.000000 mebuex-1.3.0/mebuex/scripts/gravelspoon.py
+drwxr-xr-x   0 phd       (1000) phd       (1000)        0 2024-04-07 09:06:49.307089 mebuex-1.3.0/mebuex.egg-info/
+-rw-r--r--   0 phd       (1000) phd       (1000)     4647 2024-04-07 09:06:49.000000 mebuex-1.3.0/mebuex.egg-info/PKG-INFO
+-rw-r--r--   0 phd       (1000) phd       (1000)      330 2024-04-07 09:06:49.000000 mebuex-1.3.0/mebuex.egg-info/SOURCES.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        1 2024-04-07 09:06:49.000000 mebuex-1.3.0/mebuex.egg-info/dependency_links.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)       65 2024-04-07 09:06:49.000000 mebuex-1.3.0/mebuex.egg-info/entry_points.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        6 2024-04-07 09:06:49.000000 mebuex-1.3.0/mebuex.egg-info/requires.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)        7 2024-04-07 09:06:49.000000 mebuex-1.3.0/mebuex.egg-info/top_level.txt
+-rw-r--r--   0 phd       (1000) phd       (1000)      914 2024-04-07 08:43:39.000000 mebuex-1.3.0/pyproject.toml
+-rw-r--r--   0 phd       (1000) phd       (1000)       38 2024-04-07 09:06:49.307089 mebuex-1.3.0/setup.cfg
```

### Comparing `mebuex-1.2.0/LICENSE` & `mebuex-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mebuex-1.2.0/PKG-INFO` & `mebuex-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mebuex
-Version: 1.2.0
+Version: 1.3.0
 Summary: Combining build_ext with the Meson build system
 Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
 License: MIT
 Project-URL: Homepage, https://github.com/mjziebarth/Mebuex
 Project-URL: Bug Tracker, https://github.com/mjziebarth/Mebuex/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -91,14 +91,21 @@
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+### [1.3.0] - 2024-04-07
+#### Added
+- Add the `mebuex_destpath` and `mebuex_destname` attributes to the
+  `MebuexExtension` class. This can be used from install scripts, after
+  performing the `build_ext` command, to retrieve the destination path
+  where the extension file was copied to.
+
 ### [1.2.0] - 2023-12-29
 #### Added
 - Add the `gravelspoon` command to break out of the setuptools build isolation
   and find the system NumPy includes.
 
 ### [1.1.7] - 2023-08-20
 #### Added
```

### Comparing `mebuex-1.2.0/README.md` & `mebuex-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,21 @@
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+### [1.3.0] - 2024-04-07
+#### Added
+- Add the `mebuex_destpath` and `mebuex_destname` attributes to the
+  `MebuexExtension` class. This can be used from install scripts, after
+  performing the `build_ext` command, to retrieve the destination path
+  where the extension file was copied to.
+
 ### [1.2.0] - 2023-12-29
 #### Added
 - Add the `gravelspoon` command to break out of the setuptools build isolation
   and find the system NumPy includes.
 
 ### [1.1.7] - 2023-08-20
 #### Added
```

### Comparing `mebuex-1.2.0/mebuex/build_ext.py` & `mebuex-1.3.0/mebuex/build_ext.py`

 * *Files 4% similar despite different names*

```diff
@@ -96,10 +96,15 @@
                                    "  pdir:     '" + str(pdir) + "'")
             destname = (destpath / filename).resolve()
             copy_file((Path(buildpath) / filename).resolve(),
                       destname, verbose=self.verbose,
                 dry_run=self.dry_run
             )
             # end of adapted code from setuptools/command/build_ext.py.
+
+            # Now make the destination paths available:
+            ext.mebuex_destpath = destpath
+            ext.mebuex_destname = destname
+
         else:
             # Normal build.
             super().build_extension(ext)
```

### Comparing `mebuex-1.2.0/mebuex/extension.py` & `mebuex-1.3.0/mebuex/extension.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,21 @@
 
 class MesonExtension(Extension):
     """
     An extension to be built using the Meson build system.
     This class assumes that a `meson.build` file resides in
     the root directory of the Python package sources.
     """
+    mebuex_destpath: Path | None
+    mebuex_destname: Path | None
+
     def __init__(self, name, builddir='builddir', compiledname=None):
         self.name = name
         self.builddir = builddir
         self.sourcepath = Path().resolve()
+        self.mebuex_destname = None
+        self.mebuex_destpath = None
         if compiledname is None:
             self.compiledname = name.split('.')[-1]
         else:
             self.compiledname = compiledname
         super().__init__(name, [])
```

### Comparing `mebuex-1.2.0/mebuex/scripts/gravelspoon.py` & `mebuex-1.3.0/mebuex/scripts/gravelspoon.py`

 * *Files identical despite different names*

### Comparing `mebuex-1.2.0/mebuex.egg-info/PKG-INFO` & `mebuex-1.3.0/mebuex.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mebuex
-Version: 1.2.0
+Version: 1.3.0
 Summary: Combining build_ext with the Meson build system
 Author-email: "Malte J. Ziebarth" <mjz.science@fmvkb.de>
 License: MIT
 Project-URL: Homepage, https://github.com/mjziebarth/Mebuex
 Project-URL: Bug Tracker, https://github.com/mjziebarth/Mebuex/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -91,14 +91,21 @@
 Mebuex is licensed under the MIT license (see the LICENSE file).
 
 ## Changelog
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 
+### [1.3.0] - 2024-04-07
+#### Added
+- Add the `mebuex_destpath` and `mebuex_destname` attributes to the
+  `MebuexExtension` class. This can be used from install scripts, after
+  performing the `build_ext` command, to retrieve the destination path
+  where the extension file was copied to.
+
 ### [1.2.0] - 2023-12-29
 #### Added
 - Add the `gravelspoon` command to break out of the setuptools build isolation
   and find the system NumPy includes.
 
 ### [1.1.7] - 2023-08-20
 #### Added
```

### Comparing `mebuex-1.2.0/pyproject.toml` & `mebuex-1.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61"]
 
 [project]
 name = "mebuex"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
     {name = "Malte J. Ziebarth", email = "mjz.science@fmvkb.de"},
 ]
 description = "Combining build_ext with the Meson build system"
 dependencies = [
     "meson"
 ]
```

