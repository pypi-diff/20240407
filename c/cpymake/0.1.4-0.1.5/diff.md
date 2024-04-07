# Comparing `tmp/cpymake-0.1.4.tar.gz` & `tmp/cpymake-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpymake-0.1.4.tar", last modified: Sat Apr  6 02:24:07 2024, max compression
+gzip compressed data, was "cpymake-0.1.5.tar", last modified: Sun Apr  7 02:41:02 2024, max compression
```

## Comparing `cpymake-0.1.4.tar` & `cpymake-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.125668 cpymake-0.1.4/
--rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    45885 2024-04-06 02:24:07.125668 cpymake-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2024-04-02 00:10:44.000000 cpymake-0.1.4/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.094358 cpymake-0.1.4/cpymake/
--rw-rw-rw-   0        0        0      111 2024-04-05 23:31:11.000000 cpymake-0.1.4/cpymake/__init__.py
--rw-rw-rw-   0        0        0    13056 2024-04-06 02:23:31.000000 cpymake-0.1.4/cpymake/cpymake_build_ext.py
--rw-rw-rw-   0        0        0     2610 2024-04-05 23:49:42.000000 cpymake-0.1.4/cpymake/cpymake_extension.py
-drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.125668 cpymake-0.1.4/cpymake.egg-info/
--rw-rw-rw-   0        0        0    45885 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       28 2024-04-06 02:24:07.000000 cpymake-0.1.4/cpymake.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-06 02:24:07.125668 cpymake-0.1.4/docs/
--rw-rw-rw-   0        0        0     2065 2023-10-07 14:47:33.000000 cpymake-0.1.4/docs/conf.py
--rw-rw-rw-   0        0        0     1095 2024-04-06 02:23:57.000000 cpymake-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-06 02:24:07.125668 cpymake-0.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 02:41:02.469677 cpymake-0.1.5/
+-rw-rw-rw-   0        0        0    35823 2022-02-23 09:52:53.000000 cpymake-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0    45885 2024-04-07 02:41:02.467280 cpymake-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2024-04-07 02:40:07.000000 cpymake-0.1.5/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-07 02:41:02.358455 cpymake-0.1.5/cpymake/
+-rw-rw-rw-   0        0        0       35 2024-04-07 02:40:07.000000 cpymake-0.1.5/cpymake/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:41:02.436394 cpymake-0.1.5/cpymake/command/
+-rw-rw-rw-   0        0        0        0 2024-04-07 02:40:07.000000 cpymake-0.1.5/cpymake/command/__init__.py
+-rw-rw-rw-   0        0        0    16125 2024-04-07 02:40:07.000000 cpymake-0.1.5/cpymake/command/build_ext.py
+-rw-rw-rw-   0        0        0     2620 2024-04-07 02:40:07.000000 cpymake-0.1.5/cpymake/extension.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:41:02.464734 cpymake-0.1.5/cpymake.egg-info/
+-rw-rw-rw-   0        0        0    45885 2024-04-07 02:41:02.000000 cpymake-0.1.5/cpymake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2024-04-07 02:41:02.000000 cpymake-0.1.5/cpymake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:41:02.000000 cpymake-0.1.5/cpymake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-04-07 02:41:02.000000 cpymake-0.1.5/cpymake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       28 2024-04-07 02:41:02.000000 cpymake-0.1.5/cpymake.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 02:41:02.460650 cpymake-0.1.5/docs/
+-rw-rw-rw-   0        0        0     2065 2024-04-07 02:40:07.000000 cpymake-0.1.5/docs/conf.py
+-rw-rw-rw-   0        0        0     1089 2024-04-07 02:40:07.000000 cpymake-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 02:41:02.469677 cpymake-0.1.5/setup.cfg
```

### Comparing `cpymake-0.1.4/LICENSE` & `cpymake-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.4/PKG-INFO` & `cpymake-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.4
+Version: 0.1.5
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.4/README.rst` & `cpymake-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.4/cpymake/cpymake_build_ext.py` & `cpymake-0.1.5/cpymake/command/build_ext.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 """
 cpymake's build_ext command for building a python C/C++ extension using CMake
 """
 
 import os
-import pathlib
 import subprocess
 import sysconfig
 
 from typing import List
 
 from setuptools import errors
-from setuptools.command.build import SubCommand
-from setuptools.command.build_ext import build_ext
-from cpymake.cpymake_extension import CPyMakeExtension
 
