# Comparing `tmp/imy-0.1.9.tar.gz` & `tmp/imy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imy-0.1.9.tar", max compression
+gzip compressed data, was "imy-0.2.0.tar", max compression
```

## Comparing `imy-0.1.9.tar` & `imy-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.1.9/LICENSE
--rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.1.9/README.md
--rw-r--r--   0        0        0     6739 2024-02-18 14:15:52.272165 imy-0.1.9/imy/asset_manager.py
--rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.1.9/imy/async_utils.py
--rw-r--r--   0        0        0    15342 2024-03-27 21:23:27.056230 imy-0.1.9/imy/docstrings.py
--rw-r--r--   0        0        0     6281 2024-03-28 02:52:23.623106 imy-0.1.9/imy/inject.py
--rw-r--r--   0        0        0    12808 2024-03-31 10:54:05.192818 imy-0.1.9/imy/logs.py
--rw-r--r--   0        0        0     1974 2024-02-18 18:42:25.740924 imy-0.1.9/imy/package_metadata.py
--rw-r--r--   0        0        0     9744 2024-03-26 06:26:48.132598 imy-0.1.9/imy/settings.py
--rw-r--r--   0        0        0      754 2024-03-31 10:52:30.576108 imy-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-03-07 06:41:37.092412 imy-0.2.0/LICENSE
+-rw-r--r--   0        0        0      202 2024-02-09 18:31:32.595945 imy-0.2.0/README.md
+-rw-r--r--   0        0        0     6715 2024-04-07 17:04:35.179837 imy-0.2.0/imy/assets.py
+-rw-r--r--   0        0        0     6011 2024-03-27 19:30:58.658694 imy-0.2.0/imy/async_utils.py
+-rw-r--r--   0        0        0     9815 2024-04-01 09:46:55.130648 imy-0.2.0/imy/config.py
+-rw-r--r--   0        0        0       66 2024-04-07 17:07:49.466586 imy-0.2.0/imy/docstrings/__init__.py
+-rw-r--r--   0        0        0     1726 2024-04-01 10:37:37.589305 imy-0.2.0/imy/docstrings/models.py
+-rw-r--r--   0        0        0    14281 2024-04-01 10:37:37.592638 imy-0.2.0/imy/docstrings/parsers.py
+-rw-r--r--   0        0        0     8342 2024-04-07 17:07:13.593234 imy-0.2.0/imy/inject.py
+-rw-r--r--   0        0        0    12893 2024-03-31 11:34:08.656709 imy-0.2.0/imy/logs.py
+-rw-r--r--   0        0        0     1974 2024-02-18 18:42:25.740924 imy-0.2.0/imy/package_metadata.py
+-rw-r--r--   0        0        0      754 2024-04-07 14:57:22.242956 imy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 imy-0.2.0/PKG-INFO
```

### Comparing `imy-0.1.9/LICENSE` & `imy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imy-0.1.9/imy/asset_manager.py` & `imy-0.2.0/imy/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import logging
-import os
-import string
 import tarfile
 from pathlib import Path
 from typing import *  # type: ignore
 
 
 class AssetError(Exception):
     """
@@ -13,15 +11,15 @@
 
     pass
 
 
 class AssetManager:
     """
     Provides easy access to the project's assets. Assets are individually
