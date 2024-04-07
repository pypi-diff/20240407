# Comparing `tmp/tinyfetch-0.0.2.tar.gz` & `tmp/tinyfetch-0.0.3.tar.gz`

## Comparing `tinyfetch-0.0.2.tar` & `tinyfetch-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/cli.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/core.py
--rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/src/tinyfetch/module.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/README.md
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 tinyfetch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/cli.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/core.py
+-rw-r--r--   0        0        0     2463 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/src/tinyfetch/module.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/README.md
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1973 2020-02-02 00:00:00.000000 tinyfetch-0.0.3/PKG-INFO
```

### Comparing `tinyfetch-0.0.2/src/tinyfetch/module.py` & `tinyfetch-0.0.3/src/tinyfetch/module.py`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.2/.gitignore` & `tinyfetch-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.2/LICENSE.txt` & `tinyfetch-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tinyfetch-0.0.2/pyproject.toml` & `tinyfetch-0.0.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 [project]
 name = "tinyfetch"
 dynamic = ["version"]
 description = "Python and system information command-line fetch tool"
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
-keywords = []
+keywords = [
+  "fetch", "python", "command-line", "tool", "information", "fetcher"
+]
 authors = [
   { name = "beucismis", email = "beucismis@tutamail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
@@ -28,14 +30,15 @@
 
 [project.urls]
 Source = "https://github.com/beucismis/tinyfetch"
 Issues = "https://github.com/beucismis/tinyfetch/issues"
 Documentation = "https://github.com/beucismis/tinyfetch#readme"
 
 [project.scripts]
+tfetch = "tinyfetch.cli:main"
 tinyfetch = "tinyfetch.cli:main"
 
 [tool.hatch.version]
 path = "src/tinyfetch/__init__.py"
 
 [tool.hatch.envs.default]
 dependencies = ["pytest"]
```

