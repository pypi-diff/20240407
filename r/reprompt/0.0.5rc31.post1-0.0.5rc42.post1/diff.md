# Comparing `tmp/reprompt-0.0.5rc31.post1.tar.gz` & `tmp/reprompt-0.0.5rc42.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reprompt-0.0.5rc31.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "reprompt-0.0.5rc42.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `reprompt-0.0.5rc31.post1.tar` & `reprompt-0.0.5rc42.post1.tar`

### file list

```diff
@@ -1,42 +1,41 @@
--rw-r--r--   0        0        0      334 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1157 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      417 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      418 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/template-sync.yml
--rw-r--r--   0        0        0      472 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      675 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/schedule-update-actions.yml
--rw-r--r--   0        0        0      318 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      368 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/sphinx.yml
--rw-r--r--   0        0        0      307 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.github/workflows/template-sync.yml
--rw-r--r--   0        0        0     1799 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.gitignore
--rw-r--r--   0        0        0     1540 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.pypirc
--rw-r--r--   0        0        0      459 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.vscode/launch.json
--rw-r--r--   0        0        0      817 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1141 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/LICENSE
--rw-r--r--   0        0        0    15834 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/README.md
--rw-r--r--   0        0        0      634 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/Makefile
--rw-r--r--   0        0        0     2321 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/conf.py
--rw-r--r--   0        0        0      360 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/devcontainer.md
--rw-r--r--   0        0        0       47 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/developer.md
--rw-r--r--   0        0        0      468 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/index.rst
--rw-r--r--   0        0        0      800 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/make.bat
--rw-r--r--   0        0        0       51 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/modules.rst
--rw-r--r--   0        0        0      471 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/pyproject.md
--rw-r--r--   0        0        0      425 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/python_package.hello_world.rst
--rw-r--r--   0        0        0      415 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/python_package.rst
--rw-r--r--   0        0        0       42 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/requirements.txt
--rw-r--r--   0        0        0       44 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/vscode.md
--rw-r--r--   0        0        0      208 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/docs/workflows.md
--rw-r--r--   0        0        0     6566 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/pyproject.toml
--rw-r--r--   0        0        0       42 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/src/README.md
--rw-r--r--   0        0        0     2246 2024-04-07 02:04:34.400733 reprompt-0.0.5rc31.post1/src/reprompt/__init__.py
--rw-r--r--   0        0        0     3103 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/src/reprompt/custom_httpx.py
--rw-r--r--   0        0        0      920 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/src/reprompt/tracing.py
--rw-r--r--   0        0        0      989 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/conftest.py
--rw-r--r--   0        0        0      532 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/openai_example_script.py
--rw-r--r--   0        0        0      822 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/test_init.py
--rw-r--r--   0        0        0     1679 2024-04-07 02:04:21.024590 reprompt-0.0.5rc31.post1/tests/test_openai_tracing.py
--rw-r--r--   0        0        0    17594 1970-01-01 00:00:00.000000 reprompt-0.0.5rc31.post1/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-04-07 03:06:13.250523 reprompt-0.0.5rc42.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1157 2024-04-07 03:06:13.250523 reprompt-0.0.5rc42.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      417 2024-04-07 03:06:13.250523 reprompt-0.0.5rc42.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      418 2024-04-07 03:06:13.250523 reprompt-0.0.5rc42.post1/.github/template-sync.yml
+-rw-r--r--   0        0        0      472 2024-04-07 03:06:13.250523 reprompt-0.0.5rc42.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      263 2024-04-07 03:06:13.250523 reprompt-0.0.5rc42.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      675 2024-04-07 03:06:13.250523 reprompt-0.0.5rc42.post1/.github/workflows/schedule-update-actions.yml
+-rw-r--r--   0        0        0      368 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/.github/workflows/sphinx.yml
+-rw-r--r--   0        0        0      307 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/.github/workflows/template-sync.yml
+-rw-r--r--   0        0        0     1799 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/.pypirc
+-rw-r--r--   0        0        0      459 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/.vscode/launch.json
+-rw-r--r--   0        0        0      817 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1127 2024-04-07 03:06:13.254523 reprompt-0.0.5rc42.post1/LICENSE
+-rw-r--r--   0        0        0    15834 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/README.md
+-rw-r--r--   0        0        0      634 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/Makefile
+-rw-r--r--   0        0        0     2321 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/conf.py
+-rw-r--r--   0        0        0      360 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/devcontainer.md
+-rw-r--r--   0        0        0       47 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/developer.md
+-rw-r--r--   0        0        0      468 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/index.rst
+-rw-r--r--   0        0        0      800 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/make.bat
+-rw-r--r--   0        0        0       51 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/modules.rst
+-rw-r--r--   0        0        0      471 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      425 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/python_package.hello_world.rst
+-rw-r--r--   0        0        0      415 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/python_package.rst
+-rw-r--r--   0        0        0       42 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/requirements.txt
+-rw-r--r--   0        0        0       44 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/vscode.md
+-rw-r--r--   0        0        0      208 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6627 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/pyproject.toml
+-rw-r--r--   0        0        0       42 2024-04-07 03:06:13.258523 reprompt-0.0.5rc42.post1/src/README.md
+-rw-r--r--   0        0        0     2059 2024-04-07 03:06:28.430590 reprompt-0.0.5rc42.post1/src/reprompt/__init__.py
+-rw-r--r--   0        0        0     3288 2024-04-07 03:06:13.262523 reprompt-0.0.5rc42.post1/src/reprompt/custom_httpx.py
+-rw-r--r--   0        0        0      920 2024-04-07 03:06:13.262523 reprompt-0.0.5rc42.post1/src/reprompt/tracing.py
+-rw-r--r--   0        0        0      989 2024-04-07 03:06:13.262523 reprompt-0.0.5rc42.post1/tests/conftest.py
+-rw-r--r--   0        0        0      511 2024-04-07 03:06:13.262523 reprompt-0.0.5rc42.post1/tests/openai_example_script.py
+-rw-r--r--   0        0        0      822 2024-04-07 03:06:13.262523 reprompt-0.0.5rc42.post1/tests/test_init.py
+-rw-r--r--   0        0        0     1692 2024-04-07 03:06:13.262523 reprompt-0.0.5rc42.post1/tests/test_openai_tracing.py
+-rw-r--r--   0        0        0    17715 1970-01-01 00:00:00.000000 reprompt-0.0.5rc42.post1/PKG-INFO
```

