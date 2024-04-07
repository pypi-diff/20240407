# Comparing `tmp/discovery-capability-0.9.5.tar.gz` & `tmp/discovery-capability-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-capability-0.9.5.tar", last modified: Sun Sep 24 22:21:33 2023, max compression
+gzip compressed data, was "discovery-capability-0.9.6.tar", last modified: Mon Sep 25 14:37:08 2023, max compression
```

## Comparing `discovery-capability-0.9.5.tar` & `discovery-capability-0.9.6.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.281681 discovery-capability-0.9.5/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.9.5/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.9.5/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-09-24 22:21:33.282135 discovery-capability-0.9.5/PKG-INFO
--rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.9.5/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.101091 discovery-capability-0.9.5/discovery_capability.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-09-24 22:21:32.000000 discovery-capability-0.9.5/discovery_capability.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     3140 2023-09-24 22:21:33.000000 discovery-capability-0.9.5/discovery_capability.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-09-24 22:21:32.000000 discovery-capability-0.9.5/discovery_capability.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       96 2023-09-24 22:21:32.000000 discovery-capability-0.9.5/discovery_capability.egg-info/requires.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-09-24 22:21:32.000000 discovery-capability-0.9.5/discovery_capability.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.101551 discovery-capability-0.9.5/ds_capability/
--rw-r--r--   0 doatridge   (503) staff       (20)      373 2023-09-23 23:09:45.000000 discovery-capability-0.9.5/ds_capability/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.109501 discovery-capability-0.9.5/ds_capability/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.9.5/ds_capability/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15105 2023-09-17 21:58:10.000000 discovery-capability-0.9.5/ds_capability/components/abstract_common_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3400 2023-09-23 21:15:41.000000 discovery-capability-0.9.5/ds_capability/components/commons.py
--rw-r--r--   0 doatridge   (503) staff       (20)    27164 2023-09-10 14:58:03.000000 discovery-capability-0.9.5/ds_capability/components/controller.py
--rw-r--r--   0 doatridge   (503) staff       (20)    26443 2023-09-19 17:14:53.000000 discovery-capability-0.9.5/ds_capability/components/discovery.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5213 2023-09-11 16:43:46.000000 discovery-capability-0.9.5/ds_capability/components/feature_build.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5229 2023-09-11 16:43:46.000000 discovery-capability-0.9.5/ds_capability/components/feature_select.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5177 2023-09-12 13:31:59.000000 discovery-capability-0.9.5/ds_capability/components/feature_transform.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.112007 discovery-capability-0.9.5/ds_capability/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.9.5/ds_capability/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2507 2023-09-24 20:11:52.000000 discovery-capability-0.9.5/ds_capability/handlers/duckdb_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6191 2023-08-26 18:24:33.000000 discovery-capability-0.9.5/ds_capability/handlers/mongodb_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.122354 discovery-capability-0.9.5/ds_capability/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.9.5/ds_capability/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2085 2023-09-10 16:06:14.000000 discovery-capability-0.9.5/ds_capability/intent/abstract_feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7652 2023-09-23 18:40:52.000000 discovery-capability-0.9.5/ds_capability/intent/abstract_feature_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2089 2023-09-12 13:21:18.000000 discovery-capability-0.9.5/ds_capability/intent/abstract_feature_select_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2101 2023-09-12 13:21:18.000000 discovery-capability-0.9.5/ds_capability/intent/abstract_feature_transform_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5938 2023-09-22 14:13:36.000000 discovery-capability-0.9.5/ds_capability/intent/common_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15639 2023-09-24 22:19:49.000000 discovery-capability-0.9.5/ds_capability/intent/controller_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)   147322 2023-09-23 22:46:58.000000 discovery-capability-0.9.5/ds_capability/intent/feature_build_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24898 2023-09-23 21:15:41.000000 discovery-capability-0.9.5/ds_capability/intent/feature_select_intent.py
--rw-r--r--   0 doatridge   (503) staff       (20)    30048 2023-09-19 14:30:44.000000 discovery-capability-0.9.5/ds_capability/intent/feature_transform_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.127218 discovery-capability-0.9.5/ds_capability/managers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.9.5/ds_capability/managers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.9.5/ds_capability/managers/controller_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      693 2023-09-12 13:21:18.000000 discovery-capability-0.9.5/ds_capability/managers/feature_build_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3734 2023-09-12 13:21:18.000000 discovery-capability-0.9.5/ds_capability/managers/feature_select_property_manager.py
--rw-r--r--   0 doatridge   (503) staff       (20)      596 2023-09-12 13:21:18.000000 discovery-capability-0.9.5/ds_capability/managers/feature_transform_property_manager.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.255829 discovery-capability-0.9.5/ds_capability/sample/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/lookup_complaints.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/lookup_professions.py
--rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/lookup_uk_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/lookup_uk_postcode_district.py
--rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/lookup_us_city.py
--rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/lookup_us_street_names.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/lookup_us_street_suffix.py
--rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_companies_fortune1000.py
--rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_companies_inc5000.py
--rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_uk_postcodes_primary.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_age_salary.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_city_area_code.csv
--rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_city_zipcodes_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_forename_mf.py
--rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_forename_unisex.py
--rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_full_address.py
--rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_healthcare_organisations.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_phone_code.py
--rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_profession_detail_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.9.5/ds_capability/sample/map_us_surname_rank.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25783 2023-09-23 22:55:48.000000 discovery-capability-0.9.5/ds_capability/sample/sample_data.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-09-24 22:21:33.283288 discovery-capability-0.9.5/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2271 2023-08-04 20:17:35.000000 discovery-capability-0.9.5/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.257520 discovery-capability-0.9.5/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.9.5/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.263729 discovery-capability-0.9.5/test/component/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.9.5/test/component/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3725 2023-08-26 19:08:57.000000 discovery-capability-0.9.5/test/component/controller_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7927 2023-09-10 16:06:13.000000 discovery-capability-0.9.5/test/component/controller_test_old.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3797 2023-09-19 17:33:35.000000 discovery-capability-0.9.5/test/component/discovery_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5065 2023-09-10 16:06:14.000000 discovery-capability-0.9.5/test/component/feature_build_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2140 2023-09-10 16:06:13.000000 discovery-capability-0.9.5/test/component/synthetic_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.265230 discovery-capability-0.9.5/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.9.5/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7729 2023-08-29 14:53:59.000000 discovery-capability-0.9.5/test/handlers/mongodb_handler_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-24 22:21:33.280459 discovery-capability-0.9.5/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.9.5/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     3892 2023-09-23 16:09:34.000000 discovery-capability-0.9.5/test/intent/abstract_feature_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     5438 2023-09-10 15:00:09.000000 discovery-capability-0.9.5/test/intent/controller_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4967 2023-09-10 16:06:13.000000 discovery-capability-0.9.5/test/intent/fb_analysis_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    12803 2023-09-15 23:00:58.000000 discovery-capability-0.9.5/test/intent/fb_correlate_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    14514 2023-09-11 23:44:55.000000 discovery-capability-0.9.5/test/intent/fb_diff_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7190 2023-09-23 22:05:15.000000 discovery-capability-0.9.5/test/intent/fb_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    13055 2023-09-16 14:57:34.000000 discovery-capability-0.9.5/test/intent/fb_model_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     6011 2023-09-16 22:18:17.000000 discovery-capability-0.9.5/test/intent/fs_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     4789 2023-09-18 20:35:08.000000 discovery-capability-0.9.5/test/intent/ft_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8132 2023-09-06 15:33:56.000000 discovery-capability-0.9.5/test/intent/pawan_translator.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.328985 discovery-capability-0.9.6/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1081 2023-07-03 16:32:12.000000 discovery-capability-0.9.6/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-07-03 16:32:12.000000 discovery-capability-0.9.6/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-09-25 14:37:08.329409 discovery-capability-0.9.6/PKG-INFO
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    10270 2023-07-03 16:32:12.000000 discovery-capability-0.9.6/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.147608 discovery-capability-0.9.6/discovery_capability.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    11227 2023-09-25 14:37:08.000000 discovery-capability-0.9.6/discovery_capability.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     3140 2023-09-25 14:37:08.000000 discovery-capability-0.9.6/discovery_capability.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-09-25 14:37:08.000000 discovery-capability-0.9.6/discovery_capability.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       96 2023-09-25 14:37:08.000000 discovery-capability-0.9.6/discovery_capability.egg-info/requires.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       19 2023-09-25 14:37:08.000000 discovery-capability-0.9.6/discovery_capability.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.148093 discovery-capability-0.9.6/ds_capability/
+-rw-r--r--   0 doatridge   (503) staff       (20)      373 2023-09-24 22:24:01.000000 discovery-capability-0.9.6/ds_capability/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.155491 discovery-capability-0.9.6/ds_capability/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:07.000000 discovery-capability-0.9.6/ds_capability/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15105 2023-09-17 21:58:10.000000 discovery-capability-0.9.6/ds_capability/components/abstract_common_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3400 2023-09-23 21:15:41.000000 discovery-capability-0.9.6/ds_capability/components/commons.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    27164 2023-09-10 14:58:03.000000 discovery-capability-0.9.6/ds_capability/components/controller.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    26443 2023-09-19 17:14:53.000000 discovery-capability-0.9.6/ds_capability/components/discovery.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5213 2023-09-11 16:43:46.000000 discovery-capability-0.9.6/ds_capability/components/feature_build.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5229 2023-09-11 16:43:46.000000 discovery-capability-0.9.6/ds_capability/components/feature_select.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5177 2023-09-12 13:31:59.000000 discovery-capability-0.9.6/ds_capability/components/feature_transform.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.158789 discovery-capability-0.9.6/ds_capability/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 17:24:03.000000 discovery-capability-0.9.6/ds_capability/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2507 2023-09-24 20:11:52.000000 discovery-capability-0.9.6/ds_capability/handlers/duckdb_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6191 2023-08-26 18:24:33.000000 discovery-capability-0.9.6/ds_capability/handlers/mongodb_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.169009 discovery-capability-0.9.6/ds_capability/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-24 15:42:26.000000 discovery-capability-0.9.6/ds_capability/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2085 2023-09-10 16:06:14.000000 discovery-capability-0.9.6/ds_capability/intent/abstract_feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7652 2023-09-23 18:40:52.000000 discovery-capability-0.9.6/ds_capability/intent/abstract_feature_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2089 2023-09-12 13:21:18.000000 discovery-capability-0.9.6/ds_capability/intent/abstract_feature_select_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2101 2023-09-12 13:21:18.000000 discovery-capability-0.9.6/ds_capability/intent/abstract_feature_transform_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5938 2023-09-22 14:13:36.000000 discovery-capability-0.9.6/ds_capability/intent/common_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    15639 2023-09-24 22:19:49.000000 discovery-capability-0.9.6/ds_capability/intent/controller_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   147976 2023-09-25 14:30:02.000000 discovery-capability-0.9.6/ds_capability/intent/feature_build_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24898 2023-09-23 21:15:41.000000 discovery-capability-0.9.6/ds_capability/intent/feature_select_intent.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    30048 2023-09-19 14:30:44.000000 discovery-capability-0.9.6/ds_capability/intent/feature_transform_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.174103 discovery-capability-0.9.6/ds_capability/managers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 15:58:08.000000 discovery-capability-0.9.6/ds_capability/managers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3341 2023-06-29 15:03:02.000000 discovery-capability-0.9.6/ds_capability/managers/controller_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      693 2023-09-12 13:21:18.000000 discovery-capability-0.9.6/ds_capability/managers/feature_build_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3734 2023-09-12 13:21:18.000000 discovery-capability-0.9.6/ds_capability/managers/feature_select_property_manager.py
+-rw-r--r--   0 doatridge   (503) staff       (20)      596 2023-09-12 13:21:18.000000 discovery-capability-0.9.6/ds_capability/managers/feature_transform_property_manager.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.302201 discovery-capability-0.9.6/ds_capability/sample/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     1127 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/lookup_complaints.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2341 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/lookup_professions.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   171941 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/lookup_uk_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    24106 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/lookup_uk_postcode_district.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   260492 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/lookup_us_city.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   532096 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/lookup_us_street_names.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2080 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/lookup_us_street_suffix.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   110474 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_companies_fortune1000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   540809 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_companies_inc5000.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     9609 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_uk_postcodes_primary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3260 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_age_salary.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12268 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_city_area_code.csv
+-rw-r--r--   0 doatridge   (503) staff       (20)  4153752 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_city_zipcodes_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)   570024 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_forename_mf.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    76010 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_forename_unisex.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  9811841 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_full_address.py
+-rw-r--r--   0 doatridge   (503) staff       (20) 12713221 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_healthcare_organisations.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3005 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_phone_code.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    21849 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_profession_detail_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)  2438399 2023-01-04 22:14:44.000000 discovery-capability-0.9.6/ds_capability/sample/map_us_surname_rank.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25783 2023-09-23 22:55:48.000000 discovery-capability-0.9.6/ds_capability/sample/sample_data.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      109 2023-09-25 14:37:08.330377 discovery-capability-0.9.6/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2271 2023-08-04 20:17:35.000000 discovery-capability-0.9.6/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.305630 discovery-capability-0.9.6/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:22:50.000000 discovery-capability-0.9.6/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.311225 discovery-capability-0.9.6/test/component/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-08 17:39:24.000000 discovery-capability-0.9.6/test/component/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3725 2023-08-26 19:08:57.000000 discovery-capability-0.9.6/test/component/controller_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7927 2023-09-10 16:06:13.000000 discovery-capability-0.9.6/test/component/controller_test_old.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3797 2023-09-19 17:33:35.000000 discovery-capability-0.9.6/test/component/discovery_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5065 2023-09-10 16:06:14.000000 discovery-capability-0.9.6/test/component/feature_build_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2140 2023-09-10 16:06:13.000000 discovery-capability-0.9.6/test/component/synthetic_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.312472 discovery-capability-0.9.6/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-05-19 18:23:18.000000 discovery-capability-0.9.6/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7729 2023-08-29 14:53:59.000000 discovery-capability-0.9.6/test/handlers/mongodb_handler_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-09-25 14:37:08.327594 discovery-capability-0.9.6/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-15 23:39:19.000000 discovery-capability-0.9.6/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     3892 2023-09-23 16:09:34.000000 discovery-capability-0.9.6/test/intent/abstract_feature_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     5438 2023-09-10 15:00:09.000000 discovery-capability-0.9.6/test/intent/controller_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4967 2023-09-10 16:06:13.000000 discovery-capability-0.9.6/test/intent/fb_analysis_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    12803 2023-09-15 23:00:58.000000 discovery-capability-0.9.6/test/intent/fb_correlate_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    14514 2023-09-11 23:44:55.000000 discovery-capability-0.9.6/test/intent/fb_diff_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6985 2023-09-25 14:34:32.000000 discovery-capability-0.9.6/test/intent/fb_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    13055 2023-09-16 14:57:34.000000 discovery-capability-0.9.6/test/intent/fb_model_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     6011 2023-09-16 22:18:17.000000 discovery-capability-0.9.6/test/intent/fs_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     4789 2023-09-18 20:35:08.000000 discovery-capability-0.9.6/test/intent/ft_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8132 2023-09-06 15:33:56.000000 discovery-capability-0.9.6/test/intent/pawan_translator.py
```

### Comparing `discovery-capability-0.9.5/LICENSE.txt` & `discovery-capability-0.9.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/PKG-INFO` & `discovery-capability-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.9.5
+Version: 0.9.6
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.9.5/README.rst` & `discovery-capability-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/discovery_capability.egg-info/PKG-INFO` & `discovery-capability-0.9.6/discovery_capability.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-capability
-Version: 0.9.5
+Version: 0.9.6
 Summary: Data Science to production accelerator
 Home-page: https://github.com/gigas64/discovery-capability
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Wrangling ML Visualisation Dictionary Discovery Productize Classification Feature Engineering Cleansing
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-capability-0.9.5/discovery_capability.egg-info/SOURCES.txt` & `discovery-capability-0.9.6/discovery_capability.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/components/abstract_common_component.py` & `discovery-capability-0.9.6/ds_capability/components/abstract_common_component.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/components/commons.py` & `discovery-capability-0.9.6/ds_capability/components/commons.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/components/controller.py` & `discovery-capability-0.9.6/ds_capability/components/controller.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/components/discovery.py` & `discovery-capability-0.9.6/ds_capability/components/discovery.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/components/feature_build.py` & `discovery-capability-0.9.6/ds_capability/components/feature_build.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/components/feature_select.py` & `discovery-capability-0.9.6/ds_capability/components/feature_select.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/components/feature_transform.py` & `discovery-capability-0.9.6/ds_capability/components/feature_transform.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/handlers/duckdb_handlers.py` & `discovery-capability-0.9.6/ds_capability/handlers/duckdb_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/handlers/mongodb_handlers.py` & `discovery-capability-0.9.6/ds_capability/handlers/mongodb_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/abstract_feature_build_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/abstract_feature_build_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/abstract_feature_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/abstract_feature_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/abstract_feature_select_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/abstract_feature_select_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/abstract_feature_transform_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/abstract_feature_transform_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/common_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/common_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/controller_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/controller_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/feature_build_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/feature_build_intent.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,14 @@
             for key, value in i.items():
                 if key in ['size', 'shuffle', 'seed']:
                     continue
                 rtn_lst.append(str(value)[:-7])
             return rtn_lst
         raise ValueError(f"The sample map name '{method}' was not found in the MappedSample class")
 
