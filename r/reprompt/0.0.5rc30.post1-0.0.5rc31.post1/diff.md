# Comparing `tmp/reprompt-0.0.5rc30.post1.tar.gz` & `tmp/reprompt-0.0.5rc31.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.5rc30.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.5rc31.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.5rc30.post1.tar` & `reprompt-0.0.5rc31.post1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      334 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1141 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/LICENSE
--rw-r--r--   0        0        0    15834 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/README.md
--rw-r--r--   0        0        0      634 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/docs/workflows.md
--rw-r--r--   0        0        0     6566 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/src/README.md
--rw-r--r--   0        0        0     2244 2024-04-07 02:04:15.307671 reprompt-0.0.5rc30.post1/src/reprompt/__init__.py
--rw-r--r--   0        0        0     3103 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/src/reprompt/custom_httpx.py
--rw-r--r--   0        0        0      920 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/tests/conftest.py
--rw-r--r--   0        0        0      532 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/tests/openai_example_script.py
--rw-r--r--   0        0        0      822 2024-04-07 02:03:59.947671 reprompt-0.0.5rc30.post1/tests/test_init.py
--rw-r--r--   0        0        0     1679 2024-04-07 02:03:59.951671 reprompt-0.0.5rc30.post1/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    17594 1970-01-01 00:00:00.000000 reprompt-0.0.5rc30.post1/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1141 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/LICENSE
+-rw-r--r--   0        0        0    15834 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/README.md
+-rw-r--r--   0        0        0      634 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6566 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/src/README.md
+-rw-r--r--   0        0        0     2246 2024-04-07 02:04:34.400733 reprompt-0.0.5rc31.post1/src/reprompt/__init__.py
+-rw-r--r--   0        0        0     3103 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/src/reprompt/custom_httpx.py
+-rw-r--r--   0        0        0      920 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/conftest.py
+-rw-r--r--   0        0        0      532 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/openai_example_script.py
+-rw-r--r--   0        0        0      822 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/test_init.py
+-rw-r--r--   0        0        0     1679 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    17594 1970-01-01 00:00:00.000000 reprompt-0.0.5rc31.post1/PKG-INFO
```

### Comparing `reprompt-0.0.5rc30.post1/.devcontainer/devcontainer.json` & `reprompt-0.0.5rc31.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.5rc31.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/.gitignore` & `reprompt-0.0.5rc31.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/.pre-commit-config.yaml` & `reprompt-0.0.5rc31.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/.vscode/settings.json` & `reprompt-0.0.5rc31.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/LICENSE` & `reprompt-0.0.5rc31.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/README.md` & `reprompt-0.0.5rc31.post1/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/docs/Makefile` & `reprompt-0.0.5rc31.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/docs/conf.py` & `reprompt-0.0.5rc31.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/docs/make.bat` & `reprompt-0.0.5rc31.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/docs/pylint.md` & `reprompt-0.0.5rc31.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/pyproject.toml` & `reprompt-0.0.5rc31.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/src/reprompt/__init__.py` & `reprompt-0.0.5rc31.post1/src/reprompt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #   -------------------------------------------------------------
 """Python Package Template"""
 from __future__ import annotations
 from typing import Callable
 
 from .tracing import FunctionTrace
 
-__version__ = "0.0.5-rc30-post1"
+__version__ = "0.0.5""-rc31-post1"
 
 import logging
 import functools
 import datetime
 import json
 
 # Configure logging
```

### Comparing `reprompt-0.0.5rc30.post1/src/reprompt/custom_httpx.py` & `reprompt-0.0.5rc31.post1/src/reprompt/custom_httpx.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/src/reprompt/tracing.py` & `reprompt-0.0.5rc31.post1/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/tests/conftest.py` & `reprompt-0.0.5rc31.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/tests/openai_example_script.py` & `reprompt-0.0.5rc31.post1/tests/openai_example_script.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/tests/test_init.py` & `reprompt-0.0.5rc31.post1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/tests/test_openai_tracing.py` & `reprompt-0.0.5rc31.post1/tests/test_openai_tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc30.post1/PKG-INFO` & `reprompt-0.0.5rc31.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.5rc30.post1
+Version: 0.0.5rc31.post1
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