### Comparing `reprompt-0.0.5rc31.post1/.devcontainer/devcontainer.json` & `reprompt-0.0.5rc42.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/.github/workflows/schedule-update-actions.yml` & `reprompt-0.0.5rc42.post1/.github/workflows/schedule-update-actions.yml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/.gitignore` & `reprompt-0.0.5rc42.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/.pre-commit-config.yaml` & `reprompt-0.0.5rc42.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/.vscode/settings.json` & `reprompt-0.0.5rc42.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/README.md` & `reprompt-0.0.5rc42.post1/README.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/docs/Makefile` & `reprompt-0.0.5rc42.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/docs/conf.py` & `reprompt-0.0.5rc42.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/docs/make.bat` & `reprompt-0.0.5rc42.post1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/docs/pylint.md` & `reprompt-0.0.5rc42.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/pyproject.toml` & `reprompt-0.0.5rc42.post1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,21 +17,24 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 requires-python = ">=3.8.1"
 dynamic = ["version"]
 dependencies= [
+    "httpx==0.27.0",
     "wrapt>=1.12.1"
 ]
 [project.optional-dependencies]
 spark = [
     "pyspark>=3.0.0"
 ]
 test = [
+    "httpx>=0.21.0",
+    "openai>=0.10.0",
     "bandit[toml]==1.7.5",
     "black==23.3.0",
     "check-manifest==0.49",
     "flake8-bugbear==23.5.9",
     "flake8-docstrings",
     "flake8-formatter_junit_xml",
     "flake8",
@@ -44,17 +47,17 @@
     "pytest-runner",
     "pytest==7.3.1",
     "pytest-github-actions-annotate-failures",
     "shellcheck-py==0.9.0.2"
 ]
 
 [project.urls]
