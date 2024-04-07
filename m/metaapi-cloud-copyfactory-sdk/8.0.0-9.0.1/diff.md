# Comparing `tmp/metaapi_cloud_copyfactory_sdk-8.0.0.tar.gz` & `tmp/metaapi_cloud_copyfactory_sdk-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaapi_cloud_copyfactory_sdk-8.0.0.tar", last modified: Mon Dec 11 19:03:30 2023, max compression
+gzip compressed data, was "metaapi_cloud_copyfactory_sdk-9.0.1.tar", last modified: Sat Jan  6 06:32:59 2024, max compression
```

## Comparing `metaapi_cloud_copyfactory_sdk-8.0.0.tar` & `metaapi_cloud_copyfactory_sdk-9.0.1.tar`

### file list

```diff
@@ -1,73 +1,64 @@
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.298198 metaapi_cloud_copyfactory_sdk-8.0.0/
--rw-r--r--   0 roman      (501) staff       (20)      781 2023-02-22 08:18:57.000000 metaapi_cloud_copyfactory_sdk-8.0.0/LICENSE
--rw-r--r--   0 roman      (501) staff       (20)      181 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/MANIFEST.in
--rw-r--r--   0 roman      (501) staff       (20)    18433 2023-12-11 19:03:30.298015 metaapi_cloud_copyfactory_sdk-8.0.0/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)    17675 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/README.rst
--rw-r--r--   0 roman      (501) staff       (20)     3796 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/changelog.md
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.284165 metaapi_cloud_copyfactory_sdk-8.0.0/examples/
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.287413 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/
--rw-r--r--   0 roman      (501) staff       (20)     2776 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/copytrade.py
--rw-r--r--   0 roman      (501) staff       (20)     3674 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/externalSignal.py
--rw-r--r--   0 roman      (501) staff       (20)       24 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/requirements.txt
--rw-r--r--   0 roman      (501) staff       (20)      924 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/stopoutListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1057 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/strategyTransactionListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1000 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/strategyUserLogListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1071 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/subscriberTransactionListener.py
--rw-r--r--   0 roman      (501) staff       (20)     1014 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/subscriberUserLogListener.py
--rw-r--r--   0 roman      (501) staff       (20)     3164 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/telegram.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.290576 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/
--rw-r--r--   0 roman      (501) staff       (20)     2776 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/copyTradeExample.py
--rw-r--r--   0 roman      (501) staff       (20)     3554 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/externalSignalExample.py
--rw-r--r--   0 roman      (501) staff       (20)       24 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/requirements.txt
--rw-r--r--   0 roman      (501) staff       (20)     1030 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/stopoutListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)     1032 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/strategyTransactionListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)      975 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/strategyUserLogListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)     1046 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/subscriberTransactionListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)      989 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/subscriberUserLogListenerExample.py
--rw-r--r--   0 roman      (501) staff       (20)     3180 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/examples/exampleGenerator/telegramExample.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.291626 metaapi_cloud_copyfactory_sdk-8.0.0/lib/
--rw-r--r--   0 roman      (501) staff       (20)      270 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.293400 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/
--rw-r--r--   0 roman      (501) staff       (20)       52 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/__init__.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.295422 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/
--rw-r--r--   0 roman      (501) staff       (20)        0 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)    18595 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/configuration_client.py
--rw-r--r--   0 roman      (501) staff       (20)    32773 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/configuration_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)    44845 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/copyFactory_models.py
--rw-r--r--   0 roman      (501) staff       (20)     6630 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/history_client.py
--rw-r--r--   0 roman      (501) staff       (20)     8109 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/history_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     4458 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/signal_client.py
--rw-r--r--   0 roman      (501) staff       (20)     3944 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/signal_client_test.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.297131 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/
--rw-r--r--   0 roman      (501) staff       (20)        0 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/__init__.py
--rw-r--r--   0 roman      (501) staff       (20)      718 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/stopoutListener.py
--rw-r--r--   0 roman      (501) staff       (20)     3495 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager.py
--rw-r--r--   0 roman      (501) staff       (20)     6857 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager_test.py
--rw-r--r--   0 roman      (501) staff       (20)      711 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/transactionListener.py
--rw-r--r--   0 roman      (501) staff       (20)     7466 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/transactionListenerManager.py
--rw-r--r--   0 roman      (501) staff       (20)    15751 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/transactionListenerManager_test.py
--rw-r--r--   0 roman      (501) staff       (20)      688 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/userLogListener.py
--rw-r--r--   0 roman      (501) staff       (20)     8761 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/userLogListenerManager.py
--rw-r--r--   0 roman      (501) staff       (20)    16144 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/userLogListenerManager_test.py
--rw-r--r--   0 roman      (501) staff       (20)    12657 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/trading_client.py
--rw-r--r--   0 roman      (501) staff       (20)    13490 2023-06-06 18:24:38.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/trading_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     6821 2023-02-02 11:42:24.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/domain_client.py
--rw-r--r--   0 roman      (501) staff       (20)    14227 2023-04-07 19:11:46.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/domain_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     4922 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/errorHandler.py
--rw-r--r--   0 roman      (501) staff       (20)     7380 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/httpClient.py
--rw-r--r--   0 roman      (501) staff       (20)     8725 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/httpClient_test.py
--rw-r--r--   0 roman      (501) staff       (20)     1577 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/metaApi_client.py
--rw-r--r--   0 roman      (501) staff       (20)     2488 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/metaApi_client_test.py
--rw-r--r--   0 roman      (501) staff       (20)     1008 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/methodAccessException.py
--rw-r--r--   0 roman      (501) staff       (20)      261 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/timeoutException.py
--rw-r--r--   0 roman      (501) staff       (20)     3018 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/copyFactory.py
--rw-r--r--   0 roman      (501) staff       (20)     1984 2022-07-12 03:16:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/logger.py
--rw-r--r--   0 roman      (501) staff       (20)     3566 2022-04-12 17:17:48.000000 metaapi_cloud_copyfactory_sdk-8.0.0/lib/models.py
-drwxr-xr-x   0 roman      (501) staff       (20)        0 2023-12-11 19:03:30.297802 metaapi_cloud_copyfactory_sdk-8.0.0/metaapi_cloud_copyfactory_sdk.egg-info/
--rw-r--r--   0 roman      (501) staff       (20)    18433 2023-12-11 19:03:30.000000 metaapi_cloud_copyfactory_sdk-8.0.0/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO
--rw-r--r--   0 roman      (501) staff       (20)     2584 2023-12-11 19:03:30.000000 metaapi_cloud_copyfactory_sdk-8.0.0/metaapi_cloud_copyfactory_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 roman      (501) staff       (20)        1 2023-12-11 19:03:30.000000 metaapi_cloud_copyfactory_sdk-8.0.0/metaapi_cloud_copyfactory_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 roman      (501) staff       (20)       83 2023-12-11 19:03:30.000000 metaapi_cloud_copyfactory_sdk-8.0.0/metaapi_cloud_copyfactory_sdk.egg-info/requires.txt
--rw-r--r--   0 roman      (501) staff       (20)       30 2023-12-11 19:03:30.000000 metaapi_cloud_copyfactory_sdk-8.0.0/metaapi_cloud_copyfactory_sdk.egg-info/top_level.txt
--rw-r--r--   0 roman      (501) staff       (20)       38 2023-12-11 19:03:30.298241 metaapi_cloud_copyfactory_sdk-8.0.0/setup.cfg
--rw-r--r--   0 roman      (501) staff       (20)     1646 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-8.0.0/setup.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.934109 metaapi_cloud_copyfactory_sdk-9.0.1/
+-rw-r--r--   0 roman      (501) staff       (20)      781 2023-02-22 08:18:57.000000 metaapi_cloud_copyfactory_sdk-9.0.1/LICENSE
+-rw-r--r--   0 roman      (501) staff       (20)      161 2024-01-06 06:32:35.000000 metaapi_cloud_copyfactory_sdk-9.0.1/MANIFEST.in
+-rw-r--r--   0 roman      (501) staff       (20)    18433 2024-01-06 06:32:59.933817 metaapi_cloud_copyfactory_sdk-9.0.1/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)    17675 2023-12-11 19:01:23.000000 metaapi_cloud_copyfactory_sdk-9.0.1/README.rst
+-rw-r--r--   0 roman      (501) staff       (20)     3924 2024-01-06 06:32:35.000000 metaapi_cloud_copyfactory_sdk-9.0.1/changelog.md
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.922126 metaapi_cloud_copyfactory_sdk-9.0.1/examples/
+-rw-r--r--   0 roman      (501) staff       (20)      212 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/README.md
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.924430 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/
+-rw-r--r--   0 roman      (501) staff       (20)     2774 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/copyTradeExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     3551 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/externalSignalExample.py
+-rw-r--r--   0 roman      (501) staff       (20)       26 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/requirements.txt
+-rw-r--r--   0 roman      (501) staff       (20)     1029 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/stopoutListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     1032 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/strategyTransactionListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)      975 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/strategyUserLogListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     1046 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/subscriberTransactionListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)      989 2022-11-09 04:03:01.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/subscriberUserLogListenerExample.py
+-rw-r--r--   0 roman      (501) staff       (20)     3177 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/telegramExample.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.925417 metaapi_cloud_copyfactory_sdk-9.0.1/lib/
+-rw-r--r--   0 roman      (501) staff       (20)      274 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.928398 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/
+-rw-r--r--   0 roman      (501) staff       (20)       52 2021-03-10 17:33:56.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/__init__.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.930755 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)    18618 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/configuration_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    32723 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/configuration_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    44847 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/copyfactory_models.py
+-rw-r--r--   0 roman      (501) staff       (20)     6379 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/history_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     8283 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/history_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     4379 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/signal_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     4097 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/signal_client_test.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.932754 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/
+-rw-r--r--   0 roman      (501) staff       (20)        0 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/__init__.py
+-rw-r--r--   0 roman      (501) staff       (20)      719 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/stopout_listener.py
+-rw-r--r--   0 roman      (501) staff       (20)     3491 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/stopout_listener_manager.py
+-rw-r--r--   0 roman      (501) staff       (20)     6496 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/stopout_listener_manager_test.py
+-rw-r--r--   0 roman      (501) staff       (20)      712 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/transaction_listener.py
+-rw-r--r--   0 roman      (501) staff       (20)     7201 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/transaction_listener_manager.py
+-rw-r--r--   0 roman      (501) staff       (20)    14475 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/transaction_listener_manager_test.py
+-rw-r--r--   0 roman      (501) staff       (20)      689 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/user_log_listener.py
+-rw-r--r--   0 roman      (501) staff       (20)     8807 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/user_log_listener_manager.py
+-rw-r--r--   0 roman      (501) staff       (20)    15932 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/user_log_listener_manager_test.py
+-rw-r--r--   0 roman      (501) staff       (20)    12435 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/trading_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    13491 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/trading_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     6901 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/domain_client.py
+-rw-r--r--   0 roman      (501) staff       (20)    14325 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/domain_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     4973 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/error_handler.py
+-rw-r--r--   0 roman      (501) staff       (20)     7497 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/http_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     8804 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/http_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     1586 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/metaapi_client.py
+-rw-r--r--   0 roman      (501) staff       (20)     2539 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/metaapi_client_test.py
+-rw-r--r--   0 roman      (501) staff       (20)     1036 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/method_access_exception.py
+-rw-r--r--   0 roman      (501) staff       (20)      268 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/timeout_exception.py
+-rw-r--r--   0 roman      (501) staff       (20)     3028 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/copyfactory.py
+-rw-r--r--   0 roman      (501) staff       (20)     1987 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/logger.py
+-rw-r--r--   0 roman      (501) staff       (20)     3627 2024-01-05 05:44:25.000000 metaapi_cloud_copyfactory_sdk-9.0.1/lib/models.py
+drwxr-xr-x   0 roman      (501) staff       (20)        0 2024-01-06 06:32:59.933599 metaapi_cloud_copyfactory_sdk-9.0.1/metaapi_cloud_copyfactory_sdk.egg-info/
+-rw-r--r--   0 roman      (501) staff       (20)    18433 2024-01-06 06:32:59.000000 metaapi_cloud_copyfactory_sdk-9.0.1/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 roman      (501) staff       (20)     2257 2024-01-06 06:32:59.000000 metaapi_cloud_copyfactory_sdk-9.0.1/metaapi_cloud_copyfactory_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 roman      (501) staff       (20)        1 2024-01-06 06:32:59.000000 metaapi_cloud_copyfactory_sdk-9.0.1/metaapi_cloud_copyfactory_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 roman      (501) staff       (20)       84 2024-01-06 06:32:59.000000 metaapi_cloud_copyfactory_sdk-9.0.1/metaapi_cloud_copyfactory_sdk.egg-info/requires.txt
+-rw-r--r--   0 roman      (501) staff       (20)       30 2024-01-06 06:32:59.000000 metaapi_cloud_copyfactory_sdk-9.0.1/metaapi_cloud_copyfactory_sdk.egg-info/top_level.txt
+-rw-r--r--   0 roman      (501) staff       (20)       38 2024-01-06 06:32:59.934160 metaapi_cloud_copyfactory_sdk-9.0.1/setup.cfg
+-rw-r--r--   0 roman      (501) staff       (20)     1674 2024-01-06 06:32:35.000000 metaapi_cloud_copyfactory_sdk-9.0.1/setup.py
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/LICENSE` & `metaapi_cloud_copyfactory_sdk-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/PKG-INFO` & `metaapi_cloud_copyfactory_sdk-9.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: metaapi_cloud_copyfactory_sdk
-Version: 8.0.0
+Version: 9.0.1
 Summary: Python SDK for SDK for CopyFactory trade copying API. Can copy trades both between MetaTrader 5 (MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)
 Home-page: https://github.com/metaapi/metaapi-copyfactory-python-sdk
 Author: MetaApi DMCC
 Author-email: support@metaapi.cloud
 License: SEE LICENSE IN LICENSE
 Keywords: metaapi.cloud,MetaTrader,MetaTrader 5,MetaTrader 4,MetaTrader5,MetaTrader4,MT,MT4,MT5,forex,copy trading,API,REST,client,sdk,cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 CopyFactory trade copying API for Python (a member of `metaapi.cloud <https://metaapi.cloud>`_ project)
 #######################################################################################################
 
 CopyFactory is a powerful trade copying API which makes developing forex
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/README.rst` & `metaapi_cloud_copyfactory_sdk-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/changelog.md` & `metaapi_cloud_copyfactory_sdk-9.0.1/changelog.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+9.0.1
+  - fix broken build
+
+9.0.0
+  - breaking change: change modules naming method
+  - breaking change: migrate to Python 3.8
+
 8.0.0
   - Synchronized with JavaScript SDK 8.0.0
   - breaking change: replaced `getStrategies` api method with `getStrategiesWithInfiniteScrollPagination` and `getStrategiesWithClassicPagination` methods
   - breaking change: replaced `getPortfolioStrategies` api method with `getPortfolioStrategiesWithInfiniteScrollPagination` and `getPortfolioStrategiesWithClassicPagination` methods
   - breaking change: replaced `getSubscribers` api method with `getSubscribersWithInfiniteScrollPagination` and `getSubscribersWithClassicPagination` methods
 
 7.2.0
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/copytrade.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/copyTradeExample.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # your slave MetaApi account id
 # slave account must have SUBSCRIBER value in copyFactoryRoles
 slave_account_id = os.getenv('SLAVE_ACCOUNT_ID') or '<put in your slaveAccountId here>'
 
 
 async def configure_copyfactory():
     api = MetaApi(token)
-    copy_factory = CopyFactory(token)
+    copyfactory = CopyFactory(token)
 
     try:
         master_metaapi_account = await api.metatrader_account_api.get_account(master_account_id)
         if (
             (master_metaapi_account is None)
             or master_metaapi_account.copy_factory_roles is None
             or 'PROVIDER' not in master_metaapi_account.copy_factory_roles
@@ -36,15 +36,15 @@
             or 'SUBSCRIBER' not in slave_metaapi_account.copy_factory_roles
         ):
             raise Exception(
                 'Please specify SUBSCRIBER copyFactoryRoles value in your MetaApi '
                 'account in order to use it in CopyFactory API'
             )
 
-        configuration_api = copy_factory.configuration_api
+        configuration_api = copyfactory.configuration_api
         strategies = await configuration_api.get_strategies_with_infinite_scroll_pagination()
         strategy = next((s for s in strategies if s['accountId'] == master_metaapi_account.id), None)
         if strategy:
             strategy_id = strategy['_id']
         else:
             strategy_id = await configuration_api.generate_strategy_id()
             strategy_id = strategy_id['id']
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/externalSignal.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/externalSignalExample.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # your slave MetaApi account id
 # slave account must have SUBSCRIBER value in copyFactoryRoles
 slave_account_id = os.getenv('SLAVE_ACCOUNT_ID') or '<put in your slaveAccountId here>'
 
 
 async def external_signal():
     api = MetaApi(token)
-    copy_factory = CopyFactory(token)
+    copyfactory = CopyFactory(token)
 
     try:
         master_metaapi_account = await api.metatrader_account_api.get_account(master_account_id)
         if (
             (master_metaapi_account is None)
             or master_metaapi_account.copy_factory_roles is None
             or 'PROVIDER' not in master_metaapi_account.copy_factory_roles
@@ -36,15 +36,15 @@
             or 'SUBSCRIBER' not in slave_metaapi_account.copy_factory_roles
         ):
             raise Exception(
                 'Please specify SUBSCRIBER copyFactoryRoles value in your MetaApi '
                 'account in order to use it in CopyFactory API'
             )
 
-        configuration_api = copy_factory.configuration_api
+        configuration_api = copyfactory.configuration_api
         strategies = await configuration_api.get_strategies_with_infinite_scroll_pagination()
         strategy = next((s for s in strategies if s['accountId'] == master_metaapi_account.id), None)
         if strategy:
             strategy_id = strategy['_id']
         else:
             strategy_id = await configuration_api.generate_strategy_id()
             strategy_id = strategy_id['id']
@@ -58,32 +58,29 @@
                 'accountId': master_metaapi_account.id,
             },
         )
 
         # create subscriber
         await configuration_api.update_subscriber(
             slave_metaapi_account.id,
-            {'name': 'Test subscriber', 'subscriptions': [{'strategyId': strategy_id, 'multiplier': 1}]},
+            {'name': 'Test subscriber', 'subscriptions': [{'strategyId': strategy_id, 'multiplier': 0.01}]},
         )
 
         # send external signal
-        trading_api = copy_factory.trading_api
+        trading_api = copyfactory.trading_api
         signal_client = await trading_api.get_signal_client(slave_metaapi_account.id)
         signal_id = signal_client.generate_signal_id()
         await signal_client.update_external_signal(
             strategy_id=strategy_id,
             signal_id=signal_id,
-            signal={'symbol': 'EURUSD', 'type': 'POSITION_TYPE_BUY', 'time': datetime.now(), 'volume': 0.01},
+            signal={'symbol': 'EURUSD', 'type': 'POSITION_TYPE_BUY', 'time': datetime.now(), 'volume': 1.5},
         )
 
         await asyncio.sleep(10)
 
-        # output strategy external signals
-        print(await signal_client.get_strategy_external_signals(strategy_id))
-
         # output trading signals
         print(await signal_client.get_trading_signals())
 
         # remove external signal
         await signal_client.remove_external_signal(
             strategy_id=strategy_id, signal_id=signal_id, signal={'time': datetime.now()}
         )
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/stopoutListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/stopoutListenerExample.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
 import asyncio
 from metaapi_cloud_sdk import MetaApi
 from metaapi_cloud_sdk import CopyFactory, StopoutListener
 
 # your MetaApi API token
 token = os.getenv('TOKEN') or '<put in your token here>'
+# your subscriber MetaApi account id
+account_id = os.getenv('SLAVE_ACCOUNT_ID') or '<put in your slaveAccountId here>'
 
 
 async def stopout_example():
     api = MetaApi(token)
-    copy_factory = CopyFactory(token)
+    copyfactory = CopyFactory(token)
 
     class Listener(StopoutListener):
         async def on_stopout(self, strategy_stopout_event):
             print('Strategy stopout event', strategy_stopout_event)
 
         async def on_error(self, error: Exception):
             print('Error event', error)
 
     try:
         listener = Listener()
 
-        trading_api = copy_factory.trading_api
-        listener_id = trading_api.add_stopout_listener(listener)
-
-        while True:
-            await asyncio.sleep(10)
-
+        trading_api = copyfactory.trading_api
+        listener_id = trading_api.add_stopout_listener(listener, account_id)
+        await asyncio.sleep(300)
         trading_api.remove_stopout_listener(listener_id)
     except Exception as err:
         print(api.format_error(err))
 
+
 asyncio.run(stopout_example())
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/strategyTransactionListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/strategyTransactionListenerExample.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,16 +24,13 @@
 async def transaction_listener_example():
     api = MetaApi(token)
     try:
         listener = Listener()
 
         history_api = copyfactory.history_api
         listener_id = history_api.add_strategy_transaction_listener(listener, strategy_id)
-
-        while True:
-            await asyncio.sleep(10)
-
+        await asyncio.sleep(300)
         history_api.remove_strategy_transaction_listener(listener_id)
     except Exception as err:
         print(api.format_error(err))
 
 asyncio.run(transaction_listener_example())
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/strategyUserLogListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/strategyUserLogListenerExample.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,13 @@
 async def user_log_listener_example():
     api = MetaApi(token)
     try:
         listener = Listener()
 
         trading_api = copyfactory.trading_api
         listener_id = trading_api.add_strategy_log_listener(listener, strategy_id)
-
-        while True:
-            await asyncio.sleep(10)
-
+        await asyncio.sleep(300)
         trading_api.remove_strategy_log_listener(listener_id)
     except Exception as err:
         print(api.format_error(err))
 
 asyncio.run(user_log_listener_example())
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/subscriberTransactionListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/subscriberTransactionListenerExample.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,16 +24,13 @@
 async def transaction_listener_example():
     api = MetaApi(token)
     try:
         listener = Listener()
 
         history_api = copyfactory.history_api
         listener_id = history_api.add_subscriber_transaction_listener(listener, subscriber_id)
-
-        while True:
-            await asyncio.sleep(10)
-
+        await asyncio.sleep(300)
         history_api.remove_subscriber_transaction_listener(listener_id)
     except Exception as err:
         print(api.format_error(err))
 
 asyncio.run(transaction_listener_example())
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/subscriberUserLogListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/subscriberUserLogListenerExample.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,16 +24,13 @@
 async def user_log_listener_example():
     api = MetaApi(token)
     try:
         listener = Listener()
 
         trading_api = copyfactory.trading_api
         listener_id = trading_api.add_subscriber_log_listener(listener, subscriber_id)
-
-        while True:
-            await asyncio.sleep(10)
-
+        await asyncio.sleep(300)
         trading_api.remove_subscriber_log_listener(listener_id)
     except Exception as err:
         print(api.format_error(err))
 
 asyncio.run(user_log_listener_example())
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/examples/copytrade/telegram.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/examples/exampleGenerator/telegramExample.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,31 +16,31 @@
 # Please refer to https://metaapi.cloud/docs/copyfactory/features/telegram/publish/ for details.
 # Telegram bot token
 bot_token = os.getenv('TELEGRAM_BOT_TOKEN') or '<put in your bot_token here>'
 # Telegram chat id
 chat_id = os.getenv('TELEGRAM_CHAT_ID') or '<put in your chat_id here>'
 
 
-async def telegram():
+async def telegram_example():
     api = MetaApi(token)
-    copy_factory = CopyFactory(token)
+    copyfactory = CopyFactory(token)
 
     try:
         master_metaapi_account = await api.metatrader_account_api.get_account(master_account_id)
         if (
             (master_metaapi_account is None)
             or master_metaapi_account.copy_factory_roles is None
             or 'PROVIDER' not in master_metaapi_account.copy_factory_roles
         ):
             raise Exception(
                 'Please specify PROVIDER copyFactoryRoles value in your MetaApi '
                 'account in order to use it in CopyFactory API'
             )
 
-        configuration_api = copy_factory.configuration_api
+        configuration_api = copyfactory.configuration_api
         strategies = await configuration_api.get_strategies_with_infinite_scroll_pagination()
         strategy = next((s for s in strategies if s['accountId'] == master_metaapi_account.id), None)
         if strategy:
             strategy_id = strategy['_id']
         else:
             strategy_id = await configuration_api.generate_strategy_id()
             strategy_id = strategy_id['id']
