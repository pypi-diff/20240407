# Comparing `tmp/xmlschema-3.1.0.tar.gz` & `tmp/xmlschema-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmlschema-3.1.0.tar", last modified: Wed Mar 13 05:28:26 2024, max compression
+gzip compressed data, was "xmlschema-3.2.0.tar", last modified: Mon Mar 25 21:28:36 2024, max compression
```

## Comparing `xmlschema-3.1.0.tar` & `xmlschema-3.2.0.tar`

### file list

```diff
@@ -1,571 +1,572 @@
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.898483 xmlschema-3.1.0/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-3.1.0/.coveragerc
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27485 2024-03-13 05:27:13.000000 xmlschema-3.1.0/CHANGELOG.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2024-01-07 11:20:34.000000 xmlschema-3.1.0/LICENSE
--rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-3.1.0/MANIFEST.in
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-03-13 05:28:26.897483 xmlschema-3.1.0/PKG-INFO
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2024-02-18 21:08:04.000000 xmlschema-3.1.0/README.rst
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.764483 xmlschema-3.1.0/doc/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-3.1.0/doc/Makefile
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11862 2024-02-18 10:42:48.000000 xmlschema-3.1.0/doc/api.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-3.1.0/doc/components.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5483 2024-03-13 05:27:13.000000 xmlschema-3.1.0/doc/conf.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-3.1.0/doc/converters.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-3.1.0/doc/extras.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9945 2024-01-07 11:20:34.000000 xmlschema-3.1.0/doc/features.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-3.1.0/doc/index.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-3.1.0/doc/intro.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)       82 2024-02-03 22:44:00.000000 xmlschema-3.1.0/doc/requirements.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-3.1.0/doc/testing.rst
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30692 2024-01-16 07:17:09.000000 xmlschema-3.1.0/doc/usage.rst
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-3.1.0/mypy.ini
--rw-r--r--   0 brunato   (1000) brunato   (1000)       81 2023-09-23 04:52:41.000000 xmlschema-3.1.0/pyproject.toml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2024-03-13 05:27:13.000000 xmlschema-3.1.0/requirements-dev.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2024-03-13 05:28:26.898483 xmlschema-3.1.0/setup.cfg
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2765 2024-03-13 05:27:13.000000 xmlschema-3.1.0/setup.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.771483 xmlschema-3.1.0/tests/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-3.1.0/tests/__init__.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     6753 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/check_memory.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.740483 xmlschema-3.1.0/tests/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.771483 xmlschema-3.1.0/tests/templates/demo/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/demo/demo_type_filter_test.jinja
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.773483 xmlschema-3.1.0/tests/templates/filters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/filters/name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/filters/namespace_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/filters/python_type_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/filters/qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/filters/sort_types_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-3.1.0/tests/templates/filters/type_name_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/filters/type_qname_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/templates/filters/unknown_filter_test.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.1.0/tests/templates/filters/wrong-template.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3574 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_all.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.774483 xmlschema-3.1.0/tests/test_cases/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.741483 xmlschema-3.1.0/tests/test_cases/examples/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.780483 xmlschema-3.1.0/tests/test_cases/examples/collection/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection-default.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1171 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2024-03-13 05:24:31.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection3bis.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection3bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection4.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-3.1.0/tests/test_cases/examples/collection/collection5.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.781483 xmlschema-3.1.0/tests/test_cases/examples/menù/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      559 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/examples/menù/menù-ascii.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/examples/menù/menù-ascii.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      532 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/examples/menù/menù-cp1252.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      509 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/examples/menù/menù-cp1252.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)        3 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/examples/menù/menù.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)      542 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/examples/menù/menù.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/examples/menù/menù.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.782483 xmlschema-3.1.0/tests/test_cases/examples/stockquote/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/examples/stockquote/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/examples/stockquote/stockquote.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.786483 xmlschema-3.1.0/tests/test_cases/examples/vehicles/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/bikes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/cars.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-1_error.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-1_error.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-3_errors.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-max.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-redef.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles2.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles2.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.742483 xmlschema-3.1.0/tests/test_cases/features/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.787483 xmlschema-3.1.0/tests/test_cases/features/attributes/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/attributes/default_attributes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.787483 xmlschema-3.1.0/tests/test_cases/features/builtins/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/builtins/builtins.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/builtins/builtins.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.789483 xmlschema-3.1.0/tests/test_cases/features/decoder/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-3.1.0/tests/test_cases/features/decoder/data.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/decoder/data2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-3.1.0/tests/test_cases/features/decoder/data3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/features/decoder/data4-mixed.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-3.1.0/tests/test_cases/features/decoder/long-sequence-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/features/decoder/mixed-content.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-3.1.0/tests/test_cases/features/decoder/simple-types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.791483 xmlschema-3.1.0/tests/test_cases/features/derivations/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/complex-extensions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/complex11-restrictions.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/list_types.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/derivations/list_types.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.791483 xmlschema-3.1.0/tests/test_cases/features/elements/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/elements/test_alternatives-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/elements/type_alternatives.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.796483 xmlschema-3.1.0/tests/test_cases/features/models/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/billion_laughs_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/circular_model.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/illegal-attributes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/illegal-declarations.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/illegal-occurs.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/invalid_models1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/invalid_models2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/model1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-3.1.0/tests/test_cases/features/models/models.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/other-ns.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/models/recursive-groups.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-3.1.0/tests/test_cases/features/models/valid_model1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.809483 xmlschema-3.1.0/tests/test_cases/features/namespaces/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/chameleon1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/chameleon2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/chameleon3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/default_ns_invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/default_ns_valid1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/default_ns_valid2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      256 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/dynamic-case1-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/dynamic-case1-overlap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/dynamic-case1-override.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      245 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/dynamic-case1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      448 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/dynamic-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case4-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case4-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case4a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case4b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case5a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case5b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case5c.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case1bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case2bis.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case3.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case4.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case5.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2023-10-18 10:33:30.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case6.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case7.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      466 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case8.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/included3-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/included4-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/included5-valid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/included6-invalid.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/included7-overlap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      355 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/features/namespaces/included8-redefine.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.809483 xmlschema-3.1.0/tests/test_cases/features/patterns/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/features/patterns/patterns.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-3.1.0/tests/test_cases/features/patterns/patterns.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.811483 xmlschema-3.1.0/tests/test_cases/features/wsdl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.749483 xmlschema-3.1.0/tests/test_cases/issues/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.812483 xmlschema-3.1.0/tests/test_cases/issues/issue_008/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_008/issue_008.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_008/issue_008.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.812483 xmlschema-3.1.0/tests/test_cases/issues/issue_009/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_009/issue_009.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.813483 xmlschema-3.1.0/tests/test_cases/issues/issue_013/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_013/issue_013-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_013/issue_013-1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_013/issue_013-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_013/issue_013.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_013/issue_013.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.814483 xmlschema-3.1.0/tests/test_cases/issues/issue_014/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_014/issue014.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.814483 xmlschema-3.1.0/tests/test_cases/issues/issue_018/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_018/issue_018-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_018/issue_018.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.815483 xmlschema-3.1.0/tests/test_cases/issues/issue_022/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_022/README.md
--rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_022/xml_string_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_022/xml_string_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_022/xsd_string.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.816483 xmlschema-3.1.0/tests/test_cases/issues/issue_026/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_026/issue_026-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_026/issue_026-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_026/issue_026-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_026/issue_026.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.816483 xmlschema-3.1.0/tests/test_cases/issues/issue_028/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_028/issue_028-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_028/issue_028-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_028/issue_028.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.817483 xmlschema-3.1.0/tests/test_cases/issues/issue_029/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_029/issue_029-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_029/issue_029-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_029/issue_029-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_029/issue_029.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.817483 xmlschema-3.1.0/tests/test_cases/issues/issue_035/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_035/dates.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_035/dates.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.818483 xmlschema-3.1.0/tests/test_cases/issues/issue_041/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_041/issue_041.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_041/issue_041.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.818483 xmlschema-3.1.0/tests/test_cases/issues/issue_045/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_045/issue_045.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.819483 xmlschema-3.1.0/tests/test_cases/issues/issue_046/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_046/issue_046.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_046/issue_046.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.819483 xmlschema-3.1.0/tests/test_cases/issues/issue_051/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_051/issue_051.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_051/issue_051.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.820483 xmlschema-3.1.0/tests/test_cases/issues/issue_073/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_073/issue_073-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_073/issue_073-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_073/issue_073.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.821483 xmlschema-3.1.0/tests/test_cases/issues/issue_086/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_086/issue_086-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_086/issue_086-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_086/issue_086.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.821483 xmlschema-3.1.0/tests/test_cases/issues/issue_105/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_105/issue_105.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.821483 xmlschema-3.1.0/tests/test_cases/issues/issue_111/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_111/issue_111.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.822483 xmlschema-3.1.0/tests/test_cases/issues/issue_115/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_115/Rotation.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.822483 xmlschema-3.1.0/tests/test_cases/issues/issue_171/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_171/issue_171.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_171/issue_171b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_171/issue_171c.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.823483 xmlschema-3.1.0/tests/test_cases/issues/issue_187/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_187/issue_187_1.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_187/issue_187_2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.823483 xmlschema-3.1.0/tests/test_cases/issues/issue_190/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_190/issue_190.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_190/issue_190.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.824483 xmlschema-3.1.0/tests/test_cases/issues/issue_200/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_200/issue_200.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_200/issue_200.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.825483 xmlschema-3.1.0/tests/test_cases/issues/issue_203/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_203/issue_203.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_203/issue_203.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_203/issue_203alt.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.826483 xmlschema-3.1.0/tests/test_cases/issues/issue_204/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_204/issue_204.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_204/issue_204_1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_204/issue_204_2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_204/issue_204_3.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.827483 xmlschema-3.1.0/tests/test_cases/issues/issue_208/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_208/issue_208.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_208/issue_208.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.828483 xmlschema-3.1.0/tests/test_cases/issues/issue_222/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_222/issue_222.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_222/issue_222.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.828483 xmlschema-3.1.0/tests/test_cases/issues/issue_223/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_223/issue_223.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_223/issue_223.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.746483 xmlschema-3.1.0/tests/test_cases/issues/issue_237/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.829483 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.830483 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
--rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.831483 xmlschema-3.1.0/tests/test_cases/issues/issue_243/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_243/issue_243.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_243/issue_243.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.832483 xmlschema-3.1.0/tests/test_cases/issues/issue_245/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_245/issue_245-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_245/issue_245.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_245/issue_245.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.832483 xmlschema-3.1.0/tests/test_cases/issues/issue_259/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_259/issue_259-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_259/issue_259-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.833483 xmlschema-3.1.0/tests/test_cases/issues/issue_265/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_265/issue_265-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.835483 xmlschema-3.1.0/tests/test_cases/issues/issue_266/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266-2.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.836483 xmlschema-3.1.0/tests/test_cases/issues/issue_273/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_273/issue_273.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_273/issue_273.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.836483 xmlschema-3.1.0/tests/test_cases/issues/issue_276/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_276/dummy.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_276/schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.837483 xmlschema-3.1.0/tests/test_cases/issues/issue_298/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_298/issue_298-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_298/issue_298-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_298/issue_298.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.841483 xmlschema-3.1.0/tests/test_cases/issues/issue_306/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_306/issue_306-invalid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_306/issue_306-valid.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_306/issue_306.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.842483 xmlschema-3.1.0/tests/test_cases/issues/issue_311/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_311/correct_no_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.842483 xmlschema-3.1.0/tests/test_cases/issues/issue_314/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_314/issue_314.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_314/issue_314.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.844483 xmlschema-3.1.0/tests/test_cases/issues/issue_315/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315-1.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315-2.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315-3.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315-4.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315-5.xml
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315_simple.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.844483 xmlschema-3.1.0/tests/test_cases/issues/issue_322/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_322/issue_322.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_322/issue_322.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.846483 xmlschema-3.1.0/tests/test_cases/issues/issue_324/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_324/issue_324-invalid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_324/issue_324-valid.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_324/issue_324.zip
--rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_324/issue_324a.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_324/issue_324b.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.846483 xmlschema-3.1.0/tests/test_cases/issues/issue_334/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_334/issue_334.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_334/issue_334.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_334/issue_334.zip
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.847483 xmlschema-3.1.0/tests/test_cases/issues/issue_341/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_341/issue_341.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_341/issue_341.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.848483 xmlschema-3.1.0/tests/test_cases/issues/issue_349/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_349/issue_349.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_349/issue_349.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.848483 xmlschema-3.1.0/tests/test_cases/issues/issue_362/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.848483 xmlschema-3.1.0/tests/test_cases/issues/issue_362/dir1/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.848483 xmlschema-3.1.0/tests/test_cases/issues/issue_362/dir1/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      433 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_362/dir1/dir2/issue_362_2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      334 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_362/dir1/issue_362_1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.848483 xmlschema-3.1.0/tests/test_cases/issues/issue_362/dir2/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      345 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_362/dir2/issue_362_2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)      816 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_362/issue_362_1.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.850483 xmlschema-3.1.0/tests/test_cases/issues/issue_363/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      352 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_363/issue_363-invalid-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      347 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_363/issue_363-invalid-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_363/issue_363-invalid-3.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      323 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_363/issue_363.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      544 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_363/issue_363.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.850483 xmlschema-3.1.0/tests/test_cases/issues/issue_372/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       60 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_372/issue_372-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       83 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_372/issue_372-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      549 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_372/issue_372.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.851483 xmlschema-3.1.0/tests/test_cases/issues/issue_386/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      371 2024-02-18 21:08:04.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_386/issue_386-1.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      370 2024-02-18 21:08:04.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_386/issue_386-2.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1392 2024-02-18 21:08:04.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_386/issue_386-2.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1402 2024-02-18 21:08:04.000000 xmlschema-3.1.0/tests/test_cases/issues/issue_386/issue_386.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.852483 xmlschema-3.1.0/tests/test_cases/mypy/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-3.1.0/tests/test_cases/mypy/extra_validator.py
--rwxr-xr-x   0 brunato   (1000) brunato   (1000)     3350 2024-03-13 05:27:13.000000 xmlschema-3.1.0/tests/test_cases/mypy/protocols.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-3.1.0/tests/test_cases/mypy/schema_source.py
--rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-3.1.0/tests/test_cases/mypy/simple_types.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.854483 xmlschema-3.1.0/tests/test_cases/resources/
--rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/resources/dummy file.txt
--rw-r--r--   0 brunato   (1000) brunato   (1000)       26 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/resources/dummy file.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/resources/external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/resources/malformed.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/resources/unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/resources/unused_external_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-3.1.0/tests/test_cases/resources/unused_unparsed_entity.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-3.1.0/tests/test_cases/resources/with_entity.xml
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.855483 xmlschema-3.1.0/tests/test_cases/serialization/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4558 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/serialization/abdera.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5473 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/serialization/badgerfish.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3661 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/serialization/document.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5599 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/serialization/jsonml.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2264 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/serialization/parker.json
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6725 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_cases/testfiles
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.750483 xmlschema-3.1.0/tests/test_cases/translations/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.856483 xmlschema-3.1.0/tests/test_cases/translations/pl/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    22092 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6795 2023-07-27 19:52:28.000000 xmlschema-3.1.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11960 2024-03-13 05:27:13.000000 xmlschema-3.1.0/tests/test_cli.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-3.1.0/tests/test_codegen.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    32551 2024-03-13 05:27:13.000000 xmlschema-3.1.0/tests/test_converters.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    28876 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24798 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_documents.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-3.1.0/tests/test_files.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    30639 2024-03-13 05:27:13.000000 xmlschema-3.1.0/tests/test_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    18449 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_locations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5738 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_memory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23506 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_namespaces.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-09-20 10:58:25.000000 xmlschema-3.1.0/tests/test_package.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    58232 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_resources.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-3.1.0/tests/test_schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5976 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/test_translations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2336 2024-03-13 05:27:13.000000 xmlschema-3.1.0/tests/test_typing.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-3.1.0/tests/test_validation.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    27292 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/test_w3c_suite.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-3.1.0/tests/test_wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2024-02-18 21:08:04.000000 xmlschema-3.1.0/tests/test_xpath.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.857483 xmlschema-3.1.0/tests/validation/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.1.0/tests/validation/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    79224 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/validation/test_decoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    33245 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/validation/test_encoding.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    25671 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/validation/test_validation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.864483 xmlschema-3.1.0/tests/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.1.0/tests/validators/__init__.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/validators/test_attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-3.1.0/tests/validators/test_builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34334 2024-02-18 21:08:04.000000 xmlschema-3.1.0/tests/validators/test_complex_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-3.1.0/tests/validators/test_elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16414 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/validators/test_exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    61413 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/validators/test_facets.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2023-10-27 20:18:56.000000 xmlschema-3.1.0/tests/validators/test_global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    15833 2024-02-18 21:08:04.000000 xmlschema-3.1.0/tests/validators/test_groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19335 2023-09-23 04:52:41.000000 xmlschema-3.1.0/tests/validators/test_identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-3.1.0/tests/validators/test_models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/validators/test_notations.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/validators/test_particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    50249 2024-03-13 05:27:13.000000 xmlschema-3.1.0/tests/validators/test_schemas.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/validators/test_simple_types.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-3.1.0/tests/validators/test_wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    37730 2024-01-07 11:20:34.000000 xmlschema-3.1.0/tests/validators/test_xsdbase.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1441 2024-03-13 05:27:13.000000 xmlschema-3.1.0/tox.ini
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.869483 xmlschema-3.1.0/xmlschema/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3027 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5974 2024-02-06 13:53:09.000000 xmlschema-3.1.0/xmlschema/aliases.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11866 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/cli.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.876483 xmlschema-3.1.0/xmlschema/converters/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      865 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/converters/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6640 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/converters/abdera.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6709 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/converters/badgerfish.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7855 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/converters/columnar.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24841 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/converters/default.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7977 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/converters/gdata.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     5271 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/converters/jsonml.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6137 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/converters/parker.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6132 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/converters/unordered.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24831 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/dataobjects.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38425 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/documents.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-3.1.0/xmlschema/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8979 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/exports.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.876483 xmlschema-3.1.0/xmlschema/extras/
--rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-3.1.0/xmlschema/extras/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-3.1.0/xmlschema/extras/codegen.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.752483 xmlschema-3.1.0/xmlschema/extras/templates/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.877483 xmlschema-3.1.0/xmlschema/extras/templates/python/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-3.1.0/xmlschema/extras/templates/python/bindings.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-3.1.0/xmlschema/extras/templates/python/sample.py.jinja
--rw-r--r--   0 brunato   (1000) brunato   (1000)    24452 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/extras/wsdl.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    16302 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-3.1.0/xmlschema/limits.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.754483 xmlschema-3.1.0/xmlschema/locale/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.752483 xmlschema-3.1.0/xmlschema/locale/en/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.877483 xmlschema-3.1.0/xmlschema/locale/en/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-3.1.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    64464 2022-05-20 20:00:14.000000 xmlschema-3.1.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.753483 xmlschema-3.1.0/xmlschema/locale/it/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.878483 xmlschema-3.1.0/xmlschema/locale/it/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-3.1.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-3.1.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.753483 xmlschema-3.1.0/xmlschema/locale/pl/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.879483 xmlschema-3.1.0/xmlschema/locale/pl/LC_MESSAGES/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    47395 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66282 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.754483 xmlschema-3.1.0/xmlschema/locale/ru/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.879483 xmlschema-3.1.0/xmlschema/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-3.1.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-3.1.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9098 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/locations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9432 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/names.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17001 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/namespaces.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-3.1.0/xmlschema/py.typed
--rw-r--r--   0 brunato   (1000) brunato   (1000)    49649 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/resources.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.756483 xmlschema-3.1.0/xmlschema/schemas/
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.880483 xmlschema-3.1.0/xmlschema/schemas/DSIG/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    10447 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4664 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.880483 xmlschema-3.1.0/xmlschema/schemas/HFP/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.880483 xmlschema-3.1.0/xmlschema/schemas/VC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.881483 xmlschema-3.1.0/xmlschema/schemas/WSDL/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/WSDL/soap-encoding.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/WSDL/soap-envelope.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/WSDL/wsdl-soap.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/WSDL/wsdl.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.882483 xmlschema-3.1.0/xmlschema/schemas/XENC/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4360 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/schemas/XENC/xenc-schema-11.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6669 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/schemas/XENC/xenc-schema.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.882483 xmlschema-3.1.0/xmlschema/schemas/XHTML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.882483 xmlschema-3.1.0/xmlschema/schemas/XLINK/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/XLINK/xlink.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.883483 xmlschema-3.1.0/xmlschema/schemas/XML/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/XML/xml_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.883483 xmlschema-3.1.0/xmlschema/schemas/XSD_1.0/
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-3.1.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/XSD_1.0/datatypes.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.884483 xmlschema-3.1.0/xmlschema/schemas/XSD_1.1/
--rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-3.1.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/XSD_1.1/datatypes.xsd
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-3.1.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.884483 xmlschema-3.1.0/xmlschema/schemas/XSI/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-3.1.0/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.886483 xmlschema-3.1.0/xmlschema/testing/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2023-07-27 19:52:28.000000 xmlschema-3.1.0/xmlschema/testing/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31080 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/testing/_builders.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-10-18 10:59:40.000000 xmlschema-3.1.0/xmlschema/testing/_case_class.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-12-19 09:41:12.000000 xmlschema-3.1.0/xmlschema/testing/_factory.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7658 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/testing/_helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-3.1.0/xmlschema/testing/_observers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-3.1.0/xmlschema/translation.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.892483 xmlschema-3.1.0/xmlschema/validators/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     3677 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7277 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/assertions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34229 2024-03-11 14:51:16.000000 xmlschema-3.1.0/xmlschema/validators/attributes.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-3.1.0/xmlschema/validators/builtins.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    46791 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/complex_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    66755 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/elements.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    17432 2024-02-18 21:08:04.000000 xmlschema-3.1.0/xmlschema/validators/exceptions.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    31458 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/facets.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    34011 2024-02-26 17:11:25.000000 xmlschema-3.1.0/xmlschema/validators/global_maps.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    63551 2024-03-10 08:07:35.000000 xmlschema-3.1.0/xmlschema/validators/groups.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     7108 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/helpers.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    19395 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/identities.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    23417 2023-09-23 04:52:41.000000 xmlschema-3.1.0/xmlschema/validators/models.py
--rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-3.1.0/xmlschema/validators/notations.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     6706 2024-01-07 11:20:34.000000 xmlschema-3.1.0/xmlschema/validators/particles.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)   108140 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/schemas.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    61813 2023-11-02 10:56:55.000000 xmlschema-3.1.0/xmlschema/validators/simple_types.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    38026 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/wildcards.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)    43613 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/validators/xsdbase.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.893483 xmlschema-3.1.0/xmlschema/xpath/
--rw-r--r--   0 brunato   (1000) brunato   (1000)      787 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/xpath/__init__.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1072 2024-02-18 21:08:04.000000 xmlschema-3.1.0/xmlschema/xpath/assertion_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1139 2024-02-18 21:08:04.000000 xmlschema-3.1.0/xmlschema/xpath/identity_parser.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     9622 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/xpath/mixin.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     4101 2024-03-13 05:27:13.000000 xmlschema-3.1.0/xmlschema/xpath/proxy.py
--rw-r--r--   0 brunato   (1000) brunato   (1000)     1231 2024-02-13 06:35:18.000000 xmlschema-3.1.0/xmlschema/xpath3.py
-drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-13 05:28:26.894483 xmlschema-3.1.0/xmlschema.egg-info/
--rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-03-13 05:28:26.000000 xmlschema-3.1.0/xmlschema.egg-info/PKG-INFO
--rw-rw-r--   0 brunato   (1000) brunato   (1000)    19926 2024-03-13 05:28:26.000000 xmlschema-3.1.0/xmlschema.egg-info/SOURCES.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2024-03-13 05:28:26.000000 xmlschema-3.1.0/xmlschema.egg-info/dependency_links.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2024-03-13 05:28:26.000000 xmlschema-3.1.0/xmlschema.egg-info/entry_points.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2024-03-13 05:28:26.000000 xmlschema-3.1.0/xmlschema.egg-info/requires.txt
--rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2024-03-13 05:28:26.000000 xmlschema-3.1.0/xmlschema.egg-info/top_level.txt
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.193962 xmlschema-3.2.0/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2023-03-05 21:16:57.000000 xmlschema-3.2.0/.coveragerc
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27699 2024-03-25 21:28:10.000000 xmlschema-3.2.0/CHANGELOG.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1131 2024-01-07 11:20:34.000000 xmlschema-3.2.0/LICENSE
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      330 2023-03-05 20:30:24.000000 xmlschema-3.2.0/MANIFEST.in
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-03-25 21:28:36.192962 xmlschema-3.2.0/PKG-INFO
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6120 2024-02-18 21:08:04.000000 xmlschema-3.2.0/README.rst
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.057961 xmlschema-3.2.0/doc/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      606 2018-09-23 09:23:56.000000 xmlschema-3.2.0/doc/Makefile
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11907 2024-03-25 21:28:10.000000 xmlschema-3.2.0/doc/api.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    11273 2021-08-02 14:12:17.000000 xmlschema-3.2.0/doc/components.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5483 2024-03-25 21:28:10.000000 xmlschema-3.2.0/doc/conf.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5499 2022-06-24 14:13:22.000000 xmlschema-3.2.0/doc/converters.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4841 2022-06-24 14:13:22.000000 xmlschema-3.2.0/doc/extras.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9946 2024-03-25 21:28:10.000000 xmlschema-3.2.0/doc/features.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2021-02-05 09:05:33.000000 xmlschema-3.2.0/doc/index.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-05-28 20:30:12.000000 xmlschema-3.2.0/doc/intro.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       82 2024-02-03 22:44:00.000000 xmlschema-3.2.0/doc/requirements.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5921 2021-04-11 20:19:21.000000 xmlschema-3.2.0/doc/testing.rst
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31284 2024-03-25 21:28:10.000000 xmlschema-3.2.0/doc/usage.rst
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       31 2022-03-07 13:26:41.000000 xmlschema-3.2.0/mypy.ini
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       81 2023-09-23 04:52:41.000000 xmlschema-3.2.0/pyproject.toml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      214 2024-03-13 05:27:13.000000 xmlschema-3.2.0/requirements-dev.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       38 2024-03-25 21:28:36.193962 xmlschema-3.2.0/setup.cfg
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     2765 2024-03-25 21:28:10.000000 xmlschema-3.2.0/setup.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.065961 xmlschema-3.2.0/tests/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-12-03 21:49:59.000000 xmlschema-3.2.0/tests/__init__.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     6753 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/check_memory.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.031961 xmlschema-3.2.0/tests/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.066961 xmlschema-3.2.0/tests/templates/demo/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/demo/demo_type_filter_test.jinja
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.068961 xmlschema-3.2.0/tests/templates/filters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       34 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/filters/name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/filters/namespace_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/filters/python_type_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       35 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/filters/qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       87 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/filters/sort_types_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       39 2021-04-03 19:09:14.000000 xmlschema-3.2.0/tests/templates/filters/type_name_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       40 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/filters/type_qname_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       37 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/templates/filters/unknown_filter_test.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       42 2021-02-05 09:05:33.000000 xmlschema-3.2.0/tests/templates/filters/wrong-template.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3576 2024-03-25 21:28:10.000000 xmlschema-3.2.0/tests/test_all.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.069961 xmlschema-3.2.0/tests/test_cases/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.032961 xmlschema-3.2.0/tests/test_cases/examples/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.072961 xmlschema-3.2.0/tests/test_cases/examples/collection/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      925 2020-05-28 20:30:12.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      884 2022-08-26 15:33:28.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection-default.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1171 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      798 2024-03-25 08:23:51.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      923 2020-05-28 20:30:12.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1599 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      941 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1736 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1938 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1082 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection3bis.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1979 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection3bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1364 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection4.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1743 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1658 2022-08-26 15:33:28.000000 xmlschema-3.2.0/tests/test_cases/examples/collection/collection5.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.074961 xmlschema-3.2.0/tests/test_cases/examples/menù/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      559 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/examples/menù/menù-ascii.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/examples/menù/menù-ascii.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      532 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/examples/menù/menù-cp1252.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      509 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/examples/menù/menù-cp1252.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        3 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/examples/menù/menù.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      542 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/examples/menù/menù.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/examples/menù/menù.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.074961 xmlschema-3.2.0/tests/test_cases/examples/stockquote/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1039 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/examples/stockquote/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/examples/stockquote/stockquote.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1230 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.078961 xmlschema-3.2.0/tests/test_cases/examples/vehicles/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      471 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/bikes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      469 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/cars.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      595 2022-10-01 13:42:01.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      361 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:30.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-1_error.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      468 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-1_error.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      475 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-2_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      386 2020-05-02 09:28:33.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-3_errors.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      491 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-3_errors.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      557 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-max.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-redef.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1666 2020-11-15 16:10:20.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      497 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      543 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      346 2020-05-02 09:28:32.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles2.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      432 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles2.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.033961 xmlschema-3.2.0/tests/test_cases/features/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.078961 xmlschema-3.2.0/tests/test_cases/features/attributes/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      688 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      910 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/attributes/default_attributes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.079961 xmlschema-3.2.0/tests/test_cases/features/builtins/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      584 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/builtins/builtins.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      601 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/builtins/builtins.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.081961 xmlschema-3.2.0/tests/test_cases/features/decoder/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      781 2022-05-20 20:00:14.000000 xmlschema-3.2.0/tests/test_cases/features/decoder/data.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      725 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/decoder/data2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      608 2021-04-01 09:07:37.000000 xmlschema-3.2.0/tests/test_cases/features/decoder/data3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      480 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/features/decoder/data4-mixed.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      691 2021-12-08 19:41:39.000000 xmlschema-3.2.0/tests/test_cases/features/decoder/long-sequence-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      727 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/features/decoder/mixed-content.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5913 2022-05-20 20:00:14.000000 xmlschema-3.2.0/tests/test_cases/features/decoder/simple-types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.084961 xmlschema-3.2.0/tests/test_cases/features/derivations/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1956 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/complex-extensions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      662 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3949 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/complex11-restrictions.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      599 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2051 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1027 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      322 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/list_types.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      675 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/derivations/list_types.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.085961 xmlschema-3.2.0/tests/test_cases/features/elements/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      154 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/elements/test_alternatives-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1487 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1543 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/elements/type_alternatives.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.089961 xmlschema-3.2.0/tests/test_cases/features/models/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5143 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/billion_laughs_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      301 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/circular_model.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      215 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/illegal-attributes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      647 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/illegal-declarations.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      523 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/illegal-occurs.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1192 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/invalid_models1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1541 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/invalid_models2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/model1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4794 2020-04-28 13:28:56.000000 xmlschema-3.2.0/tests/test_cases/features/models/models.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/other-ns.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      760 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/models/recursive-groups.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1062 2020-04-28 13:28:56.000000 xmlschema-3.2.0/tests/test_cases/features/models/valid_model1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.101961 xmlschema-3.2.0/tests/test_cases/features/namespaces/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      151 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/chameleon1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      205 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/chameleon2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      272 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/chameleon3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/default_ns_invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      481 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/default_ns_valid1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      375 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/default_ns_valid2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      256 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/dynamic-case1-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/dynamic-case1-overlap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/dynamic-case1-override.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      245 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/dynamic-case1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      448 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/dynamic-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      566 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      436 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      241 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case4-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      316 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case4-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case4a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      720 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case4b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      365 2022-09-08 10:16:11.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case5a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      377 2022-09-08 10:16:11.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case5b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      379 2022-09-08 10:16:11.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case5c.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      435 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case1bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      541 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case2bis.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      516 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case3.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      490 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case4.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      520 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case5.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      499 2023-10-18 10:33:30.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case6.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case7.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      466 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case8.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      261 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/included3-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      257 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/included4-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      269 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/included5-valid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      211 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/included6-invalid.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      169 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/included7-overlap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      355 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/features/namespaces/included8-redefine.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.102961 xmlschema-3.2.0/tests/test_cases/features/patterns/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      833 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/features/patterns/patterns.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3276 2020-04-07 21:42:10.000000 xmlschema-3.2.0/tests/test_cases/features/patterns/patterns.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.104961 xmlschema-3.2.0/tests/test_cases/features/wsdl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2089 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1477 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example3_types.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1954 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2132 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1962 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2996 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3163 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3414 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.042961 xmlschema-3.2.0/tests/test_cases/issues/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.104961 xmlschema-3.2.0/tests/test_cases/issues/issue_008/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      252 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_008/issue_008.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      533 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_008/issue_008.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.105961 xmlschema-3.2.0/tests/test_cases/issues/issue_009/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      303 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_009/issue_009.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.106961 xmlschema-3.2.0/tests/test_cases/issues/issue_013/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_013/issue_013-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      731 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_013/issue_013-1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      235 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_013/issue_013-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      184 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_013/issue_013.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      801 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_013/issue_013.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.106961 xmlschema-3.2.0/tests/test_cases/issues/issue_014/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      556 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_014/issue014.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.107961 xmlschema-3.2.0/tests/test_cases/issues/issue_018/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      193 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_018/issue_018-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1449 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_018/issue_018.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.108961 xmlschema-3.2.0/tests/test_cases/issues/issue_022/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1048 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_022/README.md
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      130 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_022/xml_string_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      208 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_022/xml_string_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_022/xsd_string.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.109961 xmlschema-3.2.0/tests/test_cases/issues/issue_026/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      229 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_026/issue_026-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      224 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_026/issue_026-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      213 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_026/issue_026-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_026/issue_026.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.109961 xmlschema-3.2.0/tests/test_cases/issues/issue_028/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_028/issue_028-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_028/issue_028-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      353 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_028/issue_028.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.110961 xmlschema-3.2.0/tests/test_cases/issues/issue_029/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      203 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_029/issue_029-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      159 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_029/issue_029-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      181 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_029/issue_029-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      363 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_029/issue_029.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.111961 xmlschema-3.2.0/tests/test_cases/issues/issue_035/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      869 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_035/dates.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1081 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_035/dates.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.111961 xmlschema-3.2.0/tests/test_cases/issues/issue_041/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      247 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_041/issue_041.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      708 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_041/issue_041.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.111961 xmlschema-3.2.0/tests/test_cases/issues/issue_045/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      275 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_045/issue_045.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.112961 xmlschema-3.2.0/tests/test_cases/issues/issue_046/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      354 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_046/issue_046.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      419 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_046/issue_046.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.112961 xmlschema-3.2.0/tests/test_cases/issues/issue_051/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      331 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_051/issue_051.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      824 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_051/issue_051.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.114961 xmlschema-3.2.0/tests/test_cases/issues/issue_073/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      327 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_073/issue_073-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      362 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_073/issue_073-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      685 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_073/issue_073.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.115961 xmlschema-3.2.0/tests/test_cases/issues/issue_086/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_086/issue_086-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      403 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_086/issue_086-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1328 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_086/issue_086.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.115961 xmlschema-3.2.0/tests/test_cases/issues/issue_105/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      515 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_105/issue_105.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.116961 xmlschema-3.2.0/tests/test_cases/issues/issue_111/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      698 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_111/issue_111.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      590 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.116961 xmlschema-3.2.0/tests/test_cases/issues/issue_115/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      620 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_115/Rotation.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.117961 xmlschema-3.2.0/tests/test_cases/issues/issue_171/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      535 2020-03-23 16:13:26.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_171/issue_171.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      580 2020-03-23 16:13:26.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_171/issue_171b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      504 2020-08-14 19:07:25.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_171/issue_171c.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.118961 xmlschema-3.2.0/tests/test_cases/issues/issue_187/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      666 2020-09-25 15:20:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_187/issue_187_1.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      804 2020-09-25 15:20:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_187/issue_187_2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.118961 xmlschema-3.2.0/tests/test_cases/issues/issue_190/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      109 2020-05-28 20:30:12.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_190/issue_190.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      785 2020-05-28 20:30:12.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_190/issue_190.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.119961 xmlschema-3.2.0/tests/test_cases/issues/issue_200/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      310 2020-08-14 19:07:25.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_200/issue_200.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      752 2020-08-14 19:07:25.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_200/issue_200.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.120961 xmlschema-3.2.0/tests/test_cases/issues/issue_203/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      196 2020-09-19 06:08:01.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_203/issue_203.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      960 2020-09-19 06:08:01.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_203/issue_203.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      964 2020-09-19 06:08:01.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_203/issue_203alt.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.121961 xmlschema-3.2.0/tests/test_cases/issues/issue_204/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      524 2020-09-25 15:20:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_204/issue_204.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      172 2020-09-25 15:20:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_204/issue_204_1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      186 2020-09-25 15:20:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_204/issue_204_2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      222 2020-09-25 15:20:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_204/issue_204_3.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.121961 xmlschema-3.2.0/tests/test_cases/issues/issue_208/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      306 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_208/issue_208.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1532 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_208/issue_208.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.122961 xmlschema-3.2.0/tests/test_cases/issues/issue_222/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       66 2021-01-24 21:47:47.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_222/issue_222.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      569 2021-01-24 21:47:47.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_222/issue_222.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.123961 xmlschema-3.2.0/tests/test_cases/issues/issue_223/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       46 2021-01-24 21:47:47.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_223/issue_223.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      392 2021-03-30 11:13:45.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_223/issue_223.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.038961 xmlschema-3.2.0/tests/test_cases/issues/issue_237/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.124961 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      191 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir1/issue_237.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1249 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.127961 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      141 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir2/issue_237a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      314 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir2/issue_237b.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1041 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      664 2021-04-05 21:38:16.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.128961 xmlschema-3.2.0/tests/test_cases/issues/issue_243/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      283 2021-05-03 11:37:57.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_243/issue_243.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2021-05-03 11:37:57.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_243/issue_243.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.128961 xmlschema-3.2.0/tests/test_cases/issues/issue_245/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_245/issue_245-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      757 2021-05-03 11:37:57.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_245/issue_245.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4894 2021-05-03 11:37:57.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_245/issue_245.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.129961 xmlschema-3.2.0/tests/test_cases/issues/issue_259/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     2422 2021-09-02 10:52:43.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_259/issue_259-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1432 2021-09-02 10:52:43.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_259/issue_259-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.130961 xmlschema-3.2.0/tests/test_cases/issues/issue_265/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3471 2021-10-20 14:14:48.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_265/issue_265-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1411 2021-10-20 14:14:48.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      454 2021-10-20 14:14:48.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_265/issue_265-2-override.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.131961 xmlschema-3.2.0/tests/test_cases/issues/issue_266/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      538 2021-10-20 14:14:48.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      158 2021-10-20 14:14:48.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      528 2021-10-20 14:14:48.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266-2.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      651 2021-11-11 15:30:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      551 2021-11-11 15:30:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.132961 xmlschema-3.2.0/tests/test_cases/issues/issue_273/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      299 2021-12-08 19:41:39.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_273/issue_273.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      517 2021-12-08 19:41:39.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_273/issue_273.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.132961 xmlschema-3.2.0/tests/test_cases/issues/issue_276/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      122 2021-12-08 22:11:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_276/dummy.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      495 2021-12-08 22:11:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_276/schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.133961 xmlschema-3.2.0/tests/test_cases/issues/issue_298/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      114 2022-05-22 16:17:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_298/issue_298-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      240 2022-05-22 16:17:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_298/issue_298-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      792 2022-05-22 16:17:24.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_298/issue_298.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.134961 xmlschema-3.2.0/tests/test_cases/issues/issue_306/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      881 2022-06-24 14:13:22.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      203 2022-06-24 14:13:22.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_306/issue_306-invalid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      182 2022-06-24 14:13:22.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_306/issue_306-valid.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      689 2022-06-24 14:13:22.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_306/issue_306.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.134961 xmlschema-3.2.0/tests/test_cases/issues/issue_311/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      786 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_311/correct_no_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      788 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4013 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.135961 xmlschema-3.2.0/tests/test_cases/issues/issue_314/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      267 2022-07-21 09:40:50.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_314/issue_314.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1153 2022-07-21 09:40:50.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_314/issue_314.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.137961 xmlschema-3.2.0/tests/test_cases/issues/issue_315/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       66 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315-1.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       63 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315-2.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315-3.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       76 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315-4.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       71 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315-5.xml
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      604 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      456 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315_simple.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.137961 xmlschema-3.2.0/tests/test_cases/issues/issue_322/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      155 2022-08-26 15:33:28.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_322/issue_322.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      348 2022-08-26 15:33:28.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_322/issue_322.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.138961 xmlschema-3.2.0/tests/test_cases/issues/issue_324/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_324/issue_324-invalid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      373 2022-09-08 10:16:11.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_324/issue_324-valid.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      672 2022-08-28 05:56:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_324/issue_324.zip
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      384 2022-09-08 10:16:11.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_324/issue_324a.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      190 2022-09-08 10:16:11.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_324/issue_324b.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.139961 xmlschema-3.2.0/tests/test_cases/issues/issue_334/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1814 2023-02-11 10:41:50.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_334/issue_334.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5149 2023-02-11 10:41:50.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_334/issue_334.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2663 2023-02-09 09:02:31.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_334/issue_334.zip
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.140961 xmlschema-3.2.0/tests/test_cases/issues/issue_341/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2070 2023-04-14 13:49:05.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      158 2023-04-14 13:49:05.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_341/issue_341.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1781 2023-04-14 13:49:05.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_341/issue_341.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.140961 xmlschema-3.2.0/tests/test_cases/issues/issue_349/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      329 2023-06-14 07:04:00.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_349/issue_349.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      574 2023-06-14 07:04:00.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_349/issue_349.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.140961 xmlschema-3.2.0/tests/test_cases/issues/issue_362/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.141961 xmlschema-3.2.0/tests/test_cases/issues/issue_362/dir1/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.141961 xmlschema-3.2.0/tests/test_cases/issues/issue_362/dir1/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      433 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_362/dir1/dir2/issue_362_2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      334 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_362/dir1/issue_362_1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.141961 xmlschema-3.2.0/tests/test_cases/issues/issue_362/dir2/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      345 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_362/dir2/issue_362_2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      816 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_362/issue_362_1.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.142961 xmlschema-3.2.0/tests/test_cases/issues/issue_363/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      352 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_363/issue_363-invalid-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      347 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_363/issue_363-invalid-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      376 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_363/issue_363-invalid-3.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      323 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_363/issue_363.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      544 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_363/issue_363.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.143961 xmlschema-3.2.0/tests/test_cases/issues/issue_372/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       60 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_372/issue_372-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       83 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_372/issue_372-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      549 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_372/issue_372.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.144961 xmlschema-3.2.0/tests/test_cases/issues/issue_386/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      371 2024-02-18 21:08:04.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_386/issue_386-1.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      370 2024-02-18 21:08:04.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_386/issue_386-2.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1392 2024-02-18 21:08:04.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_386/issue_386-2.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1402 2024-02-18 21:08:04.000000 xmlschema-3.2.0/tests/test_cases/issues/issue_386/issue_386.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.145961 xmlschema-3.2.0/tests/test_cases/mypy/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      911 2022-05-20 16:16:20.000000 xmlschema-3.2.0/tests/test_cases/mypy/extra_validator.py
+-rwxr-xr-x   0 brunato   (1000) brunato   (1000)     3350 2024-03-13 05:27:13.000000 xmlschema-3.2.0/tests/test_cases/mypy/protocols.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)     1905 2023-05-05 12:33:46.000000 xmlschema-3.2.0/tests/test_cases/mypy/schema_source.py
+-rwxrwxr-x   0 brunato   (1000) brunato   (1000)      646 2021-11-11 15:30:24.000000 xmlschema-3.2.0/tests/test_cases/mypy/simple_types.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.148961 xmlschema-3.2.0/tests/test_cases/resources/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       13 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/resources/dummy file.txt
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       26 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/resources/dummy file.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      171 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/resources/external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)       20 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/resources/malformed.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      308 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/resources/unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      170 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/resources/unused_external_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      270 2020-11-08 22:15:33.000000 xmlschema-3.2.0/tests/test_cases/resources/unused_unparsed_entity.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      129 2020-01-23 20:05:17.000000 xmlschema-3.2.0/tests/test_cases/resources/with_entity.xml
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.151961 xmlschema-3.2.0/tests/test_cases/serialization/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4558 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/serialization/abdera.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5473 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/serialization/badgerfish.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3661 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/serialization/document.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5599 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/serialization/jsonml.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2264 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/serialization/parker.json
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6725 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_cases/testfiles
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.042961 xmlschema-3.2.0/tests/test_cases/translations/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.151961 xmlschema-3.2.0/tests/test_cases/translations/pl/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    22092 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6795 2023-07-27 19:52:28.000000 xmlschema-3.2.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11960 2024-03-13 05:27:13.000000 xmlschema-3.2.0/tests/test_cli.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    26576 2023-02-11 10:41:50.000000 xmlschema-3.2.0/tests/test_codegen.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    32551 2024-03-13 05:27:13.000000 xmlschema-3.2.0/tests/test_converters.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    28876 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24798 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_documents.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16654 2024-03-25 21:28:10.000000 xmlschema-3.2.0/tests/test_exports.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3234 2021-02-05 08:47:55.000000 xmlschema-3.2.0/tests/test_files.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    30654 2024-03-25 21:28:10.000000 xmlschema-3.2.0/tests/test_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19738 2024-03-25 21:28:10.000000 xmlschema-3.2.0/tests/test_locations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5738 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_memory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23506 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_namespaces.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4755 2023-09-20 10:58:25.000000 xmlschema-3.2.0/tests/test_package.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    58232 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_resources.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1785 2021-09-02 10:52:43.000000 xmlschema-3.2.0/tests/test_schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5976 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/test_translations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2336 2024-03-13 05:27:13.000000 xmlschema-3.2.0/tests/test_typing.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1806 2021-09-02 10:52:43.000000 xmlschema-3.2.0/tests/test_validation.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    27292 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/test_w3c_suite.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44084 2023-05-18 20:18:16.000000 xmlschema-3.2.0/tests/test_wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15023 2024-02-18 21:08:04.000000 xmlschema-3.2.0/tests/test_xpath.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.152961 xmlschema-3.2.0/tests/validation/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.2.0/tests/validation/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    79224 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/validation/test_decoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    33245 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/validation/test_encoding.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    25671 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/validation/test_validation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.160961 xmlschema-3.2.0/tests/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2020-11-10 10:12:46.000000 xmlschema-3.2.0/tests/validators/__init__.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    25878 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/validators/test_attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14352 2020-12-23 12:38:37.000000 xmlschema-3.2.0/tests/validators/test_builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34334 2024-02-18 21:08:04.000000 xmlschema-3.2.0/tests/validators/test_complex_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     4333 2022-06-24 14:13:22.000000 xmlschema-3.2.0/tests/validators/test_elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16414 2024-01-07 11:20:34.000000 xmlschema-3.2.0/tests/validators/test_exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63262 2024-03-25 21:28:10.000000 xmlschema-3.2.0/tests/validators/test_facets.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     5409 2023-10-27 20:18:56.000000 xmlschema-3.2.0/tests/validators/test_global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    15833 2024-02-18 21:08:04.000000 xmlschema-3.2.0/tests/validators/test_groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19335 2023-09-23 04:52:41.000000 xmlschema-3.2.0/tests/validators/test_identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    52697 2023-04-14 13:49:05.000000 xmlschema-3.2.0/tests/validators/test_models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     3447 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/validators/test_notations.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     8625 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/validators/test_particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    39368 2024-03-25 21:28:10.000000 xmlschema-3.2.0/tests/validators/test_schemas.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    10292 2024-03-23 21:43:51.000000 xmlschema-3.2.0/tests/validators/test_simple_types.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    34302 2022-07-18 14:19:15.000000 xmlschema-3.2.0/tests/validators/test_wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38338 2024-03-25 21:28:10.000000 xmlschema-3.2.0/tests/validators/test_xsdbase.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1441 2024-03-13 05:41:48.000000 xmlschema-3.2.0/tox.ini
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.164961 xmlschema-3.2.0/xmlschema/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3089 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5974 2024-02-06 13:53:09.000000 xmlschema-3.2.0/xmlschema/aliases.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11866 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/cli.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.167961 xmlschema-3.2.0/xmlschema/converters/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      865 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/converters/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6640 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/converters/abdera.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6709 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/converters/badgerfish.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7855 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/converters/columnar.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24841 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/converters/default.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7977 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/converters/gdata.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     5271 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/converters/jsonml.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6137 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/converters/parker.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6132 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/converters/unordered.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24831 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/dataobjects.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38425 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/documents.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1235 2021-10-20 14:14:48.000000 xmlschema-3.2.0/xmlschema/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    14507 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/exports.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.168962 xmlschema-3.2.0/xmlschema/extras/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)        0 2021-02-05 09:05:33.000000 xmlschema-3.2.0/xmlschema/extras/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    21930 2023-05-18 20:18:16.000000 xmlschema-3.2.0/xmlschema/extras/codegen.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.043961 xmlschema-3.2.0/xmlschema/extras/templates/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.169962 xmlschema-3.2.0/xmlschema/extras/templates/python/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      997 2022-07-18 14:19:15.000000 xmlschema-3.2.0/xmlschema/extras/templates/python/bindings.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1116 2021-02-11 14:32:40.000000 xmlschema-3.2.0/xmlschema/extras/templates/python/sample.py.jinja
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    24452 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/extras/wsdl.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    16326 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      677 2020-11-10 10:13:55.000000 xmlschema-3.2.0/xmlschema/limits.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.046961 xmlschema-3.2.0/xmlschema/locale/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.045961 xmlschema-3.2.0/xmlschema/locale/en/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.169962 xmlschema-3.2.0/xmlschema/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    45327 2022-05-20 20:00:14.000000 xmlschema-3.2.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    64464 2024-03-19 14:02:56.000000 xmlschema-3.2.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.046961 xmlschema-3.2.0/xmlschema/locale/it/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.170961 xmlschema-3.2.0/xmlschema/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    47535 2022-05-20 20:00:14.000000 xmlschema-3.2.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    67361 2022-05-20 20:00:14.000000 xmlschema-3.2.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.046961 xmlschema-3.2.0/xmlschema/locale/pl/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.170961 xmlschema-3.2.0/xmlschema/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47395 2023-07-27 19:52:28.000000 xmlschema-3.2.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66282 2023-07-27 19:52:28.000000 xmlschema-3.2.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.047961 xmlschema-3.2.0/xmlschema/locale/ru/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.171962 xmlschema-3.2.0/xmlschema/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    60295 2022-06-11 14:29:39.000000 xmlschema-3.2.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    79497 2022-06-11 14:29:39.000000 xmlschema-3.2.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10643 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/locations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9653 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/names.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17001 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/namespaces.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        0 2021-09-02 10:52:43.000000 xmlschema-3.2.0/xmlschema/py.typed
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    49667 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/resources.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.048961 xmlschema-3.2.0/xmlschema/schemas/
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.171962 xmlschema-3.2.0/xmlschema/schemas/DSIG/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    10447 2023-07-27 19:52:28.000000 xmlschema-3.2.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4664 2023-07-27 19:52:28.000000 xmlschema-3.2.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.172962 xmlschema-3.2.0/xmlschema/schemas/HFP/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1534 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.172962 xmlschema-3.2.0/xmlschema/schemas/VC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      984 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.173961 xmlschema-3.2.0/xmlschema/schemas/WSDL/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19204 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/WSDL/soap-encoding.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6061 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/WSDL/soap-envelope.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6005 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/WSDL/wsdl-soap.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    11900 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/WSDL/wsdl.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.173961 xmlschema-3.2.0/xmlschema/schemas/XENC/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4360 2023-07-27 19:52:28.000000 xmlschema-3.2.0/xmlschema/schemas/XENC/xenc-schema-11.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6669 2023-07-27 19:52:28.000000 xmlschema-3.2.0/xmlschema/schemas/XENC/xenc-schema.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.174961 xmlschema-3.2.0/xmlschema/schemas/XHTML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    65477 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.174961 xmlschema-3.2.0/xmlschema/schemas/XLINK/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8051 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/XLINK/xlink.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.174961 xmlschema-3.2.0/xmlschema/schemas/XML/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1277 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/XML/xml_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.175962 xmlschema-3.2.0/xmlschema/schemas/XSD_1.0/
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    88033 2022-05-20 16:16:20.000000 xmlschema-3.2.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    44301 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/XSD_1.0/datatypes.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.176962 xmlschema-3.2.0/xmlschema/schemas/XSD_1.1/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    67728 2022-09-25 07:58:42.000000 xmlschema-3.2.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17497 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/XSD_1.1/datatypes.xsd
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3767 2022-09-12 09:59:59.000000 xmlschema-3.2.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.176962 xmlschema-3.2.0/xmlschema/schemas/XSI/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      385 2020-11-08 22:15:33.000000 xmlschema-3.2.0/xmlschema/schemas/XSI/XMLSchema-instance_minimal.xsd
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.178962 xmlschema-3.2.0/xmlschema/testing/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2063 2023-07-27 19:52:28.000000 xmlschema-3.2.0/xmlschema/testing/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31080 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/testing/_builders.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7950 2023-10-18 10:59:40.000000 xmlschema-3.2.0/xmlschema/testing/_case_class.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9443 2023-12-19 09:41:12.000000 xmlschema-3.2.0/xmlschema/testing/_factory.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7658 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/testing/_helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4891 2023-05-18 20:18:16.000000 xmlschema-3.2.0/xmlschema/testing/_observers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     2072 2023-02-11 10:41:50.000000 xmlschema-3.2.0/xmlschema/translation.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.185962 xmlschema-3.2.0/xmlschema/validators/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     3677 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/validators/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7277 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/validators/assertions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34229 2024-03-11 14:51:16.000000 xmlschema-3.2.0/xmlschema/validators/attributes.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19881 2022-08-26 15:33:28.000000 xmlschema-3.2.0/xmlschema/validators/builtins.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    47131 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/validators/complex_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    66755 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/validators/elements.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    17432 2024-02-18 21:08:04.000000 xmlschema-3.2.0/xmlschema/validators/exceptions.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    31285 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/validators/facets.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    34011 2024-02-26 17:11:25.000000 xmlschema-3.2.0/xmlschema/validators/global_maps.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    63551 2024-03-10 08:07:35.000000 xmlschema-3.2.0/xmlschema/validators/groups.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     7108 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/validators/helpers.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    19395 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/validators/identities.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    23417 2023-09-23 04:52:41.000000 xmlschema-3.2.0/xmlschema/validators/models.py
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)     1611 2022-05-20 20:00:15.000000 xmlschema-3.2.0/xmlschema/validators/notations.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     6706 2024-01-07 11:20:34.000000 xmlschema-3.2.0/xmlschema/validators/particles.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)   107664 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/validators/schemas.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    62097 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/validators/simple_types.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    38026 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/validators/wildcards.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)    42960 2024-03-25 21:28:10.000000 xmlschema-3.2.0/xmlschema/validators/xsdbase.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.187962 xmlschema-3.2.0/xmlschema/xpath/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)      787 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/xpath/__init__.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1072 2024-02-18 21:08:04.000000 xmlschema-3.2.0/xmlschema/xpath/assertion_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1139 2024-02-18 21:08:04.000000 xmlschema-3.2.0/xmlschema/xpath/identity_parser.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     9622 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/xpath/mixin.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     4101 2024-03-13 05:27:13.000000 xmlschema-3.2.0/xmlschema/xpath/proxy.py
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     1231 2024-02-13 06:35:18.000000 xmlschema-3.2.0/xmlschema/xpath3.py
+drwxr-xr-x   0 brunato   (1000) brunato   (1000)        0 2024-03-25 21:28:36.188962 xmlschema-3.2.0/xmlschema.egg-info/
+-rw-r--r--   0 brunato   (1000) brunato   (1000)     8237 2024-03-25 21:28:35.000000 xmlschema-3.2.0/xmlschema.egg-info/PKG-INFO
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)    19948 2024-03-25 21:28:36.000000 xmlschema-3.2.0/xmlschema.egg-info/SOURCES.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)        1 2024-03-25 21:28:35.000000 xmlschema-3.2.0/xmlschema.egg-info/dependency_links.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      150 2024-03-25 21:28:35.000000 xmlschema-3.2.0/xmlschema.egg-info/entry_points.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)      256 2024-03-25 21:28:35.000000 xmlschema-3.2.0/xmlschema.egg-info/requires.txt
+-rw-rw-r--   0 brunato   (1000) brunato   (1000)       10 2024-03-25 21:28:35.000000 xmlschema-3.2.0/xmlschema.egg-info/top_level.txt
```

### Comparing `xmlschema-3.1.0/CHANGELOG.rst` & `xmlschema-3.2.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 *********
 CHANGELOG
 *********
 
