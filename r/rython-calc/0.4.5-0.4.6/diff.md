# Comparing `tmp/rython_calc-0.4.5.tar.gz` & `tmp/rython_calc-0.4.6.tar.gz`

## Comparing `rython_calc-0.4.5.tar` & `rython_calc-0.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.5/Cargo.toml
--rw-r--r--   0     1001      127      367 2024-04-07 13:13:46.000000 rython_calc-0.4.5/.github/dependabot.yml
--rw-r--r--   0     1001      127     4919 2024-04-07 13:13:46.000000 rython_calc-0.4.5/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-07 13:13:46.000000 rython_calc-0.4.5/.gitignore
--rw-r--r--   0     1001      127     1075 2024-04-07 13:13:46.000000 rython_calc-0.4.5/LICENSE
--rw-r--r--   0     1001      127      603 2024-04-07 13:13:46.000000 rython_calc-0.4.5/README.md
--rw-r--r--   0     1001      127    10298 2024-04-07 13:13:46.000000 rython_calc-0.4.5/poetry.lock
--rw-r--r--   0     1001      127        0 2024-04-07 13:13:46.000000 rython_calc-0.4.5/python/cli/__init__.py
--rw-r--r--   0     1001      127     1743 2024-04-07 13:13:46.000000 rython_calc-0.4.5/python/cli/main.py
--rw-r--r--   0     1001      127      443 2024-04-07 13:13:46.000000 rython_calc-0.4.5/python/cli/performance.txt
--rw-r--r--   0     1001      127        0 2024-04-07 13:13:46.000000 rython_calc-0.4.5/python/rython/__init__.py
--rw-r--r--   0     1001      127        0 2024-04-07 13:13:46.000000 rython_calc-0.4.5/python/rython/py.typed
--rw-r--r--   0     1001      127      666 2024-04-07 13:13:46.000000 rython_calc-0.4.5/python/rython/rython_calc.pyi
--rw-r--r--   0     1001      127     3030 2024-04-07 13:13:46.000000 rython_calc-0.4.5/src/lib.rs
--rw-r--r--   0     1001      127      347 2024-04-07 13:13:46.000000 rython_calc-0.4.5/test/rython/test_rython_calc.py
--rw-r--r--   0     1001      127     7857 2024-04-07 13:13:46.000000 rython_calc-0.4.5/Cargo.lock
--rw-r--r--   0     1001      127     1595 2024-04-07 13:13:46.000000 rython_calc-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 rython_calc-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 rython_calc-0.4.6/Cargo.toml
+-rw-r--r--   0     1001      127      367 2024-04-07 13:26:46.000000 rython_calc-0.4.6/.github/dependabot.yml
+-rw-r--r--   0     1001      127     4953 2024-04-07 13:26:46.000000 rython_calc-0.4.6/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-07 13:26:46.000000 rython_calc-0.4.6/.gitignore
+-rw-r--r--   0     1001      127     1075 2024-04-07 13:26:46.000000 rython_calc-0.4.6/LICENSE
+-rw-r--r--   0     1001      127      603 2024-04-07 13:26:46.000000 rython_calc-0.4.6/README.md
+-rw-r--r--   0     1001      127    10298 2024-04-07 13:26:46.000000 rython_calc-0.4.6/poetry.lock
+-rw-r--r--   0     1001      127        0 2024-04-07 13:26:46.000000 rython_calc-0.4.6/python/cli/__init__.py
+-rw-r--r--   0     1001      127     1743 2024-04-07 13:26:46.000000 rython_calc-0.4.6/python/cli/main.py
+-rw-r--r--   0     1001      127      443 2024-04-07 13:26:46.000000 rython_calc-0.4.6/python/cli/performance.txt
+-rw-r--r--   0     1001      127        0 2024-04-07 13:26:46.000000 rython_calc-0.4.6/python/rython/__init__.py
+-rw-r--r--   0     1001      127        0 2024-04-07 13:26:46.000000 rython_calc-0.4.6/python/rython/py.typed
+-rw-r--r--   0     1001      127      666 2024-04-07 13:26:46.000000 rython_calc-0.4.6/python/rython/rython_calc.pyi
+-rw-r--r--   0     1001      127     3030 2024-04-07 13:26:46.000000 rython_calc-0.4.6/src/lib.rs
+-rw-r--r--   0     1001      127      347 2024-04-07 13:26:46.000000 rython_calc-0.4.6/test/rython/test_rython_calc.py
+-rw-r--r--   0     1001      127     7857 2024-04-07 13:26:46.000000 rython_calc-0.4.6/Cargo.lock
+-rw-r--r--   0     1001      127     1595 2024-04-07 13:26:46.000000 rython_calc-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 rython_calc-0.4.6/PKG-INFO
```

### Comparing `rython_calc-0.4.5/.github/workflows/CI.yml` & `rython_calc-0.4.6/.github/workflows/CI.yml`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,15 @@
     runs-on: ubuntu-latest
     environment: release
     permissions:
       id-token: write
     if: startsWith(github.ref, 'refs/tags/')
     needs: [linux, windows, macos, sdist]
     steps:
+      - uses: actions/checkout@v4
       - uses: actions/download-artifact@v4
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         with:
           command: upload
           args: --non-interactive --skip-existing wheels-*/*
       - name: Publish release
```

### Comparing `rython_calc-0.4.5/.gitignore` & `rython_calc-0.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.5/LICENSE` & `rython_calc-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.5/README.md` & `rython_calc-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.5/poetry.lock` & `rython_calc-0.4.6/poetry.lock`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.5/python/cli/main.py` & `rython_calc-0.4.6/python/cli/main.py`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.5/python/rython/rython_calc.pyi` & `rython_calc-0.4.6/python/rython/rython_calc.pyi`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.5/src/lib.rs` & `rython_calc-0.4.6/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rython_calc-0.4.5/Cargo.lock` & `rython_calc-0.4.6/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "rython"
-version = "0.4.5"
+version = "0.4.6"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
```

### Comparing `rython_calc-0.4.5/pyproject.toml` & `rython_calc-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.5,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "rython_calc"
 requires-python = ">=3.12"
-version = "0.4.5"
+version = "0.4.6"
 description = "Small project developed by me to learn PyO3 library."
 authors = [
     {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
 ]
 maintainers = [
     {name = "Krystian Krakowski", email = "kkrakowski22@gmail.com"}
 ]
@@ -31,15 +31,15 @@
 python-source = "python"
 bindings = "pyo3"
 module-name = "rython.rython_calc"
 strip = true
 
 [tool.poetry]
 name = "rython_calc"
-version = "0.4.5"
+version = "0.4.6"
 description = "Small project developed by me to learn PyO3 library."
 authors = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 maintainers = ["Krystian Krakowski <kkrakowski22@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `rython_calc-0.4.5/PKG-INFO` & `rython_calc-0.4.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: rython_calc
-Version: 0.4.5
+Version: 0.4.6
 Classifier: Development Status :: 1 - Planning
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Small project developed by me to learn PyO3 library.
 Author-email: Krystian Krakowski <kkrakowski22@gmail.com>
```

