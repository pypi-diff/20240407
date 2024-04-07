# Comparing `tmp/django-snowflake-5.0.2.tar.gz` & `tmp/django-snowflake-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-snowflake-5.0.2.tar", last modified: Fri Feb 23 14:26:40 2024, max compression
+gzip compressed data, was "django-snowflake-5.0.3.tar", last modified: Sun Apr  7 01:18:56 2024, max compression
```

## Comparing `django-snowflake-5.0.2.tar` & `django-snowflake-5.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-02-23 14:26:40.698435 django-snowflake-5.0.2/
--rw-rw-r--   0 tim       (1000) tim       (1000)      688 2024-02-23 14:25:27.000000 django-snowflake-5.0.2/CHANGELOG.md
--rw-rw-r--   0 tim       (1000) tim       (1000)      337 2024-02-23 14:22:50.000000 django-snowflake-5.0.2/LEGAL.md
--rw-rw-r--   0 tim       (1000) tim       (1000)     1058 2023-04-17 10:27:54.000000 django-snowflake-5.0.2/LICENSE
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-02-23 14:22:50.000000 django-snowflake-5.0.2/MANIFEST.in
--rw-r--r--   0 tim       (1000) tim       (1000)     6718 2024-02-23 14:26:40.698435 django-snowflake-5.0.2/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     5718 2024-02-23 14:24:01.000000 django-snowflake-5.0.2/README.md
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-02-23 14:26:40.694435 django-snowflake-5.0.2/django_snowflake/
--rw-rw-r--   0 tim       (1000) tim       (1000)      349 2024-02-23 14:26:02.000000 django-snowflake-5.0.2/django_snowflake/__init__.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7151 2024-02-23 14:24:08.000000 django-snowflake-5.0.2/django_snowflake/base.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2639 2024-02-23 14:22:50.000000 django-snowflake-5.0.2/django_snowflake/client.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     4232 2024-02-23 14:22:50.000000 django-snowflake-5.0.2/django_snowflake/compiler.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     2150 2023-04-10 00:45:58.000000 django-snowflake-5.0.2/django_snowflake/creation.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    29498 2024-02-23 14:24:01.000000 django-snowflake-5.0.2/django_snowflake/features.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     1891 2023-04-10 00:45:58.000000 django-snowflake-5.0.2/django_snowflake/functions.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     8679 2024-02-23 14:22:50.000000 django-snowflake-5.0.2/django_snowflake/introspection.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     3040 2024-02-23 14:22:50.000000 django-snowflake-5.0.2/django_snowflake/lookups.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     8063 2024-02-23 14:22:50.000000 django-snowflake-5.0.2/django_snowflake/operations.py
--rw-rw-r--   0 tim       (1000) tim       (1000)     7804 2024-02-23 14:24:01.000000 django-snowflake-5.0.2/django_snowflake/schema.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      766 2023-04-10 00:45:58.000000 django-snowflake-5.0.2/django_snowflake/utils.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-02-23 14:26:40.698435 django-snowflake-5.0.2/django_snowflake.egg-info/
--rw-r--r--   0 tim       (1000) tim       (1000)     6718 2024-02-23 14:26:40.000000 django-snowflake-5.0.2/django_snowflake.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)      613 2024-02-23 14:26:40.000000 django-snowflake-5.0.2/django_snowflake.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-02-23 14:26:40.000000 django-snowflake-5.0.2/django_snowflake.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       34 2024-02-23 14:26:40.000000 django-snowflake-5.0.2/django_snowflake.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       17 2024-02-23 14:26:40.000000 django-snowflake-5.0.2/django_snowflake.egg-info/top_level.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)     1181 2024-02-23 14:26:40.698435 django-snowflake-5.0.2/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-04-10 00:45:59.000000 django-snowflake-5.0.2/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-07 01:18:56.799463 django-snowflake-5.0.3/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      810 2024-04-07 01:17:45.000000 django-snowflake-5.0.3/CHANGELOG.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)      337 2024-03-01 22:35:53.000000 django-snowflake-5.0.3/LEGAL.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1058 2023-04-17 10:27:54.000000 django-snowflake-5.0.3/LICENSE
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2024-03-01 22:35:53.000000 django-snowflake-5.0.3/MANIFEST.in
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6689 2024-04-07 01:18:56.799463 django-snowflake-5.0.3/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5718 2024-04-07 01:15:59.000000 django-snowflake-5.0.3/README.md
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-07 01:18:56.799463 django-snowflake-5.0.3/django_snowflake/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      426 2024-04-07 01:17:37.000000 django-snowflake-5.0.3/django_snowflake/__init__.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7151 2024-03-01 22:37:25.000000 django-snowflake-5.0.3/django_snowflake/base.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2639 2024-03-01 22:35:53.000000 django-snowflake-5.0.3/django_snowflake/client.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     4232 2024-04-04 23:15:19.000000 django-snowflake-5.0.3/django_snowflake/compiler.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2150 2023-04-10 00:45:58.000000 django-snowflake-5.0.3/django_snowflake/creation.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      414 2024-04-07 01:16:03.000000 django-snowflake-5.0.3/django_snowflake/expressions.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    24735 2024-04-07 01:16:03.000000 django-snowflake-5.0.3/django_snowflake/features.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1891 2023-04-10 00:45:58.000000 django-snowflake-5.0.3/django_snowflake/functions.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     8679 2024-03-01 22:35:53.000000 django-snowflake-5.0.3/django_snowflake/introspection.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3040 2024-03-01 22:35:53.000000 django-snowflake-5.0.3/django_snowflake/lookups.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     8063 2024-03-01 22:35:53.000000 django-snowflake-5.0.3/django_snowflake/operations.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)     7804 2024-04-07 01:15:59.000000 django-snowflake-5.0.3/django_snowflake/schema.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      766 2023-04-10 00:45:58.000000 django-snowflake-5.0.3/django_snowflake/utils.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2024-04-07 01:18:56.799463 django-snowflake-5.0.3/django_snowflake.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     6689 2024-04-07 01:18:56.000000 django-snowflake-5.0.3/django_snowflake.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)      645 2024-04-07 01:18:56.000000 django-snowflake-5.0.3/django_snowflake.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2024-04-07 01:18:56.000000 django-snowflake-5.0.3/django_snowflake.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       34 2024-04-07 01:18:56.000000 django-snowflake-5.0.3/django_snowflake.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       17 2024-04-07 01:18:56.000000 django-snowflake-5.0.3/django_snowflake.egg-info/top_level.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1181 2024-04-07 01:18:56.799463 django-snowflake-5.0.3/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-04-10 00:45:59.000000 django-snowflake-5.0.3/setup.py
```

### Comparing `django-snowflake-5.0.2/CHANGELOG.md` & `django-snowflake-5.0.3/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 5.0.3 - 2024-04-06
+
+* Fixed `EXISTS` subqueries by removing `LIMIT 1` (which Snowflake does not
+  support) from them.
+
 ## 5.0.2 - 2024-02-23
 
 * Fixed data corruption of new model instance IDs. Connection initialization
   now sets `NOORDER_SEQUENCE_AS_DEFAULT=False` (after [the default
   changed to True](https://docs.snowflake.com/en/release-notes/bcr-bundles/2024_01/bcr-1483)
   in behavior change bundle 2024_01) to allow this backend to continue to
   retrieve the ID of newly created objects using
```

### Comparing `django-snowflake-5.0.2/LICENSE` & `django-snowflake-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/PKG-INFO` & `django-snowflake-5.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: django-snowflake
-Version: 5.0.2
+Version: 5.0.3
 Summary: Django backend for Snowflake
 Home-page: https://github.com/Snowflake-Labs/django-snowflake
 Maintainer: Tim Graham
 Maintainer-email: timograham@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Snowflake-Labs/django-snowflake
 Project-URL: Tracker, https://github.com/Snowflake-Labs/django-snowflake/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: snowflake-connector-python>=3.6.0
 
 # Snowflake backend for Django
 
 ## Install and usage
 
 Use the version of django-snowflake that corresponds to your version of
 Django. For example, to get the latest compatible release for Django 5.0.x:
@@ -166,7 +166,9 @@
         "snowflake.connector": {
             "level": "DEBUG",
             "handlers": ["console"],
         },
     },
 }
 ```
+
+
```

