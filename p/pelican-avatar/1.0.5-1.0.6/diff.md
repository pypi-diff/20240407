# Comparing `tmp/pelican_avatar-1.0.5.tar.gz` & `tmp/pelican_avatar-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Oct 30 20:22:06 2023, max compression
+gzip compressed data, was "pelican_avatar-1.0.6.tar", last modified: Sun Apr  7 09:30:08 2024, max compression
```

## Comparing `pelican_avatar-1.0.5.tar` & `pelican_avatar-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,5 @@
--rw-r--r--   0        0        0      201 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/.editorconfig
--rw-r--r--   0        0        0      735 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      610 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      559 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/CONTRIBUTING.md
--rw-r--r--   0        0        0       63 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/RELEASE.md
--rw-r--r--   0        0        0   123104 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/avatar-example.png
--rw-r--r--   0        0        0     3164 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/tasks.py
--rw-r--r--   0        0        0       50 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/tox.ini
--rw-r--r--   0        0        0       82 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/.github/FUNDING.yml
--rw-r--r--   0        0        0     2315 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/.github/workflows/main.yml
--rw-r--r--   0        0        0       36 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/pelican/plugins/avatar/__init__.py
--rw-r--r--   0        0        0     2938 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/pelican/plugins/avatar/avatar.py
--rw-r--r--   0        0        0     5512 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/pelican/plugins/avatar/test_avatar.py
--rw-r--r--   0        0        0       50 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/.gitignore
--rw-r--r--   0        0        0    34523 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/LICENSE
--rw-r--r--   0        0        0     5141 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/README.md
--rw-r--r--   0        0        0     2657 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     6580 2023-10-30 20:22:06.000000 pelican_avatar-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/LICENSE
+-rw-r--r--   0        0        0     5141 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/README.md
+-rw-r--r--   0        0        0     2311 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3164 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/tasks.py
+-rw-r--r--   0        0        0     6609 2024-04-07 09:30:02.000000 pelican_avatar-1.0.6/PKG-INFO
```

### Comparing `pelican_avatar-1.0.5/tasks.py` & `pelican_avatar-1.0.6/tasks.py`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.5/LICENSE` & `pelican_avatar-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.5/README.md` & `pelican_avatar-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pelican_avatar-1.0.5/pyproject.toml` & `pelican_avatar-1.0.6/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,101 +1,115 @@
 [project]
 name = "pelican-avatar"
-version = "1.0.5"
+version = "1.0.6"
 description = "Libravatar/Gravatar plugin for Pelican"
-authors = [{name = "Rafael Laboissière", email = "rafael@laboissiere.net"}]
-license = {text = "AGPL-3.0"}
+authors = [
+    { name = "Rafael Laboissière", email = "rafael@laboissiere.net" },
+]
 readme = "README.md"
-keywords = ["pelican", "plugin", "libravatar", "gravatar"]
+keywords = [
+    "pelican",
+    "plugin",
+    "libravatar",
+    "gravatar",
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
     "libgravatar>=0.2.5",
     "py3dns>=3.2",
     "pylibravatar>=1.7",
 ]
 
+[project.license]
+text = "AGPL-3.0"
+
 [project.urls]
 Homepage = "https://github.com/pelican-plugins/avatar"
 "Issue Tracker" = "https://github.com/pelican-plugins/avatar/issues"
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
     "ruff>=0.1.3",
 ]
 test = [
     "markdown>=3.4",
     "pytest>=7.0",
     "pytest-cov>=4.0",
     "pytest-sugar>=0.9.7",
 ]
 
-
 [tool.autopub]
 project-name = "Avatar"
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

### Comparing `pelican_avatar-1.0.5/PKG-INFO` & `pelican_avatar-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 Metadata-Version: 2.1
 Name: pelican-avatar
-Version: 1.0.5
+Version: 1.0.6
 Summary: Libravatar/Gravatar plugin for Pelican
-Project-URL: Homepage, https://github.com/pelican-plugins/avatar
-Project-URL: Issue Tracker, https://github.com/pelican-plugins/avatar/issues
-Project-URL: Funding, https://donate.getpelican.com/
-Author-email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican plugin libravatar gravatar
+Author-Email: Rafael Laboissière <rafael@laboissiere.net>
 License: AGPL-3.0
-License-File: LICENSE
-Keywords: gravatar,libravatar,pelican,plugin
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
+Project-URL: Homepage, https://github.com/pelican-plugins/avatar
+Project-URL: Issue tracker, https://github.com/pelican-plugins/avatar/issues
+Project-URL: Funding, https://donate.getpelican.com/
 Requires-Python: <4.0,>=3.8.1
-Requires-Dist: libgravatar>=0.2.5
 Requires-Dist: pelican>=4.5
+Requires-Dist: libgravatar>=0.2.5
 Requires-Dist: py3dns>=3.2
 Requires-Dist: pylibravatar>=1.7
+Requires-Dist: markdown>=3.4; extra == "markdown"
 Provides-Extra: markdown
-Requires-Dist: markdown>=3.4; extra == 'markdown'
 Description-Content-Type: text/markdown
 
 Avatar: A Plugin for Pelican
 ============================
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/avatar/main.yml?branch=main)](https://github.com/pelican-plugins/avatar/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-avatar)](https://pypi.org/project/pelican-avatar/)
```

