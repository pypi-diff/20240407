# Comparing `tmp/moe-2.1.2.tar.gz` & `tmp/moe-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moe-2.1.2.tar", max compression
+gzip compressed data, was "moe-2.1.3.tar", max compression
```

## Comparing `moe-2.1.2.tar` & `moe-2.1.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0        0        0     1066 2024-04-06 19:51:12.110586 moe-2.1.2/LICENSE
--rw-r--r--   0        0        0     3244 2024-04-06 19:51:12.110586 moe-2.1.2/README.rst
--rw-r--r--   0        0        0       38 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/README
--rw-r--r--   0        0        0     2008 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/alembic.ini
--rw-r--r--   0        0        0     2704 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/env.py
--rw-r--r--   0        0        0      495 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/script.py.mako
--rw-r--r--   0        0        0      745 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/0ce5960a081e_new_field_catalog_nums.py
--rw-r--r--   0        0        0      588 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/30668259fcd6_new_field_country.py
--rw-r--r--   0        0        0      600 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/32e9fea590b7_new_field_track_total.py
--rw-r--r--   0        0        0      582 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/60608d9d2908_new_field_media.py
--rw-r--r--   0        0        0     3186 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/6d4e785df5cb_initial_generation.py
--rw-r--r--   0        0        0      582 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/817440447857_new_field_label.py
--rw-r--r--   0        0        0      606 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/880c5a2d80ed_remove_audio_format_field.py
--rw-r--r--   0        0        0      602 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/ab11c34c1d0b_new_field_audio_format.py
--rw-r--r--   0        0        0     1155 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/ab5db9861d30_rename_custom_fields.py
--rw-r--r--   0        0        0     5699 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/bf49ac6805f7_json_multi_value_fields.py
--rw-r--r--   0        0        0      598 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/db3a470892c6_new_field_og_date.py
--rw-r--r--   0        0        0      587 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/eb8c7e20a080_new_field_barcode.py
--rw-r--r--   0        0        0      724 2024-04-06 19:51:12.114586 moe-2.1.2/alembic/versions/fe0956c93730_new_field_artists.py
--rw-r--r--   0        0        0      443 2024-04-06 19:51:12.114586 moe-2.1.2/moe/__init__.py
--rw-r--r--   0        0        0      430 2024-04-06 19:51:12.114586 moe-2.1.2/moe/add/__init__.py
--rw-r--r--   0        0        0     3736 2024-04-06 19:51:12.114586 moe-2.1.2/moe/add/add_cli.py
--rw-r--r--   0        0        0     2154 2024-04-06 19:51:12.114586 moe-2.1.2/moe/add/add_core.py
--rwxr-xr-x   0        0        0     4863 2024-04-06 19:51:12.114586 moe-2.1.2/moe/cli.py
--rw-r--r--   0        0        0    15593 2024-04-06 19:51:12.114586 moe-2.1.2/moe/config.py
--rw-r--r--   0        0        0      514 2024-04-06 19:51:12.114586 moe-2.1.2/moe/duplicate/__init__.py
--rw-r--r--   0        0        0     7141 2024-04-06 19:51:12.114586 moe-2.1.2/moe/duplicate/dup_cli.py
--rw-r--r--   0        0        0     5841 2024-04-06 19:51:12.114586 moe-2.1.2/moe/duplicate/dup_core.py
--rw-r--r--   0        0        0      454 2024-04-06 19:51:12.114586 moe-2.1.2/moe/edit/__init__.py
--rw-r--r--   0        0        0     2135 2024-04-06 19:51:12.114586 moe-2.1.2/moe/edit/edit_cli.py
--rw-r--r--   0        0        0     1801 2024-04-06 19:51:12.114586 moe-2.1.2/moe/edit/edit_core.py
--rw-r--r--   0        0        0      311 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/__init__.py
--rw-r--r--   0        0        0    19002 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/album.py
--rw-r--r--   0        0        0     5499 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/extra.py
--rw-r--r--   0        0        0    10209 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/lib_item.py
--rw-r--r--   0        0        0    16985 2024-04-06 19:51:12.114586 moe-2.1.2/moe/library/track.py
--rw-r--r--   0        0        0     4421 2024-04-06 19:51:12.114586 moe-2.1.2/moe/list.py
--rw-r--r--   0        0        0      544 2024-04-06 19:51:12.114586 moe-2.1.2/moe/moe_import/__init__.py
--rw-r--r--   0        0        0    12282 2024-04-06 19:51:12.114586 moe-2.1.2/moe/moe_import/import_cli.py
--rw-r--r--   0        0        0     3852 2024-04-06 19:51:12.114586 moe-2.1.2/moe/moe_import/import_core.py
--rw-r--r--   0        0        0      472 2024-04-06 19:51:12.114586 moe-2.1.2/moe/move/__init__.py
--rw-r--r--   0        0        0     2506 2024-04-06 19:51:12.114586 moe-2.1.2/moe/move/move_cli.py
--rw-r--r--   0        0        0    10415 2024-04-06 19:51:12.114586 moe-2.1.2/moe/move/move_core.py
--rw-r--r--   0        0        0        0 2024-04-06 19:51:12.114586 moe-2.1.2/moe/py.typed
--rw-r--r--   0        0        0     7053 2024-04-06 19:51:12.114586 moe-2.1.2/moe/query.py
--rw-r--r--   0        0        0      462 2024-04-06 19:51:12.114586 moe-2.1.2/moe/read/__init__.py
--rw-r--r--   0        0        0     1619 2024-04-06 19:51:12.114586 moe-2.1.2/moe/read/read_cli.py
--rw-r--r--   0        0        0      818 2024-04-06 19:51:12.114586 moe-2.1.2/moe/read/read_core.py
--rw-r--r--   0        0        0      450 2024-04-06 19:51:12.114586 moe-2.1.2/moe/remove/__init__.py
--rw-r--r--   0        0        0     1475 2024-04-06 19:51:12.118586 moe-2.1.2/moe/remove/rm_cli.py
--rw-r--r--   0        0        0     1228 2024-04-06 19:51:12.118586 moe-2.1.2/moe/remove/rm_core.py
--rw-r--r--   0        0        0       62 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/__init__.py
--rw-r--r--   0        0        0      209 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/cli/__init__.py
--rw-r--r--   0        0        0     2131 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/cli/prompt.py
--rw-r--r--   0        0        0     2609 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/cli/query.py
--rw-r--r--   0        0        0      153 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/core/__init__.py
--rw-r--r--   0        0        0     5651 2024-04-06 19:51:12.118586 moe-2.1.2/moe/util/core/match.py
--rw-r--r--   0        0        0     3033 2024-04-06 19:51:12.118586 moe-2.1.2/moe/write.py
--rw-r--r--   0        0        0     2144 2024-04-06 19:51:12.118586 moe-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 moe-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-07 01:26:25.377646 moe-2.1.3/LICENSE
+-rw-r--r--   0        0        0     3244 2024-04-07 01:26:25.377646 moe-2.1.3/README.rst
+-rw-r--r--   0        0        0       38 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/README
+-rw-r--r--   0        0        0     2008 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/alembic.ini
+-rw-r--r--   0        0        0     2704 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/env.py
+-rw-r--r--   0        0        0      495 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/script.py.mako
+-rw-r--r--   0        0        0      745 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/0ce5960a081e_new_field_catalog_nums.py
+-rw-r--r--   0        0        0      588 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/30668259fcd6_new_field_country.py
+-rw-r--r--   0        0        0      600 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/32e9fea590b7_new_field_track_total.py
+-rw-r--r--   0        0        0      582 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/60608d9d2908_new_field_media.py
+-rw-r--r--   0        0        0     3186 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/6d4e785df5cb_initial_generation.py
+-rw-r--r--   0        0        0      582 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/817440447857_new_field_label.py
+-rw-r--r--   0        0        0      606 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/880c5a2d80ed_remove_audio_format_field.py
+-rw-r--r--   0        0        0      602 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/ab11c34c1d0b_new_field_audio_format.py
+-rw-r--r--   0        0        0     1155 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/ab5db9861d30_rename_custom_fields.py
+-rw-r--r--   0        0        0     5699 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/bf49ac6805f7_json_multi_value_fields.py
+-rw-r--r--   0        0        0      598 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/db3a470892c6_new_field_og_date.py
+-rw-r--r--   0        0        0      587 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/eb8c7e20a080_new_field_barcode.py
+-rw-r--r--   0        0        0      724 2024-04-07 01:26:25.377646 moe-2.1.3/alembic/versions/fe0956c93730_new_field_artists.py
+-rw-r--r--   0        0        0      443 2024-04-07 01:26:25.377646 moe-2.1.3/moe/__init__.py
+-rw-r--r--   0        0        0      430 2024-04-07 01:26:25.377646 moe-2.1.3/moe/add/__init__.py
+-rw-r--r--   0        0        0     3736 2024-04-07 01:26:25.377646 moe-2.1.3/moe/add/add_cli.py
+-rw-r--r--   0        0        0     2154 2024-04-07 01:26:25.377646 moe-2.1.3/moe/add/add_core.py
+-rwxr-xr-x   0        0        0     4863 2024-04-07 01:26:25.381646 moe-2.1.3/moe/cli.py
+-rw-r--r--   0        0        0    15593 2024-04-07 01:26:25.381646 moe-2.1.3/moe/config.py
+-rw-r--r--   0        0        0      514 2024-04-07 01:26:25.381646 moe-2.1.3/moe/duplicate/__init__.py
+-rw-r--r--   0        0        0     7141 2024-04-07 01:26:25.381646 moe-2.1.3/moe/duplicate/dup_cli.py
+-rw-r--r--   0        0        0     5841 2024-04-07 01:26:25.381646 moe-2.1.3/moe/duplicate/dup_core.py
+-rw-r--r--   0        0        0      454 2024-04-07 01:26:25.381646 moe-2.1.3/moe/edit/__init__.py
+-rw-r--r--   0        0        0     2135 2024-04-07 01:26:25.381646 moe-2.1.3/moe/edit/edit_cli.py
+-rw-r--r--   0        0        0     1801 2024-04-07 01:26:25.381646 moe-2.1.3/moe/edit/edit_core.py
+-rw-r--r--   0        0        0      311 2024-04-07 01:26:25.381646 moe-2.1.3/moe/library/__init__.py
+-rw-r--r--   0        0        0    18995 2024-04-07 01:26:25.381646 moe-2.1.3/moe/library/album.py
+-rw-r--r--   0        0        0     5499 2024-04-07 01:26:25.381646 moe-2.1.3/moe/library/extra.py
+-rw-r--r--   0        0        0    10209 2024-04-07 01:26:25.381646 moe-2.1.3/moe/library/lib_item.py
+-rw-r--r--   0        0        0    16989 2024-04-07 01:26:25.381646 moe-2.1.3/moe/library/track.py
+-rw-r--r--   0        0        0     4421 2024-04-07 01:26:25.381646 moe-2.1.3/moe/list.py
+-rw-r--r--   0        0        0      544 2024-04-07 01:26:25.381646 moe-2.1.3/moe/moe_import/__init__.py
+-rw-r--r--   0        0        0    12282 2024-04-07 01:26:25.381646 moe-2.1.3/moe/moe_import/import_cli.py
+-rw-r--r--   0        0        0     3852 2024-04-07 01:26:25.381646 moe-2.1.3/moe/moe_import/import_core.py
+-rw-r--r--   0        0        0      472 2024-04-07 01:26:25.381646 moe-2.1.3/moe/move/__init__.py
+-rw-r--r--   0        0        0     2506 2024-04-07 01:26:25.381646 moe-2.1.3/moe/move/move_cli.py
+-rw-r--r--   0        0        0    10415 2024-04-07 01:26:25.381646 moe-2.1.3/moe/move/move_core.py
+-rw-r--r--   0        0        0        0 2024-04-07 01:26:25.381646 moe-2.1.3/moe/py.typed
+-rw-r--r--   0        0        0     7053 2024-04-07 01:26:25.381646 moe-2.1.3/moe/query.py
+-rw-r--r--   0        0        0      462 2024-04-07 01:26:25.381646 moe-2.1.3/moe/read/__init__.py
+-rw-r--r--   0        0        0     1619 2024-04-07 01:26:25.381646 moe-2.1.3/moe/read/read_cli.py
+-rw-r--r--   0        0        0      818 2024-04-07 01:26:25.381646 moe-2.1.3/moe/read/read_core.py
+-rw-r--r--   0        0        0      450 2024-04-07 01:26:25.381646 moe-2.1.3/moe/remove/__init__.py
+-rw-r--r--   0        0        0     1475 2024-04-07 01:26:25.381646 moe-2.1.3/moe/remove/rm_cli.py
+-rw-r--r--   0        0        0     1228 2024-04-07 01:26:25.381646 moe-2.1.3/moe/remove/rm_core.py
+-rw-r--r--   0        0        0       62 2024-04-07 01:26:25.381646 moe-2.1.3/moe/util/__init__.py
+-rw-r--r--   0        0        0      209 2024-04-07 01:26:25.381646 moe-2.1.3/moe/util/cli/__init__.py
+-rw-r--r--   0        0        0     2131 2024-04-07 01:26:25.381646 moe-2.1.3/moe/util/cli/prompt.py
+-rw-r--r--   0        0        0     2609 2024-04-07 01:26:25.381646 moe-2.1.3/moe/util/cli/query.py
+-rw-r--r--   0        0        0      153 2024-04-07 01:26:25.381646 moe-2.1.3/moe/util/core/__init__.py
+-rw-r--r--   0        0        0     5651 2024-04-07 01:26:25.381646 moe-2.1.3/moe/util/core/match.py
+-rw-r--r--   0        0        0     3033 2024-04-07 01:26:25.381646 moe-2.1.3/moe/write.py
+-rw-r--r--   0        0        0     2144 2024-04-07 01:26:25.381646 moe-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4512 1970-01-01 00:00:00.000000 moe-2.1.3/PKG-INFO
```

### Comparing `moe-2.1.2/LICENSE` & `moe-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/README.rst` & `moe-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/alembic.ini` & `moe-2.1.3/alembic/alembic.ini`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/env.py` & `moe-2.1.3/alembic/env.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/0ce5960a081e_new_field_catalog_nums.py` & `moe-2.1.3/alembic/versions/0ce5960a081e_new_field_catalog_nums.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/30668259fcd6_new_field_country.py` & `moe-2.1.3/alembic/versions/30668259fcd6_new_field_country.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/32e9fea590b7_new_field_track_total.py` & `moe-2.1.3/alembic/versions/32e9fea590b7_new_field_track_total.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/60608d9d2908_new_field_media.py` & `moe-2.1.3/alembic/versions/60608d9d2908_new_field_media.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/6d4e785df5cb_initial_generation.py` & `moe-2.1.3/alembic/versions/6d4e785df5cb_initial_generation.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/817440447857_new_field_label.py` & `moe-2.1.3/alembic/versions/817440447857_new_field_label.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/880c5a2d80ed_remove_audio_format_field.py` & `moe-2.1.3/alembic/versions/880c5a2d80ed_remove_audio_format_field.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/ab11c34c1d0b_new_field_audio_format.py` & `moe-2.1.3/alembic/versions/ab11c34c1d0b_new_field_audio_format.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/ab5db9861d30_rename_custom_fields.py` & `moe-2.1.3/alembic/versions/ab5db9861d30_rename_custom_fields.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/bf49ac6805f7_json_multi_value_fields.py` & `moe-2.1.3/alembic/versions/bf49ac6805f7_json_multi_value_fields.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/db3a470892c6_new_field_og_date.py` & `moe-2.1.3/alembic/versions/db3a470892c6_new_field_og_date.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/eb8c7e20a080_new_field_barcode.py` & `moe-2.1.3/alembic/versions/eb8c7e20a080_new_field_barcode.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/alembic/versions/fe0956c93730_new_field_artists.py` & `moe-2.1.3/alembic/versions/fe0956c93730_new_field_artists.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/add/add_cli.py` & `moe-2.1.3/moe/add/add_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/add/add_core.py` & `moe-2.1.3/moe/add/add_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/cli.py` & `moe-2.1.3/moe/cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/config.py` & `moe-2.1.3/moe/config.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/duplicate/__init__.py` & `moe-2.1.3/moe/duplicate/__init__.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/duplicate/dup_cli.py` & `moe-2.1.3/moe/duplicate/dup_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/duplicate/dup_core.py` & `moe-2.1.3/moe/duplicate/dup_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/edit/edit_cli.py` & `moe-2.1.3/moe/edit/edit_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/edit/edit_core.py` & `moe-2.1.3/moe/edit/edit_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/library/album.py` & `moe-2.1.3/moe/library/album.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 
         log.debug(
             f"MetaAlbums merged. [album_a={self!r}, album_b={other!r}, {overwrite=}]"
         )
 
     def __eq__(self, other) -> bool:
         """Compares MetaAlbums by their fields."""
-        if type(self) != type(other):  # noqa: E721
+        if not isinstance(other, MetaAlbum):
             return False
 
         for field in self.fields:
             if not hasattr(other, field) or (
                 getattr(self, field) != getattr(other, field)
             ):
                 return False
```

