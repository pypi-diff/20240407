# Comparing `tmp/jsonschema_gen-0.1.0-py3-none-any.whl.zip` & `tmp/jsonschema_gen-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 10793 bytes, number of entries: 9
--rw-r--r--  2.0 unx      234 b- defN 24-Apr-05 14:34 jsonschema_gen/__init__.py
--rw-r--r--  2.0 unx    15250 b- defN 24-Apr-05 14:34 jsonschema_gen/parsers.py
--rw-r--r--  2.0 unx     7731 b- defN 24-Apr-05 14:34 jsonschema_gen/schema.py
--rw-r--r--  2.0 unx     1814 b- defN 24-Apr-05 14:34 jsonschema_gen/utils.py
--rw-r--r--  2.0 unx     1069 b- defN 24-Apr-05 14:38 jsonschema_gen-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     7037 b- defN 24-Apr-05 14:38 jsonschema_gen-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-05 14:38 jsonschema_gen-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 24-Apr-05 14:38 jsonschema_gen-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      747 b- defN 24-Apr-05 14:38 jsonschema_gen-0.1.0.dist-info/RECORD
-9 files, 33989 bytes uncompressed, 9503 bytes compressed:  72.0%
+Zip file size: 11057 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      234 b- defN 24-Apr-07 18:10 jsonschema_gen/__init__.py
+-rw-r--r--  2.0 unx    16695 b- defN 24-Apr-07 18:10 jsonschema_gen/parsers.py
+-rw-r--r--  2.0 unx     9647 b- defN 24-Apr-07 18:10 jsonschema_gen/schema.py
+-rw-r--r--  2.0 unx     1779 b- defN 24-Apr-07 18:10 jsonschema_gen/utils.py
+-rw-r--r--  2.0 unx     1069 b- defN 24-Apr-07 18:10 jsonschema_gen-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5848 b- defN 24-Apr-07 18:10 jsonschema_gen-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 18:10 jsonschema_gen-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 24-Apr-07 18:10 jsonschema_gen-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      747 b- defN 24-Apr-07 18:10 jsonschema_gen-0.1.1.dist-info/RECORD
+9 files, 36126 bytes uncompressed, 9767 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: jsonschema_gen/schema.py
 Comment: 
 
 Filename: jsonschema_gen/utils.py
 Comment: 
 
-Filename: jsonschema_gen-0.1.0.dist-info/LICENSE
+Filename: jsonschema_gen-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: jsonschema_gen-0.1.0.dist-info/METADATA
+Filename: jsonschema_gen-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: jsonschema_gen-0.1.0.dist-info/WHEEL
+Filename: jsonschema_gen-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: jsonschema_gen-0.1.0.dist-info/top_level.txt
+Filename: jsonschema_gen-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: jsonschema_gen-0.1.0.dist-info/RECORD
+Filename: jsonschema_gen-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jsonschema_gen/__init__.py

```diff
@@ -2,8 +2,8 @@
 
 from jsonschema_gen import schema
 from jsonschema_gen.parsers import *
 
 __python_version__ = "3.8"
 __author__ = "violetblackdev@gmail.com"
 __license__ = "MIT"
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## jsonschema_gen/parsers.py

```diff
@@ -1,13 +1,14 @@
 """Collection of type parsers."""
 
 import collections.abc as c
 import inspect
 import typing as t
 from abc import ABC
+from contextlib import suppress
 from dataclasses import MISSING, fields, is_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from enum import Enum
 from inspect import _ParameterKind  # noqa: magic is required
 from numbers import Number
 from uuid import UUID, SafeUUID
@@ -20,75 +21,112 @@
                                   get_origin, is_namedtuple, is_typeddict,
                                   is_union)
 
 __all__ = [
     'TYPES', 'IncompatibleTypesError', 'Parser',
     'TypeParser', 'ListParser', 'TupleParser', 'DictParser', 'SetParser',
     'StringParser', 'IntegerParser', 'NumberParser', 'BooleanParser',
-    'ConstantParser', 'EnumTypeParser', 'EnumValueParser', 'TypedDictParser', 'TypedDictParser',
+    'ConstantParser', 'EnumTypeParser', 'EnumValueParser', 'TypedDictParser',
     'NewTypeParser', 'NamedTupleParser', 'AnyParser', 'NullParser', 'UnionParser'
 ]
 
