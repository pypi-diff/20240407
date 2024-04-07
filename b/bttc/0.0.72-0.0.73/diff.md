# Comparing `tmp/bttc-0.0.72.tar.gz` & `tmp/bttc-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bttc-0.0.72.tar", last modified: Sat Mar 30 02:57:43 2024, max compression
+gzip compressed data, was "bttc-0.0.73.tar", last modified: Sun Apr  7 14:59:20 2024, max compression
```

## Comparing `bttc-0.0.72.tar` & `bttc-0.0.73.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.135484 bttc-0.0.72/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.72/LICENSE
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2073 2024-03-30 02:57:43.131484 bttc-0.0.72/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1345 2024-03-30 02:54:41.000000 bttc-0.0.72/README.md
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5003 2024-03-30 02:54:41.000000 bttc-0.0.72/bttc/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/ble_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-03-30 02:43:20.000000 bttc-0.0.72/bttc/ble_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/bt_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    14832 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/bt_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/cli/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      606 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/cli/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/cli/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    19601 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/cli/main.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/common_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-03-30 02:43:20.000000 bttc-0.0.72/bttc/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/core.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/general_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/mobly_android_device_lib/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/mobly_android_device_lib/jsonrpc_client_base.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/mobly_android_device_lib/services/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/mobly_android_device_lib/services/sl4a_client.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/mobly_android_device_lib/services/sl4a_service.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/mobly_android_device_lib/tl4a_snippet_client.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.127484 bttc-0.0.72/bttc/profiles/
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/profiles/avrcp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/avrcp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/avrcp/avrcp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/avrcp/avrcp_target_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/avrcp/errors.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/profiles/hfp/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/hfp/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/hfp/constants.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/hfp/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/hfp/hfp_data.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/hfp/hfp_devices.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/hfp/hfp_facade.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/profiles/hfp/hfp_strategy.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/strategy.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/utils/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/ad_checker.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/device_factory.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc/utils/iperf/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/iperf/__init__.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/iperf/errors.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/key_events_handler.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/log_parser.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/logcat.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/retry.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils/typing_utils.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2868 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/utils_loader.py
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 01:52:39.000000 bttc-0.0.72/bttc/wifi_utils.py
-drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-03-30 02:57:43.131484 bttc-0.0.72/bttc.egg-info/
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     2073 2024-03-30 02:57:43.000000 bttc-0.0.72/bttc.egg-info/PKG-INFO
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1266 2024-03-30 02:57:43.000000 bttc-0.0.72/bttc.egg-info/SOURCES.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-03-30 02:57:43.000000 bttc-0.0.72/bttc.egg-info/dependency_links.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)      164 2024-03-30 02:57:43.000000 bttc-0.0.72/bttc.egg-info/requires.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-03-30 02:57:43.000000 bttc-0.0.72/bttc.egg-info/top_level.txt
--rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-03-30 02:57:43.135484 bttc-0.0.72/setup.cfg
--rw-r-----   0 johnkclee (846247) primarygroup (89939)     1682 2024-03-30 01:52:39.000000 bttc-0.0.72/setup.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.718942 bttc-0.0.73/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1061 2023-08-09 04:39:34.000000 bttc-0.0.73/LICENSE
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2075 2024-04-07 14:59:20.718942 bttc-0.0.73/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1347 2024-04-07 14:57:22.000000 bttc-0.0.73/README.md
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5003 2024-04-07 14:56:58.000000 bttc-0.0.73/bttc/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2389 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/ble_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4752 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/ble_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1723 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/bt_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    16092 2024-04-07 14:56:03.000000 bttc-0.0.73/bttc/bt_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/cli/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2100 2024-04-07 14:56:03.000000 bttc-0.0.73/bttc/cli/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1150 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/cli/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    22466 2024-04-07 14:56:03.000000 bttc-0.0.73/bttc/cli/main.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      976 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/common_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3816 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1351 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/core.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2199 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    30210 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/general_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/mobly_android_device_lib/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    13864 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/jsonrpc_client_base.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/mobly_android_device_lib/services/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6408 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_client.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2295 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_service.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     6095 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/mobly_android_device_lib/tl4a_snippet_client.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.710942 bttc-0.0.73/bttc/profiles/
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/profiles/avrcp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2077 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3189 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/avrcp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5692 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/avrcp_target_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      915 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/avrcp/errors.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc/profiles/hfp/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1221 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      962 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/constants.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      967 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1581 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_data.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     8250 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_devices.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5816 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_facade.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3324 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/profiles/hfp/hfp_strategy.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1567 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/strategy.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.718942 bttc-0.0.73/bttc/utils/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1868 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/ad_checker.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     3197 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/device_factory.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.718942 bttc-0.0.73/bttc/utils/iperf/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7860 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/iperf/__init__.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      856 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/iperf/errors.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     4643 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/key_events_handler.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7826 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/log_parser.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     7268 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/logcat.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)    43699 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/retry.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2249 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils/typing_utils.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2868 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/utils_loader.py
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     5098 2024-03-30 03:00:32.000000 bttc-0.0.73/bttc/wifi_utils.py
+drwxr-x---   0 johnkclee (846247) primarygroup (89939)        0 2024-04-07 14:59:20.714943 bttc-0.0.73/bttc.egg-info/
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     2075 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/PKG-INFO
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1266 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/SOURCES.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        1 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/dependency_links.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)      164 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/requires.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)        5 2024-04-07 14:59:20.000000 bttc-0.0.73/bttc.egg-info/top_level.txt
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)       38 2024-04-07 14:59:20.718942 bttc-0.0.73/setup.cfg
+-rw-r-----   0 johnkclee (846247) primarygroup (89939)     1682 2024-03-30 03:00:32.000000 bttc-0.0.73/setup.py
```

### Comparing `bttc-0.0.72/LICENSE` & `bttc-0.0.73/LICENSE`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/PKG-INFO` & `bttc-0.0.73/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.72
+Version: 0.0.73
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,16 +61,16 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
 * Release v0.0.66: #67, #84, #85
 * Release v0.0.65: #76, #78, #80
-* Release v0.0.64: #60, #68
```