### Comparing `moe-2.1.2/moe/library/extra.py` & `moe-2.1.3/moe/library/extra.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/library/lib_item.py` & `moe-2.1.3/moe/library/lib_item.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/library/track.py` & `moe-2.1.3/moe/library/track.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
             ):
                 self.custom[custom_field] = other_value
 
         log.debug(f"Tracks merged. [track_a={self!r}, track_b={other!r}, {overwrite=}]")
 
     def __eq__(self, other) -> bool:
         """Compares Tracks by their fields."""
-        if not isinstance(other, Track):
+        if not isinstance(other, MetaTrack):
             return False
 
         for field in self.fields:
             if not hasattr(other, field) or (
                 getattr(self, field) != getattr(other, field)
             ):
                 return False
```

### Comparing `moe-2.1.2/moe/list.py` & `moe-2.1.3/moe/list.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/moe_import/__init__.py` & `moe-2.1.3/moe/moe_import/__init__.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/moe_import/import_cli.py` & `moe-2.1.3/moe/moe_import/import_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/moe_import/import_core.py` & `moe-2.1.3/moe/moe_import/import_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/move/move_cli.py` & `moe-2.1.3/moe/move/move_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/move/move_core.py` & `moe-2.1.3/moe/move/move_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/query.py` & `moe-2.1.3/moe/query.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/read/read_cli.py` & `moe-2.1.3/moe/read/read_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/read/read_core.py` & `moe-2.1.3/moe/read/read_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/remove/rm_cli.py` & `moe-2.1.3/moe/remove/rm_cli.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/remove/rm_core.py` & `moe-2.1.3/moe/remove/rm_core.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/util/cli/prompt.py` & `moe-2.1.3/moe/util/cli/prompt.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/util/cli/query.py` & `moe-2.1.3/moe/util/cli/query.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/util/core/match.py` & `moe-2.1.3/moe/util/core/match.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/moe/write.py` & `moe-2.1.3/moe/write.py`

 * *Files identical despite different names*

### Comparing `moe-2.1.2/pyproject.toml` & `moe-2.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "Moe"
 include = ["alembic/*", "alembic/versions/*"]