-
-TYPES: t.List[t.Type['TypeParser']] = []  #: type parsers
+TYPES: t.List[t.Type['TypeParser']] = []  #: default collection of type parsers
 
 
 class IncompatibleTypesError(ValueError):
     """Annotation type is incompatible with JSONSchema."""
 
 
-class _FunctionAnnotation(t.NamedTuple):
+class FunctionAnnotation(t.NamedTuple):
+    """Function annotation with input kwargs and return values schemas."""
     kwargs: t.Optional[j.Object]
     returns: t.Optional[j.JSONSchemaType]
 
 
 class Parser:
+    """Python annotations parser.
+
+    Parse an annotation:
+
+    >>> Parser().parse_annotation(t.List[str], default=[]).json_repr()
+    {'items': {'type': 'string'}, 'default': [], 'type': 'array'}
+
+    Parse a function (method):
+
+    >>> def test(value: str) -> int: ...
+    >>> annotations = Parser().parse_function(test)
+    >>> annotations.kwargs.json_repr()
+    {'properties': {'value': {'type': 'string'}}, 'additionalProperties': False, 'required': ['value'], 'type': 'object'}
+
+    Parse a class:
+
+    >>> class C:
+    ...     def test(self, value: str) -> int: ...
+    >>> annotations_map = Parser().parse_class(C)
+    >>> annotations_map['test'].kwargs.json_repr()
+    {'properties': {'value': {'type': 'string'}}, 'additionalProperties': False, 'required': ['value'], 'type': 'object'}
+    """
 
     def __init__(
             self, *,
             strict: bool = True,
             private_arg_prefix: str = '_',
             types: t.Optional[t.List[t.Type['TypeParser']]] = None,
             locals: t.Optional[dict] = None
     ):
         """Initialize
 
         :param strict: strict parsing - allow only JSONSchema compatible types
             for example: UUID type is not allowed in `strict` because it's not an actual data type in JSON
         :param private_arg_prefix: ignore args starting with such prefix
         :param types: list of type parsers, by default :py:obj:`~jsonschema_gen.parsers.TYPES` is used
-        :param locals: a map of local variables to make string references work
+        :param locals: a map of local variables to resolve plain string references in type hints
         """
         self.strict = strict
         self.private_arg_prefix = private_arg_prefix
         self.types = types or TYPES
         self.locals = locals or {}
         self._types = [t(self) for t in self.types]
 
-    def parse_function(self, cls: t.Optional[t.Type], f: t.Callable) -> _FunctionAnnotation:
+    def parse_class(self, cls: t.Type, /) -> t.Dict[str, FunctionAnnotation]:
+        """Parse class methods and create an annotation map for the whole class."""
+        _method_map = {}
+        for name, value in vars(cls).items():
+            if self.private_arg_prefix and name.startswith(self.private_arg_prefix):
+                continue
+            if inspect.isfunction(value):
+                _method_map[name] = self.parse_function(value, cls)
+        return _method_map
+
+    def parse_function(self, f: t.Callable, /, cls: t.Optional[t.Type] = None) -> FunctionAnnotation:
         """Parse method or function arguments and return type into jsonschema style annotations."""
         sign = inspect.signature(f)
         params, required = {}, []
         additional_properties = False
+        is_staticmethod = isinstance(f, staticmethod)
 
         for n, (name, arg) in enumerate(sign.parameters.items()):
-            if any((
-                self.private_arg_prefix and name.startswith(self.private_arg_prefix),
-                n == 0 and name in ('self', 'cls'),
-                arg.kind == _ParameterKind.VAR_POSITIONAL
-            )):
+
+            if self.private_arg_prefix and name.startswith(self.private_arg_prefix):
                 continue
 