### Comparing `django-snowflake-5.0.2/README.md` & `django-snowflake-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/base.py` & `django-snowflake-5.0.3/django_snowflake/base.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/client.py` & `django-snowflake-5.0.3/django_snowflake/client.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/compiler.py` & `django-snowflake-5.0.3/django_snowflake/compiler.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/creation.py` & `django-snowflake-5.0.3/django_snowflake/creation.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/features.py` & `django-snowflake-5.0.3/django_snowflake/features.py`

 * *Files 17% similar despite different names*

```diff
@@ -39,14 +39,16 @@
     supports_table_check_constraints = False
     supports_expression_indexes = False
     supports_ignore_conflicts = False
     # This feature is specific to the Django fork used for testing.
     supports_indexes = False
     supports_index_column_ordering = False
     supports_json_field_contains = False
+    # This feature is specific to the Django fork used for testing.
+    supports_limit_in_exists = False
     supports_over_clause = True
     supports_partial_indexes = False
     # https://docs.snowflake.com/en/sql-reference/functions-regexp.html#backreferences
     supports_regex_backreferencing = False
     supports_sequence_reset = False
     supports_slicing_ordering_in_compound = True
     supports_subqueries_in_group_by = False
@@ -129,14 +131,18 @@
         #     lookup='value__bar__in', value=[['foo', 'bar'], ['a']]
         #     lookup='value__bax__in', value=[{'foo': 'bar'}, {'a': 'b'}]
         # Query:
         #   WHERE TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":bar) IN ('["foo", "bar"]')
         # needs to operate as:
         #   WHERE TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":bar) IN (PARSE_JSON('["foo", "bar"]'))
         'model_fields.test_jsonfield.TestQuerying.test_key_in',
+        # This isn't compatible with the SELECT ... FROM VALUES workaround
+        # for inserting JSON data. In other words, this query doesn't work:
+        # SELECT parse_json($1) FROM VALUES (DEFAULT);
+        'schema.tests.SchemaTests.test_db_default_output_field_resolving',
         # QuerySet.bulk_update() not supported for JSONField:
         # Expression type does not match column data type, expecting VARIANT
         # but got VARCHAR(16777216) for column JSON_FIELD
         'queries.test_bulk_update.BulkUpdateTests.test_json_field',
         # Server-side bug?
         # CAST(TO_JSON("MODEL_FIELDS_NULLABLEJSONMODEL"."VALUE":d) AS VARIANT)
         # gives '"[\\"e\\",{\\"f\\":\\"g\\"}]"' and appending [0] gives None.
@@ -203,111 +209,48 @@
             'schema.tests.SchemaTests.test_remove_unique_together_does_not_remove_meta_constraints',
             'schema.tests.SchemaTests.test_text_field_with_db_index',
         },
         'Snowflake does not enforce PositiveIntegerField constraint.': {
             'model_fields.test_integerfield.PositiveIntegerFieldTests.test_negative_values',
         },
         'Snowflake: Unsupported subquery type cannot be evaluated.': {
-            'admin_changelist.tests.ChangeListTests.test_multiple_search_fields',
-            'admin_filters.tests.ListFiltersTests.test_emptylistfieldfilter_genericrelation',
-            'admin_filters.tests.ListFiltersTests.test_emptylistfieldfilter_reverse_relationships',
-            'admin_filters.tests.ListFiltersTests.test_listfilter_genericrelation',
-            'admin_filters.tests.ListFiltersTests.test_relatedfieldlistfilter_manytomany',
-            'admin_filters.tests.ListFiltersTests.test_relatedfieldlistfilter_reverse_relationships',
-            'admin_views.tests.AdminSearchTest.test_exact_matches',
-            'admin_views.tests.AdminSearchTest.test_no_total_count',
-            'admin_views.tests.AdminSearchTest.test_search_on_sibling_models',
-            'admin_views.tests.AdminViewBasicTest.test_relation_spanning_filters',
-            'admin_views.tests.LimitChoicesToInAdminTest.test_limit_choices_to_as_callable',
-            'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_on_exists',
             'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_ref_multiple_subquery_annotation',  # noqa
             'aggregation.test_filter_argument.FilteredAggregateTests.test_filtered_aggregate_ref_subquery_annotation',
             'aggregation.tests.AggregateAnnotationPruningTests.test_referenced_composed_subquery_requires_wrapping',
             'aggregation.tests.AggregateAnnotationPruningTests.test_referenced_subquery_requires_wrapping',
-            'aggregation.tests.AggregateTestCase.test_aggregation_exists_multivalued_outeref',
             'aggregation.tests.AggregateTestCase.test_aggregation_subquery_annotation',
             'aggregation.tests.AggregateTestCase.test_aggregation_subquery_annotation_values',
-            'aggregation.tests.AggregateTestCase.test_aggregation_subquery_annotation_values_collision',
-            'aggregation_regress.tests.AggregationTests.test_annotate_and_join',
-            'annotations.tests.NonAggregateAnnotationTestCase.test_annotation_exists_aggregate_values_chaining',
             'annotations.tests.NonAggregateAnnotationTestCase.test_annotation_filter_with_subquery',
             'annotations.tests.NonAggregateAnnotationTestCase.test_annotation_subquery_outerref_transform',
-            'auth_tests.test_models.UserWithPermTestCase.test_basic',
-            'auth_tests.test_models.UserWithPermTestCase.test_nonexistent_permission',
             'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_extract_outerref',
             'db_functions.datetime.test_extract_trunc.DateFunctionTests.test_trunc_subquery_with_parameters',
-            'db_functions.datetime.test_extract_trunc.DateFunctionWithTimeZoneTests.test_extract_outerref',
             'expressions.tests.BasicExpressionsTests.test_aggregate_subquery_annotation',
             'expressions.tests.BasicExpressionsTests.test_annotation_with_deeply_nested_outerref',
             'expressions.tests.BasicExpressionsTests.test_annotation_with_nested_outerref',
             'expressions.tests.BasicExpressionsTests.test_annotation_with_outerref',
             'expressions.tests.BasicExpressionsTests.test_annotations_within_subquery',
-            'expressions.tests.BasicExpressionsTests.test_boolean_expression_combined',
-            'expressions.tests.BasicExpressionsTests.test_boolean_expression_combined_with_empty_Q',
-            'expressions.tests.BasicExpressionsTests.test_boolean_expression_in_Q',
-            'expressions.tests.BasicExpressionsTests.test_case_in_filter_if_boolean_output_field',
-            'expressions.tests.BasicExpressionsTests.test_exists_in_filter',
             'expressions.tests.BasicExpressionsTests.test_nested_outerref_with_function',
             'expressions.tests.BasicExpressionsTests.test_nested_subquery',
             'expressions.tests.BasicExpressionsTests.test_nested_subquery_join_outer_ref',
             'expressions.tests.BasicExpressionsTests.test_nested_subquery_outer_ref_2',
             'expressions.tests.BasicExpressionsTests.test_nested_subquery_outer_ref_with_autofield',
-            'expressions.tests.BasicExpressionsTests.test_order_by_exists',
             'expressions.tests.BasicExpressionsTests.test_subquery',
             'expressions.tests.BasicExpressionsTests.test_subquery_filter_by_lazy',
             'expressions.tests.BasicExpressionsTests.test_subquery_in_filter',
             'expressions.tests.FTimeDeltaTests.test_date_subquery_subtraction',
             'expressions.tests.FTimeDeltaTests.test_datetime_subquery_subtraction',
             'expressions_window.tests.WindowFunctionTests.test_subquery_row_range_rank',
-            'filtered_relation.tests.FilteredRelationTests.test_with_exclude',
-            'generic_relations.tests.GenericRelationsTests.test_queries_content_type_restriction',
-            'generic_relations_regress.tests.GenericRelationTests.test_ticket_20378',
-            'generic_relations_regress.tests.GenericRelationTests.test_ticket_20564',
-            'generic_relations_regress.tests.GenericRelationTests.test_ticket_20564_nullable_fk',
             'lookup.tests.LookupQueryingTests.test_filter_subquery_lhs',
             'lookup.tests.LookupTests.test_nested_outerref_lhs',
-            'many_to_many.tests.ManyToManyTests.test_selects',
             'model_fields.test_jsonfield.TestQuerying.test_nested_key_transform_on_subquery',
             'model_fields.test_jsonfield.TestQuerying.test_obj_subquery_lookup',
-            'model_forms.tests.LimitChoicesToTests.test_fields_for_model_applies_limit_choices_to',
-            'model_forms.tests.LimitChoicesToTests.test_limit_choices_to_callable_for_fk_rel',
-            'model_forms.tests.LimitChoicesToTests.test_limit_choices_to_callable_for_m2m_rel',
-            'model_forms.tests.LimitChoicesToTests.test_limit_choices_to_m2m_through',
-            'model_forms.tests.LimitChoicesToTests.test_limit_choices_to_no_duplicates',
             'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_in_subquery',
             'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_in_subquery_related_outerref',
-            'queries.test_qs_combinators.QuerySetSetOperationTests.test_union_with_values_list_on_annotated_and_unannotated',  # noqa
-            'queries.tests.ExcludeTest17600.test_exclude_plain',
-            'queries.tests.ExcludeTest17600.test_exclude_plain_distinct',
-            'queries.tests.ExcludeTest17600.test_exclude_with_q_is_equal_to_plain_exclude',
-            'queries.tests.ExcludeTest17600.test_exclude_with_q_is_equal_to_plain_exclude_variation',
-            'queries.tests.ExcludeTest17600.test_exclude_with_q_object_distinct',
-            'queries.tests.ExcludeTest17600.test_exclude_with_q_object_no_distinct',
-            'queries.tests.ExcludeTests.test_exclude_multivalued_exists',
             'queries.tests.ExcludeTests.test_exclude_subquery',
             'queries.tests.ExcludeTests.test_subquery_exclude_outerref',
-            'queries.tests.ExcludeTests.test_exclude_m2m_through',
-            'queries.tests.ExcludeTests.test_to_field',
-            'queries.tests.ForeignKeyToBaseExcludeTests.test_ticket_21787',
-            'queries.tests.JoinReuseTest.test_inverted_q_across_relations',
-            'queries.tests.ManyToManyExcludeTest.test_exclude_many_to_many',
-            'queries.tests.ManyToManyExcludeTest.test_ticket_12823',
-            'queries.tests.Queries1Tests.test_double_exclude',
-            'queries.tests.Queries1Tests.test_exclude',
-            'queries.tests.Queries1Tests.test_exclude_in',
-            'queries.tests.Queries1Tests.test_nested_exclude',
-            'queries.tests.Queries1Tests.test_ticket7096',
-            'queries.tests.Queries1Tests.test_tickets_5324_6704',
-            'queries.tests.Queries4Tests.test_ticket24525',
-            'queries.tests.Queries6Tests.test_tickets_8921_9188',
-            'queries.tests.Queries6Tests.test_xor_subquery',
-            'queries.tests.TestTicket24605.test_ticket_24605',
-            'queries.tests.Ticket20788Tests.test_ticket_20788',
-            'queries.tests.Ticket22429Tests.test_ticket_22429',
-            'queries.tests.Ticket23605Tests.test_ticket_23605',
         },
         'Snowflake: Window function type [ROW_NUMBER] requires ORDER BY in '
         'window specification.': {
              'expressions_window.tests.WindowFunctionTests.test_row_number_no_ordering',
         },
         # https://github.com/Snowflake-Labs/django-snowflake/issues/40
         'DatabaseOperations.sequence_reset_sql() must be implemented for this test.': {
```