-
-
     def get_number(self, start: [int, float, str]=None, stop: [int, float, str]=None, canonical: pa.Table=None,
                    relative_freq: list=None, precision: int=None, ordered: str=None, at_most: int=None, size: int=None,
                    quantity: float=None, to_header: str=None,  seed: int=None, save_intent: bool=None, intent_order: int=None,
                    intent_level: [int, str]=None, replace_intent: bool=None, remove_duplicates: bool=None) -> pa.Table:
         """ returns a number in the range from_value to to_value. if only to_value given from_value is zero
 
         :param start: optional (signed) integer or float to start from. See below for str
@@ -82,14 +80,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         start = self._extract_value(start)
         stop = self._extract_value(stop)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         if not isinstance(start, (int, float)) and not isinstance(stop, (int, float)):
@@ -188,14 +187,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         if len(selection) < 1:
             return [None] * size
         encode = encode if isinstance(encode, bool) else False
         seed = self._seed() if seed is None else seed
         relative_freq = relative_freq if isinstance(relative_freq, list) else [1]*len(selection)
@@ -239,14 +239,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         prob = probability if isinstance(probability, int) and 0 < probability < 1 else 0.5
         seed = self._seed(seed=seed)
         rtn_list = list(stats.bernoulli.rvs(p=probability, size=size, random_state=seed))
         rtn_list = list(map(bool, rtn_list))
         rtn_list = self._set_quantity(rtn_list, quantity=self._quantity(quantity), seed=seed)
@@ -305,14 +306,15 @@
          """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         if start is None or until is None:
             raise ValueError("The start or until parameters cannot be of NoneType")
         # Code block for intent
         time_unit = time_unit if isinstance(time_unit, str) and time_unit in ['s', 'ms', 'us', 'ns'] else 'us'
         as_num = as_num if isinstance(as_num, bool) else False