-Documentation = "https://github.com/syncup-ai/reprompt/tree/main#readme"
-Source = "https://github.com/syncup-ai/reprompt"
-Tracker = "https://github.com/syncup-ai/reprompt/issues"
+Documentation = "https://github.com/reprompt/reprompt/tree/main#readme"
+Source = "https://github.com/reprompt/reprompt"
+Tracker = "https://github.com/reprompt/reprompt/issues"
 
 [tool.flit.module]
 name = "reprompt"
 
 [tool.bandit]
 exclude_dirs = ["build","dist","tests","scripts"]
 number = 4
```

### Comparing `reprompt-0.0.5rc31.post1/src/reprompt/__init__.py` & `reprompt-0.0.5rc42.post1/src/reprompt/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-#   -------------------------------------------------------------
-#   Copyright (c) Microsoft Corporation. All rights reserved.
-#   Licensed under the MIT License. See LICENSE in project root for information.
-#   -------------------------------------------------------------
-"""Python Package Template"""
-from __future__ import annotations
-from typing import Callable
+"""Reprompt"""
 
-from .tracing import FunctionTrace
-
-__version__ = "0.0.5""-rc31-post1"
+from __future__ import annotations
 
-import logging
-import functools
 import datetime
+import functools
 import json
+import logging
+from typing import Callable
+
+from .custom_httpx import setup_monkey_patch
+from .tracing import FunctionTrace
 
-# Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
+# IMPORTANT: setting version for Reprompt package
+__version__ = "0.0.5""-rc42-post1"
+__all__ = ["FunctionTrace", "with_tracing", "start_trace", "TraceLogger"]
+
 
 class TraceLogger:
     @staticmethod
     def log_request(func: Callable, *args, **kwargs):
         """
         Log the request made to the OpenAI API.
         """
@@ -54,17 +53,14 @@
         result = func(*args, **kwargs)
         TraceLogger.log_response(result)
         return result
 
     return wrapper
 
 
-from .custom_httpx import setup_monkey_patch
-
-
 def start_trace(API_KEY=None):
     """
     Sets up monkey patching to intercept and log all HTTPX calls.
     """
     try:
         # Apply the monkey patch
         setup_monkey_patch()
```

### Comparing `reprompt-0.0.5rc31.post1/src/reprompt/custom_httpx.py` & `reprompt-0.0.5rc42.post1/src/reprompt/custom_httpx.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
-from datetime import datetime
-import httpx
-import logging
-import json
+"""Module providing a function printing python version."""
+
+from __future__ import annotations
+
 import asyncio
+import logging
 import os
 import uuid
+from datetime import datetime
+
+import httpx
 
 from reprompt.tracing import FunctionTrace
 
 # Configure logging
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
@@ -70,14 +74,17 @@
     if loop.is_running():
         asyncio.create_task(upload_trace_data(trace.get_trace_info()))
     else:
         asyncio.run(upload_trace_data(trace.get_trace_info()))
 
 
 def custom_send(self, request, *args, **kwargs):
+    """
+    Custom send method to intercept requests to api.openai.com.
+    """
     # Check if the request is for api.openai.com
     if "api.openai.com" in request.url.host:
         # Call the original send method
         response = _original_send(self, request, *args, **kwargs)
 
         # Log the request and response details
         openai_trace_request_response(request, response)
@@ -85,9 +92,11 @@
         # If not targeting api.openai.com, call the original send method without logging
         response = _original_send(self, request, *args, **kwargs)
 
     return response
 
 
 def setup_monkey_patch():