-version = "2.1.2"
+version = "2.1.3"
 description = "The ultimate tool for managing your music library."
 authors = ["Jacob Pavlock <jtpavlock@gmail.com>"]
 repository = "https://github.com/MoeMusic/Moe"
 documentation = "https://mrmoe.readthedocs.io/en/latest/index.html"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License",
@@ -56,15 +56,15 @@
 [tool.poetry.group.docs.dependencies]
 furo = "*"
 pypandoc = "^1.9"
 Sphinx = "^7.0.0"
 
 [tool.commitizen]
 name = "cz_customize"
-version = "2.1.2"
+version = "2.1.3"
 version_files = [
     "pyproject.toml:^version",
 ]
 tag_format = "v$version"
 
 [tool.commitizen.customize]
 schema_pattern = '(build|ci|deprecate|docs|feat|fix|perf|refactor|release|style|test)(\(\w+\))?!?:\s\S.*'
```

### Comparing `moe-2.1.2/PKG-INFO` & `moe-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Moe
-Version: 2.1.2
+Version: 2.1.3
 Summary: The ultimate tool for managing your music library.
 Home-page: https://github.com/MoeMusic/Moe
 License: MIT
 Author: Jacob Pavlock
 Author-email: jtpavlock@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 5 - Production/Stable
```

