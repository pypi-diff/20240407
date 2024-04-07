# Comparing `tmp/rython_calc-0.4.3.tar.gz` & `tmp/rython_calc-0.4.4.tar.gz`

## Comparing `rython_calc-0.4.3.tar` & `rython_calc-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.3/Cargo.toml
--rw-r--r--   0     1001      127      367 2024-04-05 19:40:45.000000 rython_calc-0.4.3/.github/dependabot.yml
--rw-r--r--   0     1001      127     4911 2024-04-05 19:40:45.000000 rython_calc-0.4.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-05 19:40:45.000000 rython_calc-0.4.3/.gitignore
--rw-r--r--   0     1001      127     1075 2024-04-05 19:40:45.000000 rython_calc-0.4.3/LICENSE
--rw-r--r--   0     1001      127      603 2024-04-05 19:40:45.000000 rython_calc-0.4.3/README.md
--rw-r--r--   0     1001      127    10298 2024-04-05 19:40:45.000000 rython_calc-0.4.3/poetry.lock
--rw-r--r--   0     1001      127        0 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/cli/__init__.py
--rw-r--r--   0     1001      127     1743 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/cli/main.py
--rw-r--r--   0     1001      127      443 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/cli/performance.txt
--rw-r--r--   0     1001      127        0 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/rython/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/rython/py.typed
--rw-r--r--   0     1001      127      666 2024-04-05 19:40:45.000000 rython_calc-0.4.3/python/rython/rython_calc.pyi
--rw-r--r--   0     1001      127     3030 2024-04-05 19:40:45.000000 rython_calc-0.4.3/src/lib.rs
--rw-r--r--   0     1001      127      347 2024-04-05 19:40:45.000000 rython_calc-0.4.3/test/rython/test_rython_calc.py
--rw-r--r--   0     1001      127     7857 2024-04-05 19:40:45.000000 rython_calc-0.4.3/Cargo.lock
--rw-r--r--   0     1001      127     1057 2024-04-05 19:40:45.000000 rython_calc-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1120 1970-01-01 00:00:00.000000 rython_calc-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.4/Cargo.toml
+-rw-r--r--   0     1001      127      367 2024-04-07 11:54:23.000000 rython_calc-0.4.4/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4911 2024-04-07 11:54:23.000000 rython_calc-0.4.4/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-07 11:54:23.000000 rython_calc-0.4.4/.gitignore
+-rw-r--r--   0     1001      127     1075 2024-04-07 11:54:23.000000 rython_calc-0.4.4/LICENSE
+-rw-r--r--   0     1001      127      603 2024-04-07 11:54:23.000000 rython_calc-0.4.4/README.md
+-rw-r--r--   0     1001      127    10298 2024-04-07 11:54:23.000000 rython_calc-0.4.4/poetry.lock
+-rw-r--r--   0     1001      127        0 2024-04-07 11:54:23.000000 rython_calc-0.4.4/python/cli/__init__.py
+-rw-r--r--   0     1001      127     1743 2024-04-07 11:54:23.000000 rython_calc-0.4.4/python/cli/main.py
+-rw-r--r--   0     1001      127      443 2024-04-07 11:54:23.000000 rython_calc-0.4.4/python/cli/performance.txt
+-rw-r--r--   0     1001      127        0 2024-04-07 11:54:23.000000 rython_calc-0.4.4/python/rython/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-07 11:54:23.000000 rython_calc-0.4.4/python/rython/py.typed
+-rw-r--r--   0     1001      127      666 2024-04-07 11:54:23.000000 rython_calc-0.4.4/python/rython/rython_calc.pyi
+-rw-r--r--   0     1001      127     3030 2024-04-07 11:54:23.000000 rython_calc-0.4.4/src/lib.rs
+-rw-r--r--   0     1001      127      347 2024-04-07 11:54:23.000000 rython_calc-0.4.4/test/rython/test_rython_calc.py
+-rw-r--r--   0     1001      127     7857 2024-04-07 11:54:23.000000 rython_calc-0.4.4/Cargo.lock
+-rw-r--r--   0     1001      127     1595 2024-04-07 11:54:23.000000 rython_calc-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 rython_calc-0.4.4/PKG-INFO
```

### Comparing `rython_calc-0.4.3/.github/workflows/CI.yml` & `rython_calc-0.4.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/.gitignore` & `rython_calc-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/LICENSE` & `rython_calc-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/README.md` & `rython_calc-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/poetry.lock` & `rython_calc-0.4.4/poetry.lock`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/python/cli/main.py` & `rython_calc-0.4.4/python/cli/main.py`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/python/rython/rython_calc.pyi` & `rython_calc-0.4.4/python/rython/rython_calc.pyi`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/src/lib.rs` & `rython_calc-0.4.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.3/Cargo.lock` & `rython_calc-0.4.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rython"
-version = "0.4.3"
+version = "0.4.4"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
```

### Comparing `rython_calc-0.4.3/pyproject.toml` & `rython_calc-0.4.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,47 +1,57 @@
-[tool.poetry]
-name = "rython-calc"
-version = "0.4.3"
-description = "Rython package to test python and rust compatibility"
-authors = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
-readme = "README.md"
-license = "MIT"
-
-[tool.poetry.dependencies]
-python = "^3.12"
-
-[tool.poetry.group.dev.dependencies]
-maturin = "^1.5.1"
-pytest = "^8.1.1"
-mypy = "^1.9.0"
-
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rython_calc"
 requires-python = ">=3.12"
+version = "0.4.4"
+description = "Small project developed by me to learn PyO3 library."
+authors = [
+    {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
+]
+maintainers = [
+    {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
+]
+readme = {file = "README.md", content-type = "text/markdown"}
+license = {file = "LICENSE"}
 classifiers = [
+    "Development Status :: 1 - Planning",
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
-authors = [
-    {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
-]
-dynamic = [
-    "license",
-    "readme",
-    "version"
-]
 
 [project.urls]
 Homepage = "https://github.com/fawq/Rython"
 Source = "https://github.com/fawq/Rython"
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 python-source = "python"
 bindings = "pyo3"
 module-name = "rython.rython_calc"
 strip = true
+
+[tool.poetry]
+name = "rython_calc"
+version = "0.4.4"
+description = "Small project developed by me to learn PyO3 library."
+authors = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
+maintainers = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
+readme = "README.md"
+license = "MIT"
+classifiers = [
+    "Development Status :: 1 - Planning",
+    "Programming Language :: Rust",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Programming Language :: Python :: Implementation :: PyPy",
+]
+
+[tool.poetry.dependencies]
+python = "^3.12"
+
+[tool.poetry.group.dev.dependencies]
+maturin = "^1.5.1"
+pytest = "^8.1.1"
+mypy = "^1.9.0"
```

### Comparing `rython_calc-0.4.3/PKG-INFO` & `rython_calc-0.4.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 Metadata-Version: 2.3
 Name: rython_calc
-Version: 0.4.3
+Version: 0.4.4
+Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
+Summary: Small project developed by me to learn PyO3 library.
 Author-email: Krystian Krakowski <kkrakowski22@gmail.com>
+Maintainer-email: Krystian Krakowski <kkrakowski22@gmail.com>
 Requires-Python: >=3.12
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Description-Content-Type: text/markdown
 Project-URL: Homepage, https://github.com/fawq/Rython
 Project-URL: Source, https://github.com/fawq/Rython
 
 # Rython
 
 ## Use text_signature to create python type
```