-            if arg.kind == _ParameterKind.POSITIONAL_ONLY:
-                raise IncompatibleTypesError('Positional only arguments cannot be converted to a JSONSchema object.')
+            # ignoring the first argument for class and instance methods
+            if cls and n == 0 and not is_staticmethod:
+                continue
+
+            if arg.kind == _ParameterKind.VAR_POSITIONAL:
+                continue
 
             if arg.kind == _ParameterKind.VAR_KEYWORD:
                 additional_properties = True
                 continue
 
+            if arg.kind == _ParameterKind.POSITIONAL_ONLY:
+                raise IncompatibleTypesError('Positional only arguments cannot be converted to a JSONSchema object.')
+
             if type(arg.annotation) is t.TypeVar:
                 if cls:
                     annotation = _parse_generic_class(cls, arg.annotation)
                 else:
                     annotation = TypeVarParser(self).parse_annotation(arg.annotation)
             else:
                 annotation = arg.annotation
@@ -106,15 +144,15 @@
         else:
             params = None
 
         if sign.return_annotation is inspect._empty:  # noqa: magic
             returns = None
         else:
             returns = self.parse_annotation(sign.return_annotation, default=...)
-        return _FunctionAnnotation(params, returns)
+        return FunctionAnnotation(params, returns)
 
     def parse_annotation(self, annotation, /, default=...) -> j.JSONSchemaType:
         """Convert python annotation into a jsonschema object."""
         if type(annotation) is t.ForwardRef:
             annotation = self.locals.get(annotation.__forward_arg__, t.Any)
 
         for parser in self._types:
@@ -166,23 +204,21 @@
     """Parse a class containing Generic hints in itself."""
     alias = base_alias = get_generic_alias(cls)
     args = base_args = alias.__args__
     while base_alias:
         base_args = base_alias.__args__
         base_cls = base_alias.__origin__
         base_alias = get_generic_alias(base_cls)
-    try:
+    with suppress(ValueError, IndexError):
         annotation = args[base_args.index(annotation)]
-    except (ValueError, IndexError):
-        pass
     return annotation
 
 
 class AnyParser(TypeParser):
-    types = (t.Any, )
+    types = (t.Any,)
     annotation = j.JSONSchemaObject
 
 
 class StringParser(TypeParser):
     types = (str, bytes, t.AnyStr)
     annotation = j.String
 
@@ -287,18 +323,15 @@
         _args = []
         for arg in self.parse_args(args):
             if type(arg) is j.AnyOf:
                 arg = t.cast(j.AnyOf, arg)
                 _args.extend(arg.items)  # noqa (ported)
             else:
                 _args.append(arg)
-        if len(_args) == 1:
-            return self.annotation(items=_args[0])
-        else:
-            return self.annotation(items=j.AnyOf(*_args))
+        return self.annotation(items=_args[0])
 
 
 class SetParser(ListParser):
     types = (set, frozenset, t.Set, c.Set, t.FrozenSet, t.MutableSet, c.MutableSet)
     annotation = j.Array
 
     def parse_annotation(self, annotation, /) -> j.JSONSchemaType:
@@ -344,15 +377,15 @@
     def parse_annotation(self, annotation: t.TypedDict, /) -> j.JSONSchemaType:
         title = annotation.__name__
         total = getattr(annotation, '__total__', True)
         properties, required = {}, []
         for key, arg in annotation.__annotations__.items():
             origin = get_origin(arg)
             if compatible_py311():
-                if origin is t.Required: # noqa: magic
+                if origin is t.Required:  # noqa: magic
                     arg = get_args(arg)[0]
                     required.append(key)
                 elif origin is t.NotRequired:  # noqa: magic
                     arg = get_args(arg)[0]
                 elif total or key in annotation.__required_keys__:  # noqa: magic
                     required.append(key)
             elif compatible_py39():