### Comparing `bttc-0.0.72/README.md` & `bttc-0.0.73/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -42,16 +42,16 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
 * Release v0.0.66: #67, #84, #85
 * Release v0.0.65: #76, #78, #80
-* Release v0.0.64: #60, #68
```

### Comparing `bttc-0.0.72/bttc/__init__.py` & `bttc-0.0.73/bttc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from bttc import errors
 from bttc import utils_loader
 from bttc.utils import device_factory
 from ppadb import client
 from typing import TypeAlias
 
 
-__version__ = '0.0.72'
+__version__ = '0.0.73'
 __author__ = 'John Lee/Yuan Long Luo/Denny Chai'
 __credits__ = 'Google Pixel PQM'
 
 
 GeneralDevice: TypeAlias = android_device.AndroidDevice
```

### Comparing `bttc-0.0.72/bttc/ble_data.py` & `bttc-0.0.73/bttc/ble_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/ble_utils.py` & `bttc-0.0.73/bttc/ble_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/bt_data.py` & `bttc-0.0.73/bttc/bt_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/bt_utils.py` & `bttc-0.0.73/bttc/bt_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Utility to support common BT operations/methods."""
 import datetime
 from functools import partial
 import logging
+import time
 
 from mobly.controllers import android_device
 from mobly.controllers.android_device_lib import adb
 from bttc import bt_data
 from bttc import common_data
 from bttc import constants
 from bttc import core
@@ -63,14 +64,15 @@
     self._bind(get_bonded_devices)
     self._bind(get_device_mac_by_name)
     self._bind(get_connected_ble_devices)
     self._bind(get_current_le_audio_active_group_id)
     self._bind(is_le_audio_device_connected)
     self._bind(is_bluetooth_enabled, 'is_enabled')
     self._bind(list_paired_devices)
+    self._bind(unbond_device)
     self.shell = safe_adb_shell(ad)
     self.enable = partial(toggle_bluetooth, ad=ad, enabled=True)
     self.disable = partial(toggle_bluetooth, ad=ad, enabled=False)
 
   @property
   def enabled(self):
     return self.is_enabled()
@@ -457,7 +459,42 @@
   ad.log.warning(
       'Failed to toggle bluetooth with enabled=%s (rt=%s):\n%s\n',
       enabled, ret_code, stdout)
 
   raise RuntimeError(
       f'Failed in toggling bluetooth (enabled={enabled}) '
       f'with stdout: "{stdout}"')
+
+
+def unbond_device(
+    ad: android_device.AndroidDevice,
+    name_or_mac: str,
+    ignore_not_exist: bool = True,
+    wait_time_sec: float = 3) -> bool:
+  """Unbonds the BT device by its' name or MAC address.
+
+  This operation requires DUT to be initialized with SL4A service.
+
+  Args:
+    ad: The Android device object.
+    name_or_mac: Name or MAC of BT device to be unbonded.
+    ignore_not_exist: True to ignore the case that if the target BT to be
+        unbondeddoes not exist.
+
+  Returns:
+    True iff the target BT device is unbonded successfully.
+  """
+  for bt_name, bonded_device_info in ad.bt.bonded_devices.items():
+    if name_or_mac in {bt_name, bonded_device_info.mac_addr}:
+      ad.sl4a.bluetoothUnbond(bonded_device_info.mac_addr)
+      ad.log.debug(
+          'Sleep %ss for unbond action to become active...', wait_time_sec)
+      time.sleep(wait_time_sec)
+      name_or_mac_set = set()
+      for bt_name, bonded_device_info in ad.bt.bonded_devices.items():
+        name_or_mac_set.add(bt_name)
+        name_or_mac_set.add(bonded_device_info.mac_addr)
+
+      return name_or_mac not in name_or_mac_set
+
+  ad.log.warning('Target device=%s does not exist!', name_or_mac)
+  return ignore_not_exist
```

### Comparing `bttc-0.0.72/bttc/cli/constants.py` & `bttc-0.0.73/bttc/cli/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/cli/main.py` & `bttc-0.0.73/bttc/cli/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 """Entry point of BTTC Cli prompt."""
 
 import cmd2
 import copy
 import contextlib
 import datetime
 import functools
+import importlib.util
+import inspect
 import logging
 import mobly
 import os
+import pathlib
 from ppadb import client
 from pprint import pprint
 import re
 import sys
 
 import bttc
 from bttc import constants as bttc_constants
@@ -45,14 +48,19 @@
 logcat_filter_parser.add_argument(
     '--logcat_wait_sec', type=int, default=10,
     help='Time in sec to follow logcat.')
 logcat_filter_parser.add_argument(
     '--logcat_only_match', type=bool, default=False,
     help='Setup to show only matched line')
 
+load_cmd2_commandset_parser = cmd2.Cmd2ArgumentParser()
+load_cmd2_commandset_parser.add_argument(
+    '-p', '--cmd2_module_path', type=str, default=None,
+    help='Cmd2 module path where holds command set class.')
+
 
 def dec_require_dut(func):
   @functools.wraps(func)
   def wrapper(*args, **kwargs):
     self = args[0]
     is_dut_ready = False
     if isinstance(self, BttcCmdApp) and self._dut:
@@ -84,14 +92,25 @@
       return
 
     return func(*args, **kwargs)
 
   return wrapper
 
 
+@cmd2.with_default_category('john_manual')
+class TestCommandSet(cmd2.CommandSet):
+  def __init__(self, app: 'BttcCmdApp'):
+    super().__init__()
+    self._app = app
+    self.namespace_history = []
+
+  def do_john_work(self, args):
+    print("!!! Do john's Customized command test works !!!")
+
+
 @cmd2.with_default_category('device_config')
 class DeviceConfigCommandSet(cmd2.CommandSet):
   def __init__(self, app: 'BttcCmdApp'):
     super().__init__()
     self._app = app
     self.namespace_history = []
 
@@ -190,19 +209,21 @@
   def __init__(self, app: 'BttcCmdApp'):
     super().__init__()
     self._app = app
     self.property_key_history = []
 
   @dec_require_dut
   def do_airplane_mode_state(self, args):
+    """Gets DUT's airplane mode state."""
     self._app.poutput(
         f'Airplane state: {self._app._dut.gm.airplane_mode_state}\n')
 
   @dec_require_dut
   def do_device_info(self, args):
