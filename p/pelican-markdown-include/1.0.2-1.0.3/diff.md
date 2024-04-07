# Comparing `tmp/pelican_markdown_include-1.0.2.tar.gz` & `tmp/pelican_markdown_include-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Oct 31 15:30:53 2023, max compression
+gzip compressed data, was "pelican_markdown_include-1.0.3.tar", last modified: Sun Apr  7 09:33:36 2024, max compression
```

## Comparing `pelican_markdown_include-1.0.2.tar` & `pelican_markdown_include-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,4 @@
--rw-r--r--   0        0        0      201 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/.editorconfig
--rw-r--r--   0        0        0      735 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      277 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/CHANGELOG.md
--rw-r--r--   0        0        0      569 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       38 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/RELEASE.md
--rw-r--r--   0        0        0     3168 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/tasks.py
--rw-r--r--   0        0        0     2325 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       40 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/pelican/plugins/md_include/__init__.py
--rw-r--r--   0        0        0     2583 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/pelican/plugins/md_include/md_include.py
--rw-r--r--   0        0        0     5126 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/pelican/plugins/md_include/test_md_include.py
--rw-r--r--   0        0        0       29 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/.gitignore
--rw-r--r--   0        0        0     4099 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/README.md
--rw-r--r--   0        0        0     2706 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     5559 2023-10-31 15:30:53.000000 pelican_markdown_include-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     4099 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/README.md
+-rw-r--r--   0        0        0     2357 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3168 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/tasks.py
+-rw-r--r--   0        0        0     5610 2024-04-07 09:33:30.000000 pelican_markdown_include-1.0.3/PKG-INFO
```

### Comparing `pelican_markdown_include-1.0.2/tasks.py` & `pelican_markdown_include-1.0.3/tasks.py`

 * *Files identical despite different names*

### Comparing `pelican_markdown_include-1.0.2/README.md` & `pelican_markdown_include-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pelican_markdown_include-1.0.2/pyproject.toml` & `pelican_markdown_include-1.0.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 [project]
 name = "pelican-markdown-include"
-version = "1.0.2"
+version = "1.0.3"
 description = "Pelican plugin for using the Markdown-Include extension"
-authors = [{name = "Rafael Laboissière", email = "rafael@laboissiere.net"}]
-license = {text = "AGPL-3.0"}
+authors = [
+    { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
+]
 readme = "README.md"
-keywords = ["pelican", "plugin", "markdown include"]
+keywords = [
+    "pelican",
+    "plugin",
+    "markdown include",
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
     "markdown>=3.4",
     "markdown-include>=0.8",
 ]
 
+[project.license]
+text = "AGPL-3.0"
+
 [project.urls]
 Homepage = "https://github.com/pelican-plugins/markdown-include"
 "Issue Tracker" = "https://github.com/pelican-plugins/markdown-include/issues"
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
@@ -55,46 +66,49 @@
 project-name = "Markdown Include"
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
+    "D100",
+    "D102",
+    "D104",
+    "D203",
+    "D213",
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

### Comparing `pelican_markdown_include-1.0.2/PKG-INFO` & `pelican_markdown_include-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: pelican-markdown-include
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pelican plugin for using the Markdown-Include extension
-Project-URL: Homepage, https://github.com/pelican-plugins/markdown-include
-Project-URL: Issue Tracker, https://github.com/pelican-plugins/markdown-include/issues
-Project-URL: Funding, https://donate.getpelican.com/
-Author-email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican plugin markdown include
+Author-Email: Rafael Laboissière <rafael@laboissiere.net>
 License: AGPL-3.0
-Keywords: markdown include,pelican,plugin
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
+Project-URL: Homepage, https://github.com/pelican-plugins/markdown-include
+Project-URL: Issue tracker, https://github.com/pelican-plugins/markdown-include/issues
+Project-URL: Funding, https://donate.getpelican.com/
 Requires-Python: <4.0,>=3.8.1
-Requires-Dist: markdown-include>=0.8
-Requires-Dist: markdown>=3.4
 Requires-Dist: pelican>=4.5
 Requires-Dist: py3dns>=3.2
+Requires-Dist: markdown>=3.4
+Requires-Dist: markdown-include>=0.8
+Requires-Dist: markdown>=3.4; extra == "markdown"
 Provides-Extra: markdown
-Requires-Dist: markdown>=3.4; extra == 'markdown'
 Description-Content-Type: text/markdown
 
 Markdown Include: A Plugin for Pelican
 ======================================
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/markdown-include/main.yml?branch=main)](https://github.com/pelican-plugins/markdown-include/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-markdown-include)](https://pypi.org/project/pelican-markdown-include/)
```