```

## jsonschema_gen/schema.py

```diff
@@ -1,14 +1,12 @@
 """Jsonschema types."""
 # pylint: disable=C0103
 
-from dataclasses import dataclass
-from functools import partial
-from typing import (Any, Collection, Dict, List, Literal, Mapping, Protocol,
-                    TypeVar)
+from dataclasses import dataclass, field
+from typing import Any, Collection, Dict, List, Literal, Mapping, Protocol, TypeVar
 
 __all__ = (
     "JSONSchemaObject",
     "JSONSchemaType",
     "Boolean",
     "String",
     "Number",
@@ -22,14 +20,15 @@
     "GUID",
     "Date",
     "DateTime",
     "Null",
     "Const",
     "Nullable",
     "Enum",
+    "Email"
 )
 
 _T = TypeVar("_T")
 _StringFormat = Literal[
     "JSONSchemaType",
     "date-time",
     "time",
@@ -47,275 +46,355 @@
     "regex",
 ]
 
 
 class JSONSchemaType(Protocol):
     """Json schema object interface."""
 
-    def get_jsonschema(self) -> Dict[str, Any]: ...
+    def json_repr(self) -> Dict[str, Any]:
+        """Produce a JSON-compatible representation of the object."""
+        return _serialize_schema_keys(vars(self))
 
 
 def _serialize_schema_value(value: Any, /) -> Any:
     if isinstance(value, Mapping):
         return _serialize_schema_keys(value)
     if isinstance(value, (list, tuple)):
         return [_serialize_schema_value(sub_value) for sub_value in value]
-    if hasattr(value, "get_jsonschema"):
-        return value.get_jsonschema()
+    if hasattr(value, "json_repr"):
+        return value.json_repr()
     return value
 
 
 def _serialize_schema_keys(obj: Mapping) -> Dict[str, Any]:
     return {
         key: _serialize_schema_value(value)
         for key, value in obj.items()
         if not key.startswith("_") and value is not None and value is not ...
     }
 
 
 @dataclass
-class JSONSchemaObject:
-    """Generic schema object."""
+class JSONSchemaObject(JSONSchemaType):
+    """Generic JSONSchema object.
 
+    >>> JSONSchemaObject().json_repr()
+    {}
+    """
     title: str = None
     description: str = None
     examples: List = None
     default: Any = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return _serialize_schema_keys(vars(self))
-
 
 @dataclass
-class Enum:
-    """Enum value alias."""
+class Enum(JSONSchemaType):
+    """Enum value.
 
+    >>> Enum([1, 2, 3]).json_repr()
+    {'enum': [1, 2, 3]}
+    """
     enum: List
     title: str = None
     description: str = None
     examples: List = None
     default: Any = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return _serialize_schema_keys(vars(self))
-
 
 @dataclass
-class Const:
+class Const(JSONSchemaType):
     """Constant value.
 
     See `constants <https://json-schema.org/understanding-json-schema/reference/const#constant-values>`_
 
+    >>> Const('1').json_repr()
+    {'const': '1'}
     """
     const: Any
     title: str = None
     description: str = None
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return _serialize_schema_keys(vars(self))
-
 
 @dataclass
-class Boolean:
+class Boolean(JSONSchemaType):
     """Boolean type.
 
     See `boolean type <https://json-schema.org/understanding-json-schema/reference/boolean>`_
-    """
 
+    >>> Boolean().json_repr()
+    {'type': 'boolean'}
+    """
     title: str = None
     description: str = None
     default: bool = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
+    def json_repr(self) -> Dict[str, Any]:
         data = _serialize_schema_keys(vars(self))
         data["type"] = "boolean"
         return data
 
 
 @dataclass
-class String:
+class String(JSONSchemaType):
     """String type.
 
     See `string type <https://json-schema.org/understanding-json-schema/reference/string>`_
-    """
 
+    >>> String().json_repr()
+    {'type': 'string'}
+    """
     minLength: int = None
     maxLength: int = None
     pattern: str = None  #: regex validation pattern
     format: _StringFormat = None  #: string format
     title: str = None
     description: str = None
     examples: List = None
     enum: List[str] = None
     default: str = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