+    """Shows DUT device information."""
     device_info = copy.copy(self._app._dut.device_info)
     device_info['init_sl4a'] = self._app.dut_init_sl4a
     device_info['init_snippet_uiautomator'] = (
         self._app.dut_init_snippet_uiautomator)
     pprint(device_info)
     print('')
 
@@ -302,14 +323,15 @@
 class BTCommandSet(cmd2.CommandSet):
   def __init__(self, app: 'BttcCmdApp'):
     super().__init__()
     self._app = app
 
   @dec_require_dut
   def do_bonded_devices(self, args):
+    """Gets DUT's bonded device information."""
     bonded_devices = self._app._dut.bt.bonded_devices
     self._app.poutput(f'Total {len(bonded_devices)} bonded devices:')
     for bonded_device in bonded_devices:
       print(f'\t{bonded_device}')
 
     print('')
 
@@ -408,15 +430,15 @@
       self._app._dut.gm.take_screenshot(path)
 
     print('')
 
   @dec_require_dut
   @cmd2.with_argparser(ui_dump_parser)
   def do_ui_dump_to(self, args):
-    """Dump current UI page to host."""
+    """Dumps current UI page to host."""
     dump_path_list = args.path or ['/tmp/test.xml']
     for path in dump_path_list:
       self._app.poutput(f'Dump UI page to {path}...\n')
       self._app._dut.gm.get_ui_xml(path)
 
     print('')
 