### Comparing `django-snowflake-5.0.2/django_snowflake/functions.py` & `django-snowflake-5.0.3/django_snowflake/functions.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/introspection.py` & `django-snowflake-5.0.3/django_snowflake/introspection.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/lookups.py` & `django-snowflake-5.0.3/django_snowflake/lookups.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/operations.py` & `django-snowflake-5.0.3/django_snowflake/operations.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/schema.py` & `django-snowflake-5.0.3/django_snowflake/schema.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake/utils.py` & `django-snowflake-5.0.3/django_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `django-snowflake-5.0.2/django_snowflake.egg-info/PKG-INFO` & `django-snowflake-5.0.3/django_snowflake.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: django-snowflake
-Version: 5.0.2
+Version: 5.0.3
 Summary: Django backend for Snowflake
 Home-page: https://github.com/Snowflake-Labs/django-snowflake
 Maintainer: Tim Graham
 Maintainer-email: timograham@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/Snowflake-Labs/django-snowflake
 Project-URL: Tracker, https://github.com/Snowflake-Labs/django-snowflake/issues
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: snowflake-connector-python>=3.6.0
 
 # Snowflake backend for Django
 
 ## Install and usage
 
 Use the version of django-snowflake that corresponds to your version of
 Django. For example, to get the latest compatible release for Django 5.0.x:
@@ -166,7 +166,9 @@
         "snowflake.connector": {
             "level": "DEBUG",
             "handlers": ["console"],
         },
     },
 }
 ```
+
+
```

### Comparing `django-snowflake-5.0.2/django_snowflake.egg-info/SOURCES.txt` & `django-snowflake-5.0.3/django_snowflake.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 setup.cfg
 setup.py
 django_snowflake/__init__.py
 django_snowflake/base.py
 django_snowflake/client.py
 django_snowflake/compiler.py
 django_snowflake/creation.py
+django_snowflake/expressions.py
 django_snowflake/features.py
 django_snowflake/functions.py
 django_snowflake/introspection.py
 django_snowflake/lookups.py
 django_snowflake/operations.py
 django_snowflake/schema.py
 django_snowflake/utils.py
```

### Comparing `django-snowflake-5.0.2/setup.cfg` & `django-snowflake-5.0.3/setup.cfg`

 * *Files identical despite different names*