+    def json_repr(self) -> Dict[str, Any]:
         data = _serialize_schema_keys(vars(self))
         data["type"] = "string"
         return data
 
 
-DateTime = partial(String, format="date-time")
-Date = partial(String, format="date")
-GUID = partial(String, format="uuid")
-Null = partial(Enum, enum=[None])
+@dataclass
+class DateTime(String):
+    """Datetime type alias.
+
+    >>> DateTime().json_repr()
+    {'format': 'date-time', 'type': 'string'}
+    """
+    format: str = 'date-time'
+
+
+@dataclass
+class Date(String):
+    """Date type alias.
+
+    >>> Date().json_repr()
+    {'format': 'date', 'type': 'string'}
+    """
+    format: str = field(init=False)
+
+    def __post_init__(self):
+        self.format = 'date'
 
 
 @dataclass
-class Number:
+class GUID(String):
+    """UUID type alias.
+
+    >>> GUID().json_repr()
+    {'format': 'uuid', 'type': 'string'}
+    """
+    format: str = field(init=False)
+
+    def __post_init__(self):
+        self.format = 'uuid'
+
+
+@dataclass
+class Email(String):
+    """UUID type alias.
+
+    >>> Email().json_repr()
+    {'format': 'email', 'type': 'string'}
+    """
+    format: str = field(init=False)
+
+    def __post_init__(self):
+        self.format = 'email'
+
+
+@dataclass
+class Null(Enum):
+    """Null value alias.
+
+    >>> Null().json_repr()
+    {'enum': [None]}
+    """
+    enum: list = field(init=False)
+
+    def __post_init__(self):
+        self.enum = [None]
+
+
+@dataclass
+class Number(JSONSchemaType):
     """Numeric data type.
 
     See `numeric type <https://json-schema.org/understanding-json-schema/reference/numeric#number>`_
-    """
 
+    >>> Number().json_repr()
+    {'type': 'number'}
+    """
     multipleOf: float = None
     minimum: float = None
     maximum: float = None
     exclusiveMinimum: float = None
     exclusiveMaximum: float = None
     title: str = None
     description: str = None
     examples: List = None
     enum: List[float] = None
     default: float = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
+    def json_repr(self) -> Dict[str, Any]:
         data = _serialize_schema_keys(vars(self))
         data["type"] = "number"
         return data
 
 
 @dataclass
-class Integer:
+class Integer(JSONSchemaType):
     """Integer type.
 
     See `integer type <https://json-schema.org/understanding-json-schema/reference/numeric#integer>`_
-    """
 
+    >>> Integer().json_repr()
+    {'type': 'integer'}
+    """
     multipleOf: int = None
     minimum: int = None
     maximum: int = None
     exclusiveMinimum: int = None
     exclusiveMaximum: int = None
     title: str = None
     description: str = None
     examples: List = None
     enum: List[int] = None
     default: int = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
+    def json_repr(self) -> Dict[str, Any]:
         data = _serialize_schema_keys(vars(self))
         data["type"] = "integer"
         return data
 
 
 @dataclass
-class Array:
+class Array(JSONSchemaType):
     """Array type.
 
     See `array type <https://json-schema.org/understanding-json-schema/reference/array>`_
-    """
 
+    >>> Array(String()).json_repr()
+    {'items': {'type': 'string'}, 'type': 'array'}
+    """
     items: JSONSchemaType = None  #: item type for a strict typed array
     prefixItems: Collection[JSONSchemaType] = None  #: a List of fixed object positions for a tuple type
     contains: JSONSchemaType = None  #: must contain this type of object
     additionalItems: bool = None  #: allow additional items
     uniqueItems: bool = None  #: specify an array as a set type
     minItems: int = None
     maxItems: int = None
     title: str = None
     description: str = None
     examples: List = None
     enum: List[List] = None
     default: List = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
+    def json_repr(self) -> Dict[str, Any]:
         data = _serialize_schema_keys(vars(self))
         data["type"] = "array"
         return data
 
 
 @dataclass
-class Object:
-    """Object type (Dictionary).
+class Object(JSONSchemaType):
+    """JSON object type (dictionary-like).
 
     See `object type <https://json-schema.org/understanding-json-schema/reference/object>`_
-    """
 
