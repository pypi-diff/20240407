# Comparing `tmp/django_mongo_backend-0.25.3.tar.gz` & `tmp/django_mongo_backend-0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mongo_backend-0.25.3.tar", max compression
+gzip compressed data, was "django_mongo_backend-0.26.tar", max compression
```

## Comparing `django_mongo_backend-0.25.3.tar` & `django_mongo_backend-0.26.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4629 2024-02-05 17:02:24.593992 django_mongo_backend-0.25.3/README.md
--rw-r--r--   0        0        0       21 2024-01-21 16:37:33.616876 django_mongo_backend-0.25.3/django_mongodb/__init__.py
--rw-r--r--   0        0        0     3913 2024-02-05 17:01:53.237736 django_mongo_backend-0.25.3/django_mongodb/base.py
--rw-r--r--   0        0        0      237 2024-01-21 16:37:33.480045 django_mongo_backend-0.25.3/django_mongodb/client.py
--rw-r--r--   0        0        0    12053 2024-02-05 21:21:00.121537 django_mongo_backend-0.25.3/django_mongodb/compiler.py
--rw-r--r--   0        0        0      805 2024-01-21 16:37:33.480477 django_mongo_backend-0.25.3/django_mongodb/creation.py
--rw-r--r--   0        0        0     3471 2024-03-14 14:24:18.197054 django_mongo_backend-0.25.3/django_mongodb/cursor.py
--rw-r--r--   0        0        0      404 2024-01-21 16:37:33.481020 django_mongo_backend-0.25.3/django_mongodb/database.py
--rw-r--r--   0        0        0      387 2024-02-05 21:38:33.051185 django_mongo_backend-0.25.3/django_mongodb/expressions.py
--rw-r--r--   0        0        0      260 2024-01-21 16:37:33.481154 django_mongo_backend-0.25.3/django_mongodb/features.py
--rw-r--r--   0        0        0      447 2024-01-21 16:37:33.481273 django_mongo_backend-0.25.3/django_mongodb/introspection.py
--rw-r--r--   0        0        0     1128 2024-01-21 16:37:33.536646 django_mongo_backend-0.25.3/django_mongodb/managers.py
--rw-r--r--   0        0        0     1539 2024-01-21 16:37:33.507095 django_mongo_backend-0.25.3/django_mongodb/models.py
--rw-r--r--   0        0        0     2125 2024-01-21 16:37:33.512723 django_mongo_backend-0.25.3/django_mongodb/operations.py
--rw-r--r--   0        0        0    13963 2024-02-05 22:14:30.943157 django_mongo_backend-0.25.3/django_mongodb/query.py
--rw-r--r--   0        0        0     1578 2024-01-21 16:37:33.481928 django_mongo_backend-0.25.3/django_mongodb/schema.py
--rw-r--r--   0        0        0     1427 2024-03-14 14:28:56.535090 django_mongo_backend-0.25.3/pyproject.toml
--rw-r--r--   0        0        0     5547 1970-01-01 00:00:00.000000 django_mongo_backend-0.25.3/PKG-INFO
+-rw-r--r--   0        0        0     4629 2024-02-05 17:02:24.593992 django_mongo_backend-0.26/README.md
+-rw-r--r--   0        0        0       21 2024-01-21 16:37:33.616876 django_mongo_backend-0.26/django_mongodb/__init__.py
+-rw-r--r--   0        0        0     3913 2024-02-05 17:01:53.237736 django_mongo_backend-0.26/django_mongodb/base.py
+-rw-r--r--   0        0        0      237 2024-01-21 16:37:33.480045 django_mongo_backend-0.26/django_mongodb/client.py
+-rw-r--r--   0        0        0    12036 2024-04-07 12:34:45.853980 django_mongo_backend-0.26/django_mongodb/compiler.py
+-rw-r--r--   0        0        0      805 2024-01-21 16:37:33.480477 django_mongo_backend-0.26/django_mongodb/creation.py
+-rw-r--r--   0        0        0     3471 2024-03-14 14:24:18.197054 django_mongo_backend-0.26/django_mongodb/cursor.py
+-rw-r--r--   0        0        0      404 2024-01-21 16:37:33.481020 django_mongo_backend-0.26/django_mongodb/database.py
+-rw-r--r--   0        0        0      387 2024-02-05 21:38:33.051185 django_mongo_backend-0.26/django_mongodb/expressions.py
+-rw-r--r--   0        0        0      260 2024-01-21 16:37:33.481154 django_mongo_backend-0.26/django_mongodb/features.py
+-rw-r--r--   0        0        0      446 2024-04-07 12:34:45.853496 django_mongo_backend-0.26/django_mongodb/introspection.py
+-rw-r--r--   0        0        0     1128 2024-01-21 16:37:33.536646 django_mongo_backend-0.26/django_mongodb/managers.py
+-rw-r--r--   0        0        0     1539 2024-01-21 16:37:33.507095 django_mongo_backend-0.26/django_mongodb/models.py
+-rw-r--r--   0        0        0     2117 2024-04-07 12:31:01.897627 django_mongo_backend-0.26/django_mongodb/operations.py
+-rw-r--r--   0        0        0    14104 2024-04-07 12:34:45.854122 django_mongo_backend-0.26/django_mongodb/query.py
+-rw-r--r--   0        0        0     1410 2024-04-07 12:28:56.051315 django_mongo_backend-0.26/django_mongodb/schema.py
+-rw-r--r--   0        0        0     1620 2024-04-07 12:34:48.336701 django_mongo_backend-0.26/pyproject.toml
+-rw-r--r--   0        0        0     5545 1970-01-01 00:00:00.000000 django_mongo_backend-0.26/PKG-INFO
```

### Comparing `django_mongo_backend-0.25.3/README.md` & `django_mongo_backend-0.26/README.md`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.25.3/django_mongodb/base.py` & `django_mongo_backend-0.26/django_mongodb/base.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.25.3/django_mongodb/compiler.py` & `django_mongo_backend-0.26/django_mongodb/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                         col.target.attname: f"${col.target.column}" for col, _, alias in self.select
                     },
                 },
             },
             {"$replaceRoot": {"newRoot": "$_id"}},
         ]
 
-    def as_operation(self, with_limits=True, with_col_aliases=False):
+    def as_operation(self, with_limits=True, with_col_aliases=False):  # noqa: C901
         combinator = self.query.combinator
         extra_select, order_by, group_by = self.pre_sql_setup(
             with_col_aliases=with_col_aliases or bool(combinator),
         )
         if combinator or extra_select or group_by or with_col_aliases:
             raise NotImplementedError
 
@@ -141,15 +141,15 @@
         except Exception:
             cursor.close()
             raise
 
         if result_type == CURSOR:
             return cursor
         if result_type == SINGLE:
-            cols = [col for col in self.select[0 : self.col_count]]
+            cols = list(self.select)
             result = cursor.fetchone()
             if result:
                 return (result.get(alias or col.target.attname) for col, _, alias in cols)
             return result
         if result_type == NO_RESULTS:
             cursor.close()
             return
```

