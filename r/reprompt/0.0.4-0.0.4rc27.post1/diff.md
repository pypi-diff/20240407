# Comparing `tmp/reprompt-0.0.4.tar.gz` & `tmp/reprompt-0.0.4rc27.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.4rc27.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.4.tar` & `reprompt-0.0.4rc27.post1.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0      334 2024-04-07 00:25:03.403742 reprompt-0.0.4/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-07 00:25:03.403879 reprompt-0.0.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-07 00:25:03.404063 reprompt-0.0.4/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-07 00:25:03.404188 reprompt-0.0.4/.github/template-sync.yml
--rw-r--r--   0        0        0      476 2024-04-07 00:25:03.404366 reprompt-0.0.4/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 00:25:03.404493 reprompt-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-07 00:25:03.404614 reprompt-0.0.4/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-07 00:25:03.404736 reprompt-0.0.4/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-07 00:25:03.404859 reprompt-0.0.4/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-07 00:25:03.404977 reprompt-0.0.4/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-07 00:25:03.405111 reprompt-0.0.4/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-07 01:12:32.734093 reprompt-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-07 01:11:22.577276 reprompt-0.0.4/.pypirc
--rw-r--r--   0        0        0      459 2024-04-07 00:25:03.405530 reprompt-0.0.4/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-07 00:25:03.405655 reprompt-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0     1141 2024-04-07 00:25:03.405762 reprompt-0.0.4/LICENSE
--rw-r--r--   0        0        0    14940 2024-04-07 00:25:03.405914 reprompt-0.0.4/README.md
--rw-r--r--   0        0        0      634 2024-04-07 00:25:03.406066 reprompt-0.0.4/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-07 00:25:03.406173 reprompt-0.0.4/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-07 00:25:03.406277 reprompt-0.0.4/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-07 00:25:03.406376 reprompt-0.0.4/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-07 00:25:03.406480 reprompt-0.0.4/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-07 00:25:03.406590 reprompt-0.0.4/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-07 00:25:03.406687 reprompt-0.0.4/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-07 00:25:03.406789 reprompt-0.0.4/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-07 00:25:03.406919 reprompt-0.0.4/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-07 00:25:03.407022 reprompt-0.0.4/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-07 00:25:03.407129 reprompt-0.0.4/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-07 00:25:03.407228 reprompt-0.0.4/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-07 00:25:03.407318 reprompt-0.0.4/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-07 00:25:03.407408 reprompt-0.0.4/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-07 00:25:03.407512 reprompt-0.0.4/docs/workflows.md
--rw-r--r--   0        0        0     6566 2024-04-07 00:26:35.378824 reprompt-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-07 00:25:03.407795 reprompt-0.0.4/src/README.md
--rw-r--r--   0        0        0     2233 2024-04-07 01:12:59.525166 reprompt-0.0.4/src/reprompt/__init__.py
--rw-r--r--   0        0        0     3103 2024-04-07 01:01:45.897266 reprompt-0.0.4/src/reprompt/custom_httpx.py
--rw-r--r--   0        0        0      920 2024-04-07 00:45:42.223861 reprompt-0.0.4/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-07 00:25:03.408249 reprompt-0.0.4/tests/conftest.py
--rw-r--r--   0        0        0     1211 2024-04-07 00:25:03.408345 reprompt-0.0.4/tests/test_methods.py
--rw-r--r--   0        0        0      532 2024-04-07 00:25:03.408445 reprompt-0.0.4/tests/test_openai_trace.py
--rw-r--r--   0        0        0    16690 1970-01-01 00:00:00.000000 reprompt-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      476 2024-04-07 01:56:06.292040 reprompt-0.0.4rc27.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      318 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0      368 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1141 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/LICENSE
+-rw-r--r--   0        0        0    14940 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/README.md
+-rw-r--r--   0        0        0      634 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6566 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/src/README.md
+-rw-r--r--   0        0        0     2244 2024-04-07 01:56:19.728235 reprompt-0.0.4rc27.post1/src/reprompt/__init__.py
+-rw-r--r--   0        0        0     3103 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/src/reprompt/custom_httpx.py
+-rw-r--r--   0        0        0      920 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/conftest.py
+-rw-r--r--   0        0        0      532 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/openai_example_script.py
+-rw-r--r--   0        0        0      822 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/test_init.py
+-rw-r--r--   0        0        0     1211 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     1679 2024-04-07 01:56:06.296040 reprompt-0.0.4rc27.post1/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    16700 1970-01-01 00:00:00.000000 reprompt-0.0.4rc27.post1/PKG-INFO
```

### Comparing `reprompt-0.0.4/.devcontainer/devcontainer.json` & `reprompt-0.0.4rc27.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.4rc27.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/.gitignore` & `reprompt-0.0.4rc27.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/.pre-commit-config.yaml` & `reprompt-0.0.4rc27.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/.vscode/settings.json` & `reprompt-0.0.4rc27.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/LICENSE` & `reprompt-0.0.4rc27.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/README.md` & `reprompt-0.0.4rc27.post1/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/docs/Makefile` & `reprompt-0.0.4rc27.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/docs/conf.py` & `reprompt-0.0.4rc27.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/docs/make.bat` & `reprompt-0.0.4rc27.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/docs/pylint.md` & `reprompt-0.0.4rc27.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/pyproject.toml` & `reprompt-0.0.4rc27.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/src/reprompt/__init__.py` & `reprompt-0.0.4rc27.post1/src/reprompt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #   -------------------------------------------------------------
 """Python Package Template"""
 from __future__ import annotations
 from typing import Callable
 
 from .tracing import FunctionTrace
 
-__version__ = "0.0.4"
+__version__ = "0.0.4-rc27-post1"
 
 import logging
 import functools
 import datetime
 import json
 
 # Configure logging
```

### Comparing `reprompt-0.0.4/src/reprompt/custom_httpx.py` & `reprompt-0.0.4rc27.post1/src/reprompt/custom_httpx.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/src/reprompt/tracing.py` & `reprompt-0.0.4rc27.post1/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/tests/conftest.py` & `reprompt-0.0.4rc27.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/tests/test_methods.py` & `reprompt-0.0.4rc27.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/tests/test_openai_trace.py` & `reprompt-0.0.4rc27.post1/tests/openai_example_script.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.4/PKG-INFO` & `reprompt-0.0.4rc27.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.4
+Version: 0.0.4rc27.post1
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
```