+    >>> Object({'name': String()}).json_repr()
+    {'properties': {'name': {'type': 'string'}}, 'type': 'object'}
+    """
     properties: Dict[str, JSONSchemaType] = None
     patternProperties: Dict[str, JSONSchemaType] = None
     additionalProperties: bool = None
     minProperties: int = None
     maxProperties: int = None
     required: List[str] = None
     title: str = None
     description: str = None
     examples: List = None
     enum: List[Dict] = None
     default: Dict = ...
 
-    def get_jsonschema(self) -> Dict[str, Any]:
+    def json_repr(self) -> Dict[str, Any]:
         data = _serialize_schema_keys(vars(self))
         data["type"] = "object"
         return data
 
 
 @dataclass
-class AnyOf:
+class AnyOf(JSONSchemaType):
     """Any of the included schemas must be valid.
 
     See `anyOf keyword <https://json-schema.org/understanding-json-schema/reference/combining#anyOf>`_
-    """
 
+    >>> AnyOf([String(), Integer()]).json_repr()
+    {'anyOf': [{'type': 'string'}, {'type': 'integer'}]}
+    """
     items: Collection[JSONSchemaType]
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return {"anyOf": [item.get_jsonschema() for item in self.items]}
+    def json_repr(self) -> Dict[str, Any]:
+        return {"anyOf": [item.json_repr() for item in self.items]}
 
 
 @dataclass
-class OneOf:
+class OneOf(JSONSchemaType):
     """Only one of the included schemas must be valid.
 
     See `oneOf keyword <https://json-schema.org/understanding-json-schema/reference/combining#oneOf>`_
-    """
 
+    >>> OneOf([String(), Integer()]).json_repr()
+    {'oneOf': [{'type': 'string'}, {'type': 'integer'}]}
+    """
     items: Collection[JSONSchemaType]
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return {"oneOf": [item.get_jsonschema() for item in self.items]}
+    def json_repr(self) -> Dict[str, Any]:
+        return {"oneOf": [item.json_repr() for item in self.items]}
 
 
 @dataclass
-class AllOf:
+class AllOf(JSONSchemaType):
     """All the included schemas must be valid.
 
     See `allOf keyword <https://json-schema.org/understanding-json-schema/reference/combining#allOf>`_
-    """
 
+    >>> AllOf([String(), Integer()]).json_repr()
+    {'allOf': [{'type': 'string'}, {'type': 'integer'}]}
+    """
     items: Collection[JSONSchemaType]
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return {"allOf": [item.get_jsonschema() for item in self.items]}
+    def json_repr(self) -> Dict[str, Any]:
+        return {"allOf": [item.json_repr() for item in self.items]}
 
 
 @dataclass
-class Not:
+class Not(JSONSchemaType):
     """Revert the condition of the schema.
 
     See `Not keyword <https://json-schema.org/understanding-json-schema/reference/combining#allOf>`_
-    """
 
+    >>> Not(Boolean()).json_repr()
+    {'not': {'type': 'boolean'}}
+    """
     item: JSONSchemaType
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return {"not": self.item.get_jsonschema()}
+    def json_repr(self) -> Dict[str, Any]:
+        return {"not": self.item.json_repr()}
 
 
 @dataclass
-class Nullable:
-    """Nullable value alias."""
+class Nullable(JSONSchemaType):
+    """Nullable value alias.
 
