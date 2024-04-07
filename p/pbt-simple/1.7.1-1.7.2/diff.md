# Comparing `tmp/pbt_simple-1.7.1.tar.gz` & `tmp/pbt_simple-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbt_simple-1.7.1.tar", max compression
+gzip compressed data, was "pbt_simple-1.7.2.tar", max compression
```

## Comparing `pbt_simple-1.7.1.tar` & `pbt_simple-1.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/LICENSE
--rw-r--r--   0        0        0      178 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/README.md
--rw-r--r--   0        0        0      952 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/__init__.py
--rw-r--r--   0        0        0     1224 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/__main__.py
--rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/build.py
--rw-r--r--   0        0        0     1550 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/git.py
--rw-r--r--   0        0        0    16053 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/install.py
--rw-r--r--   0        0        0     1125 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/list.py
--rw-r--r--   0        0        0     6728 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/config.py
--rw-r--r--   0        0        0     5611 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/misc.py
--rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/__init__.py
--rw-r--r--   0        0        0    11823 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/discovery.py
--rw-r--r--   0        0        0     3452 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/graph.py
--rw-r--r--   0        0        0     6853 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/package.py
--rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/registry/__init__.py
--rw-r--r--   0        0        0     2834 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/registry/pypi.py
--rw-r--r--   0        0        0      434 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/registry/registry.py
--rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/vcs/__init__.py
--rw-r--r--   0        0        0    10514 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/vcs/git.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/LICENSE
+-rw-r--r--   0        0        0      178 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/README.md
+-rw-r--r--   0        0        0      952 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/__init__.py
+-rw-r--r--   0        0        0     1224 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/commands/__init__.py
+-rw-r--r--   0        0        0     2684 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/commands/build.py
+-rw-r--r--   0        0        0     1550 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/commands/git.py
+-rw-r--r--   0        0        0    16053 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/commands/install.py
+-rw-r--r--   0        0        0     1209 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/commands/list.py
+-rw-r--r--   0        0        0     6728 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/config.py
+-rw-r--r--   0        0        0     5611 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/misc.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/package/__init__.py
+-rw-r--r--   0        0        0    12017 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/package/discovery.py
+-rw-r--r--   0        0        0     3452 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/package/graph.py
+-rw-r--r--   0        0        0     6853 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/package/package.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/registry/__init__.py
+-rw-r--r--   0        0        0     2834 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/registry/pypi.py
+-rw-r--r--   0        0        0      434 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/registry/registry.py
+-rw-r--r--   0        0        0        0 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/vcs/__init__.py
+-rw-r--r--   0        0        0    10514 2024-04-07 21:19:47.669496 pbt_simple-1.7.2/sbt/vcs/git.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.2/PKG-INFO
```

### Comparing `pbt_simple-1.7.1/LICENSE` & `pbt_simple-1.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/pyproject.toml` & `pbt_simple-1.7.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbt-simple"
-version = "1.7.1"
+version = "1.7.2"
 description = "A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3."
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "sbt" }]
 homepage = "https://github.com/binh-vu/pbt-simple"
 repository = "https://github.com/binh-vu/pbt-simple"
```

### Comparing `pbt_simple-1.7.1/sbt/__main__.py` & `pbt_simple-1.7.2/sbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/commands/build.py` & `pbt_simple-1.7.2/sbt/commands/build.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/commands/git.py` & `pbt_simple-1.7.2/sbt/commands/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/commands/install.py` & `pbt_simple-1.7.2/sbt/commands/install.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/commands/list.py` & `pbt_simple-1.7.2/sbt/commands/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import os
 
 import click
+
 from sbt.config import PBTConfig
-from sbt.package.discovery import (
-    discover_packages,
-)
+from sbt.package.discovery import discover_packages
 
 # environment variables that will be passed to the subprocess
 PASSTHROUGH_ENVS = [
     "PATH",
     "CC",
     "CXX",
     "LIBCLANG_PATH",
@@ -27,26 +26,29 @@
 @click.command()
 @click.option("--cwd", default=".", help="Override current working directory")
 @click.option(
     "--ignore-invalid-pkg",
     is_flag=True,
     help="whether to ignore invalid packages",
 )
+@click.option("-v", "--verbose", count=True)
 def list(
     cwd: str = ".",
     ignore_invalid_pkg: bool = False,
+    verbose: int = 0,
 ):
     cwd = os.path.abspath(cwd)
     cfg = PBTConfig.from_dir(cwd)
 
     # discovery packages
     packages = discover_packages(
         cfg.cwd,
         cfg.cache_dir,
         cfg.ignore_directories,
         cfg.ignore_directory_names,
         ignore_invalid_package=ignore_invalid_pkg,
+        verbose=verbose,
     )
 
     print("Found the following packages:")
     for package in packages.values():
         print("\t-", package.name)
```

### Comparing `pbt_simple-1.7.1/sbt/config.py` & `pbt_simple-1.7.2/sbt/config.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/misc.py` & `pbt_simple-1.7.2/sbt/misc.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/package/discovery.py` & `pbt_simple-1.7.2/sbt/package/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,34 +4,38 @@
 import re
 from operator import attrgetter
 from pathlib import Path
 from typing import cast
 
 import semver
 from loguru import logger
+from tomlkit.api import loads
+
 from sbt.misc import InvalidPackageError
 from sbt.package.package import (
     DepConstraint,
     DepConstraints,
     Package,
     PackageType,
     VersionSpec,
 )
-from tomlkit.api import loads
 
 
 def discover_packages(
     root: Path,
     cache_dir: Path,
     ignore_dirs: set[Path],
     ignore_dirnames: set[str],
     ignore_invalid_package: bool = False,
+    verbose: int = 0,
 ):
     """Find all packages in the given directory and manually linked/installed packages."""
-    candidate_pyprojects = get_candidate_pyprojects(root, ignore_dirs, ignore_dirnames)
+    candidate_pyprojects = get_candidate_pyprojects(
+        root, ignore_dirs, ignore_dirnames, verbose=verbose
+    )
 
     # mapping from package directory to its configuration
     pkgs: dict[str, Package] = {}
 
     for loc in candidate_pyprojects:
         try:
             pkg = parse_pep518_pyproject(loc)
@@ -70,22 +74,26 @@
                 )
             pkgs[pkg.name] = pkg
 
     return pkgs
 
 
 def get_candidate_pyprojects(
-    root: Path, ignore_dirs: set[Path], ignore_dirnames: set[str]
+    root: Path, ignore_dirs: set[Path], ignore_dirnames: set[str], verbose: int = 0
 ) -> list[Path]:
     outs = {}
     root = root.resolve()
 
+    if verbose >= 3:
+        print("Scaning directories for packages...")
     stack = [root]
     while len(stack) > 0:
         dir = stack.pop()
+        if verbose >= 3:
+            print(dir)
         if (
             dir.name.startswith(".")
             or dir.name in ignore_dirnames
             or dir in ignore_dirs
         ):
             continue
         if (dir / "pyproject.toml").exists():
```

### Comparing `pbt_simple-1.7.1/sbt/package/graph.py` & `pbt_simple-1.7.2/sbt/package/graph.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/package/package.py` & `pbt_simple-1.7.2/sbt/package/package.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/registry/pypi.py` & `pbt_simple-1.7.2/sbt/registry/pypi.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/sbt/vcs/git.py` & `pbt_simple-1.7.2/sbt/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.1/PKG-INFO` & `pbt_simple-1.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbt-simple
-Version: 1.7.1
+Version: 1.7.2
 Summary: A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3.
 Home-page: https://github.com/binh-vu/pbt-simple
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