-    `.tar.xz` compressed and live in the `xx_dir` directory. This class allows
+    `.tar.xz` compressed and live in the `xz_dir` directory. This class allows
     accessing them via relative paths. Whenever an asset is needed it is
     extracted first, unless it already exists in the cache.
 
     The asset manager is versioned, to ensure that assets of different library
     versions don't clash. Future versions may use this to delete old, unused
     assets but this is not implemented yet.
     """
```

### Comparing `imy-0.1.9/imy/async_utils.py` & `imy-0.2.0/imy/async_utils.py`

 * *Files identical despite different names*

### Comparing `imy-0.1.9/imy/docstrings.py` & `imy-0.2.0/imy/docstrings/parsers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,81 +1,23 @@
 from __future__ import annotations
 
 import collections
 import dataclasses
 import inspect
 import textwrap
 import typing
+import warnings
 from dataclasses import is_dataclass
 from typing import *  # type: ignore
 
+import introspection
 import introspection.typing
 from uniserde import Jsonable
-from dataclasses import dataclass
 
-
-__all__ = [
-    "parse_docstring",
-    "parse_function",
-    "parse_class",
-]
-
-
-@dataclass
-class FunctionParameter:
-    name: str
-    type: str | None
-    default: str | None
-
-    kw_only: bool
-
-    collect_positional: bool
-    collect_keyword: bool
-
-    description: str | None
-
-
-@dataclass
-class FunctionDocs:
-    name: str
-    parameters: list[FunctionParameter]
-    return_type: str | None
-    synchronous: bool
-
-    summary: str | None
-    details: str | None
-
-    raises: list[tuple[str, str]]  # type, description
-
-    @classmethod
-    def parse(cls, func: Callable) -> "FunctionDocs":
-        return parse_function(func)
-
-
-@dataclass
-class ClassField:
-    name: str
-    type: str
-    default: str | None
-
-    description: str | None
-
-
-@dataclass
-class ClassDocs:
-    name: str
-    attributes: list[ClassField]  # name, type
-    functions: list[FunctionDocs]
-
-    summary: str | None
-    details: str | None
-
-    @classmethod
-    def parse(cls, typ: Type) -> "ClassDocs":
-        return parse_class(typ)
+from . import models
 
 
 def split_docstring_into_sections(docstring: str) -> tuple[str, dict[str, str]]:
     """
     Splits the given docstring into sections separated by markdown headings. The
     result is the part of the string before the first heading, and a dictionary
     mapping the heading names to the text of the sections ("the summary").