+    >>> Nullable(String()).json_repr()
+    {'oneOf': [{'type': 'string'}, {'enum': [None]}]}
+    """
     item: JSONSchemaType
 
-    def get_jsonschema(self) -> Dict[str, Any]:
-        return {"oneOf": [self.item.get_jsonschema(), Null()]}
+    def json_repr(self) -> Dict[str, Any]:
+        return {"oneOf": [self.item.json_repr(), Null().json_repr()]}
```

## jsonschema_gen/utils.py

```diff
@@ -1,14 +1,13 @@
 """Type hints manipulation utilities."""
 
 import inspect
 import sys
 from textwrap import dedent
-from typing import (Any, Type, Union, _GenericAlias,  # noqa: magic
-                    _TypedDictMeta)
+from typing import Any, Type, Union, _GenericAlias, _TypedDictMeta  # noqa: magic
 
 __all__ = [
     'NoneType',
     'is_generic',
     'is_typeddict',
     'is_namedtuple',
     'is_union',
@@ -67,11 +66,13 @@
 
 
 def is_namedtuple(value, /) -> bool:
     return inspect.isclass(value) and issubclass(value, tuple) and hasattr(value, '_fields')
 
 
 def is_union(value, /) -> bool:
+    if getattr(value, '__origin__', None) is Union:
+        return True
     if compatible_py310():
         from types import UnionType
-        return getattr(value, '__origin__', None) is Union or type(value) is UnionType
-    return getattr(value, '__origin__', None) is Union
+        return type(value) is UnionType
+    return False
```

## Comparing `jsonschema_gen-0.1.0.dist-info/LICENSE` & `jsonschema_gen-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jsonschema_gen-0.1.0.dist-info/RECORD` & `jsonschema_gen-0.1.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-jsonschema_gen/__init__.py,sha256=INOQfAmhgDjL5YuqbvCBYN4lflhRT_wfJsnN8jxsNfg,234
-jsonschema_gen/parsers.py,sha256=MOZCKmk-ZEy-fSBbCeOOWB7yzqw1B2gIXqfDBOyzeSw,15250
-jsonschema_gen/schema.py,sha256=_Spn5upJMxedDT0IyaIbNr8BRvwao4x80bjtQabXpCs,7731
-jsonschema_gen/utils.py,sha256=eD0jt9BNI8MyASa2Sbp6ZmKPp-82Cx6nfCNuBB8d_eA,1814
-jsonschema_gen-0.1.0.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
-jsonschema_gen-0.1.0.dist-info/METADATA,sha256=p6qa_ta8B9PPdxb4gogc3nLeLw-pM1OlVvtmjX979Lw,7037
-jsonschema_gen-0.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-jsonschema_gen-0.1.0.dist-info/top_level.txt,sha256=wV62Z1cKWhMowZALG-OeLICFjBoE9w5DDJSclEYXpDU,15
-jsonschema_gen-0.1.0.dist-info/RECORD,,
+jsonschema_gen/__init__.py,sha256=6JxvObpdp8LE98x1qfoVjNwI0gdS2mG3f9aOBK5ja1Y,234
+jsonschema_gen/parsers.py,sha256=PUQV4PwpZe_7gEO-KYSBe2MMOS1BUn5r6RfD5sEPez8,16695
+jsonschema_gen/schema.py,sha256=l5Fpm0EtupWkOOUQQJtIXD2mls9otENwHo3aEVaF_N8,9647
+jsonschema_gen/utils.py,sha256=LUuvYcg_PubLDnwGORfeXwi70y_adzkI-F1NroRREfY,1779
+jsonschema_gen-0.1.1.dist-info/LICENSE,sha256=VikX3YBzWiCgZEgI93vz50l4NdJDPjkmxFbYK9IogJ8,1069
+jsonschema_gen-0.1.1.dist-info/METADATA,sha256=m2r-jQOf_ldpdoZfPxI6GydPy3jKB58qAYq47TOdq0M,5848
+jsonschema_gen-0.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+jsonschema_gen-0.1.1.dist-info/top_level.txt,sha256=wV62Z1cKWhMowZALG-OeLICFjBoE9w5DDJSclEYXpDU,15
+jsonschema_gen-0.1.1.dist-info/RECORD,,
```

