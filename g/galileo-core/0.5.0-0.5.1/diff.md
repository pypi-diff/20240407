# Comparing `tmp/galileo_core-0.5.0.tar.gz` & `tmp/galileo_core-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_core-0.5.0.tar", max compression
+gzip compressed data, was "galileo_core-0.5.1.tar", max compression
```

## Comparing `galileo_core-0.5.0.tar` & `galileo_core-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    10946 2024-04-06 08:40:11.609614 galileo_core-0.5.0/LICENSE
--rw-r--r--   0        0        0       80 2024-04-06 08:40:11.609614 galileo_core-0.5.0/README.md
--rw-r--r--   0        0        0     2323 2024-04-06 08:40:12.645613 galileo_core-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-06 08:40:12.645613 galileo_core-0.5.0/src/galileo_core/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/constants/__init__.py
--rw-r--r--   0        0        0      573 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/constants/http_headers.py
--rw-r--r--   0        0        0      362 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/constants/routes.py
--rw-r--r--   0        0        0        0 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/helpers/__init__.py
--rw-r--r--   0        0        0     1543 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/helpers/api_client.py
--rw-r--r--   0        0        0     5322 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/helpers/config.py
--rw-r--r--   0        0        0       60 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/helpers/logger.py
--rw-r--r--   0        0        0        0 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/__init__.py
--rw-r--r--   0        0        0     1382 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/action.py
--rw-r--r--   0        0        0      488 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/metric.py
--rw-r--r--   0        0        0      902 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/payload.py
--rw-r--r--   0        0        0     2096 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/request.py
--rw-r--r--   0        0        0     1934 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/rule.py
--rw-r--r--   0        0        0     1375 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/ruleset.py
--rw-r--r--   0        0        0     1124 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/protect/stage.py
--rw-r--r--   0        0        0        0 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/shared/__init__.py
--rw-r--r--   0        0        0      149 2024-04-06 08:40:11.609614 galileo_core-0.5.0/src/galileo_core/schemas/shared/metric.py
--rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    10946 2024-04-06 22:17:52.353323 galileo_core-0.5.1/LICENSE
+-rw-r--r--   0        0        0       80 2024-04-06 22:17:52.353323 galileo_core-0.5.1/README.md
+-rw-r--r--   0        0        0     2323 2024-04-06 22:17:53.241325 galileo_core-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-06 22:17:53.241325 galileo_core-0.5.1/src/galileo_core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:17:52.353323 galileo_core-0.5.1/src/galileo_core/constants/__init__.py
+-rw-r--r--   0        0        0      573 2024-04-06 22:17:52.353323 galileo_core-0.5.1/src/galileo_core/constants/http_headers.py
+-rw-r--r--   0        0        0      362 2024-04-06 22:17:52.353323 galileo_core-0.5.1/src/galileo_core/constants/routes.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/helpers/__init__.py
+-rw-r--r--   0        0        0     1543 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/helpers/api_client.py
+-rw-r--r--   0        0        0     5322 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/helpers/config.py
+-rw-r--r--   0        0        0       60 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/helpers/logger.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/__init__.py
+-rw-r--r--   0        0        0     1382 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/action.py
+-rw-r--r--   0        0        0      488 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/metric.py
+-rw-r--r--   0        0        0      902 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/payload.py
+-rw-r--r--   0        0        0     2096 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/request.py
+-rw-r--r--   0        0        0     1934 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/rule.py
+-rw-r--r--   0        0        0      831 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/ruleset.py
+-rw-r--r--   0        0        0     1124 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/protect/stage.py
+-rw-r--r--   0        0        0        0 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/shared/__init__.py
+-rw-r--r--   0        0        0      149 2024-04-06 22:17:52.357323 galileo_core-0.5.1/src/galileo_core/schemas/shared/metric.py
+-rw-r--r--   0        0        0      771 1970-01-01 00:00:00.000000 galileo_core-0.5.1/PKG-INFO
```

### Comparing `galileo_core-0.5.0/LICENSE` & `galileo_core-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/pyproject.toml` & `galileo_core-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-core"
-version = "0.5.0"
+version = "0.5.1"
 description = "Shared schemas and configuration for Galileo's Python packages."
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 packages = [{include = "galileo_core", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1,<3.13"
```

### Comparing `galileo_core-0.5.0/src/galileo_core/constants/http_headers.py` & `galileo_core-0.5.1/src/galileo_core/constants/http_headers.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/src/galileo_core/helpers/api_client.py` & `galileo_core-0.5.1/src/galileo_core/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/src/galileo_core/helpers/config.py` & `galileo_core-0.5.1/src/galileo_core/helpers/config.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/src/galileo_core/schemas/protect/action.py` & `galileo_core-0.5.1/src/galileo_core/schemas/protect/action.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/src/galileo_core/schemas/protect/payload.py` & `galileo_core-0.5.1/src/galileo_core/schemas/protect/payload.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/src/galileo_core/schemas/protect/request.py` & `galileo_core-0.5.1/src/galileo_core/schemas/protect/request.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/src/galileo_core/schemas/protect/rule.py` & `galileo_core-0.5.1/src/galileo_core/schemas/protect/rule.py`

 * *Files identical despite different names*

### Comparing `galileo_core-0.5.0/src/galileo_core/schemas/protect/ruleset.py` & `galileo_core-0.5.1/src/galileo_core/schemas/protect/stage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,25 @@
-from functools import cached_property
-from typing import Optional, Sequence
+from typing import Optional
 
-from pydantic import BaseModel, Field, computed_field, field_validator
+from pydantic import UUID4, BaseModel, Field, ValidationInfo, field_validator
 
-from galileo_core.schemas.protect.action import Action, BaseAction, PassthroughAction
-from galileo_core.schemas.protect.rule import Rule
+from galileo_core.schemas.protect.action import Action
 
 
-class Ruleset(BaseModel):
-    rules: Sequence[Rule] = Field(
-        description="List of rules to evaluate. Atleast 1 rule is required.", default_factory=list, min_length=1
+class Stage(BaseModel):
+    name: str = Field(description="Name of the stage. Must be unique within the project.")
+    project_id: UUID4 = Field(description="ID of the project to which this stage belongs.")
+    description: Optional[str] = Field(
+        description="Optional human-readable description of the goals of this guardrail.", default=None
     )
-    action: Action = Field(description="Action to take if all the rules are met.", default_factory=PassthroughAction)
-    description: Optional[str] = Field(description="Description of the ruleset.", default=None)
-    timeout: Optional[float] = Field(
-        description="Time in seconds for all the rules to be evaluated. If not provided, will evaluate all the rules to completion or the timeout of the request.",
-        default=None,
+    action: Optional[Action] = Field(
+        description="An optional action (kill switch) to take that supersedes all ruleset validations.", default=None
+    )
+    action_enabled: bool = Field(
+        description="Whether the action is enabled. If False, the action will not be applied.", default=False
     )
 
-    # https://github.com/python/mypy/issues/1362
-    @computed_field  # type: ignore[misc]
-    @cached_property
-    def timeout_ns(self) -> Optional[float]:
-        if isinstance(self.timeout, float):
-            return self.timeout * 1e9
-        return None
-
-    @field_validator("action", mode="before")
-    def validate_action(cls, value: Optional[BaseAction]) -> BaseAction:
-        if not value:
-            value = PassthroughAction()
+    @field_validator("action_enabled", mode="before")
+    def validate_action_enabled(cls, value: bool, info: ValidationInfo) -> bool:
+        if value and info.data.get("action") is None:
+            raise ValueError("Action cannot be enabled if action is not set.")
         return value
```

### Comparing `galileo_core-0.5.0/PKG-INFO` & `galileo_core-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galileo-core
-Version: 0.5.0
+Version: 0.5.1
 Summary: Shared schemas and configuration for Galileo's Python packages.
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.8.1,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

