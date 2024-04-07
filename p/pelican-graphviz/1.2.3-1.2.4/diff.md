# Comparing `tmp/pelican_graphviz-1.2.3.tar.gz` & `tmp/pelican_graphviz-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Oct 31 12:14:06 2023, max compression
+gzip compressed data, was "pelican_graphviz-1.2.4.tar", last modified: Sun Apr  7 09:37:46 2024, max compression
```

## Comparing `pelican_graphviz-1.2.3.tar` & `pelican_graphviz-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,5 @@
--rw-r--r--   0        0        0      201 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/.editorconfig
--rw-r--r--   0        0        0      735 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1093 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/CHANGELOG.md
--rw-r--r--   0        0        0      561 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      105 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/RELEASE.md
--rw-r--r--   0        0        0     6011 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/hello-world.png
--rw-r--r--   0        0        0     3166 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/tasks.py
--rw-r--r--   0        0        0       50 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/tox.ini
--rw-r--r--   0        0        0       82 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/.github/FUNDING.yml
--rw-r--r--   0        0        0     2399 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/.github/workflows/main.yml
--rw-r--r--   0        0        0       38 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/pelican/plugins/graphviz/__init__.py
--rw-r--r--   0        0        0     2282 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/pelican/plugins/graphviz/graphviz.py
--rw-r--r--   0        0        0     6621 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/pelican/plugins/graphviz/mdx_graphviz.py
--rw-r--r--   0        0        0     6519 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/pelican/plugins/graphviz/test_graphviz.py
--rw-r--r--   0        0        0       59 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/.gitignore
--rw-r--r--   0        0        0    34523 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/LICENSE
--rw-r--r--   0        0        0     6654 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/README.md
--rw-r--r--   0        0        0     2672 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     8036 2023-10-31 12:14:06.000000 pelican_graphviz-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/LICENSE
+-rw-r--r--   0        0        0     6654 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/README.md
+-rw-r--r--   0        0        0     2280 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     3166 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/tasks.py
+-rw-r--r--   0        0        0     8065 2024-04-07 09:37:41.000000 pelican_graphviz-1.2.4/PKG-INFO
```

### Comparing `pelican_graphviz-1.2.3/tasks.py` & `pelican_graphviz-1.2.4/tasks.py`

 * *Files identical despite different names*

### Comparing `pelican_graphviz-1.2.3/LICENSE` & `pelican_graphviz-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_graphviz-1.2.3/README.md` & `pelican_graphviz-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pelican_graphviz-1.2.3/pyproject.toml` & `pelican_graphviz-1.2.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,100 +1,113 @@
 [project]
 name = "pelican-graphviz"
-version = "1.2.3"
+version = "1.2.4"
 description = "Pelican plugin supporting Graphviz images in articles"
-authors = [{name = "Rafael Laboissière", email = "rafael@laboissiere.net"}]
-license = {text = "AGPL-3.0"}
+authors = [
+    { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
+]
 readme = "README.md"
-keywords = ["pelican", "plugin", "graphviz"]
+keywords = [
+    "pelican",
+    "plugin",
+    "graphviz",
+]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Framework :: Pelican",
     "Framework :: Pelican :: Plugins",
     "Intended Audience :: End Users/Desktop",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python = ">=3.8.1,<4.0"
 dependencies = [
     "pelican>=4.5",
     "py3dns>=3.2",
 ]
 
+[project.license]
+text = "AGPL-3.0"
+
 [project.urls]
 Homepage = "https://github.com/pelican-plugins/graphviz"
 "Issue Tracker" = "https://github.com/pelican-plugins/graphviz/issues"
 Funding = "https://donate.getpelican.com/"
 
 [project.optional-dependencies]
-markdown = ["markdown>=3.4"]
+markdown = [
+    "markdown>=3.4",
+]
 
 [tool.pdm.dev-dependencies]
 lint = [
     "black>=23.10.1",
     "invoke>=2.2.0",
-    "ruff>=0.1.3",
+    "ruff>=0.1.8",
 ]
 test = [
     "markdown>=3.4",
     "pytest>=7.0",
     "pytest-cov>=4.0",
     "pytest-sugar>=0.9.7",
 ]
 
-
 [tool.autopub]
 project-name = "Graphviz"
 git-username = "botpub"
 git-email = "52496925+botpub@users.noreply.github.com"
 append-github-contributor = true
 
 [tool.ruff]
 select = [
-  "B",   # flake8-bugbear
-  "BLE", # flake8-blind-except
-  "C4",  # flake8-comprehensions
-  "D",   # pydocstyle
-  "E",   # pycodestyle
-  "F",   # pyflakes
-  "I",   # isort
-  "ICN", # flake8-import-conventions
-  "ISC", # flake8-implicit-str-concat
-  "PGH", # pygrep-hooks
-  "PL",  # pylint
-  "RET", # flake8-return
-  "RUF", # ruff-specific rules
-  "SIM", # flake8-simplify
-  "T10", # flake8-debugger
-  "T20", # flake8-print
-  "TID", # flake8-tidy-imports
-  "TRY", # tryceratops
-  "UP",  # pyupgrade
-  "W",   # pycodestyle
-  "YTT", # flake8-2020
+    "B",
+    "BLE",
+    "C4",
+    "D",
+    "E",
+    "F",
+    "I",
+    "ICN",
+    "ISC",
+    "PGH",
+    "PL",
+    "RET",
+    "RUF",
+    "SIM",
+    "T10",
+    "T20",
+    "TID",
+    "TRY",
+    "UP",
+    "W",
+    "YTT",
 ]
-
 ignore = [
-  "D100",    # missing docstring in public module
-  "D102",    # missing docstring in public method
-  "D104",    # missing docstring in public package
-  "PLR0913", # too many arguments in function definition
+    "D100",
+    "D102",
+    "D104",
+    "D203",
+    "D213",
+    "PLR0913",
 ]
 
-target-version = "py38"
-
 [tool.ruff.isort]
 combine-as-imports = true
 force-sort-within-sections = true
-known-first-party = ["pelican"]
+known-first-party = [
+    "pelican",
+]
 
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = [
+    "pdm-backend",
+]
+build-backend = "pdm.backend"
```

### Comparing `pelican_graphviz-1.2.3/PKG-INFO` & `pelican_graphviz-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: pelican-graphviz
-Version: 1.2.3
+Version: 1.2.4
 Summary: Pelican plugin supporting Graphviz images in articles
-Project-URL: Homepage, https://github.com/pelican-plugins/graphviz
-Project-URL: Issue Tracker, https://github.com/pelican-plugins/graphviz/issues
-Project-URL: Funding, https://donate.getpelican.com/
-Author-email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican plugin graphviz
+Author-Email: Rafael Laboissière <rafael@laboissiere.net>
 License: AGPL-3.0
-License-File: LICENSE
-Keywords: graphviz,pelican,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Homepage, https://github.com/pelican-plugins/graphviz
+Project-URL: Issue tracker, https://github.com/pelican-plugins/graphviz/issues
+Project-URL: Funding, https://donate.getpelican.com/
 Requires-Python: <4.0,>=3.8.1
 Requires-Dist: pelican>=4.5
 Requires-Dist: py3dns>=3.2
+Requires-Dist: markdown>=3.4; extra == "markdown"
 Provides-Extra: markdown
-Requires-Dist: markdown>=3.4; extra == 'markdown'
 Description-Content-Type: text/markdown
 
 Graphviz: A Plugin for Pelican
 ==============================
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/graphviz/main.yml?branch=main)](https://github.com/pelican-plugins/graphviz/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-graphviz)](https://pypi.org/project/pelican-graphviz/)
```