-    # Replace the send method with the custom one
+    """
+    Replace the httpx send method with the custom one
+    """
     httpx.Client.send = custom_send
```

### Comparing `reprompt-0.0.5rc31.post1/src/reprompt/tracing.py` & `reprompt-0.0.5rc42.post1/src/reprompt/tracing.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/tests/conftest.py` & `reprompt-0.0.5rc42.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/tests/test_init.py` & `reprompt-0.0.5rc42.post1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `reprompt-0.0.5rc31.post1/tests/test_openai_tracing.py` & `reprompt-0.0.5rc42.post1/tests/test_openai_tracing.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from __future__ import annotations
+
+import json
+from unittest.mock import patch
+
 import pytest
-from unittest.mock import patch, MagicMock
+from openai import OpenAI
+
 from reprompt import start_trace
 from reprompt.custom_httpx import openai_trace_request_response
-from openai import OpenAI
-import json
 
 
 @pytest.fixture
 def mock_openai_response():
     """Mock OpenAI API response."""
     return {"choices": [{"text": "Test response"}]}
 
@@ -18,16 +22,15 @@
     with patch("reprompt.custom_httpx.openai_trace_request_response") as mock:
         yield mock
 
 
 def openai_call():
     start_trace("test")
 
-    client = OpenAI()
-    OpenAI.api_key = "test"
+    client = OpenAI(api_key="test")
 
     completion = client.completions.create(
         model="gpt-3.5-turbo-instruct", prompt="Say this is a test", max_tokens=7, temperature=0
     )
 
 
 def test_openai_api_call_traced_correctly(mock_openai_response, mock_trace_function):
```

### Comparing `reprompt-0.0.5rc31.post1/PKG-INFO` & `reprompt-0.0.5rc42.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: reprompt
-Version: 0.0.5rc31.post1
+Version: 0.0.5rc42.post1
 Summary: Reprompt
 Author-email: Lukas Martinelli <me@lukasmartinelli.ch>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx==0.27.0
 Requires-Dist: wrapt>=1.12.1
 Requires-Dist: pyspark>=3.0.0 ; extra == "spark"
+Requires-Dist: httpx>=0.21.0 ; extra == "test"
+Requires-Dist: openai>=0.10.0 ; extra == "test"
 Requires-Dist: bandit[toml]==1.7.5 ; extra == "test"
 Requires-Dist: black==23.3.0 ; extra == "test"
 Requires-Dist: check-manifest==0.49 ; extra == "test"
 Requires-Dist: flake8-bugbear==23.5.9 ; extra == "test"
 Requires-Dist: flake8-docstrings ; extra == "test"
 Requires-Dist: flake8-formatter_junit_xml ; extra == "test"
 Requires-Dist: flake8 ; extra == "test"
@@ -27,17 +30,17 @@
 Requires-Dist: pylint_junit ; extra == "test"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
 Requires-Dist: pytest-mock<3.10.1 ; extra == "test"
 Requires-Dist: pytest-runner ; extra == "test"
 Requires-Dist: pytest==7.3.1 ; extra == "test"
 Requires-Dist: pytest-github-actions-annotate-failures ; extra == "test"
 Requires-Dist: shellcheck-py==0.9.0.2 ; extra == "test"
-Project-URL: Documentation, https://github.com/syncup-ai/reprompt/tree/main#readme
-Project-URL: Source, https://github.com/syncup-ai/reprompt
-Project-URL: Tracker, https://github.com/syncup-ai/reprompt/issues
+Project-URL: Documentation, https://github.com/reprompt/reprompt/tree/main#readme
+Project-URL: Source, https://github.com/reprompt/reprompt
+Project-URL: Tracker, https://github.com/reprompt/reprompt/issues
 Provides-Extra: spark
 Provides-Extra: test
 
 # Instructions
 
 
 Once you have a venv
```

