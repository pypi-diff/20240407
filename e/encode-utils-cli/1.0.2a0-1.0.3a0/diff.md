# Comparing `tmp/encode_utils_cli-1.0.2a0.tar.gz` & `tmp/encode_utils_cli-1.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encode_utils_cli-1.0.2a0.tar", max compression
+gzip compressed data, was "encode_utils_cli-1.0.3a0.tar", max compression
```

## Comparing `encode_utils_cli-1.0.2a0.tar` & `encode_utils_cli-1.0.3a0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1065 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/LICENSE
--rw-r--r--   0        0        0      929 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/README.md
--rw-r--r--   0        0        0     3059 2024-03-15 14:20:14.862771 encode_utils_cli-1.0.2a0/pyproject.toml
--rw-r--r--   0        0        0       48 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/__init__.py
--rw-r--r--   0        0        0      156 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/__main__.py
--rw-r--r--   0        0        0      936 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/_cli.py
--rw-r--r--   0        0        0     2066 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/chapt2bmqpyml.py
--rw-r--r--   0        0        0      807 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/frames_denum.py
--rw-r--r--   0        0        0     1147 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/mpls2chap.py
--rw-r--r--   0        0        0      434 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/num_frames.py
--rw-r--r--   0        0        0     1193 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/re_chapters.py
--rw-r--r--   0        0        0     1186 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/re_titles.py
--rw-r--r--   0        0        0     1117 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/screens2bm.py
--rw-r--r--   0        0        0       48 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/util/__init__.py
--rw-r--r--   0        0        0     2364 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/util/load_mpls.py
--rw-r--r--   0        0        0      427 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/util/source.py
--rw-r--r--   0        0        0      670 2024-03-15 14:20:02.994809 encode_utils_cli-1.0.2a0/src/encode_utils_cli/util/timeconv.py
--rw-r--r--   0        0        0     2192 2024-03-15 14:20:02.998808 encode_utils_cli-1.0.2a0/src/encode_utils_cli/vs_screens.py
--rw-r--r--   0        0        0      755 2024-03-15 14:20:02.998808 encode_utils_cli-1.0.2a0/src/encode_utils_cli/zones_validator.py
--rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 encode_utils_cli-1.0.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/LICENSE
+-rw-r--r--   0        0        0     1196 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/README.md
+-rw-r--r--   0        0        0     3059 2024-04-07 15:41:30.422299 encode_utils_cli-1.0.3a0/pyproject.toml
+-rw-r--r--   0        0        0       48 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/__main__.py
+-rw-r--r--   0        0        0      936 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/_cli.py
+-rw-r--r--   0        0        0     2066 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/chapt2bmqpyml.py
+-rw-r--r--   0        0        0      807 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/frames_denum.py
+-rw-r--r--   0        0        0     1147 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/mpls2chap.py
+-rw-r--r--   0        0        0      434 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/num_frames.py
+-rw-r--r--   0        0        0     1193 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/re_chapters.py
+-rw-r--r--   0        0        0     1186 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/re_titles.py
+-rw-r--r--   0        0        0     1117 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/screens2bm.py
+-rw-r--r--   0        0        0       48 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/util/__init__.py
+-rw-r--r--   0        0        0     2364 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/util/load_mpls.py
+-rw-r--r--   0        0        0      427 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/util/source.py
+-rw-r--r--   0        0        0      670 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/util/timeconv.py
+-rw-r--r--   0        0        0     2192 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/vs_screens.py
+-rw-r--r--   0        0        0      755 2024-04-07 15:41:22.046223 encode_utils_cli-1.0.3a0/src/encode_utils_cli/zones_validator.py
+-rw-r--r--   0        0        0     2299 1970-01-01 00:00:00.000000 encode_utils_cli-1.0.3a0/PKG-INFO
```

### Comparing `encode_utils_cli-1.0.2a0/LICENSE` & `encode_utils_cli-1.0.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/README.md` & `encode_utils_cli-1.0.3a0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # encode-utils-cli
 
 > Encode utils collection
 
