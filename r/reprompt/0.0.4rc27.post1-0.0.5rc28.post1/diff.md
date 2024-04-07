# Comparing `tmp/reprompt-0.0.4rc27.post1.tar.gz` & `tmp/reprompt-0.0.5rc28.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.4rc27.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.5rc28.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.4rc27.post1.tar` & `reprompt-0.0.5rc28.post1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0      334 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1141 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/LICENSE
--rw-r--r--   0        0        0    14940 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/README.md
--rw-r--r--   0        0        0      634 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/workflows.md
--rw-r--r--   0        0        0     6566 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/src/README.md
--rw-r--r--   0        0        0     2244 2024-04-07 01:56:19.728235 reprompt-0.0.4rc27.post1/src/reprompt/__init__.py
--rw-r--r--   0        0        0     3103 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/src/reprompt/custom_httpx.py
--rw-r--r--   0        0        0      920 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/conftest.py
--rw-r--r--   0        0        0      532 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/openai_example_script.py
--rw-r--r--   0        0        0      822 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/test_init.py
--rw-r--r--   0        0        0     1211 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/test_methods.py
--rw-r--r--   0        0        0     1679 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    16700 1970-01-01 00:00:00.000000 reprompt-0.0.4rc27.post1/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1141 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/LICENSE
+-rw-r--r--   0        0        0    15834 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/README.md
+-rw-r--r--   0        0        0      634 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-07 01:58:38.623006 reprompt-0.0.5rc28.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6566 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/src/README.md
+-rw-r--r--   0        0        0     2244 2024-04-07 01:58:51.910963 reprompt-0.0.5rc28.post1/src/reprompt/__init__.py
+-rw-r--r--   0        0        0     3103 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/src/reprompt/custom_httpx.py
+-rw-r--r--   0        0        0      920 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/tests/conftest.py
+-rw-r--r--   0        0        0      532 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/tests/openai_example_script.py
+-rw-r--r--   0        0        0      822 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/tests/test_init.py
+-rw-r--r--   0        0        0     1679 2024-04-07 01:58:38.627006 reprompt-0.0.5rc28.post1/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    17594 1970-01-01 00:00:00.000000 reprompt-0.0.5rc28.post1/PKG-INFO
```

### Comparing `reprompt-0.0.4rc27.post1/.devcontainer/devcontainer.json` & `reprompt-0.0.5rc28.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.5rc28.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/.gitignore` & `reprompt-0.0.5rc28.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/.pre-commit-config.yaml` & `reprompt-0.0.5rc28.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/.vscode/settings.json` & `reprompt-0.0.5rc28.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/LICENSE` & `reprompt-0.0.5rc28.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/README.md` & `reprompt-0.0.5rc28.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+# Instructions
+
+
+Once you have a venv
+
+```
+pip install flit
+```
+
+Navigate to the project root and run:
+
+```
+flit install --symlink
+```
+
+This command installs the package in editable mode (similar to pip install -e .), allowing you to make
+changes to the code and see them reflected without reinstalling.
+
+Running the Tests
+Run Tests with pytest:
+
+```
+pytest
+```
+
+This command discovers and runs all tests in the tests directory.
+
+
+## How do I release a new version of reprompt?
+
+The repository is configured to automatically upload the package to PyPI when the version number changes. This is handled by a GitHub Actions workflow defined in .github/workflows/CI.yml. To trigger the upload:
+
+1. Change the version number in `src/reprompt/__init__.py`
+2. Commit and Push the changes to your repository.
+3. The GitHub Actions workflow will automatically build the package and upload it to PyPI.
+
+
 # Python Project Template
 
 This project is a template for creating Python projects that follows the Python Standards declared in PEP 621. It uses a pyproject.yaml file to configure the project and Flit to simplify the build process and publish to PyPI. Flit simplifies the build and packaging process for Python projects by eliminating the need for separate setup.py and setup.cfg files. With Flit, you can manage all relevant configurations within the pyproject.toml file, streamlining development and promoting maintainability by centralizing project metadata, dependencies, and build specifications in one place.
 
 ## Project Organization
 
 - `.github/workflows`: Contains GitHub Actions used for building, testing, and publishing.
```

### Comparing `reprompt-0.0.4rc27.post1/docs/Makefile` & `reprompt-0.0.5rc28.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/docs/conf.py` & `reprompt-0.0.5rc28.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/docs/make.bat` & `reprompt-0.0.5rc28.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/docs/pylint.md` & `reprompt-0.0.5rc28.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/pyproject.toml` & `reprompt-0.0.5rc28.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/src/reprompt/__init__.py` & `reprompt-0.0.5rc28.post1/src/reprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #   -------------------------------------------------------------
 """Python Package Template"""
 from __future__ import annotations
 from typing import Callable
 
 from .tracing import FunctionTrace
 
-__version__ = "0.0.4-rc27-post1"
+__version__ = "0.0.5-rc28-post1"
 
 import logging
 import functools
 import datetime
 import json
 
 # Configure logging
```

### Comparing `reprompt-0.0.4rc27.post1/src/reprompt/custom_httpx.py` & `reprompt-0.0.5rc28.post1/src/reprompt/custom_httpx.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/src/reprompt/tracing.py` & `reprompt-0.0.5rc28.post1/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/tests/conftest.py` & `reprompt-0.0.5rc28.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/tests/openai_example_script.py` & `reprompt-0.0.5rc28.post1/tests/openai_example_script.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/tests/test_init.py` & `reprompt-0.0.5rc28.post1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/tests/test_openai_tracing.py` & `reprompt-0.0.5rc28.post1/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4rc27.post1/PKG-INFO` & `reprompt-0.0.5rc28.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.4rc27.post1
+Version: 0.0.5rc28.post1
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -33,14 +33,51 @@
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
 Project-URL: Documentation, https://github.com/syncup-ai/reprompt/tree/main#readme
 Project-URL: Source, https://github.com/syncup-ai/reprompt
 Project-URL: Tracker, https://github.com/syncup-ai/reprompt/issues
 Provides-Extra: spark
 Provides-Extra: test
 
+# Instructions
+
+
+Once you have a venv
+
+```
+pip install flit
+```
+
+Navigate to the project root and run:
+
+```
+flit install --symlink
+```
+
+This command installs the package in editable mode (similar to pip install -e .), allowing you to make
+changes to the code and see them reflected without reinstalling.
+
+Running the Tests
+Run Tests with pytest:
+
+```
+pytest
+```
+
+This command discovers and runs all tests in the tests directory.
+
+
+## How do I release a new version of reprompt?
+
+The repository is configured to automatically upload the package to PyPI when the version number changes. This is handled by a GitHub Actions workflow defined in .github/workflows/CI.yml. To trigger the upload:
+
+1. Change the version number in `src/reprompt/__init__.py`
+2. Commit and Push the changes to your repository.
+3. The GitHub Actions workflow will automatically build the package and upload it to PyPI.
+
+
 # Python Project Template
 
 This project is a template for creating Python projects that follows the Python Standards declared in PEP 621. It uses a pyproject.yaml file to configure the project and Flit to simplify the build process and publish to PyPI. Flit simplifies the build and packaging process for Python projects by eliminating the need for separate setup.py and setup.cfg files. With Flit, you can manage all relevant configurations within the pyproject.toml file, streamlining development and promoting maintainability by centralizing project metadata, dependencies, and build specifications in one place.
 
 ## Project Organization
 
 - `.github/workflows`: Contains GitHub Actions used for building, testing, and publishing.
```