@@ -459,18 +481,35 @@
   def _init_dut(self, serial: str):
     self._dut = bttc.get(
         serial,
         init_snippet_uiautomator=self.dut_init_snippet_uiautomator,
         init_sl4a=self.dut_init_sl4a)
     self.prompt = BttcCmdApp.DEVICE_PROMPT_PROMPT.format(serial=serial)
 
+  def do_load_test_cmd2(self, args):
+    self.register_command_set(TestCommandSet(self))
+
   @dec_require_dut
   def do_device_time(self, args):
     self.poutput(f'{self._dut.gm.device_datetime}\n')
 
+  @cmd2.with_argparser(load_cmd2_commandset_parser)
+  def do_load_cmd2_command_set(self, args):
+    """Loads cmd2 command set from given module path."""
+    target_cmd2_module_path = os.path.expanduser(args.cmd2_module_path)
+    if not os.path.isfile(target_cmd2_module_path):
+      logging.warning(
+          'The given cmd2 module path "%s" does not exist!',
+          target_cmd2_module_path)
+      return
+
+    self.poutput(
+        f'Loading cmd command set from {target_cmd2_module_path}...')
+    load_cmd2_module(self, target_cmd2_module_path)
+
   @dec_require_dut
   def do_load_sl4a(self, args):
     """Loads SL4A service in DUT."""
     device_factory.load_sl4a(self._dut)
     self.dut_init_sl4a = True
 
   @dec_require_dut
@@ -605,17 +644,54 @@
         for service_name in stopped_services:
           self.poutput(f'Unregistering {service_name}...')
           self._dut.services.unregister(service_name)
 
         self._dut.adb.forward('--remove-all')
 
 
+def load_current_workdir_cmd2_modules(c: BttcCmdApp):
+  """Loads cmd2 modules from current working directory if any."""
+  logging.debug('Searching local cmd2 module(s)...')
+  for py_module in [
+      f for f in os.listdir('.')
+      if os.path.isfile(f) and f.endswith('_cli.py')]:
+    py_module_path = os.path.join(os.getcwd(), py_module)
+    load_cmd2_module(c, py_module_path)
+
+
+def load_cmd2_module(c: BttcCmdApp, cmd2_module_path: str):
+  """Loads Cmd2 module from given file path."""
+  cmd2_module_name = pathlib.Path(cmd2_module_path).name
+  local_module_name = f'local_cmd2.{cmd2_module_name}'
+  spec = importlib.util.spec_from_file_location(
+      local_module_name, cmd2_module_path)
+  loaded_module = importlib.util.module_from_spec(spec)
+  sys.modules[local_module_name] = loaded_module
+  spec.loader.exec_module(loaded_module)
+  loaded_cmd_set_cls_num = 0
+  for cmd_set_cls in [
+      cls for _, cls in inspect.getmembers(loaded_module, inspect.isclass)
+      if issubclass(cls, cmd2.CommandSet)]:
+    print(
+        f'\t{Color.BOLD}Loaded customized cmd2 CommandSet: '
+        f'{Color.UNDERLINE}{Color.CYAN}{cmd_set_cls}{Color.END}!')
+    # CLASS_ATTR_DEFAULT_HELP_CATEGORY
+    cmd_set_obj = cmd_set_cls(c)
+    cmd_set_obj.__class__.CLASS_ATTR_DEFAULT_HELP_CATEGORY = 'hahaha'
+    c.register_command_set(cmd_set_obj)
+    loaded_cmd_set_cls_num += 1
+  print(
+      f'\t{Color.BOLD}===== Total {loaded_cmd_set_cls_num:,d}'
+      f' cmd2 CommandSet found! ====={Color.END}\n\n')
+
+
 def go(serial: str | None = None):
   """Enters Cli prompt."""
   c = BttcCmdApp(serial)
+  load_current_workdir_cmd2_modules(c)
   c.cmdloop()
   c.free_dut()
   print('=' * 10 + f' {EXIST_MSG} ' + '=' * 10)
   print('')
   os._exit(0)