@@ -221,15 +163,15 @@
     return summary, details, sections
 
 
 def parse_docstring(
     docstring: str,
     *,
     key_sections: Iterable[str],
-) -> tuple[str | None, str | None, dict[str, dict[str, str]]]:
+) -> models.Docstring:
     """
     Parses a docstring into
 
     - summary
     - details
     - sections
 
@@ -272,15 +214,19 @@
     # Make sure all requested sections are present
     missing_sections = key_sections - key_value_sections.keys()
 
     for missing_section in missing_sections:
         key_value_sections[missing_section] = {}
 
     # Done
-    return summary, details, key_value_sections
+    return models.Docstring(
+        summary=summary,
+        details=details,
+        key_sections=key_value_sections,
+    )
 
 
 def parse_function(func: Callable[..., Any]) -> models.FunctionDocs:
     """
     Given a function, parse its signature an docstring into a `FunctionDocs`
     object.
     """
@@ -337,32 +283,27 @@
             description=None,
         )
 
     # Parse the docstring
     docstring = inspect.getdoc(func)
 
     if docstring is None:
-        summary = None
-        details = None
-        raises = []
+        parsed = models.Docstring(summary=None, details=None, key_sections={})
     else:
-        summary, details, sections = parse_docstring(
-            docstring,
-            key_sections=["args", "raises"],
-        )
+        parsed = parse_docstring(docstring, key_sections=["args", "raises"])
 
-        raw_params = sections["args"]
-        raw_raises = sections["raises"]
+        raw_params = parsed.key_sections["args"]
+        raw_raises = parsed.key_sections["raises"]
 
         # Add any information learned about parameters from the docstring
         for param_name, param_details in raw_params.items():
             try:
                 result_param = parameters[param_name]
             except KeyError:
-                revel.warning(
+                warnings.warn(
                     f"The docstring for function `{func.__name__}` mentions a parameter `{param_name}` that does not exist in the function signature."
                 )
                 continue
 
             result_param.description = param_details
 
         # Add information about raised exceptions
@@ -370,61 +311,62 @@
 
     # Build the result
     return models.FunctionDocs(
         name=func.__name__,
         parameters=list(parameters.values()),
         return_type=parse_annotation(signature.return_annotation),
         synchronous=not inspect.iscoroutinefunction(func),
-        summary=summary,
-        details=details,
+        summary=parsed.summary,
+        details=parsed.details,
         raises=raises,
     )
 
 
 def _parse_class_docstring_with_inheritance(
     cls: type,
     *,
     key_sections: Iterable[str],
-) -> tuple[str | None, str | None, dict[str, dict[str, str]]]:
+) -> models.Docstring:
     """
     Parses the docstring of a class in the same format as `parse_docstring`, but
     accounts for inheritance: Key-Value sections of all classes are merged, in a
     way that preserves child docs over parent docs.
     """
 
     # Parse the docstring for this class
     raw_docs = inspect.getdoc(cls)
+
     key_sections = set(key_sections)
     parsed_docs = parse_docstring(
         "" if raw_docs is None else raw_docs,
         key_sections=key_sections,
     )
 
     # Get the docstrings for the base classes
-    base_docs: list[tuple[str | None, str | None, dict[str, dict[str, str]]]] = []
+    base_docs: list[models.Docstring] = []
 
     for base in cls.__bases__:
         base_docs.append(
             _parse_class_docstring_with_inheritance(
                 base,
                 key_sections=key_sections,
             )
         )
 
     # Merge the docstrings
     result_sections: dict[str, dict[str, str]] = {}
     all_in_order = base_docs + [parsed_docs]
 
     for docs in all_in_order:
-        for section_name, section in docs[2].items():
+        for section_name, section in docs.key_sections.items():
             result_section = result_sections.setdefault(section_name, {})
             result_section.update(section)
 
     # Done
-    return parsed_docs[0], parsed_docs[1], result_sections
+    return parsed_docs
 
 
 def parse_class(cls: type) -> models.ClassDocs:
     """
     Given a class, parse its signature an docstring into a `ClassDocs` object.
     """
 
@@ -491,15 +433,15 @@
     # Add any information learned about fields from the docstring
     raw_attributes = sections["attributes"]
 
     for field_name, field_details in raw_attributes.items():
         try:
             result_field = fields_by_name[field_name]
         except KeyError:
-            revel.warning(
+            warnings.warn(
                 f"The docstring for class `{cls.__name__}` mentions a field `{field_name}` that does not exist in the class."
             )
             continue
 
         result_field.description = field_details
 
     # If `__init__` is missing documentation for any parameters, try to copy the
```

### Comparing `imy-0.1.9/imy/inject.py` & `imy-0.2.0/imy/inject.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+"""
+A very simple dependency injection system, in pure Python.
+
+To use this, create an `Injector` instance, and bind factory functions to it.
+Each factory may depend on types provided by other factories, and returns a
+value, which is then stored in the injector.
+
+When a value is requested from the injector, it will either return an existing
+value if one is already available, or call the appropriate factory function(s)
+to create it.
+
+For convenience, a global injector is also provided, which can be accessed using
+global functions such as `get` and `bind`.
+"""
+
 from __future__ import annotations
 
 import inspect
 import io
 from typing import *  # type: ignore
 
 import introspection.typing
@@ -16,14 +31,44 @@
 ]
 
 T = TypeVar("T")
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
+def _key_from_type_annotation(annotation: Any) -> Type:
+    """
+    Given a type annotation, return the type that should be used as a key.
+    """
+    info = introspection.typing.TypeInfo(annotation)
+
+    if info.type is None:
+        raise ValueError("`None` cannot be used as a key.")
+
+    assert inspect.isclass(info.type), (annotation, info.type)
+
+    return info.type  # type: ignore
+
+
+def _key_from_type(parameter: Type) -> Type:
+    """
+    Given a type as would be passed into a function (like __getitem__), return
+    the type that should be used as a key.
+
+    This is in contrast to a type annotation, which may contain strings, forward
+    references, etc.
+    """
+    origin = get_origin(parameter)
+    key = parameter if origin is None else parameter
+
+    assert inspect.isclass(key), (parameter, key)
+
+    return key
+
+
 class DependencyCycleError(Exception):
     def __init__(self, sequence: Sequence[Type]) -> None:
         super().__init__()
         self._sequence = sequence
 
     def __str__(self) -> str:
         f = io.StringIO()
@@ -52,61 +97,66 @@
         # Make sure the parameter has a type annotation
         if parameter.annotation is parameter.empty:
             raise ValueError(
                 f"All parameters of factory functions need to have type annotations. `{parameter.name}` is missing one."
             )
 
         # Return type
-        info = introspection.typing.TypeInfo(parameter.annotation)
-        parameter_types.append(info.type)  # type: ignore
+        parameter_types.append(_key_from_type_annotation(parameter.annotation))
 
     # Return type
     return_type = signature.return_annotation
 
     if return_type is signature.empty:
         raise ValueError("Factory functions need to have a return type annotation.")
 
-    if return_type is None:
-        raise ValueError("Factory functions must return a value.")
-
-    if not inspect.isclass(return_type):
-        raise ValueError("Factory functions must return a class.")
+    return_type_key = _key_from_type_annotation(return_type)
 
     # Done
-    return parameter_types, return_type
+    return parameter_types, return_type_key
 
 
 class Injector:
+    """
+    TODO
+
+    Note on generic keys (e.g. "list[int]"): Factory functions may use arbitrarily
+    complex type annotations, however only the base type is used as a key. This
+    means that even though a `list[int]` may be attached, during retrieval,
+    `list[str]` will return the same, in this case incorrect, instance.
+
+    This is a compromise to keep the system simple and fast, since hashing
+    recursive types would be slow and is rarely useful anyway.
+    """
+
     def __init__(
         self,
         *,
         items: Iterable[Any] = [],
-        item_factories: Iterable[Callable] = [],
     ) -> None:
         # Keeps track of all components currently attached to the injector
         self._components: dict[Type, Any] = {type(item): item for item in items}
 
         # Factories can be used to create items if they are not already
         # available in the injector. Each factory may depend on any number of
         # other items and returns the newly created item.
         self._factories: dict[Type, tuple[list[Type], Callable]] = {}
 
-        for factory in item_factories:
-            types, item_type = _parse_factory(factory)
-            self._factories[item_type] = (types, factory)
-
     def _get(
         self,
-        key: Type[T],
+        raw_key: Type[T],
         *,
-        in_flight: list[Type[T]],
+        in_flight: list[Type],
     ) -> T:
         """
         Helper function for `__getitem__`.
         """
+        # Get the actual key to use
+        key = _key_from_type(raw_key)
+
         # If the item is already available in this injector, just return it
         try:
             return self._components[key]
         except KeyError:
             pass
 
         # If an item of this type is currently being constructed, there's a
@@ -114,15 +164,15 @@
         if key in in_flight:
             raise DependencyCycleError(in_flight + [key])
 
         # Try to find a factory that can create the item
         try:
             factory_param_types, factory = self._factories[key]
         except KeyError:
-            raise KeyError(key)
+            raise KeyError(raw_key)
 
         # Get all of the factory's dependencies
         factory_args: list[Any] = []
 
         for param_type in factory_param_types:
             factory_args.append(
                 self._get(
@@ -159,50 +209,65 @@
         Adds the given item to the injector. If the item is already present, it
         will be replaced.
 
         ## Raises
 
         `ValueError`: If the item is not an instance of the given type.
         """
