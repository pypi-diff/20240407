# Comparing `tmp/wireup-0.7.1.tar.gz` & `tmp/wireup-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wireup-0.7.1.tar", max compression
+gzip compressed data, was "wireup-0.7.2.tar", max compression
```

## Comparing `wireup-0.7.1.tar` & `wireup-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     3347 2024-03-05 23:04:12.231334 wireup-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     3326 2024-03-05 22:46:09.837135 wireup-0.7.1/readme.md
--rw-r--r--   0        0        0      745 2024-03-05 22:22:58.471243 wireup-0.7.1/wireup/__init__.py
--rw-r--r--   0        0        0     2317 2024-02-15 23:34:59.902308 wireup-0.7.1/wireup/annotation/__init__.py
--rw-r--r--   0        0        0     3695 2024-01-31 21:18:57.389020 wireup-0.7.1/wireup/errors.py
--rw-r--r--   0        0        0     2961 2024-03-05 22:16:54.258450 wireup-0.7.1/wireup/import_util.py
--rw-r--r--   0        0        0        0 2024-01-16 23:17:49.853379 wireup-0.7.1/wireup/integration/__init__.py
--rw-r--r--   0        0        0     1537 2024-01-31 20:47:52.794068 wireup-0.7.1/wireup/integration/fastapi_integration.py
--rw-r--r--   0        0        0     1901 2024-01-31 20:47:52.798068 wireup-0.7.1/wireup/integration/flask_integration.py
--rw-r--r--   0        0        0      722 2024-01-31 20:47:52.798068 wireup-0.7.1/wireup/integration/util.py
--rw-r--r--   0        0        0        0 2023-09-14 21:08:33.059327 wireup-0.7.1/wireup/ioc/__init__.py
--rw-r--r--   0        0        0    15688 2024-01-31 21:40:40.390041 wireup-0.7.1/wireup/ioc/dependency_container.py
--rw-r--r--   0        0        0     2589 2023-11-29 20:56:37.410314 wireup-0.7.1/wireup/ioc/initialization_context.py
--rw-r--r--   0        0        0     2649 2024-01-31 20:47:52.798068 wireup-0.7.1/wireup/ioc/override_manager.py
--rw-r--r--   0        0        0     3740 2023-12-22 19:48:57.175332 wireup-0.7.1/wireup/ioc/parameter.py
--rw-r--r--   0        0        0     1884 2024-01-16 23:17:49.853379 wireup-0.7.1/wireup/ioc/proxy.py
--rw-r--r--   0        0        0     6727 2024-01-31 21:41:13.773781 wireup-0.7.1/wireup/ioc/service_registry.py
--rw-r--r--   0        0        0     3897 2024-01-31 21:40:43.930013 wireup-0.7.1/wireup/ioc/types.py
--rw-r--r--   0        0        0     1776 2024-01-31 20:47:52.798068 wireup-0.7.1/wireup/ioc/util.py
--rw-r--r--   0        0        0        0 2023-10-22 19:11:24.510952 wireup-0.7.1/wireup/py.typed
--rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 wireup-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3510 2024-04-07 19:43:59.695910 wireup-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     3327 2024-04-07 19:40:26.353780 wireup-0.7.2/readme.md
+-rw-r--r--   0        0        0      745 2024-04-06 10:38:15.863651 wireup-0.7.2/wireup/__init__.py
+-rw-r--r--   0        0        0     2720 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/annotation/__init__.py
+-rw-r--r--   0        0        0     4002 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/errors.py
+-rw-r--r--   0        0        0     2961 2024-03-29 14:28:28.443108 wireup-0.7.2/wireup/import_util.py
+-rw-r--r--   0        0        0        0 2024-03-29 14:24:37.869539 wireup-0.7.2/wireup/integration/__init__.py
+-rw-r--r--   0        0        0     1537 2024-04-02 21:36:05.205145 wireup-0.7.2/wireup/integration/fastapi_integration.py
+-rw-r--r--   0        0        0     1901 2024-03-29 14:24:37.869539 wireup-0.7.2/wireup/integration/flask_integration.py
+-rw-r--r--   0        0        0      722 2024-03-29 14:24:37.869539 wireup-0.7.2/wireup/integration/util.py
+-rw-r--r--   0        0        0        0 2023-09-14 21:08:33.059327 wireup-0.7.2/wireup/ioc/__init__.py
+-rw-r--r--   0        0        0    15862 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/ioc/dependency_container.py
+-rw-r--r--   0        0        0     2589 2024-03-29 14:24:37.873539 wireup-0.7.2/wireup/ioc/initialization_context.py
+-rw-r--r--   0        0        0     3049 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/ioc/override_manager.py
+-rw-r--r--   0        0        0     3740 2024-04-06 10:38:15.863651 wireup-0.7.2/wireup/ioc/parameter.py
+-rw-r--r--   0        0        0     1884 2024-03-29 14:24:37.873539 wireup-0.7.2/wireup/ioc/proxy.py
+-rw-r--r--   0        0        0     6746 2024-03-29 14:28:28.443108 wireup-0.7.2/wireup/ioc/service_registry.py
+-rw-r--r--   0        0        0     3897 2024-04-02 20:58:05.389534 wireup-0.7.2/wireup/ioc/types.py
+-rw-r--r--   0        0        0     1992 2024-04-07 19:40:26.361780 wireup-0.7.2/wireup/ioc/util.py
+-rw-r--r--   0        0        0        0 2023-10-22 19:11:24.510952 wireup-0.7.2/wireup/py.typed
+-rw-r--r--   0        0        0     4699 1970-01-01 00:00:00.000000 wireup-0.7.2/PKG-INFO
```

### Comparing `wireup-0.7.1/pyproject.toml` & `wireup-0.7.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wireup"
-version = "0.7.1"
+version = "0.7.2"
 description = "Python Dependency Injection Library"
 authors = ["Aldo Mateli <aldo.mateli@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/maldoinc/wireup"
 packages = [
     { include = "wireup" }
@@ -45,35 +45,33 @@
 Changelog = "https://github.com/maldoinc/wireup/releases"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 graphlib2 = {version="^0.4.7", python=">=3.8,<3.9"}
 
 [tool.poetry.group.dev.dependencies]
-ruff = "0.1.*"
+ruff = "0.3.4"
 setuptools = "^68.0.0"
 mkdocs = "^1.5.2"
 mkdocs-material = "^9.4.14"
 mkdocstrings-python = "^1.6.2"
 mkdocs-open-in-new-tab = "^1.0.2"
 mike = "^1.1.2"
 typing-extensions = "^4.7.1"
-mypy = "1.7.1"
-flask = "^3.0.0"
+mypy = "1.9.0"
 coverage = "^7.3.2"
-fastapi = "^0.105.0"
-httpx = "^0.26.0"
+tox = "^4.14.2"
 
 [tool.ruff]
 target-version = "py38"
 line-length = 120
 src = ["wireup"]
-fixable = ["ALL"]
-select = ["ALL"]
-ignore = [
+lint.fixable = ["ALL"]
+lint.select = ["ALL"]
+lint.ignore = [
     "ANN401", # Allow returning any. Parameter bag has to store/retrieve arbitraty types.
     "PT009", # Prefer using assertEqual instead of plain asserts
     "ANN101", # Exclude self from type hint requirement,
     "TD003", # Exclude "missing issue link for todos",
     "FIX002", # Disable "Line contains to do, consider resolving the issue". It will be done, in due time.
     "D100", # Disable undocumented public module. The definitions themselves will be documented
     "D104", # Same as above, disable missing docstring in public package,
@@ -82,14 +80,17 @@
     "D107", # Disable required docs for __init. Can be redundant if class also has them.
     "A003", # Disable "shadows builtin". OverrideManager.set was flagged by this
 
     # Disable as they may cause conflicts with ruff formatter
     "COM812",
     "ISC001"
 ]
+[tool.ruff.lint.per-file-ignores]
+"test/*" = ["D", "ANN", "PT", "SLF001", "T201", "EM101", "TRY", "FA100", "B008", "RUF009", "F401", "SIM117"]
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 # Taken from https://coverage.readthedocs.io/en/latest/excluding.html
 [tool.coverage.report]
@@ -102,7 +103,10 @@
     "raise NotImplementedError",
     "if 0:",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
     "class .*\\bProtocol\\):",
     "@(abc\\.)?abstractmethod",
     ]
+
+[tool.mypy]
+exclude = "wireup.integration"
```

### Comparing `wireup-0.7.1/readme.md` & `wireup-0.7.2/readme.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [![Coverage](https://img.shields.io/codeclimate/coverage/maldoinc/wireup?label=Coverage)](https://codeclimate.com/github/maldoinc/wireup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wireup)](https://pypi.org/project/wireup/)
 [![PyPI - Version](https://img.shields.io/pypi/v/wireup)](https://pypi.org/project/wireup/)
 </div>
 
 > [!TIP]
 >    Simplify Dependency injection for Flask using the new
-[Flask integration](https://maldoinc.github.io/wireup/latest/integrations/flask/)!
+[Flask integration](https://maldoinc.github.io/wireup/latest/integrations/flask)!
 >
 >    * Automatically inject dependencies without having to manually call autowire.
 >    * Expose flask application configuration in the container.
 
 ---
 
 ## ⚡ Key Features
@@ -24,15 +24,15 @@
 * Interfaces / Abstract classes
 * Multiple Containers 
 * Static factories
 * Singleton/Transient dependencies
 * Framework Agnostic
 * Simplified usage in 
 [Flask](https://maldoinc.github.io/wireup/latest/integrations/flask/) 
-and [FastApi](https://maldoinc.github.io/wireup/latest/integrations/flask/) using the first-party integrations.
+and [FastApi](https://maldoinc.github.io/wireup/latest/integrations/fastapi/) using the first-party integrations.
 
 ## 📋 Quickstart
 
 Example showing a Database service, a repository and a web view which uses the repository to fetch all posts 
 from a fictional blog db.
 
 **1. Register dependencies**
```

### Comparing `wireup-0.7.1/wireup/__init__.py` & `wireup-0.7.2/wireup/__init__.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/annotation/__init__.py` & `wireup-0.7.2/wireup/annotation/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,81 @@
 from __future__ import annotations
 
+import contextlib
 import importlib
 from enum import Enum
-from typing import Any
+from typing import TYPE_CHECKING
 
 from wireup.ioc.types import (
     ContainerProxyQualifier,
     ContainerProxyQualifierValue,
     EmptyContainerInjectionRequest,
+    InjectableType,
     ParameterWrapper,
     TemplatedString,
 )
 
+if TYPE_CHECKING:
+    from collections.abc import Callable
+
 
 def wire(
     *,
     param: str | None = None,
     expr: str | None = None,
     qualifier: ContainerProxyQualifierValue = None,
-) -> Any:
+) -> InjectableType | Callable[[], InjectableType]:
     """Inject resources from the container to autowired method arguments.
 
     Arguments are exclusive and only one of them must be used at any time.
     !!! note
         Methods MUST be still decorated with autowire for this to work.
 
     :param param: Inject a given parameter by name.
     :param expr: Inject a string value using a templated string.
     Parameters inside `${}` will be replaced with their corresponding value.
 
     :param qualifier: Qualify which implementation to bind when there are multiple components
     implementing an interface that is registered in the container via `@abstract`.
     """
-    if param:
-        return ParameterWrapper(param)
+    res: InjectableType
 
-    if expr:
-        return ParameterWrapper(TemplatedString(expr))
-
-    if qualifier:
-        return ContainerProxyQualifier(qualifier)
+    if param:
+        res = ParameterWrapper(param)
+    elif expr:
+        res = ParameterWrapper(TemplatedString(expr))
+    elif qualifier:
+        res = ContainerProxyQualifier(qualifier)
+    else:
+        res = EmptyContainerInjectionRequest()
+
+    # Fastapi needs all dependencies to be wrapped with Depends.
+    with contextlib.suppress(ModuleNotFoundError):
+
+        def _inner() -> InjectableType:
+            return res
+
+        # This will act as a flag so that wireup knows this dependency belongs to it.
+        _inner.__is_wireup_depends__ = True  # type: ignore[attr-defined]
+        return importlib.import_module("fastapi").Depends(_inner)  # type: ignore[no-any-return]
 
-    try:
-        # Allow fastapi users to do .get() without any params
-        # It is meant to be used as a default value in where Depends() is expected
-        return importlib.import_module("fastapi").Depends(EmptyContainerInjectionRequest)
-    except ModuleNotFoundError:
-        return EmptyContainerInjectionRequest()
+    return res
 
 
 class ParameterEnum(Enum):
     """Enum with a `.wire` method allowing easy injection of members.
 
     Allows you to add application parameters as enum members and their names as values.
     When you need to inject a parameter instead of referencing it by name you can
     annotate the parameter with the wire function call or set that as the default value.
 
     This will inject a parameter by name and won't work with expressions.
     """
 
-    def wire(self) -> Any:
+    def wire(self) -> InjectableType | Callable[[], InjectableType]:
         """Inject the parameter this enumeration member represents.
 
         Equivalent of `wire(param=EnumParam.enum_member.value)`
         """
         return wire(param=self.value)
```

### Comparing `wireup-0.7.1/wireup/errors.py` & `wireup-0.7.2/wireup/errors.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,7 +92,14 @@
 
 
 class InvalidRegistrationTypeError(WireupError):
     """Raised when attempting to call @container.register with an invalid argument."""
 
     def __init__(self, attempted: Any) -> None:
         super().__init__(f"Cannot register {attempted} with the container. Allowed types are callables and types")
+
+
+class UnknownOverrideRequestedError(WireupError):
+    """Raised when attempting to override a service which does not exist."""
+
+    def __init__(self, klass: type, qualifier: ContainerProxyQualifierValue) -> None:
+        super().__init__(f"Cannot override unknown {klass} with qualifier '{qualifier}'.")
```

### Comparing `wireup-0.7.1/wireup/import_util.py` & `wireup-0.7.2/wireup/import_util.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/integration/fastapi_integration.py` & `wireup-0.7.2/wireup/integration/fastapi_integration.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/integration/flask_integration.py` & `wireup-0.7.2/wireup/integration/flask_integration.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/integration/util.py` & `wireup-0.7.2/wireup/integration/util.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/ioc/dependency_container.py` & `wireup-0.7.2/wireup/ioc/dependency_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     ServiceLifetime,
 )
 
 if TYPE_CHECKING:
     from .initialization_context import InitializationContext
     from .parameter import ParameterBag
 
-
 __T = TypeVar("__T")
 __ObjectIdentifier = Tuple[type, ContainerProxyQualifierValue]
 
 
 class DependencyContainer:
     """Dependency Injection and Service Locator container registry.
 
@@ -69,15 +68,17 @@
         """:param parameter_bag: ParameterBag instance holding parameter information."""
         self.__service_registry: _ServiceRegistry = _ServiceRegistry()
         self.__initialized_objects: dict[__ObjectIdentifier, Any] = {}
         self.__active_overrides: dict[__ObjectIdentifier, Any] = {}
         self.__initialized_proxies: dict[__ObjectIdentifier, ContainerProxy[Any]] = {}
         self.__buildable_types: set[type] = set()
         self.__params: ParameterBag = parameter_bag
-        self.__override_manager: OverrideManager = OverrideManager(self.__active_overrides)
+        self.__override_manager: OverrideManager = OverrideManager(
+            self.__active_overrides, self.__service_registry.is_type_with_qualifier_known
+        )
 
     def get(self, klass: type[__T], qualifier: ContainerProxyQualifierValue = None) -> __T:
         """Get an instance of the requested type.
 
         Use this to locate services by their type but strongly prefer using injection instead.
 
         :param qualifier: Qualifier for the class if it was registered with one.
@@ -265,15 +266,18 @@
         if fn := self.__service_registry.factory_functions.get(obj_id):
             instance = fn(**self.__callable_get_params_to_inject(fn))
         else:
             args = self.__callable_get_params_to_inject(klass)
             instance = klass(**args)
 
         if self.__service_registry.is_impl_singleton(klass):
-            self.__initialized_objects[klass, qualifier] = instance
+            self.__initialized_objects[obj_id] = instance
+
+            if obj_id in self.__initialized_proxies:
+                del self.__initialized_proxies[obj_id]
 
         self.__buildable_types.add(klass)
         return instance
 
     def __initialize_container_proxy_object_from_parameter(self, annotated_parameter: AnnotatedParameter) -> Any:
         # Disable type checker here as the only caller ensures that klass is not none to avoid the call entirely.
         annotated_type: type = annotated_parameter.klass  # type: ignore[assignment]
```

### Comparing `wireup-0.7.1/wireup/ioc/initialization_context.py` & `wireup-0.7.2/wireup/ioc/initialization_context.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/ioc/override_manager.py` & `wireup-0.7.2/wireup/ioc/override_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 from __future__ import annotations
 
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, Iterator
 
+from wireup.errors import UnknownOverrideRequestedError
+
 if TYPE_CHECKING:
+    from collections.abc import Callable
+
     from wireup.ioc.types import ContainerProxyQualifierValue, ServiceOverride
 
 
 class OverrideManager:
     """Enables overriding of services registered with the container."""
 
-    def __init__(self, active_overrides: dict[tuple[type, ContainerProxyQualifierValue], Any]) -> None:
+    def __init__(
+        self,
+        active_overrides: dict[tuple[type, ContainerProxyQualifierValue], Any],
+        is_valid_override: Callable[[type, ContainerProxyQualifierValue], bool],
+    ) -> None:
+        self.__is_valid_override = is_valid_override
         self.__active_overrides = active_overrides
 
     def set(self, target: type, new: Any, qualifier: ContainerProxyQualifierValue = None) -> None:
         """Override the `target` service with `new`.
 
         Subsequent autowire calls to `target` will result in `new` being injected.
 
         :param target: The target service to override.
         :param qualifier: The qualifier of the service to override. Set this if service is registered
         with the qualifier parameter set to a value.
         :param new: The new object to be injected instead of `target`.
         """
+        if not self.__is_valid_override(target, qualifier):
+            raise UnknownOverrideRequestedError(klass=target, qualifier=qualifier)
+
         self.__active_overrides[target, qualifier] = new
 
     def delete(self, target: type, qualifier: ContainerProxyQualifierValue = None) -> None:
         """Clear active override for the `target` service."""
         if (target, qualifier) in self.__active_overrides:
             del self.__active_overrides[target, qualifier]
```

### Comparing `wireup-0.7.1/wireup/ioc/parameter.py` & `wireup-0.7.2/wireup/ioc/parameter.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/ioc/proxy.py` & `wireup-0.7.2/wireup/ioc/proxy.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/ioc/service_registry.py` & `wireup-0.7.2/wireup/ioc/service_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         klass: type,
         qualifier: ContainerProxyQualifierValue,
         lifetime: ServiceLifetime,
     ) -> None:
         if self.is_type_with_qualifier_known(klass, qualifier):
             raise DuplicateServiceRegistrationError(klass, qualifier)
 
-        if self.is_interface_known(klass.__base__):
+        if klass.__base__ and self.is_interface_known(klass.__base__):
             if qualifier in self.known_interfaces[klass.__base__]:
                 raise DuplicateQualifierForInterfaceError(klass, qualifier)
 
             self.known_interfaces[klass.__base__][qualifier] = klass
 
         self.known_impls[klass].add(qualifier)
         self.target_init_context(klass, lifetime)
```

### Comparing `wireup-0.7.1/wireup/ioc/types.py` & `wireup-0.7.2/wireup/ioc/types.py`

 * *Files identical despite different names*

### Comparing `wireup-0.7.1/wireup/ioc/util.py` & `wireup-0.7.2/wireup/ioc/util.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from __future__ import annotations
 
 import typing
 from inspect import Parameter
 from typing import Any
 
-from wireup.ioc.types import AnnotatedParameter, EmptyContainerInjectionRequest, InjectableType
+from wireup.ioc.types import AnnotatedParameter, InjectableType
 
 
 def parameter_get_type_and_annotation(parameter: Parameter) -> AnnotatedParameter:
     """Get the annotation injection type from a signature's Parameter.
 
     Returns either the first annotation for an Annotated type or the default value.
     """
 
-    def map_to_injectable_type(metadata: Any) -> InjectableType | None:
-        if isinstance(metadata, InjectableType):
-            return metadata
-
-        if (
-            str(metadata.__class__) == "<class 'fastapi.params.Depends'>"
-            and metadata.dependency == EmptyContainerInjectionRequest
-        ):
-            return EmptyContainerInjectionRequest()
+    def get_injectable_type(metadata: Any) -> InjectableType | None:
+        # When using fastapi, the injectable type will be wrapped with Depends.
+        # As such, it needs to be unwrapped in order to get the actual metadata
+        # Need to be careful here not to unwrap FastAPI dependencies
+        # not owned by wireup as they might cause side effects.
+        if hasattr(metadata, "dependency") and hasattr(metadata.dependency, "__is_wireup_depends__"):
+            metadata = metadata.dependency()
 
-        return None
+        return metadata if isinstance(metadata, InjectableType) else None
 
     if hasattr(parameter.annotation, "__metadata__") and hasattr(parameter.annotation, "__args__"):
         klass = parameter.annotation.__args__[0]
-        annotation = next(
-            (map_to_injectable_type(ann) for ann in parameter.annotation.__metadata__ if map_to_injectable_type(ann)),
-            None,
-        )
+        annotation = None
+
+        for ann in parameter.annotation.__metadata__:
+            if injectable_type := get_injectable_type(ann):
+                annotation = injectable_type
+                break
     else:
         klass = None if parameter.annotation is Parameter.empty else parameter.annotation
-        annotation = None if parameter.default is Parameter.empty else parameter.default
+        annotation = None if parameter.default is Parameter.empty else get_injectable_type(parameter.default)
 
     return AnnotatedParameter(klass=klass, annotation=annotation)
 
 
 def is_type_autowireable(obj_type: Any) -> bool:
     """Determine if the given type is can be autowired without additional annotations."""
     if obj_type is None or obj_type in {int, float, str, bool, complex, bytes, bytearray, memoryview}:
```

### Comparing `wireup-0.7.1/PKG-INFO` & `wireup-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wireup
-Version: 0.7.1
+Version: 0.7.2
 Summary: Python Dependency Injection Library
 Home-page: https://github.com/maldoinc/wireup
 License: MIT
 Keywords: flask,django,injector,dependency injection,dependency injection container,dependency injector
 Author: Aldo Mateli
 Author-email: aldo.mateli@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -41,15 +41,15 @@
 [![Coverage](https://img.shields.io/codeclimate/coverage/maldoinc/wireup?label=Coverage)](https://codeclimate.com/github/maldoinc/wireup)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/wireup)](https://pypi.org/project/wireup/)
 [![PyPI - Version](https://img.shields.io/pypi/v/wireup)](https://pypi.org/project/wireup/)
 </div>
 
 > [!TIP]
 >    Simplify Dependency injection for Flask using the new
-[Flask integration](https://maldoinc.github.io/wireup/latest/integrations/flask/)!
+[Flask integration](https://maldoinc.github.io/wireup/latest/integrations/flask)!
 >
 >    * Automatically inject dependencies without having to manually call autowire.
 >    * Expose flask application configuration in the container.
 
 ---
 
 ## ⚡ Key Features
@@ -57,15 +57,15 @@
 * Interfaces / Abstract classes
 * Multiple Containers 
 * Static factories
 * Singleton/Transient dependencies
 * Framework Agnostic
 * Simplified usage in 
 [Flask](https://maldoinc.github.io/wireup/latest/integrations/flask/) 
-and [FastApi](https://maldoinc.github.io/wireup/latest/integrations/flask/) using the first-party integrations.
+and [FastApi](https://maldoinc.github.io/wireup/latest/integrations/fastapi/) using the first-party integrations.
 
 ## 📋 Quickstart
 
 Example showing a Database service, a repository and a web view which uses the repository to fetch all posts 
 from a fictional blog db.
 
 **1. Register dependencies**
```

