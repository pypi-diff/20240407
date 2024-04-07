# Comparing `tmp/stock-open-api-1.0.1.tar.gz` & `tmp/stock-open-api-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/stock-open-api-1.0.1.tar", last modified: Wed Apr  3 07:06:51 2024, max compression
+gzip compressed data, was "dist/stock-open-api-1.0.2.tar", last modified: Sun Apr  7 02:20:45 2024, max compression
```

## Comparing `stock-open-api-1.0.1.tar` & `stock-open-api-1.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/
--rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/requirements/production.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     3181 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/api/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/api/bse/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/bse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/company.py
--rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/company_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/hk_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/hk_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/kcb_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/kcb_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/neeq_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/neeq_stock_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/sz_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/us_chinese_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/eastmoney/us_chinese_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/api/ipo3/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/ipo3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/ipo3/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/ipo3/neeq_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/api/jqka/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/jqka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/jqka/company.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/api/sse/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/sse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/sse/sh_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/sse/sh_stock_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/api/szse/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/szse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/api/szse/sz_stock.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/items/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/items/list_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/convert_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/excel_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/iterator_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/json_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/request_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/table_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/time_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/utils/ua_util.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 07:06:42.000000 stock-open-api-1.0.1/stock_open_api/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-04-03 07:06:50.000000 stock-open-api-1.0.1/stock_open_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-03 07:06:51.000000 stock-open-api-1.0.1/stock_open_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:06:50.000000 stock-open-api-1.0.1/stock_open_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 07:06:50.000000 stock-open-api-1.0.1/stock_open_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 07:06:50.000000 stock-open-api-1.0.1/stock_open_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:06:50.000000 stock-open-api-1.0.1/stock_open_api.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      414 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/requirements/production.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3181 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/api/bse/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/bse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4293 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/company_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/hk_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3402 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/hk_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8179 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/kcb_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/kcb_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/neeq_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/neeq_stock_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5385 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/sz_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/us_chinese_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/eastmoney/us_chinese_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/api/ipo3/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/ipo3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/ipo3/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/ipo3/neeq_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/api/jqka/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/jqka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/jqka/company.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/api/sse/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/sse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/sse/sh_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/sse/sh_stock_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/api/szse/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/szse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/api/szse/sz_stock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/items/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/items/list_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/convert_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/excel_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/iterator_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/json_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/request_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/table_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/time_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/utils/ua_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-07 02:20:31.000000 stock-open-api-1.0.2/stock_open_api/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8690 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 02:20:45.000000 stock-open-api-1.0.2/stock_open_api.egg-info/zip-safe
```

### Comparing `stock-open-api-1.0.1/PKG-INFO` & `stock-open-api-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-1.0.1/README.md` & `stock-open-api-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/setup.py` & `stock-open-api-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/company.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/company.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/company_config.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/company_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/hk_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/hk_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/hk_stock_config.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/hk_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/kcb_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/kcb_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/kcb_stock_config.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/kcb_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/neeq_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/neeq_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/neeq_stock_config.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/neeq_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/sh_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/sz_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/sz_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/us_chinese_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/us_chinese_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/eastmoney/us_chinese_stock_config.py` & `stock-open-api-1.0.2/stock_open_api/api/eastmoney/us_chinese_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/ipo3/config.py` & `stock-open-api-1.0.2/stock_open_api/api/ipo3/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 @File    : config.py
 @Date    : 2024-04-03
 """
 
 COMPANY_INFO_KEY_MAP = {
     "股票名称": "stock_name",
     "股票代码": "stock_code",
+    "最新价": "last_price",
+    "涨跌额": "change_value",
+    "涨跌幅": "change_rate",
     "所属行业": "industry",
     "今开": "open_price",
     "最高": "high_price",
     "平均价": "average_price",
     "市盈率": "pe_ratio",
     "成交量": "volume",
     "总市值": "total_market_value",
```

### Comparing `stock-open-api-1.0.1/stock_open_api/api/ipo3/neeq_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/ipo3/neeq_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/jqka/company.py` & `stock-open-api-1.0.2/stock_open_api/api/jqka/company.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/sse/sh_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/sse/sh_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/sse/sh_stock_config.py` & `stock-open-api-1.0.2/stock_open_api/api/sse/sh_stock_config.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/api/szse/sz_stock.py` & `stock-open-api-1.0.2/stock_open_api/api/szse/sz_stock.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/utils/convert_util.py` & `stock-open-api-1.0.2/stock_open_api/utils/convert_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/utils/excel_util.py` & `stock-open-api-1.0.2/stock_open_api/utils/excel_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/utils/request_util.py` & `stock-open-api-1.0.2/stock_open_api/utils/request_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api/utils/table_util.py` & `stock-open-api-1.0.2/stock_open_api/utils/table_util.py`

 * *Files identical despite different names*

### Comparing `stock-open-api-1.0.1/stock_open_api.egg-info/PKG-INFO` & `stock-open-api-1.0.2/stock_open_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stock-open-api
-Version: 1.0.1
+Version: 1.0.2
 Summary: a api collection for stock
 Home-page: https://github.com/mouday/stock-open-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
 Description: # Stock Open Api
```

### Comparing `stock-open-api-1.0.1/stock_open_api.egg-info/SOURCES.txt` & `stock-open-api-1.0.2/stock_open_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

