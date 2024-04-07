# Comparing `tmp/ckanext-files-0.2.2.tar.gz` & `tmp/ckanext-files-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-files-0.2.2.tar", last modified: Mon Mar 18 16:53:45 2024, max compression
+gzip compressed data, was "ckanext-files-0.2.3.tar", last modified: Sun Apr  7 16:20:42 2024, max compression
```

## Comparing `ckanext-files-0.2.2.tar` & `ckanext-files-0.2.3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.935404 ckanext-files-0.2.2/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-03-08 12:12:51.000000 ckanext-files-0.2.2/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2024-03-18 14:10:35.000000 ckanext-files-0.2.2/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-03-18 16:53:45.935404 ckanext-files-0.2.2/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14070 2024-03-13 11:29:37.000000 ckanext-files-0.2.2/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.918738 ckanext-files-0.2.2/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.918738 ckanext-files-0.2.2/ckanext/file_manager/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext-files-0.2.2/ckanext/file_manager/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/file_manager/collection.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/file_manager/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/file_manager/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.918738 ckanext-files-0.2.2/ckanext/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/ckanext/files/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.922071 ckanext-files-0.2.2/ckanext/files/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      185 2024-03-12 01:26:55.000000 ckanext-files-0.2.2/ckanext/files/assets/resource.config
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.922071 ckanext-files-0.2.2/ckanext/files/assets/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8250 2024-03-12 23:08:02.000000 ckanext-files-0.2.2/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    24988 2024-03-12 23:08:02.000000 ckanext-files-0.2.2/ckanext/files/assets/scripts/files--queue.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    39331 2024-03-12 23:22:40.000000 ckanext-files-0.2.2/ckanext/files/assets/scripts/files--shared.js
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.922071 ckanext-files-0.2.2/ckanext/files/assets/styles/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2024-03-10 22:56:48.000000 ckanext-files-0.2.2/ckanext/files/assets/styles/files--style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      358 2024-03-11 14:56:58.000000 ckanext-files-0.2.2/ckanext/files/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10850 2024-03-18 14:21:41.000000 ckanext-files-0.2.2/ckanext/files/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2024-03-18 14:21:43.000000 ckanext-files-0.2.2/ckanext/files/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1660 2024-03-13 15:43:29.000000 ckanext-files-0.2.2/ckanext/files/command.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2024-03-12 19:50:35.000000 ckanext-files-0.2.2/ckanext/files/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3588 2024-03-06 16:16:51.000000 ckanext-files-0.2.2/ckanext/files/exceptions.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-03-10 22:10:41.000000 ckanext-files-0.2.2/ckanext/files/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-03-06 13:53:18.000000 ckanext-files-0.2.2/ckanext/files/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.925404 ckanext-files-0.2.2/ckanext/files/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/ckanext/files/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9035 2024-03-13 16:05:56.000000 ckanext-files-0.2.2/ckanext/files/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3906 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2796 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2079 2024-03-11 23:03:53.000000 ckanext-files-0.2.2/ckanext/files/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.915405 ckanext-files-0.2.2/ckanext/files/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.925404 ckanext-files-0.2.2/ckanext/files/migration/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/ckanext/files/migration/files/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/files/migration/files/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/ckanext/files/migration/files/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.928738 ckanext-files-0.2.2/ckanext/files/migration/files/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-03-13 16:00:43.000000 ckanext-files-0.2.2/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2980 2024-03-13 11:24:07.000000 ckanext-files-0.2.2/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-03-10 22:10:40.000000 ckanext-files-0.2.2/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.928738 ckanext-files-0.2.2/ckanext/files/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-03-07 19:03:17.000000 ckanext-files-0.2.2/ckanext/files/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-03-06 11:39:37.000000 ckanext-files-0.2.2/ckanext/files/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1874 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/model/file.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-03-18 14:19:53.000000 ckanext-files-0.2.2/ckanext/files/model/owner.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-03-13 11:24:08.000000 ckanext-files-0.2.2/ckanext/files/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-03-06 12:02:59.000000 ckanext-files-0.2.2/ckanext/files/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.928738 ckanext-files-0.2.2/ckanext/files/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-03-06 16:19:48.000000 ckanext-files-0.2.2/ckanext/files/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7500 2024-03-13 17:24:04.000000 ckanext-files-0.2.2/ckanext/files/storage/fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10684 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/storage/google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4338 2024-03-18 14:21:43.000000 ckanext-files-0.2.2/ckanext/files/storage/redis.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.928738 ckanext-files-0.2.2/ckanext/files/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.915405 ckanext-files-0.2.2/ckanext/files/templates/files/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.928738 ckanext-files-0.2.2/ckanext/files/templates/files/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-03-10 22:58:04.000000 ckanext-files-0.2.2/ckanext/files/templates/files/snippets/_asset.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-03-12 01:26:55.000000 ckanext-files-0.2.2/ckanext/files/templates/files/snippets/_resource.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5129 2024-03-12 19:30:24.000000 ckanext-files-0.2.2/ckanext/files/templates/files/snippets/file_table.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2045 2024-03-12 19:30:24.000000 ckanext-files-0.2.2/ckanext/files/templates/files/snippets/uploader_v1.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.932071 ckanext-files-0.2.2/ckanext/files/templates/files/user/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-03-12 19:30:24.000000 ckanext-files-0.2.2/ckanext/files/templates/files/user/delete.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      793 2024-03-12 19:30:24.000000 ckanext-files-0.2.2/ckanext/files/templates/files/user/index.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-03-08 17:50:00.000000 ckanext-files-0.2.2/ckanext/files/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.932071 ckanext-files-0.2.2/ckanext/files/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/ckanext/files/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3477 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.932071 ckanext-files-0.2.2/ckanext/files/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/ckanext/files/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-03-11 23:03:53.000000 ckanext-files-0.2.2/ckanext/files/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-03-06 16:16:50.000000 ckanext-files-0.2.2/ckanext/files/tests/logic/test_validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.932071 ckanext-files-0.2.2/ckanext/files/tests/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-03-06 14:42:42.000000 ckanext-files-0.2.2/ckanext/files/tests/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-03-11 11:36:18.000000 ckanext-files-0.2.2/ckanext/files/tests/storage/test_fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10301 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/tests/storage/test_google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/tests/storage/test_redis.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    12019 2024-03-18 14:21:38.000000 ckanext-files-0.2.2/ckanext/files/tests/test_base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-03-11 23:03:53.000000 ckanext-files-0.2.2/ckanext/files/tests/test_config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-03-06 13:53:18.000000 ckanext-files-0.2.2/ckanext/files/tests/test_utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2024-03-13 17:23:30.000000 ckanext-files-0.2.2/ckanext/files/types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4099 2024-03-11 23:03:53.000000 ckanext-files-0.2.2/ckanext/files/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4293 2024-03-13 11:14:35.000000 ckanext-files-0.2.2/ckanext/files/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-03-18 16:53:45.932071 ckanext-files-0.2.2/ckanext_files.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-03-18 16:53:45.000000 ckanext-files-0.2.2/ckanext_files.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2987 2024-03-18 16:53:45.000000 ckanext-files-0.2.2/ckanext_files.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-03-18 16:53:45.000000 ckanext-files-0.2.2/ckanext_files.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      241 2024-03-18 16:53:45.000000 ckanext-files-0.2.2/ckanext_files.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-03-18 16:53:45.000000 ckanext-files-0.2.2/ckanext_files.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-03-18 16:53:45.000000 ckanext-files-0.2.2/ckanext_files.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-03-18 16:53:45.000000 ckanext-files-0.2.2/ckanext_files.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-03-13 11:11:59.000000 ckanext-files-0.2.2/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2000 2024-03-18 16:53:45.935404 ckanext-files-0.2.2/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext-files-0.2.2/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14070 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.456360 ckanext-files-0.2.3/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/file_manager/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext-files-0.2.3/ckanext/file_manager/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/file_manager/collection.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/file_manager/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/file_manager/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      185 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/resource.config
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/assets/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8250 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    26019 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/assets/scripts/files--queue.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    44982 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/assets/scripts/files--shared.js
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/assets/styles/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       54 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/styles/files--style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      358 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10850 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1355 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/command.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4113 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/exceptions.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9684 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3907 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2875 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2159 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.456360 ckanext-files-0.2.3/ckanext/files/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.459693 ckanext-files-0.2.3/ckanext/files/migration/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/migration/files/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/migration/files/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/migration/files/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2472 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/model/file.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/model/owner.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7500 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/storage/fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10667 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/storage/google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4465 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/storage/redis.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.456360 ckanext-files-0.2.3/ckanext/files/templates/files/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/_asset.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/_resource.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5129 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/file_table.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2045 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/snippets/uploader_v1.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/templates/files/user/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/user/delete.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      793 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/files/user/index.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3442 2024-04-07 16:20:32.000000 ckanext-files-0.2.3/ckanext/files/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/ckanext/files/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/logic/test_validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.463026 ckanext-files-0.2.3/ckanext/files/tests/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/test_fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10311 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/test_google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/storage/test_redis.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    12019 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/test_base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/test_config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/tests/test_utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4069 2024-04-07 14:32:45.000000 ckanext-files-0.2.3/ckanext/files/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4293 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/ckanext/files/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/ckanext_files.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2987 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      241 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-07 16:20:42.000000 ckanext-files-0.2.3/ckanext_files.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-04-01 12:19:47.000000 ckanext-files-0.2.3/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2000 2024-04-07 16:20:42.466359 ckanext-files-0.2.3/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext-files-0.2.3/setup.py
```

### Comparing `ckanext-files-0.2.2/LICENSE` & `ckanext-files-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/PKG-INFO` & `ckanext-files-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-files-0.2.2/README.md` & `ckanext-files-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/file_manager/collection.py` & `ckanext-files-0.2.3/ckanext/file_manager/collection.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/file_manager/plugin.py` & `ckanext-files-0.2.3/ckanext/file_manager/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/file_manager/views.py` & `ckanext-files-0.2.3/ckanext/file_manager/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js` & `ckanext-files-0.2.3/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/assets/scripts/files--queue.js` & `ckanext-files-0.2.3/ckanext/files/assets/scripts/files--queue.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,32 @@
 "use strict";
+/**
+ * Add selected file to upload queue whenever `[data-queue-scheduler]`
+ * dispatches `change` event.
+ *
+ */
 ckan.module("files--scheduler", function($) {
     return {
         initialize() {
             const scheduler = this.$("[data-queue-scheduler]");
             scheduler.on("change", (event) => this.push(...event.target.files));
         },
         push(...files) {
             files.forEach((file) => this.sandbox.publish(ckan.CKANEXT_FILES.topics.addFileToQueue, file));
         },
     };
 });