+`v3.2.0`_ (2024-03-25)
+======================
+* Add *download_schemas()* to package API (#387)
+* Fix issue with facets on list types (#396)
+
 `v3.1.0`_ (2024-03-13)
 ======================
 * Add GData converter (issue #388/PR #391)
 * Fix typing protocols usage
 * Extend XSD annotations parsing (issue #366)
 
 `v3.0.2`_ (2024-02-18)
@@ -675,7 +680,8 @@
 .. _v2.4.0: https://github.com/brunato/xmlschema/compare/v2.3.1...v2.4.0
 .. _v2.5.0: https://github.com/brunato/xmlschema/compare/v2.4.0...v2.5.0
 .. _v2.5.1: https://github.com/brunato/xmlschema/compare/v2.5.0...v2.5.1
 .. _v3.0.0: https://github.com/brunato/xmlschema/compare/v2.5.1...v3.0.0
 .. _v3.0.1: https://github.com/brunato/xmlschema/compare/v3.0.0...v3.0.1
 .. _v3.0.2: https://github.com/brunato/xmlschema/compare/v3.0.1...v3.0.2
 .. _v3.1.0: https://github.com/brunato/xmlschema/compare/v3.0.2...v3.1.0
+.. _v3.2.0: https://github.com/brunato/xmlschema/compare/v3.1.0...v3.2.0
```

### Comparing `xmlschema-3.1.0/LICENSE` & `xmlschema-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/PKG-INFO` & `xmlschema-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 3.1.0
+Version: 3.2.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-3.1.0/README.rst` & `xmlschema-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/doc/Makefile` & `xmlschema-3.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/doc/api.rst` & `xmlschema-3.2.0/doc/api.rst`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,15 @@
 
 XML resources API
 =================
 
 .. autofunction:: xmlschema.fetch_resource
 .. autofunction:: xmlschema.fetch_schema_locations
 .. autofunction:: xmlschema.fetch_schema
+.. autofunction:: xmlschema.download_schemas
 
 .. autoclass:: xmlschema.XMLResource
 
     .. autoattribute:: root
     .. autoattribute:: text
     .. autoattribute:: name
     .. autoattribute:: url
```

### Comparing `xmlschema-3.1.0/doc/components.rst` & `xmlschema-3.2.0/doc/components.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/doc/conf.py` & `xmlschema-3.2.0/doc/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 author = 'Davide Brunato'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '3.1'
+version = '3.2'
 # The full version, including alpha/beta/rc tags.
-release = '3.1.0'
+release = '3.2.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 # language = None
```

### Comparing `xmlschema-3.1.0/doc/converters.rst` & `xmlschema-3.2.0/doc/converters.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/doc/extras.rst` & `xmlschema-3.2.0/doc/extras.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/doc/features.rst` & `xmlschema-3.2.0/doc/features.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 added since a specific release. These features are regulated by arguments,
 alternative classes or module parameters.
 
 
 XSD 1.0 and 1.1 support
 =======================
 
-From release v1.0.14 XSD 1.1 support has been added to the library through the class
+Since release v1.0.14 XSD 1.1 support has been added to the library through the class
 :class:`xmlschema.XMLSchema11`. You have to use this class for XSD 1.1 schemas instead the default
 class :class:`xmlschema.XMLSchema`, that is linked to XSD 1.0 validator :class:`xmlschema.XMLSchema10`.
 
 The XSD 1.1 validator can be used also for validating XSD 1.0 schemas, except for a
 restricted set of cases related to content extension in a complexType (the extension
 of a complex content with simple base is allowed in XSD 1.0 and forbidden in XSD 1.1).
```

### Comparing `xmlschema-3.1.0/doc/testing.rst` & `xmlschema-3.2.0/doc/testing.rst`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/doc/usage.rst` & `xmlschema-3.2.0/doc/usage.rst`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,17 @@
 Creating a local copy of a remote XSD schema for offline use
 ------------------------------------------------------------
 
 Sometimes, it is advantageous to validate XML files using an XSD schema located
 at a remote location while also having the option to store the same schema
 locally for offline use.
 
+The first option is to build a schema and then export the XSD sources to a local
+directory:
+
 .. code-block:: py
 
     import xmlschema
     schema = xmlschema.XMLSchema("https://www.omg.org/spec/ReqIF/20110401/reqif.xsd")
     schema.export(target='my_schemas', save_remote=True)
     schema = xmlschema.XMLSchema("my_schemas/reqif.xsd")  # works without internet
 
@@ -153,14 +156,25 @@
 
 becomes
 
 .. code-block:: xml
 
     <xsd:import namespace="http://www.w3.org/1999/xhtml" schemaLocation="my_schemas/www.omg.org/spec/ReqIF/20110402/driver.xsd"/>
 
+The alternative option is to download the XSD resources directly:
+
+.. code-block:: py
+
+    from xmlschema import download_schemas
+    download_schemas("https://www.omg.org/spec/ReqIF/20110401/reqif.xsd", target='my_schemas')
+
+For default the original XSD schemas are not changed and a location map is returned. This map
+is also written to a LOCATION_MAP dictionary in the target directory as the module `__init__.py`,
+so can be used after as *uri_mapper* argument for building the schema instance.
+
 .. note::
 
     Since release v2.5.0 the ``schemaLocation`` attributes are rewritten with
     local paths that don't start with the target directory path, in order to be
     reusable from any working directory. Furthermore for default the residual
     redundant imports from different location hints, are cleaned stripping
     ``schemaLocation`` attributes from them.
```

### Comparing `xmlschema-3.1.0/setup.py` & `xmlschema-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 with Path(__file__).parent.joinpath('README.rst').open() as readme:
     long_description = readme.read()
 
 
 setup(
     name='xmlschema',
-    version='3.1.0',
+    version='3.2.0',
     packages=find_packages(include=['xmlschema*']),
     package_data={
         'xmlschema': ['py.typed', 'locale/**/*.mo', 'locale/**/*.po', 'schemas/*/*.xsd'],
         'xmlschema.extras': ['templates/*/*.jinja'],
     },
     entry_points={
         'console_scripts': [
```

### Comparing `xmlschema-3.1.0/tests/check_memory.py` & `xmlschema-3.2.0/tests/check_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_all.py` & `xmlschema-3.2.0/tests/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             tests.addTests(loader.discover(start_dir=tests_dir, pattern=pattern))
             return tests
 
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_helpers.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_namespaces.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_locations.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_resources.py"))
-        tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_regex.py"))
+        tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_exports.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_xpath.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_cli.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_converters.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_documents.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_dataobjects.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_codegen.py"))
         tests.addTests(loader.discover(start_dir=tests_dir, pattern="test_translations.py"))
```

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection-1_error.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection-1_error.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection-default.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection-default.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection-redef-xmlns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection.py` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection2.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection2.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection3.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection3.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection3bis.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection3bis.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection3bis.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection3bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection4.xml` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection4.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection4.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection4.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/collection/collection5.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/collection/collection5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/menù/menù-ascii.xml` & `xmlschema-3.2.0/tests/test_cases/examples/menù/menù-ascii.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/menù/menù-ascii.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/menù/menù-ascii.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/menù/menù-cp1252.xml` & `xmlschema-3.2.0/tests/test_cases/examples/menù/menù-cp1252.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/menù/menù.xml` & `xmlschema-3.2.0/tests/test_cases/examples/menù/menù.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/stockquote/stockquote.wsdl` & `xmlschema-3.2.0/tests/test_cases/examples/stockquote/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/stockquote/stockquote.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/stockquote/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl` & `xmlschema-3.2.0/tests/test_cases/examples/stockquote/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/vehicles/invalid.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/vehicles/invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-max.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-max.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip` & `xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles-schemas.xsd.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/examples/vehicles/vehicles.xsd` & `xmlschema-3.2.0/tests/test_cases/examples/vehicles/vehicles.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd` & `xmlschema-3.2.0/tests/test_cases/features/attributes/default_attributes-missing_group.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/attributes/default_attributes.xsd` & `xmlschema-3.2.0/tests/test_cases/features/attributes/default_attributes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/builtins/builtins.xml` & `xmlschema-3.2.0/tests/test_cases/features/builtins/builtins.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/builtins/builtins.xsd` & `xmlschema-3.2.0/tests/test_cases/features/builtins/builtins.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/decoder/data.xml` & `xmlschema-3.2.0/tests/test_cases/features/decoder/data.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/decoder/data2.xml` & `xmlschema-3.2.0/tests/test_cases/features/decoder/data2.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/decoder/data3.xml` & `xmlschema-3.2.0/tests/test_cases/features/decoder/data3.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/decoder/long-sequence-1.xsd` & `xmlschema-3.2.0/tests/test_cases/features/decoder/long-sequence-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/decoder/mixed-content.xsd` & `xmlschema-3.2.0/tests/test_cases/features/decoder/mixed-content.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/decoder/simple-types.xsd` & `xmlschema-3.2.0/tests/test_cases/features/decoder/simple-types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/derivations/complex-extensions.xsd` & `xmlschema-3.2.0/tests/test_cases/features/derivations/complex-extensions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd` & `xmlschema-3.2.0/tests/test_cases/features/derivations/complex-with-simple-content-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/derivations/complex11-restrictions.xsd` & `xmlschema-3.2.0/tests/test_cases/features/derivations/complex11-restrictions.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd` & `xmlschema-3.2.0/tests/test_cases/features/derivations/invalid-enumeration-restriction.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd` & `xmlschema-3.2.0/tests/test_cases/features/derivations/invalid-restrictions1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd` & `xmlschema-3.2.0/tests/test_cases/features/derivations/invalid-restrictions2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/derivations/list_types.xsd` & `xmlschema-3.2.0/tests/test_cases/features/derivations/list_types.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd` & `xmlschema-3.2.0/tests/test_cases/features/elements/type_alternatives-no-ns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/elements/type_alternatives.xsd` & `xmlschema-3.2.0/tests/test_cases/features/elements/type_alternatives.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/billion_laughs_model.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/billion_laughs_model.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/illegal-declarations.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/illegal-declarations.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/illegal-occurs.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/illegal-occurs.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/invalid_models1.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/invalid_models1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/invalid_models2.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/invalid_models2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/models.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/models.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/recursive-groups.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/recursive-groups.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/models/valid_model1.xsd` & `xmlschema-3.2.0/tests/test_cases/features/models/valid_model1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case1.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case2.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case4a.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case4a.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/import-case4b.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/import-case4b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case2.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case2bis.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case2bis.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case3.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case3.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/namespaces/include-case5.xsd` & `xmlschema-3.2.0/tests/test_cases/features/namespaces/include-case5.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/patterns/patterns.xml` & `xmlschema-3.2.0/tests/test_cases/features/patterns/patterns.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/patterns/patterns.xsd` & `xmlschema-3.2.0/tests/test_cases/features/patterns/patterns.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example3.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example3_no_types.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example3_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example4.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example4_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example5.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example5_valid.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl` & `xmlschema-3.2.0/tests/test_cases/features/wsdl/wsdl11_example5_with_fault.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_008/issue_008.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_008/issue_008.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_013/issue_013-1.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_013/issue_013-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_013/issue_013.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_013/issue_013.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_014/issue014.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_014/issue014.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_018/issue_018.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_018/issue_018.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_022/README.md` & `xmlschema-3.2.0/tests/test_cases/issues/issue_022/README.md`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_022/xsd_string.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_022/xsd_string.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_026/issue_026.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_026/issue_026.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_035/dates.xml` & `xmlschema-3.2.0/tests/test_cases/issues/issue_035/dates.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_035/dates.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_035/dates.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_041/issue_041.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_041/issue_041.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_051/issue_051.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_051/issue_051.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_073/issue_073.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_073/issue_073.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_086/issue_086.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_086/issue_086.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_105/issue_105.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_105/issue_105.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_111/issue_111.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_111/issue_111.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_111/issue_111_skeleton.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_115/Rotation.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_115/Rotation.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_171/issue_171.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_171/issue_171.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_171/issue_171b.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_171/issue_171b.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_187/issue_187_1.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_187/issue_187_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_187/issue_187_2.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_187/issue_187_2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_190/issue_190.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_190/issue_190.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_200/issue_200.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_200/issue_200.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_203/issue_203.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_203/issue_203.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_203/issue_203alt.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_203/issue_203alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_204/issue_204.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_204/issue_204.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_208/issue_208.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_208/issue_208.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_222/issue_222.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_222/issue_222.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl` & `xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir1/stockquoteservice.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl` & `xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir2/stockquote.wsdl`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_237/dir2/stockquote.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_243/issue_243.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_243/issue_243.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_245/issue_245-valid.xml` & `xmlschema-3.2.0/tests/test_cases/issues/issue_245/issue_245-valid.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_245/issue_245.xml` & `xmlschema-3.2.0/tests/test_cases/issues/issue_245/issue_245.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_245/issue_245.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_245/issue_245.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_259/issue_259-1.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_259/issue_259-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_259/issue_259-2.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_259/issue_259-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_265/issue_265-1.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_265/issue_265-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_265/issue_265-2-invalid.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266-1.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266-2.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266b-1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_266/issue_266b-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_273/issue_273.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_273/issue_273.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_298/issue_298.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_298/issue_298.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_306/issue_306-alt.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_306/issue_306.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_306/issue_306.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_311/correct_no_list.xml` & `xmlschema-3.2.0/tests/test_cases/issues/issue_311/correct_no_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml` & `xmlschema-3.2.0/tests/test_cases/issues/issue_311/incorrect_with_list.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_311/kPartModel_reduit_issue.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_314/issue_314.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_314/issue_314.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_315/issue_315_mixed.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_324/issue_324.zip` & `xmlschema-3.2.0/tests/test_cases/issues/issue_324/issue_324.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_334/issue_334.xml` & `xmlschema-3.2.0/tests/test_cases/issues/issue_334/issue_334.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_334/issue_334.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_334/issue_334.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_334/issue_334.zip` & `xmlschema-3.2.0/tests/test_cases/issues/issue_334/issue_334.zip`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_341/issue_341-ext.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_341/issue_341.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_341/issue_341.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_349/issue_349.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_349/issue_349.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_362/issue_362_1.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_362/issue_362_1.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_363/issue_363.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_363/issue_363.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_372/issue_372.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_372/issue_372.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_386/issue_386-2.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_386/issue_386-2.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/issues/issue_386/issue_386.xsd` & `xmlschema-3.2.0/tests/test_cases/issues/issue_386/issue_386.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/mypy/extra_validator.py` & `xmlschema-3.2.0/tests/test_cases/mypy/extra_validator.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/mypy/protocols.py` & `xmlschema-3.2.0/tests/test_cases/mypy/protocols.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/mypy/schema_source.py` & `xmlschema-3.2.0/tests/test_cases/mypy/schema_source.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/mypy/simple_types.py` & `xmlschema-3.2.0/tests/test_cases/mypy/simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/serialization/abdera.json` & `xmlschema-3.2.0/tests/test_cases/serialization/abdera.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/serialization/badgerfish.json` & `xmlschema-3.2.0/tests/test_cases/serialization/badgerfish.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/serialization/document.xml` & `xmlschema-3.2.0/tests/test_cases/serialization/document.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/serialization/jsonml.json` & `xmlschema-3.2.0/tests/test_cases/serialization/jsonml.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/serialization/parker.json` & `xmlschema-3.2.0/tests/test_cases/serialization/parker.json`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/testfiles` & `xmlschema-3.2.0/tests/test_cases/testfiles`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd` & `xmlschema-3.2.0/tests/test_cases/translations/pl/tw-1(5)8e.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml` & `xmlschema-3.2.0/tests/test_cases/translations/pl/tytul_wykonawczy_niekompletny.xml`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_cli.py` & `xmlschema-3.2.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_codegen.py` & `xmlschema-3.2.0/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_converters.py` & `xmlschema-3.2.0/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_dataobjects.py` & `xmlschema-3.2.0/tests/test_dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_documents.py` & `xmlschema-3.2.0/tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_files.py` & `xmlschema-3.2.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_helpers.py` & `xmlschema-3.2.0/tests/test_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -613,15 +613,15 @@
             self.assertRaises(ValueError, set_logging_level, 'WRONG')
         finally:
             logger.setLevel(current_level)
 
     def test_logged_decorator(self):
         logger = logging.getLogger('xmlschema')
 
-        def func():
+        def func(*args, **kwargs):
             logger.warning('Warning log line')
             logger.info('Info log line')
             logger.debug('Debug log line')
 
         with self.assertLogs('xmlschema', level='DEBUG') as ctx:
             logged(func)(loglevel='ERROR')
             self.assertEqual(logger.level, logging.DEBUG)
```

### Comparing `xmlschema-3.1.0/tests/test_locations.py` & `xmlschema-3.2.0/tests/test_locations.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,29 +4,27 @@
 # All rights reserved.
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
-"""Tests concerning XML resources"""
-
 import unittest
 import os
 import pathlib
 import platform
 
 from urllib.parse import urlsplit, uses_relative
 from pathlib import Path, PurePath, PureWindowsPath, PurePosixPath
 from unittest.mock import patch, MagicMock
 
 import xmlschema.locations
 from xmlschema.locations import LocationPath, LocationPosixPath, LocationWindowsPath, \
     is_url, is_local_url, is_remote_url, url_path_is_file, normalize_url, \
-    normalize_locations
+    normalize_locations, match_location
 
 TEST_CASES_DIR = str(pathlib.Path(__file__).absolute().parent.joinpath('test_cases'))
 
 DRIVE_REGEX = '(/[a-zA-Z]:|/)' if platform.system() == 'Windows' else ''
 
 XML_WITH_NAMESPACES = '<pfa:root xmlns:pfa="http://xmlschema.test/nsa">\n' \
                       '  <pfb:elem xmlns:pfb="http://xmlschema.test/nsb"/>\n' \
@@ -377,14 +375,43 @@
 
         locations = normalize_locations(
             {'tns0': 'alpha', 'tns1': 'http://example.com/beta'}, keep_relative=True
         )
         self.assertListEqual(locations, [('tns0', 'file:alpha'),
                                          ('tns1', 'http://example.com/beta')])
 
+    def test_match_location(self):
+        self.assertIsNone(match_location('schema.xsd', []))
+
+        locations = ['schema1.xsd', 'schema']
+        self.assertIsNone(match_location('schema.xsd', locations))
+
+        locations = ['schema.xsd', 'schema']
+        self.assertEqual(match_location('schema.xsd', locations), 'schema.xsd')
+
+        locations = ['schema', 'schema.xsd']
+        self.assertEqual(match_location('schema.xsd', locations), 'schema.xsd')
+
+        locations = ['../schema.xsd', 'a/schema.xsd']
+        self.assertIsNone(match_location('schema.xsd', locations))
+
+        locations = ['../schema.xsd', 'b/schema.xsd']
+        self.assertEqual(match_location('a/schema.xsd', locations), '../schema.xsd')
+
+        locations = ['../schema.xsd', 'a/schema.xsd']
+        self.assertEqual(match_location('a/schema.xsd', locations), 'a/schema.xsd')
+
+        locations = ['../schema.xsd', './a/schema.xsd']
+        self.assertEqual(match_location('a/schema.xsd', locations), './a/schema.xsd')
+
+        locations = ['/../schema.xsd', '/a/schema.xsd']
+        self.assertIsNone(match_location('a/schema.xsd', locations))
+        self.assertEqual(match_location('/a/schema.xsd', locations), '/a/schema.xsd')
+        self.assertEqual(match_location('/schema.xsd', locations), '/../schema.xsd')
+
 
 if __name__ == '__main__':
-    header_template = "Test xmlschema's locations with Python {} on platform {}"
+    header_template = "Test xmlschema locations.py module with Python {} on platform {}"
     header = header_template.format(platform.python_version(), platform.platform())
     print('{0}\n{1}\n{0}'.format("*" * len(header), header))
 
     unittest.main()
```

### Comparing `xmlschema-3.1.0/tests/test_memory.py` & `xmlschema-3.2.0/tests/test_memory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_namespaces.py` & `xmlschema-3.2.0/tests/test_namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_package.py` & `xmlschema-3.2.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_resources.py` & `xmlschema-3.2.0/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_schemas.py` & `xmlschema-3.2.0/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_translations.py` & `xmlschema-3.2.0/tests/test_translations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_typing.py` & `xmlschema-3.2.0/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_validation.py` & `xmlschema-3.2.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_w3c_suite.py` & `xmlschema-3.2.0/tests/test_w3c_suite.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_wsdl.py` & `xmlschema-3.2.0/tests/test_wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/test_xpath.py` & `xmlschema-3.2.0/tests/test_xpath.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validation/test_decoding.py` & `xmlschema-3.2.0/tests/validation/test_decoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validation/test_encoding.py` & `xmlschema-3.2.0/tests/validation/test_encoding.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validation/test_validation.py` & `xmlschema-3.2.0/tests/validation/test_validation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_attributes.py` & `xmlschema-3.2.0/tests/validators/test_attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_builtins.py` & `xmlschema-3.2.0/tests/validators/test_builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_complex_types.py` & `xmlschema-3.2.0/tests/validators/test_complex_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_elements.py` & `xmlschema-3.2.0/tests/validators/test_elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_exceptions.py` & `xmlschema-3.2.0/tests/validators/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_facets.py` & `xmlschema-3.2.0/tests/validators/test_facets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1139,14 +1139,50 @@
                             <xs:maxLength value="20"/>
                         </xs:restriction>
                     </xs:simpleType>
                 </xs:schema>"""))
 
         self.assertIn("'maxLength' facet value is fixed to 30", str(ec.exception))
 
+    def test_restriction_on_list__issue_396(self):
+        schema = self.schema_class(dedent("""\
+            <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+              <xs:element name="list_of_strings">
+                <xs:simpleType>
+                  <xs:restriction>
+                    <xs:simpleType>
+                      <xs:list>
+                        <xs:simpleType>
+                          <xs:restriction base="xs:string">
+                            <xs:minLength value="5"/>
+                            <xs:maxLength value="6"/>
+                          </xs:restriction>
+                        </xs:simpleType>
+                      </xs:list>
+                    </xs:simpleType>
+                    <xs:minLength value="1"/>
+                    <xs:maxLength value="6"/>
+                  </xs:restriction>
+                </xs:simpleType>
+              </xs:element>
+            </xs:schema>"""))
+
+        self.assertTrue(schema.is_valid('<list_of_strings>abcde</list_of_strings>'))
+        self.assertTrue(schema.is_valid('<list_of_strings>abcdef</list_of_strings>'))
+        self.assertFalse(schema.is_valid('<list_of_strings>abcd</list_of_strings>'))
+        self.assertFalse(schema.is_valid('<list_of_strings>abcdefg</list_of_strings>'))
+        self.assertFalse(schema.is_valid('<list_of_strings>     </list_of_strings>'))
+
+        self.assertTrue(schema.is_valid('<list_of_strings>abcde abcde abcde '
+                                        'abcde abcde abcde</list_of_strings>'))
+        self.assertFalse(schema.is_valid('<list_of_strings>abcde abcde abcde '
+                                         'abcde abcd abcde</list_of_strings>'))
+        self.assertFalse(schema.is_valid('<list_of_strings>abcde abcde abcde '
+                                         'abcde abcde abcde abcde</list_of_strings>'))
+
 
 class TestXsd11Identities(TestXsdFacets):
 
     schema_class = XMLSchema11
 
     def test_explicit_timezone_facet(self):
         schema = self.schema_class(dedent("""\
```

### Comparing `xmlschema-3.1.0/tests/validators/test_global_maps.py` & `xmlschema-3.2.0/tests/validators/test_global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_groups.py` & `xmlschema-3.2.0/tests/validators/test_groups.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_identities.py` & `xmlschema-3.2.0/tests/validators/test_identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_models.py` & `xmlschema-3.2.0/tests/validators/test_models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_notations.py` & `xmlschema-3.2.0/tests/validators/test_notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_particles.py` & `xmlschema-3.2.0/tests/validators/test_particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_schemas.py` & `xmlschema-3.2.0/tests/validators/test_schemas.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,24 +5,20 @@
 # This file is distributed under the terms of the MIT License.
 # See the file 'LICENSE' in the root directory of the present
 # distribution, or http://opensource.org/licenses/MIT.
 #
 # @author Davide Brunato <brunato@sissa.it>
 #
 import unittest
-import filecmp
 import logging
-import tempfile
 import warnings
 import pathlib
 import pickle
 import platform
-import glob
 import os
-import re
 from textwrap import dedent
 from xml.etree.ElementTree import Element
 
 import xmlschema
 from xmlschema import XMLSchemaParseError, XMLSchemaIncludeWarning, XMLSchemaImportWarning
 from xmlschema.names import XML_NAMESPACE, LOCATION_HINTS, SCHEMAS_DIR, XSD_ELEMENT, XSI_TYPE
 from xmlschema.validators import XMLSchemaBase, XMLSchema10, XMLSchema11, \
@@ -679,246 +675,14 @@
         self.assertEqual(len(schema.elements), 2)
 
         # Adding other namespaces do not require rebuild
         schema3 = schema.add_schema(source3, build=True)
         self.assertEqual(len(schema.maps.namespaces['http://xmlschema.test/ns1']), 1)
         self.assertEqual(len(schema3.elements), 1)
 
-    def test_export_errors__issue_187(self):
-        with self.assertRaises(ValueError) as ctx:
-            self.vh_schema.export(target=self.vh_dir)
-
-        self.assertIn("target directory", str(ctx.exception))
-        self.assertIn("is not empty", str(ctx.exception))
-
-        with self.assertRaises(ValueError) as ctx:
-            self.vh_schema.export(target=self.vh_xsd_file)
-
-        self.assertIn("target", str(ctx.exception))
-        self.assertIn("is not a directory", str(ctx.exception))
-
-        with self.assertRaises(ValueError) as ctx:
-            self.vh_schema.export(target=self.vh_xsd_file + '/target')
-
-        self.assertIn("target parent", str(ctx.exception))
-        self.assertIn("is not a directory", str(ctx.exception))
-
-        with tempfile.TemporaryDirectory() as dirname:
-            with self.assertRaises(ValueError) as ctx:
-                self.vh_schema.export(target=dirname + 'subdir/target')
-
-            self.assertIn("target parent directory", str(ctx.exception))
-            self.assertIn("does not exist", str(ctx.exception))
-
-    def test_export_same_directory__issue_187(self):
-        with tempfile.TemporaryDirectory() as dirname:
-            self.vh_schema.export(target=dirname)
-
-            for filename in os.listdir(dirname):
-                with pathlib.Path(dirname).joinpath(filename).open() as fp:
-                    exported_schema = fp.read()
-                with pathlib.Path(self.vh_dir).joinpath(filename).open() as fp:
-                    original_schema = fp.read()
-
-                if platform.system() == 'Windows':
-                    exported_schema = re.sub(r'\s+', '', exported_schema)
-                    original_schema = re.sub(r'\s+', '', original_schema)
-
-                self.assertEqual(exported_schema, original_schema)
-
-        self.assertFalse(os.path.isdir(dirname))
-
-    def test_export_another_directory__issue_187(self):
-        vh_schema_file = self.casepath('issues/issue_187/issue_187_1.xsd')
-        vh_schema = self.schema_class(vh_schema_file)
-
-        with tempfile.TemporaryDirectory() as dirname:
-            vh_schema.export(target=dirname)
-
-            path = pathlib.Path(dirname).joinpath('examples/vehicles/*.xsd')
-            for filename in glob.iglob(pathname=str(path)):
-                with pathlib.Path(dirname).joinpath(filename).open() as fp:
-                    exported_schema = fp.read()
-
-                basename = os.path.basename(filename)
-                with pathlib.Path(self.vh_dir).joinpath(basename).open() as fp:
-                    original_schema = fp.read()
-
-                if platform.system() == 'Windows':
-                    exported_schema = re.sub(r'\s+', '', exported_schema)
-                    original_schema = re.sub(r'\s+', '', original_schema)
-
-                self.assertEqual(exported_schema, original_schema)
-
-            with pathlib.Path(dirname).joinpath('issue_187_1.xsd').open() as fp:
-                exported_schema = fp.read()
-            with open(vh_schema_file) as fp:
-                original_schema = fp.read()
-
-            if platform.system() == 'Windows':
-                exported_schema = re.sub(r'\s+', '', exported_schema)
-                original_schema = re.sub(r'\s+', '', original_schema)
-
-            self.assertNotEqual(exported_schema, original_schema)
-
-            if platform.system() != 'Windows':
-                repl = str(pathlib.Path('file').joinpath(str(self.TEST_CASES_DIR).lstrip('/')))
-                self.assertEqual(
-                    exported_schema,
-                    original_schema.replace('../..', repl)
-                )
-
-            schema_file = pathlib.Path(dirname).joinpath('issue_187_1.xsd')
-            schema = xmlschema.XMLSchema(schema_file)
-            ns_schemas = schema.maps.namespaces['http://example.com/vehicles']
-
-            self.assertEqual(len(ns_schemas), 4)
-            self.assertEqual(ns_schemas[0].name, 'issue_187_1.xsd')
-            self.assertEqual(ns_schemas[1].name, 'cars.xsd')
-            self.assertEqual(ns_schemas[2].name, 'types.xsd')
-            self.assertEqual(ns_schemas[3].name, 'bikes.xsd')
-
-        self.assertFalse(os.path.isdir(dirname))
-
-    @unittest.skipIf(SKIP_REMOTE_TESTS, "Remote networks are not accessible.")
-    def test_export_remote__issue_187(self):
-        vh_schema_file = self.casepath('issues/issue_187/issue_187_2.xsd')
-        vh_schema = self.schema_class(vh_schema_file)
-
-        with tempfile.TemporaryDirectory() as dirname:
-            vh_schema.export(target=dirname)
-
-            with pathlib.Path(dirname).joinpath('issue_187_2.xsd').open() as fp:
-                exported_schema = fp.read()
-            with open(vh_schema_file) as fp:
-                original_schema = fp.read()
-
-            if platform.system() == 'Windows':
-                exported_schema = re.sub(r'\s+', '', exported_schema)
-                original_schema = re.sub(r'\s+', '', original_schema)
-
-            self.assertEqual(exported_schema, original_schema)
-
-        self.assertFalse(os.path.isdir(dirname))
-
-        with tempfile.TemporaryDirectory() as dirname:
-            vh_schema.export(target=dirname, save_remote=True)
-            path = pathlib.Path(dirname).joinpath('brunato/xmlschema/master/tests/test_cases/'
-                                                  'examples/vehicles/*.xsd')
-
-            for filename in glob.iglob(pathname=str(path)):
-                with pathlib.Path(dirname).joinpath(filename).open() as fp:
-                    exported_schema = fp.read()
-
-                basename = os.path.basename(filename)
-                with pathlib.Path(self.vh_dir).joinpath(basename).open() as fp:
-                    original_schema = fp.read()
-                self.assertEqual(exported_schema, original_schema)
-
-            with pathlib.Path(dirname).joinpath('issue_187_2.xsd').open() as fp:
-                exported_schema = fp.read()
-            with open(vh_schema_file) as fp:
-                original_schema = fp.read()
-
-            if platform.system() == 'Windows':
-                exported_schema = re.sub(r'\s+', '', exported_schema)
-                original_schema = re.sub(r'\s+', '', original_schema)
-
-            self.assertNotEqual(exported_schema, original_schema)
-            self.assertNotIn('https://', exported_schema)
-            self.assertEqual(
-                exported_schema,
-                original_schema.replace('https://raw.githubusercontent.com',
-                                        'https/raw.githubusercontent.com')
-            )
-
-            schema_file = pathlib.Path(dirname).joinpath('issue_187_2.xsd')
-            schema = xmlschema.XMLSchema(schema_file)
-            ns_schemas = schema.maps.namespaces['http://example.com/vehicles']
-
-            self.assertEqual(len(ns_schemas), 4)
-            self.assertEqual(ns_schemas[0].name, 'issue_187_2.xsd')
-            self.assertEqual(ns_schemas[1].name, 'cars.xsd')
-            self.assertEqual(ns_schemas[2].name, 'types.xsd')
-            self.assertEqual(ns_schemas[3].name, 'bikes.xsd')
-
-        self.assertFalse(os.path.isdir(dirname))
-
-        # Test with DEBUG logging level
-        with tempfile.TemporaryDirectory() as dirname:
-            with self.assertLogs('xmlschema', level='DEBUG') as ctx:
-                vh_schema.export(target=dirname, save_remote=True, loglevel='DEBUG')
-                self.assertGreater(len(ctx.output), 0)
-                self.assertTrue(any('Write modified XSD' in line for line in ctx.output))
-                self.assertTrue(any('Write unchanged XSD' in line for line in ctx.output))
-
-        self.assertFalse(os.path.isdir(dirname))
-
-    @unittest.skipIf(platform.system() == 'Windows', 'skip, Windows systems save with <CR><LF>')
-    def test_export_other_encoding(self):
-        schema_file = self.casepath('examples/menù/menù.xsd')
-        schema_ascii_file = self.casepath('examples/menù/menù-ascii.xsd')
-        schema_cp1252_file = self.casepath('examples/menù/menù-cp1252.xsd')
-
-        schema = self.schema_class(schema_file)
-        with tempfile.TemporaryDirectory() as dirname:
-            schema.export(target=dirname)
-            exported_schema = pathlib.Path(dirname).joinpath('menù.xsd')
-            self.assertTrue(filecmp.cmp(schema_file, exported_schema))
-            self.assertFalse(filecmp.cmp(schema_ascii_file, exported_schema))
-            self.assertFalse(filecmp.cmp(schema_cp1252_file, exported_schema))
-
-        schema = self.schema_class(schema_ascii_file)
-        with tempfile.TemporaryDirectory() as dirname:
-            schema.export(target=dirname)
-            exported_schema = pathlib.Path(dirname).joinpath('menù-ascii.xsd')
-            self.assertFalse(filecmp.cmp(schema_file, exported_schema))
-            self.assertTrue(filecmp.cmp(schema_ascii_file, exported_schema))
-            self.assertFalse(filecmp.cmp(schema_cp1252_file, exported_schema))
-
-        schema = self.schema_class(schema_cp1252_file)
-        with tempfile.TemporaryDirectory() as dirname:
-            schema.export(target=dirname)
-            exported_schema = pathlib.Path(dirname).joinpath('menù-cp1252.xsd')
-            self.assertFalse(filecmp.cmp(schema_file, exported_schema))
-            self.assertFalse(filecmp.cmp(schema_ascii_file, exported_schema))
-            self.assertTrue(filecmp.cmp(schema_cp1252_file, exported_schema))
-
-    def test_export_more_remote_imports__issue_362(self):
-        schema_file = self.casepath('issues/issue_362/issue_362_1.xsd')
-        with warnings.catch_warnings(record=True):
-            warnings.simplefilter("always")
-            schema = self.schema_class(schema_file)
-
-        self.assertIn('{http://xmlschema.test/tns1}root', schema.maps.elements)
-        self.assertIn('{http://xmlschema.test/tns1}item1', schema.maps.elements)
-        self.assertIn('{http://xmlschema.test/tns2}item2', schema.maps.elements)
-        self.assertIn('{http://xmlschema.test/tns2}item3', schema.maps.elements)
-
-        with tempfile.TemporaryDirectory() as dirname:
-            schema.export(target=dirname)
-
-            exported_files = set(
-                str(x.relative_to(dirname)).replace('\\', '/')
-                for x in pathlib.Path(dirname).glob('**/*.xsd')
-            )
-            self.assertSetEqual(
-                exported_files,
-                {'issue_362_1.xsd', 'dir2/issue_362_2.xsd', 'dir1/issue_362_1.xsd',
-                 'dir1/dir2/issue_362_2.xsd', 'issue_362_1.xsd', 'dir2/issue_362_2.xsd',
-                 'dir1/issue_362_1.xsd', 'dir1/dir2/issue_362_2.xsd'}
-            )
-
-            schema_file = pathlib.Path(dirname).joinpath('issue_362_1.xsd')
-            schema = self.schema_class(schema_file)
-            self.assertIn('{http://xmlschema.test/tns1}root', schema.maps.elements)
-            self.assertIn('{http://xmlschema.test/tns1}item1', schema.maps.elements)
-            self.assertIn('{http://xmlschema.test/tns2}item2', schema.maps.elements)
-            self.assertIn('{http://xmlschema.test/tns2}item3', schema.maps.elements)
-
     def test_pickling_subclassed_schema__issue_263(self):
         cases_dir = pathlib.Path(__file__).parent.parent
         schema_file = cases_dir.joinpath('test_cases/examples/vehicles/vehicles.xsd')
         xml_file = cases_dir.joinpath('test_cases/examples/vehicles/vehicles.xml')
 
         schema = self.CustomXMLSchema(str(schema_file))
         self.assertTrue(schema.is_valid(str(xml_file)))
@@ -936,27 +700,19 @@
         schema = CustomLocalXMLSchema(str(schema_file))
         self.assertTrue(schema.is_valid(str(xml_file)))
 
         with self.assertRaises((pickle.PicklingError, AttributeError)) as ec:
             pickle.dumps(schema)
         self.assertIn("Can't pickle", str(ec.exception))
 
-    def test_deprecated_check_schema_method(self):
+    def test_meta_schema_validation(self):
+        self.assertTrue(self.schema_class.meta_schema.is_valid(self.vh_xsd_file))
 
-        with warnings.catch_warnings(record=True) as ctx:
-            warnings.simplefilter("always")
-
-            self.schema_class.check_schema(self.vh_schema)
-
-            self.assertEqual(len(ctx), 1, "Expected one import warning")
-            self.assertIn("check_schema() class method will be removed in v3.0",
-                          str(ctx[0].message))
-
-        with self.assertRaises(RuntimeError):
-            self.schema_class.meta_schema.check_schema(self.vh_schema)
+        invalid_xsd = self.casepath('examples/vehicles/invalid.xsd')
+        self.assertFalse(self.schema_class.meta_schema.is_valid(invalid_xsd))
 
     def test_default_namespace_mapping__issue_266(self):
         schema_file = self.casepath('issues/issue_266/issue_266b-1.xsd')
         with self.assertRaises(XMLSchemaParseError) as ec:
             self.schema_class(schema_file)
 
         error_message = str(ec.exception)
@@ -1002,14 +758,26 @@
         schema = self.schema_class(dedent("""\
             <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
                 <xs:element name="root"/>
             </xs:schema>"""), use_xpath3=True)
 
         self.assertFalse(schema.use_xpath3)
 
+    def test_xmlns_namespace_forbidden(self):
+        source = dedent("""\
+             <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema"
+                     targetNamespace="http://www.w3.org/2000/xmlns/">
+                 <xs:element name="root"/>
+             </xs:schema>""")
+
+        with self.assertRaises(ValueError) as ctx:
+            self.schema_class(source)
+
+        self.assertIn('http://www.w3.org/2000/xmlns/', str(ctx.exception))
+
 
 class TestXMLSchema11(TestXMLSchema10):
 
     schema_class = XMLSchema11
 
     class CustomXMLSchema(XMLSchema11):
         pass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `xmlschema-3.1.0/tests/validators/test_simple_types.py` & `xmlschema-3.2.0/tests/validators/test_simple_types.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_wildcards.py` & `xmlschema-3.2.0/tests/validators/test_wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/tests/validators/test_xsdbase.py` & `xmlschema-3.2.0/tests/validators/test_xsdbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,14 +348,31 @@
                             <xs:element name="node" targetNamespace=""/>
                         </xs:sequence>
                     </xs:complexType>
                 </xs:element>
             </xs:schema>""")
         self.assertEqual(schema.elements['root'].type.content[0].name, 'node')
 
+    def test_xmlns_namespace_forbidden(self):
+        source = dedent("""\
+          <xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema">
+            <xs:element name="root">
+              <xs:complexType>
+                <xs:sequence>
+                  <xs:element name="node" targetNamespace="http://www.w3.org/2000/xmlns/"/>
+                </xs:sequence>
+              </xs:complexType>
+            </xs:element>
+          </xs:schema>""")
+
+        with self.assertRaises(ValueError) as ctx:
+            XMLSchema11(source)
+
+        self.assertIn('http://www.w3.org/2000/xmlns/', str(ctx.exception))
+
     def test_id_property(self):
         name = '{%s}motorbikes' % self.schema.target_namespace
         elem = ElementTree.Element(XSD_ELEMENT, name=name, id='1999')
         xsd_element = self.FakeElement(elem=elem, name=name, schema=self.schema, parent=None)
         self.assertEqual(xsd_element.id, '1999')
 
     def test_validation_attempted(self):
```

### Comparing `xmlschema-3.1.0/tox.ini` & `xmlschema-3.2.0/tox.ini`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/__init__.py` & `xmlschema-3.2.0/xmlschema/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,40 +18,42 @@
 from .xpath import ElementPathMixin
 from .converters import ElementData, XMLSchemaConverter, \
     UnorderedConverter, ParkerConverter, BadgerFishConverter, \
     AbderaConverter, JsonMLConverter, ColumnarConverter, GDataConverter
 from .dataobjects import DataElement, DataElementConverter, DataBindingConverter
 from .documents import validate, is_valid, iter_errors, iter_decode, \
     to_dict, to_json, to_etree, from_json, XmlDocument
+from .exports import download_schemas
 
 from .validators import (
     XMLSchemaValidatorError, XMLSchemaParseError, XMLSchemaNotBuiltError,
     XMLSchemaModelError, XMLSchemaModelDepthError, XMLSchemaValidationError,
     XMLSchemaDecodeError, XMLSchemaEncodeError, XMLSchemaChildrenValidationError,
     XMLSchemaStopValidation, XMLSchemaIncludeWarning, XMLSchemaImportWarning,
     XMLSchemaTypeTableWarning, XMLSchemaAssertPathWarning, XsdGlobals, XMLSchemaBase,
     XMLSchema, XMLSchema10, XMLSchema11, XsdComponent, XsdType, XsdElement, XsdAttribute
 )
 
-__version__ = '3.1.0'
+__version__ = '3.2.0'
 __author__ = "Davide Brunato"
 __contact__ = "brunato@sissa.it"
 __copyright__ = "Copyright 2016-2024, SISSA"
 __license__ = "MIT"
 __status__ = "Production/Stable"
 
 __all__ = [
     'limits', 'translation', 'XMLSchemaException', 'XMLResourceError',
     'XMLSchemaNamespaceError', 'etree_tostring', 'normalize_url', 'normalize_locations',
     'fetch_resource', 'fetch_namespaces', 'fetch_schema_locations', 'fetch_schema',
     'XMLResource', 'ElementPathMixin', 'ElementData', 'XMLSchemaConverter',
     'UnorderedConverter', 'ParkerConverter', 'BadgerFishConverter', 'GDataConverter',
     'AbderaConverter', 'JsonMLConverter', 'ColumnarConverter', 'DataElement',
-    'DataElementConverter', 'DataBindingConverter', 'validate', 'is_valid', 'iter_errors',
-    'iter_decode', 'to_dict', 'to_json', 'to_etree', 'from_json', 'XmlDocument',
+    'DataElementConverter', 'DataBindingConverter', 'validate', 'is_valid',
+    'iter_errors', 'iter_decode', 'to_dict', 'to_json', 'to_etree', 'from_json',
+    'XmlDocument', 'download_schemas',
     'XMLSchemaValidatorError', 'XMLSchemaParseError', 'XMLSchemaNotBuiltError',
     'XMLSchemaModelError', 'XMLSchemaModelDepthError', 'XMLSchemaValidationError',
     'XMLSchemaDecodeError', 'XMLSchemaEncodeError', 'XMLSchemaChildrenValidationError',
     'XMLSchemaStopValidation', 'XMLSchemaIncludeWarning', 'XMLSchemaImportWarning',
     'XMLSchemaTypeTableWarning', 'XMLSchemaAssertPathWarning',
     'XsdGlobals', 'XMLSchemaBase', 'XMLSchema', 'XMLSchema10', 'XMLSchema11',
     'XsdComponent', 'XsdType', 'XsdElement', 'XsdAttribute',
```

### Comparing `xmlschema-3.1.0/xmlschema/aliases.py` & `xmlschema-3.2.0/xmlschema/aliases.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/cli.py` & `xmlschema-3.2.0/xmlschema/cli.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/__init__.py` & `xmlschema-3.2.0/xmlschema/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/abdera.py` & `xmlschema-3.2.0/xmlschema/converters/abdera.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/badgerfish.py` & `xmlschema-3.2.0/xmlschema/converters/badgerfish.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/columnar.py` & `xmlschema-3.2.0/xmlschema/converters/columnar.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/default.py` & `xmlschema-3.2.0/xmlschema/converters/default.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/gdata.py` & `xmlschema-3.2.0/xmlschema/converters/gdata.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/jsonml.py` & `xmlschema-3.2.0/xmlschema/converters/jsonml.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/parker.py` & `xmlschema-3.2.0/xmlschema/converters/parker.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/converters/unordered.py` & `xmlschema-3.2.0/xmlschema/converters/unordered.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/dataobjects.py` & `xmlschema-3.2.0/xmlschema/dataobjects.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/documents.py` & `xmlschema-3.2.0/xmlschema/documents.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/exceptions.py` & `xmlschema-3.2.0/xmlschema/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/extras/codegen.py` & `xmlschema-3.2.0/xmlschema/extras/codegen.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/extras/templates/python/bindings.py.jinja` & `xmlschema-3.2.0/xmlschema/extras/templates/python/bindings.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/extras/templates/python/sample.py.jinja` & `xmlschema-3.2.0/xmlschema/extras/templates/python/sample.py.jinja`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/extras/wsdl.py` & `xmlschema-3.2.0/xmlschema/extras/wsdl.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/helpers.py` & `xmlschema-3.2.0/xmlschema/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 import re
 import logging
 from collections import Counter
 from decimal import Decimal
 from functools import wraps
 from typing import Any, Callable, Iterable, Iterator, List, MutableMapping, \
-    MutableSequence, Optional, Tuple, Union
+    MutableSequence, Optional, Tuple, TypeVar, Union
 from xml.etree.ElementTree import ParseError
 
 from .exceptions import XMLSchemaValueError, XMLSchemaTypeError
 from .names import XML_NAMESPACE, XSI_SCHEMA_LOCATION, XSI_NONS_SCHEMA_LOCATION
 from .aliases import ElementType, NamespacesType, AtomicValueType, NumericValueType
 from .translation import gettext as _
 
@@ -38,24 +38,27 @@
                 _("{!r} is not a valid loglevel").format(level)
             )
         logger.setLevel(getattr(logging, _level))
     else:
         logger.setLevel(level)
 
 
-def logged(func: Callable[..., Any]) -> Callable[..., Any]:
+RT = TypeVar('RT')
+
+
+def logged(func: Callable[..., RT]) -> Callable[..., RT]:
     """
     A decorator for activating a logging level for a function. The keyword
-    argument 'loglevel' is popped from the keyword arguments and used by the
+    argument 'loglevel' is obtained from the keyword arguments and used by the
     wrapper function to set the logging level of the decorated function and
     to restore the original level after the call.
     """
     @wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Any:
-        loglevel: Optional[Union[int, str]] = kwargs.pop('loglevel', None)
+        loglevel: Optional[Union[int, str]] = kwargs.get('loglevel')
         if loglevel is None:
             return func(*args, **kwargs)
         else:
             current_level = logger.level
             set_logging_level(loglevel)
             try:
                 return func(*args, **kwargs)
```

### Comparing `xmlschema-3.1.0/xmlschema/limits.py` & `xmlschema-3.2.0/xmlschema/limits.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.2.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po` & `xmlschema-3.2.0/xmlschema/locale/en/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.2.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po` & `xmlschema-3.2.0/xmlschema/locale/it/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.2.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po` & `xmlschema-3.2.0/xmlschema/locale/pl/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo` & `xmlschema-3.2.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.mo`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po` & `xmlschema-3.2.0/xmlschema/locale/ru/LC_MESSAGES/xmlschema.po`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/locations.py` & `xmlschema-3.2.0/xmlschema/locations.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 import os.path
 import ntpath
 import posixpath
 import platform
 import string
 from collections.abc import MutableMapping
 from pathlib import Path, PurePath, PurePosixPath, PureWindowsPath
-from typing import Optional
+from typing import Optional, Iterable
 from urllib.parse import urlsplit, urlunsplit, unquote, quote_from_bytes
 
 from .exceptions import XMLSchemaValueError
 from .aliases import NormalizedLocationsType, LocationsType
 
 
 DRIVE_LETTERS = frozenset(string.ascii_letters)
 
 
 class LocationPath(PurePath):
     """
     A version of pathlib.PurePath with an enhanced URI conversion and for
     the normalization of location paths.
 
-    A system independent path normalization without resolution is essential
-    for processing resource locations, so the use or base class internals
-    can be necessary for using pathlib.
+    A system independent path normalization without resolution is essential for
+    processing resource locations, so the use or base class internals can be
+    necessary for using pathlib. Despite the URL path has to be considered
+    case-sensitive (ref. https://www.w3.org/TR/WD-html40-970708/htmlweb.html)
+    this not always happen. On the other hand the initial source is often a
+    filepath, so the better choice is to maintain location paths still related
+    to the operating system.
     """
     _path_module = os.path
 
     def __new__(cls, *args: str) -> 'LocationPath':
         if cls is LocationPath:
             cls = LocationWindowsPath if os.name == 'nt' else LocationPosixPath
         return super().__new__(cls, *args)
@@ -258,7 +262,40 @@
             else:
                 normalized_locations.append((ns, normalize_url(value, base_url, keep_relative)))
     else:
         normalized_locations.extend(
             [(ns, normalize_url(url, base_url, keep_relative)) for ns, url in locations]
         )
     return normalized_locations
+
+
+def match_location(url: str, locations: Iterable[str]) -> Optional[str]:
+    """
+    Match a URL against a group of locations. Give priority to exact matches,
+    then to the match with the highest score after filtering out the locations
+    that are not compatible with provided url. The score of a location path is
+    determined by the number of path levels minus the number of parent steps.
+    If no match is found returns `None`.
+    """
+    def is_compatible(loc: str) -> bool:
+        parts = urlsplit(loc)
+        return not parts.scheme or scheme == parts.scheme and netloc == parts.netloc
+
+    if url in locations:
+        return url
+
+    scheme, netloc = urlsplit(url)[:2]
+    path = LocationPath.from_uri(url).normalize()
+    matching_url = None
+    matching_score = None
+
+    for other_url in filter(is_compatible, locations):
+        other_path = LocationPath.from_uri(other_url).normalize()
+        pattern = other_path.as_posix().replace('..', '*')
+
+        if path.match(pattern):
+            score = pattern.count('/') - pattern.count('*')
+            if matching_score is None or matching_score < score:
+                matching_score = score
+                matching_url = other_url
+
+    return matching_url
```

### Comparing `xmlschema-3.1.0/xmlschema/names.py` & `xmlschema-3.2.0/xmlschema/names.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 
 XSI_NAMESPACE = 'http://www.w3.org/2001/XMLSchema-instance'
 "URI of the XML Schema Instance namespace (xsi)"
 
 XML_NAMESPACE = 'http://www.w3.org/XML/1998/namespace'
 "URI of the XML namespace (xml)"
 
+XMLNS_NAMESPACE = 'http://www.w3.org/2000/xmlns/'
+"""
+Special namespace, reserved for making xmlns declarations with the use of extended
+names. Can't be used as a target namespace for a schema or for its components.
+"""
+
 XHTML_NAMESPACE = 'http://www.w3.org/1999/xhtml'
 XHTML_DATATYPES_NAMESPACE = 'http://www.w3.org/1999/xhtml/datatypes/'
 "URIs of the Extensible Hypertext Markup Language namespace (html)"
 
 XLINK_NAMESPACE = 'http://www.w3.org/1999/xlink'
 "URI of the XML Linking Language (XLink)"
```

### Comparing `xmlschema-3.1.0/xmlschema/namespaces.py` & `xmlschema-3.2.0/xmlschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/resources.py` & `xmlschema-3.2.0/xmlschema/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from collections import deque
 from io import StringIO, BytesIO
 from itertools import zip_longest
 from pathlib import Path
 from typing import cast, Any, AnyStr, Dict, Optional, IO, Iterator, \
     List, MutableMapping, Union, Tuple
 from urllib.request import urlopen
-from urllib.parse import urlsplit
+from urllib.parse import urlsplit, unquote
 from urllib.error import URLError
 
 from elementpath import XPathToken, XPathContext, XPath2Parser, ElementNode, \
     LazyElementNode, DocumentNode, build_lxml_node_tree, build_node_tree
 from elementpath.etree import ElementTree, PyElementTree, SafeXMLParser, etree_tostring
 from elementpath.protocols import LxmlElementProtocol
 
@@ -276,15 +276,15 @@
         return self._text
 
     @property
     def name(self) -> Optional[str]:
         """
         The source name, is `None` if the instance is created from an Element or a string.
         """
-        return None if self._url is None else os.path.basename(self._url)
+        return None if self._url is None else os.path.basename(unquote(self._url))
 
     @property
     def url(self) -> Optional[str]:
         """
         The source URL, `None` if the instance is created from an Element or a string.
         """
         return self._url
```

### Comparing `xmlschema-3.1.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd` & `xmlschema-3.2.0/xmlschema/schemas/DSIG/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd` & `xmlschema-3.2.0/xmlschema/schemas/DSIG/xmldsig11-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd` & `xmlschema-3.2.0/xmlschema/schemas/HFP/XMLSchema-hasFacetAndProperty_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd` & `xmlschema-3.2.0/xmlschema/schemas/VC/XMLSchema-versioning.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/WSDL/soap-encoding.xsd` & `xmlschema-3.2.0/xmlschema/schemas/WSDL/soap-encoding.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/WSDL/soap-envelope.xsd` & `xmlschema-3.2.0/xmlschema/schemas/WSDL/soap-envelope.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/WSDL/wsdl-soap.xsd` & `xmlschema-3.2.0/xmlschema/schemas/WSDL/wsdl-soap.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/WSDL/wsdl.xsd` & `xmlschema-3.2.0/xmlschema/schemas/WSDL/wsdl.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XENC/xenc-schema-11.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XENC/xenc-schema-11.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XENC/xenc-schema.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XENC/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XHTML/xhtml1-strict.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XLINK/xlink.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XLINK/xlink.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XML/xml_minimal.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XML/xml_minimal.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XSD_1.0/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XSD_1.0/datatypes.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XSD_1.0/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XSD_1.1/XMLSchema.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XSD_1.1/datatypes.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XSD_1.1/datatypes.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd` & `xmlschema-3.2.0/xmlschema/schemas/XSD_1.1/xsd11-extra.xsd`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/testing/__init__.py` & `xmlschema-3.2.0/xmlschema/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/testing/_builders.py` & `xmlschema-3.2.0/xmlschema/testing/_builders.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/testing/_case_class.py` & `xmlschema-3.2.0/xmlschema/testing/_case_class.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/testing/_factory.py` & `xmlschema-3.2.0/xmlschema/testing/_factory.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/testing/_helpers.py` & `xmlschema-3.2.0/xmlschema/testing/_helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/testing/_observers.py` & `xmlschema-3.2.0/xmlschema/testing/_observers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/translation.py` & `xmlschema-3.2.0/xmlschema/translation.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/__init__.py` & `xmlschema-3.2.0/xmlschema/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/assertions.py` & `xmlschema-3.2.0/xmlschema/validators/assertions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/attributes.py` & `xmlschema-3.2.0/xmlschema/validators/attributes.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/builtins.py` & `xmlschema-3.2.0/xmlschema/validators/builtins.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/complex_types.py` & `xmlschema-3.2.0/xmlschema/validators/complex_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ..helpers import get_qname, local_name
 
 from .exceptions import XMLSchemaDecodeError
 from .helpers import get_xsd_derivation_attribute
 from .xsdbase import XSD_TYPE_DERIVATIONS, XsdComponent, XsdType, ValidationMixin
 from .attributes import XsdAttributeGroup
 from .assertions import XsdAssert
-from .simple_types import FacetsValueType, XsdSimpleType, XsdUnion
+from .simple_types import FacetsValueType, XsdSimpleType, XsdUnion, XsdAtomic
 from .groups import XsdGroup
 from .wildcards import XsdOpenContent, XsdDefaultOpenContent
 
 XSD_MODEL_GROUP_TAGS = {XSD_GROUP, XSD_SEQUENCE, XSD_ALL, XSD_CHOICE}
 
 
 class XsdComplexType(XsdType, ValidationMixin[Union[ElementType, str, bytes], Any]):
@@ -533,26 +533,29 @@
             return 'simple'
         elif self.mixed:
             return 'mixed'
         else:
             return 'element-only'
 
     @property
+    def root_type(self) -> BaseXsdType:
+        if self.attributes or self.base_type is None:
+            return cast('XsdComplexType', self.maps.types[XSD_ANY_TYPE])
+        else:
+            return self.base_type.root_type
+
+    @property
     def sequence_type(self) -> str:
         if self.is_empty():
             return 'empty-sequence()'
-        elif not self.has_simple_content():
-            st = 'xs:untypedAtomic'
+        elif isinstance(self.content, XsdAtomic):
+            name = self.content.primitive_type.local_name
+            st = 'item()' if name is None else f'xs:{name}'
         else:
-            try:
-                name = self.content.primitive_type.local_name  # type: ignore[union-attr]
-            except AttributeError:
-                st = 'xs:untypedAtomic'
-            else:
-                st = 'item()' if name is None else f'xs:{name}'
+            st = 'xs:untypedAtomic'
 
         return f"{st}{'*' if self.is_emptiable() else '+'}"
 
     @staticmethod
     def is_simple() -> bool:
         return False
 
@@ -598,14 +601,18 @@
             return False
         else:
             return not self.content.mixed
 
     def is_list(self) -> bool:
         return isinstance(self.content, XsdSimpleType) and self.content.is_list()
 
+    def is_dynamic_consistent(self, other: Any) -> bool:
+        return other.name == XSD_ANY_TYPE or self.is_derived(other) or \
+            isinstance(other, XsdUnion) and any(self.is_derived(mt) for mt in other.member_types)
+
     def validate(self, obj: Union[ElementType, str, bytes],
                  use_defaults: bool = True,
                  namespaces: Optional[NamespacesType] = None,
                  max_depth: Optional[int] = None,
                  extra_validator: Optional[ExtraValidatorType] = None) -> None:
         kwargs: Any = {
             'use_defaults': use_defaults,
```

### Comparing `xmlschema-3.1.0/xmlschema/validators/elements.py` & `xmlschema-3.2.0/xmlschema/validators/elements.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/exceptions.py` & `xmlschema-3.2.0/xmlschema/validators/exceptions.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/facets.py` & `xmlschema-3.2.0/xmlschema/validators/facets.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 """
 This module contains declarations and classes for XML Schema constraint facets.
 """
 import re
 import math
 import operator
 from abc import abstractmethod
-from typing import TYPE_CHECKING, cast, Any, List, Optional, Pattern, Union, \
-    MutableSequence, overload, Tuple, Type, Dict
+from typing import TYPE_CHECKING, cast, overload, Any, Dict, List, \
+    MutableSequence, Optional, Pattern, Union, Tuple, Type
 from xml.etree.ElementTree import Element
 
 from elementpath import XPathContext, ElementPathError, \
     translate_pattern, RegexError, ElementNode
 from elementpath.datatypes import AnyAtomicType
 
 from ..names import XSD_LENGTH, XSD_MIN_LENGTH, XSD_MAX_LENGTH, XSD_ENUMERATION, \
@@ -50,28 +50,28 @@
     fixed = False
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
                  parent: Union['XsdList', 'XsdAtomicRestriction'],
                  base_type: Optional[BaseXsdType]) -> None:
         self.base_type = base_type
+        self._validator = self._skip_validation
         super(XsdFacet, self).__init__(elem, schema, parent)
 
     def __repr__(self) -> str:
         return '%s(value=%r, fixed=%r)' % (self.__class__.__name__, self.value, self.fixed)
 
     def __call__(self, value: Any) -> None:
         try:
             self._validator(value)
         except TypeError:
             reason = _("invalid type {!r} provided").format(type(value))
             raise XMLSchemaValidationError(self, value, reason) from None
 
-    @staticmethod
-    def _validator(_: Any) -> None:
+    def _skip_validation(self, value: Any) -> None:
         return
 
     def _parse(self) -> None:
         if 'fixed' in self.elem.attrib and self.elem.attrib['fixed'] in ('true', '1'):
             self.fixed = True
         base_facet = self.base_facet
         self.base_value = None if base_facet is None else base_facet.value
@@ -98,24 +98,24 @@
     @property
     def base_facet(self) -> Optional['XsdFacet']:
         """
         An object of the same type if the instance has a base facet, `None` otherwise.
         """
         base_type: Optional[BaseXsdType] = self.base_type
         tag = self.elem.tag
-        while True:
-            if base_type is None:
-                return None
+        while base_type is not None:
             try:
                 base_facet = base_type.facets[tag]  # type: ignore[union-attr]
             except (AttributeError, KeyError):
                 base_type = base_type.base_type
             else:
-                assert isinstance(base_facet, self.__class__)
+                assert isinstance(base_facet, XsdFacet)
                 return base_facet
+        else:
+            return None
 
 
 class XsdWhiteSpaceFacet(XsdFacet):
     """
     XSD *whiteSpace* facet.
 
     ..  <whiteSpace
@@ -128,19 +128,19 @@
     """
     value: str
     _ADMITTED_TAGS = XSD_WHITE_SPACE,
 
     def _parse_value(self, elem: ElementType) -> None:
         self.value = elem.attrib['value']
         if self.value == 'collapse':
-            self._validator = self.collapse_white_space_validator  # type: ignore[assignment]
+            self._validator = self.collapse_white_space_validator
         elif self.value == 'replace':
             if self.base_value == 'collapse':
                 self.parse_error(_("facet value can be only 'collapse'"))
-            self._validator = self.replace_white_space_validator  # type: ignore[assignment]
+            self._validator = self.replace_white_space_validator
         elif self.base_value == 'collapse':
             self.parse_error(_("facet value can be only 'collapse'"))
         elif self.base_value == 'replace':
             self.parse_error(_("facet value can be only 'replace' or 'collapse'"))
 
     def replace_white_space_validator(self, value: str) -> None:
         if '\t' in value or '\n' in value:
@@ -177,17 +177,17 @@
         if self.base_value is not None and self.value != self.base_value:
             msg = _("base facet has a different length ({})")
             self.parse_error(msg.format(self.base_value))
 
         primitive_type = getattr(self.base_type, 'primitive_type', None)
         if primitive_type is None or primitive_type.name not in {XSD_QNAME, XSD_NOTATION_TYPE}:
             # See: https://www.w3.org/Bugs/Public/show_bug.cgi?id=4009
-            self._validator = self._length_validator  # type: ignore[assignment]
+            self._validator = self.length_validator
 
-    def _length_validator(self, value: Any) -> None:
+    def length_validator(self, value: Any) -> None:
         if len(value) != self.value:
             reason = _("length has to be {!r}").format(self.value)
             raise XMLSchemaValidationError(self, value, reason)
 
 
 class XsdMinLengthFacet(XsdFacet):
     """
@@ -211,17 +211,17 @@
         if self.base_value is not None and self.value < self.base_value:
             msg = _("base facet has a greater min length ({})")
             self.parse_error(msg.format(self.base_value))
 
         primitive_type = getattr(self.base_type, 'primitive_type', None)
         if primitive_type is None or primitive_type.name not in {XSD_QNAME, XSD_NOTATION_TYPE}:
             # See: https://www.w3.org/Bugs/Public/show_bug.cgi?id=4009
-            self._validator = self._min_length_validator  # type: ignore[assignment]
+            self._validator = self.min_length_validator
 
-    def _min_length_validator(self, value: Any) -> None:
+    def min_length_validator(self, value: Any) -> None:
         if len(value) < self.value:
             reason = _("value length cannot be lesser than {!r}").format(self.value)
             raise XMLSchemaValidationError(self, value, reason)
 
 
 class XsdMaxLengthFacet(XsdFacet):
     """
@@ -245,17 +245,17 @@
         if self.base_value is not None and self.value > self.base_value:
             msg = _("base type has a lesser max length ({})")
             self.parse_error(msg.format(self.base_value))
 
         primitive_type = getattr(self.base_type, 'primitive_type', None)
         if primitive_type is None or primitive_type.name not in {XSD_QNAME, XSD_NOTATION_TYPE}:
             # See: https://www.w3.org/Bugs/Public/show_bug.cgi?id=4009
-            self._validator = self._max_length_validator  # type: ignore[assignment]
+            self._validator = self.max_length_validator
 
-    def _max_length_validator(self, value: Any) -> None:
+    def max_length_validator(self, value: Any) -> None:
         if len(value) > self.value:
             reason = _("value length cannot be greater than {!r}").format(self.value)
             raise XMLSchemaValidationError(self, value, reason)
 
 
 class XsdMinInclusiveFacet(XsdFacet):
     """
@@ -505,31 +505,31 @@
     value: str
     base_type: BaseXsdType
     _ADMITTED_TAGS = XSD_EXPLICIT_TIMEZONE,
 
     def _parse_value(self, elem: ElementType) -> None:
         self.value = elem.attrib['value']
         if self.value == 'prohibited':
-            self._validator = self._prohibited_timezone_validator  # type: ignore[assignment]
+            self._validator = self.prohibited_timezone_validator
         elif self.value == 'required':
-            self._validator = self._required_timezone_validator  # type: ignore[assignment]
+            self._validator = self.required_timezone_validator
         elif self.value != 'optional':
             self.value = 'optional'  # Error already detected by meta-schema validation
 
         facet: Any = self.base_type.get_facet(XSD_EXPLICIT_TIMEZONE)
         if facet is not None and facet.value != self.value and facet.value != 'optional':
             msg = _("invalid restriction from {!r}")
             self.parse_error(msg.format(facet.value))
 
-    def _required_timezone_validator(self, value: Any) -> None:
+    def required_timezone_validator(self, value: Any) -> None:
         if value.tzinfo is None:
             reason = _("time zone required for value {!r}").format(self.value)
             raise XMLSchemaValidationError(self, value, reason)
 
-    def _prohibited_timezone_validator(self, value: Any) -> None:
+    def prohibited_timezone_validator(self, value: Any) -> None:
         if value.tzinfo is not None:
             reason = _("time zone prohibited for value {!r}").format(self.value)
             raise XMLSchemaValidationError(self, value, reason)
 
 
 class XsdEnumerationFacets(MutableSequence[ElementType], XsdFacet):
     """
```

### Comparing `xmlschema-3.1.0/xmlschema/validators/global_maps.py` & `xmlschema-3.2.0/xmlschema/validators/global_maps.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/groups.py` & `xmlschema-3.2.0/xmlschema/validators/groups.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/helpers.py` & `xmlschema-3.2.0/xmlschema/validators/helpers.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/identities.py` & `xmlschema-3.2.0/xmlschema/validators/identities.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/models.py` & `xmlschema-3.2.0/xmlschema/validators/models.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/notations.py` & `xmlschema-3.2.0/xmlschema/validators/notations.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/particles.py` & `xmlschema-3.2.0/xmlschema/validators/particles.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/schemas.py` & `xmlschema-3.2.0/xmlschema/validators/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import logging
 import threading
 import warnings
 import re
 import sys
 from copy import copy as _copy, deepcopy
 from operator import attrgetter
+from pathlib import Path
 from typing import cast, Callable, ItemsView, List, Optional, Dict, Any, \
     Set, Union, Tuple, Type, Iterator, Counter
 from xml.etree.ElementTree import Element, ParseError
 
 from elementpath import XPathToken, SchemaElementNode, build_schema_node_tree
 
 from ..exceptions import XMLSchemaTypeError, XMLSchemaKeyError, XMLSchemaRuntimeError, \
@@ -34,21 +35,21 @@
 from ..names import VC_MIN_VERSION, VC_MAX_VERSION, VC_TYPE_AVAILABLE, \
     VC_TYPE_UNAVAILABLE, VC_FACET_AVAILABLE, VC_FACET_UNAVAILABLE, XSD_NOTATION, \
     XSD_ATTRIBUTE, XSD_ATTRIBUTE_GROUP, XSD_GROUP, XSD_SIMPLE_TYPE, XSI_TYPE, \
     XSD_COMPLEX_TYPE, XSD_ELEMENT, XSD_SEQUENCE, XSD_CHOICE, XSD_ALL, XSD_ANY, \
     XSD_ANY_ATTRIBUTE, XSD_ANY_TYPE, XSD_NAMESPACE, XML_NAMESPACE, XSI_NAMESPACE, \
     VC_NAMESPACE, SCHEMAS_DIR, LOCATION_HINTS, XSD_ANNOTATION, XSD_INCLUDE, \
     XSD_IMPORT, XSD_REDEFINE, XSD_OVERRIDE, XSD_DEFAULT_OPEN_CONTENT, \
-    XSD_ANY_SIMPLE_TYPE, XSD_UNION, XSD_LIST, XSD_RESTRICTION
+    XSD_ANY_SIMPLE_TYPE, XSD_UNION, XSD_LIST, XSD_RESTRICTION, XMLNS_NAMESPACE
 from ..aliases import ElementType, XMLSourceType, NamespacesType, LocationsType, \
     SchemaType, SchemaSourceType, ConverterType, ComponentClassType, DecodeType, \
     EncodeType, BaseXsdType, ExtraValidatorType, ValidationHookType, UriMapperType, \
     SchemaGlobalType, FillerType, DepthFillerType, ValueHookType, ElementHookType
 from ..translation import gettext as _
-from ..helpers import set_logging_level, logged, prune_etree, get_namespace, \
+from ..helpers import set_logging_level, prune_etree, get_namespace, \
     get_qname, is_defuse_error
 from ..namespaces import NamespaceResourcesMap, NamespaceMapper, NamespaceView
 from ..locations import is_local_url, is_remote_url, url_path_is_file, \
     normalize_url, normalize_locations
 from ..resources import XMLResource
 from ..converters import XMLSchemaConverter
 from ..xpath import XMLSchemaProxy, ElementPathMixin
@@ -379,14 +380,19 @@
             if '' not in self.namespaces:
                 self.namespaces[''] = namespace
 
         elif '' not in self.namespaces:
             # If not declared map the default namespace to no namespace
             self.namespaces[''] = ''
 
+        if self.target_namespace == XMLNS_NAMESPACE:
+            # https://www.w3.org/TR/xmlschema11-1/#sec-nss-special
+            msg = _(f"The namespace {XMLNS_NAMESPACE} cannot be used as 'targetNamespace'")
+            raise XMLSchemaValueError(msg)
+
         logger.debug("Schema targetNamespace is %r", self.target_namespace)
         logger.debug("Declared namespaces: %r", self.namespaces)
 
         # Parses the schema defaults
         if 'attributeFormDefault' in root.attrib:
             self.attribute_form_default = root.attrib['attributeFormDefault']
 
@@ -999,35 +1005,14 @@
         schema.imports = self.imports.copy()
         schema.includes = self.includes.copy()
         schema.maps = self.maps.copy(validator=schema)
         return schema
 
     __copy__ = copy
 
-    @classmethod
-    def check_schema(cls, schema: SchemaType,
-                     namespaces: Optional[NamespacesType] = None) -> None:
-        """
-        Validates the given schema against the XSD meta-schema (:attr:`meta_schema`).
-
-        :param schema: the schema instance that has to be validated.
-        :param namespaces: is an optional mapping from namespace prefix to URI.
-
-        :raises: :exc:`XMLSchemaValidationError` if the schema is invalid.
-        """
-        if cls.meta_schema is None:
-            raise XMLSchemaRuntimeError(_("meta-schema unavailable for %r") % cls)
-
-        msg = f"check_schema() class method will be removed in v3.0, use " \
-            f"{cls.__name__}.meta_schema instead for validating XSD data."
-        warnings.warn(msg, DeprecationWarning, stacklevel=1)
-
-        for error in cls.meta_schema.iter_errors(schema.source, namespaces=namespaces):
-            raise error
-
     def check_validator(self, validation: str = 'strict') -> None:
         """Checks the status of a schema validator against a validation mode."""
         check_validation_mode(validation)
 
         if self.built:
             pass
         elif self.meta_schema is None:
@@ -1494,34 +1479,35 @@
             defuse=self.defuse,
             timeout=self.timeout,
             uri_mapper=self.uri_mapper,
             build=build,
             use_xpath3=self.use_xpath3,
         )
 
-    def export(self, target: str,
+    def export(self, target: Union[str, Path],
                save_remote: bool = False,
                remove_residuals: bool = True,
                exclude_locations: Optional[List[str]] = None,
-               loglevel: Optional[Union[str, int]] = None) -> None:
+               loglevel: Optional[Union[str, int]] = None) -> Dict[str, str]:
         """
         Exports a schema instance. The schema instance is exported to a
         directory with also the hierarchy of imported/included schemas.
 
         :param target: a path to a local empty directory.
         :param save_remote: if `True` is provided saves also remote schemas.
         :param remove_residuals: for default removes residual remote schema \
         locations from redundant import statements.
         :param exclude_locations: explicitly exclude schema locations from \
         substitution or removal.
         :param loglevel: for setting a different logging level for schema export.
+        :return: a dictionary containing the map of modified locations.
         """
-        logged(export_schema)(
-            obj=self,
-            target_dir=target,
+        return export_schema(
+            schema=self,
+            target=target,
             save_remote=save_remote,
             remove_residuals=remove_residuals,
             exclude_locations=exclude_locations,
             loglevel=loglevel
         )
 
     def version_check(self, elem: ElementType) -> bool:
@@ -2220,15 +2206,15 @@
                         schema = self.get_schema(namespace)
                         xsd_element = schema.find(key, namespaces)
 
         if not isinstance(xsd_element, XsdElement):
             if path is not None:
                 reason = _("the path %r doesn't match any element of the schema!") % path
             else:
-                reason = _("unable to select an element for decoding data, "
+                reason = _("unable to select an element for encoding data, "
                            "provide a valid 'path' argument.")
             raise XMLSchemaEncodeError(self, obj, self.elements, reason, namespaces=namespaces)
         else:
             yield from xsd_element.iter_encode(obj, validation, **kwargs)
 
     def encode(self, obj: Any, path: Optional[str] = None, validation: str = 'strict',
                *args: Any, **kwargs: Any) -> EncodeType[Any]:
@@ -2279,14 +2265,15 @@
       version = token
       xml:lang = language
       {any attributes with non-schema namespace . . .}>
       Content: ((include | import | redefine | annotation)*, (((simpleType | complexType | group |
       attributeGroup) | element | attribute | notation), annotation*)*)
     </schema>
     """
+    meta_schema: XMLSchemaBase
     meta_schema = os.path.join(SCHEMAS_DIR, 'XSD_1.0/XMLSchema.xsd')  # type: ignore
     BASE_SCHEMAS = {
         XML_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XML/xml_minimal.xsd'),
         XSI_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XSI/XMLSchema-instance_minimal.xsd'),
     }
 
 
@@ -2321,14 +2308,15 @@
       version = token
       xml:lang = language
       {any attributes with non-schema namespace . . .}>
       Content: ((include | import | redefine | annotation)*, (((simpleType | complexType | group |
       attributeGroup) | element | attribute | notation), annotation*)*)
     </schema>
     """
+    meta_schema: XMLSchemaBase
     meta_schema = os.path.join(SCHEMAS_DIR, 'XSD_1.1/XMLSchema.xsd')  # type: ignore
     XSD_VERSION = '1.1'
 
     BASE_SCHEMAS = {
         XML_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XML/xml_minimal.xsd'),
         XSI_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XSI/XMLSchema-instance_minimal.xsd'),
         XSD_NAMESPACE: os.path.join(SCHEMAS_DIR, 'XSD_1.1/xsd11-extra.xsd'),
```

### Comparing `xmlschema-3.1.0/xmlschema/validators/simple_types.py` & `xmlschema-3.2.0/xmlschema/validators/simple_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,14 +342,23 @@
         return False
 
     @property
     def content_type_label(self) -> str:
         return 'empty' if self.max_length == 0 else 'simple'
 
     @property
+    def root_type(self) -> BaseXsdType:
+        if self.base_type is None:
+            return self
+        elif isinstance(self.base_type, XsdAtomic):
+            return self.base_type.primitive_type
+        else:
+            return self.base_type.root_type
+
+    @property
     def sequence_type(self) -> str:
         if self.is_empty():
             return 'empty-sequence()'
 
         root_type = self.root_type
         if root_type.name is not None:
             sequence_type = f'xs:{root_type.local_name}'
@@ -783,15 +792,15 @@
     ..  <list
           id = ID
           itemType = QName
           {any attributes with non-schema namespace ...}>
           Content: (annotation?, simpleType?)
         </list>
     """
-    base_type: XsdSimpleType
+    item_type: XsdSimpleType
     _ADMITTED_TAGS = {XSD_LIST}
     _white_space_elem = ElementTree.Element(
         XSD_WHITE_SPACE, attrib={'value': 'collapse', 'fixed': 'true'}
     )
 
     def __init__(self, elem: ElementType,
                  schema: SchemaType,
@@ -800,103 +809,103 @@
         facets: Optional[Dict[Optional[str], FacetsValueType]] = {
             XSD_WHITE_SPACE: XsdWhiteSpaceFacet(self._white_space_elem, schema, self, self)
         }
         super(XsdList, self).__init__(elem, schema, parent, name, facets)
 
     def __repr__(self) -> str:
         if self.name is None:
-            return '%s(item_type=%r)' % (self.__class__.__name__, self.base_type)
+            return '%s(item_type=%r)' % (self.__class__.__name__, self.item_type)
         else:
             return '%s(name=%r)' % (self.__class__.__name__, self.prefixed_name)
 
     def __setattr__(self, name: str, value: Any) -> None:
         if name == 'elem' and value is not None and value.tag != XSD_LIST:
             if value.tag == XSD_SIMPLE_TYPE:
                 for child in value:
                     if child.tag == XSD_LIST:
                         super(XsdList, self).__setattr__(name, child)
                         return
             raise XMLSchemaValueError(
                 "a {0!r} definition required for {1!r}".format(XSD_LIST, self)
             )
-        elif name == 'base_type':
+        elif name == 'item_type':
             if not value.is_atomic():
                 raise XMLSchemaValueError(
-                    _("%r: a list must be based on atomic data types") % self
+                    _("%r: a list must be based on atomic data types") % value
                 )
         elif name == 'white_space' and value is None:
             value = 'collapse'
         super(XsdList, self).__setattr__(name, value)
 
     def _parse(self) -> None:
-        base_type: Any
+        item_type: Any
 
         child = self._parse_child_component(self.elem)
         if child is not None:
             # Case of a local simpleType declaration inside the list tag
             try:
-                base_type = self.schema.simple_type_factory(child, parent=self)
+                item_type = self.schema.simple_type_factory(child, parent=self)
             except XMLSchemaParseError as err:
                 self.parse_error(err)
-                base_type = self.any_atomic_type
+                item_type = self.any_atomic_type
 
             if 'itemType' in self.elem.attrib:
                 self.parse_error(_("ambiguous list type declaration"))
 
         else:
             # List tag with itemType attribute that refers to a global type
             try:
                 item_qname = self.schema.resolve_qname(self.elem.attrib['itemType'])
             except (KeyError, ValueError, RuntimeError) as err:
                 if 'itemType' not in self.elem.attrib:
                     self.parse_error(_("missing list type declaration"))
                 else:
                     self.parse_error(err)
-                base_type = self.any_atomic_type
+                item_type = self.any_atomic_type
             else:
                 try:
-                    base_type = self.maps.lookup_type(item_qname)
+                    item_type = self.maps.lookup_type(item_qname)
                 except KeyError:
                     msg = _("unknown type {!r}")
                     self.parse_error(msg.format(self.elem.attrib['itemType']))
-                    base_type = self.any_atomic_type
+                    item_type = self.any_atomic_type
                 else:
-                    if isinstance(base_type, tuple):
+                    if isinstance(item_type, tuple):
                         msg = _("circular definition found for type {!r}")
                         self.parse_error(msg.format(item_qname))
-                        base_type = self.any_atomic_type
+                        item_type = self.any_atomic_type
 
-        if base_type.final == '#all' or 'list' in base_type.final:
+        if item_type.final == '#all' or 'list' in item_type.final:
             msg = _("'final' value of the itemType %r forbids derivation by list")
-            self.parse_error(msg % base_type)
+            self.parse_error(msg % item_type)
 
-        if base_type.name == XSD_ANY_ATOMIC_TYPE:
+        if item_type.name == XSD_ANY_ATOMIC_TYPE:
             msg = _("cannot use xs:anyAtomicType as base type of a user-defined type")
             self.parse_error(msg)
 
         try:
-            self.base_type = base_type
+            self.item_type = item_type
         except XMLSchemaValueError as err:
             self.parse_error(err)
-            self.base_type = self.any_atomic_type
+            self.item_type = self.any_atomic_type
         else:
-            if not base_type.allow_empty and self.min_length != 0:
+            if not item_type.allow_empty and self.min_length != 0:
                 self.allow_empty = False
 
     @property
     def variety(self) -> Optional[str]:
         return 'list'
 
     @property
     def admitted_facets(self) -> Set[str]:
         return XSD_10_LIST_FACETS if self.xsd_version == '1.0' else XSD_11_LIST_FACETS
 
     @property
-    def item_type(self) -> BaseXsdType:
-        return self.base_type
+    def root_type(self) -> BaseXsdType:
+        return self.item_type.root_type
 
     def is_atomic(self) -> bool:
         return False
 
     def is_list(self) -> bool:
         return True
 
@@ -907,33 +916,33 @@
         elif isinstance(other, tuple):
             other[1].parse_error(f"global type {other[0].tag!r} is not built")
             return False
         elif derivation and self.derivation and derivation != self.derivation:
             return False
         elif other.name in self._special_types:
             return derivation != 'extension'
-        elif self.base_type is other:
+        elif self.item_type is other:
             return True
         else:
             return False
 
     def iter_components(self, xsd_classes: ComponentClassType = None) \
             -> Iterator[XsdComponent]:
         if xsd_classes is None or isinstance(self, xsd_classes):
             yield self
-        if self.base_type.parent is not None:
-            yield from self.base_type.iter_components(xsd_classes)
+        if self.item_type.parent is not None:
+            yield from self.item_type.iter_components(xsd_classes)
 
     def iter_decode(self, obj: Union[str, bytes],
                     validation: str = 'lax', **kwargs: Any) \
             -> IterDecodeType[Union[XMLSchemaValidationError,
                               List[Optional[AtomicValueType]]]]:
         items = []
         for chunk in self.normalize(obj).split():
-            for result in self.base_type.iter_decode(chunk, validation, **kwargs):
+            for result in self.item_type.iter_decode(chunk, validation, **kwargs):
                 if isinstance(result, XMLSchemaValidationError):
                     yield result
                 else:
                     assert not isinstance(result, list)
                     items.append(result)
         else:
             yield items
@@ -941,15 +950,15 @@
     def iter_encode(self, obj: Any, validation: str = 'lax', **kwargs: Any) \
             -> IterEncodeType[EncodedValueType]:
         if not hasattr(obj, '__iter__') or isinstance(obj, (str, bytes)):
             obj = [obj]
 
         encoded_items: List[Any] = []
         for item in obj:
-            for result in self.base_type.iter_encode(item, validation, **kwargs):
+            for result in self.item_type.iter_encode(item, validation, **kwargs):
                 if isinstance(result, XMLSchemaValidationError):
                     yield result
                 else:
                     encoded_items.append(result)
 
         yield ' '.join(item for item in encoded_items if item is not None)
```

### Comparing `xmlschema-3.1.0/xmlschema/validators/wildcards.py` & `xmlschema-3.2.0/xmlschema/validators/wildcards.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/validators/xsdbase.py` & `xmlschema-3.2.0/xmlschema/validators/xsdbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from elementpath import select
 from elementpath.etree import etree_tostring
 
 from ..exceptions import XMLSchemaValueError, XMLSchemaTypeError
 from ..names import XSD_ANNOTATION, XSD_APPINFO, XSD_DOCUMENTATION, \
     XSD_ANY_TYPE, XSD_ANY_SIMPLE_TYPE, XSD_ANY_ATOMIC_TYPE, XSD_ID, \
-    XSD_QNAME, XSD_OVERRIDE, XSD_NOTATION_TYPE, XSD_DECIMAL
+    XSD_QNAME, XSD_OVERRIDE, XSD_NOTATION_TYPE, XSD_DECIMAL, XMLNS_NAMESPACE
 from ..aliases import ElementType, NamespacesType, SchemaType, BaseXsdType, \
     ComponentClassType, ExtraValidatorType, DecodeType, IterDecodeType, \
     EncodeType, IterEncodeType
 from ..translation import gettext as _
 from ..helpers import get_qname, local_name, get_prefixed_qname, \
     is_etree_element, is_etree_document
 from ..resources import XMLResource
@@ -480,14 +480,19 @@
         """
         XSD 1.1 targetNamespace attribute in elements and attributes declarations.
         """
         if 'targetNamespace' not in self.elem.attrib:
             return
 
         self._target_namespace = self.elem.attrib['targetNamespace'].strip()
+        if self._target_namespace == XMLNS_NAMESPACE:
+            # https://www.w3.org/TR/xmlschema11-1/#sec-nss-special
+            msg = _(f"The namespace {XMLNS_NAMESPACE} cannot be used as 'targetNamespace'")
+            raise XMLSchemaValueError(msg)
+
         if 'name' not in self.elem.attrib:
             msg = _("attribute 'name' must be present when "
                     "'targetNamespace' attribute is provided")
             self.parse_error(msg)
         if 'form' in self.elem.attrib:
             msg = _("attribute 'form' must be absent when "
                     "'targetNamespace' attribute is provided")
@@ -782,32 +787,15 @@
     @property
     def root_type(self) -> BaseXsdType:
         """
         The root type of the type definition hierarchy. For an atomic type
         is the primitive type. For a list is the primitive type of the item.
         For a union is the base union type. For a complex type is xs:anyType.
         """
-        if getattr(self, 'attributes', None):
-            return cast('XsdComplexType', self.maps.types[XSD_ANY_TYPE])
-        elif self.base_type is None:
-            if self.is_simple():
-                return cast('XsdSimpleType', self)
-            return cast('XsdComplexType', self.maps.types[XSD_ANY_TYPE])
-
-        primitive_type: BaseXsdType
-        try:
-            if self.base_type.is_simple():
-                primitive_type = self.base_type.primitive_type  # type: ignore[union-attr]
-            else:
-                primitive_type = self.base_type.content.primitive_type  # type: ignore[union-attr]
-        except AttributeError:
-            # The type has complex or XsdList content
-            return self.base_type.root_type
-        else:
-            return primitive_type
+        raise NotImplementedError()
 
     @property
     def simple_type(self) -> Optional['XsdSimpleType']:
         """
         Property that is the instance itself for a simpleType. For a
         complexType is the instance's *content* if this is a simpleType
         or `None` if the instance's *content* is a model group.
@@ -912,17 +900,15 @@
         if not block:
             return False
 
         _block = {x for x in block.split() if x in ('extension', 'restriction')}
         return any(self.is_derived(xsd_type, derivation) for derivation in _block)
 
     def is_dynamic_consistent(self, other: Any) -> bool:
-        return other.name == XSD_ANY_TYPE or self.is_derived(other) or \
-            hasattr(other, 'member_types') and \
-            any(self.is_derived(mt) for mt in other.member_types)  # pragma: no cover
+        raise NotImplementedError()
 
     def is_key(self) -> bool:
         return self.name == XSD_ID or self.is_derived(self.maps.types[XSD_ID])
 
     def is_qname(self) -> bool:
         return self.name == XSD_QNAME or self.is_derived(self.maps.types[XSD_QNAME])
```

### Comparing `xmlschema-3.1.0/xmlschema/xpath/__init__.py` & `xmlschema-3.2.0/xmlschema/xpath/__init__.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/xpath/assertion_parser.py` & `xmlschema-3.2.0/xmlschema/xpath/assertion_parser.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/xpath/identity_parser.py` & `xmlschema-3.2.0/xmlschema/xpath/identity_parser.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/xpath/mixin.py` & `xmlschema-3.2.0/xmlschema/xpath/mixin.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/xpath/proxy.py` & `xmlschema-3.2.0/xmlschema/xpath/proxy.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema/xpath3.py` & `xmlschema-3.2.0/xmlschema/xpath3.py`

 * *Files identical despite different names*

### Comparing `xmlschema-3.1.0/xmlschema.egg-info/PKG-INFO` & `xmlschema-3.2.0/xmlschema.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmlschema
-Version: 3.1.0
+Version: 3.2.0
 Summary: An XML Schema validator and decoder
 Home-page: https://github.com/sissaschool/xmlschema
 Author: Davide Brunato
 Author-email: brunato@sissa.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `xmlschema-3.1.0/xmlschema.egg-info/SOURCES.txt` & `xmlschema-3.2.0/xmlschema.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 tests/check_memory.py
 tests/test_all.py
 tests/test_cli.py
 tests/test_codegen.py
 tests/test_converters.py
 tests/test_dataobjects.py
 tests/test_documents.py
+tests/test_exports.py
 tests/test_files.py
 tests/test_helpers.py
 tests/test_locations.py
 tests/test_memory.py
 tests/test_namespaces.py
 tests/test_package.py
 tests/test_resources.py
```