@@ -53,15 +53,15 @@
                 'description': 'Some useful description about your strategy',
                 'accountId': master_metaapi_account.id,
                 'telegram': {'publishing': {'token': bot_token, 'chatId': chat_id, 'template': '${description}'}},
             },
         )
 
         # send external signal
-        trading_api = copy_factory.trading_api
+        trading_api = copyfactory.trading_api
         signal_client = await trading_api.get_signal_client(master_metaapi_account.id)
         signal_id = signal_client.generate_signal_id()
         await signal_client.update_external_signal(
             strategy_id=strategy_id,
             signal_id=signal_id,
             signal={'symbol': 'EURUSD', 'type': 'POSITION_TYPE_BUY', 'time': datetime.now(), 'volume': 0.01},
         )
@@ -72,8 +72,8 @@
         await signal_client.remove_external_signal(
             strategy_id=strategy_id, signal_id=signal_id, signal={'time': datetime.now()}
         )
     except Exception as err:
         print(api.format_error(err))
 
 
-asyncio.run(telegram())
+asyncio.run(telegram_example())
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/configuration_client.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/configuration_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,42 @@
-from ..metaApi_client import MetaApiClient
-from ...models import random_id, convert_iso_time_to_date, format_request
-from .copyFactory_models import (
+from copy import deepcopy
+from typing import List, Union
+
+from .copyfactory_models import (
     StrategyId,
     CopyFactoryStrategyUpdate,
     CopyFactorySubscriberUpdate,
     CopyFactorySubscriber,
     CopyFactoryStrategy,
     CopyFactoryPortfolioStrategy,
     CopyFactoryPortfolioStrategyUpdate,
     CopyFactoryCloseInstructions,
     GetStrategiesOptions,
     ApiVersion,
     GetPortfolioStrategiesOptions,
     ClassicPaginationList,
     GetSubscribersOptions,
 )
-from typing import List, Union
 from ..domain_client import DomainClient
-from copy import deepcopy
+from ..metaapi_client import MetaApiClient
+from ...models import random_id, convert_iso_time_to_date, format_request
 
 
 class ConfigurationClient(MetaApiClient):
     """metaapi.cloud CopyFactory configuration API (trade copying configuration API) client (see
     https://metaapi.cloud/docs/copyfactory/)"""
 
     def __init__(self, domain_client: DomainClient):
-        """Inits CopyFactory configuration API client instance.
+        """Initializes CopyFactory configuration API client instance.
 
         Args:
             domain_client: Domain client.
         """
         super().__init__(domain_client)
-        self._domainClient = domain_client
+        self._domain_client = domain_client
 
     async def generate_strategy_id(self) -> StrategyId:
         """Retrieves new unused strategy id. Method is accessible only with API access token. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/generateStrategyId/
 
         Returns:
             A coroutine resolving with strategy id generated.
@@ -43,15 +44,15 @@
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('generate_strategy_id')
         opts = {
             'url': f"/users/current/configuration/unused-strategy-id",
             'method': 'GET',
             'headers': {'auth-token': self._token},
         }
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     @staticmethod
     def generate_account_id() -> str:
         """Generates random account id.
 
         Returns:
             Account id.
@@ -103,15 +104,15 @@
             return self._handle_no_access_exception('get_strategies')
         opts = {
             'url': f"/users/current/configuration/strategies",
             'method': 'GET',
             'params': options,
             'headers': {'auth-token': self._token, 'api-version': api_version},
         }
-        result = await self._domainClient.request_copyfactory(opts, True)
+        result = await self._domain_client.request_copyfactory(opts, True)
         convert_iso_time_to_date(result)
         return result
 
     async def get_strategy(self, strategy_id: str) -> CopyFactoryStrategy:
         """Retrieves CopyFactory copy trading strategy by id. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/getStrategy/
 
@@ -124,15 +125,15 @@
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_strategy')
         opts = {
             'url': f"/users/current/configuration/strategies/{strategy_id}",
             'method': 'GET',
             'headers': {'auth-token': self._token},
         }
-        strategy = await self._domainClient.request_copyfactory(opts)
+        strategy = await self._domain_client.request_copyfactory(opts)
         convert_iso_time_to_date(strategy)
         return strategy
 
     async def update_strategy(self, strategy_id: str, strategy: CopyFactoryStrategyUpdate):
         """Updates a CopyFactory strategy. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/updateStrategy/
 
@@ -149,15 +150,15 @@
         format_request(payload)
         opts = {
             'url': f"/users/current/configuration/strategies/{strategy_id}",
             'method': 'PUT',
             'headers': {'auth-token': self._token},
             'body': payload,
         }
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def remove_strategy(self, strategy_id: str, close_instructions: CopyFactoryCloseInstructions = None):
         """Deletes a CopyFactory strategy. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/removeStrategy/
 
         Args:
             strategy_id: Copy trading strategy id.
@@ -172,15 +173,15 @@
             'url': f"/users/current/configuration/strategies/{strategy_id}",
             'method': 'DELETE',
             'headers': {'auth-token': self._token},
         }
         if close_instructions is not None:
             format_request(close_instructions)
             opts['body'] = close_instructions
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def get_portfolio_strategies_with_infinite_scroll_pagination(
         self, options: GetPortfolioStrategiesOptions = None
     ) -> List[CopyFactoryStrategy]:
         """Retrieves CopyFactory copy portfolio strategies. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/getPortfolioStrategies/
 
@@ -225,15 +226,15 @@
             return self._handle_no_access_exception('get_portfolio_strategies')
         opts = {
             'url': f"/users/current/configuration/portfolio-strategies",
             'method': 'GET',
             'params': options,
             'headers': {'auth-token': self._token, 'api-version': api_version},
         }
-        result = await self._domainClient.request_copyfactory(opts, True)
+        result = await self._domain_client.request_copyfactory(opts, True)
         convert_iso_time_to_date(result)
         return result
 
     async def get_portfolio_strategy(self, portfolio_id: str) -> CopyFactoryPortfolioStrategy:
         """Retrieves a CopyFactory copy portfolio strategy by id. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/getPortfolioStrategy/
 
@@ -246,15 +247,15 @@
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_portfolio_strategy')
         opts = {
             'url': f"/users/current/configuration/portfolio-strategies/{portfolio_id}",
             'method': 'GET',
             'headers': {'auth-token': self._token},
         }
-        strategy = await self._domainClient.request_copyfactory(opts)
+        strategy = await self._domain_client.request_copyfactory(opts)
         convert_iso_time_to_date(strategy)
         return strategy
 
     async def update_portfolio_strategy(self, portfolio_id: str, portfolio: CopyFactoryPortfolioStrategyUpdate):
         """Updates a CopyFactory portfolio strategy. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/updatePortfolioStrategy/
 
@@ -271,15 +272,15 @@
         format_request(payload)
         opts = {
             'url': f"/users/current/configuration/portfolio-strategies/{portfolio_id}",
             'method': 'PUT',
             'headers': {'auth-token': self._token},
             'body': payload,
         }
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def remove_portfolio_strategy(
         self, portfolio_id: str, close_instructions: CopyFactoryCloseInstructions = None
     ):
         """Deletes a CopyFactory portfolio strategy. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/removePortfolioStrategy/
 
@@ -296,15 +297,15 @@
             'url': f"/users/current/configuration/portfolio-strategies/{portfolio_id}",
             'method': 'DELETE',
             'headers': {'auth-token': self._token},
         }
         if close_instructions is not None:
             format_request(close_instructions)
             opts['body'] = close_instructions
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def remove_portfolio_strategy_member(
         self, portfolio_id: str, strategy_id: str, close_instructions: CopyFactoryCloseInstructions = None
     ):
         """Deletes a portfolio strategy member. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/removePortfolioStrategyMember/
 
@@ -322,15 +323,15 @@
             'url': f"/users/current/configuration/portfolio-strategies/{portfolio_id}" f"/members/{strategy_id}",
             'method': 'DELETE',
             'headers': {'auth-token': self._token},
         }
         if close_instructions is not None:
             format_request(close_instructions)
             opts['body'] = close_instructions
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def get_subscribers_with_infinite_scroll_pagination(
         self, options: GetSubscribersOptions = None
     ) -> List[CopyFactorySubscriber]:
         """Returns CopyFactory subscribers the user has configured. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/getSubscribers/
 
@@ -373,15 +374,15 @@
             return self._handle_no_access_exception('get_subscribers')
         opts = {
             'url': f"/users/current/configuration/subscribers",
             'method': 'GET',
             'params': options,
             'headers': {'auth-token': self._token, 'api-version': api_version},
         }
-        result = await self._domainClient.request_copyfactory(opts, True)
+        result = await self._domain_client.request_copyfactory(opts, True)
         convert_iso_time_to_date(result)
         return result
 
     async def get_subscriber(self, subscriber_id: str) -> CopyFactorySubscriber:
         """Returns CopyFactory subscriber by id. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/getSubscriber/
 
@@ -394,15 +395,15 @@
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_subscriber')
         opts = {
             'url': f"/users/current/configuration/subscribers/{subscriber_id}",
             'method': 'GET',
             'headers': {'auth-token': self._token},
         }
-        subscriber = await self._domainClient.request_copyfactory(opts)
+        subscriber = await self._domain_client.request_copyfactory(opts)
         convert_iso_time_to_date(subscriber)
         return subscriber
 
     async def update_subscriber(self, subscriber_id: str, subscriber: CopyFactorySubscriberUpdate):
         """Updates CopyFactory subscriber configuration. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/updateSubscriber/
 
@@ -419,15 +420,15 @@
         format_request(payload)
         opts = {
             'url': f"/users/current/configuration/subscribers/{subscriber_id}",
             'method': 'PUT',
             'headers': {'auth-token': self._token},
             'body': payload,
         }
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def remove_subscriber(self, subscriber_id: str, close_instructions: CopyFactoryCloseInstructions = None):
         """Deletes subscriber configuration. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/removeSubscriber/
 
         Args:
             subscriber_id: Subscriber id.
@@ -442,15 +443,15 @@
             'url': f"/users/current/configuration/subscribers/{subscriber_id}",
             'method': 'DELETE',
             'headers': {'auth-token': self._token},
         }
         if close_instructions is not None:
             format_request(close_instructions)
             opts['body'] = close_instructions
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def remove_subscription(
         self, subscriber_id: str, strategy_id: str, close_instructions: CopyFactoryCloseInstructions = None
     ):
         """Deletes a subscription of subscriber to a strategy. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/configuration/removeSubscription/
 
@@ -468,8 +469,8 @@
             'url': f"/users/current/configuration/subscribers/{subscriber_id}/subscriptions/{strategy_id}",
             'method': 'DELETE',
             'headers': {'auth-token': self._token},
         }
         if close_instructions is not None:
             format_request(close_instructions)
             opts['body'] = close_instructions
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/configuration_client_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/configuration_client_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from .configuration_client import ConfigurationClient
-from ...models import date, format_date
-import pytest
-import json
-import respx
 from copy import deepcopy
-from httpx import Response
+
+import pytest
 from mock import MagicMock, AsyncMock
 
+from .configuration_client import ConfigurationClient
+from ...models import date, format_date
+
 domain_client = MagicMock()
 copy_factory_client = ConfigurationClient(domain_client)
 token = 'header.payload.sign'
 
 
 @pytest.fixture(autouse=True)
 async def run_around_tests():
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/copyFactory_models.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/copyfactory_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing_extensions import TypedDict, Literal
-from typing import List, Optional, TypeVar
 from datetime import datetime
 from enum import Enum
+from typing import List, Optional, TypeVar
+
+from typing_extensions import TypedDict, Literal
 
 CopyFactoryStrategySymbolMapping = TypedDict(
     "CopyFactoryStrategySymbolMapping",
     {"from": str, "to": str},  # Symbol name to convert from.  # Symbol name to convert to.
 )
 """CopyFactory strategy symbol mapping."""
 