@@ -385,14 +387,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         precision = precision if isinstance(precision, (float, int)) else 3
         seed = self._seed() if seed is None else seed
         if not all(isinstance(value, tuple) for value in intervals):
             raise ValueError("The intervals list must be a list of tuples")
         interval_tbl = self.get_category(selection=intervals, relative_freq=relative_freq, size=size, seed=seed,
@@ -465,14 +468,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed() if seed is None else seed
         precision = precision if isinstance(precision, int) else 3
         generator = np.random.default_rng(seed=seed)
         rtn_list = list(generator.normal(loc=mean, scale=std, size=size))
         rtn_list = list(np.around(rtn_list, precision))
@@ -511,14 +515,15 @@
        """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed() if seed is None else seed
         number = self._extract_value(number)
         number = int(number * size) if isinstance(number, float) and 0 <= number <= 1 else int(number)
         number = number if 0 <= number < size else size
         if isinstance(number, int) and 0 <= number <= size:
@@ -560,14 +565,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed() if seed is None else seed
         probability = self._extract_value(probability)
         rtn_list = list(stats.bernoulli.rvs(p=probability, size=size, random_state=seed))
         rtn_list = self._set_quantity(rtn_list, quantity=self._quantity(quantity), seed=seed)
         to_header = to_header if isinstance(to_header, str) else next(self.label_gen)
@@ -605,14 +611,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         precision = precision if isinstance(precision, int) else 3
         seed = self._seed() if seed is None else seed
         rtn_list = stats.truncnorm((lower - mean) / std, (upper - mean) / std, loc=mean, scale=std)
         rtn_list = rtn_list.rvs(size, random_state=seed).round(precision)
         rtn_list = self._set_quantity(rtn_list, quantity=self._quantity(quantity), seed=seed)
@@ -650,14 +657,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed() if seed is None else seed
         precision = 3 if precision is None else precision
         is_stats = is_stats if isinstance(is_stats, bool) else False
         if is_stats:
             rtn_list = eval(f"stats.{distribution}.rvs(size=size, random_state=_seed, **kwargs)", globals(), locals())
@@ -716,14 +724,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         choice_only = False if choice_only is None or not isinstance(choice_only, bool) else choice_only
         as_binary = as_binary if isinstance(as_binary, bool) else False
         quantity = self._quantity(quantity)
         seed = self._seed(seed=seed)
         if choices is None or not isinstance(choices, dict):
@@ -790,14 +799,15 @@
         :return: a sample list
         """
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         if sample_name not in self.sample_list:
             raise ValueError(f"The sample list '{sample_name}' does not exist as a sample list")
         sample_size = sample_size if isinstance(sample_size, int) else size
         quantity = self._quantity(quantity)
         seed = self._seed(seed=seed)
@@ -856,14 +866,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    column_name=column_name, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         if sample_map not in self.sample_map:
             raise ValueError(f"The sample map '{sample_map}' does not exist as a sample maps")
         _seed = self._seed(seed=seed)
         shuffle = shuffle if isinstance(shuffle, bool) else True
         tbl = eval(f"MappedSample.{sample_map}(size={size}, shuffle={shuffle}, seed={_seed}, **{kwargs})")
@@ -914,14 +925,15 @@
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
         canonical = self._get_canonical(canonical)
         other = self._get_canonical(other)
+        size = self._extract_value(size)
         if other is None or other.num_rows == 0:
             return None
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         date_jitter = date_jitter if isinstance(date_jitter, int) else 2
         units_allowed = ['W', 'D', 'h', 'm', 's', 'milli', 'micro']
         date_units = date_units if isinstance(date_units, str) and date_units in units_allowed else 'D'
@@ -1025,14 +1037,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # remove intent params
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed(seed=seed)
         prob_nulls = prob_nulls if isinstance(prob_nulls, float) and 0 < prob_nulls < 1 else 0.1
         category_encode = category_encode if isinstance(category_encode, bool) else True
         # cat
         canonical = self.get_category(selection=['SUSPENDED', 'ACTIVE', 'PENDING', 'INACTIVE', 'ARCHIVE'],
@@ -1134,14 +1147,15 @@
         """
         # intent persist options
         self._set_intend_signature(self._intent_builder(method=inspect.currentframe().f_code.co_name, params=locals()),
                                    intent_level=intent_level, intent_order=intent_order, replace_intent=replace_intent,
                                    remove_duplicates=remove_duplicates, save_intent=save_intent)
         # Code block for intent
         canonical = self._get_canonical(canonical)
+        size = self._extract_value(size)
         if not isinstance(size, int):
             raise ValueError("size not set. Size must be an int greater than zero")
         seed = self._seed(seed=seed)
         num_columns = num_columns if isinstance(num_columns, int) else 1
         name_prefix = name_prefix if isinstance(name_prefix, str) else ''
         label_gen = Commons.label_gen()
         rtn_tbl = None
```

### Comparing `discovery-capability-0.9.5/ds_capability/intent/feature_select_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/feature_select_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/intent/feature_transform_intent.py` & `discovery-capability-0.9.6/ds_capability/intent/feature_transform_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/managers/controller_property_manager.py` & `discovery-capability-0.9.6/ds_capability/managers/controller_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/managers/feature_build_property_manager.py` & `discovery-capability-0.9.6/ds_capability/managers/feature_build_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/managers/feature_select_property_manager.py` & `discovery-capability-0.9.6/ds_capability/managers/feature_select_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/managers/feature_transform_property_manager.py` & `discovery-capability-0.9.6/ds_capability/managers/feature_transform_property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/lookup_complaints.py` & `discovery-capability-0.9.6/ds_capability/sample/lookup_complaints.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/lookup_professions.py` & `discovery-capability-0.9.6/ds_capability/sample/lookup_professions.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/lookup_uk_city.py` & `discovery-capability-0.9.6/ds_capability/sample/lookup_uk_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/lookup_uk_postcode_district.py` & `discovery-capability-0.9.6/ds_capability/sample/lookup_uk_postcode_district.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/lookup_us_city.py` & `discovery-capability-0.9.6/ds_capability/sample/lookup_us_city.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/lookup_us_street_names.py` & `discovery-capability-0.9.6/ds_capability/sample/lookup_us_street_names.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/lookup_us_street_suffix.py` & `discovery-capability-0.9.6/ds_capability/sample/lookup_us_street_suffix.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_companies_fortune1000.py` & `discovery-capability-0.9.6/ds_capability/sample/map_companies_fortune1000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_companies_inc5000.py` & `discovery-capability-0.9.6/ds_capability/sample/map_companies_inc5000.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_uk_postcodes_primary.py` & `discovery-capability-0.9.6/ds_capability/sample/map_uk_postcodes_primary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_age_salary.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_age_salary.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_city_area_code.csv` & `discovery-capability-0.9.6/ds_capability/sample/map_us_city_area_code.csv`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_city_zipcodes_rank.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_city_zipcodes_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_forename_mf.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_forename_mf.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_forename_unisex.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_forename_unisex.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_full_address.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_full_address.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_healthcare_organisations.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_healthcare_organisations.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_phone_code.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_phone_code.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_profession_detail_rank.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_profession_detail_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/map_us_surname_rank.py` & `discovery-capability-0.9.6/ds_capability/sample/map_us_surname_rank.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/ds_capability/sample/sample_data.py` & `discovery-capability-0.9.6/ds_capability/sample/sample_data.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/setup.py` & `discovery-capability-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/component/controller_test.py` & `discovery-capability-0.9.6/test/component/controller_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/component/controller_test_old.py` & `discovery-capability-0.9.6/test/component/controller_test_old.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/component/discovery_test.py` & `discovery-capability-0.9.6/test/component/discovery_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/component/feature_build_test.py` & `discovery-capability-0.9.6/test/component/feature_build_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/component/synthetic_test.py` & `discovery-capability-0.9.6/test/component/synthetic_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/handlers/mongodb_handler_test.py` & `discovery-capability-0.9.6/test/handlers/mongodb_handler_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/abstract_feature_intent_test.py` & `discovery-capability-0.9.6/test/intent/abstract_feature_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/controller_intent_test.py` & `discovery-capability-0.9.6/test/intent/controller_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/fb_analysis_intent_test.py` & `discovery-capability-0.9.6/test/intent/fb_analysis_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/fb_correlate_intent_test.py` & `discovery-capability-0.9.6/test/intent/fb_correlate_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/fb_diff_intent_test.py` & `discovery-capability-0.9.6/test/intent/fb_diff_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/fb_intent_test.py` & `discovery-capability-0.9.6/test/intent/fb_intent_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -147,23 +147,16 @@
         self.assertEqual(['P_A', 'P_B', 'P_C'], tbl.column_names)
 
     def test_get_sample_map(self):
         fb = FeatureBuild.from_memory()
         tools: FeatureBuildIntent = fb.tools
         print(tools.sample_map)
         # tools.get_sample_map('us_persona', size=10, )
-        i = tools.sample_inspect('us_zipcodes_detail').parameters
-        rtn_lst = []
-        for key, value in i.items():
-            if key in ['size', 'shuffle', 'seed']:
-                continue
-            rtn_lst.append(str(value)[:-7])
-        print(rtn_lst)
-
-
+        i = tools.sample_inspect('us_persona')
+        print(i)
 
     def test_raise(self):
         with self.assertRaises(KeyError) as context:
             env = os.environ['NoEnvValueTest']
         self.assertTrue("'NoEnvValueTest'" in str(context.exception))
 
 def pm_view(capability: str, task: str, section: str=None):
```

### Comparing `discovery-capability-0.9.5/test/intent/fb_model_intent_test.py` & `discovery-capability-0.9.6/test/intent/fb_model_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/fs_intent_test.py` & `discovery-capability-0.9.6/test/intent/fs_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/ft_intent_test.py` & `discovery-capability-0.9.6/test/intent/ft_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-capability-0.9.5/test/intent/pawan_translator.py` & `discovery-capability-0.9.6/test/intent/pawan_translator.py`

 * *Files identical despite different names*

