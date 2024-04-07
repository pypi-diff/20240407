# Comparing `tmp/pbt_simple-1.7.0.tar.gz` & `tmp/pbt_simple-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbt_simple-1.7.0.tar", max compression
+gzip compressed data, was "pbt_simple-1.7.1.tar", max compression
```

## Comparing `pbt_simple-1.7.0.tar` & `pbt_simple-1.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/LICENSE
--rw-r--r--   0        0        0      178 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/README.md
--rw-r--r--   0        0        0      952 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/__init__.py
--rw-r--r--   0        0        0     1224 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/__main__.py
--rw-r--r--   0        0        0        0 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/commands/__init__.py
--rw-r--r--   0        0        0     2684 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/commands/build.py
--rw-r--r--   0        0        0     1550 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/commands/git.py
--rw-r--r--   0        0        0    16053 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/commands/install.py
--rw-r--r--   0        0        0     1125 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/commands/list.py
--rw-r--r--   0        0        0     6728 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/config.py
--rw-r--r--   0        0        0     5611 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/misc.py
--rw-r--r--   0        0        0        0 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/package/__init__.py
--rw-r--r--   0        0        0    11788 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/package/discovery.py
--rw-r--r--   0        0        0     3452 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/package/graph.py
--rw-r--r--   0        0        0     6853 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/package/package.py
--rw-r--r--   0        0        0        0 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/registry/__init__.py
--rw-r--r--   0        0        0     2834 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/registry/pypi.py
--rw-r--r--   0        0        0      434 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/registry/registry.py
--rw-r--r--   0        0        0        0 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/vcs/__init__.py
--rw-r--r--   0        0        0    10514 2024-04-01 23:39:49.898494 pbt_simple-1.7.0/sbt/vcs/git.py
--rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/LICENSE
+-rw-r--r--   0        0        0      178 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/README.md
+-rw-r--r--   0        0        0      952 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/__init__.py
+-rw-r--r--   0        0        0     1224 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/__init__.py
+-rw-r--r--   0        0        0     2684 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/build.py
+-rw-r--r--   0        0        0     1550 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/git.py
+-rw-r--r--   0        0        0    16053 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/install.py
+-rw-r--r--   0        0        0     1125 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/commands/list.py
+-rw-r--r--   0        0        0     6728 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/config.py
+-rw-r--r--   0        0        0     5611 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/misc.py
+-rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/__init__.py
+-rw-r--r--   0        0        0    11823 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/discovery.py
+-rw-r--r--   0        0        0     3452 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/graph.py
+-rw-r--r--   0        0        0     6853 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/package/package.py
+-rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/registry/__init__.py
+-rw-r--r--   0        0        0     2834 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/registry/pypi.py
+-rw-r--r--   0        0        0      434 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/registry/registry.py
+-rw-r--r--   0        0        0        0 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/vcs/__init__.py
+-rw-r--r--   0        0        0    10514 2024-04-07 20:17:25.063980 pbt_simple-1.7.1/sbt/vcs/git.py
+-rw-r--r--   0        0        0     1365 1970-01-01 00:00:00.000000 pbt_simple-1.7.1/PKG-INFO
```

### Comparing `pbt_simple-1.7.0/LICENSE` & `pbt_simple-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/pyproject.toml` & `pbt_simple-1.7.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pbt-simple"
-version = "1.7.0"
+version = "1.7.1"
 description = "A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3."
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "sbt" }]
 homepage = "https://github.com/binh-vu/pbt-simple"
 repository = "https://github.com/binh-vu/pbt-simple"
```

### Comparing `pbt_simple-1.7.0/sbt/__main__.py` & `pbt_simple-1.7.1/sbt/__main__.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/commands/build.py` & `pbt_simple-1.7.1/sbt/commands/build.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/commands/git.py` & `pbt_simple-1.7.1/sbt/commands/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/commands/install.py` & `pbt_simple-1.7.1/sbt/commands/install.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/commands/list.py` & `pbt_simple-1.7.1/sbt/commands/list.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/config.py` & `pbt_simple-1.7.1/sbt/config.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/misc.py` & `pbt_simple-1.7.1/sbt/misc.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/package/discovery.py` & `pbt_simple-1.7.1/sbt/package/discovery.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,32 +71,32 @@
             pkgs[pkg.name] = pkg
 
     return pkgs
 
 
 def get_candidate_pyprojects(
     root: Path, ignore_dirs: set[Path], ignore_dirnames: set[str]
-):
-    outs = []
+) -> list[Path]:
+    outs = {}
     root = root.resolve()
 
     stack = [root]
     while len(stack) > 0:
         dir = stack.pop()
         if (
             dir.name.startswith(".")
             or dir.name in ignore_dirnames
             or dir in ignore_dirs
         ):
             continue
         if (dir / "pyproject.toml").exists():
-            outs.append(dir)
+            outs[dir.absolute()] = 1
         stack.extend([subdir for subdir in dir.iterdir() if subdir.is_dir()])
 
-    return outs
+    return list(outs.keys())
 
 
 def parse_pep518_pyproject(loc: Path) -> Package:
     """Parse project metadata from the directory.
 
     Arguments:
         pyproject_file: path to the pyproject.toml file
```

### Comparing `pbt_simple-1.7.0/sbt/package/graph.py` & `pbt_simple-1.7.1/sbt/package/graph.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/package/package.py` & `pbt_simple-1.7.1/sbt/package/package.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/registry/pypi.py` & `pbt_simple-1.7.1/sbt/registry/pypi.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/sbt/vcs/git.py` & `pbt_simple-1.7.1/sbt/vcs/git.py`

 * *Files identical despite different names*

### Comparing `pbt_simple-1.7.0/PKG-INFO` & `pbt_simple-1.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pbt-simple
-Version: 1.7.0
+Version: 1.7.1
 Summary: A simpler version of [PBT](https://github.com/binh-vu/pbt) for installing a package (and its local dependencies in editable mode) and build extension modules written in PYO3.
 Home-page: https://github.com/binh-vu/pbt-simple
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