```

### Comparing `bttc-0.0.72/bttc/common_data.py` & `bttc-0.0.73/bttc/common_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/constants.py` & `bttc-0.0.73/bttc/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/core.py` & `bttc-0.0.73/bttc/core.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/errors.py` & `bttc-0.0.73/bttc/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/general_utils.py` & `bttc-0.0.73/bttc/general_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/mobly_android_device_lib/jsonrpc_client_base.py` & `bttc-0.0.73/bttc/mobly_android_device_lib/jsonrpc_client_base.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/mobly_android_device_lib/services/sl4a_client.py` & `bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/mobly_android_device_lib/services/sl4a_service.py` & `bttc-0.0.73/bttc/mobly_android_device_lib/services/sl4a_service.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/mobly_android_device_lib/tl4a_snippet_client.py` & `bttc-0.0.73/bttc/mobly_android_device_lib/tl4a_snippet_client.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/avrcp/__init__.py` & `bttc-0.0.73/bttc/profiles/avrcp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/avrcp/avrcp_facade.py` & `bttc-0.0.73/bttc/profiles/avrcp/avrcp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/avrcp/avrcp_target_devices.py` & `bttc-0.0.73/bttc/profiles/avrcp/avrcp_target_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/avrcp/errors.py` & `bttc-0.0.73/bttc/profiles/avrcp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/hfp/__init__.py` & `bttc-0.0.73/bttc/profiles/hfp/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/hfp/constants.py` & `bttc-0.0.73/bttc/profiles/hfp/constants.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/hfp/errors.py` & `bttc-0.0.73/bttc/profiles/hfp/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/hfp/hfp_data.py` & `bttc-0.0.73/bttc/profiles/hfp/hfp_data.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/hfp/hfp_devices.py` & `bttc-0.0.73/bttc/profiles/hfp/hfp_devices.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/hfp/hfp_facade.py` & `bttc-0.0.73/bttc/profiles/hfp/hfp_facade.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/profiles/hfp/hfp_strategy.py` & `bttc-0.0.73/bttc/profiles/hfp/hfp_strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/strategy.py` & `bttc-0.0.73/bttc/strategy.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/ad_checker.py` & `bttc-0.0.73/bttc/utils/ad_checker.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/device_factory.py` & `bttc-0.0.73/bttc/utils/device_factory.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/iperf/__init__.py` & `bttc-0.0.73/bttc/utils/iperf/__init__.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/iperf/errors.py` & `bttc-0.0.73/bttc/utils/iperf/errors.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/key_events_handler.py` & `bttc-0.0.73/bttc/utils/key_events_handler.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/log_parser.py` & `bttc-0.0.73/bttc/utils/log_parser.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/logcat.py` & `bttc-0.0.73/bttc/utils/logcat.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/retry.py` & `bttc-0.0.73/bttc/utils/retry.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils/typing_utils.py` & `bttc-0.0.73/bttc/utils/typing_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/utils_loader.py` & `bttc-0.0.73/bttc/utils_loader.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc/wifi_utils.py` & `bttc-0.0.73/bttc/wifi_utils.py`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/bttc.egg-info/PKG-INFO` & `bttc-0.0.73/bttc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bttc
-Version: 0.0.72
+Version: 0.0.73
 Summary: A package to provide common utilities for BT testing.
 Home-page: https://github.com/johnklee/bt_test_common
 Author: John Lee/Yuan Long Luo/Denny Chai
 Author-email: puremonkey2007@gmail.com
 License: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
@@ -61,16 +61,16 @@
 >>> import bttc
 >>> dut = bttc.get('07311JECB08252', {'wifi'})
 >>> dut.wifi.status()
 <WifiStatus.ENABLED: 'enabled'>
 ```
 
 ## Release info
+* Release v0.0.73: #158, #163
 * Release v0.0.72: #153, #155, #51, #157
 * Release v0.0.71: #123, #134, #140
 * Release v0.0.70: #128, #132, #135
 * Release v0.0.69: #58, #59, #63, #109, #111, #113, #116, #119
 * Release v0.0.68: #99, #101, #103
 * Release v0.0.67: #90, #91, #95
 * Release v0.0.66: #67, #84, #85
 * Release v0.0.65: #76, #78, #80
-* Release v0.0.64: #60, #68
```

### Comparing `bttc-0.0.72/bttc.egg-info/SOURCES.txt` & `bttc-0.0.73/bttc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bttc-0.0.72/setup.py` & `bttc-0.0.73/setup.py`

 * *Files identical despite different names*