+# VV Whilst a build_ext it's different enough to just extend from Command
+# (although distutils' original is way better)
+# NOTE: May wish to revert for other os' like darwin (mac?)
+# from setuptools.command.build_ext import build_ext
+from setuptools import Command
+from setuptools.command.build import SubCommand
+from cpymake.extension import Extension
 
-# NOTE:
-#   Whilst we do not use a lot of the variables set in setuptools' build_ext
-# and distutils' build_ext (although a few more of those are used) it could be safer to
-# just call their version in initalize and finalize options but at the same time ...
-# then again what hppens if they move more stuff from distutils to setuptools and change
-# the way some options are used (such as build-temp).
-#   Ideally we would just inherit distutils' version but that is deprecated so....
-#   Ah Forget it we're gonna rewrte all the *_options functions!
+# NOTE: By not inheriting from setuptools' build_ext (as we'd rather extend distutil's)
+# we have to reimplement a lot of methods but it (could) be worth it
 
 
 # Sub Command is a Protocol but we want to explicitly inherit
-class CPyMakeBuildExt(build_ext, SubCommand):  # pylint: disable=too-many-ancestors
+class build_ext(Command, SubCommand):  # pylint: disable=too-many-instance-attributes
     """CPyMake's build_ext class that can be used as a plugin for setuptools
     to build extension modules that use CMake as their build (generator) system
     """
 
     description = "build C/C++ extensions using CMake (compile/link to build directory)"
 
     user_options = [
@@ -44,16 +41,18 @@
                 "platform name to cross-compile for, if supported "
                 f"(default: {sysconfig.get_platform()})"
             ),
         ),
         (
             "inplace",
             "i",
-            "ignore build-lib and put compiled extensions into the source "
-            + "directory alongside your pure Python modules",
+            (
+                "ignore build-lib and put compiled extensions into the source "
+                "directory alongside your pure Python modules"
+            ),
         ),
         ("define=", "D", "C preprocessor macros to define"),
         ("undef=", "U", "C preprocessor macros to undefine"),
         ("debug", "g", "compile/link with debugging information"),
         ("force", "f", "forcibly build everything (ignore file timestamps)"),
         ("parallel=", "j", "number of parallel build jobs"),
     ]
@@ -64,29 +63,24 @@
     # help_options = [
     #     ("help-compiler", None, "list available compilers", show_compilers),
     # ]
 
     # override
     def initialize_options(self):
         # pylint: disable=attribute-defined-outside-init
-
         print("***** Initialize_options Called!")
 
         self.package = None
         self.extensions = None
 
         self.build_lib = None
         self.build_temp = None
         self.plat_name = None
         self.inplace = 0
         self.editable_mode = False
-        # self.ext_map = {} #<- I don't think we need this!
-        # self.ext_map = {}
-        # ^^ Irritatingly if we just add this we can use setuptools functions
-        # that expect this variable
 
         self.define = None
         self.undef = None
         self.debug = None
         self.force = None
         self.parallel = None
 
@@ -103,15 +97,15 @@
             ("debug", "debug"),
             ("force", "force"),
             ("parallel", "parallel"),
             ("plat_name", "plat_name"),
         )
 
         if self.package is None:
-            self.package = self.distribution.ext_package
+            self.package = self.distribution.ext_package  # <- what is this !!?
 
         self.extensions = self.distribution.ext_modules or []
 
         if os.name == "nt":
             if self.debug:
                 self.build_temp = os.path.join(self.build_temp, "Debug")
             else:
@@ -200,33 +194,54 @@
             print("******", extension)
             # Looks dodgy but it's been years since I made this so...
             # Actually maybe not...
             # self.package = (  # pylint: disable=attribute-defined-outside-init
             #     extension.package_name
             # )
             # extension_dir = self.get_extension_build_directory(extension.name)
-            extension_dir = self.build_lib
+            # extension_dir = os.path.abspath(
+            #     os.path.dirname(self.get_ext_fullpath(extension.name))
+            # )
+            # extension_path = "apep" #os.path.dirname(self.get_ext_fullpath(extension.name))
+            extension_path = os.path.dirname(self.get_ext_fullpath(extension.name))
+            extension_base = os.getcwd() #os.path.abspath(self.build_lib)
+
+            # print("extension_dir:", extension_path)#dir)
+            print("extension_path:", extension_path)#dir)
+            print("extension_base:", extension_base)#dir)
+            print("cwd:", os.getcwd())
             extension_suffix = (
                 # self.extension_suffix  # sysconfig.get_config_var("EXT_SUFFIX")
                 sysconfig.get_config_var("EXT_SUFFIX")
             )