@@ -231,15 +232,15 @@
     setting will act as an extra line of protection to restrict trades if actual risk exceeds the value of expected
     subscription risk multiplied by maxRiskCoefficient. As a result trade volume will be decreased correspondingly or
     trade will be skipped if resulting volume is less than minVolume. Default value is 5, minimum value is 1."""
     expression: Optional[str]
     """math.js expression which will be used to calculate trade volume
     (see https://mathjs.org/docs/expressions/syntax.html). Following variables are available in expression
     scope: providerVolume - provider signal trade size; providerTradeAmount - provider signal trade value in
-    trade copier base curency; multiplier - subscription multiplier value; providerBalance - provider balance
+    trade copier base currency; multiplier - subscription multiplier value; providerBalance - provider balance
     value in trade copier base currency; balance - subscriber balance value in trade copier base currency;
     quoteOrOpenPrice - current asset price (for market orders) or open price (for pending orders) on subscriber
     side; tickValue - current asset tick value on subscriber side expressed in trade copier base currency;
     tickSize - tick size on subscriber side; providerScaledVolume - provider trade volume multiplied by provider
     contract size; contractSize - subscriber contract size; providerStopLoss - provider signal stop loss price;
     providerTakeProfit - provider signal take profit price; accountCurrencyExchangeRate - subscriber exchange
     rate of account currency to trade copier base currency."""
@@ -334,15 +335,15 @@
     allowed to open new positions with a symbol equal to the symbol of an existing strategy position (can be used to
     gracefully exit strategies trading in netting mode or placing a series of related trades per symbol). immediately
     means to close all positions immediately. One of 'by-position', 'by-symbol', 'immediately'."""
     riskLimits: Optional[List[CopyFactoryStrategyRiskLimit]]
     """Account risk limits. You can configure trading to be stopped once total drawdown generated during
     specific period is exceeded. Can be specified either for balance or equity drawdown."""
     maxLeverage: Optional[float]
-    """Setting indicating maxumum leverage allowed when opening a new positions. Any trade which results in a
+    """Setting indicating maximum leverage allowed when opening a new positions. Any trade which results in a
     higher leverage will be discarded."""
     copyStopLoss: Optional[bool]
     """Flag indicating whether stop loss should be copied. Default is to copy stop loss."""
     copyTakeProfit: Optional[bool]
     """Flag indicating whether take profit should be copied. Default is to copy take profit."""
     allowedSides: Optional[List[str]]
     """Trade sides which will be copied. Buy trades only, sell trades only or all trades. Default is to copy
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/history_client.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/history_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,41 @@
-from ..metaApi_client import MetaApiClient
-from ...models import format_date, convert_iso_time_to_date
-from .copyFactory_models import CopyFactoryTransaction
-from .streaming.transactionListenerManager import TransactionListenerManager
-from .streaming.transactionListener import TransactionListener
 from datetime import datetime
 from typing import List
+
+from .copyfactory_models import CopyFactoryTransaction
+from .streaming.transaction_listener import TransactionListener
+from .streaming.transaction_listener_manager import TransactionListenerManager
 from ..domain_client import DomainClient
+from ..metaapi_client import MetaApiClient
+from ...models import format_date, convert_iso_time_to_date
 
 
 class HistoryClient(MetaApiClient):
     """metaapi.cloud CopyFactory history API (trade copying history API) client (see
     https://metaapi.cloud/docs/copyfactory/)"""
 
     def __init__(self, domain_client: DomainClient):
-        """Inits CopyFactory history API client instance.
+        """Initializes CopyFactory history API client instance.
 
         Args:
             domain_client: Domain client.
         """
         super().__init__(domain_client)
-        self._domainClient = domain_client
-        self._transactionListenerManager = TransactionListenerManager(domain_client)
+        self._domain_client = domain_client
+        self._transaction_listener_manager = TransactionListenerManager(domain_client)
 
-    async def get_provided_transactions(self, time_from: datetime, time_till: datetime,
-                                        strategy_ids: List[str] = None, subscriber_ids: List[str] = None,
-                                        offset: int = None, limit: int = None) -> 'List[CopyFactoryTransaction]':
+    async def get_provided_transactions(
+        self,
+        time_from: datetime,
+        time_till: datetime,
+        strategy_ids: List[str] = None,
+        subscriber_ids: List[str] = None,
+        offset: int = None,
+        limit: int = None,
+    ) -> 'List[CopyFactoryTransaction]':
         """Returns list of transactions on the strategies the current user provides to other users. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/history/getProvidedTransactions/
 
         Args:
             time_from: Time to load transactions from.
             time_till: Time to load transactions till.
             strategy_ids: The list of strategy ids to filter transactions by.
@@ -37,42 +44,42 @@
             limit: Pagination limit. Default value is 1000.
 
         Returns:
             A coroutine resolving with transactions found.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_provided_transactions')
-        params = {
-            'from': format_date(time_from),
-            'till': format_date(time_till)
-        }
+        params = {'from': format_date(time_from), 'till': format_date(time_till)}
         if strategy_ids:
             params['strategyId'] = strategy_ids
         if subscriber_ids:
             params['subscriberId'] = subscriber_ids
         if not (offset is None):
             params['offset'] = offset
         if limit:
             params['limit'] = limit
         opts = {
-          'url': f'/users/current/provided-transactions',
-          'method': 'GET',
-          'headers': {
-            'auth-token': self._token
-          },
-          'params': params
+            'url': f'/users/current/provided-transactions',
+            'method': 'GET',
+            'headers': {'auth-token': self._token},
+            'params': params,
         }
-        transactions = await self._domainClient.request_copyfactory(opts, True)
+        transactions = await self._domain_client.request_copyfactory(opts, True)
         convert_iso_time_to_date(transactions)
         return transactions
 
-    async def get_subscription_transactions(self, time_from: datetime, time_till: datetime,
-                                            strategy_ids: List[str] = None, subscriber_ids: List[str] = None,
-                                            offset: int = None, limit: int = None) -> \
-            'List[CopyFactoryTransaction]':
+    async def get_subscription_transactions(
+        self,
+        time_from: datetime,
+        time_till: datetime,
+        strategy_ids: List[str] = None,
+        subscriber_ids: List[str] = None,
+        offset: int = None,
+        limit: int = None,
+    ) -> 'List[CopyFactoryTransaction]':
         """Returns list of trades on the strategies the current user subscribed to
         https://metaapi.cloud/docs/copyfactory/restApi/api/history/getSubscriptionTransactions/
 
         Args:
             time_from: Time to load transactions from.
             time_till: Time to load transactions till.
             strategy_ids: The list of strategy ids to filter transactions by.
@@ -81,75 +88,73 @@
             limit: Pagination limit. Default value is 1000.
 
         Returns:
             A coroutine resolving with transactions found.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_subscription_transactions')
-        params = {
-            'from': format_date(time_from),
-            'till': format_date(time_till)
-        }
+        params = {'from': format_date(time_from), 'till': format_date(time_till)}
         if strategy_ids:
             params['strategyId'] = strategy_ids
         if subscriber_ids:
             params['subscriberId'] = subscriber_ids
         if not (offset is None):
             params['offset'] = offset
         if limit:
             params['limit'] = limit
         opts = {
-          'url': f'/users/current/subscription-transactions',
-          'method': 'GET',
-          'headers': {
-            'auth-token': self._token
-          },
-          'params': params
+            'url': f'/users/current/subscription-transactions',
+            'method': 'GET',
+            'headers': {'auth-token': self._token},
+            'params': params,
         }
-        transactions = await self._domainClient.request_copyfactory(opts, True)
+        transactions = await self._domain_client.request_copyfactory(opts, True)
         convert_iso_time_to_date(transactions)
         return transactions
 
-    def add_strategy_transaction_listener(self, listener: TransactionListener, strategy_id: str,
-                                          start_time: datetime = None) -> str:
+    def add_strategy_transaction_listener(
+        self, listener: TransactionListener, strategy_id: str, start_time: datetime = None
+    ) -> str:
         """Adds a strategy transaction listener and creates a job to make requests.
 
         Args:
             listener: Transaction listener.
             strategy_id: Strategy id.
             start_time: Transaction search start time.
 
         Returns:
             Listener id.
         """
-        return self._transactionListenerManager.add_strategy_transaction_listener(listener, strategy_id, start_time)
+        return self._transaction_listener_manager.add_strategy_transaction_listener(listener, strategy_id, start_time)
 
     def remove_strategy_transaction_listener(self, listener_id: str):
         """Removes strategy transaction listener and cancels the event stream.
 
         Args:
             listener_id: Strategy transaction listener id.
         """
-        self._transactionListenerManager.remove_strategy_transaction_listener(listener_id)
+        self._transaction_listener_manager.remove_strategy_transaction_listener(listener_id)
 
-    def add_subscriber_transaction_listener(self, listener: TransactionListener, subscriber_id: str,
-                                            start_time: datetime = None) -> str:
+    def add_subscriber_transaction_listener(
+        self, listener: TransactionListener, subscriber_id: str, start_time: datetime = None
+    ) -> str:
         """Adds a subscriber transaction listener and creates a job to make requests.
 
         Args:
             listener: Transaction listener.
             subscriber_id: Subscriber id.
             start_time: Transaction search start time.
 
         Returns:
             Listener id.
         """
-        return self._transactionListenerManager.add_subscriber_transaction_listener(listener, subscriber_id,
-                                                                                    start_time)
+        return self._transaction_listener_manager.add_subscriber_transaction_listener(
+            listener, subscriber_id, start_time
+        )
 
     def remove_subscriber_transaction_listener(self, listener_id: str):
         """Removes subscriber transaction listener and cancels the event stream.
 
         Args:
             listener_id: Subscriber transaction listener id.
         """
-        self._transactionListenerManager.remove_subscriber_transaction_listener(listener_id)
+        self._transaction_listener_manager.remove_subscriber_transaction_listener(listener_id)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/history_client_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/history_client_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-from .history_client import HistoryClient
-from ...models import date, format_date
 from datetime import datetime
+
 import pytest
 import respx
 from mock import MagicMock, AsyncMock
+
+from .history_client import HistoryClient
+from ...models import date, format_date
+
 domain_client = MagicMock()
 history_client = HistoryClient(domain_client)
 token = 'header.payload.sign'
 
 
 @pytest.fixture(autouse=True)
 async def run_around_tests():
@@ -20,177 +23,174 @@
 
 
 class TestHistoryClient:
     @respx.mock
     @pytest.mark.asyncio
     async def test_retrieve_transactions_for_provided_strategies_from_api(self):
         """Should retrieve transactions performed on provided strategies from API."""
-        expected = [{
-            'id': '64664661:close',
-            'type': 'DEAL_TYPE_SELL',
-            'time': '2020-08-02T21:01:01.830Z',
-            'subscriberId': 'e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
-            'symbol': 'EURJPY',
-            'subscriber': {
-                'id': 'subscriberId',
-                'name': 'Subscriber'
-            },
-            'demo': False,
-            'providerUser': {
-                'id': 'providerId',
-                'name': 'Provider'
-            },
-            'strategy': {
-                'id': 'ABCD'
-            },
-            'improvement': 0,
-            'providerCommission': 0,
-            'platformCommission': 0,
-            'quantity': -0.04,
-            'lotPrice': 117566.08744776,
-            'tickPrice': 124.526,
-            'amount': -4702.643497910401,
-            'commission': -0.14,
-            'swap': -0.14,
-            'profit': 0.49
-        }]
+        expected = [
+            {
+                'id': '64664661:close',
+                'type': 'DEAL_TYPE_SELL',
+                'time': '2020-08-02T21:01:01.830Z',
+                'subscriberId': 'e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
+                'symbol': 'EURJPY',
+                'subscriber': {'id': 'subscriberId', 'name': 'Subscriber'},
+                'demo': False,
+                'providerUser': {'id': 'providerId', 'name': 'Provider'},
+                'strategy': {'id': 'ABCD'},
+                'improvement': 0,
+                'providerCommission': 0,
+                'platformCommission': 0,
+                'quantity': -0.04,
+                'lotPrice': 117566.08744776,
+                'tickPrice': 124.526,
+                'amount': -4702.643497910401,
+                'commission': -0.14,
+                'swap': -0.14,
+                'profit': 0.49,
+            }
+        ]
         time_from = datetime.now()
         time_till = datetime.now()
         domain_client.request_copyfactory = AsyncMock(return_value=expected)
         accounts = await history_client.get_provided_transactions(
-            time_from, time_till, ['ABCD'], ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'], 100, 200)
+            time_from, time_till, ['ABCD'], ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'], 100, 200
+        )
         expected[0]['time'] = date(expected[0]['time'])
         assert accounts == expected
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/provided-transactions',
-            'method': 'GET',
-            'headers': {
-                'auth-token': token
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/provided-transactions',
+                'method': 'GET',
+                'headers': {'auth-token': token},
+                'params': {
+                    'from': format_date(time_from),
+                    'till': format_date(time_till),
+                    'strategyId': ['ABCD'],
+                    'subscriberId': ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'],
+                    'offset': 100,
+                    'limit': 200,
+                },
             },
-            'params': {
-                'from': format_date(time_from),
-                'till': format_date(time_till),
-                'strategyId': ['ABCD'],
-                'subscriberId': ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'],
-                'offset': 100,
-                'limit': 200
-            },
-        }, True)
+            True,
+        )
 
     @pytest.mark.asyncio
     async def test_not_retrieve_transactions_for_provided_strategies_with_account_token(self):
         """Should not retrieve transactions on provided strategies from API with account token."""
         domain_client.token = 'token'
         history_client = HistoryClient(domain_client)
         try:
             await history_client.get_provided_transactions(datetime.now(), datetime.now())
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke get_provided_transactions method, because ' + \
-                   'you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke get_provided_transactions method, because '
+                + 'you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_retrieve_transactions_for_subscribed_strategies_from_api(self):
         """Should retrieve transactions performed on strategies current user is subscribed to from API."""
-        expected = [{
-            'id': '64664661:close',
-            'type': 'DEAL_TYPE_SELL',
-            'time': '2020-08-02T21:01:01.830Z',
-            'subscriberId': 'e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
-            'symbol': 'EURJPY',
-            'subscriberUser': {
-                'id': 'subscriberId',
-                'name': 'Subscriber'
-            },
-            'demo': False,
-            'providerUser': {
-                'id': 'providerId',
-                'name': 'Provider'
-            },
-            'strategy': {
-                'id': 'ABCD'
-            },
-            'improvement': 0,
-            'providerCommission': 0,
-            'platformCommission': 0,
-            'quantity': -0.04,
-            'lotPrice': 117566.08744776,
-            'tickPrice': 124.526,
-            'amount': -4702.643497910401,
-            'commission': -0.14,
-            'swap': -0.14,
-            'profit': 0.49
-        }]
+        expected = [
+            {
+                'id': '64664661:close',
+                'type': 'DEAL_TYPE_SELL',
+                'time': '2020-08-02T21:01:01.830Z',
+                'subscriberId': 'e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
+                'symbol': 'EURJPY',
+                'subscriberUser': {'id': 'subscriberId', 'name': 'Subscriber'},
+                'demo': False,
+                'providerUser': {'id': 'providerId', 'name': 'Provider'},
+                'strategy': {'id': 'ABCD'},
+                'improvement': 0,
+                'providerCommission': 0,
+                'platformCommission': 0,
+                'quantity': -0.04,
+                'lotPrice': 117566.08744776,
+                'tickPrice': 124.526,
+                'amount': -4702.643497910401,
+                'commission': -0.14,
+                'swap': -0.14,
+                'profit': 0.49,
+            }
+        ]
         time_from = datetime.now()
         time_till = datetime.now()
         domain_client.request_copyfactory = AsyncMock(return_value=expected)
         accounts = await history_client.get_subscription_transactions(
-            time_from, time_till, ['ABCD'], ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'], 100, 200)
+            time_from, time_till, ['ABCD'], ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'], 100, 200
+        )
         expected[0]['time'] = date(expected[0]['time'])
         assert accounts == expected
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/subscription-transactions',
-            'method': 'GET',
-            'headers': {
-                'auth-token': token
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/subscription-transactions',
+                'method': 'GET',
+                'headers': {'auth-token': token},
+                'params': {
+                    'from': format_date(time_from),
+                    'till': format_date(time_till),
+                    'strategyId': ['ABCD'],
+                    'subscriberId': ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'],
+                    'offset': 100,
+                    'limit': 200,
+                },
             },
-            'params': {
-                'from': format_date(time_from),
-                'till': format_date(time_till),
-                'strategyId': ['ABCD'],
-                'subscriberId': ['e8867baa-5ec2-45ae-9930-4d5cea18d0d6'],
-                'offset': 100,
-                'limit': 200
-            },
-        }, True)
+            True,
+        )
 
     @pytest.mark.asyncio
     async def test_not_retrieve_transactions_for_subscribed_strategies_with_account_token(self):
         """Should not retrieve transactions on strategies subscribed to from API with account token."""
         history_client = HistoryClient(domain_client)
         try:
             await history_client.get_subscription_transactions(datetime.now(), datetime.now())
         except Exception as err:
-            assert err.__str__() == 'You can not invoke get_subscription_transactions method, ' + \
-                   'because you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke get_subscription_transactions method, '
+                + 'because you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
 
 class TestTransactionListener:
-
     @pytest.mark.asyncio
     async def test_add_strategy_transaction_listener(self):
         """Should add strategy listener."""
         call_stub = MagicMock(return_value='listenerId')
-        history_client._transactionListenerManager.add_strategy_transaction_listener = call_stub
+        history_client._transaction_listener_manager.add_strategy_transaction_listener = call_stub
         listener = MagicMock()
         listener_id = history_client.add_strategy_transaction_listener(listener, 'ABCD')
         assert listener_id == 'listenerId'
         call_stub.assert_called_with(listener, 'ABCD', None)
 
     @pytest.mark.asyncio
     async def test_remove_strategy_transaction_listener(self):
         """Should remove strategy listener."""
         call_stub = MagicMock()
-        history_client._transactionListenerManager.remove_strategy_transaction_listener = call_stub
+        history_client._transaction_listener_manager.remove_strategy_transaction_listener = call_stub
         history_client.remove_strategy_transaction_listener('id')
         call_stub.assert_called_with('id')
 
     @pytest.mark.asyncio
     async def test_add_subscriber_transaction_listener(self):
         """Should add subscriber listener."""
         call_stub = MagicMock(return_value='listenerId')
-        history_client._transactionListenerManager.add_subscriber_transaction_listener = call_stub
+        history_client._transaction_listener_manager.add_subscriber_transaction_listener = call_stub
         listener = MagicMock()
         listener_id = history_client.add_subscriber_transaction_listener(listener, 'accountId')
         assert listener_id == 'listenerId'
         call_stub.assert_called_with(listener, 'accountId', None)
 
     @pytest.mark.asyncio
     async def test_remove_subscriber_transaction_listener(self):
         """Should remove subscriber listener."""
         call_stub = MagicMock()
-        history_client._transactionListenerManager.remove_subscriber_transaction_listener = call_stub
+        history_client._transaction_listener_manager.remove_subscriber_transaction_listener = call_stub
         history_client.remove_subscriber_transaction_listener('id')
         call_stub.assert_called_with('id')
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/signal_client.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/signal_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from ..domain_client import DomainClient
-from .copyFactory_models import CopyFactoryExternalSignalUpdate, CopyFactoryExternalSignalRemove, \
-    CopyFactoryTradingSignal, CopyFactoryExternalSignal
-from typing import List
 from copy import deepcopy
+from typing import List
+
+from .copyfactory_models import (
+    CopyFactoryExternalSignalUpdate,
+    CopyFactoryExternalSignalRemove,
+    CopyFactoryTradingSignal,
+    CopyFactoryExternalSignal,
+)
+from ..domain_client import DomainClient
 from ...models import convert_iso_time_to_date, format_request, random_id
 
 
 class SignalClient:
     """CopyFactory client for signal requests."""
 
     def __init__(self, account_id: str, host: dict, domain_client: DomainClient):
-        """Inits CopyFactory signal client instance.
+        """Initializes CopyFactory signal client instance.
 
         Args:
             account_id: Account id.
             host: Host data.
             domain_client: Domain client.
         """
-        self._accountId = account_id
-        self._domainClient = domain_client
+        self._account_id = account_id
+        self._domain_client = domain_client
         self._host = host
 
     @staticmethod
     def generate_signal_id():
         """Generates random signal id.
 
         Returns:
@@ -34,21 +39,19 @@
         """Returns trading signals the subscriber is subscribed to. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/getTradingSignals/
 
         Returns:
             A coroutine which resolves with signals found.
         """
         opts = {
-            'url': f'/users/current/subscribers/{self._accountId}/signals',
+            'url': f'/users/current/subscribers/{self._account_id}/signals',
             'method': 'GET',
-            'headers': {
-                'auth-token': self._domainClient.token
-            }
+            'headers': {'auth-token': self._domain_client.token},
         }
-        result = await self._domainClient.request_signal(opts, self._host, self._accountId)
+        result = await self._domain_client.request_signal(opts, self._host, self._account_id)
         convert_iso_time_to_date(result)
         return result
 
     async def get_strategy_external_signals(self, strategy_id: str) -> 'List[CopyFactoryExternalSignal]':
         """Returns active external signals of a strategy. Requires access to
         copyfactory-api:rest:public:external-signals:getSignals method which is included into reader role.
         Requires access to strategy, account resources.
@@ -58,19 +61,17 @@
 
         Returns:
             A coroutine which resolves with external signals found.
         """
         opts = {
             'url': f'/users/current/strategies/{strategy_id}/external-signals',
             'method': 'GET',
-            'headers': {
-                'auth-token': self._domainClient.token
-            }
+            'headers': {'auth-token': self._domain_client.token},
         }
-        result = await self._domainClient.request_signal(opts, self._host, self._accountId)
+        result = await self._domain_client.request_signal(opts, self._host, self._account_id)
         convert_iso_time_to_date(result)
         return result
 
     async def update_external_signal(self, strategy_id: str, signal_id: str, signal: CopyFactoryExternalSignalUpdate):
         """Updates external signal for a strategy. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/updateExternalSignal/
 
@@ -83,20 +84,18 @@
             A coroutine which resolves when external signal is updated.
         """
         payload: dict = deepcopy(signal)
         format_request(payload)
         opts = {
             'url': f"/users/current/strategies/{strategy_id}/external-signals/{signal_id}",
             'method': 'PUT',
-            'headers': {
-                'auth-token': self._domainClient.token
-            },
-            'body': payload
+            'headers': {'auth-token': self._domain_client.token},
+            'body': payload,
         }
-        return await self._domainClient.request_signal(opts, self._host, self._accountId)
+        return await self._domain_client.request_signal(opts, self._host, self._account_id)
 
     async def remove_external_signal(self, strategy_id: str, signal_id: str, signal: CopyFactoryExternalSignalRemove):
         """Removes (closes) external signal for a strategy. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/removeExternalSignal/
 
         Args:
             strategy_id: Strategy id.
@@ -107,13 +106,11 @@
             A coroutine which resolves when external signal is removed.
         """
         payload: dict = deepcopy(signal)
         format_request(payload)
         opts = {
             'url': f"/users/current/strategies/{strategy_id}/external-signals/{signal_id}/remove",
             'method': 'POST',
-            'headers': {
-                'auth-token': self._domainClient.token
-            },
-            'body': payload
+            'headers': {'auth-token': self._domain_client.token},
+            'body': payload,
         }
-        return await self._domainClient.request_signal(opts, self._host, self._accountId)
+        return await self._domain_client.request_signal(opts, self._host, self._account_id)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/signal_client_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/signal_client_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from .signal_client import SignalClient
 import pytest
-from ...models import date
 from mock import MagicMock, AsyncMock
+
+from .signal_client import SignalClient
+from ...models import date
+
 domain_client = MagicMock()
 token = 'header.payload.sign'
-host = {
-    'host': 'https://copyfactory-api-v1',
-    'region': 'vint-hill',
-    'domain': 'agiliumtrade.ai'
-}
+host = {'host': 'https://copyfactory-api-v1', 'region': 'vint-hill', 'domain': 'agiliumtrade.ai'}
 signal_client = SignalClient('accountId', host, domain_client)
 
 
 @pytest.fixture(autouse=True)
 async def run_around_tests():
     global domain_client
     domain_client = MagicMock()
@@ -32,84 +30,92 @@
     async def test_update_external_signal(self):
         """Should update external signal."""
         signal = {
             'symbol': 'EURUSD',
             'type': 'POSITION_TYPE_BUY',
             'time': date('2020-08-24T00:00:00.000Z'),
             'updateTime': date('2020-08-24T00:00:00.000Z'),
-            'volume': 1
+            'volume': 1,
         }
         expected_signal = {
             'symbol': 'EURUSD',
             'type': 'POSITION_TYPE_BUY',
             'time': '2020-08-24T00:00:00.000Z',
             'updateTime': '2020-08-24T00:00:00.000Z',
-            'volume': 1
+            'volume': 1,
         }
 
         await signal_client.update_external_signal('ABCD', '0123456', signal)
-        domain_client.request_signal.assert_called_with({
-            'url': '/users/current/strategies/ABCD/external-signals/0123456',
-            'method': 'PUT',
-            'headers': {
-                'auth-token': token
+        domain_client.request_signal.assert_called_with(
+            {
+                'url': '/users/current/strategies/ABCD/external-signals/0123456',
+                'method': 'PUT',
+                'headers': {'auth-token': token},
+                'body': expected_signal,
             },
-            'body': expected_signal
-        }, host, 'accountId')
+            host,
+            'accountId',
+        )
 
     @pytest.mark.asyncio
     async def test_remove_external_signal(self):
         """Should remove external signal."""
         signal = {'time': '2020-08-24T00:00:00.000Z'}
         await signal_client.remove_external_signal('ABCD', '0123456', signal)
-        domain_client.request_signal.assert_called_with({
-              'url': '/users/current/strategies/ABCD/external-signals/0123456/remove',
-              'method': 'POST',
-              'headers': {
-                'auth-token': token
-              },
-              'body': signal
-        }, host, 'accountId')
+        domain_client.request_signal.assert_called_with(
+            {
+                'url': '/users/current/strategies/ABCD/external-signals/0123456/remove',
+                'method': 'POST',
+                'headers': {'auth-token': token},
+                'body': signal,
+            },
+            host,
+            'accountId',
+        )
 
     @pytest.mark.asyncio
     async def test_retrieve_signals(self):
         """Should retrieve signals."""
-        expected = [{
-            'symbol': 'EURUSD',
-            'type': 'POSITION_TYPE_BUY',
-            'time': '2020-08-24T00:00:00.000Z',
-            'closeAfter': '2020-08-24T00:00:00.000Z',
-            'volume': 1
-        }]
+        expected = [
+            {
+                'symbol': 'EURUSD',
+                'type': 'POSITION_TYPE_BUY',
+                'time': '2020-08-24T00:00:00.000Z',
+                'closeAfter': '2020-08-24T00:00:00.000Z',
+                'volume': 1,
+            }
+        ]
 
         domain_client.request_signal = AsyncMock(return_value=expected)
         stopouts = await signal_client.get_trading_signals()
         assert stopouts == expected
-        domain_client.request_signal.assert_called_with({
-            'url': '/users/current/subscribers/accountId/signals',
-            'method': 'GET',
-            'headers': {
-                'auth-token': token
-            },
-        }, host, 'accountId')
+        domain_client.request_signal.assert_called_with(
+            {'url': '/users/current/subscribers/accountId/signals', 'method': 'GET', 'headers': {'auth-token': token}},
+            host,
+            'accountId',
+        )
 
     @pytest.mark.asyncio
     async def test_retrieve_external_signals(self):
         """Should retrieve strategy external signals."""
-        expected = [{
-            'id': '1',
-            'symbol': 'EURUSD',
-            'type': 'POSITION_TYPE_BUY',
-            'time': '2020-08-24T00:00:00.000Z',
-            'volume': 1
-        }]
+        expected = [
+            {
+                'id': '1',
+                'symbol': 'EURUSD',
+                'type': 'POSITION_TYPE_BUY',
+                'time': '2020-08-24T00:00:00.000Z',
+                'volume': 1,
+            }
+        ]
 
         domain_client.request_signal = AsyncMock(return_value=expected)
         signals = await signal_client.get_strategy_external_signals('ABCD')
         assert signals == expected
-        domain_client.request_signal.assert_called_with({
-            'url': '/users/current/strategies/ABCD/external-signals',
-            'method': 'GET',
-            'headers': {
-                'auth-token': token
+        domain_client.request_signal.assert_called_with(
+            {
+                'url': '/users/current/strategies/ABCD/external-signals',
+                'method': 'GET',
+                'headers': {'auth-token': token},
             },
-        }, host, 'accountId')
+            host,
+            'accountId',
+        )
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/stopoutListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/stopout_listener.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import abstractmethod
-from ..copyFactory_models import CopyFactoryStrategyStopout
 from typing import List
 
+from ..copyfactory_models import CopyFactoryStrategyStopout
+
 
 class StopoutListener:
     """Stopout listener for handling a stream of stopout events."""
 
     @abstractmethod
     async def on_stopout(self, strategy_stopout_event: List[CopyFactoryStrategyStopout]):
         """Calls a predefined function with the packets data.
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/stopout_listener_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,90 +1,101 @@
-from ...metaApi_client import MetaApiClient
+import asyncio
+
+import math
+
+from .stopout_listener import StopoutListener
 from ...domain_client import DomainClient
-from ....models import random_id
-from .stopoutListener import StopoutListener
+from ...metaapi_client import MetaApiClient
 from ....logger import LoggerManager
-import math
-import asyncio
+from ....models import random_id
 
 
 class StopoutListenerManager(MetaApiClient):
     """Stopout event listener manager."""
 
     def __init__(self, domain_client: DomainClient):
-        """Inits stopout listener manager instance.
+        """Initializes stopout listener manager instance.
 
         Args:
             domain_client: Domain client.
         """
         super().__init__(domain_client)
-        self._domainClient = domain_client
-        self._stopoutListeners = {}
-        self._errorThrottleTime = 1
+        self._domain_client = domain_client
+        self._stopout_listeners = {}
+        self._error_throttle_time = 1
         self._logger = LoggerManager.get_logger('StopoutListenerManager')
 
     @property
     def stopout_listeners(self):
         """Returns the dictionary of stopout listeners.
 
         Returns:
             Dictionary of stopout listeners.
         """
-        return self._stopoutListeners
+        return self._stopout_listeners
 
-    def add_stopout_listener(self, listener: StopoutListener, account_id: str = None, strategy_id: str = None,
-                             sequence_number: int = None) -> str:
+    def add_stopout_listener(
+        self, listener: StopoutListener, account_id: str = None, strategy_id: str = None, sequence_number: int = None
+    ) -> str:
         """Adds a stopout listener.
 
         Args:
             listener: Stopout listener.
             account_id:  Account id.
             strategy_id: Strategy id.
             sequence_number: Event sequence number.
 
         Returns:
             Stopout listener id.
         """
         listener_id = random_id(10)
-        self._stopoutListeners[listener_id] = listener
-        asyncio.create_task(self._start_stopout_event_job(listener_id, listener, account_id, strategy_id,
-                                                          sequence_number))
+        self._stopout_listeners[listener_id] = listener
+        asyncio.create_task(
+            self._start_stopout_event_job(listener_id, listener, account_id, strategy_id, sequence_number)
+        )
         return listener_id
 
     def remove_stopout_listener(self, listener_id: str):
         """Removes stopout listener by id.
 
         Args:
             listener_id: listener id.
         """
-        if listener_id in self._stopoutListeners:
-            del self._stopoutListeners[listener_id]
+        if listener_id in self._stopout_listeners:
+            del self._stopout_listeners[listener_id]
 
-    async def _start_stopout_event_job(self, listener_id: str, listener: StopoutListener, account_id: str = None,
-                                       strategy_id: str = None, sequence_number: int = None):
-        throttle_time = self._errorThrottleTime
-        while listener_id in self._stopoutListeners:
+    async def _start_stopout_event_job(
+        self,
+        listener_id: str,
+        listener: StopoutListener,
+        account_id: str = None,
+        strategy_id: str = None,
+        sequence_number: int = None,
+    ):
+        throttle_time = self._error_throttle_time
+        while listener_id in self._stopout_listeners:
             opts = {
                 'url': '/users/current/stopouts/stream',
                 'method': 'GET',
                 'params': {
                     'previousSequenceNumber': sequence_number,
                     'subscriberId': account_id,
                     'strategyId': strategy_id,
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': self._token
+                    'limit': 1000,
                 },
+                'headers': {'auth-token': self._token},
             }
             try:
-                packets = await self._domainClient.request_copyfactory(opts, True)
+                packets = await self._domain_client.request_copyfactory(opts, True)
                 await listener.on_stopout(packets)
-                throttle_time = self._errorThrottleTime
-                if listener_id in self._stopoutListeners and len(packets):
+                throttle_time = self._error_throttle_time
+                if listener_id in self._stopout_listeners and len(packets):
                     sequence_number = packets[-1]['sequenceNumber']
             except Exception as err:
                 await listener.on_error(err)
-                self._logger.error(f'Failed to retrieve stopouts stream for strategy {strategy_id}, ' +
-                                   f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds', err)
+                self._logger.error(
+                    f'Failed to retrieve stopouts stream for strategy {strategy_id}, '
+                    + f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds',
+                    err,
+                )
                 await asyncio.sleep(throttle_time)
                 throttle_time = min(throttle_time * 2, 30)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/stopoutListenerManager_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/stopout_listener_manager_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,55 @@
-from ....models import date
-from .stopoutListenerManager import StopoutListenerManager
-from .stopoutListener import StopoutListener
-from ...domain_client import DomainClient
-from mock import MagicMock, patch, AsyncMock
 from asyncio import sleep
+
 import pytest
+from mock import MagicMock, patch, AsyncMock
+
+from .stopout_listener import StopoutListener
+from .stopout_listener_manager import StopoutListenerManager
+from ...domain_client import DomainClient
+from ....models import date
 
 token = 'header.payload.sign'
 expected = [
     {
         'subscriberId': 'accountId',
         'reason': 'monthly-balance',
         'stoppedAt': date('2020-08-08T07:57:30.328Z'),
-        'strategy': {
-            'id': 'ABCD',
-            'name': 'Strategy'
-        },
+        'strategy': {'id': 'ABCD', 'name': 'Strategy'},
         'reasonDescription': 'total strategy equity drawdown exceeded limit',
-        'sequenceNumber': 2
+        'sequenceNumber': 2,
     },
     {
         'subscriberId': 'accountId',
         'reason': 'monthly-balance',
         'stoppedAt': date('2020-08-08T07:57:31.328Z'),
-        'strategy': {
-            'id': 'ABCD',
-            'name': 'Strategy'
-        },
+        'strategy': {'id': 'ABCD', 'name': 'Strategy'},
         'reasonDescription': 'total strategy equity drawdown exceeded limit',
-        'sequenceNumber': 3
-    }]
+        'sequenceNumber': 3,
+    },
+]
 
 expected2 = [
     {
         'subscriberId': 'accountId',
         'reason': 'monthly-balance',
         'stoppedAt': date('2020-08-08T07:57:32.328Z'),
-        'strategy': {
-            'id': 'ABCD',
-            'name': 'Strategy'
-        },
+        'strategy': {'id': 'ABCD', 'name': 'Strategy'},
         'reasonDescription': 'total strategy equity drawdown exceeded limit',
-        'sequenceNumber': 4
+        'sequenceNumber': 4,
     },
     {
         'subscriberId': 'accountId',
         'reason': 'monthly-balance',
         'stoppedAt': date('2020-08-08T07:57:33.328Z'),
-        'strategy': {
-            'id': 'ABCD',
-            'name': 'Strategy'
-        },
+        'strategy': {'id': 'ABCD', 'name': 'Strategy'},
         'reasonDescription': 'total strategy equity drawdown exceeded limit',
-        'sequenceNumber': 5
-    }]
+        'sequenceNumber': 5,
+    },
+]
 domain_client = DomainClient(MagicMock(), token)
 stopout_listener_manager = StopoutListenerManager(domain_client)
 call_stub = MagicMock()
 error_stub = MagicMock()
 listener = StopoutListener()
 
 
@@ -80,38 +72,24 @@
     global listener
     listener = Listener()
 
     async def get_stopout_func(arg, arg2):
         if arg == {
             'url': '/users/current/stopouts/stream',
             'method': 'GET',
-            'params': {
-                'previousSequenceNumber': 1,
-                'subscriberId': 'accountId',
-                'strategyId': 'ABCD',
-                'limit': 1000
-            },
-            'headers': {
-                'auth-token': token
-            },
+            'params': {'previousSequenceNumber': 1, 'subscriberId': 'accountId', 'strategyId': 'ABCD', 'limit': 1000},
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected
         elif arg == {
             'url': '/users/current/stopouts/stream',
             'method': 'GET',
-            'params': {
-                'previousSequenceNumber': 3,
-                'subscriberId': 'accountId',
-                'strategyId': 'ABCD',
-                'limit': 1000
-            },
-            'headers': {
-                'auth-token': token
-            },
+            'params': {'previousSequenceNumber': 3, 'subscriberId': 'accountId', 'strategyId': 'ABCD', 'limit': 1000},
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected2
         else:
             await sleep(0.1)
             return []
 
@@ -119,27 +97,29 @@
     domain_client.request_copyfactory = get_stopout_mock
 
 
 class TestStopoutListenerManager:
     @pytest.mark.asyncio
     async def test_add_stopout_listener(self):
         """Should add stopout listener."""
-        with patch('lib.clients.copyFactory.streaming.stopoutListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.stopout_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = stopout_listener_manager.add_stopout_listener(listener, 'accountId', 'ABCD', 1)
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             call_stub.assert_any_call(expected2)
             stopout_listener_manager.remove_stopout_listener(id)
 
     @pytest.mark.asyncio
     async def test_remove_stopout_listener(self):
         """Should remove stopout listener."""
-        with patch('lib.clients.copyFactory.streaming.stopoutListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.stopout_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = stopout_listener_manager.add_stopout_listener(listener, 'accountId', 'ABCD', 1)
             await sleep(0.08)
             stopout_listener_manager.remove_stopout_listener(id)
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             assert call_stub.call_count == 1
 
@@ -161,30 +141,29 @@
             if arg == {
                 'url': '/users/current/stopouts/stream',
                 'method': 'GET',
                 'params': {
                     'previousSequenceNumber': 1,
                     'subscriberId': 'accountId',
                     'strategyId': 'ABCD',
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': token
+                    'limit': 1000,
                 },
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.05)
                 return expected
             else:
                 await sleep(0.5)
                 return []
 
         get_stopout_mock = AsyncMock(side_effect=get_stopout_func)
         domain_client.request_copyfactory = get_stopout_mock
-        with patch('lib.clients.copyFactory.streaming.stopoutListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.stopout_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = stopout_listener_manager.add_stopout_listener(listener, 'accountId', 'ABCD', 1)
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             assert error_stub.call_count == 1
             error_stub.assert_any_call(error)
             await sleep(0.06)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/transactionListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/transaction_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import abstractmethod
-from ..copyFactory_models import CopyFactoryTransaction
 from typing import List
 
+from ..copyfactory_models import CopyFactoryTransaction
+
 
 class TransactionListener:
     """Transaction listener for handling a stream of transaction events."""
 
     @abstractmethod
     async def on_transaction(self, transaction_event: List[CopyFactoryTransaction]):
         """Calls a predefined function with the packets data.
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/transactionListenerManager.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/transaction_listener_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,166 +1,170 @@
-from ...metaApi_client import MetaApiClient
-from ...domain_client import DomainClient
-from ....models import random_id, format_date, date
-from ...errorHandler import NotFoundException
-from .transactionListener import TransactionListener
+import asyncio
 from datetime import datetime, timedelta
-from ....logger import LoggerManager
+
 import math
-import asyncio
+
+from .transaction_listener import TransactionListener
+from ...domain_client import DomainClient
+from ...error_handler import NotFoundException
+from ...metaapi_client import MetaApiClient
+from ....logger import LoggerManager
+from ....models import random_id, format_date, date
 
 
 class TransactionListenerManager(MetaApiClient):
     """Transaction listener manager."""
 
     def __init__(self, domain_client: DomainClient):
-        """Inits transaction listener manager instance.
+        """Initializes transaction listener manager instance.
 
         Args:
             domain_client: Domain client.
         """
         super().__init__(domain_client)
-        self._domainClient = domain_client
-        self._strategyTransactionListeners = {}
-        self._subscriberTransactionListeners = {}
-        self._errorThrottleTime = 1
+        self._domain_client = domain_client
+        self._strategy_transaction_listeners = {}
+        self._subscriber_transaction_listeners = {}
+        self._error_throttle_time = 1
         self._logger = LoggerManager.get_logger('TransactionListenerManager')
 
     @property
     def strategy_transaction_listeners(self):
         """Returns the dictionary of strategy transaction listeners.
 
         Returns:
             Dictionary of strategy transaction listeners.
         """
-        return self._strategyTransactionListeners
+        return self._strategy_transaction_listeners
 
     @property
     def subscriber_transaction_listeners(self):
         """Returns the dictionary of subscriber transaction listeners.
 
         Returns:
             Dictionary of subscriber transaction listeners.
         """
-        return self._subscriberTransactionListeners
+        return self._subscriber_transaction_listeners
 
-    def add_strategy_transaction_listener(self, listener: TransactionListener, strategy_id: str,
-                                          start_time: datetime = None):
+    def add_strategy_transaction_listener(
+        self, listener: TransactionListener, strategy_id: str, start_time: datetime = None
+    ):
         """Adds a strategy transaction listener.
 
         Args:
             listener: User transaction listener.
             strategy_id: Strategy id.
             start_time: Transaction search start time.
 
         Returns:
             Strategy transaction listener id.
         """
         listener_id = random_id(10)
-        self._strategyTransactionListeners[listener_id] = listener
-        asyncio.create_task(self._start_strategy_transaction_stream_job(listener_id, listener, strategy_id,
-                                                                        start_time))
+        self._strategy_transaction_listeners[listener_id] = listener
+        asyncio.create_task(self._start_strategy_transaction_stream_job(listener_id, listener, strategy_id, start_time))
         return listener_id
 
-    def add_subscriber_transaction_listener(self, listener: TransactionListener, subscriber_id: str,
-                                            start_time: datetime = None):
+    def add_subscriber_transaction_listener(
+        self, listener: TransactionListener, subscriber_id: str, start_time: datetime = None
+    ):
         """Adds a subscriber transaction listener.
 
         Args:
             listener: User transaction listener.
             subscriber_id: Subscriber id.
             start_time: Transaction search start time.
 
         Returns:
             Subscriber transaction listener id.
         """
         listener_id = random_id(10)
-        self._subscriberTransactionListeners[listener_id] = listener
-        asyncio.create_task(self._start_subscriber_transaction_stream_job(listener_id, listener, subscriber_id,
-                                                                          start_time))
+        self._subscriber_transaction_listeners[listener_id] = listener
+        asyncio.create_task(
+            self._start_subscriber_transaction_stream_job(listener_id, listener, subscriber_id, start_time)
+        )
         return listener_id
 
     def remove_strategy_transaction_listener(self, listener_id: str):
         """Removes strategy transaction listener by id.
 
         Args:
             listener_id: Listener id.
         """
-        if listener_id in self._strategyTransactionListeners:
-            del self._strategyTransactionListeners[listener_id]
+        if listener_id in self._strategy_transaction_listeners:
+            del self._strategy_transaction_listeners[listener_id]
 
     def remove_subscriber_transaction_listener(self, listener_id: str):
         """Removes subscriber transaction listener by id.
 
         Args:
             listener_id: Listener id.
         """
-        if listener_id in self._subscriberTransactionListeners:
-            del self._subscriberTransactionListeners[listener_id]
+        if listener_id in self._subscriber_transaction_listeners:
+            del self._subscriber_transaction_listeners[listener_id]
 
-    async def _start_strategy_transaction_stream_job(self, listener_id: str, listener: TransactionListener,
-                                                     strategy_id: str, start_time: datetime = None):
-        throttle_time = self._errorThrottleTime
-        while listener_id in self._strategyTransactionListeners:
+    async def _start_strategy_transaction_stream_job(
+        self, listener_id: str, listener: TransactionListener, strategy_id: str, start_time: datetime = None
+    ):
+        throttle_time = self._error_throttle_time
+        while listener_id in self._strategy_transaction_listeners:
             opts = {
                 'url': f'/users/current/strategies/{strategy_id}/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': self._token
-                }
+                'params': {'limit': 1000},
+                'headers': {'auth-token': self._token},
             }
             if start_time:
                 opts['params']['startTime'] = format_date(start_time)
             try:
-                packets = await self._domainClient.request_copyfactory(opts, True)
+                packets = await self._domain_client.request_copyfactory(opts, True)
                 await listener.on_transaction(packets)
-                throttle_time = self._errorThrottleTime
-                if listener_id in self._strategyTransactionListeners and len(packets):
+                throttle_time = self._error_throttle_time
+                if listener_id in self._strategy_transaction_listeners and len(packets):
                     start_time = date(packets[0]['time']) + timedelta(milliseconds=1)
             except NotFoundException as err:
                 await listener.on_error(err)
                 self._logger.error(f'Strategy {strategy_id} not found, removing listener f{listener_id}')
-                if listener_id in self._strategyTransactionListeners:
-                    del self._strategyTransactionListeners[listener_id]
+                if listener_id in self._strategy_transaction_listeners:
+                    del self._strategy_transaction_listeners[listener_id]
             except Exception as err:
                 await listener.on_error(err)
-                self._logger.error(f'Failed to retrieve transactions stream for strategy {strategy_id}, ' +
-                                   f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds', err)
+                self._logger.error(
+                    f'Failed to retrieve transactions stream for strategy {strategy_id}, '
+                    + f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds',
+                    err,
+                )
                 await asyncio.sleep(throttle_time)
                 throttle_time = min(throttle_time * 2, 30)
 
-    async def _start_subscriber_transaction_stream_job(self, listener_id: str, listener: TransactionListener,
-                                                       subscriber_id: str, start_time: datetime = None):
-        throttle_time = self._errorThrottleTime
-        while listener_id in self._subscriberTransactionListeners:
+    async def _start_subscriber_transaction_stream_job(
+        self, listener_id: str, listener: TransactionListener, subscriber_id: str, start_time: datetime = None
+    ):
+        throttle_time = self._error_throttle_time
+        while listener_id in self._subscriber_transaction_listeners:
             opts = {
                 'url': f'/users/current/subscribers/{subscriber_id}/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': self._token
-                }
+                'params': {'limit': 1000},
+                'headers': {'auth-token': self._token},
             }
             if start_time:
                 opts['params']['startTime'] = format_date(start_time)
             try:
-                packets = await self._domainClient.request_copyfactory(opts, True)
+                packets = await self._domain_client.request_copyfactory(opts, True)
                 await listener.on_transaction(packets)
-                throttle_time = self._errorThrottleTime
-                if listener_id in self._subscriberTransactionListeners and len(packets):
+                throttle_time = self._error_throttle_time
+                if listener_id in self._subscriber_transaction_listeners and len(packets):
                     start_time = date(packets[0]['time']) + timedelta(milliseconds=1)
             except NotFoundException as err:
                 await listener.on_error(err)
                 self._logger.error(f'Subscriber {subscriber_id} not found, removing listener f{listener_id}')
-                if listener_id in self._subscriberTransactionListeners:
-                    del self._subscriberTransactionListeners[listener_id]
+                if listener_id in self._subscriber_transaction_listeners:
+                    del self._subscriber_transaction_listeners[listener_id]
             except Exception as err:
                 await listener.on_error(err)
-                self._logger.error(f'Failed to retrieve transactions stream for subscriber {subscriber_id}, ' +
-                                   f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds', err)
+                self._logger.error(
+                    f'Failed to retrieve transactions stream for subscriber {subscriber_id}, '
+                    + f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds',
+                    err,
+                )
                 await asyncio.sleep(throttle_time)
                 throttle_time = min(throttle_time * 2, 30)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/transactionListenerManager_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/transaction_listener_manager_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-from ....models import date
-from .transactionListenerManager import TransactionListenerManager
-from .transactionListener import TransactionListener
-from ...domain_client import DomainClient
-from ..copyFactory_models import CopyFactoryTransaction
-from ...errorHandler import NotFoundException
-from mock import MagicMock, patch, AsyncMock
 from asyncio import sleep
 from typing import List
+
 import pytest
+from mock import MagicMock, patch, AsyncMock
+
+from .transaction_listener import TransactionListener
+from .transaction_listener_manager import TransactionListenerManager
+from ..copyfactory_models import CopyFactoryTransaction
+from ...domain_client import DomainClient
+from ...error_handler import NotFoundException
+from ....models import date
 
 token = 'header.payload.sign'
-expected = [{
-    'id': '64664661:close',
-    'type': 'DEAL_TYPE_SELL',
-    'time': '2020-08-08T08:57:30.328Z'
-}, {
-    'id': '64664660:close',
-    'type': 'DEAL_TYPE_SELL',
-    'time': '2020-08-08T07:57:30.328Z'
-}]
-
-expected2 = [{
-    'id': '64664663:close',
-    'type': 'DEAL_TYPE_SELL',
-    'time': '2020-08-08T10:57:30.328Z'
-}, {
-    'id': '64664662:close',
-    'type': 'DEAL_TYPE_SELL',
-    'time': '2020-08-08T09:57:30.328Z'
-}]
+expected = [
+    {'id': '64664661:close', 'type': 'DEAL_TYPE_SELL', 'time': '2020-08-08T08:57:30.328Z'},
+    {'id': '64664660:close', 'type': 'DEAL_TYPE_SELL', 'time': '2020-08-08T07:57:30.328Z'},
+]
+
+expected2 = [
+    {'id': '64664663:close', 'type': 'DEAL_TYPE_SELL', 'time': '2020-08-08T10:57:30.328Z'},
+    {'id': '64664662:close', 'type': 'DEAL_TYPE_SELL', 'time': '2020-08-08T09:57:30.328Z'},
+]
 domain_client = DomainClient(MagicMock(), token)
 transaction_listener_manager = TransactionListenerManager(domain_client)
 call_stub = MagicMock()
 error_stub = MagicMock()
 listener = TransactionListener()
 
 
@@ -60,64 +52,58 @@
 
 @pytest.fixture()
 async def prepare_strategy_transactions():
     async def get_transactions_func(arg, arg2):
         if arg == {
             'url': '/users/current/strategies/ABCD/transactions/stream',
             'method': 'GET',
-            'params': {
-                'startTime': '2020-08-08T00:00:00.000Z',
-                'limit': 1000
-            },
-            'headers': {
-                'auth-token': token
-            },
+            'params': {'startTime': '2020-08-08T00:00:00.000Z', 'limit': 1000},
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected
         elif arg == {
             'url': '/users/current/strategies/ABCD/transactions/stream',
             'method': 'GET',
-            'params': {
-                'startTime': '2020-08-08T08:57:30.329Z',
-                'limit': 1000
-            },
-            'headers': {
-                'auth-token': token
-            },
+            'params': {'startTime': '2020-08-08T08:57:30.329Z', 'limit': 1000},
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected2
         else:
             await sleep(0.1)
             return []
 
     domain_client.request_copyfactory = AsyncMock(side_effect=get_transactions_func)
 
 
 class TestStrategyTransactions:
     @pytest.mark.asyncio
     async def test_add_strategy_listener(self, prepare_strategy_transactions):
         """Should add listener."""
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_strategy_transaction_listener(listener, 'ABCD',
-                                                                                date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_strategy_transaction_listener(
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             call_stub.assert_any_call(expected2)
             transaction_listener_manager.remove_strategy_transaction_listener(id)
 
     @pytest.mark.asyncio
     async def test_remove_strategy_listener(self, prepare_strategy_transactions):
         """Should remove listener."""
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_strategy_transaction_listener(listener, 'ABCD',
-                                                                                date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_strategy_transaction_listener(
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.08)
             transaction_listener_manager.remove_strategy_transaction_listener(id)
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             assert call_stub.call_count == 1
 
     @pytest.mark.asyncio
@@ -134,33 +120,30 @@
                 raise error
             if call_count == 2:
                 raise error2
 
             if arg == {
                 'url': '/users/current/strategies/ABCD/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'startTime': '2020-08-08T00:00:00.000Z',
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': token
-                },
+                'params': {'startTime': '2020-08-08T00:00:00.000Z', 'limit': 1000},
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.05)
                 return expected
             else:
                 await sleep(0.5)
                 return []
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_transaction_func)
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_strategy_transaction_listener(listener, 'ABCD',
-                                                                                date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_strategy_transaction_listener(
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             assert error_stub.call_count == 1
             error_stub.assert_any_call(error)
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
@@ -179,43 +162,35 @@
         """Should remove listener on not found error."""
         error = NotFoundException('test')
 
         async def get_transactions_func(arg, arg2):
             if arg == {
                 'url': '/users/current/strategies/ABCD/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'startTime': '2020-08-08T00:00:00.000Z',
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': token
-                },
+                'params': {'startTime': '2020-08-08T00:00:00.000Z', 'limit': 1000},
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 return expected
             elif arg == {
                 'url': '/users/current/strategies/ABCD/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'startTime': '2020-08-08T08:57:30.329Z',
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': token
-                },
+                'params': {'startTime': '2020-08-08T08:57:30.329Z', 'limit': 1000},
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 raise error
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_transactions_func)
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_strategy_transaction_listener(listener, 'ABCD',
-                                                                                date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_strategy_transaction_listener(
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
             assert call_stub.call_count == 1
             await sleep(0.2)
@@ -230,64 +205,58 @@
 
 @pytest.fixture()
 async def prepare_subscriber_transactions():
     async def get_transactions_func(arg, arg2):
         if arg == {
             'url': '/users/current/subscribers/accountId/transactions/stream',
             'method': 'GET',
-            'params': {
-                'startTime': '2020-08-08T00:00:00.000Z',
-                'limit': 1000
-            },
-            'headers': {
-                'auth-token': token
-            },
+            'params': {'startTime': '2020-08-08T00:00:00.000Z', 'limit': 1000},
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected
         elif arg == {
             'url': '/users/current/subscribers/accountId/transactions/stream',
             'method': 'GET',
-            'params': {
-                'startTime': '2020-08-08T08:57:30.329Z',
-                'limit': 1000
-            },
-            'headers': {
-                'auth-token': token
-            },
+            'params': {'startTime': '2020-08-08T08:57:30.329Z', 'limit': 1000},
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected2
         else:
             await sleep(0.1)
             return []
 
     domain_client.request_copyfactory = AsyncMock(side_effect=get_transactions_func)
 
 
 class TestSubscriberTransactions:
     @pytest.mark.asyncio
     async def test_add_subscriber_listener(self, prepare_subscriber_transactions):
         """Should add listener."""
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_subscriber_transaction_listener(listener, 'accountId',
-                                                                                  date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_subscriber_transaction_listener(
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             call_stub.assert_any_call(expected2)
             transaction_listener_manager.remove_subscriber_transaction_listener(id)
 
     @pytest.mark.asyncio
     async def test_remove_strategy_listener(self, prepare_subscriber_transactions):
         """Should remove listener."""
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_subscriber_transaction_listener(listener, 'accountId',
-                                                                                  date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_subscriber_transaction_listener(
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.08)
             transaction_listener_manager.remove_subscriber_transaction_listener(id)
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             assert call_stub.call_count == 1
 
     @pytest.mark.asyncio
@@ -304,33 +273,30 @@
                 raise error
             if call_count == 2:
                 raise error2
 
             if arg == {
                 'url': '/users/current/subscribers/accountId/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'startTime': '2020-08-08T00:00:00.000Z',
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': token
-                },
+                'params': {'startTime': '2020-08-08T00:00:00.000Z', 'limit': 1000},
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.05)
                 return expected
             else:
                 await sleep(0.5)
                 return []
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_transaction_func)
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_subscriber_transaction_listener(listener, 'accountId',
-                                                                                  date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_subscriber_transaction_listener(
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             assert error_stub.call_count == 1
             error_stub.assert_any_call(error)
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
@@ -349,43 +315,35 @@
         """Should remove listener on not found error."""
         error = NotFoundException('test')
 
         async def get_transactions_func(arg, arg2):
             if arg == {
                 'url': '/users/current/subscribers/accountId/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'startTime': '2020-08-08T00:00:00.000Z',
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': token
-                },
+                'params': {'startTime': '2020-08-08T00:00:00.000Z', 'limit': 1000},
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 return expected
             elif arg == {
                 'url': '/users/current/subscribers/accountId/transactions/stream',
                 'method': 'GET',
-                'params': {
-                    'startTime': '2020-08-08T08:57:30.329Z',
-                    'limit': 1000
-                },
-                'headers': {
-                    'auth-token': token
-                },
+                'params': {'startTime': '2020-08-08T08:57:30.329Z', 'limit': 1000},
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 raise error
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_transactions_func)
-        with patch('lib.clients.copyFactory.streaming.transactionListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
-            id = transaction_listener_manager.add_subscriber_transaction_listener(listener, 'accountId',
-                                                                                  date('2020-08-08T00:00:00.000Z'))
+        with patch(
+            'lib.clients.copyfactory.streaming.transaction_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
+            id = transaction_listener_manager.add_subscriber_transaction_listener(
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z')
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
             assert call_stub.call_count == 1
             await sleep(0.2)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/userLogListener.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/user_log_listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from abc import abstractmethod
-from ..copyFactory_models import CopyFactoryUserLogMessage
 from typing import List
 
+from ..copyfactory_models import CopyFactoryUserLogMessage
+
 
 class UserLogListener:
     """User log listener for handling a stream of transaction events."""
 
     @abstractmethod
     async def on_user_log(self, log_event: List[CopyFactoryUserLogMessage]):
         """Calls a predefined function with the packets data.
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/userLogListenerManager.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/user_log_listener_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,96 @@
-from ...metaApi_client import MetaApiClient
-from ...domain_client import DomainClient
-from ....models import random_id, format_date, date
-from ...errorHandler import NotFoundException
-from .userLogListener import UserLogListener
-from ..copyFactory_models import LogLevel
-from datetime import datetime, timedelta
-from ....logger import LoggerManager
 import asyncio
+from datetime import datetime, timedelta
+
 import math
 
+from .user_log_listener import UserLogListener
+from ..copyfactory_models import LogLevel
+from ...domain_client import DomainClient
+from ...error_handler import NotFoundException
+from ...metaapi_client import MetaApiClient
+from ....logger import LoggerManager
+from ....models import random_id, format_date, date
+
 
 class UserLogListenerManager(MetaApiClient):
     """User log listener manager."""
 
     def __init__(self, domain_client: DomainClient):
-        """Inits user log listener manager instance.
+        """Initializes user log listener manager instance.
 
         Args:
             domain_client: Domain client.
         """
         super().__init__(domain_client)
-        self._domainClient = domain_client
-        self._strategyLogListeners = {}
-        self._subscriberLogListeners = {}
-        self._errorThrottleTime = 1
+        self._domain_client = domain_client
+        self._strategy_log_listeners = {}
+        self._subscriber_log_listeners = {}
+        self._error_throttle_time = 1
         self._logger = LoggerManager.get_logger('UserLogListenerManager')
 
     @property
     def strategy_log_listeners(self):
         """Returns the dictionary of strategy log listeners.
 
         Returns:
             Dictionary of strategy log listeners.
         """
-        return self._strategyLogListeners
+        return self._strategy_log_listeners
 
     @property
     def subscriber_log_listeners(self):
         """Returns the dictionary of subscriber log listeners.
 
         Returns:
             Dictionary of subscriber log listeners.
         """
-        return self._subscriberLogListeners
+        return self._subscriber_log_listeners
 
-    def add_strategy_log_listener(self, listener: UserLogListener, strategy_id: str, start_time: datetime = None,
-                                  position_id: str = None, level: LogLevel = None, limit: int = None):
+    def add_strategy_log_listener(
+        self,
+        listener: UserLogListener,
+        strategy_id: str,
+        start_time: datetime = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        limit: int = None,
+    ):
         """Adds a strategy transaction listener.
 
         Args:
             listener: User transaction listener.
             strategy_id: Strategy id.
             start_time: Transaction search start time.
             position_id: Position id filter.
             level: Minimum severity level.
             limit: Log pagination limit.
 
         Returns:
             Strategy log listener id.
         """
         listener_id = random_id(10)
-        self._strategyLogListeners[listener_id] = listener
-        asyncio.create_task(self._start_strategy_log_stream_job(listener_id, listener, strategy_id, start_time,
-                                                                position_id, level, limit))
+        self._strategy_log_listeners[listener_id] = listener
+        asyncio.create_task(
+            self._start_strategy_log_stream_job(
+                listener_id, listener, strategy_id, start_time, position_id, level, limit
+            )
+        )
         return listener_id
 
-    def add_subscriber_log_listener(self, listener: UserLogListener, subscriber_id: str, start_time: datetime = None,
-                                    strategy_id: str = None, position_id: str = None, level: LogLevel = None,
-                                    limit: int = None):
+    def add_subscriber_log_listener(
+        self,
+        listener: UserLogListener,
+        subscriber_id: str,
+        start_time: datetime = None,
+        strategy_id: str = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        limit: int = None,
+    ):
         """Adds a subscriber transaction listener.
 
         Args:
             listener: User transaction listener.
             subscriber_id: Subscriber id.
             start_time: Transaction search start time.
             strategy_id: Strategy id filter.
@@ -79,115 +98,135 @@
             level: Minimum severity level.
             limit: Log pagination limit.
 
         Returns:
             Subscriber transaction listener id.
         """
         listener_id = random_id(10)
-        self._subscriberLogListeners[listener_id] = listener
-        asyncio.create_task(self._start_subscriber_log_stream_job(listener_id, listener, subscriber_id, start_time,
-                                                                  strategy_id, position_id, level, limit))
+        self._subscriber_log_listeners[listener_id] = listener
+        asyncio.create_task(
+            self._start_subscriber_log_stream_job(
+                listener_id, listener, subscriber_id, start_time, strategy_id, position_id, level, limit
+            )
+        )
         return listener_id
 
     def remove_strategy_log_listener(self, listener_id: str):
         """Removes strategy log listener by id.
 
         Args:
             listener_id: Listener id.
         """
-        if listener_id in self._strategyLogListeners:
-            del self._strategyLogListeners[listener_id]
+        if listener_id in self._strategy_log_listeners:
+            del self._strategy_log_listeners[listener_id]
 
     def remove_subscriber_log_listener(self, listener_id: str):
         """Removes subscriber transaction listener by id.
 
         Args:
             listener_id: Listener id.
         """
-        if listener_id in self._subscriberLogListeners:
-            del self._subscriberLogListeners[listener_id]
+        if listener_id in self._subscriber_log_listeners:
+            del self._subscriber_log_listeners[listener_id]
 
-    async def _start_strategy_log_stream_job(self, listener_id: str, listener: UserLogListener,
-                                             strategy_id: str, start_time: datetime = None, position_id: str = None,
-                                             level: LogLevel = None, limit: int = None):
-        throttle_time = self._errorThrottleTime
-        while listener_id in self._strategyLogListeners:
+    async def _start_strategy_log_stream_job(
+        self,
+        listener_id: str,
+        listener: UserLogListener,
+        strategy_id: str,
+        start_time: datetime = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        limit: int = None,
+    ):
+        throttle_time = self._error_throttle_time
+        while listener_id in self._strategy_log_listeners:
             opts = {
                 'url': f'/users/current/strategies/{strategy_id}/user-log/stream',
                 'method': 'GET',
                 'params': {},
-                'headers': {
-                    'auth-token': self._token
-                }
+                'headers': {'auth-token': self._token},
             }
             if start_time:
                 opts['params']['startTime'] = format_date(start_time)
             if position_id:
                 opts['params']['positionId'] = position_id
             if level:
                 opts['params']['level'] = level
             if limit:
                 opts['params']['limit'] = limit
             try:
-                packets = await self._domainClient.request_copyfactory(opts, True)
+                packets = await self._domain_client.request_copyfactory(opts, True)
                 # stop job if user has unsubscribed in time of new packets has been received
-                if listener_id not in self._strategyLogListeners:
+                if listener_id not in self._strategy_log_listeners:
                     return
                 await listener.on_user_log(packets)
-                throttle_time = self._errorThrottleTime
-                if listener_id in self._strategyLogListeners and len(packets):
+                throttle_time = self._error_throttle_time
+                if listener_id in self._strategy_log_listeners and len(packets):
                     start_time = date(packets[0]['time']) + timedelta(milliseconds=1)
             except NotFoundException as err:
                 await listener.on_error(err)
                 self._logger.error(f'Strategy {strategy_id} not found, removing listener f{listener_id}')
-                if listener_id in self._strategyLogListeners:
-                    del self._strategyLogListeners[listener_id]
+                if listener_id in self._strategy_log_listeners:
+                    del self._strategy_log_listeners[listener_id]
             except Exception as err:
                 await listener.on_error(err)
-                self._logger.error(f'Failed to retrieve user log stream for strategy {strategy_id}, ' +
-                                   f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds', err)
+                self._logger.error(
+                    f'Failed to retrieve user log stream for strategy {strategy_id}, '
+                    + f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds',
+                    err,
+                )
                 await asyncio.sleep(throttle_time)
                 throttle_time = min(throttle_time * 2, 30)
 
-    async def _start_subscriber_log_stream_job(self, listener_id: str, listener: UserLogListener, subscriber_id: str,
-                                               start_time: datetime = None, strategy_id: str = None,
-                                               position_id: str = None, level: LogLevel = None, limit: int = None):
-        throttle_time = self._errorThrottleTime
-        while listener_id in self._subscriberLogListeners:
+    async def _start_subscriber_log_stream_job(
+        self,
+        listener_id: str,
+        listener: UserLogListener,
+        subscriber_id: str,
+        start_time: datetime = None,
+        strategy_id: str = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        limit: int = None,
+    ):
+        throttle_time = self._error_throttle_time
+        while listener_id in self._subscriber_log_listeners:
             opts = {
                 'url': f'/users/current/subscribers/{subscriber_id}/user-log/stream',
                 'method': 'GET',
                 'params': {},
-                'headers': {
-                    'auth-token': self._token
-                }
+                'headers': {'auth-token': self._token},
             }
             if start_time:
                 opts['params']['startTime'] = format_date(start_time)
             if strategy_id:
                 opts['params']['strategyId'] = strategy_id
             if position_id:
                 opts['params']['positionId'] = position_id
             if level:
                 opts['params']['level'] = level
             if limit:
                 opts['params']['limit'] = limit
             try:
-                packets = await self._domainClient.request_copyfactory(opts, True)
+                packets = await self._domain_client.request_copyfactory(opts, True)
                 # stop job if user has unsubscribed in time of new packets has been received
-                if listener_id not in self._subscriberLogListeners:
+                if listener_id not in self._subscriber_log_listeners:
                     return
                 await listener.on_user_log(packets)
-                throttle_time = self._errorThrottleTime
-                if listener_id in self._subscriberLogListeners and len(packets):
+                throttle_time = self._error_throttle_time
+                if listener_id in self._subscriber_log_listeners and len(packets):
                     start_time = date(packets[0]['time']) + timedelta(milliseconds=1)
             except NotFoundException as err:
                 await listener.on_error(err)
                 self._logger.error(f'Subscriber {subscriber_id} not found, removing listener f{listener_id}')
-                if listener_id in self._subscriberLogListeners:
-                    del self._subscriberLogListeners[listener_id]
+                if listener_id in self._subscriber_log_listeners:
+                    del self._subscriber_log_listeners[listener_id]
             except Exception as err:
                 await listener.on_error(err)
-                self._logger.error(f'Failed to retrieve user log stream for subscriber {subscriber_id}, ' +
-                                   f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds', err)
+                self._logger.error(
+                    f'Failed to retrieve user log stream for subscriber {subscriber_id}, '
+                    + f'listener {listener_id}, retrying in {math.floor(throttle_time)} seconds',
+                    err,
+                )
                 await asyncio.sleep(throttle_time)
                 throttle_time = min(throttle_time * 2, 30)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/streaming/userLogListenerManager_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/streaming/user_log_listener_manager_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,30 @@
-from ....models import date
-from .userLogListenerManager import UserLogListenerManager
-from .userLogListener import UserLogListener
-from ...domain_client import DomainClient
-from ..copyFactory_models import CopyFactoryUserLogMessage
-from ...errorHandler import NotFoundException
-from mock import MagicMock, patch, AsyncMock
 from asyncio import sleep
 from typing import List
+
 import pytest
+from mock import MagicMock, patch, AsyncMock
+
+from .user_log_listener import UserLogListener
+from .user_log_listener_manager import UserLogListenerManager
+from ..copyfactory_models import CopyFactoryUserLogMessage
+from ...domain_client import DomainClient
+from ...error_handler import NotFoundException
+from ....models import date
 
 token = 'header.payload.sign'
-expected = [{
-    'time': '2020-08-08T08:57:30.328Z',
-    'level': 'INFO',
-    'message': 'message1'
-}, {
-    'time': '2020-08-08T07:57:30.328Z',
-    'level': 'INFO',
-    'message': 'message0'
-}]
-
-expected2 = [{
-    'time': '2020-08-08T10:57:30.328Z',
-    'level': 'INFO',
-    'message': 'message3'
-}, {
-    'time': '2020-08-08T09:57:30.328Z',
-    'level': 'INFO',
-    'message': 'message2'
-}]
+expected = [
+    {'time': '2020-08-08T08:57:30.328Z', 'level': 'INFO', 'message': 'message1'},
+    {'time': '2020-08-08T07:57:30.328Z', 'level': 'INFO', 'message': 'message0'},
+]
+
+expected2 = [
+    {'time': '2020-08-08T10:57:30.328Z', 'level': 'INFO', 'message': 'message3'},
+    {'time': '2020-08-08T09:57:30.328Z', 'level': 'INFO', 'message': 'message2'},
+]
 
 domain_client = DomainClient(MagicMock(), token)
 user_log_listener_manager = UserLogListenerManager(domain_client)
 call_stub = MagicMock()
 error_stub = MagicMock()
 listener = UserLogListener()
 
@@ -66,64 +58,64 @@
         if arg == {
             'url': '/users/current/strategies/ABCD/user-log/stream',
             'method': 'GET',
             'params': {
                 'startTime': '2020-08-08T00:00:00.000Z',
                 'positionId': 'positionId',
                 'level': 'DEBUG',
-                'limit': 10
-            },
-            'headers': {
-                'auth-token': token
+                'limit': 10,
             },
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected
         elif arg == {
             'url': '/users/current/strategies/ABCD/user-log/stream',
             'method': 'GET',
             'params': {
                 'startTime': '2020-08-08T08:57:30.329Z',
                 'positionId': 'positionId',
                 'level': 'DEBUG',
-                'limit': 10
-            },
-            'headers': {
-                'auth-token': token
+                'limit': 10,
             },
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected2
         else:
             await sleep(0.1)
             return []
 
     domain_client.request_copyfactory = AsyncMock(side_effect=get_logs_func)
 
 
 class TestStrategyLogs:
     @pytest.mark.asyncio
     async def test_add_strategy_listener(self, prepare_strategy_logs):
         """Should add listener."""
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_strategy_log_listener(
-                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10)
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10
+            )
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             call_stub.assert_any_call(expected2)
             user_log_listener_manager.remove_strategy_log_listener(id)
 
     @pytest.mark.asyncio
     async def test_remove_strategy_listener(self, prepare_strategy_logs):
         """Should remove listener."""
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_strategy_log_listener(
-                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10)
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10
+            )
             await sleep(0.11)
             user_log_listener_manager.remove_strategy_log_listener(id)
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             assert call_stub.call_count == 1
 
     @pytest.mark.asyncio
@@ -144,31 +136,31 @@
             if arg == {
                 'url': '/users/current/strategies/ABCD/user-log/stream',
                 'method': 'GET',
                 'params': {
                     'startTime': '2020-08-08T00:00:00.000Z',
                     'positionId': 'positionId',
                     'level': 'DEBUG',
-                    'limit': 10
-                },
-                'headers': {
-                    'auth-token': token
+                    'limit': 10,
                 },
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.05)
                 return expected
             else:
                 await sleep(0.5)
                 return []
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_transaction_func)
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_strategy_log_listener(
-                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10)
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             assert error_stub.call_count == 1
             error_stub.assert_any_call(error)
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
@@ -191,43 +183,41 @@
             if arg == {
                 'url': '/users/current/strategies/ABCD/user-log/stream',
                 'method': 'GET',
                 'params': {
                     'startTime': '2020-08-08T00:00:00.000Z',
                     'positionId': 'positionId',
                     'level': 'DEBUG',
-                    'limit': 10
-                },
-                'headers': {
-                    'auth-token': token
+                    'limit': 10,
                 },
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 return expected
             elif arg == {
                 'url': '/users/current/strategies/ABCD/user-log/stream',
                 'method': 'GET',
                 'params': {
                     'startTime': '2020-08-08T08:57:30.329Z',
                     'positionId': 'positionId',
                     'level': 'DEBUG',
-                    'limit': 10
-                },
-                'headers': {
-                    'auth-token': token
+                    'limit': 10,
                 },
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 raise error
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_logs_func)
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_strategy_log_listener(
-                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10)
+                listener, 'ABCD', date('2020-08-08T00:00:00.000Z'), 'positionId', 'DEBUG', 10
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
             assert call_stub.call_count == 1
             await sleep(0.2)
@@ -247,65 +237,65 @@
             'url': '/users/current/subscribers/accountId/user-log/stream',
             'method': 'GET',
             'params': {
                 'startTime': '2020-08-08T00:00:00.000Z',
                 'strategyId': 'strategyId',
                 'positionId': 'positionId',
                 'level': 'DEBUG',
-                'limit': 10
-            },
-            'headers': {
-                'auth-token': token
+                'limit': 10,
             },
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected
         elif arg == {
             'url': '/users/current/subscribers/accountId/user-log/stream',
             'method': 'GET',
             'params': {
                 'startTime': '2020-08-08T08:57:30.329Z',
                 'strategyId': 'strategyId',
                 'positionId': 'positionId',
                 'level': 'DEBUG',
-                'limit': 10
-            },
-            'headers': {
-                'auth-token': token
+                'limit': 10,
             },
+            'headers': {'auth-token': token},
         }:
             await sleep(0.1)
             return expected2
         else:
             await sleep(0.1)
             return []
 
     domain_client.request_copyfactory = AsyncMock(side_effect=get_logs_func)
 
 
 class TestSubscriberTransactions:
     @pytest.mark.asyncio
     async def test_add_subscriber_listener(self, prepare_subscriber_logs):
         """Should add listener."""
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_subscriber_log_listener(
-                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10)
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10
+            )
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             call_stub.assert_any_call(expected2)
             user_log_listener_manager.remove_subscriber_log_listener(id)
 
     @pytest.mark.asyncio
     async def test_remove_strategy_listener(self, prepare_subscriber_logs):
         """Should remove listener."""
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_subscriber_log_listener(
-                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10)
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10
+            )
             await sleep(0.11)
             user_log_listener_manager.remove_subscriber_log_listener(id)
             await sleep(0.22)
             call_stub.assert_any_call(expected)
             assert call_stub.call_count == 1
 
     @pytest.mark.asyncio
@@ -327,31 +317,31 @@
                 'url': '/users/current/subscribers/accountId/user-log/stream',
                 'method': 'GET',
                 'params': {
                     'startTime': '2020-08-08T00:00:00.000Z',
                     'strategyId': 'strategyId',
                     'positionId': 'positionId',
                     'level': 'DEBUG',
-                    'limit': 10
-                },
-                'headers': {
-                    'auth-token': token
+                    'limit': 10,
                 },
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.05)
                 return expected
             else:
                 await sleep(0.5)
                 return []
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_transaction_func)
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_subscriber_log_listener(
-                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10)
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             assert error_stub.call_count == 1
             error_stub.assert_any_call(error)
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
@@ -375,44 +365,42 @@
                 'url': '/users/current/subscribers/accountId/user-log/stream',
                 'method': 'GET',
                 'params': {
                     'startTime': '2020-08-08T00:00:00.000Z',
                     'strategyId': 'strategyId',
                     'positionId': 'positionId',
                     'level': 'DEBUG',
-                    'limit': 10
-                },
-                'headers': {
-                    'auth-token': token
+                    'limit': 10,
                 },
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 return expected
             elif arg == {
                 'url': '/users/current/subscribers/accountId/user-log/stream',
                 'method': 'GET',
                 'params': {
                     'startTime': '2020-08-08T08:57:30.329Z',
                     'strategyId': 'strategyId',
                     'positionId': 'positionId',
                     'level': 'DEBUG',
-                    'limit': 10
-                },
-                'headers': {
-                    'auth-token': token
+                    'limit': 10,
                 },
+                'headers': {'auth-token': token},
             }:
                 await sleep(0.1)
                 raise error
 
         domain_client.request_copyfactory = AsyncMock(side_effect=get_logs_func)
-        with patch('lib.clients.copyFactory.streaming.userLogListenerManager.asyncio.sleep',
-                   new=lambda x: sleep(x / 10)):
+        with patch(
+            'lib.clients.copyfactory.streaming.user_log_listener_manager.asyncio.sleep', new=lambda x: sleep(x / 10)
+        ):
             id = user_log_listener_manager.add_subscriber_log_listener(
-                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10)
+                listener, 'accountId', date('2020-08-08T00:00:00.000Z'), 'strategyId', 'positionId', 'DEBUG', 10
+            )
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 1
             assert call_stub.call_count == 0
             await sleep(0.06)
             assert domain_client.request_copyfactory.call_count == 2
             assert call_stub.call_count == 1
             await sleep(0.2)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/trading_client.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/trading_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,46 @@
-from ..metaApi_client import MetaApiClient
-from ..domain_client import DomainClient
-from .streaming.stopoutListenerManager import StopoutListenerManager
-from .streaming.userLogListenerManager import UserLogListenerManager
-from .signal_client import SignalClient
-from .copyFactory_models import CopyFactoryStrategyStopout, CopyFactoryUserLogMessage, \
-    CopyFactoryStrategyStopoutReason, LogLevel
-from .streaming.stopoutListener import StopoutListener
-from .streaming.userLogListener import UserLogListener
+from datetime import datetime
 from typing import List
+
 from httpx import Response
-from datetime import datetime
+
+from .copyfactory_models import (
+    CopyFactoryStrategyStopout,
+    CopyFactoryUserLogMessage,
+    CopyFactoryStrategyStopoutReason,
+    LogLevel,
+)
+from .signal_client import SignalClient
+from .streaming.stopout_listener import StopoutListener
+from .streaming.stopout_listener_manager import StopoutListenerManager
+from .streaming.user_log_listener import UserLogListener
+from .streaming.user_log_listener_manager import UserLogListenerManager
+from ..domain_client import DomainClient
+from ..metaapi_client import MetaApiClient
 from ...models import format_date, convert_iso_time_to_date
 
 
 class TradingClient(MetaApiClient):
     """metaapi.cloud CopyFactory trading API (trade copying trading API) client (see
     https://metaapi.cloud/docs/copyfactory/)"""
 
     def __init__(self, domain_client: DomainClient):
-        """Inits CopyFactory trading API client instance.
+        """Initializes CopyFactory trading API client instance.
 
         Args:
             domain_client: Domain client.
         """
         super().__init__(domain_client)
-        self._domainClient = domain_client
-        self._stopoutListenerManager = StopoutListenerManager(domain_client)
-        self._userLogListenerManager = UserLogListenerManager(domain_client)
-
-    async def resynchronize(self, subscriber_id: str, strategy_ids: List[str] = None,
-                            position_ids: List[str] = None) -> Response:
+        self._domain_client = domain_client
+        self._stopout_listener_manager = StopoutListenerManager(domain_client)
+        self._user_log_listener_manager = UserLogListenerManager(domain_client)
+
+    async def resynchronize(
+        self, subscriber_id: str, strategy_ids: List[str] = None, position_ids: List[str] = None
+    ) -> Response:
         """Resynchronizes the account. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/resynchronize/
 
         Args:
             subscriber_id: Account id.
             strategy_ids: Array of strategy ids to resynchronize. Default is to synchronize all strategies.
             position_ids: Array of position ids to resynchronize. Default is to synchronize all positions.
@@ -45,35 +52,33 @@
             return self._handle_no_access_exception('resynchronize')
         params = {}
         if strategy_ids:
             params['strategyId'] = strategy_ids
         if position_ids:
             params['positionId'] = position_ids
         opts = {
-          'url': f'/users/current/subscribers/{subscriber_id}/resynchronize',
-          'method': 'POST',
-          'headers': {
-            'auth-token': self._token
-          },
-          'params': params,
+            'url': f'/users/current/subscribers/{subscriber_id}/resynchronize',
+            'method': 'POST',
+            'headers': {'auth-token': self._token},
+            'params': params,
         }
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
     async def get_signal_client(self, account_id: str):
         """Generates an instance of signal client for an account.
 
         Args:
             account_id: Account id.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_signal_client')
 
-        account_data = await self._domainClient.get_account_info(account_id)
-        host = await self._domainClient.get_signal_client_host(account_data['regions'])
-        return SignalClient(account_data['id'], host, self._domainClient)
+        account_data = await self._domain_client.get_account_info(account_id)
+        host = await self._domain_client.get_signal_client_host(account_data['regions'])
+        return SignalClient(account_data['id'], host, self._domain_client)
 
     async def get_stopouts(self, subscriber_id: str) -> 'List[CopyFactoryStrategyStopout]':
         """Returns subscriber account stopouts. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/getStopOuts/
 
         Args:
             subscriber_id: Account id.
@@ -82,49 +87,45 @@
             A coroutine which resolves with stopouts found.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_stopouts')
         opts = {
             'url': f'/users/current/subscribers/{subscriber_id}/stopouts',
             'method': 'GET',
-            'headers': {
-                'auth-token': self._token
-            }
+            'headers': {'auth-token': self._token},
         }
-        result = await self._domainClient.request_copyfactory(opts)
+        result = await self._domain_client.request_copyfactory(opts)
         convert_iso_time_to_date(result)
         return result
 
-    async def reset_subscription_stopouts(self, subscriber_id: str, strategy_id: str,
-                                          reason: CopyFactoryStrategyStopoutReason) -> Response:
+    async def reset_subscription_stopouts(
+        self, subscriber_id: str, strategy_id: str, reason: CopyFactoryStrategyStopoutReason
+    ) -> Response:
         """Resets subscription stopouts. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/resetSubscriptionStopOuts/
 
         Args:
             subscriber_id: Account id.
             strategy_id: Strategy id.
             reason: Stopout reason to reset.
 
         Returns:
             A coroutine which resolves when the stopouts are reset.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('reset_subscription_stopouts')
         opts = {
-            'url': f'/users/current/subscribers/{subscriber_id}/subscription-strategies/{strategy_id}' +
-                   f'/stopouts/{reason}/reset',
+            'url': f'/users/current/subscribers/{subscriber_id}/subscription-strategies/{strategy_id}'
+            + f'/stopouts/{reason}/reset',
             'method': 'POST',
-            'headers': {
-                'auth-token': self._token
-            }
+            'headers': {'auth-token': self._token},
         }
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
-    async def reset_subscriber_stopouts(self, subscriber_id: str, reason: CopyFactoryStrategyStopoutReason) \
-            -> Response:
+    async def reset_subscriber_stopouts(self, subscriber_id: str, reason: CopyFactoryStrategyStopoutReason) -> Response:
         """Resets subscriber stopouts. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/resetSubscriberStopOuts/
 
         Args:
             subscriber_id: Account id.
             reason: Stopout reason to reset.
 
@@ -132,23 +133,29 @@
             A coroutine which resolves when the stopouts are reset.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('reset_subscriber_stopouts')
         opts = {
             'url': f'/users/current/subscribers/{subscriber_id}/stopouts/{reason}/reset',
             'method': 'POST',
-            'headers': {
-                'auth-token': self._token
-            }
+            'headers': {'auth-token': self._token},
         }
-        return await self._domainClient.request_copyfactory(opts)
+        return await self._domain_client.request_copyfactory(opts)
 
-    async def get_user_log(self, subscriber_id: str, start_time: datetime = None, end_time: datetime = None,
-                           strategy_id: str = None, position_id: str = None, level: LogLevel = None,
-                           offset: int = 0, limit: int = 1000) -> 'List[CopyFactoryUserLogMessage]':
+    async def get_user_log(
+        self,
+        subscriber_id: str,
+        start_time: datetime = None,
+        end_time: datetime = None,
+        strategy_id: str = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        offset: int = 0,
+        limit: int = 1000,
+    ) -> 'List[CopyFactoryUserLogMessage]':
         """Returns copy trading user log for an account and time range, sorted in reverse chronological order. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/getUserLog/
 
         Args:
             subscriber_id: Subscriber id.
             start_time: Time to start loading data from.
             end_time: Time to stop loading data at.
@@ -159,43 +166,45 @@
             limit: Pagination limit. Default is 1000.
 
         Returns:
             A coroutine which resolves with log records found.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_user_log')
-        params = {
-            'offset': offset,
-            'limit': limit
-        }
+        params = {'offset': offset, 'limit': limit}
         if start_time:
             params['startTime'] = format_date(start_time)
         if end_time:
             params['endTime'] = format_date(end_time)
         if strategy_id:
             params['strategyId'] = strategy_id
         if position_id:
             params['positionId'] = position_id
         if level:
             params['level'] = level
         opts = {
             'url': f'/users/current/subscribers/{subscriber_id}/user-log',
             'method': 'GET',
-            'headers': {
-                'auth-token': self._token
-            },
-            'params': params
+            'headers': {'auth-token': self._token},
+            'params': params,
         }
-        result = await self._domainClient.request_copyfactory(opts, True)
+        result = await self._domain_client.request_copyfactory(opts, True)
         convert_iso_time_to_date(result)
         return result
 
-    async def get_strategy_log(self, strategy_id: str, start_time: datetime = None, end_time: datetime = None,
-                               position_id: str = None, level: LogLevel = None,
-                               offset: int = 0, limit: int = 1000) -> 'List[CopyFactoryUserLogMessage]':
+    async def get_strategy_log(
+        self,
+        strategy_id: str,
+        start_time: datetime = None,
+        end_time: datetime = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        offset: int = 0,
+        limit: int = 1000,
+    ) -> 'List[CopyFactoryUserLogMessage]':
         """Returns event log for CopyFactory strategy, sorted in reverse chronological order. See
         https://metaapi.cloud/docs/copyfactory/restApi/api/trading/getStrategyLog/
 
         Args:
             strategy_id: Strategy id to retrieve log for.
             start_time: Time to start loading data from.
             end_time: Time to stop loading data at.
@@ -205,107 +214,119 @@
             limit: Pagination limit. Default is 1000.
 
         Returns:
             A coroutine which resolves with log records found.
         """
         if self._is_not_jwt_token():
             return self._handle_no_access_exception('get_strategy_log')
-        params = {
-            'offset': offset,
-            'limit': limit
-        }
+        params = {'offset': offset, 'limit': limit}
         if start_time:
             params['startTime'] = format_date(start_time)
         if end_time:
             params['endTime'] = format_date(end_time)
         if position_id:
             params['positionId'] = position_id
         if level:
             params['level'] = level
         opts = {
             'url': f'/users/current/strategies/{strategy_id}/user-log',
             'method': 'GET',
-            'headers': {
-                'auth-token': self._token
-            },
-            'params': params
+            'headers': {'auth-token': self._token},
+            'params': params,
         }
-        result = await self._domainClient.request_copyfactory(opts, True)
+        result = await self._domain_client.request_copyfactory(opts, True)
         convert_iso_time_to_date(result)
         return result
 
-    def add_stopout_listener(self, listener: StopoutListener, account_id: str = None, strategy_id: str = None,
-                             sequence_number: int = None) -> str:
+    def add_stopout_listener(
+        self, listener: StopoutListener, account_id: str = None, strategy_id: str = None, sequence_number: int = None
+    ) -> str:
         """Adds a stopout listener and creates a job to make requests.
 
         Args:
             listener: Stopout listener.
             account_id: Account id.
             strategy_id: Strategy id.
             sequence_number: Sequence number.
 
         Returns:
             Listener id.
         """
-        return self._stopoutListenerManager.add_stopout_listener(listener, account_id, strategy_id, sequence_number)
+        return self._stopout_listener_manager.add_stopout_listener(listener, account_id, strategy_id, sequence_number)
 
     def remove_stopout_listener(self, listener_id: str):
         """Removes stopout listener and cancels the event stream.
 
         Args:
             listener_id: Stopout listener id.
         """
-        self._stopoutListenerManager.remove_stopout_listener(listener_id)
+        self._stopout_listener_manager.remove_stopout_listener(listener_id)
 
-    def add_strategy_log_listener(self, listener: UserLogListener, strategy_id: str, start_time: datetime = None,
-                                  position_id: str = None, level: LogLevel = None, limit: int = None) -> str:
+    def add_strategy_log_listener(
+        self,
+        listener: UserLogListener,
+        strategy_id: str,
+        start_time: datetime = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        limit: int = None,
+    ) -> str:
         """Adds a strategy log listener and creates a job to make requests.
 
         Args:
             listener: User log listener.
             strategy_id: Strategy id.
             start_time: Log search start time.
             position_id: Position id filter.
             level: Minimum severity level.
             limit: Log pagination limit.
 
         Returns:
             Listener id.
         """
-        return self._userLogListenerManager.add_strategy_log_listener(listener, strategy_id, start_time, position_id,
-                                                                      level, limit)
+        return self._user_log_listener_manager.add_strategy_log_listener(
+            listener, strategy_id, start_time, position_id, level, limit
+        )
 
     def remove_strategy_log_listener(self, listener_id: str):
         """Removes strategy log listener and cancels the event stream.
 
         Args:
             listener_id: Strategy log listener id.
         """
-        self._userLogListenerManager.remove_strategy_log_listener(listener_id)
+        self._user_log_listener_manager.remove_strategy_log_listener(listener_id)
 
-    def add_subscriber_log_listener(self, listener: UserLogListener, subscriber_id: str, start_time: datetime = None,
-                                    strategy_id: str = None, position_id: str = None, level: LogLevel = None,
-                                    limit: int = None) -> str:
+    def add_subscriber_log_listener(
+        self,
+        listener: UserLogListener,
+        subscriber_id: str,
+        start_time: datetime = None,
+        strategy_id: str = None,
+        position_id: str = None,
+        level: LogLevel = None,
+        limit: int = None,
+    ) -> str:
         """Adds a subscriber log listener and creates a job to make requests.
 
         Args:
             listener: User log listener.
             subscriber_id: Subscriber id.
             start_time: Log search start time.
             strategy_id: Strategy id filter.
             position_id: Position id filter.
             level: Minimum severity level.
             limit: Log pagination limit.
 
         Returns:
             Listener id.
         """
-        return self._userLogListenerManager.add_subscriber_log_listener(
-            listener, subscriber_id, start_time, strategy_id, position_id, level, limit)
+        return self._user_log_listener_manager.add_subscriber_log_listener(
+            listener, subscriber_id, start_time, strategy_id, position_id, level, limit
+        )
 
     def remove_subscriber_log_listener(self, listener_id: str):
         """Removes subscriber log listener and cancels the event stream.
 
         Args:
             listener_id: Subscriber log listener id.
         """
-        self._userLogListenerManager.remove_subscriber_log_listener(listener_id)
+        self._user_log_listener_manager.remove_subscriber_log_listener(listener_id)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/copyFactory/trading_client_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/copyfactory/trading_client_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-from .trading_client import TradingClient
 import pytest
-from ...models import date
 from mock import MagicMock, AsyncMock
+
+from .trading_client import TradingClient
+from ...models import date
+
 copy_factory_api_url = 'https://copyfactory-application-history-master-v1.agiliumtrade.agiliumtrade.ai'
 domain_client = MagicMock()
 trading_client = TradingClient(domain_client)
 token = 'header.payload.sign'
 
 
 @pytest.fixture(autouse=True)
@@ -19,280 +21,287 @@
 
 
 class TestTradingClient:
     @pytest.mark.asyncio
     async def test_resynchronize_copyfactory_account(self):
         """Should resynchronize CopyFactory account."""
         await trading_client.resynchronize('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', ['ABCD'], ['0123456'])
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/resynchronize',
-            'method': 'POST',
-            'headers': {
-                'auth-token': token
-            },
-            'params': {
-                'strategyId': ['ABCD'],
-                'positionId': ['0123456']
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/resynchronize',
+                'method': 'POST',
+                'headers': {'auth-token': token},
+                'params': {'strategyId': ['ABCD'], 'positionId': ['0123456']},
             }
-        })
+        )
 
     @pytest.mark.asyncio
     async def test_not_resynchronize_account_with_account_token(self):
         """Should not resynchronize CopyFactory subscriber with account token."""
         domain_client.token = 'token'
         trading_client = TradingClient(domain_client)
         try:
-            await trading_client.resynchronize('e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
-                                               ['ABCD'], ['0123456'])
+            await trading_client.resynchronize('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', ['ABCD'], ['0123456'])
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke resynchronize method, ' + \
-                   'because you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke resynchronize method, '
+                + 'because you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
     @pytest.mark.asyncio
     async def test_retrieve_stopouts(self):
         """Should retrieve stopouts."""
-        expected = [{
-            'strategyId': 'accountId',
-            'reason': 'monthly-balance',
-            'stoppedAt': '2020-08-08T07:57:30.328Z',
-            'strategy': {
-                'id': 'ABCD',
-                'name': 'Strategy'
-            },
-            'reasonDescription': 'total strategy equity drawdown exceeded limit',
-            'sequenceNumber': 2
-        }]
+        expected = [
+            {
+                'strategyId': 'accountId',
+                'reason': 'monthly-balance',
+                'stoppedAt': '2020-08-08T07:57:30.328Z',
+                'strategy': {'id': 'ABCD', 'name': 'Strategy'},
+                'reasonDescription': 'total strategy equity drawdown exceeded limit',
+                'sequenceNumber': 2,
+            }
+        ]
         domain_client.request_copyfactory = AsyncMock(return_value=expected)
         stopouts = await trading_client.get_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6')
         assert stopouts == expected
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/stopouts',
-            'method': 'GET',
-            'headers': {
-                'auth-token': token
-            },
-        })
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/stopouts',
+                'method': 'GET',
+                'headers': {'auth-token': token},
+            }
+        )
 
     @pytest.mark.asyncio
     async def test_not_retrieve_stopouts_with_account_token(self):
         """Should not retrieve stopouts from API with account token."""
         domain_client.token = 'token'
         trading_client = TradingClient(domain_client)
         try:
             await trading_client.get_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6')
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke get_stopouts method, ' + \
-                   'because you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke get_stopouts method, '
+                + 'because you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
     @pytest.mark.asyncio
     async def test_reset_stopouts(self):
         """Should reset stopouts."""
         await trading_client.reset_subscription_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', 'ABCD', 'daily-equity')
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/subscribers/' +
-            'e8867baa-5ec2-45ae-9930-4d5cea18d0d6/subscription-strategies/ABCD/stopouts/daily-equity/reset',
-            'method': 'POST',
-            'headers': {
-                'auth-token': token
-            },
-        })
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/subscribers/'
+                + 'e8867baa-5ec2-45ae-9930-4d5cea18d0d6/subscription-strategies/ABCD/stopouts/daily-equity/reset',
+                'method': 'POST',
+                'headers': {'auth-token': token},
+            }
+        )
 
     @pytest.mark.asyncio
     async def test_not_reset_stopouts_with_account_token(self):
         """Should not reset stopouts with account token."""
         domain_client.token = 'token'
         trading_client = TradingClient(domain_client)
         try:
-            await trading_client.reset_subscription_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
-                                                             'ABCD', 'daily-equity')
+            await trading_client.reset_subscription_stopouts(
+                'e8867baa-5ec2-45ae-9930-4d5cea18d0d6', 'ABCD', 'daily-equity'
+            )
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke reset_subscription_stopouts method, ' + \
-                   'because you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke reset_subscription_stopouts method, '
+                + 'because you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
     @pytest.mark.asyncio
     async def test_reset_subscriber_stopouts(self):
         """Should reset subscriber stopouts."""
         await trading_client.reset_subscriber_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', 'daily-equity')
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/stopouts/daily-equity/reset',
-            'method': 'POST',
-            'headers': {
-                'auth-token': token
-            },
-        })
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/stopouts/daily-equity/reset',
+                'method': 'POST',
+                'headers': {'auth-token': token},
+            }
+        )
 
     @pytest.mark.asyncio
     async def test_not_reset_subscriber_stopouts_with_account_token(self):
         """Should not reset subscriber stopouts with account token."""
         domain_client.token = 'token'
         trading_client = TradingClient(domain_client)
         try:
-            await trading_client.reset_subscriber_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
-                                                           'daily-equity')
+            await trading_client.reset_subscriber_stopouts('e8867baa-5ec2-45ae-9930-4d5cea18d0d6', 'daily-equity')
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke reset_subscriber_stopouts method, ' + \
-                   'because you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke reset_subscriber_stopouts method, '
+                + 'because you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
     @pytest.mark.asyncio
     async def test_retrieve_copy_trading_log(self):
         """Should retrieve copy trading user log."""
-        expected = [{
-          'time': '2020-08-08T07:57:30.328Z',
-          'level': 'INFO',
-          'message': 'message'
-        }]
+        expected = [{'time': '2020-08-08T07:57:30.328Z', 'level': 'INFO', 'message': 'message'}]
         domain_client.request_copyfactory = AsyncMock(return_value=expected)
-        records = await trading_client.get_user_log('e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
-                                                    date('2020-08-01T00:00:00.000Z'),
-                                                    date('2020-08-10T00:00:00.000Z'), 'strategyId', 'positionId')
+        records = await trading_client.get_user_log(
+            'e8867baa-5ec2-45ae-9930-4d5cea18d0d6',
+            date('2020-08-01T00:00:00.000Z'),
+            date('2020-08-10T00:00:00.000Z'),
+            'strategyId',
+            'positionId',
+        )
         assert records == expected
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/user-log',
-            'method': 'GET',
-            'params': {
-                'startTime': '2020-08-01T00:00:00.000Z',
-                'endTime': '2020-08-10T00:00:00.000Z',
-                'offset': 0,
-                'limit': 1000,
-                'strategyId': 'strategyId',
-                'positionId': 'positionId'
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/subscribers/e8867baa-5ec2-45ae-9930-4d5cea18d0d6/user-log',
+                'method': 'GET',
+                'params': {
+                    'startTime': '2020-08-01T00:00:00.000Z',
+                    'endTime': '2020-08-10T00:00:00.000Z',
+                    'offset': 0,
+                    'limit': 1000,
+                    'strategyId': 'strategyId',
+                    'positionId': 'positionId',
+                },
+                'headers': {'auth-token': token},
             },
-            'headers': {
-                'auth-token': token
-            },
-        }, True)
+            True,
+        )
 
     @pytest.mark.asyncio
     async def test_not_retrieve_copy_trading_log_with_account_token(self):
         """Should not retrieve copy trading user log from API with account token."""
         domain_client.token = 'token'
         trading_client = TradingClient(domain_client)
         try:
             await trading_client.get_user_log('e8867baa-5ec2-45ae-9930-4d5cea18d0d6')
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke get_user_log method, ' + \
-                   'because you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke get_user_log method, '
+                + 'because you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
     @pytest.mark.asyncio
     async def test_retrieve_copy_trading_strategy_log(self):
         """Should retrieve copy trading strategy log."""
-        expected = [{
-            'time': '2020-08-08T07:57:30.328Z',
-            'level': 'INFO',
-            'message': 'message'
-        }]
+        expected = [{'time': '2020-08-08T07:57:30.328Z', 'level': 'INFO', 'message': 'message'}]
         domain_client.request_copyfactory = AsyncMock(return_value=expected)
-        records = await trading_client.get_strategy_log('ABCD', date('2020-08-01T00:00:00.000Z'),
-                                                        date('2020-08-10T00:00:00.000Z'), 'positionId', 'DEBUG')
+        records = await trading_client.get_strategy_log(
+            'ABCD', date('2020-08-01T00:00:00.000Z'), date('2020-08-10T00:00:00.000Z'), 'positionId', 'DEBUG'
+        )
         assert records == expected
-        domain_client.request_copyfactory.assert_called_with({
-            'url': '/users/current/strategies/ABCD/user-log',
-            'method': 'GET',
-            'params': {
-                'startTime': '2020-08-01T00:00:00.000Z',
-                'endTime': '2020-08-10T00:00:00.000Z',
-                'offset': 0,
-                'limit': 1000,
-                'level': 'DEBUG',
-                'positionId': 'positionId'
-            },
-            'headers': {
-                'auth-token': token
+        domain_client.request_copyfactory.assert_called_with(
+            {
+                'url': '/users/current/strategies/ABCD/user-log',
+                'method': 'GET',
+                'params': {
+                    'startTime': '2020-08-01T00:00:00.000Z',
+                    'endTime': '2020-08-10T00:00:00.000Z',
+                    'offset': 0,
+                    'limit': 1000,
+                    'level': 'DEBUG',
+                    'positionId': 'positionId',
+                },
+                'headers': {'auth-token': token},
             },
-        }, True)
+            True,
+        )
 
     @pytest.mark.asyncio
     async def test_not_retrieve_copy_trading_strategy_log_with_account_token(self):
         """Should not retrieve copy trading strategy log from API with account token."""
         domain_client.token = 'token'
         trading_client = TradingClient(domain_client)
         try:
             await trading_client.get_strategy_log('ABCD')
             pytest.fail()
         except Exception as err:
-            assert err.__str__() == 'You can not invoke get_strategy_log method, ' + \
-                   'because you have connected with account access token. Please use API access token from ' + \
-                   'https://app.metaapi.cloud/token page to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke get_strategy_log method, '
+                + 'because you have connected with account access token. Please use API access token from '
+                + 'https://app.metaapi.cloud/token page to invoke this method.'
+            )
 
     @pytest.mark.asyncio
     async def test_get_account(self):
         """Should get account."""
         domain_client.get_account_info = AsyncMock(return_value={'id': 'accountId', 'regions': ['vint-hill']})
 
         async def get_signal_client_host(regions):
-            return {
-                'host': 'https://copyfactory-api-v1',
-                'regions': regions,
-                'domain': 'agiliumtrade.ai'
-            }
+            return {'host': 'https://copyfactory-api-v1', 'regions': regions, 'domain': 'agiliumtrade.ai'}
 
         domain_client.get_signal_client_host = AsyncMock(side_effect=get_signal_client_host)
         client = await trading_client.get_signal_client('accountId')
-        assert client._accountId == 'accountId'
+        assert client._account_id == 'accountId'
         assert client._host['regions'] == ['vint-hill']
 
     @pytest.mark.asyncio
     async def test_add_stopout_listener(self):
         """Should add stopout listener."""
         call_stub = MagicMock(return_value='listenerId')
-        trading_client._stopoutListenerManager.add_stopout_listener = call_stub
+        trading_client._stopout_listener_manager.add_stopout_listener = call_stub
         listener = MagicMock()
         listener_id = trading_client.add_stopout_listener(listener, 'accountId', 'ABCD', 1)
         assert listener_id == 'listenerId'
         call_stub.assert_called_with(listener, 'accountId', 'ABCD', 1)
 
     @pytest.mark.asyncio
     async def test_remove_stopout_listener(self):
         """Should remove stopout listener."""
         call_stub = MagicMock()
-        trading_client._stopoutListenerManager.remove_stopout_listener = call_stub
+        trading_client._stopout_listener_manager.remove_stopout_listener = call_stub
         trading_client.remove_stopout_listener('id')
         call_stub.assert_called_with('id')
 
 
 class TestUserLogListener:
-
     @pytest.mark.asyncio
     async def test_add_strategy_log_listener(self):
         """Should add strategy listener."""
         call_stub = MagicMock(return_value='listenerId')
-        trading_client._userLogListenerManager.add_strategy_log_listener = call_stub
+        trading_client._user_log_listener_manager.add_strategy_log_listener = call_stub
         listener = MagicMock()
         listener_id = trading_client.add_strategy_log_listener(listener, 'ABCD')
         assert listener_id == 'listenerId'
         call_stub.assert_called_with(listener, 'ABCD', None, None, None, None)
 
     @pytest.mark.asyncio
     async def test_remove_strategy_log_listener(self):
         """Should remove stopout listener."""
         call_stub = MagicMock()
-        trading_client._stopoutListenerManager.remove_stopout_listener = call_stub
+        trading_client._stopout_listener_manager.remove_stopout_listener = call_stub
         trading_client.remove_stopout_listener('id')
         call_stub.assert_called_with('id')
 
     @pytest.mark.asyncio
     async def test_add_subscriber_log_listener(self):
         """Should add subscriber listener."""
         call_stub = MagicMock(return_value='listenerId')
-        trading_client._userLogListenerManager.add_subscriber_log_listener = call_stub
+        trading_client._user_log_listener_manager.add_subscriber_log_listener = call_stub
         listener = MagicMock()
         listener_id = trading_client.add_subscriber_log_listener(listener, 'accountId')
         assert listener_id == 'listenerId'
         call_stub.assert_called_with(listener, 'accountId', None, None, None, None, None)
 
     @pytest.mark.asyncio
     async def test_remove_subscriber_log_listener(self):
         """Should remove subscriber listener."""
         call_stub = MagicMock()
-        trading_client._userLogListenerManager.remove_subscriber_log_listener = call_stub
+        trading_client._user_log_listener_manager.remove_subscriber_log_listener = call_stub
         trading_client.remove_subscriber_log_listener('id')
         call_stub.assert_called_with('id')
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/domain_client.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/domain_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
+import asyncio
+from copy import copy
 from datetime import datetime
 from typing import List
-from copy import copy
-from ..models import promise_any
+
 from typing_extensions import TypedDict
-import asyncio
+
+from ..models import promise_any
 
 
 class AccountInfo(TypedDict):
     """Account request info."""
+
     id: str
     """Primary account id."""
     regions: List[str]
     """Account available regions."""
 
 
 class DomainClient:
     """Connection URL and request managing client"""
 
     def __init__(self, http_client, token: str, domain: str = None):
-        """Inits domain client instance.
+        """Initializes domain client instance.
 
         Args:
             http_client: HTTP client.
             token: Authorization token.
             domain: Domain to connect to, default is agiliumtrade.agiliumtrade.ai.
         """
-        self._httpClient = http_client
+        self._http_client = http_client
         self._domain = domain or 'agiliumtrade.agiliumtrade.ai'
         self._token = token
-        self._urlCache = None
-        self._regionCache = []
-        self._regionIndex = 0
+        self._url_cache = None
+        self._region_cache = []
+        self._region_index = 0
 
     @property
     def domain(self) -> str:
         """Returns domain client domain.
 
         Returns:
             Client domain.
@@ -59,38 +62,42 @@
 
         Returns:
             Request result.
         """
         await self._update_host()
         try:
             request_opts = copy(opts)
-            request_opts['url'] = self._urlCache['url'] + request_opts['url']
-            return await self._httpClient.request(request_opts, is_extended_timeout)
+            request_opts['url'] = self._url_cache['url'] + request_opts['url']
+            return await self._http_client.request(request_opts, is_extended_timeout)
         except Exception as err:
-            if err.__class__.__name__ not in ['ConflictException', 'InternalException', 'ApiException',
-                                              'ConnectTimeout']:
+            if err.__class__.__name__ not in [
+                'ConflictException',
+                'InternalException',
+                'ApiException',
+                'ConnectTimeout',
+            ]:
                 raise err
             else:
-                if len(self._regionCache) == self._regionIndex + 1:
-                    self._regionIndex = 0
+                if len(self._region_cache) == self._region_index + 1:
+                    self._region_index = 0
                     raise err
                 else:
-                    self._regionIndex += 1
+                    self._region_index += 1
                     return await self.request_copyfactory(opts, is_extended_timeout)
 
     async def request(self, opts: dict):
         """Sends an http request.
 
         Args:
             opts: Request options.
 
         Returns:
             Request result.
         """
-        return await self._httpClient.request(opts)
+        return await self._http_client.request(opts)
 
     async def request_signal(self, opts: dict, host: dict, account_id: str):
         """Sends a signal client request.
 
         Args:
             opts: Request options.
             host: Signal client host data.
@@ -101,15 +108,15 @@
         """
         asyncio.create_task(self._update_account_regions(host, account_id))
         tasks = []
         for region in host['regions']:
             request_opts = copy(opts)
             request_opts['url'] = f'{host["host"]}.{region}.{host["domain"]}' + opts["url"]
             request_opts['headers'] = {'auth-token': self._token}
-            tasks.append(asyncio.create_task(self._httpClient.request_with_failover(request_opts)))
+            tasks.append(asyncio.create_task(self._http_client.request_with_failover(request_opts)))
         return await promise_any(tasks)
 
     async def get_signal_client_host(self, regions: List[str]) -> dict:
         """Returns CopyFactory host for signal client requests.
 
         Args:
             regions: Subscriber regions.
@@ -118,82 +125,82 @@
             Signal client CopyFactory host.
         """
         await self._update_host()
         return {
             'host': 'https://copyfactory-api-v1',
             'regions': regions,
             'lastUpdated': datetime.now().timestamp(),
-            'domain': self._urlCache['domain']
+            'domain': self._url_cache['domain'],
         }
 
     async def get_account_info(self, account_id: str) -> AccountInfo:
         """Returns account data by id.
 
         Args:
             account_id: Account id.
 
         Returns:
             Account data.
         """
+
         async def get_account(id: str):
             account_opts = {
                 'url': f'https://mt-provisioning-api-v1.{self.domain}/users/current/accounts/{id}',
                 'method': 'GET',
-                'headers': {
-                  'auth-token': self.token
-                },
+                'headers': {'auth-token': self.token},
             }
-            return await self._httpClient.request_with_failover(account_opts)
+            return await self._http_client.request_with_failover(account_opts)
 
         account_data = await get_account(account_id)
         if 'primaryAccountId' in account_data:
             primary_account_id = account_data['primaryAccountId']
             account_data = await get_account(primary_account_id)
         else:
             primary_account_id = account_data['_id']
 
-        regions = [account_data['region']] + \
-            (list(map(lambda replica: replica['region'], account_data['accountReplicas'])) if
-             'accountReplicas' in account_data else [])
+        regions = [account_data['region']] + (
+            list(map(lambda replica: replica['region'], account_data['accountReplicas']))
+            if 'accountReplicas' in account_data
+            else []
+        )
 
-        return {
-            'id': primary_account_id,
-            'regions': regions
-        }
+        return {'id': primary_account_id, 'regions': regions}
 
     async def _update_host(self):
-        if not self._urlCache or self._urlCache['lastUpdated'] < datetime.now().timestamp() - 60 * 10:
+        if not self._url_cache or self._url_cache['lastUpdated'] < datetime.now().timestamp() - 60 * 10:
             await self._update_regions()
-            url_settings = await self._httpClient.request({
-                'url': f'https://mt-provisioning-api-v1.{self._domain}/users/current/servers/mt-client-api',
-                'method': 'GET',
-                'headers': {
-                    'auth-token': self._token
+            url_settings = await self._http_client.request(
+                {
+                    'url': f'https://mt-provisioning-api-v1.{self._domain}/users/current/servers/mt-client-api',
+                    'method': 'GET',
+                    'headers': {'auth-token': self._token},
                 }
-            })
-            self._urlCache = {
-                'url': f'https://copyfactory-api-v1.{self._regionCache[self._regionIndex]}.{url_settings["domain"]}',
+            )
+            self._url_cache = {
+                'url': f'https://copyfactory-api-v1.{self._region_cache[self._region_index]}.{url_settings["domain"]}',
                 'domain': url_settings['domain'],
-                'lastUpdated': datetime.now().timestamp()
+                'lastUpdated': datetime.now().timestamp(),
             }
         else:
-            self._urlCache = {
-                'url': f'https://copyfactory-api-v1.{self._regionCache[self._regionIndex]}.{self._urlCache["domain"]}',
-                'domain': self._urlCache['domain'],
-                'lastUpdated': datetime.now().timestamp()
+            self._url_cache = {
+                'url': f'https://copyfactory-api-v1.'
+                f'{self._region_cache[self._region_index]}.'
+                f'{self._url_cache["domain"]}',
+                'domain': self._url_cache['domain'],
+                'lastUpdated': datetime.now().timestamp(),
             }
 
     async def _update_regions(self):
-        self._regionIndex = 0
-        self._regionCache = await self._httpClient.request({
-            'url': f'https://mt-provisioning-api-v1.{self._domain}/users/current/regions',
-            'method': 'GET',
-            'headers': {
-                'auth-token': self._token
-            },
-        })
+        self._region_index = 0
+        self._region_cache = await self._http_client.request(
+            {
+                'url': f'https://mt-provisioning-api-v1.{self._domain}/users/current/regions',
+                'method': 'GET',
+                'headers': {'auth-token': self._token},
+            }
+        )
 
     async def _update_account_regions(self, host: dict, account_id: str):
         if host['lastUpdated'] < datetime.now().timestamp() - 60 * 10:
             account_data = await self.get_account_info(account_id)
             host['lastUpdated'] = datetime.now().timestamp()
             host['regions'] = account_data['regions']
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/domain_client_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/domain_client_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from .httpClient import HttpClient
-from .domain_client import DomainClient
-from mock import AsyncMock, ANY
+import asyncio
+import json
+from datetime import datetime
+
 import pytest
-from freezegun import freeze_time
 import respx
-import json
+from freezegun import freeze_time
 from httpx import Response
-from datetime import datetime
-import asyncio
+from mock import AsyncMock, ANY
+
+from .domain_client import DomainClient
+from .http_client import HttpClient
 
 http_client = HttpClient()
 domain_client = DomainClient(http_client, 'token')
 request_mock = AsyncMock()
 
 token = 'header.payload.sign'
 expected = [{'_id': 'ABCD'}]
@@ -19,91 +21,84 @@
 
 request_call: respx.Route
 regions_call: respx.Route
 host_call: respx.Route
 signal_vint_call: respx.Route
 signal_us_west_call: respx.Route
 get_account_call: respx.Route
-strategies_url = 'https://copyfactory-api-v1.vint-hill.agiliumtrade.agiliumtrade.ai/users/current/' +\
-                 'configuration/strategies'
+strategies_url = (
+    'https://copyfactory-api-v1.vint-hill.agiliumtrade.agiliumtrade.ai/users/current/' + 'configuration/strategies'
+)
 regions_url = 'https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/regions'
 host_url = 'https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/servers/mt-client-api'
-opts = {
-    'url': '/users/current/configuration/strategies',
-    'method': 'GET',
-    'headers': {
-        'auth-token': token
-    }
-}
+opts = {'url': '/users/current/configuration/strategies', 'method': 'GET', 'headers': {'auth-token': token}}
 host = {
     'host': 'https://copyfactory-api-v1',
     'lastUpdated': datetime.now().timestamp(),
     'regions': ['vint-hill'],
-    'domain': 'agiliumtrade.ai'
+    'domain': 'agiliumtrade.ai',
 }
-signal_opts = {
-    'url': '/users/current/subscribers/accountId/signals',
-    'method': 'GET',
-}
-expectedSignals = [{
-    'strategy': {'id': '1234', 'name': 'Test strategy'},
-    'positionId': '123456',
-    'time': '2021-11-19T18:56:32.590Z',
-    'symbol': 'GBPUSD',
-    'type': 'limit',
-    'side': 'buy',
-}]
+signal_opts = {'url': '/users/current/subscribers/accountId/signals', 'method': 'GET'}
+expectedSignals = [
+    {
+        'strategy': {'id': '1234', 'name': 'Test strategy'},
+        'positionId': '123456',
+        'time': '2021-11-19T18:56:32.590Z',
+        'symbol': 'GBPUSD',
+        'type': 'limit',
+        'side': 'buy',
+    }
+]
 expected_account = {'_id': 'accountId2', 'region': 'germany', 'accountReplicas': []}
 
 
 @pytest.fixture(autouse=True)
 async def run_around_tests():
     global http_client
     http_client = HttpClient()
     global domain_client
     domain_client = DomainClient(http_client, token)
 
     global request_call
     request_call = respx.get(strategies_url).mock(return_value=Response(200, content=json.dumps(expected)))
 
     global regions_call
-    regions_call = respx.get(regions_url)\
-        .mock(return_value=Response(200, content=json.dumps(['vint-hill', 'us-west'])))
+    regions_call = respx.get(regions_url).mock(return_value=Response(200, content=json.dumps(['vint-hill', 'us-west'])))
 
     global host_call
-    host_call = respx.get(host_url)\
-        .mock(return_value=Response(200, content=json.dumps({'domain': 'agiliumtrade.agiliumtrade.ai'})))
+    host_call = respx.get(host_url).mock(
+        return_value=Response(200, content=json.dumps({'domain': 'agiliumtrade.agiliumtrade.ai'}))
+    )
 
     global signal_vint_call
-    signal_vint_call = respx.get('https://copyfactory-api-v1.vint-hill.agiliumtrade.ai/users/current/subscribers/'
-                                 'accountId/signals')\
-        .mock(return_value=Response(200, content=json.dumps(expectedSignals)))
+    signal_vint_call = respx.get(
+        'https://copyfactory-api-v1.vint-hill.agiliumtrade.ai/users/current/subscribers/' 'accountId/signals'
+    ).mock(return_value=Response(200, content=json.dumps(expectedSignals)))
 
     global signal_us_west_call
-    signal_us_west_call = respx.get('https://copyfactory-api-v1.us-west.agiliumtrade.ai/users/current/subscribers/'
-                                    'accountId/signals')\
-        .mock(return_value=Response(500))
+    signal_us_west_call = respx.get(
+        'https://copyfactory-api-v1.us-west.agiliumtrade.ai/users/current/subscribers/' 'accountId/signals'
+    ).mock(return_value=Response(500))
 
     global get_account_call
-    get_account_call = respx.get('https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/'
-                                 'accounts/accountId')\
-        .mock(return_value=Response(200, content=json.dumps(expected_account)))
+    get_account_call = respx.get(
+        'https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/' 'accounts/accountId'
+    ).mock(return_value=Response(200, content=json.dumps(expected_account)))
 
     global host
     host = {
         'host': 'https://copyfactory-api-v1',
         'lastUpdated': datetime.now().timestamp(),
         'regions': ['vint-hill'],
-        'domain': 'agiliumtrade.ai'
+        'domain': 'agiliumtrade.ai',
     }
     yield
 
 
 class TestDomainClient:
-
     @respx.mock
     @pytest.mark.asyncio
     async def test_execute_request(self):
         """Should execute request."""
         response = await domain_client.request_copyfactory(opts)
         assert response == expected
 
@@ -163,45 +158,48 @@
             assert err.__class__.__name__ == 'ValidationException'
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_try_another_region_if_first_failed(self):
         """Should try another region if the first failed."""
         request_call.mock(return_value=Response(500))
-        us_west_call = respx.get('https://copyfactory-api-v1.us-west.agiliumtrade.agiliumtrade.ai/users/current/' +
-                                 'configuration/strategies')\
-            .mock(return_value=Response(200, content=json.dumps(expected)))
+        us_west_call = respx.get(
+            'https://copyfactory-api-v1.us-west.agiliumtrade.agiliumtrade.ai/users/current/'
+            + 'configuration/strategies'
+        ).mock(return_value=Response(200, content=json.dumps(expected)))
         response = await domain_client.request_copyfactory(opts)
         assert response == expected
         assert us_west_call.call_count == 1
         assert host_call.call_count == 1
         assert regions_call.call_count == 1
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_return_error_if_all_regions_failed(self):
         """Should return error if all regions failed."""
         request_call.mock(return_value=Response(500))
-        respx.get('https://copyfactory-api-v1.us-west.agiliumtrade.agiliumtrade.ai/users/current/' +
-                  'configuration/strategies') \
-            .mock(return_value=Response(500))
+        respx.get(
+            'https://copyfactory-api-v1.us-west.agiliumtrade.agiliumtrade.ai/users/current/'
+            + 'configuration/strategies'
+        ).mock(return_value=Response(500))
         try:
             await domain_client.request_copyfactory(opts)
             pytest.fail()
         except Exception as err:
             assert err.__class__.__name__ == 'InternalException'
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_roll_over_to_first_region_if_all_regions_failed(self):
         """Should roll over to the first region if all regions failed."""
         request_call.mock(return_value=Response(500))
-        respx.get('https://copyfactory-api-v1.us-west.agiliumtrade.agiliumtrade.ai/users/current/' +
-                  'configuration/strategies') \
-            .mock(return_value=Response(500))
+        respx.get(
+            'https://copyfactory-api-v1.us-west.agiliumtrade.agiliumtrade.ai/users/current/'
+            + 'configuration/strategies'
+        ).mock(return_value=Response(500))
         try:
             await domain_client.request_copyfactory(opts)
             pytest.fail()
         except Exception as err:
             assert err.__class__.__name__ == 'InternalException'
 
         request_call.mock(return_value=Response(200, content=json.dumps(expected)))
@@ -209,24 +207,22 @@
         assert response == expected
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_execute_normal_request(self):
         """Should execute request."""
         opts = {
-            'url':  'https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/accounts/accountId',
+            'url': 'https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/accounts/accountId',
             'method': 'GET',
-            'headers': {
-                'auth-token': token
-            },
+            'headers': {'auth-token': token},
         }
 
-        request_stub = respx.get('https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/'
-                                 'accounts/accountId') \
-            .mock(return_value=Response(200, content=json.dumps(expected)))
+        request_stub = respx.get(
+            'https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/' 'accounts/accountId'
+        ).mock(return_value=Response(200, content=json.dumps(expected)))
         response = await domain_client.request(opts)
         assert response == expected
         assert request_stub.call_count == 1
 
 
 class TestRequestSignal:
     @respx.mock
@@ -265,25 +261,34 @@
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_update_host_if_expired(self):
         """Should execute a request and update host if expired."""
         with freeze_time(start_time) as frozen_datetime:
             host['lastUpdated'] = datetime.now().timestamp()
-            signal_germany_call = respx.get('https://copyfactory-api-v1.germany.agiliumtrade.ai/users/current/'
-                                            'subscribers/accountId/signals')\
-                .mock(return_value=Response(200, content=json.dumps(expectedSignals)))
-
-            signal_france_call = respx.get('https://copyfactory-api-v1.france.agiliumtrade.ai/users/current/'
-                                           'subscribers/accountId/signals')\
-                .mock(return_value=Response(200, content=json.dumps([])))
-
-            get_account_call.mock(return_value=Response(200, content=json.dumps({
-                '_id': 'accountId', 'region': 'germany',
-                'accountReplicas': [{'_id': 'accountId2', 'region': 'france'}]})))
+            signal_germany_call = respx.get(
+                'https://copyfactory-api-v1.germany.agiliumtrade.ai/users/current/' 'subscribers/accountId/signals'
+            ).mock(return_value=Response(200, content=json.dumps(expectedSignals)))
+
+            signal_france_call = respx.get(
+                'https://copyfactory-api-v1.france.agiliumtrade.ai/users/current/' 'subscribers/accountId/signals'
+            ).mock(return_value=Response(200, content=json.dumps([])))
+
+            get_account_call.mock(
+                return_value=Response(
+                    200,
+                    content=json.dumps(
+                        {
+                            '_id': 'accountId',
+                            'region': 'germany',
+                            'accountReplicas': [{'_id': 'accountId2', 'region': 'france'}],
+                        }
+                    ),
+                )
+            )
 
             await domain_client.request_signal(signal_opts, host, 'accountId')
             await asyncio.sleep(0.05)
             assert get_account_call.call_count == 0
             assert signal_germany_call.call_count == 0
             assert signal_france_call.call_count == 0
             frozen_datetime.tick(610)
@@ -306,54 +311,59 @@
         account = await domain_client.get_account_info('accountId')
         assert account == {'id': 'accountId2', 'regions': ['germany']}
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_get_account_with_replicas(self):
         """Should get account with replicas."""
-        get_account_call.mock(return_value=Response(200, content=json.dumps({
-            '_id': 'accountId',
-            'region': 'vint-hill',
-            'accountReplicas': [
-                {
-                    '_id': 'accountId2',
-                    'region': 'us-west',
-                }
-            ]
-        })))
+        get_account_call.mock(
+            return_value=Response(
+                200,
+                content=json.dumps(
+                    {
+                        '_id': 'accountId',
+                        'region': 'vint-hill',
+                        'accountReplicas': [{'_id': 'accountId2', 'region': 'us-west'}],
+                    }
+                ),
+            )
+        )
         account = await domain_client.get_account_info('accountId')
         assert account == {'id': 'accountId', 'regions': ['vint-hill', 'us-west']}
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_get_primary_account_if_requested_is_replica(self):
         """Should get primary account if requested account is a replica."""
-        get_account_call.mock(return_value=Response(200, content=json.dumps({
-            '_id': 'accountId',
-            'region': 'vint-hill',
-            'primaryAccountId': 'accountId2'
-        })))
-        respx.get('https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/accounts/accountId2')\
-            .mock(return_value=Response(200, content=json.dumps({
-                '_id': 'accountId2', 'region': 'us-west', 'accountReplicas': [
+        get_account_call.mock(
+            return_value=Response(
+                200, content=json.dumps({'_id': 'accountId', 'region': 'vint-hill', 'primaryAccountId': 'accountId2'})
+            )
+        )
+        respx.get('https://mt-provisioning-api-v1.agiliumtrade.agiliumtrade.ai/users/current/accounts/accountId2').mock(
+            return_value=Response(
+                200,
+                content=json.dumps(
                     {
-                        '_id': 'accountId',
-                        'region': 'vint-hill',
+                        '_id': 'accountId2',
+                        'region': 'us-west',
+                        'accountReplicas': [{'_id': 'accountId', 'region': 'vint-hill'}],
                     }
-                ]
-            })))
+                ),
+            )
+        )
         account = await domain_client.get_account_info('accountId')
         assert account == {'id': 'accountId2', 'regions': ['us-west', 'vint-hill']}
 
 
 class TestGetSignalClientHost:
     @respx.mock
     @pytest.mark.asyncio
     async def test_return_signal_client_host(self):
         """Should return signal client host."""
         response = await domain_client.get_signal_client_host(['vint-hill'])
         assert response == {
             'host': 'https://copyfactory-api-v1',
             'lastUpdated': ANY,
             'regions': ['vint-hill'],
-            'domain': 'agiliumtrade.agiliumtrade.ai'
+            'domain': 'agiliumtrade.agiliumtrade.ai',
         }
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/errorHandler.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/error_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Tuple, List
+
 from typing_extensions import TypedDict
 
 
 class ApiException(Exception):
     """Base class for API exceptions. Contains indication of HTTP status.
 
     Attributes:
         status_code: HTTP status code.
         url: API request URL.
     """
 
     def __init__(self, message: str, status: int, url: str = None):
-        """Inits ApiException
+        """Initializes ApiException.
 
         Args:
             message: Exception message.
             status: HTTP status.
             url: API request URL.
         """
         super().__init__(f'{message}. Request URL: {url}' if url else message)
@@ -59,41 +60,41 @@
         self.args = args
 
 
 class NotFoundException(ApiException):
     """Throwing this exception results in 404 (Not Found) HTTP response code."""
 
     def __init__(self, message: str, url: str = None):
-        """Inits not found exception.
+        """Initializes not found exception.
 
         Args:
             message: Exception message.
             url: API request URL.
         """
         super().__init__(message, 404, url)
 
 
 class ForbiddenException(ApiException):
     """Throwing this exception results in 403 (Forbidden) HTTP response code."""
 
     def __init__(self, message: str, url: str = None):
-        """Inits forbidden exception.
+        """Initializes forbidden exception.
 
         Args:
             message: Exception message.
             url: API request URL.
         """
         super().__init__(message, 403, url)
 
 
 class UnauthorizedException(ApiException):
     """Throwing this exception results in 401 (Unauthorized) HTTP response code."""
 
     def __init__(self, message: str, url: str = None):
-        """Inits unauthorized exception.
+        """Initializes unauthorized exception.
 
         Args:
             message: Exception message.
             url: API request URL.
         """
         super().__init__(message, 401, url)
 
@@ -102,15 +103,15 @@
     """Represents validation exception. Throwing this exception results in 400 (Bad Request) HTTP response code.
 
     Attributes:
         _details: Validation exception details
     """
 
     def __init__(self, message: str, details: List[dict] = None, url: str = None):
-        """Inits validation error.
+        """Initializes validation error.
 
         Args:
             message: Exception message.
             details: Exception data.
             url: API request URL.
         """
         super().__init__(message + ', check error.details for more information', 400, url)
@@ -126,52 +127,53 @@
         return self._details
 
 
 class InternalException(ApiException):
     """Represents unexpected exception. Throwing this error results in 500 (Internal Error) HTTP response code."""
 
     def __init__(self, message: str, url: str = None):
-        """Inits unexpected exception.
+        """Initializes unexpected exception.
 
         Args:
             message: Exception message.
             url: API request URL.
         """
         super().__init__(message, 500, url)
 
 
 class ConflictException(ApiException):
     """Represents conflict exception. Throwing this exception results in 409 (Conflict) HTTP response code."""
 
     def __init__(self, message: str, url: str = None):
-        """Inits conflict exception.
+        """Initializes conflict exception.
 
         Args:
             message: Exception message.
             url: API request URL.
         """
         super().__init__(message, 409, url)
 
 
 class TooManyRequestsErrorMetadata(TypedDict):
     """Metadata for too many requests error."""
+
     periodInMinutes: float
     """Throttling period in minutes."""
     requestsPerPeriodAllowed: int
     """Available requests for periodInMinutes."""
     recommendedRetryTime: str
     """Recommended date to retry request."""
 
 
 class TooManyRequestsException(ApiException):
     """Represents too many requests error. Throwing this exception results in 429 (Too Many Requests) HTTP response
     code."""
 
     def __init__(self, message: str, metadata: TooManyRequestsErrorMetadata, url: str):
-        """Inits too many requests exception.
+        """Initializes too many requests exception.
 
         Args:
             message: Exception message.
             metadata: Error metadata.
             url: API request URL.
         """
         super().__init__(message, 429, url)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/httpClient.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/http_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,89 +1,101 @@
-from .errorHandler import UnauthorizedException, ForbiddenException, ApiException, ConflictException, \
-    ValidationException, InternalException, NotFoundException, TooManyRequestsException
-from typing_extensions import TypedDict
-from typing import Optional
-from ..models import ExceptionMessage, date
-from .timeoutException import TimeoutException
-import json
 import asyncio
+import json
 import sys
-import httpx
 from datetime import datetime
+from typing import Optional
+
+import httpx
 from httpx import HTTPError, Response
+from typing_extensions import TypedDict
 
+from .error_handler import (
+    UnauthorizedException,
+    ForbiddenException,
+    ApiException,
+    ConflictException,
+    ValidationException,
+    InternalException,
+    NotFoundException,
+    TooManyRequestsException,
+)
+from .timeout_exception import TimeoutException
+from ..models import ExceptionMessage, date
 
 if sys.version_info[0] == 3 and sys.version_info[1] >= 8 and sys.platform.startswith('win'):
     asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
 
 class RequestOptions(TypedDict):
     """Options for HttpClient requests."""
+
     timeout: float
     method: Optional[str]
     url: str
     headers: Optional[dict]
     params: Optional[dict]
     body: Optional[dict]
     files: Optional[dict]
 
 
 class HttpClient:
     """HTTP client library based on requests module."""
+
     def __init__(self, timeout: float = 10, extended_timeout: float = 70, retry_opts=None):
-        """Inits HttpClient class instance.
+        """Initializes HttpClient class instance.
 
         Args:
             timeout: Request timeout in seconds.
             extended_timeout: Extended request timeout in seconds.
             retry_opts: Retry options.
         """
         if retry_opts is None:
             retry_opts = {}
         self._timeout = timeout
-        self._extendedTimeout = extended_timeout
+        self._extended_timeout = extended_timeout
         self._retries = retry_opts['retries'] if 'retries' in retry_opts else 5
-        self._minRetryDelayInSeconds = retry_opts['minDelayInSeconds'] if 'minDelayInSeconds' in retry_opts else 1
-        self._maxRetryDelayInSeconds = retry_opts['maxDelayInSeconds'] if 'maxDelayInSeconds' in retry_opts else 30
+        self._min_retry_delay_in_seconds = retry_opts['minDelayInSeconds'] if 'minDelayInSeconds' in retry_opts else 1
+        self._max_retry_delay_in_seconds = retry_opts['maxDelayInSeconds'] if 'maxDelayInSeconds' in retry_opts else 30
 
     async def request(self, options: dict, is_extended_timeout: bool = False):
         """Performs a request. Response errors are returned as ApiError or subclasses.
 
         Args:
             options: Request options.
             is_extended_timeout: Whether to run the request with an extended timeout.
 
         Returns:
             Request result.
         """
-        options['timeout'] = self._extendedTimeout if is_extended_timeout else self._timeout
+        options['timeout'] = self._extended_timeout if is_extended_timeout else self._timeout
         try:
             response = await self._make_request(options)
             response.raise_for_status()
             if response.content:
                 try:
                     response = response.json()
                 except Exception as err:
                     print('Error parsing json', err)
         except HTTPError as err:
             raise self._convert_error(err)
         return response
 
-    async def request_with_failover(self, options: RequestOptions, retry_counter: int = 0, end_time: float = None) \
-            -> Response:
+    async def request_with_failover(
+        self, options: RequestOptions, retry_counter: int = 0, end_time: float = None
+    ) -> Response:
         """Performs a request. Response errors are returned as ApiException or subclasses.
 
         Args:
             options: Request options.
 
         Returns:
             A request response.
         """
         if not end_time:
-            end_time = datetime.now().timestamp() + self._maxRetryDelayInSeconds * self._retries
+            end_time = datetime.now().timestamp() + self._max_retry_delay_in_seconds * self._retries
         retry_after_seconds = 0
         try:
             response = await self._make_request(options)
             response.raise_for_status()
             if response.status_code == 202:
                 retry_after_seconds = response.headers['retry-after']
                 if isinstance(retry_after_seconds, str):
@@ -120,17 +132,19 @@
             raise TimeoutException('Timed out waiting for the response')
 
     async def _handle_error(self, err, retry_counter: int, end_time: float):
         if err.__class__.__name__ == 'ConnectTimeout':
             error = err
         else:
             error = self._convert_error(err)
-        if error.__class__.__name__ in ['ConflictException', 'InternalException', 'ApiException', 'ConnectTimeout'] \
-                and retry_counter < self._retries:
-            pause = min(pow(2, retry_counter) * self._minRetryDelayInSeconds, self._maxRetryDelayInSeconds)
+        if (
+            error.__class__.__name__ in ['ConflictException', 'InternalException', 'ApiException', 'ConnectTimeout']
+            and retry_counter < self._retries
+        ):
+            pause = min(pow(2, retry_counter) * self._min_retry_delay_in_seconds, self._max_retry_delay_in_seconds)
             await asyncio.sleep(pause)
             return retry_counter + 1
         elif error.__class__.__name__ == 'TooManyRequestsException':
             retry_time = date(error.metadata['recommendedRetryTime']).timestamp()
             if retry_time < end_time:
                 await asyncio.sleep(retry_time - datetime.now().timestamp())
                 return retry_counter
@@ -139,16 +153,19 @@
     def _convert_error(self, err: HTTPError):
         if err.__class__.__name__ == 'ConnectTimeout':
             return err
         try:
             response: ExceptionMessage or TypedDict = json.loads(err.response.text)
         except Exception:
             response = {}
-        err_message = response['message'] if 'message' in response else (
-            err.response.reason_phrase if hasattr(err, 'response') else None)
+        err_message = (
+            response['message']
+            if 'message' in response
+            else (err.response.reason_phrase if hasattr(err, 'response') else None)
+        )
         url = err.request.url
         status = None
         if hasattr(err, 'response'):
             status = err.response.status_code
         if status == 400:
             details = response['details'] if 'details' in response else []
             return ValidationException(err_message, details, url)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/httpClient_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/http_client_test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,112 +1,115 @@
-from .httpClient import HttpClient
+import json
 import re
+from datetime import datetime
+
 import pytest
 import respx
-from datetime import datetime
-import json
 from httpx import Response
+
+from .http_client import HttpClient
 from ..models import format_date
-httpClient: HttpClient = None
+
+http_client: HttpClient = None
 test_url = 'http://example.com'
 opts = {}
 
 
 @pytest.fixture(autouse=True)
 async def run_around_tests():
-    global httpClient
-    httpClient = HttpClient()
+    global http_client
+    http_client = HttpClient()
     global opts
     opts = {'url': test_url}
     yield
 
 
 class TestHttpClient:
     @pytest.mark.asyncio
     async def test_load(self):
         """Should load HTML page from example.com"""
-        response = await httpClient.request(opts)
+        response = await http_client.request(opts)
         text = response.text
         assert re.search('doctype html', text)
 
     @pytest.mark.asyncio
     async def test_load(self):
         """Should load HTML page from example.com with failover"""
-        response = await httpClient.request_with_failover(opts)
+        response = await http_client.request_with_failover(opts)
         text = response.text
         assert re.search('doctype html', text)
 
     @pytest.mark.asyncio
     async def test_not_found(self):
         """Should return NotFound exception if server returns 404"""
-        opts = {
-            'url': f'{test_url}/not-found'
-        }
+        opts = {'url': f'{test_url}/not-found'}
         try:
-            await httpClient.request_with_failover(opts)
+            await http_client.request_with_failover(opts)
             raise Exception('NotFoundException is expected')
         except Exception as err:
             assert err.__class__.__name__ == 'NotFoundException'
 
     @pytest.mark.asyncio
     async def test_timeout(self):
         """Should return ConnectTimeout exception if request is timed out"""
-        httpClient = HttpClient(0.001, 60, {'retries': 2, 'minDelayInSeconds': 0.05, 'maxDelayInSeconds': 0.2})
+        http_client = HttpClient(0.001, 60, {'retries': 2, 'minDelayInSeconds': 0.05, 'maxDelayInSeconds': 0.2})
         try:
-            await httpClient.request_with_failover(opts)
+            await http_client.request_with_failover(opts)
             raise Exception('ConnectTimeout is expected')
         except Exception as err:
             assert err.__class__.__name__ == 'ConnectTimeout'
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_retry_on_api_exception(self):
         """Should retry request on fail with ApiException exception."""
-        respx.get(test_url).mock(side_effect=[Response(502), Response(502),
-                                              Response(200, content=json.dumps('response'))])
-        response = await httpClient.request_with_failover(opts)
+        respx.get(test_url).mock(
+            side_effect=[Response(502), Response(502), Response(200, content=json.dumps('response'))]
+        )
+        response = await http_client.request_with_failover(opts)
         assert response == 'response'
         assert respx.get(test_url).call_count == 3
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_retry_on_internal_exception(self):
         """Should retry request on fail with InternalException exception."""
-        respx.get(test_url).mock(side_effect=[Response(500), Response(500),
-                                              Response(200, content=json.dumps('response'))])
-        response = await httpClient.request_with_failover(opts)
+        respx.get(test_url).mock(
+            side_effect=[Response(500), Response(500), Response(200, content=json.dumps('response'))]
+        )
+        response = await http_client.request_with_failover(opts)
         assert response == 'response'
         assert respx.get(test_url).call_count == 3
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_return_error_on_retry_limit_exceeded(self):
         """Should return error if retry limit exceeded."""
         respx.get(test_url).mock(side_effect=Response(502))
-        httpClient = HttpClient(10, 60, {'retries': 2})
+        http_client = HttpClient(10, 60, {'retries': 2})
         try:
-            await httpClient.request_with_failover(opts)
+            await http_client.request_with_failover(opts)
             raise Exception('ApiException is expected')
         except Exception as err:
             assert err.__class__.__name__ == 'ApiException'
         assert respx.get(test_url).call_count == 3
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_not_retry_if_exception_not_internal_exception_or_api_exception(self):
         """Should not retry if exception is neither InternalException nor ApiException."""
         error = {
             'id': 1,
             'error': 'error',
             'message': 'test',
-            'details': [{'parameter': 'password', 'value': 'wrong', 'message': 'Invalid value'}]
+            'details': [{'parameter': 'password', 'value': 'wrong', 'message': 'Invalid value'}],
         }
         respx.get(test_url).mock(side_effect=[Response(400, json=error), Response(400, json=error), Response(204)])
         try:
-            await httpClient.request_with_failover(opts)
+            await http_client.request_with_failover(opts)
             raise Exception('ValidationException is expected')
         except Exception as err:
             assert err.__class__.__name__ == 'ValidationException'
             assert err.__str__() == f'test, check error.details for more information. Request URL: {opts["url"]}'
             assert err.details == error['details']
         assert respx.get(test_url).call_count == 1
 
@@ -116,82 +119,101 @@
         recommended_retry_time = format_date(datetime.fromtimestamp(date))
         return Response(429, content=json.dumps({"metadata": {"recommendedRetryTime": recommended_retry_time}}))
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_retry_after_wait_on_too_many_requests_error(self):
         """Should retry request after waiting on fail with TooManyRequestsException error."""
-        respx.get(test_url).mock(side_effect=[self.get_too_many_requests_error(2),
-                                              self.get_too_many_requests_error(3),
-                                              Response(200, content=json.dumps('response'))])
-        response = await httpClient.request_with_failover(opts)
+        respx.get(test_url).mock(
+            side_effect=[
+                self.get_too_many_requests_error(2),
+                self.get_too_many_requests_error(3),
+                Response(200, content=json.dumps('response')),
+            ]
+        )
+        response = await http_client.request_with_failover(opts)
         assert response == 'response'
         assert respx.get(test_url).call_count == 3
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_return_error_if_recommended_time_too_long(self):
         """Should return error if recommended retry time is too long."""
-        respx.get(test_url).mock(side_effect=[self.get_too_many_requests_error(2),
-                                              self.get_too_many_requests_error(300),
-                                              Response(200, content=json.dumps('response'))])
+        respx.get(test_url).mock(
+            side_effect=[
+                self.get_too_many_requests_error(2),
+                self.get_too_many_requests_error(300),
+                Response(200, content=json.dumps('response')),
+            ]
+        )
         try:
-            await httpClient.request_with_failover(opts)
+            await http_client.request_with_failover(opts)
             raise Exception('TooManyRequestsException is expected')
         except Exception as err:
             assert err.__class__.__name__ == 'TooManyRequestsException'
         assert respx.get(test_url).call_count == 2
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_not_count_retrying_too_many_requests_exception(self):
         """Should not count retrying TooManyRequestsException error."""
-        respx.get(test_url).mock(side_effect=[self.get_too_many_requests_error(2), Response(502),
-                                              Response(200, content=json.dumps('response'))])
-        httpClient = HttpClient(10, 60, {'retries': 1})
-        response = await httpClient.request_with_failover(opts)
+        respx.get(test_url).mock(
+            side_effect=[
+                self.get_too_many_requests_error(2),
+                Response(502),
+                Response(200, content=json.dumps('response')),
+            ]
+        )
+        http_client = HttpClient(10, 60, {'retries': 1})
+        response = await http_client.request_with_failover(opts)
         assert response == 'response'
         assert respx.get(test_url).call_count == 3
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_wait_for_retry_after_header(self):
         """Should wait for the retry-after header time before retrying."""
-        httpClient = HttpClient()
-        respx.get(test_url).mock(side_effect=[
-            Response(202, headers={'retry-after': '3'}),
-            Response(202, headers={'retry-after': '3'}),
-            Response(200, content=json.dumps('response'))])
-        response = await httpClient.request_with_failover(opts)
+        http_client = HttpClient()
+        respx.get(test_url).mock(
+            side_effect=[
+                Response(202, headers={'retry-after': '3'}),
+                Response(202, headers={'retry-after': '3'}),
+                Response(200, content=json.dumps('response')),
+            ]
+        )
+        response = await http_client.request_with_failover(opts)
         assert response == 'response'
         assert respx.get(test_url).call_count == 3
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_return_error_if_retry_after_time_too_long(self):
         """Should return TimeoutException error if retry-after header time is too long."""
-        httpClient = HttpClient(10, 60, {'maxDelayInSeconds': 3})
-        respx.get(test_url).mock(side_effect=[
-            Response(202, headers={'retry-after': '30'}),
-            Response(202, headers={'retry-after': '30'}),
-            Response(200, content=json.dumps('response'))])
+        http_client = HttpClient(10, 60, {'maxDelayInSeconds': 3})
+        respx.get(test_url).mock(
+            side_effect=[
+                Response(202, headers={'retry-after': '30'}),
+                Response(202, headers={'retry-after': '30'}),
+                Response(200, content=json.dumps('response')),
+            ]
+        )
         try:
-            await httpClient.request_with_failover(opts)
+            await http_client.request_with_failover(opts)
             raise Exception('TimeoutException is expected')
         except Exception as err:
             assert err.__class__.__name__ == 'TimeoutException'
             assert err.args[0] == 'Timed out waiting for the response'
         assert respx.get(test_url).call_count == 1
 
     @respx.mock
     @pytest.mark.asyncio
     async def test_return_error_if_timed_out_to_retry(self):
         """Should return TimeoutException error if timed out to retry."""
         respx.get(test_url).mock(side_effect=Response(202, headers={'retry-after': '1'}))
-        httpClient = HttpClient(10, 60, {'maxDelayInSeconds': 2, 'retries': 3})
+        http_client = HttpClient(10, 60, {'maxDelayInSeconds': 2, 'retries': 3})
         try:
-            await httpClient.request_with_failover(opts)
+            await http_client.request_with_failover(opts)
             raise Exception('TimeoutException is expected')
         except Exception as err:
             assert err.__class__.__name__ == 'TimeoutException'
             assert err.args[0] == 'Timed out waiting for the response'
         assert respx.get(test_url).call_count == 6
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/metaApi_client.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/metaapi_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from .methodAccessException import MethodAccessException
 from .domain_client import DomainClient
+from .method_access_exception import MethodAccessException
 
 
 class MetaApiClient:
     """metaapi.cloud MetaTrader API client."""
 
     def __init__(self, domain_client: DomainClient):
-        """Inits MetaTrader API client instance.
+        """Initializes MetaTrader API client instance.
 
         Args:
             domain_client: Domain client.
         """
-        self._domainClient = domain_client
+        self._domain_client = domain_client
         self._token = domain_client.token
 
     @property
     def _token_type(self) -> str:
         """Returns type of current token.
 
         Returns:
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/metaApi_client_test.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/metaapi_client_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from .httpClient import HttpClient
-from .metaApi_client import MetaApiClient
-from mock import MagicMock
 import pytest
+from mock import MagicMock
+
+from .metaapi_client import MetaApiClient
+
 domain_client = MagicMock()
 api_client = MetaApiClient(domain_client)
 
 
 @pytest.fixture(autouse=True)
 async def run_around_tests():
     global domain_client
@@ -43,21 +44,27 @@
 
     @pytest.mark.asyncio
     async def test_handle_no_access_exception_with_account_token(self):
         """Should handle no access exception with account token."""
         try:
             api_client._handle_no_access_exception('methodName')
         except Exception as err:
-            assert err.__str__() == 'You can not invoke methodName method, because you have connected with account ' + \
-                   'access token. Please use API access token from https://app.metaapi.cloud/token page to invoke ' + \
-                   'this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke methodName method, because you have connected with account '
+                + 'access token. Please use API access token from https://app.metaapi.cloud/token page to invoke '
+                + 'this method.'
+            )
 
     @pytest.mark.asyncio
     async def test_handle_no_access_exception_with_api_token(self):
         """Should handle no access exception with api token."""
         domain_client.token = 'header.payload.sign'
         api_client = MetaApiClient(domain_client)
         try:
             api_client._handle_no_access_exception('methodName')
         except Exception as err:
-            assert err.__str__() == 'You can not invoke methodName method, because you have connected with API ' + \
-                'access token. Please use account access token to invoke this method.'
+            assert (
+                err.__str__()
+                == 'You can not invoke methodName method, because you have connected with API '
+                + 'access token. Please use account access token to invoke this method.'
+            )
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/clients/methodAccessException.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/clients/method_access_exception.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 class MethodAccessException(Exception):
     """Exception which indicates that user doesn't have access to a method."""
 
     def __init__(self, method_name: str, access_type: str = 'api'):
-        """Inits the method access exception.
+        """Initializes the method access exception.
 
         Args:
             method_name: Name of method.
             access_type: Type of method access.
         """
         if access_type == 'api':
-            error_message = f'You can not invoke {method_name} method, because you have connected with API ' + \
-                            'access token. Please use account access token to invoke this method.'
+            error_message = (
+                f'You can not invoke {method_name} method, because you have connected with API '
+                + 'access token. Please use account access token to invoke this method.'
+            )
         elif access_type == 'account':
-            error_message = f'You can not invoke {method_name} method, because you have connected with account ' + \
-                            'access token. Please use API access token from https://app.metaapi.cloud/token page ' + \
-                            'to invoke this method.'
+            error_message = (
+                f'You can not invoke {method_name} method, because you have connected with account '
+                + 'access token. Please use API access token from https://app.metaapi.cloud/token page '
+                + 'to invoke this method.'
+            )
         else:
             error_message = ''
         super().__init__(error_message)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/copyFactory.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/copyfactory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-from .clients.httpClient import HttpClient
-from .clients.domain_client import DomainClient
-from .clients.copyFactory.configuration_client import ConfigurationClient
-from .clients.copyFactory.history_client import HistoryClient
-from .clients.copyFactory.trading_client import TradingClient
-from typing_extensions import TypedDict
 from typing import Optional
+
+from typing_extensions import TypedDict
+
+from .clients.copyfactory.configuration_client import ConfigurationClient
+from .clients.copyfactory.history_client import HistoryClient
+from .clients.copyfactory.trading_client import TradingClient
+from .clients.domain_client import DomainClient
+from .clients.http_client import HttpClient
 from .logger import LoggerManager
 
 
 class RetryOpts(TypedDict):
     retries: Optional[int]
     """Maximum amount of request retries, default value is 5."""
     minDelayInSeconds: Optional[float]
     """Minimum delay in seconds until request retry, default value is 1."""
     maxDelayInSeconds: Optional[float]
     """Maximum delay in seconds until request retry, default value is 30."""
 
 
 class CopyFactoryOpts(TypedDict):
     """CopyFactory options"""
+
     domain: Optional[str]
     """Domain to connect to."""
     extendedTimeout: Optional[float]
     """Timeout for extended http requests in seconds."""
     requestTimeout: Optional[float]
     """Timeout for http requests in seconds."""
     retryOpts: Optional[RetryOpts]
     """Options for request retries."""
 
 
 class CopyFactory:
     """MetaApi CopyFactory copy trading API SDK"""
 
     def __init__(self, token: str, opts: CopyFactoryOpts = None):
-        """Inits CopyFactory class instance.
+        """Initializes CopyFactory class instance.
 
         Args:
             token: Authorization token.
             opts: Connection options.
         """
         opts: CopyFactoryOpts = opts or {}
         domain = opts['domain'] if 'domain' in opts else 'agiliumtrade.agiliumtrade.ai'
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/logger.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
+from datetime import datetime
 from logging import Logger
 from typing import Callable
-from datetime import datetime
+
 logging_enabled = False
 
 
 class LoggerManager:
     """Manages loggers of the entire sdk."""
 
     @staticmethod
@@ -29,14 +30,15 @@
             logger = logging.getLogger(category)
             original_log = logger._log
 
             def logging_func(level, msg, args, exc_info=None, extra=None, stack_info=False, stacklevel=1):
                 if isinstance(msg, Callable):
                     msg = msg()
                 original_log(level, msg, args, exc_info, extra, stack_info, stacklevel)
+
             logger._log = logging_func
             return logger
         else:
             return NativeLogger(category)
 
 
 class NativeLogger(Logger):
@@ -54,12 +56,13 @@
 
     def error(self, msg, *args, **kwargs):
         self._log('error', msg, args)
 
     def exception(self, msg, *args, **kwargs):
         self._log('error', msg, args)
 
-    def _log(self, level: str, msg, args, exc_info=None, extra=None, stack_info: bool = None,
-             stacklevel: int = None) -> None:
+    def _log(
+        self, level: str, msg, args, exc_info=None, extra=None, stack_info: bool = None, stacklevel: int = None
+    ) -> None:
         if isinstance(msg, Callable):
             msg = msg()
         print(f'[{datetime.now().isoformat()}] {msg}', *args)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/lib/models.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/lib/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import asyncio
+import random
+import string
 from datetime import datetime
-from typing_extensions import TypedDict
 from typing import List, Optional
+
 import iso8601
-import random
-import string
 import pytz
-import asyncio
+from typing_extensions import TypedDict
 
 
 def date(date_time: str or float or int or datetime) -> datetime:
     """Parses a date string into a datetime object."""
     if isinstance(date_time, float) or isinstance(date_time, int):
         return datetime.fromtimestamp(max(date_time, 100000)).astimezone(pytz.utc)
     elif isinstance(date_time, datetime):
@@ -24,29 +25,31 @@
         return date_object.astimezone(pytz.utc).isoformat(timespec='milliseconds').replace('+00:00', 'Z')
     else:
         return date_object
 
 
 def random_id(length: int = 32) -> str:
     """Generates a random id of 32 symbols."""
-    return ''.join(random.choice(string.ascii_lowercase) for i in range(length))
+    return ''.join(random.choice(string.ascii_lowercase) for _ in range(length))
 
 
 class ValidationDetails(TypedDict):
     """Object to supply additional information for validation exceptions."""
+
     parameter: str
     """Name of invalid parameter."""
     value: Optional[str]
     """Entered invalid value."""
     message: str
     """Error message."""
 
 
 class ExceptionMessage(TypedDict):
     """A REST API response that contains an exception message"""
+
     id: int
     """Error id"""
     error: str
     """Error name"""
     numericCode: Optional[int]
     """Numeric error code"""
     stringCode: Optional[str]
@@ -57,20 +60,26 @@
     """Additional information about error. Used to supply validation error details."""
 
 
 def convert_iso_time_to_date(data):
     """Converts time fields of incoming data into datetime."""
     if not isinstance(data, str):
         for field in data:
-            if isinstance(data,  dict):
+            if isinstance(data, dict):
                 value = data[field]
             else:
                 value = field
-            if isinstance(value, str) and field in ['closeAfter', 'stoppedAt', 'stoppedTill', 'startTime', 'time',
-                                                    'updateTime']:
+            if isinstance(value, str) and field in [
+                'closeAfter',
+                'stoppedAt',
+                'stoppedTill',
+                'startTime',
+                'time',
+                'updateTime',
+            ]:
                 data[field] = date(value)
             if isinstance(value, list):
                 for item in value:
                     convert_iso_time_to_date(item)
             if isinstance(value, dict):
                 convert_iso_time_to_date(value)
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO` & `metaapi_cloud_copyfactory_sdk-9.0.1/metaapi_cloud_copyfactory_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: metaapi-cloud-copyfactory-sdk
-Version: 8.0.0
+Version: 9.0.1
 Summary: Python SDK for SDK for CopyFactory trade copying API. Can copy trades both between MetaTrader 5 (MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)
 Home-page: https://github.com/metaapi/metaapi-copyfactory-python-sdk
 Author: MetaApi DMCC
 Author-email: support@metaapi.cloud
 License: SEE LICENSE IN LICENSE
 Keywords: metaapi.cloud,MetaTrader,MetaTrader 5,MetaTrader 4,MetaTrader5,MetaTrader4,MT,MT4,MT5,forex,copy trading,API,REST,client,sdk,cloud
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 CopyFactory trade copying API for Python (a member of `metaapi.cloud <https://metaapi.cloud>`_ project)
 #######################################################################################################
 
 CopyFactory is a powerful trade copying API which makes developing forex
```

### Comparing `metaapi_cloud_copyfactory_sdk-8.0.0/setup.py` & `metaapi_cloud_copyfactory_sdk-9.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
-install_requires = ['aiohttp==3.7.4', 'typing-extensions>=4,<5', 'iso8601', 'pytz', 'requests==2.24.0', 'httpx==0.23.0']
+install_requires = [
+    'aiohttp==3.7.4',
+    'typing-extensions>=4.0.0',
+    'iso8601',
+    'pytz',
+    'requests>=2.28.0',
+    'httpx==0.23.0',
+]
 
 tests_require = [
     'pytest==6.2.5',
     'pytest-mock',
     'pytest-asyncio==0.16.0',
     'asynctest',
     'aiohttp',
     'mock',
     'freezegun==1.0.0',
     'respx==0.19.2',
 ]
 
 setuptools.setup(
     name="metaapi_cloud_copyfactory_sdk",
-    version="8.0.0",
+    version="9.0.1",
     author="MetaApi DMCC",
     author_email="support@metaapi.cloud",
     description="Python SDK for SDK for CopyFactory trade copying API. Can copy trades both between MetaTrader 5 "
     "(MT5) and MetaTrader 4 (MT4). (https://metaapi.cloud)",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     keywords=[
@@ -51,9 +58,9 @@
     tests_require=tests_require,
     license='SEE LICENSE IN LICENSE',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
 )
```