-[![PyPI version](https://img.shields.io/pypi/v/encode-utils-cli)](https://pypi.org/project/encode-utils-cli)
-[![Documentation](https://img.shields.io/badge/docs-github-blue.svg)](https://deadnews.github.io/encode-utils-cli)
-[![Main](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml)
-[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/encode-utils-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/encode-utils-cli/main)
-[![codecov](https://codecov.io/gh/DeadNews/encode-utils-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/encode-utils-cli)
+[![PyPI: Version](https://img.shields.io/pypi/v/encode-utils-cli?logo=pypi&logoColor=white)](https://pypi.org/project/encode-utils-cli)
+[![GitHub: Release](https://img.shields.io/github/v/release/deadnews/encode-utils-cli?logo=github&logoColor=white)](https://github.com/deadnews/encode-utils-cli/releases/latest)
+[![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/encode-utils-cli)
+[![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/encode-utils-cli/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/encode-utils-cli/main)
+[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/encode-utils-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/encode-utils-cli/actions/workflows/main.yml)
+[![CI: coverage](https://img.shields.io/codecov/c/github/deadnews/encode-utils-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/encode-utils-cli)
 
 ## Installation
 
 ```sh
-pip install encode-utils-cli
-# or
 pipx install encode-utils-cli
+# or
+pip install encode-utils-cli
 ```
-
-## CLI Reference
-
-<https://deadnews.github.io/encode-utils-cli/cli/>
```

### Comparing `encode_utils_cli-1.0.2a0/pyproject.toml` & `encode_utils_cli-1.0.3a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "encode-utils-cli"
-version = "1.0.2-alpha.0"
+version = "1.0.3-alpha.0"
 description = "Encode utils collection"
-authors = ["DeadNews <aurczpbgr@mozmail.com>"]
+authors = ["DeadNews <deadnewsgit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/deadnews/encode-utils-cli"
 repository = "https://github.com/deadnews/encode-utils-cli"
 documentation = "https://deadnews.github.io/encode-utils-cli"
 keywords = ["cli", "encode", "vapoursynth", "mpls"]
 classifiers = [
```

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/_cli.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/chapt2bmqpyml.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/chapt2bmqpyml.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/frames_denum.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/frames_denum.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/mpls2chap.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/mpls2chap.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/re_chapters.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/re_chapters.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/re_titles.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/re_titles.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/screens2bm.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/screens2bm.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/util/load_mpls.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/util/load_mpls.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/util/timeconv.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/util/timeconv.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/vs_screens.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/vs_screens.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/src/encode_utils_cli/zones_validator.py` & `encode_utils_cli-1.0.3a0/src/encode_utils_cli/zones_validator.py`

 * *Files identical despite different names*

### Comparing `encode_utils_cli-1.0.2a0/PKG-INFO` & `encode_utils_cli-1.0.3a0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: encode-utils-cli
-Version: 1.0.2a0
+Version: 1.0.3a0
 Summary: Encode utils collection
 Home-page: https://github.com/deadnews/encode-utils-cli
 License: MIT
 Keywords: cli,encode,vapoursynth,mpls
 Author: DeadNews
-Author-email: aurczpbgr@mozmail.com
+Author-email: deadnewsgit@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -26,25 +26,22 @@
 Project-URL: Repository, https://github.com/deadnews/encode-utils-cli
 Description-Content-Type: text/markdown
 
 # encode-utils-cli
 
 > Encode utils collection
 
-[![PyPI version](https://img.shields.io/pypi/v/encode-utils-cli)](https://pypi.org/project/encode-utils-cli)
-[![Documentation](https://img.shields.io/badge/docs-github-blue.svg)](https://deadnews.github.io/encode-utils-cli)
-[![Main](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml/badge.svg)](https://github.com/DeadNews/encode-utils-cli/actions/workflows/main.yml)
-[![pre-commit.ci](https://results.pre-commit.ci/badge/github/DeadNews/encode-utils-cli/main.svg)](https://results.pre-commit.ci/latest/github/DeadNews/encode-utils-cli/main)
-[![codecov](https://codecov.io/gh/DeadNews/encode-utils-cli/branch/main/graph/badge.svg?token=OCZDZIYPMC)](https://codecov.io/gh/DeadNews/encode-utils-cli)
+[![PyPI: Version](https://img.shields.io/pypi/v/encode-utils-cli?logo=pypi&logoColor=white)](https://pypi.org/project/encode-utils-cli)
+[![GitHub: Release](https://img.shields.io/github/v/release/deadnews/encode-utils-cli?logo=github&logoColor=white)](https://github.com/deadnews/encode-utils-cli/releases/latest)
+[![Documentation](https://img.shields.io/badge/documentation-gray.svg?logo=materialformkdocs&logoColor=white)](https://deadnews.github.io/encode-utils-cli)
+[![CI: pre-commit](https://results.pre-commit.ci/badge/github/DeadNews/encode-utils-cli/main.svg)](https://results.pre-commit.ci/latest/github/deadnews/encode-utils-cli/main)
+[![CI: main](https://img.shields.io/github/actions/workflow/status/deadnews/encode-utils-cli/main.yml?branch=main&logo=github&logoColor=white&label=main)](https://github.com/deadnews/encode-utils-cli/actions/workflows/main.yml)
+[![CI: coverage](https://img.shields.io/codecov/c/github/deadnews/encode-utils-cli?token=OCZDZIYPMC&logo=codecov&logoColor=white)](https://app.codecov.io/gh/deadnews/encode-utils-cli)
 
 ## Installation
 
 ```sh
-pip install encode-utils-cli
-# or
 pipx install encode-utils-cli
+# or
+pip install encode-utils-cli
 ```
 
-## CLI Reference
-
-<https://deadnews.github.io/encode-utils-cli/cli/>
-
```