+        # Get the actual key to use
+        key = _key_from_type(item_type)
+
         # Make sure the item is of the correct type
-        if not isinstance(item, item_type):
+        if not isinstance(item, key):
             raise ValueError(
                 f"Item has to be of type `{item_type}`, not `{type(item)}`"
             )
 
         # Add the item to the injector
-        self._components[item_type] = item
+        self._components[key] = item
 
     def bind(
         self,
-        type: Type | None = None,
+        as_type: Type | None = None,
     ) -> Callable[[Callable[P, R]], Callable[P, R]]:
         """
         Adds the decorated function to the injector as a factory. The function's
         result must be in instance of the given type or subclass thereof.
 
         ## Raises
 
         `ValueError`: If the function's return type is not a subclass of the given
             type.
+
+        `TypeError`: If there is already a factory for the type.
         """
 
         def decorator(func: Callable[P, R]) -> Callable[P, R]:
             # Parse the factory
-            param_types, return_type = _parse_factory(func)
-            key_type = return_type if type is None else type
+            param_keys, return_key = _parse_factory(func)
 
-            # Make sure the factory indeed returns the correct type
-            if type is not None and not issubclass(return_type, type):
-                raise ValueError(
-                    f"The factory has to return values of type `{type}` (or any subclass), not `{return_type}`"
+            if as_type is None:
+                key_type = return_key
+            else:
+                key_type = _key_from_type(as_type)
+
+                # Make sure the factory indeed returns the correct type
+                if not issubclass(return_key, key_type):
+                    raise ValueError(
+                        f"The factory has to return values of type `{key_type}` (or any subclass), not `{return_key}`"
+                    )
+
+            # Make sure there isn't already a factory for this type
+            if key_type in self._factories:
+                raise TypeError(
+                    f"There is already a factory for type `{key_type}`. Only one factory per type is allowed."
                 )
 
             # Register the factory
-            self._factories[key_type] = (param_types, func)
+            self._factories[key_type] = (param_keys, func)
             return func
 
         return decorator
 
 
 # Expose a global injector
 GLOBAL_INJECTOR = Injector()
```

### Comparing `imy-0.1.9/imy/logs.py` & `imy-0.2.0/imy/logs.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,55 +21,63 @@
 import uniserde
 from bson import ObjectId
 from uniserde import BsonDoc
 
 from . import async_utils
 
 try:
-    import motor  # type: ignore
-    import motor.motor_asyncio  # type: ignore
     import pymongo.collection
 except ImportError:
     if TYPE_CHECKING:
-        import motor  # type: ignore
-        import motor.motor_asyncio  # type: ignore
         import pymongo.collection
 
 
 __all__ = [
     "LogLevel",
     "LOG_LEVEL_NAMES",
+    "LOG_LEVEL_ANNOUNCEMENT",
     "Environment",
     "levels_greater_than_or_equal",
     "MongoDbLogger",
     "setup_logging",
 ]
 
 
 T = TypeVar("T")
 
 
-LogLevel: TypeAlias = Literal["debug", "info", "warning", "error", "fatal"]
+LogLevel: TypeAlias = Literal[
+    "debug",
+    "info",
+    "announcement",
+    "warning",
+    "error",
+    "fatal",
+]
 LOG_LEVEL_NAMES = get_args(LogLevel)  # In ascending order!
 
+# Add the announcement level to the logging module
+LOG_LEVEL_ANNOUNCEMENT = (logging.INFO + logging.WARNING) // 2
+logging.addLevelName(LOG_LEVEL_ANNOUNCEMENT, "ANNOUNCEMENT")
+
 Environment: TypeAlias = Literal["development", "production"]
 
 
 # Keep track of all living persistence loggers, so they can be flushed at exit
 _ALL_MONGODB_LOGGERS: weakref.WeakSet[MongoDbLogger] = weakref.WeakSet()
 
 
 @atexit.register
 def _flush_all_persistence_loggers() -> None:
     for logger in _ALL_MONGODB_LOGGERS:
         logger.flush_sync()
 
 
 def _log_level_to_python(level: LogLevel) -> int:
-    return getattr(logging, level.upper())
+    return logging.getLevelName(level.upper())
 
 
 def _log_level_from_python(level: int) -> LogLevel:
     return logging.getLevelName(level).lower()
 
 
 def levels_greater_than_or_equal(level: LogLevel) -> set[LogLevel]:
```

### Comparing `imy-0.1.9/imy/package_metadata.py` & `imy-0.2.0/imy/package_metadata.py`

 * *Files identical despite different names*

### Comparing `imy-0.1.9/imy/settings.py` & `imy-0.2.0/imy/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """
-Utilities for loading settings from JSON files and environment variables.
+Utilities for loading configuration from JSON files and environment variables.
 """
 
 from __future__ import annotations
 
 import enum
 import os
 from collections.abc import Iterable
 from datetime import datetime, timedelta
 from pathlib import Path
 from typing import *  # type: ignore
-from typing import Annotated, TypeVar
 
 import introspection.typing
 import json5
 import uniserde
 import uniserde.case_convert
 from typing_extensions import dataclass_transform
 from uniserde import Jsonable, ObjectId
 
 __all__ = [
-    "SettingsError",
-    "Settings",
+    "ConfigurationError",
+    "Config",
 ]
 
 
 _DEFAULTS_BY_TYPE: dict[Type, Any] = {
     Any: None,
     bool: False,
     bytes: b"",
@@ -42,24 +41,24 @@
     timedelta: timedelta(),
     tuple: tuple(),
     Union: None,
     ObjectId: "",
 }  # type: ignore
 
 
-class SettingsError(ValueError):
+class ConfigurationError(ValueError):
     """
-    Raised when settings couldn't be loaded, for whichever reason.
+    Raised when the configuration couldn't be loaded, for whichever reason.
     """
 
     pass
 
 
 @dataclass_transform()
-class Settings:
+class Config:
     @classmethod
     def _get_fields(cls) -> Iterable[tuple[str, type]]:
         """
         Returns iterators over all fields and their types.
         """
         for attr_name, type_info in introspection.typing.get_type_annotations(
             cls
@@ -121,62 +120,64 @@
         Parses the provided fields and values into a dictionary, transforming
         the field names using the provided `case_transform` function. The result
         is a tuple of two dictionaries: the first contains the parsed fields,
         the second any unparsed, i.e. superfluous values.
 
         ## Raises
 
-        `SettingsError`: if any fields are missing, or of the wrong type.
+        `ConfigurationError`: if any fields are missing, or of the wrong type.
         """
         # Prepare everything as dictionaries for quick lookup
         field_dict: dict[str, Type] = dict(fields)
         value_dict: dict[str, Any] = dict(values)
 
         # Parse the fields, popping them from the value dictionary
         parsed_fields: dict[str, Any] = {}
 
         for py_name, py_type in field_dict.items():
             doc_name = case_transform(py_name)
 
             try:
                 raw_value = value_dict.pop(doc_name)
             except KeyError:
-                raise SettingsError(f"The settings are missing the field `{doc_name}`")
+                raise ConfigurationError(
+                    f"The config is missing the field `{doc_name}`"
+                )
 
             try:
                 parsed_value = uniserde.from_json(raw_value, py_type)
             except uniserde.SerdeError as err:
-                raise SettingsError(
+                raise ConfigurationError(
                     f"`{raw_value}` is not a valid value for `{doc_name}`"
                 ) from err
 
             parsed_fields[py_name] = parsed_value
 
         # Are superfluous values allowed?
         if raise_on_superfluous and value_dict:
-            raise SettingsError(
-                f"The settings contain superfluous fields: `{'`, `'.join(value_dict)}`"
+            raise ConfigurationError(
+                f"The config contains superfluous fields: `{'`, `'.join(value_dict)}`"
             )
 
         # Done
         return parsed_fields, value_dict
 
     @classmethod
     def _load_from_values(
         cls,
         *,
         values: Iterable[tuple[str, Any]],
         case_transform: Callable[[str], str],
     ) -> Self:
         """
-        Loads an instance of the settings from the provided values.
+        Loads an instance of the config from the provided values.
 
         ## Raises
 
-        `SettingsError`: if any fields are missing, superfluous or of the wrong
+        `ConfigurationError`: if any fields are missing, superfluous or of the wrong
             type.
         """
         # Parse the fields
         parsed_fields, unparsed_fields = cls._parse_fields(
             fields=cls._get_fields(),
             values=values,
             case_transform=case_transform,
@@ -197,27 +198,27 @@
 
     @classmethod
     def load_from_json(
         cls,
         source: Path | IO[str] | IO[bytes] | Jsonable,
     ) -> Self:
         """
-        Loads an instance of the settings from the provided JSON source. The
+        Loads an instance of the config from the provided JSON source. The
         source can either be a path to a file, an open file-like object, or the
         result of `json.parse`.
 
         Note that **strings are not treated as paths**, but rather as already
         parsed string values.
 
         If `source` is a `Path`, and the file doesn't exist, a template will be
         dumped to the location to help out the user.
 
         ## Raises
 
-        `SettingsError`: if any fields are missing, superfluous or of the wrong
+        `ConfigurationError`: if any fields are missing, superfluous or of the wrong
             type.
         """
 
         # Load the JSON
         #
         # If a path was provided but doesn't exist, dump a template
         if isinstance(source, Path):
@@ -226,73 +227,73 @@
                     raw_values = json5.load(f)
 
             except FileNotFoundError:
                 source.parent.mkdir(parents=True, exist_ok=True)
                 with open(source, "w") as f:
                     f.write(cls._create_json_template(cls._get_fields()))
 
-                raise SettingsError(
-                    f"Could not find the settings file at `{source}`. A template has been created for you. Please fill out the values, then try again"
+                raise ConfigurationError(
+                    f"Could not find the config file at `{source}`. A template has been created for you. Please fill out the values, then try again"
                 )
 
             except ValueError as err:
-                raise SettingsError(f"`{source}` is not a valid JSON file: {err}")
+                raise ConfigurationError(f"`{source}` is not a valid JSON file: {err}")
 
         # If the source is already parsed, use it as-is
         elif isinstance(source, (type(None), bool, int, float, str, tuple, list, dict)):
             raw_values = source
 
         # Read & parse file-like objects
         else:
             try:
                 raw_values = json5.load(source)
 
             except ValueError as err:
-                raise SettingsError(f"`{source}` is not valid JSON: {err}")
+                raise ConfigurationError(f"`{source}` is not valid JSON: {err}")
 
         # Make sure the JSON has parsed into a dictionary
         if not isinstance(raw_values, dict):
-            raise SettingsError("The settings JSON must be a dictionary.")
+            raise ConfigurationError("The config JSON must be a dictionary.")
 
         # Parse the values into an instance
         return cls._load_from_values(
             values=raw_values.items(),
             case_transform=uniserde.case_convert.all_lower_to_camel_case,
         )
 
     @classmethod
     def load_from_environment(
         cls,
     ) -> Self:
         """
-        Loads an instance of the settings from the provided JSON source. The
+        Loads an instance of the config from the provided JSON source. The
         source can either be a path to a file, an open file-like object, or the
         result of `json.parse`.
 
         Note that **strings are not treated as paths**, but rather as already
         parsed string values.
 
         ## Raises
 
-        `SettingsError`: if any fields are missing, superfluous or of the wrong
+        `ConfigurationError`: if any fields are missing, superfluous or of the wrong
             type.
         """
 
         raise NotImplementedError("TODO: This function is entirely untested")
 
         # Fetch all fields from the environment
         raw_values: dict[str, str] = {}
 
         for py_field_name, field_type in cls._get_fields():
             env_name = py_field_name.upper()
 
             try:
                 raw_value = os.environ[env_name]
             except KeyError:
-                raise SettingsError(
+                raise ConfigurationError(
                     f"There is no environment variable set for `{env_name}`"
                 )
 
             raw_values[env_name] = raw_value
 
         # Right now all values are strings. Parse them into something more
         # adequate using JSON.
@@ -304,14 +305,14 @@
                 semi_parsed[py_field_name] = raw_value
                 continue
 
             # Otherwise drag them through the JSON parser
             try:
                 semi_parsed[py_field_name] = json5.loads(raw_value)
             except ValueError as err:
-                raise SettingsError(f"`{raw_value}` is not a valid value") from err
+                raise ConfigurationError(f"`{raw_value}` is not a valid value") from err
 
         # Parse the fields into an instance
         return cls._load_from_values(
             values=semi_parsed.items(),
             case_transform=str.upper,
         )
```

### Comparing `imy-0.1.9/pyproject.toml` & `imy-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "imy"
-version = "0.1.9"
+version = "0.2.0"
 description = "Random utilities I can't go without"
 authors = ["Jakob Pinterits <jakob.pinterits@gmail.com>"]
 license = "MIT"
 repository = "https://gitlab.com/Vivern/i-miss-you"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `imy-0.1.9/PKG-INFO` & `imy-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imy
-Version: 0.1.9
+Version: 0.2.0
 Summary: Random utilities I can't go without
 Home-page: https://gitlab.com/Vivern/i-miss-you
 License: MIT
 Author: Jakob Pinterits
 Author-email: jakob.pinterits@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