+            print("extension fullname =", self.get_ext_fullname(extension.name))
+            print("extension filename =", self.get_ext_filename(extension.name))
+            print("extension fullpath =", self.get_ext_fullpath(extension.name))
 
             # Should I also allow this to be overridable in extension?
             config = "Debug" if self.debug else "Release"
             cmake_args = [
                 f"-DCMAKE_BUILD_TYPE={config}",
-                f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{config}={extension_dir}",
+                # f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY_{config}={extension_dir}",
+                f"-DCMAKE_LIBRARY_OUTPUT_DIRECTORY={extension_path}",
                 # Needed for windows (more specifically .dll platforms).
                 # It is safe to leave for all systems although will erroneously
                 # add any .exe's created, which shouldn't exist anyway
                 #
                 # May remove for .so systems but without further testing it is
                 # an unnecessary risk to remove
-                f"-DCMAKE_RUNTIME_OUTPUT_DIRECTORY_{config}={extension_dir}",
-                f"-DPYTHON_EXTENSION_SUFFIX={extension_suffix}",
+                # f"-DCMAKE_RUNTIME_OUTPUT_DIRECTORY_{config}={extension_dir}",
+                (
+                    "-DCMAKE_RUNTIME_OUTPUT_DIRECTORY="
+                    f"$<PATH:ABSOLUTE_PATH,{extension_path},{extension_base}>"
+                ),
+                # f"-DPYTHON_EXTENSION_SUFFIX={extension_suffix}",
+                f"-DPYTHON_EXTENSION={extension_suffix}",
+                #NOTE: VV Doesn't work on windows for some reason (being overwritten)
+                # f"-DCMAKE_SHARED_LIBRARY_SUFFIX={extension_suffix}",
             ]
             if extension.generator:
                 cmake_args.append(f"-G {extension.generator}")
 
             # Config -> outputs in our temp dir
             print(
                 "----- Configure:\n",
@@ -254,17 +269,18 @@
                 build_cmd.append(f"-j {self.parallel}")
             else:
                 build_cmd.append("-j")
 
             print("##### pre-run")
             print(
                 "----- Configure:\n",
-                subprocess.run(build_cmd, 
-                               # check=True
-                               )  # cwd=self.build_temp,
+                subprocess.run(
+                    build_cmd,
+                    # check=True
+                ),  # cwd=self.build_temp,
             )
             print("##### post-run")
 
     # TODO: These three functions need a rewrite! I think we can use special cmake
     # runs, unfortunatly I'm not 100% sure plus it may well
     # be considered "a side affect" although not really? but i guess configure is
     # required
@@ -278,25 +294,24 @@
 
         # They sort an interator and convert to dict but lets just make it here
 
         # might be neater to just use if rather than if not
         if not self.inplace:
             return {}
 
-        build_py = self.get_finalized_command("build_py")
         output_mapping = {}
 
         for ext in self.extensions:
-            inplace_file, regular_file = self._get_inplace_equivalent(build_py, ext)
+            inplace_file, regular_file = self.get_ext_paths(ext.name)
             output_mapping[regular_file] = inplace_file
 
         return output_mapping
 
     # override
-    def get_outputs(self) -> List[str]:
+    def get_outputs(self) -> list[str]:
         print("****** Get_outputs Called")
 
         # NOTE: Ideally we would also get clibs that the CMake extension requires/builds
         # unfortunatly I dont yet see how so for now.....
         # Can cmake tell us ??? I think so, so... what happens then can we use
         # vars set in run? will run have been "run" first?
 
@@ -331,16 +346,72 @@
         Raise Setuptools' SetupError if invalid extension found
         """
 
         print("***** Check_extensions_list Called")
 
         if not isinstance(extensions, list):
             raise errors.SetupError(
-                "'ext_modules' argument must be a list of CeMakeExtension instances "
+                "'ext_modules' argument must be a list of cpymake's "
+                "Extension instances "
                 f"however ext_modules had type {type(extensions)}"
             )
 
-        if not all(isinstance(ext, CPyMakeExtension) for ext in extensions):
+        if not all(isinstance(ext, Extension) for ext in extensions):
             raise errors.SetupError(
                 "Each element of 'ext_modules' must be an instance of "
-                "the CeMakeExtension class"
+                "the cpymake's Extension class"
             )
+
+    # -- Name generators -----------------------------------------------
+    def get_ext_fullname(self, ext_name: str) -> str:
+        """Adds the `package.` prefix"""
+        if self.package is None:
+            return ext_name
+
+        return self.package + "." + ext_name
+
+    def get_ext_filename(self, ext_name: str) -> str:
+        """Converts the name of an extension (eg. "foo.bar") into the name
+        of the file from which it will be loaded (eg. "foo/bar.so", or
+        "foo\bar.pyd").
+        """
+
+        ext_path = ext_name.split(".")
+        ext_suffix = os.getenv("CPYMAKE_EXT_SUFFIX") or sysconfig.get_config_var(
+            "EXT_SUFFIX"
+        )
+
+        return os.path.join(*ext_path) + ext_suffix
+
+    def get_ext_paths(self, ext_name) -> tuple[str, str]:
+        fullname = self.get_ext_fullname(ext_name)
+        modpath = fullname.split(".")
+
+        # TODO: Check for bugs as original code only used last elem of modpath
+        filename = self.get_ext_filename(fullname)
+        package = ".".join(modpath[:-1])
+
+        build_py = self.get_finalized_command("build_py")
+        package_dir = build_py.get_package_dir(package)  # type: ignore
+
+        # NOTE: os.path.basename required with this version. Depends on whether
+        # os.path.join (with multiple args) has greater complexity than
+        # os.path.basename (depends on whether concat is more complex than
+        # iteration (depending on C implementation))
+        inplace_file = os.path.join(package_dir, os.path.basename(filename))
+        regular_file = os.path.join(self.build_lib, filename)
+        return (inplace_file, regular_file)
+
+    def get_ext_fullpath(self, ext_name: str) -> str:
+        """Returns the path of the filename for a given extension.
+
+        The file is located in `build_lib` or directly in the package
+        (inplace option).
+        """
+        inplace_path, regular_path = self.get_ext_paths(ext_name)
+
+        if not self.inplace:
+            # returning: build_dir/package/path/filename
+            return regular_path
+
+        # returning: package_dir/filename
+        return os.path.abspath(inplace_path)
```

### Comparing `cpymake-0.1.4/cpymake/cpymake_extension.py` & `cpymake-0.1.5/cpymake/extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """ This module contains setuptools extension subclasses to allow 
 describing CMake builds to generate libraries for python extension 
 modules
 
 """
-import os.path
+# import os.path
 from dataclasses import dataclass
 
 from setuptools import errors
-from setuptools.extension import Extension
+from setuptools.extension import Extension as _Extension
 
 
 @dataclass
-class CPyMakeExtension(Extension):
+class Extension(_Extension):
     """This is the main ``Extension`` class for describing cmake python
     extension module builds.
 
     Attributes
     ----------
     package_name : str
       The name of the package, in dotted notation
```

### Comparing `cpymake-0.1.4/cpymake.egg-info/PKG-INFO` & `cpymake-0.1.5/cpymake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymake
-Version: 0.1.4
+Version: 0.1.5
 Summary: Allows building of CMake defined Python Extension modules
 Author-email: James Calo <jamesafcalo@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `cpymake-0.1.4/docs/conf.py` & `cpymake-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cpymake-0.1.4/pyproject.toml` & `cpymake-0.1.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cpymake"
-version = "0.1.4"
+version = "0.1.5"
 readme = "README.rst"
 description = "Allows building of CMake defined Python Extension modules"
 requires-python = ">=3.11"
 license = {file = "LICENSE"}
 authors = [
     {name = "James Calo", email = "jamesafcalo@gmail.com"},
 ]
@@ -25,14 +25,14 @@
 [project.urls]
 #Homepage = "https://example.com"
 #Documentation = "https://readthedocs.org"
 Repository = "https://github.com/SagaraBattousai/cpymake.git"
 #Changelog = "https://github.com/me/spam/blob/master/CHANGELOG.md"
 
 [project.entry-points."distutils.commands"]
-cpymake = "cpymake.cpymake_build_ext:CPyMakeBuildExt"
+cpymake = "cpymake.command.build_ext:build_ext"
 
 [tool.setuptools.packages.find]
 exclude = ["docs_build"] # temp
 
 [tool.black]
 preview = true
```

