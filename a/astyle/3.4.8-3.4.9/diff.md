# Comparing `tmp/astyle-3.4.8.tar.gz` & `tmp/astyle-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astyle-3.4.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "astyle-3.4.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `astyle-3.4.8.tar` & `astyle-3.4.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 astyle-3.4.8/.cmake-format.yaml
--rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 astyle-3.4.8/.cmakelintrc
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 astyle-3.4.8/.github/dependabot.yml
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 astyle-3.4.8/.github/workflows/main.yml
--rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 astyle-3.4.8/.github/workflows/version.yml
--rw-r--r--   0        0        0     2358 2022-11-09 12:37:21.000000 astyle-3.4.8/.gitignore
--rwxr-xr-x   0        0        0      101 2022-11-09 12:37:21.000000 astyle-3.4.8/.gitlint
--rw-r--r--   0        0        0     3278 2022-11-09 12:37:21.000000 astyle-3.4.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 astyle-3.4.8/.pre-commit-hooks.yaml
--rwxr-xr-x   0        0        0      157 2022-11-09 12:37:21.000000 astyle-3.4.8/.yamllint.yaml
--rw-r--r--   0        0        0      942 2022-11-09 12:37:21.000000 astyle-3.4.8/CMakeLists.txt
--rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 astyle-3.4.8/LICENSE
--rw-r--r--   0        0        0     5466 2022-11-09 12:37:21.000000 astyle-3.4.8/README.md
--rw-r--r--   0        0        0     2357 2022-11-09 12:37:21.000000 astyle-3.4.8/pyproject.toml
--rwxr-xr-x   0        0        0      703 2022-11-09 12:37:21.000000 astyle-3.4.8/scripts/git-commit.sh
--rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 astyle-3.4.8/src/astyle/__init__.py
--rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 astyle-3.4.8/src/astyle/__main__.py
--rw-r--r--   0        0        0      274 2022-11-09 12:37:21.000000 astyle-3.4.8/src/astyle/_version.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 astyle-3.4.8/src/astyle/py.typed
--rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 astyle-3.4.8/tests/astyle_test.py
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 astyle-3.4.8/tests/expected.c
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 astyle-3.4.8/tests/input.c
--rw-r--r--   0        0        0     6954 2022-11-09 12:37:21.000000 astyle-3.4.8/PKG-INFO
+-rw-r--r--   0        0        0       20 2022-11-09 12:37:21.000000 astyle-3.4.9/.cmake-format.yaml
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 astyle-3.4.9/.cmakelintrc
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 astyle-3.4.9/.github/dependabot.yml
+-rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 astyle-3.4.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0      515 2022-11-09 12:37:21.000000 astyle-3.4.9/.github/workflows/version.yml
+-rw-r--r--   0        0        0     2364 2022-11-09 12:37:21.000000 astyle-3.4.9/.gitignore
+-rwxr-xr-x   0        0        0      101 2022-11-09 12:37:21.000000 astyle-3.4.9/.gitlint
+-rw-r--r--   0        0        0     3278 2022-11-09 12:37:21.000000 astyle-3.4.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 astyle-3.4.9/.pre-commit-hooks.yaml
+-rwxr-xr-x   0        0        0      157 2022-11-09 12:37:21.000000 astyle-3.4.9/.yamllint.yaml
+-rw-r--r--   0        0        0      518 2022-11-09 12:37:21.000000 astyle-3.4.9/CMakeLists.txt
+-rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 astyle-3.4.9/LICENSE
+-rw-r--r--   0        0        0     5782 2022-11-09 12:37:21.000000 astyle-3.4.9/README.md
+-rw-r--r--   0        0        0     2357 2022-11-09 12:37:21.000000 astyle-3.4.9/pyproject.toml
+-rwxr-xr-x   0        0        0      701 2022-11-09 12:37:21.000000 astyle-3.4.9/scripts/git-commit.sh
+-rw-r--r--   0        0        0      402 2022-11-09 12:37:21.000000 astyle-3.4.9/src/astyle/__init__.py
+-rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 astyle-3.4.9/src/astyle/__main__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 astyle-3.4.9/src/astyle/_version.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 astyle-3.4.9/src/astyle/py.typed
+-rw-r--r--   0        0        0      707 2022-11-09 12:37:21.000000 astyle-3.4.9/tests/astyle_test.py
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 astyle-3.4.9/tests/expected.c
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 astyle-3.4.9/tests/input.c
+-rw-r--r--   0        0        0     7270 2022-11-09 12:37:21.000000 astyle-3.4.9/PKG-INFO
```

### Comparing `astyle-3.4.8/.github/workflows/main.yml` & `astyle-3.4.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `astyle-3.4.8/.github/workflows/version.yml` & `astyle-3.4.9/.github/workflows/version.yml`

 * *Files identical despite different names*

### Comparing `astyle-3.4.8/.gitignore` & `astyle-3.4.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+data/
 _version.py
 *.ninja
 
 # create by https://github.com/iamcco/coc-gitignore (Thu May 18 2023 14:53:43 GMT+0800 (China Standard Time))
 # CMake.gitignore:
 CMakeLists.txt.user
 CMakeCache.txt