### Comparing `django_mongo_backend-0.25.3/django_mongodb/creation.py` & `django_mongo_backend-0.26/django_mongodb/creation.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.25.3/django_mongodb/cursor.py` & `django_mongo_backend-0.26/django_mongodb/cursor.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.25.3/django_mongodb/managers.py` & `django_mongo_backend-0.26/django_mongodb/managers.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.25.3/django_mongodb/models.py` & `django_mongo_backend-0.26/django_mongodb/models.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.25.3/django_mongodb/operations.py` & `django_mongo_backend-0.26/django_mongodb/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 class DatabaseOperations(BaseDatabaseOperations):
     compiler_module = "django_mongodb.compiler"
 
     def quote_name(self, name):
         if name.startswith('"') and name.endswith('"'):
             return name
-        return '"{}"'.format(name)
+        return f'"{name}"'
 
     def sql_flush(self, style, tables, *, reset_sequences=False, allow_cascade=False):
         return [{"op": "flush", "collection": table} for table in tables]
 
     def execute_sql_flush(self, sql_list):
         with self.connection.cursor() as conn:
             for sql in sql_list:
```

### Comparing `django_mongo_backend-0.25.3/django_mongodb/query.py` & `django_mongo_backend-0.26/django_mongodb/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from django.db.models.expressions import BaseExpression, Col, Expression, Value
 from django.db.models.fields.related_lookups import RelatedExact, RelatedIn
 from django.db.models.lookups import (
     Exact,
     GreaterThan,
     GreaterThanOrEqual,
     In,
+    IntegerFieldExact,
     LessThan,
     LessThanOrEqual,
     Lookup,
 )
 from django.db.models.sql import Query
 from django.db.models.sql.where import NothingNode, WhereNode
 