+/**
+ * Add to queue a file, that has associated incomplete upload.
+ *
+ * Supports a number of properties to verify that the new file matches
+ * previously uploaded file.
+ *
+ *
+ */
 ckan.module("files--restorer", function($) {
     return {
         options: {
             name: "",
             size: 0,
             uploaded: 0,
             id: "",
@@ -60,26 +73,28 @@
         teardown() {
             ckan.pubsub.unsubscribe(ckan.CKANEXT_FILES.topics.addFileToQueue, this._onFile);
             ckan.pubsub.unsubscribe(ckan.CKANEXT_FILES.topics.restoreFileInQueue, this._onFile);
         },
         _onFile(file, options = {
             id: "",
             uploaded: 0,
+            uploaderInstance: null,
             uploader: null,
             storage: null
         }) {
             const widget = this.tpl.clone(true).appendTo(this.el);
             const info = {
                 file,
                 id: options.id,
                 uploaded: options.uploaded || 0,
-                uploader: this.sandbox.files.makeUploader(options.uploader || this.options.uploader, {
+                uploader: options.uploaderInstance || this.sandbox.files.makeUploader(options.uploader || this.options.uploader, {
                     storage: options.storage || this.options.storage
                 }),
             };
+            console.log(info);
             this.widgets.set(widget[0], info);
             widget.on("click", "[data-upload-resume]", this._onWidgetResume);
             widget.on("click", "[data-upload-pause]", this._onWidgetPause);
             info.uploader.addEventListener("commit", (event) => (info.id = event.detail.id));
             info.uploader.addEventListener("fail", ({
                 detail: {
                     reasons,
@@ -175,8 +190,8 @@
                 .removeClass("bg-primary")
                 .addClass("bg-secondary");
             info.uploader.pause(info.file);
             this.toggleAnimation(widget, false);
         },
     };
 });
-//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXF1ZXVlLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vdHMvZmlsZXMtLXF1ZXVlLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7QUFBQSxJQUFJLENBQUMsTUFBTSxDQUFDLGtCQUFrQixFQUFFLFVBQVUsQ0FBQztJQUN6QyxPQUFPO1FBQ0wsVUFBVTtZQUNSLE1BQU0sU0FBUyxHQUFHLElBQUksQ0FBQyxDQUFDLENBQUMsd0JBQXdCLENBQUMsQ0FBQztZQUNuRCxTQUFTLENBQUMsRUFBRSxDQUFDLFFBQVEsRUFBRSxDQUFDLEtBQVksRUFBRSxFQUFFLENBQ3RDLElBQUksQ0FBQyxJQUFJLENBQUMsR0FBSSxLQUFLLENBQUMsTUFBMkIsQ0FBQyxLQUFNLENBQUMsQ0FDeEQsQ0FBQztRQUNKLENBQUM7UUFFRCxJQUFJLENBQUMsR0FBRyxLQUFhO1lBQ25CLEtBQUssQ0FBQyxPQUFPLENBQUMsQ0FBQyxJQUFJLEVBQUUsRUFBRSxDQUNyQixJQUFJLENBQUMsT0FBTyxDQUFDLE9BQU8sQ0FBQyxJQUFJLENBQUMsYUFBYSxDQUFDLE1BQU0sQ0FBQyxjQUFjLEVBQUUsSUFBSSxDQUFDLENBQ3JFLENBQUM7UUFDSixDQUFDO0tBQ0ssQ0FBQztBQUNYLENBQUMsQ0FBQyxDQUFDO0FBRUgsSUFBSSxDQUFDLE1BQU0sQ0FBQyxpQkFBaUIsRUFBRSxVQUFVLENBQUM7SUFDeEMsT0FBTztRQUNMLE9BQU8sRUFBRTtZQUNQLElBQUksRUFBRSxFQUFFO1lBQ1IsSUFBSSxFQUFFLENBQUM7WUFDUCxRQUFRLEVBQUUsQ0FBQztZQUNYLEVBQUUsRUFBRSxFQUFFO1NBQ1A7UUFFRCxVQUFVO1lBQ1IsQ0FBQyxDQUFDLFFBQVEsQ0FBQyxJQUFJLEVBQUUsS0FBSyxDQUFDLENBQUM7WUFDeEIsSUFBSSxDQUFDLEVBQUUsQ0FBQyxFQUFFLENBQUMsUUFBUSxFQUFFLElBQUksQ0FBQyxTQUFTLENBQUMsQ0FBQztRQUN2QyxDQUFDO1FBRUQsU0FBUyxDQUFD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LGVBQWUsQ0FBQyxNQUFNLEVBQUUsSUFBSSxDQUFDLENBQUM7UUFDckMsQ0FBQztRQUVELGNBQWMsQ0FBQyxLQUE0QjtZQUN6QyxNQUFNLElBQUksR0FBRyxJQUFJLENBQUMsT0FBTyxDQUFDLEdBQUcsQ0FBQyxLQUFLLENBQUMsY0FBYyxDQUFDLENBQUM7WUFDcEQsSUFBSSxJQUFJLENBQUMsUUFBUSxJQUFJLElBQUksQ0FBQyxLQUFLO2dCQUFFLE9BQU87WUFFeEMsTUFBTSxNQUFNLEdBQUcsQ0FBQyxDQUFDLEtBQUssQ0FBQyxjQUFjLENBQUMsQ0FBQztZQUN2QyxNQUFNO2lCQUNILElBQUksQ0FBQyx3QkFBd0IsQ0FBQztpQkFDOUIsV0FBVyxDQUFDLFlBQVksQ0FBQztpQkFDekIsUUFBUSxDQUFDLGNBQWMsQ0FBQyxDQUFDO1lBRTVCLElBQUksQ0FBQyxRQUFRLENBQUMsS0FBSyxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsQ0FBQztZQUMvQixJQUFJLENBQUMsZUFBZSxDQUFDLE1BQU0sRUFBRSxLQUFLLENBQUMsQ0FBQztRQUN0QyxDQUFDO0tBQ0YsQ0FBQztBQUNKLENBQUMsQ0FBQyxDQUFDIiwic291cmNlc0NvbnRlbnQiOlsiY2thbi5tb2R1bGUoXCJmaWxlcy0tc2NoZWR1bGVyXCIsIGZ1bmN0aW9uICgkKSB7XG4gIHJldHVybiB7XG4gICAgaW5pdGlhbGl6ZSgpIHtcbiAgICAgIGNvbnN0IHNjaGVkdWxlciA9IHRoaXMuJChcIltkYXRhLXF1ZXVlLXNjaGVkdWxlcl1cIik7XG4gICAgICBzY2hlZHVsZXIub24oXCJjaGFuZ2VcIiwgKGV2ZW50OiBFdmVudCkgPT5cbiAgICAgICAgdGhpcy5wdXNoKC4uLihldmVudC50YXJnZXQgYXMgSFRNTElucHV0RWxlbWVudCkuZmlsZXMhKSxcbiAgICAgICk7XG4gICAgfSxcblxuICAgIHB1c2goLi4uZmlsZXM6IEZpbGVbXSkge1xuICAgICAgZmlsZXMuZm9yRWFjaCgoZmlsZSkgPT5cbiAgICAgICAgdGhpcy5zYW5kYm94LnB1Ymxpc2goY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5hZGRGaWxlVG9RdWV1ZSwgZmlsZSksXG4gICAgICApO1xuICAgIH0sXG4gIH0gYXMgYW55O1xufSk7XG5cbmNrYW4ubW9kdWxlKFwiZmlsZXMtLXJlc3RvcmVyXCIsIGZ1bmN0aW9uICgkKSB7XG4gIHJldHVybiB7XG4gICAgb3B0aW9uczoge1xuICAgICAgbmFtZTogXCJcIixcbiAgICAgIHNpemU6IDAsXG4gICAgICB1cGxvYWRlZDogMCxcbiAgICAgIGlkOiBcIlwiLFxuICAgIH0sXG5cbiAgICBpbml0aWFsaXplKCkge1xuICAgICAgJC5wcm94eUFsbCh0aGlzLCAvX29uLyk7XG4gICAgICB0aGlzLmVsLm9uKFwiY2hhbmdlXCIsIHRoaXMuX29uQ2hhbmdlKTtcbiAgICB9LFxuXG4gICAgX29uQ2hhbmdlKGV2ZW50OiBFdmVudCkge1xuICAgICAgY29uc3QgZmlsZSA9IChldmVudC50YXJnZXQgYXMgSFRNTElucHV0RWxlbWVudCkuZmlsZXM/LlswXTtcblxuICAgICAgaWYgKCFmaWxlKSB7XG4gICAgICAgIHJldHVybjtcbiAgICAgIH1cblxuICAgICAgaWYgKHRoaXMub3B0aW9ucy5uYW1lICYmIGZpbGUubmFtZSAhPT0gdGhpcy5vcHRpb25zLm5hbWUpIHtcbiAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeShcbiAgICAgICAgICBcIk5hbWUgbWlzbWF0Y2guXCIsXG4gICAgICAgICAgYEV4cGVjdGVkIG5hbWU6ICR7dGhpcy5vcHRpb25zLm5hbWV9YCxcbiAgICAgICAgKTtcbiAgICAgICAgcmV0dXJuO1xuICAgICAgfVxuXG4gICAgICBpZiAodGhpcy5vcHRpb25zLnNpemUgJiYgZmlsZS5zaXplICE9PSB0aGlzLm9wdGlvbnMuc2l6ZSkge1xuICAgICAgICB0aGlzLnNhbmRib3gubm90aWZ5KFxuICAgICAgICAgIFwiU2l6ZSBtaXNtYXRjaC5cIixcbiAgICAgICAgICBgRXhwZWN0ZWQgc2l6ZTogJHt0aGlzLm9wdGlvbnMuc2l6ZS50b0xvY2FsZVN0cmluZygpfSBieXRlc2AsXG4gICAgICAgICk7XG4gICAgICAgIHJldHVybjtcbiAgICAgIH1cblxuICAgICAgdGhpcy5zYW5kYm94LnB1Ymxpc2goY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5yZXN0b3JlRmlsZUluUXVldWUsIGZpbGUsIHtcbiAgICAgICAgaWQ6IHRoaXMub3B0aW9ucy5pZCxcbiAgICAgICAgdXBsb2FkZWQ6IHRoaXMub3B0aW9ucy51cGxvYWRlZCxcbiAgICAgIH0pO1xuICAgIH0sXG4gIH07XG59KTtcbmNrYW4ubW9kdWxlKFwiZmlsZXMtLXF1ZXVlXCIsIGZ1bmN0aW9uICgkKSB7XG4gIHJldHVybiB7XG4gICAgb3B0aW9uczoge1xuICAgICAgc3RvcmFnZTogXCJkZWZhdWx0XCIsXG4gICAgICB1cGxvYWRlcjogXCJTdGFuZGFyZFwiLFxuICAgIH0sXG5cbiAgICBpbml0aWFsaXplKCkge1xuICAgICAgJC5wcm94eUFsbCh0aGlzLCAvX29uLyk7XG4gICAgICBja2FuLnB1YnN1Yi5zdWJzY3JpYmUoXG4gICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MuYWRkRmlsZVRvUXVldWUsXG4gICAgICAgIHRoaXMuX29uRmlsZSxcbiAgICAgICk7XG4gICAgICBja2FuLnB1YnN1Yi5zdWJzY3JpYmUoXG4gICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MucmVzdG9yZUZpbGVJblF1ZXVlLFxuICAgICAgICB0aGlzLl9vbkZpbGUsXG4gICAgICApO1xuXG4gICAgICB0aGlzLnRwbCA9IHRoaXMuJChcIltkYXRhLXVwbG9hZC10ZW1wbGF0ZV1cIilcbiAgICAgICAgLnJlbW92ZSgpXG4gICAgICAgIC5yZW1vdmVBdHRyKFwiZGF0YS11cGxvYWQtdGVtcGxhdGUgaGlkZGVuXCIpO1xuXG4gICAgICB0aGlzLndpZGdldHMgPSBuZXcgV2Vha01hcCgpO1xuICAgIH0sXG5cbiAgICB0ZWFyZG93bigpIHtcbiAgICAgIGNrYW4ucHVic3ViLnVuc3Vic2NyaWJlKFxuICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLmFkZEZpbGVUb1F1ZXVlLFxuICAgICAgICB0aGlzLl9vbkZpbGUsXG4gICAgICApO1xuICAgICAgY2thbi5wdWJzdWIudW5zdWJzY3JpYmUoXG4gICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MucmVzdG9yZUZpbGVJblF1ZXVlLFxuICAgICAgICB0aGlzLl9vbkZpbGUsXG4gICAgICApO1xuICAgIH0sXG5cbiAgICBfb25GaWxlKFxuICAgICAgZmlsZTogRmlsZSxcbiAgICAgIG9wdGlvbnMgPSB7IGlkOiBcIlwiLCB1cGxvYWRlZDogMCwgdXBsb2FkZXI6IG51bGwsIHN0b3JhZ2U6IG51bGwgfSxcbiAgICApIHtcbiAgICAgIGNvbnN0IHdpZGdldCA9IHRoaXMudHBsLmNsb25lKHRydWUpLmFwcGVuZFRvKHRoaXMuZWwpO1xuICAgICAgY29uc3QgaW5mbyA9IHtcbiAgICAgICAgZmlsZSxcbiAgICAgICAgaWQ6IG9wdGlvbnMuaWQsXG4gICAgICAgIHVwbG9hZGVkOiBvcHRpb25zLnVwbG9hZGVkIHx8IDAsXG4gICAgICAgIHVwbG9hZGVyOiB0aGlzLnNhbmRib3guZmlsZXMubWFrZVVwbG9hZGVyKFxuICAgICAgICAgIG9wdGlvbnMudXBsb2FkZXIgfHwgdGhpcy5vcHRpb25zLnVwbG9hZGVyLFxuICAgICAgICAgIHsgc3RvcmFnZTogb3B0aW9ucy5zdG9yYWdlIHx8IHRoaXMub3B0aW9ucy5zdG9yYWdlIH0sXG4gICAgICAgICksXG4gICAgICB9O1xuXG4gICAgICB0aGlzLndpZGdldHMuc2V0KHdpZGdldFswXSwgaW5mbyk7XG5cbiAgICAgIHdpZGdldC5vbihcImNsaWNrXCIsIFwiW2RhdGEtdXBsb2FkLXJlc3VtZV1cIiwgdGhpcy5fb25XaWRnZXRSZXN1bWUpO1xuICAgICAgd2lkZ2V0Lm9uKFwiY2xpY2tcIiwgXCJbZGF0YS11cGxvYWQtcGF1c2VdXCIsIHRoaXMuX29uV2lkZ2V0UGF1c2UpO1xuXG4gICAgICBpbmZvLnVwbG9hZGVyLmFkZEV2ZW50TGlzdGVuZXIoXG4gICAgICAgIFwiY29tbWl0XCIsXG4gICAgICAgIChldmVudDogQ3VzdG9tRXZlbnQpID0+IChpbmZvLmlkID0gZXZlbnQuZGV0YWlsLmlkKSxcbiAgICAgICk7XG4gICAgICBpbmZvLnVwbG9hZGVyLmFkZEV2ZW50TGlzdGVuZXIoXG4gICAgICAgIFwiZmFpbFwiLFxuICAgICAgICAoe1xuICAgICAgICAgIGRldGFpbDogeyByZWFzb25zLCBmaWxlIH0sXG4gICAgICAgIH06IEN1c3RvbUV2ZW50PHtcbiAgICAgICAgICByZWFzb25zOiB7IFtrZXk6IHN0cmluZ106IHN0cmluZ1tdIH07XG4gICAgICAgICAgZmlsZTogRmlsZTtcbiAgICAgICAgfT4pID0+IHtcbiAgICAgICAgICB0aGlzLnNhbmRib3gubm90aWZ5KFxuICAgICAgICAgICAgZmlsZS5uYW1lLFxuICAgICAgICAgICAgT2JqZWN0LmVudHJpZXMocmVhc29ucylcbiAgICAgICAgICAgICAgLmZpbHRlcigoW2ssIHZdKSA9PiBrWzBdICE9PSBcIl9cIilcbiAgICAgICAgICAgICAgLm1hcCgoW2ssIHZdKSA9PiAoQXJyYXkuaXNBcnJheSh2KSA/IHYuam9pbihcIjsgXCIpIDogdikpXG4gICAgICAgICAgICAgIC5qb2luKFwiOyBcIiksXG4gICAgICAgICAgKTtcbiAgICAgICAgICB0aGlzLnRvZ2dsZUFuaW1hdGlvbih3aWRnZXQsIGZhbHNlKTtcblxuICAgICAgICAgIHdpZGdldFxuICAgICAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgICAgICAucmVtb3ZlQ2xhc3MoXCJiZy1wcmltYXJ5IGJnLXNlY29uZGFyeVwiKVxuICAgICAgICAgICAgLmFkZENsYXNzKFwiYmctZGFuZ2VyIHByb2dyZXNzLWJhci1kYW5nZXJcIik7XG4gICAgICAgIH0sXG4gICAgICApO1xuICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICBcImVycm9yXCIsXG4gICAgICAgICh7XG4gICAgICAgICAgZGV0YWlsOiB7IG1lc3NhZ2UsIGZpbGUgfSxcbiAgICAgICAgfTogQ3VzdG9tRXZlbnQ8eyBtZXNzYWdlOiBzdHJpbmc7IGZpbGU6IEZpbGUgfT4pID0+IHtcbiAgICAgICAgICB0aGlzLnNhbmRib3gubm90aWZ5KGZpbGUubmFtZSwgbWVzc2FnZSk7XG4gICAgICAgICAgdGhpcy50b2dnbGVBbmltYXRpb24od2lkZ2V0LCBmYWxzZSk7XG4gICAgICAgICAgd2lkZ2V0XG4gICAgICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgICAgIC5yZW1vdmVDbGFzcyhcImJnLXByaW1hcnkgYmctc2Vjb25kYXJ5XCIpXG4gICAgICAgICAgICAuYWRkQ2xhc3MoXCJiZy1kYW5nZXIgcHJvZ3Jlc3MtYmFyLWRhbmdlclwiKTtcbiAgICAgICAgfSxcbiAgICAgICk7XG5cbiAgICAgIGluZm8udXBsb2FkZXIuYWRkRXZlbnRMaXN0ZW5lcihcbiAgICAgICAgXCJwcm9ncmVzc1wiLFxuICAgICAgICAoeyBkZXRhaWw6IHsgbG9hZGVkLCB0b3RhbCB9IH06IEN1c3RvbUV2ZW50KSA9PlxuICAgICAgICAgIHRoaXMuc2V0V2lkZ2V0Q29tcGxldGlvbih3aWRnZXQsIGxvYWRlZCwgdG90YWwpLFxuICAgICAgKTtcbiAgICAgIGluZm8udXBsb2FkZXIuYWRkRXZlbnRMaXN0ZW5lcihcbiAgICAgICAgXCJmaW5pc2hcIixcbiAgICAgICAgKHsgZGV0YWlsOiB7IGZpbGUsIHJlc3VsdCB9IH06IEN1c3RvbUV2ZW50KSA9PiB7XG4gICAgICAgICAgdGhpcy50b2dnbGVBbmltYXRpb24od2lkZ2V0LCBmYWxzZSk7XG4gICAgICAgICAgd2lkZ2V0XG4gICAgICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgICAgIC5yZW1vdmVDbGFzcyhcImJnLXByaW1hcnkgYmctc2Vjb25kYXJ5XCIpXG4gICAgICAgICAgICAuYWRkQ2xhc3MoXCJiZy1zdWNjZXNzIHByb2dyZXNzLWJhci1zdWNjZXNzXCIpO1xuICAgICAgICAgIHRoaXMuc2FuZGJveC5wdWJsaXNoKFxuICAgICAgICAgICAgY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5xdWV1ZUl0ZW1VcGxvYWRlZCxcbiAgICAgICAgICAgIGZpbGUsXG4gICAgICAgICAgICByZXN1bHQsXG4gICAgICAgICAgKTtcbiAgICAgICAgfSxcbiAgICAgICk7XG5cbiAgICAgIHRoaXMuc2V0V2lkZ2V0TmFtZSh3aWRnZXQsIGluZm8uZmlsZS5uYW1lKTtcbiAgICAgIHRoaXMuc2V0V2lkZ2V0Q29tcGxldGlvbih3aWRnZXQsIGluZm8udXBsb2FkZWQsIGluZm8uZmlsZS5zaXplKTtcbiAgICB9LFxuXG4gICAgc2V0V2lkZ2V0TmFtZSh3aWRnZXQ6IEpRdWVyeSwgbmFtZTogc3RyaW5nKSB7XG4gICAgICB3aWRnZXQuZmluZChcIltkYXRhLWl0ZW0tbmFtZV1cIikudGV4dChuYW1lKTtcbiAgICB9LFxuXG4gICAgc2V0V2lkZ2V0Q29tcGxldGlvbih3aWRnZXQ6IEpRdWVyeSwgdXBsb2FkZWQ6IG51bWJlciwgdG90YWw6IG51bWJlcikge1xuICAgICAgY29uc3QgdmFsdWUgPSAodXBsb2FkZWQgKiAxMDApIC8gdG90YWw7XG4gICAgICBjb25zdCBpbmZvID0gdGhpcy53aWRnZXRzLmdldCh3aWRnZXRbMF0pO1xuICAgICAgaW5mby51cGxvYWRlZCA9IHVwbG9hZGVkO1xuXG4gICAgICBjb25zdCBjb21wbGV0aW9uID0gdmFsdWUudG9GaXhlZCgwKSArIFwiJVwiO1xuICAgICAgd2lkZ2V0XG4gICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAudGV4dChjb21wbGV0aW9uKVxuICAgICAgICAuY3NzKFwid2lkdGhcIiwgY29tcGxldGlvbik7XG4gICAgfSxcblxuICAgIHRvZ2dsZUFuaW1hdGlvbih3aWRnZXQ6IEpRdWVyeSwgc3RhdGU6IGJvb2xlYW4pIHtcbiAgICAgIHdpZGdldFxuICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgLnRvZ2dsZUNsYXNzKFwicHJvZ3Jlc3MtYmFyLWFuaW1hdGVkIGFjdGl2ZVwiLCBzdGF0ZSk7XG4gICAgfSxcblxuICAgIF9vbldpZGdldFJlc3VtZShldmVudDogSlF1ZXJ5LlRyaWdnZXJlZEV2ZW50KSB7XG4gICAgICBjb25zdCBpbmZvID0gdGhpcy53aWRnZXRzLmdldChldmVudC5kZWxlZ2F0ZVRhcmdldCk7XG4gICAgICBpZiAoaW5mby51cGxvYWRlZCA+PSBpbmZvLnRvdGFsKSByZXR1cm47XG5cbiAgICAgIGNvbnN0IHdpZGdldCA9ICQoZXZlbnQuZGVsZWdhdGVUYXJnZXQpO1xuICAgICAgd2lkZ2V0XG4gICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAucmVtb3ZlQ2xhc3MoXCJiZy1zZWNvbmRhcnlcIilcbiAgICAgICAgLmFkZENsYXNzKFwiYmctcHJpbWFyeVwiKTtcblxuICAgICAgaWYgKGluZm8uaWQpIHtcbiAgICAgICAgaW5mby51cGxvYWRlci5yZXN1bWUoaW5mby5maWxlLCBpbmZvLmlkKTtcbiAgICAgIH0gZWxzZSB7XG4gICAgICAgIGluZm8udXBsb2FkZXIudXBsb2FkKGluZm8uZmlsZSk7XG4gICAgICB9XG5cbiAgICAgIHRoaXMudG9nZ2xlQW5pbWF0aW9uKHdpZGdldCwgdHJ1ZSk7XG4gICAgfSxcblxuICAgIF9vbldpZGdldFBhdXNlKGV2ZW50OiBKUXVlcnkuVHJpZ2dlcmVkRXZlbnQpIHtcbiAgICAgIGNvbnN0IGluZm8gPSB0aGlzLndpZGdldHMuZ2V0KGV2ZW50LmRlbGVnYXRlVGFyZ2V0KTtcbiAgICAgIGlmIChpbmZvLnVwbG9hZGVkID49IGluZm8udG90YWwpIHJldHVybjtcblxuICAgICAgY29uc3Qgd2lkZ2V0ID0gJChldmVudC5kZWxlZ2F0ZVRhcmdldCk7XG4gICAgICB3aWRnZXRcbiAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgIC5yZW1vdmVDbGFzcyhcImJnLXByaW1hcnlcIilcbiAgICAgICAgLmFkZENsYXNzKFwiYmctc2Vjb25kYXJ5XCIpO1xuXG4gICAgICBpbmZvLnVwbG9hZGVyLnBhdXNlKGluZm8uZmlsZSk7XG4gICAgICB0aGlzLnRvZ2dsZUFuaW1hdGlvbih3aWRnZXQsIGZhbHNlKTtcbiAgICB9LFxuICB9O1xufSk7XG4iXX0=
+//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXF1ZXVlLmpzIiwic291cmNlUm9vdCI6IiIsInNvdXJjZXMiOlsiLi4vdHMvZmlsZXMtLXF1ZXVlLnRzIl0sIm5hbWVzIjpbXSwibWFwcGluZ3MiOiI7QUFBQTs7OztHQUlHO0FBQ0gsSUFBSSxDQUFDLE1BQU0sQ0FBQyxrQkFBa0IsRUFBRSxVQUFVLENBQUM7SUFDekMsT0FBTztRQUNMLFVBQVU7WUFDUixNQUFNLFNBQVMsR0FBRyxJQUFJLENBQUMsQ0FBQyxDQUFDLHdCQUF3QixDQUFDLENBQUM7WUFDbkQsU0FBUyxDQUFDLEVBQUUsQ0FBQyxRQUFRLEVBQUUsQ0FBQyxLQUFZLEVBQUUsRUFBRSxDQUN0QyxJQUFJLENBQUMsSUFBSSxDQUFDLEdBQUksS0FBSyxDQUFDLE1BQTJCLENBQUMsS0FBTSxDQUFDLENBQ3hELENBQUM7UUFDSixDQUFDO1FBRUQsSUFBSSxDQUFDLEdBQUcsS0FBYTtZQUNuQixLQUFLLENBQUMsT0FBTyxDQUFDLENBQUMsSUFBSSxFQUFFLEVBQUUsQ0FDckIsSUFBSSxDQUFDLE9BQU8sQ0FBQyxPQUFPLENBQUMsSUFBSSxDQUFDLGFBQWEsQ0FBQyxNQUFNLENBQUMsY0FBYyxFQUFFLElBQUksQ0FBQyxDQUNyRSxDQUFDO1FBQ0osQ0FBQztLQUNGLENBQUM7QUFDSixDQUFDLENBQUMsQ0FBQztBQUVIOzs7Ozs7O0dBT0c7QUFDSCxJQUFJLENBQUMsTUFBTSxDQUFDLGlCQUFpQixFQUFFLFVBQVUsQ0FBQztJQUN4QyxPQUFPO1FBQ0wsT0FBTyxFQUFFO1lBQ1AsSUFBSSxFQUFFLEVBQUU7WUFDUixJQUFJLEVBQUUsQ0FBQztZQUNQLFFBQVEsRUFBRSxDQUFDO1lBQ1gsRUFBRSxFQUFFLEVBQUU7U0FDUDtRQUVELFVBQVU7WUFDUixDQUFDLENBQUMsUUFBUSxDQUFDLElBQUksRUFBRSxLQUFLLENBQUMsQ0FBQztZQUN4QixJQUFJLENBQUMsRUFBRSxDQUFDLEVBQUUsQ0FBQyxRQUFRLEVBQUUsSUFBSSxDQUFDLFNBQVMsQ0FBQyxD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LENBQUM7WUFDM0MsQ0FBQztpQkFBTSxDQUFDO2dCQUNOLElBQUksQ0FBQyxRQUFRLENBQUMsTUFBTSxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsQ0FBQztZQUNsQyxDQUFDO1lBRUQsSUFBSSxDQUFDLGVBQWUsQ0FBQyxNQUFNLEVBQUUsSUFBSSxDQUFDLENBQUM7UUFDckMsQ0FBQztRQUVELGNBQWMsQ0FBQyxLQUE0QjtZQUN6QyxNQUFNLElBQUksR0FBRyxJQUFJLENBQUMsT0FBTyxDQUFDLEdBQUcsQ0FBQyxLQUFLLENBQUMsY0FBYyxDQUFDLENBQUM7WUFDcEQsSUFBSSxJQUFJLENBQUMsUUFBUSxJQUFJLElBQUksQ0FBQyxLQUFLO2dCQUFFLE9BQU87WUFFeEMsTUFBTSxNQUFNLEdBQUcsQ0FBQyxDQUFDLEtBQUssQ0FBQyxjQUFjLENBQUMsQ0FBQztZQUN2QyxNQUFNO2lCQUNILElBQUksQ0FBQyx3QkFBd0IsQ0FBQztpQkFDOUIsV0FBVyxDQUFDLFlBQVksQ0FBQztpQkFDekIsUUFBUSxDQUFDLGNBQWMsQ0FBQyxDQUFDO1lBRTVCLElBQUksQ0FBQyxRQUFRLENBQUMsS0FBSyxDQUFDLElBQUksQ0FBQyxJQUFJLENBQUMsQ0FBQztZQUMvQixJQUFJLENBQUMsZUFBZSxDQUFDLE1BQU0sRUFBRSxLQUFLLENBQUMsQ0FBQztRQUN0QyxDQUFDO0tBQ0YsQ0FBQztBQUNKLENBQUMsQ0FBQyxDQUFDIiwic291cmNlc0NvbnRlbnQiOlsiLyoqXG4gKiBBZGQgc2VsZWN0ZWQgZmlsZSB0byB1cGxvYWQgcXVldWUgd2hlbmV2ZXIgYFtkYXRhLXF1ZXVlLXNjaGVkdWxlcl1gXG4gKiBkaXNwYXRjaGVzIGBjaGFuZ2VgIGV2ZW50LlxuICpcbiAqL1xuY2thbi5tb2R1bGUoXCJmaWxlcy0tc2NoZWR1bGVyXCIsIGZ1bmN0aW9uICgkKSB7XG4gIHJldHVybiB7XG4gICAgaW5pdGlhbGl6ZSgpIHtcbiAgICAgIGNvbnN0IHNjaGVkdWxlciA9IHRoaXMuJChcIltkYXRhLXF1ZXVlLXNjaGVkdWxlcl1cIik7XG4gICAgICBzY2hlZHVsZXIub24oXCJjaGFuZ2VcIiwgKGV2ZW50OiBFdmVudCkgPT5cbiAgICAgICAgdGhpcy5wdXNoKC4uLihldmVudC50YXJnZXQgYXMgSFRNTElucHV0RWxlbWVudCkuZmlsZXMhKSxcbiAgICAgICk7XG4gICAgfSxcblxuICAgIHB1c2goLi4uZmlsZXM6IEZpbGVbXSkge1xuICAgICAgZmlsZXMuZm9yRWFjaCgoZmlsZSkgPT5cbiAgICAgICAgdGhpcy5zYW5kYm94LnB1Ymxpc2goY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5hZGRGaWxlVG9RdWV1ZSwgZmlsZSksXG4gICAgICApO1xuICAgIH0sXG4gIH07XG59KTtcblxuLyoqXG4gKiBBZGQgdG8gcXVldWUgYSBmaWxlLCB0aGF0IGhhcyBhc3NvY2lhdGVkIGluY29tcGxldGUgdXBsb2FkLlxuICpcbiAqIFN1cHBvcnRzIGEgbnVtYmVyIG9mIHByb3BlcnRpZXMgdG8gdmVyaWZ5IHRoYXQgdGhlIG5ldyBmaWxlIG1hdGNoZXNcbiAqIHByZXZpb3VzbHkgdXBsb2FkZWQgZmlsZS5cbiAqXG4gKlxuICovXG5ja2FuLm1vZHVsZShcImZpbGVzLS1yZXN0b3JlclwiLCBmdW5jdGlvbiAoJCkge1xuICByZXR1cm4ge1xuICAgIG9wdGlvbnM6IHtcbiAgICAgIG5hbWU6IFwiXCIsXG4gICAgICBzaXplOiAwLFxuICAgICAgdXBsb2FkZWQ6IDAsXG4gICAgICBpZDogXCJcIixcbiAgICB9LFxuXG4gICAgaW5pdGlhbGl6ZSgpIHtcbiAgICAgICQucHJveHlBbGwodGhpcywgL19vbi8pO1xuICAgICAgdGhpcy5lbC5vbihcImNoYW5nZVwiLCB0aGlzLl9vbkNoYW5nZSk7XG4gICAgfSxcblxuICAgIF9vbkNoYW5nZShldmVudDogRXZlbnQpIHtcbiAgICAgIGNvbnN0IGZpbGUgPSAoZXZlbnQudGFyZ2V0IGFzIEhUTUxJbnB1dEVsZW1lbnQpLmZpbGVzPy5bMF07XG5cbiAgICAgIGlmICghZmlsZSkge1xuICAgICAgICByZXR1cm47XG4gICAgICB9XG5cbiAgICAgIGlmICh0aGlzLm9wdGlvbnMubmFtZSAmJiBmaWxlLm5hbWUgIT09IHRoaXMub3B0aW9ucy5uYW1lKSB7XG4gICAgICAgIHRoaXMuc2FuZGJveC5ub3RpZnkoXG4gICAgICAgICAgXCJOYW1lIG1pc21hdGNoLlwiLFxuICAgICAgICAgIGBFeHBlY3RlZCBuYW1lOiAke3RoaXMub3B0aW9ucy5uYW1lfWAsXG4gICAgICAgICk7XG4gICAgICAgIHJldHVybjtcbiAgICAgIH1cblxuICAgICAgaWYgKHRoaXMub3B0aW9ucy5zaXplICYmIGZpbGUuc2l6ZSAhPT0gdGhpcy5vcHRpb25zLnNpemUpIHtcbiAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeShcbiAgICAgICAgICBcIlNpemUgbWlzbWF0Y2guXCIsXG4gICAgICAgICAgYEV4cGVjdGVkIHNpemU6ICR7dGhpcy5vcHRpb25zLnNpemUudG9Mb2NhbGVTdHJpbmcoKX0gYnl0ZXNgLFxuICAgICAgICApO1xuICAgICAgICByZXR1cm47XG4gICAgICB9XG5cbiAgICAgIHRoaXMuc2FuZGJveC5wdWJsaXNoKGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MucmVzdG9yZUZpbGVJblF1ZXVlLCBmaWxlLCB7XG4gICAgICAgIGlkOiB0aGlzLm9wdGlvbnMuaWQsXG4gICAgICAgIHVwbG9hZGVkOiB0aGlzLm9wdGlvbnMudXBsb2FkZWQsXG4gICAgICB9KTtcbiAgICB9LFxuICB9O1xufSk7XG5ja2FuLm1vZHVsZShcImZpbGVzLS1xdWV1ZVwiLCBmdW5jdGlvbiAoJCkge1xuICByZXR1cm4ge1xuICAgIG9wdGlvbnM6IHtcbiAgICAgIHN0b3JhZ2U6IFwiZGVmYXVsdFwiLFxuICAgICAgdXBsb2FkZXI6IFwiU3RhbmRhcmRcIixcbiAgICB9LFxuXG4gICAgaW5pdGlhbGl6ZSgpIHtcbiAgICAgICQucHJveHlBbGwodGhpcywgL19vbi8pO1xuICAgICAgY2thbi5wdWJzdWIuc3Vic2NyaWJlKFxuICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLmFkZEZpbGVUb1F1ZXVlLFxuICAgICAgICB0aGlzLl9vbkZpbGUsXG4gICAgICApO1xuICAgICAgY2thbi5wdWJzdWIuc3Vic2NyaWJlKFxuICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLnJlc3RvcmVGaWxlSW5RdWV1ZSxcbiAgICAgICAgdGhpcy5fb25GaWxlLFxuICAgICAgKTtcblxuICAgICAgdGhpcy50cGwgPSB0aGlzLiQoXCJbZGF0YS11cGxvYWQtdGVtcGxhdGVdXCIpXG4gICAgICAgIC5yZW1vdmUoKVxuICAgICAgICAucmVtb3ZlQXR0cihcImRhdGEtdXBsb2FkLXRlbXBsYXRlIGhpZGRlblwiKTtcblxuICAgICAgdGhpcy53aWRnZXRzID0gbmV3IFdlYWtNYXAoKTtcbiAgICB9LFxuXG4gICAgdGVhcmRvd24oKSB7XG4gICAgICBja2FuLnB1YnN1Yi51bnN1YnNjcmliZShcbiAgICAgICAgY2thbi5DS0FORVhUX0ZJTEVTLnRvcGljcy5hZGRGaWxlVG9RdWV1ZSxcbiAgICAgICAgdGhpcy5fb25GaWxlLFxuICAgICAgKTtcbiAgICAgIGNrYW4ucHVic3ViLnVuc3Vic2NyaWJlKFxuICAgICAgICBja2FuLkNLQU5FWFRfRklMRVMudG9waWNzLnJlc3RvcmVGaWxlSW5RdWV1ZSxcbiAgICAgICAgdGhpcy5fb25GaWxlLFxuICAgICAgKTtcbiAgICB9LFxuXG4gICAgX29uRmlsZShcbiAgICAgIGZpbGU6IEZpbGUsXG4gICAgICAgIG9wdGlvbnMgPSB7IGlkOiBcIlwiLCB1cGxvYWRlZDogMCwgdXBsb2FkZXJJbnN0YW5jZTogbnVsbCwgdXBsb2FkZXI6IG51bGwsIHN0b3JhZ2U6IG51bGwgfSxcbiAgICApIHtcbiAgICAgIGNvbnN0IHdpZGdldCA9IHRoaXMudHBsLmNsb25lKHRydWUpLmFwcGVuZFRvKHRoaXMuZWwpO1xuICAgICAgY29uc3QgaW5mbyA9IHtcbiAgICAgICAgZmlsZSxcbiAgICAgICAgaWQ6IG9wdGlvbnMuaWQsXG4gICAgICAgIHVwbG9hZGVkOiBvcHRpb25zLnVwbG9hZGVkIHx8IDAsXG4gICAgICAgIHVwbG9hZGVyOiBvcHRpb25zLnVwbG9hZGVySW5zdGFuY2UgfHwgdGhpcy5zYW5kYm94LmZpbGVzLm1ha2VVcGxvYWRlcihcbiAgICAgICAgICBvcHRpb25zLnVwbG9hZGVyIHx8IHRoaXMub3B0aW9ucy51cGxvYWRlcixcbiAgICAgICAgICB7IHN0b3JhZ2U6IG9wdGlvbnMuc3RvcmFnZSB8fCB0aGlzLm9wdGlvbnMuc3RvcmFnZSB9LFxuICAgICAgICApLFxuICAgICAgfTtcblxuICAgICAgICBjb25zb2xlLmxvZyhpbmZvKVxuICAgICAgdGhpcy53aWRnZXRzLnNldCh3aWRnZXRbMF0sIGluZm8pO1xuXG4gICAgICB3aWRnZXQub24oXCJjbGlja1wiLCBcIltkYXRhLXVwbG9hZC1yZXN1bWVdXCIsIHRoaXMuX29uV2lkZ2V0UmVzdW1lKTtcbiAgICAgIHdpZGdldC5vbihcImNsaWNrXCIsIFwiW2RhdGEtdXBsb2FkLXBhdXNlXVwiLCB0aGlzLl9vbldpZGdldFBhdXNlKTtcblxuICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICBcImNvbW1pdFwiLFxuICAgICAgICAoZXZlbnQ6IEN1c3RvbUV2ZW50KSA9PiAoaW5mby5pZCA9IGV2ZW50LmRldGFpbC5pZCksXG4gICAgICApO1xuICAgICAgaW5mby51cGxvYWRlci5hZGRFdmVudExpc3RlbmVyKFxuICAgICAgICBcImZhaWxcIixcbiAgICAgICAgKHtcbiAgICAgICAgICBkZXRhaWw6IHsgcmVhc29ucywgZmlsZSB9LFxuICAgICAgICB9OiBDdXN0b21FdmVudDx7XG4gICAgICAgICAgcmVhc29uczogeyBba2V5OiBzdHJpbmddOiBzdHJpbmdbXSB9O1xuICAgICAgICAgIGZpbGU6IEZpbGU7XG4gICAgICAgIH0+KSA9PiB7XG4gICAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeShcbiAgICAgICAgICAgIGZpbGUubmFtZSxcbiAgICAgICAgICAgIE9iamVjdC5lbnRyaWVzKHJlYXNvbnMpXG4gICAgICAgICAgICAgIC5maWx0ZXIoKFtrLCB2XSkgPT4ga1swXSAhPT0gXCJfXCIpXG4gICAgICAgICAgICAgIC5tYXAoKFtrLCB2XSkgPT4gKEFycmF5LmlzQXJyYXkodikgPyB2LmpvaW4oXCI7IFwiKSA6IHYpKVxuICAgICAgICAgICAgICAuam9pbihcIjsgXCIpLFxuICAgICAgICAgICk7XG4gICAgICAgICAgdGhpcy50b2dnbGVBbmltYXRpb24od2lkZ2V0LCBmYWxzZSk7XG5cbiAgICAgICAgICB3aWRnZXRcbiAgICAgICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAgICAgLnJlbW92ZUNsYXNzKFwiYmctcHJpbWFyeSBiZy1zZWNvbmRhcnlcIilcbiAgICAgICAgICAgIC5hZGRDbGFzcyhcImJnLWRhbmdlciBwcm9ncmVzcy1iYXItZGFuZ2VyXCIpO1xuICAgICAgICB9LFxuICAgICAgKTtcbiAgICAgIGluZm8udXBsb2FkZXIuYWRkRXZlbnRMaXN0ZW5lcihcbiAgICAgICAgXCJlcnJvclwiLFxuICAgICAgICAoe1xuICAgICAgICAgIGRldGFpbDogeyBtZXNzYWdlLCBmaWxlIH0sXG4gICAgICAgIH06IEN1c3RvbUV2ZW50PHsgbWVzc2FnZTogc3RyaW5nOyBmaWxlOiBGaWxlIH0+KSA9PiB7XG4gICAgICAgICAgdGhpcy5zYW5kYm94Lm5vdGlmeShmaWxlLm5hbWUsIG1lc3NhZ2UpO1xuICAgICAgICAgIHRoaXMudG9nZ2xlQW5pbWF0aW9uKHdpZGdldCwgZmFsc2UpO1xuICAgICAgICAgIHdpZGdldFxuICAgICAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgICAgICAucmVtb3ZlQ2xhc3MoXCJiZy1wcmltYXJ5IGJnLXNlY29uZGFyeVwiKVxuICAgICAgICAgICAgLmFkZENsYXNzKFwiYmctZGFuZ2VyIHByb2dyZXNzLWJhci1kYW5nZXJcIik7XG4gICAgICAgIH0sXG4gICAgICApO1xuXG4gICAgICBpbmZvLnVwbG9hZGVyLmFkZEV2ZW50TGlzdGVuZXIoXG4gICAgICAgIFwicHJvZ3Jlc3NcIixcbiAgICAgICAgKHsgZGV0YWlsOiB7IGxvYWRlZCwgdG90YWwgfSB9OiBDdXN0b21FdmVudCkgPT5cbiAgICAgICAgICB0aGlzLnNldFdpZGdldENvbXBsZXRpb24od2lkZ2V0LCBsb2FkZWQsIHRvdGFsKSxcbiAgICAgICk7XG4gICAgICBpbmZvLnVwbG9hZGVyLmFkZEV2ZW50TGlzdGVuZXIoXG4gICAgICAgIFwiZmluaXNoXCIsXG4gICAgICAgICh7IGRldGFpbDogeyBmaWxlLCByZXN1bHQgfSB9OiBDdXN0b21FdmVudCkgPT4ge1xuICAgICAgICAgIHRoaXMudG9nZ2xlQW5pbWF0aW9uKHdpZGdldCwgZmFsc2UpO1xuICAgICAgICAgIHdpZGdldFxuICAgICAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgICAgICAucmVtb3ZlQ2xhc3MoXCJiZy1wcmltYXJ5IGJnLXNlY29uZGFyeVwiKVxuICAgICAgICAgICAgLmFkZENsYXNzKFwiYmctc3VjY2VzcyBwcm9ncmVzcy1iYXItc3VjY2Vzc1wiKTtcbiAgICAgICAgICB0aGlzLnNhbmRib3gucHVibGlzaChcbiAgICAgICAgICAgIGNrYW4uQ0tBTkVYVF9GSUxFUy50b3BpY3MucXVldWVJdGVtVXBsb2FkZWQsXG4gICAgICAgICAgICBmaWxlLFxuICAgICAgICAgICAgcmVzdWx0LFxuICAgICAgICAgICk7XG4gICAgICAgIH0sXG4gICAgICApO1xuXG4gICAgICB0aGlzLnNldFdpZGdldE5hbWUod2lkZ2V0LCBpbmZvLmZpbGUubmFtZSk7XG4gICAgICB0aGlzLnNldFdpZGdldENvbXBsZXRpb24od2lkZ2V0LCBpbmZvLnVwbG9hZGVkLCBpbmZvLmZpbGUuc2l6ZSk7XG4gICAgfSxcblxuICAgIHNldFdpZGdldE5hbWUod2lkZ2V0OiBKUXVlcnksIG5hbWU6IHN0cmluZykge1xuICAgICAgd2lkZ2V0LmZpbmQoXCJbZGF0YS1pdGVtLW5hbWVdXCIpLnRleHQobmFtZSk7XG4gICAgfSxcblxuICAgIHNldFdpZGdldENvbXBsZXRpb24od2lkZ2V0OiBKUXVlcnksIHVwbG9hZGVkOiBudW1iZXIsIHRvdGFsOiBudW1iZXIpIHtcbiAgICAgIGNvbnN0IHZhbHVlID0gKHVwbG9hZGVkICogMTAwKSAvIHRvdGFsO1xuICAgICAgY29uc3QgaW5mbyA9IHRoaXMud2lkZ2V0cy5nZXQod2lkZ2V0WzBdKTtcbiAgICAgIGluZm8udXBsb2FkZWQgPSB1cGxvYWRlZDtcblxuICAgICAgY29uc3QgY29tcGxldGlvbiA9IHZhbHVlLnRvRml4ZWQoMCkgKyBcIiVcIjtcbiAgICAgIHdpZGdldFxuICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgLnRleHQoY29tcGxldGlvbilcbiAgICAgICAgLmNzcyhcIndpZHRoXCIsIGNvbXBsZXRpb24pO1xuICAgIH0sXG5cbiAgICB0b2dnbGVBbmltYXRpb24od2lkZ2V0OiBKUXVlcnksIHN0YXRlOiBib29sZWFuKSB7XG4gICAgICB3aWRnZXRcbiAgICAgICAgLmZpbmQoXCJbZGF0YS11cGxvYWQtcHJvZ3Jlc3NdXCIpXG4gICAgICAgIC50b2dnbGVDbGFzcyhcInByb2dyZXNzLWJhci1hbmltYXRlZCBhY3RpdmVcIiwgc3RhdGUpO1xuICAgIH0sXG5cbiAgICBfb25XaWRnZXRSZXN1bWUoZXZlbnQ6IEpRdWVyeS5UcmlnZ2VyZWRFdmVudCkge1xuICAgICAgY29uc3QgaW5mbyA9IHRoaXMud2lkZ2V0cy5nZXQoZXZlbnQuZGVsZWdhdGVUYXJnZXQpO1xuICAgICAgaWYgKGluZm8udXBsb2FkZWQgPj0gaW5mby50b3RhbCkgcmV0dXJuO1xuXG4gICAgICBjb25zdCB3aWRnZXQgPSAkKGV2ZW50LmRlbGVnYXRlVGFyZ2V0KTtcbiAgICAgIHdpZGdldFxuICAgICAgICAuZmluZChcIltkYXRhLXVwbG9hZC1wcm9ncmVzc11cIilcbiAgICAgICAgLnJlbW92ZUNsYXNzKFwiYmctc2Vjb25kYXJ5XCIpXG4gICAgICAgIC5hZGRDbGFzcyhcImJnLXByaW1hcnlcIik7XG5cbiAgICAgIGlmIChpbmZvLmlkKSB7XG4gICAgICAgIGluZm8udXBsb2FkZXIucmVzdW1lKGluZm8uZmlsZSwgaW5mby5pZCk7XG4gICAgICB9IGVsc2Uge1xuICAgICAgICBpbmZvLnVwbG9hZGVyLnVwbG9hZChpbmZvLmZpbGUpO1xuICAgICAgfVxuXG4gICAgICB0aGlzLnRvZ2dsZUFuaW1hdGlvbih3aWRnZXQsIHRydWUpO1xuICAgIH0sXG5cbiAgICBfb25XaWRnZXRQYXVzZShldmVudDogSlF1ZXJ5LlRyaWdnZXJlZEV2ZW50KSB7XG4gICAgICBjb25zdCBpbmZvID0gdGhpcy53aWRnZXRzLmdldChldmVudC5kZWxlZ2F0ZVRhcmdldCk7XG4gICAgICBpZiAoaW5mby51cGxvYWRlZCA+PSBpbmZvLnRvdGFsKSByZXR1cm47XG5cbiAgICAgIGNvbnN0IHdpZGdldCA9ICQoZXZlbnQuZGVsZWdhdGVUYXJnZXQpO1xuICAgICAgd2lkZ2V0XG4gICAgICAgIC5maW5kKFwiW2RhdGEtdXBsb2FkLXByb2dyZXNzXVwiKVxuICAgICAgICAucmVtb3ZlQ2xhc3MoXCJiZy1wcmltYXJ5XCIpXG4gICAgICAgIC5hZGRDbGFzcyhcImJnLXNlY29uZGFyeVwiKTtcblxuICAgICAgaW5mby51cGxvYWRlci5wYXVzZShpbmZvLmZpbGUpO1xuICAgICAgdGhpcy50b2dnbGVBbmltYXRpb24od2lkZ2V0LCBmYWxzZSk7XG4gICAgfSxcbiAgfTtcbn0pO1xuIl19
```

### Comparing `ckanext-files-0.2.2/ckanext/files/assets/scripts/files--shared.js` & `ckanext-files-0.2.3/ckanext/files/assets/scripts/files--shared.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -8,15 +8,15 @@
             restoreFileInQueue: "ckanext:files:queue:file:restore",
             queueItemUploaded: "ckanext:files:queue:file:uploaded",
         };
         CKANEXT_FILES.defaultSettings = {
             storage: "default",
         };
 
-        function upload(file, uploader = new adapters.Standard()) {
+        function upload(file, uploader = makeUploader("Standard")) {
             return uploader.upload(file);
         }
 
         function makeUploader(adapter, ...options) {
             const factory = adapters[adapter];
             if (!factory) {
                 throw new Error(`Uploader ${adapter} is not registered`);
@@ -71,15 +71,15 @@
                 }
                 dispatchProgress(file, loaded, total) {
                     this.dispatchEvent(new CustomEvent("progress", {
                         detail: {
                             file,
                             loaded,
                             total
-                        }
+                        },
                     }));
                 }
                 dispatchFinish(file, result) {
                     this.dispatchEvent(new CustomEvent("finish", {
                         detail: {
                             file,
                             result
@@ -203,19 +203,19 @@
                         start = uploaded;
                     }
                     this.dispatchProgress(file, file.size, file.size);
                     info = await this._completeUpload(info);
                     this.dispatchFinish(file, info);
                 }
                 _initializeUpload(file) {
-                    return new Promise((done, fail) => this.sandbox.client.call("POST", "files_upload_initialize", {
+                    return new Promise((done, fail) => this.sandbox.client.call("POST", "files_upload_initialize", Object.assign({}, this.settings.initializePayload || {}, {
                         storage: this.settings.storage,
                         name: file.name,
                         size: file.size,
-                    }, (data) => {
+                    }), (data) => {
                         done(data.result);
                     }, (resp) => {
                         fail(typeof resp.responseJSON === "string" ?
                             resp.responseText :
                             resp.responseJSON.error);
                     }));
                 }
@@ -255,17 +255,17 @@
                     const form = new FormData();
                     form.append("upload", part);
                     form.append("position", String(position));
                     form.append("id", id);
                     request.send(form);
                 }
                 _completeUpload(info) {
-                    return new Promise((done, fail) => this.sandbox.client.call("POST", "files_upload_complete", {
+                    return new Promise((done, fail) => this.sandbox.client.call("POST", "files_upload_complete", Object.assign({}, this.settings.completePayload || {}, {
                         id: info.id,
-                    }, (data) => {
+                    }), (data) => {
                         done(data.result);
                     }, (resp) => {
                         fail(typeof resp.responseJSON === "string" ?
                             resp.responseText :
                             resp.responseJSON.error);
                     }));
                 }
@@ -273,8 +273,8 @@
             Multipart.defaultSettings = {
                 chunkSize: 1024 * 1024 * 5
             };
             adapters.Multipart = Multipart;
         })(adapters = CKANEXT_FILES.adapters || (CKANEXT_FILES.adapters = {}));
     })(CKANEXT_FILES = ckan.CKANEXT_FILES || (ckan.CKANEXT_FILES = {}));
 })(ckan || (ckan = {}));
-//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXNoYXJlZC5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3RzL2ZpbGVzLS1zaGFyZWQudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IjtBQUFBLElBQVUsSUFBSSxDQXVYYjtBQXZYRCxXQUFVLElBQUk7SUFLWixJQUFpQixhQUFhLENBaVg3QjtJQWpYRCxXQUFpQixhQUFhO1FBTWYsb0JBQU0sR0FBRztZQUNwQixjQUFjLEVBQUUsOEJBQThCO1lBQzlDLGtCQUFrQixFQUFFLGtDQUFrQztZQUN0RCxpQkFBaUIsRUFBRSxtQ0FBbUM7U0FDdkQsQ0FBQztRQUVXLDZCQUFlLEdBQUc7WUFDN0IsT0FBTyxFQUFFLFNBQVM7U0FDbkIsQ0FBQztRQUVGLFNBQVMsTUFBTSxDQUNiLElBQVUsRUFDVixXQUEwQixJQUFJLFFBQVEsQ0FBQyxRQUFRLEVBQUU7WUFFakQsT0FBTyxRQUFRLENBQUMsTUFBTSxDQUFDLElBQUksQ0FBQyxDQUFDO1FBQy9CLENBQUM7UUFFRCxTQUFTLFlBQVksQ0FBQyxPQUFlLEVBQUUsR0FBRyxPQUFZO1lBQ3BELE1BQU0sT0FBTyxHQUE2QyxRQUFTLENBQ2pFLE9BQU8sQ0FDUixDQUFDO1lBQ0YsSUFBSSxDQUFDLE9BQU8sRUFBRSxDQUFDO2dCQUNiLE1BQU0sSUFBSSxLQUFLLENBQUMsWUFBWSxPQUFPLG9CQUFvQixDQUFDLENBQUM7WUFDM0QsQ0FBQztZQUNELE9BQU8sSUFBSSxPQUFPLENBQUMsR0FBRyxPQUFPLENBQUMsQ0FBQztRQUNqQyxDQUFDO1FBRUQsSUFBSSxDQUFDLE9BQU8sQ0FBQyxNQUFNLENBQUMsRUFBRSxLQUFLLEVBQUUsRUFBRSxNQUFNLEVBQUUsWUFBWSxFQUFFLEVBQUUsQ0FBQyxDQUFDO1FBRXpELElBQWlCLFFBQVEsQ0E2VXhCO1FBN1VELFdBQWlCLFFBQVE7WUFVdkIsTUFBYSxJQUFLLFNBQVEsV0FBVztnQkFNbkMsWUFBWSxRQUFRLEdBQUcsRUFBRTtvQkFDdkIsS0FBSyxFQUFFLENB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QUNFLEVBQUUsRUFBRSxJQUFJLENBQUMsRUFBRTtxQkFDWixFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1osSUFBSSxDQUFDLElBQUksQ0FBQyxNQUFNLENBQUMsQ0FBQztvQkFDcEIsQ0FBQyxFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1osSUFBSSxDQUNGLE9BQU8sSUFBSSxDQUFDLFlBQVksS0FBSyxRQUFROzRCQUNuQyxDQUFDLENBQUMsSUFBSSxDQUFDLFlBQVk7NEJBQ25CLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWSxDQUFDLEtBQUssQ0FDNUIsQ0FBQztvQkFDSixDQUFDLENBQ0YsQ0FDRixDQUFDO2dCQUNKLENBQUM7O1lBcE1NLHlCQUFlLEdBQUcsRUFBRSxTQUFTLEVBQUUsSUFBSSxHQUFHLElBQUksR0FBRyxDQUFDLEVBQUUsQ0FBQztZQUQ3QyxrQkFBUyxZQXNNckIsQ0FBQTtRQUNILENBQUMsRUE3VWdCLFFBQVEsR0FBUixzQkFBUSxLQUFSLHNCQUFRLFFBNlV4QjtJQUNILENBQUMsRUFqWGdCLGFBQWEsR0FBYixrQkFBYSxLQUFiLGtCQUFhLFFBaVg3QjtBQUNILENBQUMsRUF2WFMsSUFBSSxLQUFKLElBQUksUUF1WGIiLCJzb3VyY2VzQ29udGVudCI6WyJuYW1lc3BhY2UgY2thbiB7XG4gIGV4cG9ydCB2YXIgc2FuZGJveDogYW55O1xuICBleHBvcnQgdmFyIHB1YnN1YjogYW55O1xuICBleHBvcnQgdmFyIG1vZHVsZTogKG5hbWU6IHN0cmluZywgaW5pdGlhbGl6ZXI6ICgkOiBhbnkpID0+IGFueSkgPT4gYW55O1xuXG4gIGV4cG9ydCBuYW1lc3BhY2UgQ0tBTkVYVF9GSUxFUyB7XG4gICAgdHlwZSBVcGxvYWRlclNldHRpbmdzID0ge1xuICAgICAgc3RvcmFnZTogc3RyaW5nO1xuICAgICAgW2tleTogc3RyaW5nXTogYW55O1xuICAgIH07XG5cbiAgICBleHBvcnQgY29uc3QgdG9waWNzID0ge1xuICAgICAgYWRkRmlsZVRvUXVldWU6IFwiY2thbmV4dDpmaWxlczpxdWV1ZTpmaWxlOmFkZFwiLFxuICAgICAgcmVzdG9yZUZpbGVJblF1ZXVlOiBcImNrYW5leHQ6ZmlsZXM6cXVldWU6ZmlsZTpyZXN0b3JlXCIsXG4gICAgICBxdWV1ZUl0ZW1VcGxvYWRlZDogXCJja2FuZXh0OmZpbGVzOnF1ZXVlOmZpbGU6dXBsb2FkZWRcIixcbiAgICB9O1xuXG4gICAgZXhwb3J0IGNvbnN0IGRlZmF1bHRTZXR0aW5ncyA9IHtcbiAgICAgIHN0b3JhZ2U6IFwiZGVmYXVsdFwiLFxuICAgIH07XG5cbiAgICBmdW5jdGlvbiB1cGxvYWQoXG4gICAgICBmaWxlOiBGaWxlLFxuICAgICAgdXBsb2FkZXI6IGFkYXB0ZXJzLkJhc2UgPSBuZXcgYWRhcHRlcnMuU3RhbmRhcmQoKSxcbiAgICApIHtcbiAgICAgIHJldHVybiB1cGxvYWRlci51cGxvYWQoZmlsZSk7XG4gICAgfVxuXG4gICAgZnVuY3Rpb24gbWFrZVVwbG9hZGVyKGFkYXB0ZXI6IHN0cmluZywgLi4ub3B0aW9uczogYW55KSB7XG4gICAgICBjb25zdCBmYWN0b3J5ID0gKDx7IFtrZXk6IHN0cmluZ106IHR5cGVvZiBhZGFwdGVycy5CYXNlIH0+YWRhcHRlcnMpW1xuICAgICAgICBhZGFwdGVyXG4gICAgICBdO1xuICAgICAgaWYgKCFmYWN0b3J5KSB7XG4gICAgICAgIHRocm93IG5ldyBFcnJvcihgVXBsb2FkZXIgJHthZGFwdGVyfSBpcyBub3QgcmVnaXN0ZXJlZGApO1xuICAgICAgfVxuICAgICAgcmV0dXJuIG5ldyBmYWN0b3J5KC4uLm9wdGlvbnMpO1xuICAgIH1cblxuICAgIGNrYW4uc2FuZGJveC5leHRlbmQoeyBmaWxlczogeyB1cGxvYWQsIG1ha2VVcGxvYWRlciB9IH0pO1xuXG4gICAgZXhwb3J0IG5hbWVzcGFjZSBhZGFwdGVycyB7XG4gICAgICBleHBvcnQgdHlwZSBTdG9yYWdlRGF0YSA9IHtcbiAgICAgICAgdXBsb2FkZWQ6IG51bWJlcjtcbiAgICAgICAgc2l6ZTogbnVtYmVyO1xuICAgICAgfTtcbiAgICAgIGV4cG9ydCB0eXBlIFVwbG9hZEluZm8gPSB7XG4gICAgICAgIGlkOiBzdHJpbmc7XG4gICAgICAgIHN0b3JhZ2VfZGF0YTogU3RvcmFnZURhdGE7XG4gICAgICB9O1xuXG4gICAgICBleHBvcnQgY2xhc3MgQmFzZSBleHRlbmRzIEV2ZW50VGFyZ2V0IHtcbiAgICAgICAgc3RhdGljIGRlZmF1bHRTZXR0aW5nczogT2JqZWN0ID0ge307XG4gICAgICAgIHByb3RlY3RlZCBzZXR0aW5nczogVXBsb2FkZXJTZXR0aW5ncztcbiAgICAgICAgcHJvdGVjdGVkIHNhbmRib3g6IGFueTtcbiAgICAgICAgcHJvdGVjdGVkIGNzcmZUb2tlbjogc3RyaW5nO1xuXG4gICAgICAgIGNvbnN0cnVjdG9yKHNldHRpbmdzID0ge30pIHtcbiAgICAgICAgICBzdXBlcigpO1xuICAgICAgICAgIHRoaXMuc2V0dGluZ3MgPSB7XG4gICAgICAgICAgICAuLi5kZWZhdWx0U2V0dGluZ3MsXG4gICAgICAgICAgICAuLi4odGhpcy5jb25zdHJ1Y3RvciBhcyB0eXBlb2YgQmFzZSkuZGVmYXVsdFNldHRpbmdzLFxuICAgICAgICAgICAgLi4uc2V0dGluZ3MsXG4gICAgICAgICAgfTtcbiAgICAgICAgICB0aGlzLnNhbmRib3ggPSBja2FuLnNhbmRib3goKTtcblxuICAgICAgICAgIGNvbnN0IGNzcmZGaWVsZCA9XG4gICAgICAgICAgICBkb2N1bWVudFxuICAgICAgICAgICAgICAucXVlcnlTZWxlY3RvcihcIm1ldGFbbmFtZT1jc3JmX2ZpZWxkX25hbWVdXCIpXG4gICAgICAgICAgICAgID8uZ2V0QXR0cmlidXRlKFwiY29udGVudFwiKSA/PyBcIl9jc3JmX3Rva2VuXCI7XG4gICAgICAgICAgdGhpcy5jc3JmVG9rZW4gPVxuICAgICAgICAgICAgZG9jdW1lbnRcbiAgICAgICAgICAgICAgLnF1ZXJ5U2VsZWN0b3IoYG1ldGFbbmFtZT0ke2NzcmZGaWVsZH1dYClcbiAgICAgICAgICAgICAgPy5nZXRBdHRyaWJ1dGUoXCJjb250ZW50XCIpIHx8IFwiXCI7XG4gICAgICAgIH1cblxuICAgICAgICB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIkJhc2UudXBsb2FkIGlzIG5vdCBpbXBsZW1lbnRlZFwiKTtcbiAgICAgICAgfVxuXG4gICAgICAgIHJlc3VtZShmaWxlOiBGaWxlLCBpZDogc3RyaW5nKSB7XG4gICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiQmFzZS5yZXN1bWUgaXMgbm90IGltcGxlbWVudGVkXCIpO1xuICAgICAgICB9XG5cbiAgICAgICAgZGlzcGF0Y2hTdGFydChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KG5ldyBDdXN0b21FdmVudChcInN0YXJ0XCIsIHsgZGV0YWlsOiB7IGZpbGUgfSB9KSk7XG4gICAgICAgIH1cbiAgICAgICAgZGlzcGF0Y2hDb21taXQoZmlsZTogRmlsZSwgaWQ6IHN0cmluZykge1xuICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImNvbW1pdFwiLCB7IGRldGFpbDogeyBmaWxlLCBpZCB9IH0pLFxuICAgICAgICAgICk7XG4gICAgICAgIH1cbiAgICAgICAgZGlzcGF0Y2hQcm9ncmVzcyhmaWxlOiBGaWxlLCBsb2FkZWQ6IG51bWJlciwgdG90YWw6IG51bWJlcikge1xuICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcInByb2dyZXNzXCIsIHsgZGV0YWlsOiB7IGZpbGUsIGxvYWRlZCwgdG90YWwgfSB9KSxcbiAgICAgICAgICApO1xuICAgICAgICB9XG4gICAgICAgIGRpc3BhdGNoRmluaXNoKGZpbGU6IEZpbGUsIHJlc3VsdDogT2JqZWN0KSB7XG4gICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiZmluaXNoXCIsIHsgZGV0YWlsOiB7IGZpbGUsIHJlc3VsdCB9IH0pLFxuICAgICAgICAgICk7XG4gICAgICAgIH1cbiAgICAgICAgZGlzcGF0Y2hGYWlsKGZpbGU6IEZpbGUsIHJlYXNvbnM6IHsgW2tleTogc3RyaW5nXTogc3RyaW5nW10gfSkge1xuICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImZhaWxcIiwgeyBkZXRhaWw6IHsgZmlsZSwgcmVhc29ucyB9IH0pLFxuICAgICAgICAgICk7XG4gICAgICAgIH1cbiAgICAgICAgZGlzcGF0Y2hFcnJvcihmaWxlOiBGaWxlLCBtZXNzYWdlOiBzdHJpbmcpIHtcbiAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJlcnJvclwiLCB7IGRldGFpbDogeyBmaWxlLCBtZXNzYWdlIH0gfSksXG4gICAgICAgICAgKTtcbiAgICAgICAgfVxuICAgICAgfVxuICAgICAgZXhwb3J0IGNsYXNzIFN0YW5kYXJkIGV4dGVuZHMgQmFzZSB7XG4gICAgICAgIHVwbG9hZChmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgY29uc3QgcmVxdWVzdCA9IG5ldyBYTUxIdHRwUmVxdWVzdCgpO1xuICAgICAgICAgIGNvbnN0IHByb21pc2UgPSB0aGlzLl9hZGRMaXN0ZW5lcnMocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgdGhpcy5fcHJlcGFyZVJlcXVlc3QocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgdGhpcy5fc2VuZFJlcXVlc3QocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgcmV0dXJuIHByb21pc2U7XG4gICAgICAgIH1cblxuICAgICAgICBfYWRkTGlzdGVuZXJzKFxuICAgICAgICAgIHJlcXVlc3Q6IFhNTEh0dHBSZXF1ZXN0LFxuICAgICAgICAgIGZpbGU6IEZpbGUsXG4gICAgICAgICk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgIHJlcXVlc3QudXBsb2FkLmFkZEV2ZW50TGlzdGVuZXIoXCJsb2Fkc3RhcnRcIiwgKGV2ZW50KSA9PlxuICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFN0YXJ0KGZpbGUpLFxuICAgICAgICAgICk7XG5cbiAgICAgICAgICByZXF1ZXN0LnVwbG9hZC5hZGRFdmVudExpc3RlbmVyKFwicHJvZ3Jlc3NcIiwgKGV2ZW50KSA9PlxuICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIGV2ZW50LmxvYWRlZCwgZXZlbnQudG90YWwpLFxuICAgICAgICAgICk7XG5cbiAgICAgICAgICByZXR1cm4gbmV3IFByb21pc2UoKGRvbmUsIGZhaWwpID0+IHtcbiAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImxvYWRcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgIGNvbnN0IHJlc3VsdCA9IEpTT04ucGFyc2UocmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgICBpZiAocmVzdWx0LnN1Y2Nlc3MpIHtcbiAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoQ29tbWl0KGZpbGUsIHJlc3VsdC5yZXN1bHQuaWQpO1xuICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hGaW5pc2goZmlsZSwgcmVzdWx0LnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgZG9uZShyZXN1bHQucmVzdWx0KTtcbiAgICAgICAgICAgICAgfSBlbHNlIHtcbiAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmFpbChmaWxlLCByZXN1bHQuZXJyb3IpO1xuXG4gICAgICAgICAgICAgICAgZmFpbChyZXN1bHQuZXJyb3IpO1xuICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9KTtcblxuICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwiZXJyb3JcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFcnJvcihmaWxlLCByZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgIGZhaWwocmVxdWVzdC5yZXNwb25zZVRleHQpO1xuICAgICAgICAgICAgfSk7XG4gICAgICAgICAgfSk7XG4gICAgICAgIH1cblxuICAgICAgICBfcHJlcGFyZVJlcXVlc3QocmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsIGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICByZXF1ZXN0Lm9wZW4oXG4gICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQudXJsKFwiL2FwaS9hY3Rpb24vZmlsZXNfZmlsZV9jcmVhdGVcIiksXG4gICAgICAgICAgKTtcblxuICAgICAgICAgIGlmICh0aGlzLmNzcmZUb2tlbikge1xuICAgICAgICAgICAgcmVxdWVzdC5zZXRSZXF1ZXN0SGVhZGVyKFwiWC1DU1JGVG9rZW5cIiwgdGhpcy5jc3JmVG9rZW4pO1xuICAgICAgICAgIH1cbiAgICAgICAgfVxuXG4gICAgICAgIF9zZW5kUmVxdWVzdChyZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCwgZmlsZTogRmlsZSkge1xuICAgICAgICAgIGNvbnN0IGRhdGEgPSBuZXcgRm9ybURhdGEoKTtcbiAgICAgICAgICBkYXRhLmFwcGVuZChcInVwbG9hZFwiLCBmaWxlKTtcblxuICAgICAgICAgIGRhdGEuYXBwZW5kKFwic3RvcmFnZVwiLCB0aGlzLnNldHRpbmdzLnN0b3JhZ2UpO1xuICAgICAgICAgIHJlcXVlc3Quc2VuZChkYXRhKTtcbiAgICAgICAgfVxuICAgICAgfVxuXG4gICAgICBleHBvcnQgY2xhc3MgTXVsdGlwYXJ0IGV4dGVuZHMgQmFzZSB7XG4gICAgICAgIHN0YXRpYyBkZWZhdWx0U2V0dGluZ3MgPSB7IGNodW5rU2l6ZTogMTAyNCAqIDEwMjQgKiA1IH07XG5cbiAgICAgICAgcHJpdmF0ZSBfYWN0aXZlOiBTZXQ8RmlsZT47XG5cbiAgICAgICAgY29uc3RydWN0b3Ioc2V0dGluZ3M6IE9iamVjdCkge1xuICAgICAgICAgIHN1cGVyKHNldHRpbmdzKTtcbiAgICAgICAgICB0aGlzLl9hY3RpdmUgPSBuZXcgU2V0KCk7XG4gICAgICAgIH1cblxuICAgICAgICBhc3luYyB1cGxvYWQoZmlsZTogRmlsZSkge1xuICAgICAgICAgIGlmICh0aGlzLl9hY3RpdmUuaGFzKGZpbGUpKSB7XG4gICAgICAgICAgICBjb25zb2xlLndhcm4oXCJGaWxlIHVwbG9hZCBpbiBwcm9ncmVzc1wiKTtcbiAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICB9XG4gICAgICAgICAgdGhpcy5fYWN0aXZlLmFkZChmaWxlKTtcblxuICAgICAgICAgIGxldCBpbmZvO1xuXG4gICAgICAgICAgdHJ5IHtcbiAgICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl9pbml0aWFsaXplVXBsb2FkKGZpbGUpO1xuICAgICAgICAgIH0gY2F0Y2ggKGVycikge1xuICAgICAgICAgICAgaWYgKHR5cGVvZiBlcnIgPT09IFwic3RyaW5nXCIpIHtcbiAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEVycm9yKGZpbGUsIGVycik7XG4gICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmFpbChmaWxlLCBlcnIgYXMgYW55KTtcbiAgICAgICAgICAgIH1cbiAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICB9XG5cbiAgICAgICAgICB0aGlzLmRpc3BhdGNoQ29tbWl0KGZpbGUsIGluZm8uaWQpO1xuICAgICAgICAgIHRoaXMuZGlzcGF0Y2hTdGFydChmaWxlKTtcblxuICAgICAgICAgIHRoaXMuX2RvVXBsb2FkKGZpbGUsIGluZm8pO1xuICAgICAgICB9XG5cbiAgICAgICAgYXN5bmMgcmVzdW1lKGZpbGU6IEZpbGUsIGlkOiBzdHJpbmcpIHtcbiAgICAgICAgICBpZiAodGhpcy5fYWN0aXZlLmhhcyhmaWxlKSkge1xuICAgICAgICAgICAgY29uc29sZS53YXJuKFwiRmlsZSB1cGxvYWQgaW4gcHJvZ3Jlc3NcIik7XG4gICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgfVxuICAgICAgICAgIHRoaXMuX2FjdGl2ZS5hZGQoZmlsZSk7XG5cbiAgICAgICAgICBsZXQgaW5mbyA9IGF3YWl0IHRoaXMuX3Nob3dVcGxvYWQoaWQpO1xuICAgICAgICAgIHRoaXMuZGlzcGF0Y2hTdGFydChmaWxlKTtcblxuICAgICAgICAgIHRoaXMuX2RvVXBsb2FkKGZpbGUsIGluZm8pO1xuICAgICAgICB9XG5cbiAgICAgICAgcGF1c2UoZmlsZTogRmlsZSkge1xuICAgICAgICAgIHRoaXMuX2FjdGl2ZS5kZWxldGUoZmlsZSk7XG4gICAgICAgIH1cblxuICAgICAgICBhc3luYyBfZG9VcGxvYWQoZmlsZTogRmlsZSwgaW5mbzogVXBsb2FkSW5mbykge1xuICAgICAgICAgIGxldCBzdGFydCA9IGluZm8uc3RvcmFnZV9kYXRhLnVwbG9hZGVkIHx8IDA7XG5cbiAgICAgICAgICB3aGlsZSAoc3RhcnQgPCBmaWxlLnNpemUpIHtcbiAgICAgICAgICAgIGlmICghdGhpcy5fYWN0aXZlLmhhcyhmaWxlKSkge1xuICAgICAgICAgICAgICBjb25zb2xlLmluZm8oXCJGaWxlIHVwbG9hZCBpcyBwYXVzZWRcIik7XG4gICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgaW5mbyA9IGF3YWl0IHRoaXMuX3VwbG9hZENodW5rKFxuICAgICAgICAgICAgICBpbmZvLFxuICAgICAgICAgICAgICBmaWxlLnNsaWNlKHN0YXJ0LCBzdGFydCArIHRoaXMuc2V0dGluZ3MuY2h1bmtTaXplKSxcbiAgICAgICAgICAgICAgc3RhcnQsXG4gICAgICAgICAgICApO1xuXG4gICAgICAgICAgICBjb25zdCB1cGxvYWRlZCA9IGluZm8uc3RvcmFnZV9kYXRhLnVwbG9hZGVkO1xuICAgICAgICAgICAgaWYgKHVwbG9hZGVkIDw9IHN0YXJ0KSB7XG4gICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIlVwbG9hZGVkIHNpemUgaXMgcmVkdWNlZFwiKTtcbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIHVwbG9hZGVkLCBmaWxlLnNpemUpO1xuICAgICAgICAgICAgc3RhcnQgPSB1cGxvYWRlZDtcbiAgICAgICAgICB9XG5cbiAgICAgICAgICB0aGlzLmRpc3BhdGNoUHJvZ3Jlc3MoZmlsZSwgZmlsZS5zaXplLCBmaWxlLnNpemUpO1xuICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl9jb21wbGV0ZVVwbG9hZChpbmZvKTtcbiAgICAgICAgICB0aGlzLmRpc3BhdGNoRmluaXNoKGZpbGUsIGluZm8pO1xuICAgICAgICB9XG5cbiAgICAgICAgX2luaXRpYWxpemVVcGxvYWQoZmlsZTogRmlsZSk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT5cbiAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgXCJQT1NUXCIsXG4gICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX2luaXRpYWxpemVcIixcbiAgICAgICAgICAgICAge1xuICAgICAgICAgICAgICAgIHN0b3JhZ2U6IHRoaXMuc2V0dGluZ3Muc3RvcmFnZSxcbiAgICAgICAgICAgICAgICBuYW1lOiBmaWxlLm5hbWUsXG4gICAgICAgICAgICAgICAgc2l6ZTogZmlsZS5zaXplLFxuICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAoZGF0YTogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgIChyZXNwOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICBmYWlsKFxuICAgICAgICAgICAgICAgICAgdHlwZW9mIHJlc3AucmVzcG9uc2VKU09OID09PSBcInN0cmluZ1wiXG4gICAgICAgICAgICAgICAgICAgID8gcmVzcC5yZXNwb25zZVRleHRcbiAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgKSxcbiAgICAgICAgICApO1xuICAgICAgICB9XG4gICAgICAgIF9zaG93VXBsb2FkKGlkOiBzdHJpbmcpOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICByZXR1cm4gbmV3IFByb21pc2UoKGRvbmUsIGZhaWwpID0+XG4gICAgICAgICAgICB0aGlzLnNhbmRib3guY2xpZW50LmNhbGwoXG4gICAgICAgICAgICAgIFwiR0VUXCIsXG4gICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX3Nob3dcIixcbiAgICAgICAgICAgICAgYD9pZD0ke2lkfWAsXG4gICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICBkb25lKGRhdGEucmVzdWx0KTtcbiAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgKHJlc3A6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgPyByZXNwLnJlc3BvbnNlVGV4dFxuICAgICAgICAgICAgICAgICAgICA6IHJlc3AucmVzcG9uc2VKU09OLmVycm9yLFxuICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApLFxuICAgICAgICAgICk7XG4gICAgICAgIH1cblxuICAgICAgICBfdXBsb2FkQ2h1bmsoXG4gICAgICAgICAgaW5mbzogVXBsb2FkSW5mbyxcbiAgICAgICAgICBwYXJ0OiBCbG9iLFxuICAgICAgICAgIHN0YXJ0OiBudW1iZXIsXG4gICAgICAgICk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgIGlmICghcGFydC5zaXplKSB7XG4gICAgICAgICAgICB0aHJvdyBuZXcgRXJyb3IoXCIwLWxlbmd0aCBjaHVua3MgYXJlIG5vdCBhbGxvd2VkXCIpO1xuICAgICAgICAgIH1cbiAgICAgICAgICBjb25zdCByZXF1ZXN0ID0gbmV3IFhNTEh0dHBSZXF1ZXN0KCk7XG5cbiAgICAgICAgICBjb25zdCByZXN1bHQgPSBuZXcgUHJvbWlzZTxVcGxvYWRJbmZvPigoZG9uZSwgZmFpbCkgPT4ge1xuICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwibG9hZFwiLCAoZXZlbnQpID0+IHtcbiAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gSlNPTi5wYXJzZShyZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgIGlmIChyZXN1bHQuc3VjY2Vzcykge1xuICAgICAgICAgICAgICAgIGRvbmUocmVzdWx0LnJlc3VsdCk7XG4gICAgICAgICAgICAgIH0gZWxzZSB7XG4gICAgICAgICAgICAgICAgZmFpbChyZXN1bHQuZXJyb3IpO1xuICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9KTtcblxuICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwiZXJyb3JcIiwgKGV2ZW50KSA9PlxuICAgICAgICAgICAgICBmYWlsKHJlcXVlc3QucmVzcG9uc2VUZXh0KSxcbiAgICAgICAgICAgICk7XG4gICAgICAgICAgfSk7XG5cbiAgICAgICAgICByZXF1ZXN0Lm9wZW4oXG4gICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQudXJsKFwiL2FwaS9hY3Rpb24vZmlsZXNfdXBsb2FkX3VwZGF0ZVwiKSxcbiAgICAgICAgICApO1xuXG4gICAgICAgICAgaWYgKHRoaXMuY3NyZlRva2VuKSB7XG4gICAgICAgICAgICByZXF1ZXN0LnNldFJlcXVlc3RIZWFkZXIoXCJYLUNTUkZUb2tlblwiLCB0aGlzLmNzcmZUb2tlbik7XG4gICAgICAgICAgfVxuXG4gICAgICAgICAgdGhpcy5fc2VuZFJlcXVlc3QocmVxdWVzdCwgcGFydCwgc3RhcnQsIGluZm8uaWQpO1xuXG4gICAgICAgICAgcmV0dXJuIHJlc3VsdDtcbiAgICAgICAgfVxuXG4gICAgICAgIF9zZW5kUmVxdWVzdChcbiAgICAgICAgICByZXF1ZXN0OiBYTUxIdHRwUmVxdWVzdCxcbiAgICAgICAgICBwYXJ0OiBCbG9iLFxuICAgICAgICAgIHBvc2l0aW9uOiBudW1iZXIsXG4gICAgICAgICAgaWQ6IHN0cmluZyxcbiAgICAgICAgKSB7XG4gICAgICAgICAgY29uc3QgZm9ybSA9IG5ldyBGb3JtRGF0YSgpO1xuICAgICAgICAgIGZvcm0uYXBwZW5kKFwidXBsb2FkXCIsIHBhcnQpO1xuICAgICAgICAgIGZvcm0uYXBwZW5kKFwicG9zaXRpb25cIiwgU3RyaW5nKHBvc2l0aW9uKSk7XG4gICAgICAgICAgZm9ybS5hcHBlbmQoXCJpZFwiLCBpZCk7XG4gICAgICAgICAgcmVxdWVzdC5zZW5kKGZvcm0pO1xuICAgICAgICB9XG5cbiAgICAgICAgX2NvbXBsZXRlVXBsb2FkKGluZm86IFVwbG9hZEluZm8pOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICByZXR1cm4gbmV3IFByb21pc2UoKGRvbmUsIGZhaWwpID0+XG4gICAgICAgICAgICB0aGlzLnNhbmRib3guY2xpZW50LmNhbGwoXG4gICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICBcImZpbGVzX3VwbG9hZF9jb21wbGV0ZVwiLFxuICAgICAgICAgICAgICB7XG4gICAgICAgICAgICAgICAgaWQ6IGluZm8uaWQsXG4gICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICBkb25lKGRhdGEucmVzdWx0KTtcbiAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgKHJlc3A6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgPyByZXNwLnJlc3BvbnNlVGV4dFxuICAgICAgICAgICAgICAgICAgICA6IHJlc3AucmVzcG9uc2VKU09OLmVycm9yLFxuICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICApLFxuICAgICAgICAgICk7XG4gICAgICAgIH1cbiAgICAgIH1cbiAgICB9XG4gIH1cbn1cbiJdfQ==
+//# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiZmlsZXMtLXNoYXJlZC5qcyIsInNvdXJjZVJvb3QiOiIiLCJzb3VyY2VzIjpbIi4uL3RzL2ZpbGVzLS1zaGFyZWQudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6IjtBQUFBLElBQVUsSUFBSSxDQXlZYjtBQXpZRCxXQUFVLElBQUk7SUFLVixJQUFpQixhQUFhLENBbVk3QjtJQW5ZRCxXQUFpQixhQUFhO1FBTWIsb0JBQU0sR0FBRztZQUNsQixjQUFjLEVBQUUsOEJBQThCO1lBQzlDLGtCQUFrQixFQUFFLGtDQUFrQztZQUN0RCxpQkFBaUIsRUFBRSxtQ0FBbUM7U0FDekQsQ0FBQztRQUVXLDZCQUFlLEdBQUc7WUFDM0IsT0FBTyxFQUFFLFNBQVM7U0FDckIsQ0FBQztRQUVGLFNBQVMsTUFBTSxDQUNYLElBQVUsRUFDVixXQUEwQixZQUFZLENBQUMsVUFBVSxDQUFDO1lBRWxELE9BQU8sUUFBUSxDQUFDLE1BQU0sQ0FBQyxJQUFJLENBQUMsQ0FBQztRQUNqQyxDQUFDO1FBRUQsU0FBUyxZQUFZLENBQUMsT0FBZSxFQUFFLEdBQUcsT0FBWTtZQUNsRCxNQUFNLE9BQU8sR0FBNkMsUUFBUyxDQUMvRCxPQUFPLENBQ1YsQ0FBQztZQUNGLElBQUksQ0FBQyxPQUFPLEVBQUUsQ0FBQztnQkFDWCxNQUFNLElBQUksS0FBSyxDQUFDLFlBQVksT0FBTyxvQkFBb0IsQ0FBQyxDQUFDO1lBQzdELENBQUM7WUFDRCxPQUFPLElBQUksT0FBTyxDQUFDLEdBQUcsT0FBTyxDQUFDLENBQUM7UUFDbkMsQ0FBQztRQUVELElBQUksQ0FBQyxPQUFPLENBQUMsTUFBTSxDQUFDLEVBQUUsS0FBSyxFQUFFLEVBQUUsTUFBTSxFQUFFLFlBQVksRUFBRSxFQUFFLENBQUMsQ0FBQztRQUV6RCxJQUFpQixRQUFRLENBK1Z4QjtRQS9WRCxXQUFpQixRQUFRO1lBV3JCLE1BQWEsSUFBSyxTQUFRLFdBQVc7Z0JBTWpDLFlBQVksUUFBUSxHQUFHLEVBQUU7b0JBQ3JCLEtBQUssRUFBRSxDQUFDO29C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LENBQUMsT0FBTyxDQUFDLE1BQU0sQ0FBQyxJQUFJLENBQ3BCLE1BQU0sRUFDTix1QkFBdUIsRUFDdkIsTUFBTSxDQUFDLE1BQU0sQ0FDVCxFQUFFLEVBQ0YsSUFBSSxDQUFDLFFBQVEsQ0FBQyxlQUFlLElBQUksRUFBRSxFQUNuQzt3QkFDSSxFQUFFLEVBQUUsSUFBSSxDQUFDLEVBQUU7cUJBQ2QsQ0FDSixFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1YsSUFBSSxDQUFDLElBQUksQ0FBQyxNQUFNLENBQUMsQ0FBQztvQkFDdEIsQ0FBQyxFQUNELENBQUMsSUFBUyxFQUFFLEVBQUU7d0JBQ1YsSUFBSSxDQUNBLE9BQU8sSUFBSSxDQUFDLFlBQVksS0FBSyxRQUFROzRCQUNqQyxDQUFDLENBQUMsSUFBSSxDQUFDLFlBQVk7NEJBQ25CLENBQUMsQ0FBQyxJQUFJLENBQUMsWUFBWSxDQUFDLEtBQUssQ0FDaEMsQ0FBQztvQkFDTixDQUFDLENBQ0osQ0FDSixDQUFDO2dCQUNOLENBQUM7O1lBOU1NLHlCQUFlLEdBQUcsRUFBRSxTQUFTLEVBQUUsSUFBSSxHQUFHLElBQUksR0FBRyxDQUFDLEVBQUUsQUFBakMsQ0FBa0M7WUFEL0Msa0JBQVMsWUFnTnJCLENBQUE7UUFDTCxDQUFDLEVBL1ZnQixRQUFRLEdBQVIsc0JBQVEsS0FBUixzQkFBUSxRQStWeEI7SUFDTCxDQUFDLEVBbllnQixhQUFhLEdBQWIsa0JBQWEsS0FBYixrQkFBYSxRQW1ZN0I7QUFDTCxDQUFDLEVBellTLElBQUksS0FBSixJQUFJLFFBeVliIiwic291cmNlc0NvbnRlbnQiOlsibmFtZXNwYWNlIGNrYW4ge1xuICAgIGV4cG9ydCB2YXIgc2FuZGJveDogYW55O1xuICAgIGV4cG9ydCB2YXIgcHVic3ViOiBhbnk7XG4gICAgZXhwb3J0IHZhciBtb2R1bGU6IChuYW1lOiBzdHJpbmcsIGluaXRpYWxpemVyOiAoJDogYW55KSA9PiBhbnkpID0+IGFueTtcblxuICAgIGV4cG9ydCBuYW1lc3BhY2UgQ0tBTkVYVF9GSUxFUyB7XG4gICAgICAgIHR5cGUgVXBsb2FkZXJTZXR0aW5ncyA9IHtcbiAgICAgICAgICAgIHN0b3JhZ2U6IHN0cmluZztcbiAgICAgICAgICAgIFtrZXk6IHN0cmluZ106IGFueTtcbiAgICAgICAgfTtcblxuICAgICAgICBleHBvcnQgY29uc3QgdG9waWNzID0ge1xuICAgICAgICAgICAgYWRkRmlsZVRvUXVldWU6IFwiY2thbmV4dDpmaWxlczpxdWV1ZTpmaWxlOmFkZFwiLFxuICAgICAgICAgICAgcmVzdG9yZUZpbGVJblF1ZXVlOiBcImNrYW5leHQ6ZmlsZXM6cXVldWU6ZmlsZTpyZXN0b3JlXCIsXG4gICAgICAgICAgICBxdWV1ZUl0ZW1VcGxvYWRlZDogXCJja2FuZXh0OmZpbGVzOnF1ZXVlOmZpbGU6dXBsb2FkZWRcIixcbiAgICAgICAgfTtcblxuICAgICAgICBleHBvcnQgY29uc3QgZGVmYXVsdFNldHRpbmdzID0ge1xuICAgICAgICAgICAgc3RvcmFnZTogXCJkZWZhdWx0XCIsXG4gICAgICAgIH07XG5cbiAgICAgICAgZnVuY3Rpb24gdXBsb2FkKFxuICAgICAgICAgICAgZmlsZTogRmlsZSxcbiAgICAgICAgICAgIHVwbG9hZGVyOiBhZGFwdGVycy5CYXNlID0gbWFrZVVwbG9hZGVyKFwiU3RhbmRhcmRcIiksXG4gICAgICAgICkge1xuICAgICAgICAgICAgcmV0dXJuIHVwbG9hZGVyLnVwbG9hZChmaWxlKTtcbiAgICAgICAgfVxuXG4gICAgICAgIGZ1bmN0aW9uIG1ha2VVcGxvYWRlcihhZGFwdGVyOiBzdHJpbmcsIC4uLm9wdGlvbnM6IGFueSkge1xuICAgICAgICAgICAgY29uc3QgZmFjdG9yeSA9ICg8eyBba2V5OiBzdHJpbmddOiB0eXBlb2YgYWRhcHRlcnMuQmFzZSB9PmFkYXB0ZXJzKVtcbiAgICAgICAgICAgICAgICBhZGFwdGVyXG4gICAgICAgICAgICBdO1xuICAgICAgICAgICAgaWYgKCFmYWN0b3J5KSB7XG4gICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKGBVcGxvYWRlciAke2FkYXB0ZXJ9IGlzIG5vdCByZWdpc3RlcmVkYCk7XG4gICAgICAgICAgICB9XG4gICAgICAgICAgICByZXR1cm4gbmV3IGZhY3RvcnkoLi4ub3B0aW9ucyk7XG4gICAgICAgIH1cblxuICAgICAgICBja2FuLnNhbmRib3guZXh0ZW5kKHsgZmlsZXM6IHsgdXBsb2FkLCBtYWtlVXBsb2FkZXIgfSB9KTtcblxuICAgICAgICBleHBvcnQgbmFtZXNwYWNlIGFkYXB0ZXJzIHtcbiAgICAgICAgICAgIGV4cG9ydCB0eXBlIFN0b3JhZ2VEYXRhID0ge1xuICAgICAgICAgICAgICAgIHVwbG9hZGVkOiBudW1iZXI7XG4gICAgICAgICAgICAgICAgc2l6ZTogbnVtYmVyO1xuICAgICAgICAgICAgfTtcblxuICAgICAgICAgICAgZXhwb3J0IHR5cGUgVXBsb2FkSW5mbyA9IHtcbiAgICAgICAgICAgICAgICBpZDogc3RyaW5nO1xuICAgICAgICAgICAgICAgIHN0b3JhZ2VfZGF0YTogU3RvcmFnZURhdGE7XG4gICAgICAgICAgICB9O1xuXG4gICAgICAgICAgICBleHBvcnQgY2xhc3MgQmFzZSBleHRlbmRzIEV2ZW50VGFyZ2V0IHtcbiAgICAgICAgICAgICAgICBzdGF0aWMgZGVmYXVsdFNldHRpbmdzOiBPYmplY3QgPSB7fTtcbiAgICAgICAgICAgICAgICBwcm90ZWN0ZWQgc2V0dGluZ3M6IFVwbG9hZGVyU2V0dGluZ3M7XG4gICAgICAgICAgICAgICAgcHJvdGVjdGVkIHNhbmRib3g6IGFueTtcbiAgICAgICAgICAgICAgICBwcm90ZWN0ZWQgY3NyZlRva2VuOiBzdHJpbmc7XG5cbiAgICAgICAgICAgICAgICBjb25zdHJ1Y3RvcihzZXR0aW5ncyA9IHt9KSB7XG4gICAgICAgICAgICAgICAgICAgIHN1cGVyKCk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MgPSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAuLi5kZWZhdWx0U2V0dGluZ3MsXG4gICAgICAgICAgICAgICAgICAgICAgICAuLi4odGhpcy5jb25zdHJ1Y3RvciBhcyB0eXBlb2YgQmFzZSkuZGVmYXVsdFNldHRpbmdzLFxuICAgICAgICAgICAgICAgICAgICAgICAgLi4uc2V0dGluZ3MsXG4gICAgICAgICAgICAgICAgICAgIH07XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveCA9IGNrYW4uc2FuZGJveCgpO1xuXG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IGNzcmZGaWVsZCA9XG4gICAgICAgICAgICAgICAgICAgICAgICBkb2N1bWVudFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIC5xdWVyeVNlbGVjdG9yKFwibWV0YVtuYW1lPWNzcmZfZmllbGRfbmFtZV1cIilcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICA/LmdldEF0dHJpYnV0ZShcImNvbnRlbnRcIikgPz8gXCJfY3NyZl90b2tlblwiO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmNzcmZUb2tlbiA9XG4gICAgICAgICAgICAgICAgICAgICAgICBkb2N1bWVudFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIC5xdWVyeVNlbGVjdG9yKGBtZXRhW25hbWU9JHtjc3JmRmllbGR9XWApXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgPy5nZXRBdHRyaWJ1dGUoXCJjb250ZW50XCIpIHx8IFwiXCI7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgdXBsb2FkKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiQmFzZS51cGxvYWQgaXMgbm90IGltcGxlbWVudGVkXCIpO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIHJlc3VtZShmaWxlOiBGaWxlLCBpZDogc3RyaW5nKSB7XG4gICAgICAgICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIkJhc2UucmVzdW1lIGlzIG5vdCBpbXBsZW1lbnRlZFwiKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBkaXNwYXRjaFN0YXJ0KGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwic3RhcnRcIiwgeyBkZXRhaWw6IHsgZmlsZSB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaENvbW1pdChmaWxlOiBGaWxlLCBpZDogc3RyaW5nKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImNvbW1pdFwiLCB7IGRldGFpbDogeyBmaWxlLCBpZCB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICBkaXNwYXRjaFByb2dyZXNzKGZpbGU6IEZpbGUsIGxvYWRlZDogbnVtYmVyLCB0b3RhbDogbnVtYmVyKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcInByb2dyZXNzXCIsIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBkZXRhaWw6IHsgZmlsZSwgbG9hZGVkLCB0b3RhbCB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgfSksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgIGRpc3BhdGNoRmluaXNoKGZpbGU6IEZpbGUsIHJlc3VsdDogT2JqZWN0KSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hFdmVudChcbiAgICAgICAgICAgICAgICAgICAgICAgIG5ldyBDdXN0b21FdmVudChcImZpbmlzaFwiLCB7IGRldGFpbDogeyBmaWxlLCByZXN1bHQgfSB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hGYWlsKGZpbGU6IEZpbGUsIHJlYXNvbnM6IHsgW2tleTogc3RyaW5nXTogc3RyaW5nW10gfSkge1xuICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRXZlbnQoXG4gICAgICAgICAgICAgICAgICAgICAgICBuZXcgQ3VzdG9tRXZlbnQoXCJmYWlsXCIsIHsgZGV0YWlsOiB7IGZpbGUsIHJlYXNvbnMgfSB9KSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgZGlzcGF0Y2hFcnJvcihmaWxlOiBGaWxlLCBtZXNzYWdlOiBzdHJpbmcpIHtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEV2ZW50KFxuICAgICAgICAgICAgICAgICAgICAgICAgbmV3IEN1c3RvbUV2ZW50KFwiZXJyb3JcIiwgeyBkZXRhaWw6IHsgZmlsZSwgbWVzc2FnZSB9IH0pLFxuICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgZXhwb3J0IGNsYXNzIFN0YW5kYXJkIGV4dGVuZHMgQmFzZSB7XG4gICAgICAgICAgICAgICAgdXBsb2FkKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVxdWVzdCA9IG5ldyBYTUxIdHRwUmVxdWVzdCgpO1xuICAgICAgICAgICAgICAgICAgICBjb25zdCBwcm9taXNlID0gdGhpcy5fYWRkTGlzdGVuZXJzKHJlcXVlc3QsIGZpbGUpO1xuICAgICAgICAgICAgICAgICAgICB0aGlzLl9wcmVwYXJlUmVxdWVzdChyZXF1ZXN0LCBmaWxlKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5fc2VuZFJlcXVlc3QocmVxdWVzdCwgZmlsZSk7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBwcm9taXNlO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9hZGRMaXN0ZW5lcnMoXG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Q6IFhNTEh0dHBSZXF1ZXN0LFxuICAgICAgICAgICAgICAgICAgICBmaWxlOiBGaWxlLFxuICAgICAgICAgICAgICAgICk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnVwbG9hZC5hZGRFdmVudExpc3RlbmVyKFwibG9hZHN0YXJ0XCIsIChldmVudCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hTdGFydChmaWxlKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnVwbG9hZC5hZGRFdmVudExpc3RlbmVyKFwicHJvZ3Jlc3NcIiwgKGV2ZW50KSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIGV2ZW50LmxvYWRlZCwgZXZlbnQudG90YWwpLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwibG9hZFwiLCAoZXZlbnQpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBjb25zdCByZXN1bHQgPSBKU09OLnBhcnNlKHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBpZiAocmVzdWx0LnN1Y2Nlc3MpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaENvbW1pdChmaWxlLCByZXN1bHQucmVzdWx0LmlkKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZpbmlzaChmaWxlLCByZXN1bHQucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShyZXN1bHQucmVzdWx0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0aGlzLmRpc3BhdGNoRmFpbChmaWxlLCByZXN1bHQuZXJyb3IpO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwocmVzdWx0LmVycm9yKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgICAgICB9KTtcblxuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5hZGRFdmVudExpc3RlbmVyKFwiZXJyb3JcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEVycm9yKGZpbGUsIHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKHJlcXVlc3QucmVzcG9uc2VUZXh0KTtcbiAgICAgICAgICAgICAgICAgICAgICAgIH0pO1xuICAgICAgICAgICAgICAgICAgICB9KTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfcHJlcGFyZVJlcXVlc3QocmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsIGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5vcGVuKFxuICAgICAgICAgICAgICAgICAgICAgICAgXCJQT1NUXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICB0aGlzLnNhbmRib3guY2xpZW50LnVybChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIi9hcGkvYWN0aW9uL2ZpbGVzX2ZpbGVfY3JlYXRlXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICApO1xuXG4gICAgICAgICAgICAgICAgICAgIGlmICh0aGlzLmNzcmZUb2tlbikge1xuICAgICAgICAgICAgICAgICAgICAgICAgcmVxdWVzdC5zZXRSZXF1ZXN0SGVhZGVyKFwiWC1DU1JGVG9rZW5cIiwgdGhpcy5jc3JmVG9rZW4pO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3NlbmRSZXF1ZXN0KHJlcXVlc3Q6IFhNTEh0dHBSZXF1ZXN0LCBmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IGRhdGEgPSBuZXcgRm9ybURhdGEoKTtcbiAgICAgICAgICAgICAgICAgICAgZGF0YS5hcHBlbmQoXCJ1cGxvYWRcIiwgZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgZGF0YS5hcHBlbmQoXCJzdG9yYWdlXCIsIHRoaXMuc2V0dGluZ3Muc3RvcmFnZSk7XG4gICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2VuZChkYXRhKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9XG5cbiAgICAgICAgICAgIGV4cG9ydCBjbGFzcyBNdWx0aXBhcnQgZXh0ZW5kcyBCYXNlIHtcbiAgICAgICAgICAgICAgICBzdGF0aWMgZGVmYXVsdFNldHRpbmdzID0geyBjaHVua1NpemU6IDEwMjQgKiAxMDI0ICogNSB9O1xuXG4gICAgICAgICAgICAgICAgcHJpdmF0ZSBfYWN0aXZlID0gbmV3IFNldDxGaWxlPigpO1xuXG4gICAgICAgICAgICAgICAgY29uc3RydWN0b3Ioc2V0dGluZ3M6IE9iamVjdCkge1xuICAgICAgICAgICAgICAgICAgICBzdXBlcihzZXR0aW5ncyk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgYXN5bmMgdXBsb2FkKGZpbGU6IEZpbGUpIHtcbiAgICAgICAgICAgICAgICAgICAgaWYgKHRoaXMuX2FjdGl2ZS5oYXMoZmlsZSkpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGNvbnNvbGUud2FybihcIkZpbGUgdXBsb2FkIGluIHByb2dyZXNzXCIpO1xuICAgICAgICAgICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2FjdGl2ZS5hZGQoZmlsZSk7XG5cbiAgICAgICAgICAgICAgICAgICAgbGV0IGluZm87XG5cbiAgICAgICAgICAgICAgICAgICAgdHJ5IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl9pbml0aWFsaXplVXBsb2FkKGZpbGUpO1xuICAgICAgICAgICAgICAgICAgICB9IGNhdGNoIChlcnIpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGlmICh0eXBlb2YgZXJyID09PSBcInN0cmluZ1wiKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEVycm9yKGZpbGUsIGVycik7XG4gICAgICAgICAgICAgICAgICAgICAgICB9IGVsc2Uge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hGYWlsKGZpbGUsIGVyciBhcyBhbnkpO1xuICAgICAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICAgICAgcmV0dXJuO1xuICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaENvbW1pdChmaWxlLCBpbmZvLmlkKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFN0YXJ0KGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2RvVXBsb2FkKGZpbGUsIGluZm8pO1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIGFzeW5jIHJlc3VtZShmaWxlOiBGaWxlLCBpZDogc3RyaW5nKSB7XG4gICAgICAgICAgICAgICAgICAgIGlmICh0aGlzLl9hY3RpdmUuaGFzKGZpbGUpKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICBjb25zb2xlLndhcm4oXCJGaWxlIHVwbG9hZCBpbiBwcm9ncmVzc1wiKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJldHVybjtcbiAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICB0aGlzLl9hY3RpdmUuYWRkKGZpbGUpO1xuXG4gICAgICAgICAgICAgICAgICAgIGxldCBpbmZvID0gYXdhaXQgdGhpcy5fc2hvd1VwbG9hZChpZCk7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hTdGFydChmaWxlKTtcblxuICAgICAgICAgICAgICAgICAgICB0aGlzLl9kb1VwbG9hZChmaWxlLCBpbmZvKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBwYXVzZShmaWxlOiBGaWxlKSB7XG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX2FjdGl2ZS5kZWxldGUoZmlsZSk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgYXN5bmMgX2RvVXBsb2FkKGZpbGU6IEZpbGUsIGluZm86IFVwbG9hZEluZm8pIHtcbiAgICAgICAgICAgICAgICAgICAgbGV0IHN0YXJ0ID0gaW5mby5zdG9yYWdlX2RhdGEudXBsb2FkZWQgfHwgMDtcblxuICAgICAgICAgICAgICAgICAgICB3aGlsZSAoc3RhcnQgPCBmaWxlLnNpemUpIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIGlmICghdGhpcy5fYWN0aXZlLmhhcyhmaWxlKSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGNvbnNvbGUuaW5mbyhcIkZpbGUgdXBsb2FkIGlzIHBhdXNlZFwiKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICByZXR1cm47XG4gICAgICAgICAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl91cGxvYWRDaHVuayhcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBpbmZvLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZpbGUuc2xpY2Uoc3RhcnQsIHN0YXJ0ICsgdGhpcy5zZXR0aW5ncy5jaHVua1NpemUpLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHN0YXJ0LFxuICAgICAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICAgICAgY29uc3QgdXBsb2FkZWQgPSBpbmZvLnN0b3JhZ2VfZGF0YS51cGxvYWRlZDtcbiAgICAgICAgICAgICAgICAgICAgICAgIGlmICh1cGxvYWRlZCA8PSBzdGFydCkge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRocm93IG5ldyBFcnJvcihcIlVwbG9hZGVkIHNpemUgaXMgcmVkdWNlZFwiKTtcbiAgICAgICAgICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaFByb2dyZXNzKGZpbGUsIHVwbG9hZGVkLCBmaWxlLnNpemUpO1xuICAgICAgICAgICAgICAgICAgICAgICAgc3RhcnQgPSB1cGxvYWRlZDtcbiAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuZGlzcGF0Y2hQcm9ncmVzcyhmaWxlLCBmaWxlLnNpemUsIGZpbGUuc2l6ZSk7XG4gICAgICAgICAgICAgICAgICAgIGluZm8gPSBhd2FpdCB0aGlzLl9jb21wbGV0ZVVwbG9hZChpbmZvKTtcbiAgICAgICAgICAgICAgICAgICAgdGhpcy5kaXNwYXRjaEZpbmlzaChmaWxlLCBpbmZvKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfaW5pdGlhbGl6ZVVwbG9hZChmaWxlOiBGaWxlKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcImZpbGVzX3VwbG9hZF9pbml0aWFsaXplXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgT2JqZWN0LmFzc2lnbihcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MuaW5pdGlhbGl6ZVBheWxvYWQgfHwge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHN0b3JhZ2U6IHRoaXMuc2V0dGluZ3Muc3RvcmFnZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIG5hbWU6IGZpbGUubmFtZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHNpemU6IGZpbGUuc2l6ZSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG5cbiAgICAgICAgICAgICAgICBfc2hvd1VwbG9hZChpZDogc3RyaW5nKTogUHJvbWlzZTxVcGxvYWRJbmZvPiB7XG4gICAgICAgICAgICAgICAgICAgIHJldHVybiBuZXcgUHJvbWlzZSgoZG9uZSwgZmFpbCkgPT5cbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQuY2FsbChcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBcIkdFVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX3Nob3dcIixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICBgP2lkPSR7aWR9YCxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAoZGF0YTogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRvbmUoZGF0YS5yZXN1bHQpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH0sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgKHJlc3A6IGFueSkgPT4ge1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBmYWlsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgdHlwZW9mIHJlc3AucmVzcG9uc2VKU09OID09PSBcInN0cmluZ1wiXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgPyByZXNwLnJlc3BvbnNlVGV4dFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIDogcmVzcC5yZXNwb25zZUpTT04uZXJyb3IsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICksXG4gICAgICAgICAgICAgICAgICAgICk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX3VwbG9hZENodW5rKFxuICAgICAgICAgICAgICAgICAgICBpbmZvOiBVcGxvYWRJbmZvLFxuICAgICAgICAgICAgICAgICAgICBwYXJ0OiBCbG9iLFxuICAgICAgICAgICAgICAgICAgICBzdGFydDogbnVtYmVyLFxuICAgICAgICAgICAgICAgICk6IFByb21pc2U8VXBsb2FkSW5mbz4ge1xuICAgICAgICAgICAgICAgICAgICBpZiAoIXBhcnQuc2l6ZSkge1xuICAgICAgICAgICAgICAgICAgICAgICAgdGhyb3cgbmV3IEVycm9yKFwiMC1sZW5ndGggY2h1bmtzIGFyZSBub3QgYWxsb3dlZFwiKTtcbiAgICAgICAgICAgICAgICAgICAgfVxuICAgICAgICAgICAgICAgICAgICBjb25zdCByZXF1ZXN0ID0gbmV3IFhNTEh0dHBSZXF1ZXN0KCk7XG5cbiAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gbmV3IFByb21pc2U8VXBsb2FkSW5mbz4oKGRvbmUsIGZhaWwpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3QuYWRkRXZlbnRMaXN0ZW5lcihcImxvYWRcIiwgKGV2ZW50KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgY29uc3QgcmVzdWx0ID0gSlNPTi5wYXJzZShyZXF1ZXN0LnJlc3BvbnNlVGV4dCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgaWYgKHJlc3VsdC5zdWNjZXNzKSB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGRvbmUocmVzdWx0LnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSBlbHNlIHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXN1bHQuZXJyb3IpO1xuICAgICAgICAgICAgICAgICAgICAgICAgICAgIH1cbiAgICAgICAgICAgICAgICAgICAgICAgIH0pO1xuXG4gICAgICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LmFkZEV2ZW50TGlzdGVuZXIoXCJlcnJvclwiLCAoZXZlbnQpID0+XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgZmFpbChyZXF1ZXN0LnJlc3BvbnNlVGV4dCksXG4gICAgICAgICAgICAgICAgICAgICAgICApO1xuICAgICAgICAgICAgICAgICAgICB9KTtcblxuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0Lm9wZW4oXG4gICAgICAgICAgICAgICAgICAgICAgICBcIlBPU1RcIixcbiAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2FuZGJveC5jbGllbnQudXJsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiL2FwaS9hY3Rpb24vZmlsZXNfdXBsb2FkX3VwZGF0ZVwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcblxuICAgICAgICAgICAgICAgICAgICBpZiAodGhpcy5jc3JmVG9rZW4pIHtcbiAgICAgICAgICAgICAgICAgICAgICAgIHJlcXVlc3Quc2V0UmVxdWVzdEhlYWRlcihcIlgtQ1NSRlRva2VuXCIsIHRoaXMuY3NyZlRva2VuKTtcbiAgICAgICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgICAgIHRoaXMuX3NlbmRSZXF1ZXN0KHJlcXVlc3QsIHBhcnQsIHN0YXJ0LCBpbmZvLmlkKTtcblxuICAgICAgICAgICAgICAgICAgICByZXR1cm4gcmVzdWx0O1xuICAgICAgICAgICAgICAgIH1cblxuICAgICAgICAgICAgICAgIF9zZW5kUmVxdWVzdChcbiAgICAgICAgICAgICAgICAgICAgcmVxdWVzdDogWE1MSHR0cFJlcXVlc3QsXG4gICAgICAgICAgICAgICAgICAgIHBhcnQ6IEJsb2IsXG4gICAgICAgICAgICAgICAgICAgIHBvc2l0aW9uOiBudW1iZXIsXG4gICAgICAgICAgICAgICAgICAgIGlkOiBzdHJpbmcsXG4gICAgICAgICAgICAgICAgKSB7XG4gICAgICAgICAgICAgICAgICAgIGNvbnN0IGZvcm0gPSBuZXcgRm9ybURhdGEoKTtcbiAgICAgICAgICAgICAgICAgICAgZm9ybS5hcHBlbmQoXCJ1cGxvYWRcIiwgcGFydCk7XG4gICAgICAgICAgICAgICAgICAgIGZvcm0uYXBwZW5kKFwicG9zaXRpb25cIiwgU3RyaW5nKHBvc2l0aW9uKSk7XG4gICAgICAgICAgICAgICAgICAgIGZvcm0uYXBwZW5kKFwiaWRcIiwgaWQpO1xuICAgICAgICAgICAgICAgICAgICByZXF1ZXN0LnNlbmQoZm9ybSk7XG4gICAgICAgICAgICAgICAgfVxuXG4gICAgICAgICAgICAgICAgX2NvbXBsZXRlVXBsb2FkKGluZm86IFVwbG9hZEluZm8pOiBQcm9taXNlPFVwbG9hZEluZm8+IHtcbiAgICAgICAgICAgICAgICAgICAgcmV0dXJuIG5ldyBQcm9taXNlKChkb25lLCBmYWlsKSA9PlxuICAgICAgICAgICAgICAgICAgICAgICAgdGhpcy5zYW5kYm94LmNsaWVudC5jYWxsKFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiUE9TVFwiLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIFwiZmlsZXNfdXBsb2FkX2NvbXBsZXRlXCIsXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgT2JqZWN0LmFzc2lnbihcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAge30sXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIHRoaXMuc2V0dGluZ3MuY29tcGxldGVQYXlsb2FkIHx8IHt9LFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICBpZDogaW5mby5pZCxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICApLFxuICAgICAgICAgICAgICAgICAgICAgICAgICAgIChkYXRhOiBhbnkpID0+IHtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgZG9uZShkYXRhLnJlc3VsdCk7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgfSxcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAocmVzcDogYW55KSA9PiB7XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgIGZhaWwoXG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICB0eXBlb2YgcmVzcC5yZXNwb25zZUpTT04gPT09IFwic3RyaW5nXCJcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICA/IHJlc3AucmVzcG9uc2VUZXh0XG4gICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgOiByZXNwLnJlc3BvbnNlSlNPTi5lcnJvcixcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICAgICAgICAgICAgICB9LFxuICAgICAgICAgICAgICAgICAgICAgICAgKSxcbiAgICAgICAgICAgICAgICAgICAgKTtcbiAgICAgICAgICAgICAgICB9XG4gICAgICAgICAgICB9XG4gICAgICAgIH1cbiAgICB9XG59XG4iXX0=
```

### Comparing `ckanext-files-0.2.2/ckanext/files/base.py` & `ckanext-files-0.2.3/ckanext/files/base.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/cli.py` & `ckanext-files-0.2.3/ckanext/files/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/command.py` & `ckanext-files-0.2.3/ckanext/files/command.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,31 +9,26 @@
 from ckan.lib.cli import CkanCommand
 
 from ckanext.files.model.base import metadata
 
 log = logging.getLogger(__name__)
 
 
-def drop_tables():
-    """Drop tables defined in model."""
-    metadata.drop_all(model.meta.engine)
-
-
 def create_tables():
     """Create tables defined in model."""
     metadata.create_all(model.meta.engine)
 
 
 class FilesCommand(CkanCommand):
     """
     ckanext-files management commands.
 
     Usage::
         paster --plugin=ckanext-files files  -c ckan.ini initdb
-        paster --plugin=ckanext-files files  -c ckan.ini dropdb
+        paster --plugin=ckanext-files files  -c ckan.ini createdb
     """
 
     summary = __doc__.split("\n")[0]
     usage = __doc__
 
     parser = paste.script.command.Command.standard_parser(verbose=True)
     parser.add_option(
@@ -49,28 +44,19 @@
         self._load_config()
 
         if not len(self.args):
             print(self.usage)  # noqa
 
         elif self.args[0] == "initdb":
             self._init()
-        elif self.args[0] == "dropdb":
-            self._drop()
         elif self.args[0] == "createdb":
             self._create()
 
     def _init(self):
-        self._drop()
         self._create()
         log.info("DB tables are reinitialized")
 
-    def _drop(self):
-        model.Session.rollback()
-
-        drop_tables()
-        log.info("DB tables are removed")
-
     def _create(self):
         model.Session.rollback()
 
         create_tables()
         log.info("DB tables are setup")
```

### Comparing `ckanext-files-0.2.2/ckanext/files/config.py` & `ckanext-files-0.2.3/ckanext/files/config.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/exceptions.py` & `ckanext-files-0.2.3/ckanext/files/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -84,14 +84,29 @@
         # type: (type, str) -> None
         return super(MissingStorageConfigurationError, self).__init__(
             adapter,
             "{} option is required".format(option),
         )
 
 
+class MissingFileError(StorageError):
+    """File does not exist."""
+
+    def __init__(self, storage, filename):
+        # type: (str, str) -> None
+        self.storage = storage
+        self.filename = filename
+
+    def __str__(self):
+        return "File {} does not exist inside {} storage".format(
+            self.filename,
+            self.storage,
+        )
+
+
 class LargeUploadError(UploadError):
     """Storage cannot be initialized due to missing option."""
 
     def __init__(self, actual_size, max_size):
         # type: (int, int) -> None
         self.actual_size = actual_size
         self.max_size = max_size
@@ -120,20 +135,27 @@
         # type: (str) -> None
         self.strategy = strategy
 
     def __str__(self):
         return "Unknown name strategy {}".format(self.strategy)
 
 
-class MissingFileError(StorageError):
-    """File does not exist."""
+class UploadExtrasError(UploadError):
+    """Wrong extras passed during upload."""
 
-    def __init__(self, storage, filename):
-        # type: (str, str) -> None
-        self.storage = storage
-        self.filename = filename
+    def __init__(self, extras):
+        # type: (Any) -> None
+        self.extras = extras
 
     def __str__(self):
-        return "File {} does not exist inside {} storage".format(
-            self.filename,
-            self.storage,
-        )
+        return "Wrong extras: {}".format(self.extras)
+
+
+class MissingExtrasError(UploadExtrasError):
+    """Wrong extras passed during upload."""
+
+    def __init__(self, key):
+        # type: (Any) -> None
+        self.key = key
+
+    def __str__(self):
+        return "Key {} is missing from upload extras".format(self.key)
```

### Comparing `ckanext-files-0.2.2/ckanext/files/helpers.py` & `ckanext-files-0.2.3/ckanext/files/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/interfaces.py` & `ckanext-files-0.2.3/ckanext/files/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/logic/action.py` & `ckanext-files-0.2.3/ckanext/files/logic/action.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,45 +18,67 @@
 _actions, action = make_collector()
 
 
 def get_actions():
     return dict(_actions)
 
 
+def _flat_mask(data):
+    # type: (dict[str, types.Any]) -> dict[tuple[types.Any], types.Any]
+    result = {}  # type: dict[tuple[types.Any], types.Any]
+
+    for k, v in data.items():
+        if isinstance(v, dict):
+            result.update({(k,) + sk: sv for sk, sv in _flat_mask(v).items()})
+        else:
+            result[(k,)] = v
+
+    return result
+
+
 @action
 @tk.side_effect_free
 @validate(schema.file_search_by_user)
 def files_file_search_by_user(context, data_dict):
     # type: (types.Any, dict[str, types.Any]) -> dict[str, types.Any]
     tk.check_access("files_file_search_by_user", context, data_dict)
     sess = context["session"]
 
     user = model.User.get(data_dict.get("user", context["user"]))
     if not user:
         raise tk.ObjectNotFound("user")
 
     q = sess.query(File).join(
         Owner,
-        sa.and_(File.id == Owner.item_id, Owner.item_type == "file"),  # type: ignore
+        sa.and_(File.id == Owner.item_id, Owner.item_type == "file"),
     )
 
     if "storage" in data_dict:
         q = q.filter(File.storage == data_dict["storage"])
 
     q = q.filter(sa.and_(Owner.owner_type == "user", Owner.owner_id == user.id))
 
+    inspector = sa.inspect(File)  # type: types.Any
+    columns = inspector.columns
+
+    for mask in ["storage_data", "plugin_data"]:
+        if mask in data_dict:
+            for k, v in _flat_mask(data_dict[mask]).items():
+                field = columns[mask]
+                for segment in k:
+                    field = field[segment]
+
+                q = q.filter(field.astext == v)
+
     total = q.count()
 
     parts = data_dict["sort"].split(".")
     sort = parts[0]
     sort_path = parts[1:]
 
-    inspector = sa.inspect(File)  # type: types.Any
-    columns = inspector.columns
-
     if sort not in columns:
         raise tk.ValidationError({"sort": ["Unknown sort column"]})
 
     column = columns[sort]
 
     if sort_path and sort == "storage_data":
         for part in sort_path:
@@ -211,14 +233,15 @@
     return fileobj.dictize(context)
 
 
 @action
 @validate(schema.upload_initialize)
 def files_upload_initialize(context, data_dict):
     # type: (types.Any, dict[str, types.Any]) -> dict[str, types.Any]
+
     tk.check_access("files_upload_initialize", context, data_dict)
     _ensure_name(data_dict)
     extras = data_dict.get("__extras", {})
 
     try:
         storage = shared.get_storage(data_dict["storage"])
     except exceptions.UnknownStorageError as err:
```

### Comparing `ckanext-files-0.2.2/ckanext/files/logic/auth.py` & `ckanext-files-0.2.3/ckanext/files/logic/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         return user
 
     return model.User.get(context["user"])
 
 
 def _is_owner(user_id, file_id):
     # type: (str, str) -> bool
-    stmt = Owner.owner_of(file_id, "file").where(
+    stmt = Owner.owners_of(file_id, "file").where(
         sa.and_(
             Owner.owner_type == "user",
             Owner.owner_ie == user_id,
         ),
     )
     return model.Session.query(stmt.exists()).scalar()
```

### Comparing `ckanext-files-0.2.2/ckanext/files/logic/schema.py` & `ckanext-files-0.2.3/ckanext/files/logic/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
     return {
         "start": [default(0), int_validator],
         "rows": [default(10), int_validator],
         "sort": [default("name"), unicode_safe],
         "reverse": [boolean_validator],
         "storage": [ignore_empty, unicode_safe],
+        "storage_data": [ignore_empty],
+        "plugin_data": [ignore_empty],
     }
 
 
 @validator_args
 def file_search_by_user(ignore_missing, unicode_safe, default, ignore_not_sysadmin):
     # type: (types.Any, types.Any, types.Any, types.Any) -> types.Any
     schema = _base_file_search()
```

### Comparing `ckanext-files-0.2.2/ckanext/files/logic/validators.py` & `ckanext-files-0.2.3/ckanext/files/logic/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,27 +24,29 @@
 
 @validator
 def files_into_upload(value):
     # type: (Any) -> types.Upload
     """Convert value into werkzeug.FileStorage object"""
     if isinstance(value, FileStorage):
         if not value.content_length:
-            value.headers["content-length"] = str(value.stream.seek(0, 2))
+            value.stream.seek(0, 2)
+            value.headers["content-length"] = str(value.stream.tell())
             value.stream.seek(0)
         return value
 
     if isinstance(value, cgi.FieldStorage):
         if not value.filename or not value.file:
             raise ValueError(value)
 
         mime, _encoding = mimetypes.guess_type(value.filename)
         if not mime:
             mime = magic.from_buffer(value.file.read(1024), True)
             value.file.seek(0)
-        size = value.file.seek(0, 2)
+        value.file.seek(0, 2)
+        size = value.file.tell()
         value.file.seek(0)
 
         return FileStorage(
             value.file,
             value.filename,
             content_type=mime,
             content_length=size,
@@ -52,15 +54,16 @@
 
     if isinstance(value, six.text_type):
         value = value.encode()
 
     if isinstance(value, (bytes, bytearray)):
         stream = BytesIO(value)
         mime = magic.from_buffer(stream.read(1024), True)
-        size = stream.seek(0, 2)
+        stream.seek(0, 2)
+        size = stream.tell()
         stream.seek(0)
 
         return FileStorage(stream, content_type=mime, content_length=size)
 
     msg = "Unsupported source type: {}".format(type(value))
     raise tk.Invalid(msg)
```

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/alembic.ini` & `ckanext-files-0.2.3/ckanext/files/migration/files/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/env.py` & `ckanext-files-0.2.3/ckanext/files/migration/files/env.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py` & `ckanext-files-0.2.3/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py` & `ckanext-files-0.2.3/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py` & `ckanext-files-0.2.3/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py` & `ckanext-files-0.2.3/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     op.add_column("files_file", sa.Column("plugin_data", JSONB, server_default="{}"))
     op.add_column("files_file", sa.Column("mtime", sa.DateTime()))
     op.add_column("files_file", sa.Column("atime", sa.DateTime()))
     op.alter_column("files_file", "uploaded_at", new_column_name="ctime")
     op.alter_column("files_file", "kind", new_column_name="storage")
 
     columns = [table.c.id, table.c.last_access, table.c.path, table.c.extras]
-    stmt = sa.select(*columns) if tk.check_ckan_version("2.10") else sa.select(columns)
+    stmt = sa.select(*columns) if tk.check_ckan_version("2.9") else sa.select(columns)
 
     for id, last_access, path, extras in bind.execute(stmt):
         op.execute(
             sa.update(table)
             .values(
                 atime=last_access,
                 extras=dict(extras or {}, filename=os.path.basename(path)),
@@ -89,15 +89,17 @@
     op.alter_column(
         "files_file",
         "storage_data",
         server_default=None,
         new_column_name="extras",
     )
 
-    stmt = sa.select(table.c.id, table.c.atime, table.c.extras)
+    columns = [table.c.id, table.c.atime, table.c.extras]
+    stmt = sa.select(*columns) if tk.check_ckan_version("2.9") else sa.select(columns)
+
     for id, atime, extras in bind.execute(stmt):
         extras = dict(extras)
         path = extras.pop("filename", None)
         if not path:
             continue
         op.execute(
             sa.update(table)
```

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py` & `ckanext-files-0.2.3/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py` & `ckanext-files-0.2.3/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/model/file.py` & `ckanext-files-0.2.3/ckanext/files/model/file.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from datetime import datetime  # isort: skip # noqa: F401
 
 
 from ckanext.files import types  # isort: skip # noqa: F401
 
 if six.PY3:
-    from typing import Any  # isort: skip # noqa: F401
+    from typing import Any, Literal  # isort: skip # noqa: F401
 
 
 class File(Base):  # type: ignore
     __tablename__ = "files_file"
     id = Column(UnicodeText, primary_key=True, default=make_uuid)
     name = Column(UnicodeText, nullable=False)
     storage = Column(UnicodeText, nullable=False)
@@ -57,7 +57,22 @@
             moment = now()
 
         if access:
             self.atime = moment
 
         if modification:
             self.mtime = moment
+
+    def patch_data(self, patch, dict_path=None, prop="plugin_data"):
+        # type: (dict[str, Any], list[str]|None, Literal["storage_data", "plugin_data"]) -> dict[str, Any]
+        data = copy.deepcopy(getattr(self, prop))  # type: dict[str, Any]
+
+        target = data  # type: dict[str, Any] | Any
+        if dict_path:
+            for part in dict_path:
+                target = target.setdefault(part, {})
+                if not isinstance(target, dict):
+                    raise TypeError(part)
+        target.update(patch)
+
+        setattr(self, prop, data)
+        return data
```

### Comparing `ckanext-files-0.2.2/ckanext/files/model/owner.py` & `ckanext-files-0.2.3/ckanext/files/model/owner.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/plugin.py` & `ckanext-files-0.2.3/ckanext/files/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/storage/fs.py` & `ckanext-files-0.2.3/ckanext/files/storage/fs.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/storage/google_cloud.py` & `ckanext-files-0.2.3/ckanext/files/storage/google_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
         super(GoogleCloudStorage, self).__init__(**settings)
 
         credentials = None
         credentials_file = settings.get("credentials_file", None)
         if credentials_file:
             try:
                 credentials = Credentials.from_service_account_file(credentials_file)
-            except FileNotFoundError:
+            except IOError:
                 raise exceptions.InvalidStorageConfigurationError(  # noqa: B904
                     type(self),
                     "file `{}` does not exist".format(credentials_file),
                 )
 
         self.client = Client(credentials=credentials)
 
@@ -288,15 +288,15 @@
     def make_manager(self):
         return GoogleCloudManager(self)
 
     @classmethod
     def declare_config_options(cls, declaration, key):
         # type: (types.Declaration, types.Key) -> None
         super().declare_config_options(declaration, key)
-        declaration.declare(key.path).required().set_description(
+        declaration.declare(key.path, "").set_description(
             "Path to the folder where uploaded data will be stored.",
         )
         declaration.declare(key.bucket).required().set_description(
             "Name of the GCS bucket where uploaded data will be stored.",
         )
         declaration.declare(key.credentials_file).set_description(
             "Path to the credentials file used for authentication by GCS client."
```

### Comparing `ckanext-files-0.2.2/ckanext/files/storage/redis.py` & `ckanext-files-0.2.3/ckanext/files/storage/redis.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,19 @@
     def copy(self, data, name, extras):
         # type: (types.MinimalStorageData, str, dict[str, types.Any]) -> RedisStorageData
         filename = self.compute_name(name, extras)
 
         src = self.storage.settings["prefix"] + data["filename"]
         dest = self.storage.settings["prefix"] + filename
 
-        self.storage.redis.copy(src, dest)
+        try:
+            self.storage.redis.copy(src, dest)
+        except AttributeError:
+            self.storage.redis.restore(dest, 0, self.storage.redis.dump(src))
+
         return RedisStorageData(data, filename=filename)
 
     def move(self, data, name, extras):
         # type: (types.MinimalStorageData, str, dict[str, types.Any]) -> RedisStorageData
         filename = self.compute_name(name, extras)
 
         src = self.storage.settings["prefix"] + data["filename"]
```

### Comparing `ckanext-files-0.2.2/ckanext/files/templates/files/snippets/file_table.html` & `ckanext-files-0.2.3/ckanext/files/templates/files/snippets/file_table.html`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/templates/files/snippets/uploader_v1.html` & `ckanext-files-0.2.3/ckanext/files/templates/files/snippets/uploader_v1.html`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/templates/files/user/delete.html` & `ckanext-files-0.2.3/ckanext/files/templates/files/user/delete.html`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/templates/files/user/index.html` & `ckanext-files-0.2.3/ckanext/files/templates/files/user/index.html`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/conftest.py` & `ckanext-files-0.2.3/ckanext/files/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,18 +43,17 @@
         migrate_db_for("files")
 
 else:
 
     @pytest.fixture
     def clean_db(reset_db):
         # type: (Any) -> None
-        from ckanext.files.command import create_tables, drop_tables
+        from ckanext.files.command import create_tables
 
         reset_db()
-        drop_tables()
         create_tables()
 
 
 class FakeFileStorage(FileStorage):
     def __init__(self, stream, filename):
         # type: (Any, str) -> None
         super(FakeFileStorage, self).__init__(stream, filename, "uplod")
```

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/logic/test_action.py` & `ckanext-files-0.2.3/ckanext/files/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/logic/test_validators.py` & `ckanext-files-0.2.3/ckanext/files/tests/logic/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/storage/test_fs.py` & `ckanext-files-0.2.3/ckanext/files/tests/storage/test_fs.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/storage/test_google_cloud.py` & `ckanext-files-0.2.3/ckanext/files/tests/storage/test_google_cloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import base64
 import hashlib
 import json
 import os
 from io import BytesIO
-from urllib.parse import quote_plus
 from uuid import UUID
 
 import pytest
 import six
+from six.moves.urllib.parse import quote_plus
 from werkzeug.datastructures import FileStorage
 
 import ckan.plugins.toolkit as tk
 
 from ckanext.files import exceptions
 from ckanext.files.storage import google_cloud as gc
```

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/storage/test_redis.py` & `ckanext-files-0.2.3/ckanext/files/tests/storage/test_redis.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/test_base.py` & `ckanext-files-0.2.3/ckanext/files/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/test_config.py` & `ckanext-files-0.2.3/ckanext/files/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/tests/test_utils.py` & `ckanext-files-0.2.3/ckanext/files/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/types.py` & `ckanext-files-0.2.3/ckanext/files/types.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext/files/utils.py` & `ckanext-files-0.2.3/ckanext/files/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
 def ensure_size(upload, max_size):
     # type: (types.Upload, int) -> int
     """Return filesize or rise an exception if it exceedes max_size."""
 
     filesize = upload.content_length
     if not filesize:
-        # in py2 .seek returns None for empty stream.
-        filesize = upload.stream.seek(0, 2) or 0
+        upload.stream.seek(0, 2)
+        filesize = upload.stream.tell()
         upload.stream.seek(0)
 
     if filesize > max_size:
         raise exceptions.LargeUploadError(filesize, max_size)
 
     return filesize
```

### Comparing `ckanext-files-0.2.2/ckanext/files/views.py` & `ckanext-files-0.2.3/ckanext/files/views.py`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/ckanext_files.egg-info/PKG-INFO` & `ckanext-files-0.2.3/ckanext_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.2
+Version: 0.2.3
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-files-0.2.2/ckanext_files.egg-info/SOURCES.txt` & `ckanext-files-0.2.3/ckanext_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/pyproject.toml` & `ckanext-files-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-files-0.2.2/setup.cfg` & `ckanext-files-0.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-files
-version = 0.2.2
+version = 0.2.3
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-files
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