```

### Comparing `astyle-3.4.8/.pre-commit-config.yaml` & `astyle-3.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `astyle-3.4.8/LICENSE` & `astyle-3.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `astyle-3.4.8/README.md` & `astyle-3.4.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 ### pre-commit
 
 `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/Freed-Wu/mirrors-astyle
-    rev: 3.4.8
+    rev: 3.4.9
     hooks:
       - id: astyle
 ```
 
 ```shell
 pre-commit install
 git commit
@@ -84,17 +84,21 @@
 and will be faster than this repository which uses source code.
 
 ## Similar Projects
 
 ### pre-commit hooks
 
 - [mirrors-clang-format](https://github.com/pre-commit/mirrors-clang-format)
+- [CLinters](https://github.com/pocc/pre-commit-hooks): it requires you install
+  linters and formatters in your machine and it calls them. So it cannot
+  ensure the versions of linters and formatters are same as others, which means
+  it cannot ensure **reproducibility**.
 - [astyle_precommit_hook](https://github.com/mellowcandle/astyle_precommit_hook):
   it uses git hook, not pre-commit, which make it cannot use many hooks at the
-  same time.
+  same time. It cannot ensure **reproducibility**, too.
 - [pyastyle](https://github.com/timonwong/pyastyle): stop maintaining.
 - [astyle_py](https://github.com/igrr/astyle_py): it uses wasm, not native
   binary programs like this project.
 
 ### Python distributions
 
 - [clang-format-wheel](https://github.com/ssciwr/clang-format-wheel)
```

### Comparing `astyle-3.4.8/pyproject.toml` & `astyle-3.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astyle-3.4.8/scripts/git-commit.sh` & `astyle-3.4.9/scripts/git-commit.sh`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env bash
 cd "$(dirname "$(readlink -f "$0")")/.." || exit 1
 
 version="$(curl 'https://gitlab.com/api/v4/projects/41218592/repository/tags?per_page=1' | jq -r '.[].name')"
 perl -pi -e's/(?<=^    rev: )\S+/'"$version/" README.md
-perl -pi -e's/(?<=^set\(VERSION )\S+)/'"$version/" CMakeLists.txt
+perl -pi -e's/(?<=^set\(VERSION \S+/'"$version/" CMakeLists.txt
 [ -n "$(git diff)" ] || exit
 
 git add pyproject.toml README.md CMakeLists.txt
 git config --global user.name 'Github Actions'
 git config --global user.email '41898282+github-actions[bot]@users.noreply.github.com'
 git commit -m ":bookmark: Dump version to $version"
 git tag "$version"
```

### Comparing `astyle-3.4.8/tests/astyle_test.py` & `astyle-3.4.9/tests/astyle_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     def test_astyle(testcase, tmp_path: Path) -> None:
         r"""Test astyle."""
         input, expected = testcase
         output = os.path.join(tmp_path, input)
         input = os.path.join(os.path.dirname(__file__), input)
         expected = os.path.join(os.path.dirname(__file__), expected)
         copy(input, tmp_path)
-        astyle("--options=none", "--suffix=none", output)
+        assert astyle("--options=none", "--suffix=none", output) == 0
         assert Path(output).read_text() == Path(expected).read_text()
```

### Comparing `astyle-3.4.8/PKG-INFO` & `astyle-3.4.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astyle
-Version: 3.4.8
+Version: 3.4.9
 Summary: Artistic Style is a source code indenter, formatter, and beautifier for the C, C++, C++/CLI, Objective‑C, C# and Java programming languages
 Keywords: astyle
 Author-Email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -97,15 +97,15 @@
 ### pre-commit
 
 `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/Freed-Wu/mirrors-astyle
-    rev: 3.4.8
+    rev: 3.4.9
     hooks:
       - id: astyle
 ```
 
 ```shell
 pre-commit install
 git commit
@@ -115,17 +115,21 @@
 and will be faster than this repository which uses source code.
 
 ## Similar Projects
 
 ### pre-commit hooks
 
 - [mirrors-clang-format](https://github.com/pre-commit/mirrors-clang-format)
+- [CLinters](https://github.com/pocc/pre-commit-hooks): it requires you install
+  linters and formatters in your machine and it calls them. So it cannot
+  ensure the versions of linters and formatters are same as others, which means
+  it cannot ensure **reproducibility**.
 - [astyle_precommit_hook](https://github.com/mellowcandle/astyle_precommit_hook):
   it uses git hook, not pre-commit, which make it cannot use many hooks at the
-  same time.
+  same time. It cannot ensure **reproducibility**, too.
 - [pyastyle](https://github.com/timonwong/pyastyle): stop maintaining.
 - [astyle_py](https://github.com/igrr/astyle_py): it uses wasm, not native
   binary programs like this project.
 
 ### Python distributions
 
 - [clang-format-wheel](https://github.com/ssciwr/clang-format-wheel)
```