@@ -34,20 +35,18 @@
         self.node = node
         self.mongo_meta = mongo_meta
 
     def requires_search(self) -> bool:
         return False
 
     @abc.abstractmethod
-    def get_mongo_query(self, compiler, connection, requires_search=...) -> dict:
-        ...
+    def get_mongo_query(self, compiler, connection, requires_search=...) -> dict: ...
 
     @abc.abstractmethod
-    def get_mongo_search(self, compiler, connection) -> dict:
-        ...
+    def get_mongo_search(self, compiler, connection) -> dict: ...
 
 
 class RawMongoQueryExpression(Node):
     def __init__(self, node: RawMongoDBQuery, mongo_meta):
         super().__init__(node, mongo_meta)
         self.node = node
 
@@ -90,16 +89,15 @@
             return {}
         if not self.rhs:
             return {}
         else:
             return self._get_mongo_search(compiler, connection)
 
     @abc.abstractmethod
-    def _get_mongo_search(self, compiler, connection) -> dict:
-        ...
+    def _get_mongo_search(self, compiler, connection) -> dict: ...
 
 
 class MongoExact(MongoLookup):
     """MongoDB Query Node for Exact"""
 
     filter_operator = "$eq"
 
@@ -144,15 +142,17 @@
 
 class MongoEqualityComparison(MongoLookup):
     """MongoDB Query Node for LessThanOrEqual"""
 
     filter_operator: str
 
     def __init__(
-        self, operator: LessThan | LessThanOrEqual | GreaterThan | GreaterThanOrEqual, mongo_meta
+        self,
+        operator: LessThan | LessThanOrEqual | GreaterThan | GreaterThanOrEqual,
+        mongo_meta,
     ):
         super().__init__(operator, mongo_meta)
         self.filter_operator = {
             LessThan: "$lt",
             LessThanOrEqual: "$lte",
             GreaterThan: "$gt",
             GreaterThanOrEqual: "$gte",
@@ -182,16 +182,15 @@
         else:
             return {}
 
     def get_mongo_search(self, compiler, connection) -> dict:
         return self._get_mongo_search(compiler, connection)
 
     @abstractmethod
-    def _get_mongo_search(self, compiler, connection) -> dict:
-        ...
+    def _get_mongo_search(self, compiler, connection) -> dict: ...
 
 
 class MongoSearchLookup(SearchNode):
     """MongoDB Search Query Node for SearchVectorExact"""
 
     def __init__(self, exact: Lookup, mongo_meta):
         super().__init__(exact, mongo_meta)
@@ -256,14 +255,15 @@
 
 class MongoWhereNode:
     """MongoDB Query Node for WhereNode"""
 
     node_map = {
         NothingNode: MongoNothingNode,
         Exact: MongoExact,
+        IntegerFieldExact: MongoExact,
         RelatedIn: MongoRelatedIn,
         RelatedExact: MongoExact,
         In: MongoIn,
         LessThan: MongoEqualityComparison,
         LessThanOrEqual: MongoEqualityComparison,
         GreaterThan: MongoEqualityComparison,
         GreaterThanOrEqual: MongoEqualityComparison,
@@ -310,15 +310,18 @@
         elif self.connector == "OR":
             return {"$or": child_queries} if not self.negated else {"$nor": child_queries}
         else:
             raise Exception(f"Unsupported connector: {self.connector}")
 
     def get_mongo_search(self, compiler, connection) -> dict:
         child_queries = list(
-            filter(bool, [child.get_mongo_search(compiler, connection) for child in self.children])
+            filter(
+                bool,
+                [child.get_mongo_search(compiler, connection) for child in self.children],
+            )
         )
         if len(child_queries) == 0:
             return {}
         elif self.connector == "AND":
             return {"compound": {"must": child_queries}}
         elif self.connector == "OR":
             return {"compound": {"should": child_queries}}
@@ -351,15 +354,18 @@
         self.col = col
         self.mongo_meta = mongo_meta
         self.alias = alias
 
     def get_mongo(self):
         return {
             "$group": {"_id": None, "_count": {"$sum": 1}},
-            "$project": {"_id": None, (self.alias or self.col.output_field.column): "$_count"},
+            "$project": {
+                "_id": None,
+                (self.alias or self.col.output_field.column): "$_count",
+            },
         }
 
 
 class MongoSelect:
     def __init__(self, _cols: list[tuple[Expression, tuple, str | None]], mongo_meta):
         self.mongo_meta = mongo_meta
         self.cols = []
```

### Comparing `django_mongo_backend-0.25.3/django_mongodb/schema.py` & `django_mongo_backend-0.26/django_mongodb/schema.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,69 +1,48 @@
 from django.db.backends.base.schema import BaseDatabaseSchemaEditor
 
 
 class DatabaseSchemaEditor(BaseDatabaseSchemaEditor):
     def quote_value(self, value):
         return value
 
-    def add_constraint(self, model, constraint):
-        ...
+    def add_constraint(self, model, constraint): ...
 
-    def add_field(self, model, field):
-        ...
+    def add_field(self, model, field): ...
 
-    def add_index(self, model, index):
-        ...
+    def add_index(self, model, index): ...
 
-    def alter_db_table(self, model, old_db_table, new_db_table):
-        ...
+    def alter_db_table(self, model, old_db_table, new_db_table): ...
 
-    def alter_db_table_comment(self, model, old_db_table_comment, new_db_table_comment):
-        ...
+    def alter_db_table_comment(self, model, old_db_table_comment, new_db_table_comment): ...
 
-    def alter_db_tablespace(self, model, old_db_tablespace, new_db_tablespace):
-        ...
+    def alter_db_tablespace(self, model, old_db_tablespace, new_db_tablespace): ...
 
-    def alter_field(self, model, old_field, new_field, strict=False):
-        ...
+    def alter_field(self, model, old_field, new_field, strict=False): ...
 
-    def alter_index_together(self, model, old_index_together, new_index_together):
-        ...
+    def alter_index_together(self, model, old_index_together, new_index_together): ...
 
-    def alter_unique_together(self, model, old_unique_together, new_unique_together):
-        ...
+    def alter_unique_together(self, model, old_unique_together, new_unique_together): ...
 
-    def create_model(self, model):
-        ...
+    def create_model(self, model): ...
 
-    def delete_model(self, model):
-        ...
+    def delete_model(self, model): ...
 
-    def effective_default(self, field):
-        ...
+    def effective_default(self, field): ...
 
-    def prepare_default(self, value):
-        ...
+    def prepare_default(self, value): ...
 
-    def quote_name(self, name):
-        ...
+    def quote_name(self, name): ...
 
-    def remove_constraint(self, model, constraint):
-        ...
+    def remove_constraint(self, model, constraint): ...
 
-    def remove_field(self, model, field):
-        ...
+    def remove_field(self, model, field): ...
 
-    def remove_index(self, model, index):
-        ...
+    def remove_index(self, model, index): ...
 
-    def remove_procedure(self, procedure_name, param_types=()):
-        ...
+    def remove_procedure(self, procedure_name, param_types=()): ...
 
-    def rename_index(self, model, old_index_name, new_index_name):
-        ...
+    def rename_index(self, model, old_index_name, new_index_name): ...
 
-    def skip_default(self, field):
-        ...
+    def skip_default(self, field): ...
 
-    def skip_default_on_alter(self, field):
-        ...
+    def skip_default_on_alter(self, field): ...
```

### Comparing `django_mongo_backend-0.25.3/PKG-INFO` & `django_mongo_backend-0.26/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mongo-backend
-Version: 0.25.3
+Version: 0.26
 Summary: 
 Home-page: https://github.com/gersmann/django-mongo-backend
 Keywords: django,mongodb,backend
 Author: gersmann
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

