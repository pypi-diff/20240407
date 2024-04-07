# Comparing `tmp/systembridgemodels-4.1.0.tar.gz` & `tmp/systembridgemodels-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systembridgemodels-4.1.0.tar", last modified: Thu Apr  4 00:59:19 2024, max compression
+gzip compressed data, was "systembridgemodels-4.1.1.tar", last modified: Sun Apr  7 12:01:09 2024, max compression
```

## Comparing `systembridgemodels-4.1.0.tar` & `systembridgemodels-4.1.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.886464 systembridgemodels-4.1.0/systembridgemodels/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-04 00:59:17.000000 systembridgemodels-4.1.0/systembridgemodels/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/action.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.886464 systembridgemodels-4.1.0/systembridgemodels/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/media_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.886464 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/system.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/fixtures/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/media_play.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.890464 systembridgemodels-4.1.0/systembridgemodels/modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/disks.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/displays.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/processes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/modules/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/open_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/open_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/systembridgemodels/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/systembridgemodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-04 00:59:19.000000 systembridgemodels-4.1.0/systembridgemodels.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 00:59:19.894464 systembridgemodels-4.1.0/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_battery.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_disks.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_displays.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_gpus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_processes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13937 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/modules/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_keyboard_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_keyboard_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2209 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_get_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_media_play.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_notification.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_open_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_open_url.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-04 00:58:56.000000 systembridgemodels-4.1.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.492801 systembridgemodels-4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-07 12:01:09.492801 systembridgemodels-4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:01:09.492801 systembridgemodels-4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.484801 systembridgemodels-4.1.1/systembridgemodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-07 12:01:08.000000 systembridgemodels-4.1.1/systembridgemodels/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.484801 systembridgemodels-4.1.1/systembridgemodels/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/media_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.488801 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/fixtures/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/media_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/media_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/media_play.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.488801 systembridgemodels-4.1.1/systembridgemodels/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4956 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/modules/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/open_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/open_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/systembridgemodels/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.492801 systembridgemodels-4.1.1/systembridgemodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-07 12:01:09.000000 systembridgemodels-4.1.1/systembridgemodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-07 12:01:09.000000 systembridgemodels-4.1.1/systembridgemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:01:09.000000 systembridgemodels-4.1.1/systembridgemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 12:01:09.000000 systembridgemodels-4.1.1/systembridgemodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 12:01:09.000000 systembridgemodels-4.1.1/systembridgemodels.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.492801 systembridgemodels-4.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:01:09.492801 systembridgemodels-4.1.1/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_disks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_displays.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_gpus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_media.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_processes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/modules/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_keyboard_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_keyboard_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_media_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_media_directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_media_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_media_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_media_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_media_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_notification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_open_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_open_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-07 12:00:47.000000 systembridgemodels-4.1.1/tests/test_version.py
```

### Comparing `systembridgemodels-4.1.0/LICENSE` & `systembridgemodels-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/pyproject.toml` & `systembridgemodels-4.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/setup.py` & `systembridgemodels-4.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/const.py` & `systembridgemodels-4.1.1/systembridgemodels/const.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/media_files.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/cpu.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/disks.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/media.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/memory.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/networks.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/sensors.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/fixtures/modules/system.py` & `systembridgemodels-4.1.1/systembridgemodels/fixtures/modules/system.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """Fixture for system module."""
-from systembridgemodels.modules.system import System, SystemUser
+
+from systembridgemodels.modules.system import RunMode, System, SystemUser
 
 FIXTURE_SYSTEM = System(
     boot_time=1234,
     fqdn="hostname.local",
     hostname="hostname",
     ip_address_4="192.168.1.100",
     mac_address="00:00:00:00:00:00",
     platform_version="1.0.0",
     platform="platform",
+    run_mode=RunMode.STANDALONE,
     uptime=1234,
     users=[
         SystemUser(
             name="username",
             active=True,
             terminal="terminal",
             host="host",
@@ -24,10 +26,11 @@
     version="1.0.0",
     camera_usage=[
         "camera1",
         "camera2",
     ],
     ip_address_6="::1",
     pending_reboot=True,
+    version_latest_url="https://github.com/timmo001/system-bridge/releases/latest",
     version_latest="4.99.0",
     version_newer_available=True,
 )
```

### Comparing `systembridgemodels-4.1.0/systembridgemodels/media_control.py` & `systembridgemodels-4.1.1/systembridgemodels/media_control.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/media_files.py` & `systembridgemodels-4.1.1/systembridgemodels/media_files.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/__init__.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/cpu.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/cpu.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/disks.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/disks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/gpus.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/gpus.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/media.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/media.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/memory.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/memory.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/networks.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/networks.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/sensors.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/sensors.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/modules/system.py` & `systembridgemodels-4.1.1/systembridgemodels/modules/system.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 """System."""
+
 from __future__ import annotations
 
 from dataclasses import dataclass
+from enum import StrEnum
+
+
+class RunMode(StrEnum):
+    """Run Mode."""
+
+    STANDALONE = "standalone"
+    PYTHON = "python"
 
 
 @dataclass
 class SystemUser:
     """System User."""
 
     name: str
@@ -23,16 +32,18 @@
     boot_time: float
     fqdn: str
     hostname: str
     ip_address_4: str
     mac_address: str
     platform_version: str
     platform: str
+    run_mode: RunMode
     uptime: float
     users: list[SystemUser]
     uuid: str
     version: str
     camera_usage: list[str] | None = None
     ip_address_6: str | None = None
     pending_reboot: bool | None = None
+    version_latest_url: str | None = None
     version_latest: str | None = None
     version_newer_available: bool | None = None
```

### Comparing `systembridgemodels-4.1.0/systembridgemodels/notification.py` & `systembridgemodels-4.1.1/systembridgemodels/notification.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels/settings.py` & `systembridgemodels-4.1.1/systembridgemodels/settings.py`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/systembridgemodels.egg-info/SOURCES.txt` & `systembridgemodels-4.1.1/systembridgemodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `systembridgemodels-4.1.0/tests/test_media_play.py` & `systembridgemodels-4.1.1/tests/test_media_play.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 """Test the media_play model."""
 
+from syrupy.assertion import SnapshotAssertion
+
 from systembridgemodels.media_play import MediaPlay
 
 
-def test_media_play():
+def test_media_play(snapshot: SnapshotAssertion):
     """Test the media_play."""
     media_play = MediaPlay(
         url="https://www.example.com/audio.mp3",
         album="Album",
         artist="Artist",
         autoplay=True,
         cover="https://www.example.com/cover.png",
         title="Title",
         volume=100,
     )
     assert isinstance(media_play, MediaPlay)
-    assert media_play.url == "https://www.example.com/audio.mp3"
-    assert media_play.album == "Album"
-    assert media_play.artist == "Artist"
-    assert media_play.autoplay is True
-    assert media_play.cover == "https://www.example.com/cover.png"
-    assert media_play.title == "Title"
-    assert media_play.volume == 100
+    assert media_play == snapshot
```

