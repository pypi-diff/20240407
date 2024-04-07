# Comparing `tmp/sqllineage-1.5.1.tar.gz` & `tmp/sqllineage-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqllineage-1.5.1.tar", last modified: Sun Feb  4 14:03:48 2024, max compression
+gzip compressed data, was "sqllineage-1.5.2.tar", last modified: Sun Apr  7 13:04:55 2024, max compression
```

## Comparing `sqllineage-1.5.1.tar` & `sqllineage-1.5.2.tar`

### file list

```diff
@@ -1,281 +1,284 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.034114 sqllineage-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-02-04 14:02:19.000000 sqllineage-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-04 14:02:19.000000 sqllineage-1.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-02-04 14:03:48.034114 sqllineage-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-02-04 14:02:19.000000 sqllineage-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-04 14:03:48.034114 sqllineage-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-02-04 14:02:19.000000 sqllineage-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.962115 sqllineage-1.5.1/sqllineage/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.966115 sqllineage-1.5.1/sqllineage/build/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)   145386 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/editor.worker.js
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/editor.worker.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   637125 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/editor.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-02-04 14:02:48.000000 sqllineage-1.5.1/sqllineage/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-02-04 14:02:48.000000 sqllineage-1.5.1/sqllineage/build/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-02-04 14:02:48.000000 sqllineage-1.5.1/sqllineage/build/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-04 14:02:48.000000 sqllineage-1.5.1/sqllineage/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-04 14:02:48.000000 sqllineage-1.5.1/sqllineage/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.958115 sqllineage-1.5.1/sqllineage/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.966115 sqllineage-1.5.1/sqllineage/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    69444 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/css/main.c1b86fee.css
--rw-r--r--   0 runner    (1001) docker     (127)   146886 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/css/main.c1b86fee.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.974115 sqllineage-1.5.1/sqllineage/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/js/333.97bcedbd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    45386 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/js/333.97bcedbd.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)  3568960 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/js/main.a990fd89.js
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/js/main.a990fd89.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127) 13448212 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/js/main.a990fd89.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.990115 sqllineage-1.5.1/sqllineage/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    62792 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.990115 sqllineage-1.5.1/sqllineage/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18989 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/holders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.990115 sqllineage-1.5.1/sqllineage/core/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/metadata/dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/metadata/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.990115 sqllineage-1.5.1/sqllineage/core/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.990115 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4402 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.994115 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/create_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/cte.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/noop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/rename.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    10494 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.994115 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.994115 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/cte.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/core/parser/sqlparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.962115 sqllineage-1.5.1/sqllineage/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.014115 sqllineage-1.5.1/sqllineage/data/tpcds/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query01.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query02.sql
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query03.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query04.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query05.sql
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query06.sql
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query07.sql
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query08.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query09.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query10.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query11.sql
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query12.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query13.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query14.sql
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query15.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query16.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query17.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query18.sql
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query19.sql
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query20.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query21.sql
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query22.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query23.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query24.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query25.sql
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query26.sql
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query27.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query28.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query29.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query30.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query31.sql
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query32.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query33.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query34.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query35.sql
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query36.sql
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query37.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query38.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query39.sql
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query40.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query41.sql
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query42.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query43.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query44.sql
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query45.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query46.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query47.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query48.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query49.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query50.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query51.sql
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query52.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query53.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query54.sql
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query55.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query56.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query57.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query58.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query59.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query60.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query61.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query62.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query63.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query64.sql
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query65.sql
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query66.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query67.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query68.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query69.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query70.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query71.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query72.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query73.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query74.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query75.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query76.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query77.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query78.sql
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query79.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query80.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query81.sql
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query82.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query83.sql
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query84.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query85.sql
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query86.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query87.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query88.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query89.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query90.sql
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query91.sql
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query92.sql
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query93.sql
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query94.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query95.sql
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query96.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query97.sql
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query98.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/data/tpcds/query99.sql
--rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.014115 sqllineage-1.5.1/sqllineage/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/utils/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineage/utils/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.030115 sqllineage-1.5.1/sqllineage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9106 2024-02-04 14:03:47.000000 sqllineage-1.5.1/sqllineage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-04 14:03:46.000000 sqllineage-1.5.1/sqllineage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.018115 sqllineage-1.5.1/sqllineagejs/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/config-overrides.js
--rw-r--r--   0 runner    (1001) docker     (127)  1282472 2024-02-04 14:02:46.000000 sqllineage-1.5.1/sqllineagejs/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.018115 sqllineage-1.5.1/sqllineagejs/public/
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/public/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/public/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.018115 sqllineage-1.5.1/sqllineagejs/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/App.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.018115 sqllineage-1.5.1/sqllineagejs/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/api/client.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.018115 sqllineage-1.5.1/sqllineagejs/src/app/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/app/store.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.962115 sqllineage-1.5.1/sqllineagejs/src/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.022115 sqllineage-1.5.1/sqllineagejs/src/features/directory/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/directory/Directory.js
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/directory/DirectoryTreeItem.js
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/directory/directorySlice.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.022115 sqllineage-1.5.1/sqllineagejs/src/features/editor/
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/editor/DAG.js
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/editor/DAGDesc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/editor/Editor.js
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/editor/editorSlice.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.022115 sqllineage-1.5.1/sqllineagejs/src/features/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/widget/LoadError.js
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/features/widget/Loading.js
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-02-04 14:02:19.000000 sqllineage-1.5.1/sqllineagejs/src/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:47.962115 sqllineage-1.5.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.022115 sqllineage-1.5.1/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_metadata_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/core/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.022115 sqllineage-1.5.1/tests/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.026115 sqllineage-1.5.1/tests/sql/column/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_case_when.py
--rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_cast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_column.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_column_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_column_specified_in_dml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_from_cte.py
--rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_from_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_from_subquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    14167 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_lateral_alias_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_select_union.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_column_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_metadata_unqualified_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/column/test_metadata_wildcard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.030115 sqllineage-1.5.1/tests/sql/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-04 14:03:48.030115 sqllineage-1.5.1/tests/sql/table/multiple_statements/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/multiple_statements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/multiple_statements/test_split.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/multiple_statements/test_tmp_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/multiple_statements/test_tsql_no_semicolon.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/multiple_statements/test_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_create_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_cte.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_cte_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_insert_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_merge_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_other_with_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_other_with_lineage_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_other_without_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_other_without_lineage_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_path_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_select_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-04 14:02:19.000000 sqllineage-1.5.1/tests/sql/table/test_update_dialect_specific.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.582532 sqllineage-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-04-07 13:03:17.000000 sqllineage-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-07 13:03:17.000000 sqllineage-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-07 13:04:55.582532 sqllineage-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8432 2024-04-07 13:03:17.000000 sqllineage-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 13:04:55.582532 sqllineage-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3230 2024-04-07 13:03:17.000000 sqllineage-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.514531 sqllineage-1.5.2/sqllineage/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.518531 sqllineage-1.5.2/sqllineage/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)   145386 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/editor.worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/editor.worker.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   637125 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/editor.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-07 13:03:55.000000 sqllineage-1.5.2/sqllineage/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-07 13:03:55.000000 sqllineage-1.5.2/sqllineage/build/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-07 13:03:55.000000 sqllineage-1.5.2/sqllineage/build/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 13:03:55.000000 sqllineage-1.5.2/sqllineage/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 13:03:55.000000 sqllineage-1.5.2/sqllineage/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.510532 sqllineage-1.5.2/sqllineage/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.518531 sqllineage-1.5.2/sqllineage/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    69444 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/css/main.c1b86fee.css
+-rw-r--r--   0 runner    (1001) docker     (127)   146886 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/css/main.c1b86fee.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.526532 sqllineage-1.5.2/sqllineage/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/js/333.97bcedbd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45386 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/js/333.97bcedbd.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)  3568960 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/js/main.a990fd89.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/js/main.a990fd89.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 13448212 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/js/main.a990fd89.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.542532 sqllineage-1.5.2/sqllineage/build/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    62792 2024-04-07 13:04:53.000000 sqllineage-1.5.2/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3438 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.542532 sqllineage-1.5.2/sqllineage/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18989 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/holders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.542532 sqllineage-1.5.2/sqllineage/core/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/metadata/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/metadata/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7135 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.542532 sqllineage-1.5.2/sqllineage/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     4498 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.542532 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.546532 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/create_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/cte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6466 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/noop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/rename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8598 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.546532 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11900 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.546532 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/cte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/swap_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7769 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/core/parser/sqlparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.510532 sqllineage-1.5.2/sqllineage/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.566532 sqllineage-1.5.2/sqllineage/data/tpcds/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query01.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query02.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query03.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query04.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query05.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query06.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query07.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query08.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query09.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query10.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query11.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query12.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query13.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query14.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query15.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query16.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query17.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query18.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query19.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query20.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query21.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query22.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query23.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query24.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query25.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query26.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query27.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query28.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query29.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query30.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query31.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query32.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query33.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query34.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query35.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query36.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query37.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query38.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query39.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query40.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query41.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query42.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query43.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query44.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query45.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query46.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query47.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query48.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query49.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query50.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query51.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query52.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query53.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query54.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query55.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query56.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query57.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query58.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query59.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query60.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query61.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query62.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query63.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query64.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query65.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query66.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query67.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query68.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query69.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query70.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query71.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query72.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query73.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query74.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query75.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query76.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query77.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query78.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query79.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query80.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query81.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query82.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query83.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query84.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query85.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query86.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query87.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query88.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query89.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query90.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query91.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query92.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query93.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query94.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query95.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query96.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query97.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query98.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/data/tpcds/query99.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8341 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.566532 sqllineage-1.5.2/sqllineage/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/utils/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineage/utils/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.582532 sqllineage-1.5.2/sqllineage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10043 2024-04-07 13:04:54.000000 sqllineage-1.5.2/sqllineage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9217 2024-04-07 13:04:55.000000 sqllineage-1.5.2/sqllineage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:04:54.000000 sqllineage-1.5.2/sqllineage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 13:04:54.000000 sqllineage-1.5.2/sqllineage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-07 13:04:54.000000 sqllineage-1.5.2/sqllineage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 13:04:54.000000 sqllineage-1.5.2/sqllineage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.566532 sqllineage-1.5.2/sqllineagejs/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/config-overrides.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1282598 2024-04-07 13:03:53.000000 sqllineage-1.5.2/sqllineagejs/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.570531 sqllineage-1.5.2/sqllineagejs/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/public/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/public/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.570531 sqllineage-1.5.2/sqllineagejs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9090 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/App.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.570531 sqllineage-1.5.2/sqllineagejs/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/api/client.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.570531 sqllineage-1.5.2/sqllineagejs/src/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/app/store.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.510532 sqllineage-1.5.2/sqllineagejs/src/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.570531 sqllineage-1.5.2/sqllineagejs/src/features/directory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/directory/Directory.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/directory/DirectoryTreeItem.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/directory/directorySlice.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.570531 sqllineage-1.5.2/sqllineagejs/src/features/editor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/editor/DAG.js
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/editor/DAGDesc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/editor/Editor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/editor/editorSlice.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.570531 sqllineage-1.5.2/sqllineagejs/src/features/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/widget/LoadError.js
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/features/widget/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-07 13:03:17.000000 sqllineage-1.5.2/sqllineagejs/src/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.514531 sqllineage-1.5.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.574531 sqllineage-1.5.2/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_metadata_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/core/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.574531 sqllineage-1.5.2/tests/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.578532 sqllineage-1.5.2/tests/sql/column/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.578532 sqllineage-1.5.2/tests/sql/column/multiple_statements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/multiple_statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/multiple_statements/test_session_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_case_when.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4166 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_cast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_column_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_column_specified_in_dml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_from_cte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4345 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_from_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_from_subquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14192 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_lateral_alias_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_select_union.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_column_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_metadata_unqualified_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9574 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/column/test_metadata_wildcard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.578532 sqllineage-1.5.2/tests/sql/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:04:55.582532 sqllineage-1.5.2/tests/sql/table/multiple_statements/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/multiple_statements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/multiple_statements/test_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/multiple_statements/test_tmp_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/multiple_statements/test_tsql_no_semicolon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/multiple_statements/test_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_create_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_cte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_cte_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_insert_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_merge_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_other_with_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_other_with_lineage_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_other_without_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_other_without_lineage_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_path_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_select_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-07 13:03:17.000000 sqllineage-1.5.2/tests/sql/table/test_update_dialect_specific.py
```

### Comparing `sqllineage-1.5.1/LICENSE` & `sqllineage-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/PKG-INFO` & `sqllineage-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqllineage
-Version: 1.5.1
+Version: 1.5.2
 Summary: SQL Lineage Analysis Tool powered by Python
 Home-page: https://github.com/reata/sqllineage
 Author: Reata
 Author-email: reddevil.hjw@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlparse==0.4.4
 Requires-Dist: networkx>=2.4
-Requires-Dist: sqlfluff==2.3.5
+Requires-Dist: sqlfluff==3.0.3
 Requires-Dist: sqlalchemy>=2.0.0
 Provides-Extra: ci
 Requires-Dist: bandit; extra == "ci"
 Requires-Dist: black; extra == "ci"
 Requires-Dist: flake8; extra == "ci"
 Requires-Dist: flake8-blind-except; extra == "ci"
 Requires-Dist: flake8-builtins; extra == "ci"
```

### Comparing `sqllineage-1.5.1/README.md` & `sqllineage-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/setup.py` & `sqllineage-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     python_requires=">=3.8",
     install_requires=[
         "sqlparse==0.4.4",
         "networkx>=2.4",
-        "sqlfluff==2.3.5",
+        "sqlfluff==3.0.3",
         "sqlalchemy>=2.0.0",
     ],
     entry_points={"console_scripts": ["sqllineage = sqllineage.cli:main"]},
     extras_require={
         "ci": [
             "bandit",
             "black",
```

### Comparing `sqllineage-1.5.1/sqllineage/build/asset-manifest.json` & `sqllineage-1.5.2/sqllineage/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/editor.worker.js` & `sqllineage-1.5.2/sqllineage/build/editor.worker.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/editor.worker.js.map` & `sqllineage-1.5.2/sqllineage/build/editor.worker.js.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/favicon.ico` & `sqllineage-1.5.2/sqllineage/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/index.html` & `sqllineage-1.5.2/sqllineage/build/index.html`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/logo192.png` & `sqllineage-1.5.2/sqllineage/build/logo192.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/logo512.png` & `sqllineage-1.5.2/sqllineage/build/logo512.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/css/main.c1b86fee.css` & `sqllineage-1.5.2/sqllineage/build/static/css/main.c1b86fee.css`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/css/main.c1b86fee.css.map` & `sqllineage-1.5.2/sqllineage/build/static/css/main.c1b86fee.css.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/js/333.97bcedbd.chunk.js` & `sqllineage-1.5.2/sqllineage/build/static/js/333.97bcedbd.chunk.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/js/333.97bcedbd.chunk.js.map` & `sqllineage-1.5.2/sqllineage/build/static/js/333.97bcedbd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/js/main.a990fd89.js` & `sqllineage-1.5.2/sqllineage/build/static/js/main.a990fd89.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/js/main.a990fd89.js.LICENSE.txt` & `sqllineage-1.5.2/sqllineage/build/static/js/main.a990fd89.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/js/main.a990fd89.js.map` & `sqllineage-1.5.2/sqllineage/build/static/js/main.a990fd89.js.map`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf` & `sqllineage-1.5.2/sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/cli.py` & `sqllineage-1.5.2/sqllineage/cli.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/analyzer.py` & `sqllineage-1.5.2/sqllineage/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/holders.py` & `sqllineage-1.5.2/sqllineage/core/holders.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/metadata/dummy.py` & `sqllineage-1.5.2/sqllineage/core/metadata/dummy.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/metadata/sqlalchemy.py` & `sqllineage-1.5.2/sqllineage/core/metadata/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/metadata_provider.py` & `sqllineage-1.5.2/sqllineage/core/metadata_provider.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/models.py` & `sqllineage-1.5.2/sqllineage/core/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,36 +8,40 @@
 
 class Schema:
     """
     Data Class for Schema
     """
 
     unknown = "<default>"
-    default = SQLLineageConfig.DEFAULT_SCHEMA or unknown
 
-    def __init__(self, name: str = default):
+    def __init__(self, name: Optional[str] = None):
         """
         :param name: schema name
         """
-        self.raw_name = escape_identifier_name(name)
+        if name:
+            self.raw_name = escape_identifier_name(name)
+        elif SQLLineageConfig.DEFAULT_SCHEMA:
+            self.raw_name = escape_identifier_name(SQLLineageConfig.DEFAULT_SCHEMA)
+        else:
+            self.raw_name = escape_identifier_name(Schema.unknown)
 
     def __str__(self):
         return self.raw_name
 
     def __repr__(self):
         return "Schema: " + str(self)
 
     def __eq__(self, other):
         return isinstance(other, Schema) and str(self) == str(other)
 
     def __hash__(self):
         return hash(str(self))
 
     def __bool__(self):
-        return str(self) != self.default
+        return str(self) != self.unknown
 
 
 class Table:
     """
     Data Class for Table
     """
```

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/__init__.py` & `sqllineage-1.5.2/sqllineage/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/analyzer.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 import warnings
 from typing import Dict, List
 
-from sqlfluff.core import Linter, SQLLexError, SQLParseError, dialect_readout
+from sqlfluff.core import (
+    FluffConfig,
+    Linter,
+    SQLLexError,
+    SQLParseError,
+    dialect_readout,
+)
 from sqlfluff.core.parser import BaseSegment
 
 from sqllineage.core.analyzer import LineageAnalyzer
 from sqllineage.core.holders import StatementLineageHolder
 from sqllineage.core.metadata_provider import MetaDataProvider
 from sqllineage.core.parser.sqlfluff.extractors.base import BaseExtractor
 from sqllineage.exceptions import (
@@ -69,15 +75,17 @@
                 else:
                     raise UnsupportedStatementException(
                         f"SQLLineage doesn't support analyzing statement type [{statement_segment.type}] for SQL:"
                         f"{sql}"
                     )
 
     def _list_specific_statement_segment(self, sql: str):
-        parsed = Linter(dialect=self._dialect).parse_string(sql)
+        parsed = Linter(
+            config=FluffConfig.from_root(overrides={"dialect": self._dialect})
+        ).parse_string(sql)
         violations = [
             str(e)
             for e in parsed.violations
             if isinstance(e, (SQLLexError, SQLParseError))
         ]
         if violations:
             violation_msg = "\n".join(violations)
```

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/base.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
                 if sq.query.get_child("with_compound_statement")
                 else SelectExtractor
             )
             subquery_holder = extractor_cls(
                 self.dialect, self.metadata_provider
             ).extract(sq.query, AnalyzerContext(cte=holder.cte, write={sq}))
             # remove WRITE tag from subquery so that the combined holder won't have multiple WRITE dataset
-            nx.set_node_attributes(subquery_holder.graph, {sq, False}, NodeTag.WRITE)
+            nx.set_node_attributes(subquery_holder.graph, {sq: False}, NodeTag.WRITE)
             holder |= subquery_holder
 
     @staticmethod
     def _init_holder(context: AnalyzerContext) -> SubQueryLineageHolder:
         """
         Initialize lineage holder for a given 'AnalyzerContext'
         :param context: a previous context that the lineage extractor must consider
```

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/copy.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/copy.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/create_insert.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/create_insert.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/cte.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/cte.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/drop.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/drop.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/merge.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/merge.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/noop.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/noop.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/rename.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/rename.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/select.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/select.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/extractors/update.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/extractors/update.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/models.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/models.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlfluff/utils.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlfluff/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -55,28 +55,20 @@
 
 def find_from_expression_element(segment: BaseSegment) -> Optional[BaseSegment]:
     """
     segment can be of type:
         from_clause as grandparent
         from_expression/join_clause as parent
     """
-    from_expression_element = None
-    if segment.type in ["from_clause", "update_statement"]:
-        if from_expression := segment.get_child("from_expression"):
-            non_bracket = from_expression
-            while bracketed := non_bracket.get_child("bracketed"):
-                non_bracket = bracketed
-            if seg := non_bracket.get_child("from_expression_element"):
-                from_expression_element = seg
-            elif seg := non_bracket.get_child("from_expression"):
-                if sub_seg := seg.get_child("from_expression_element"):
-                    from_expression_element = sub_seg
-    elif segment.type in ("from_expression", "join_clause"):
-        if seg := segment.get_child("from_expression_element"):
-            from_expression_element = seg
+    try:
+        from_expression_element = next(
+            segment.recursive_crawl("from_expression_element")
+        )
+    except StopIteration:
+        from_expression_element = None
     return from_expression_element
 
 
 def find_table_identifier(segment: BaseSegment) -> Optional[BaseSegment]:
     """
     recursively find table identifier
     """
@@ -90,22 +82,16 @@
     return table_identifier
 
 
 def list_join_clause(segment: BaseSegment) -> List[BaseSegment]:
     """
     traverse from_clause, recursively goes into bracket by default
     """
-    if from_expression := segment.get_child("from_expression"):
-        if bracketed := from_expression.get_child("bracketed"):
-            join_clauses = bracketed.get_children("join_clause")
-            if inner_bracket := bracketed.get_child("bracketed"):
-                join_clauses = list_join_clause(inner_bracket) + join_clauses
-            return join_clauses
-        else:
-            return from_expression.get_children("join_clause")
+    if segment.type in ["from_clause", "update_statement"]:
+        return list(segment.recursive_crawl("join_clause"))
     return []
 
 
 def list_expression_from_when_clause(
     when_clause: BaseSegment, sub_type: str
 ) -> List[BaseSegment]:
     """
```

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/__init__.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/__init__.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/analyzer.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/analyzer.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/base.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/base.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/cte.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/cte.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/source.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/source.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/swap_partition.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/swap_partition.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/handlers/target.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/handlers/target.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/models.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/models.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/core/parser/sqlparse/utils.py` & `sqllineage-1.5.2/sqllineage/core/parser/sqlparse/utils.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query01.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query01.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query02.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query02.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query04.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query04.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query05.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query05.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query06.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query06.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query07.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query07.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query08.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query08.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query09.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query09.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query10.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query10.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query11.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query11.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query12.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query12.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query13.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query13.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query14.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query14.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query15.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query15.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query16.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query16.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query17.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query17.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query18.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query18.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query19.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query19.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query20.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query20.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query21.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query21.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query23.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query23.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query24.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query24.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query25.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query25.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query26.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query26.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query27.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query27.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query28.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query28.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query29.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query29.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query30.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query30.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query31.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query31.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query32.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query32.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query33.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query33.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query34.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query34.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query35.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query35.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query36.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query36.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query37.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query37.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query38.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query38.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query39.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query39.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query40.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query40.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query41.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query41.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query42.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query42.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query43.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query43.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query44.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query44.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query45.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query45.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query46.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query46.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query47.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query47.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query48.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query48.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query49.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query49.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query50.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query50.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query51.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query51.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query53.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query53.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query54.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query54.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query56.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query56.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query57.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query57.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query58.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query58.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query59.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query59.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query60.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query60.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query61.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query61.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query62.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query62.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query63.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query63.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query64.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query64.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query65.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query65.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query66.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query66.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query67.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query67.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query68.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query68.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query69.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query69.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query70.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query70.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query71.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query71.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query72.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query72.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query73.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query73.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query74.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query74.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query75.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query75.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query76.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query76.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query77.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query77.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query78.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query78.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query79.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query79.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query80.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query80.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query81.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query81.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query82.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query82.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query83.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query83.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query84.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query84.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query85.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query85.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query86.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query86.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query87.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query87.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query88.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query88.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query89.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query89.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query90.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query90.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query91.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query91.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query92.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query92.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query93.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query93.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query94.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query94.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query95.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query95.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query97.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query97.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query98.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query98.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/data/tpcds/query99.sql` & `sqllineage-1.5.2/sqllineage/data/tpcds/query99.sql`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/drawing.py` & `sqllineage-1.5.2/sqllineage/drawing.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/io.py` & `sqllineage-1.5.2/sqllineage/io.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/runner.py` & `sqllineage-1.5.2/sqllineage/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -195,18 +195,18 @@
 
         with self._metadata_provider.session() as session:
             stmt_holders = []
             for stmt in self._stmt:
                 stmt_holder = analyzer.analyze(stmt, session.metadata_provider)
                 if write := stmt_holder.write:
                     tgt_table = next(iter(write))
-                    if isinstance(tgt_table, Table):
-                        session.register_session_metadata(
-                            tgt_table, stmt_holder.get_table_columns(tgt_table)
-                        )
+                    if isinstance(tgt_table, Table) and (
+                        tgt_columns := stmt_holder.get_table_columns(tgt_table)
+                    ):
+                        session.register_session_metadata(tgt_table, tgt_columns)
                 stmt_holders.append(stmt_holder)
             self._stmt_holders = stmt_holders
             self._sql_holder = SQLLineageHolder.of(
                 session.metadata_provider, *self._stmt_holders
             )
         self._evaluated = True
```

### Comparing `sqllineage-1.5.1/sqllineage/utils/entities.py` & `sqllineage-1.5.2/sqllineage/utils/entities.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage/utils/helpers.py` & `sqllineage-1.5.2/sqllineage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineage.egg-info/PKG-INFO` & `sqllineage-1.5.2/sqllineage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqllineage
-Version: 1.5.1
+Version: 1.5.2
 Summary: SQL Lineage Analysis Tool powered by Python
 Home-page: https://github.com/reata/sqllineage
 Author: Reata
 Author-email: reddevil.hjw@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sqlparse==0.4.4
 Requires-Dist: networkx>=2.4
-Requires-Dist: sqlfluff==2.3.5
+Requires-Dist: sqlfluff==3.0.3
 Requires-Dist: sqlalchemy>=2.0.0
 Provides-Extra: ci
 Requires-Dist: bandit; extra == "ci"
 Requires-Dist: black; extra == "ci"
 Requires-Dist: flake8; extra == "ci"
 Requires-Dist: flake8-blind-except; extra == "ci"
 Requires-Dist: flake8-builtins; extra == "ci"
```

### Comparing `sqllineage-1.5.1/sqllineage.egg-info/SOURCES.txt` & `sqllineage-1.5.2/sqllineage.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -217,14 +217,16 @@
 tests/sql/column/test_column_select_from_subquery.py
 tests/sql/column/test_column_select_function.py
 tests/sql/column/test_column_select_lateral_alias_ref.py
 tests/sql/column/test_column_select_union.py
 tests/sql/column/test_column_update.py
 tests/sql/column/test_metadata_unqualified_column.py
 tests/sql/column/test_metadata_wildcard.py
+tests/sql/column/multiple_statements/__init__.py
+tests/sql/column/multiple_statements/test_session_metadata.py
 tests/sql/table/__init__.py
 tests/sql/table/test_create.py
 tests/sql/table/test_create_dialect_specific.py
 tests/sql/table/test_cte.py
 tests/sql/table/test_cte_dialect_specific.py
 tests/sql/table/test_insert.py
 tests/sql/table/test_insert_dialect_specific.py
```

### Comparing `sqllineage-1.5.1/sqllineagejs/package-lock.json` & `sqllineage-1.5.2/sqllineagejs/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9164638300375145%*

 * *Differences: {"'dependencies'": "{'body-parser': {'version': '1.20.2', 'resolved': "*

 * *                   "'https://registry.npmjs.org/body-parser/-/body-parser-1.20.2.tgz', "*

 * *                   "'integrity': "*

 * *                   "'sha512-ml9pReCu3M61kGlqoTm2umSXTlRTuGTx0bfYj+uIUKKYycG5NtSbeetV3faSU6R7ajOPw0g/J1PvK4qNy7s5bA==', "*

 * *                   "'requires': {'content-type': '~1.0.5', 'raw-body': '2.5.2'}}, 'content-type': "*

 * *                   "{'version': '1.0.5', 'resolved': "*

 * *                   "'https://registry.np […]*

```diff
@@ -3915,31 +3915,31 @@
                     "dev": true,
                     "integrity": "sha512-Tpp60P6IUJDTuOq/5Z8cdskzJujfwqfOTkrwIwj7IRISpnkJnT6SyJ4PCPnGMoFjC9ddhal5KVIYtAt97ix05A==",
                     "resolved": "https://registry.npmjs.org/ms/-/ms-2.0.0.tgz",
                     "version": "2.0.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-jWi7abTbYwajOytWCQc37VulmWiRae5RyTpaCyDcS5/lMdtwSz5lOpDE67srw/HYe35f1z3fDQw+3txg7gNtWw==",
+            "integrity": "sha512-ml9pReCu3M61kGlqoTm2umSXTlRTuGTx0bfYj+uIUKKYycG5NtSbeetV3faSU6R7ajOPw0g/J1PvK4qNy7s5bA==",
             "requires": {
                 "bytes": "3.1.2",
-                "content-type": "~1.0.4",
+                "content-type": "~1.0.5",
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "destroy": "1.2.0",
                 "http-errors": "2.0.0",
                 "iconv-lite": "0.4.24",
                 "on-finished": "2.4.1",
                 "qs": "6.11.0",
-                "raw-body": "2.5.1",
+                "raw-body": "2.5.2",
                 "type-is": "~1.6.18",
                 "unpipe": "1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.20.1.tgz",
-            "version": "1.20.1"
+            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.20.2.tgz",
+            "version": "1.20.2"
         },
         "bonjour": {
             "dev": true,
             "integrity": "sha1-jokKGD2O6aI5OzhExpGkK897yfU=",
             "requires": {
                 "array-flatten": "^2.1.0",
                 "deep-equal": "^1.0.1",
@@ -4352,32 +4352,32 @@
                 "safe-buffer": "5.2.1"
             },
             "resolved": "https://registry.npmjs.org/content-disposition/-/content-disposition-0.5.4.tgz",
             "version": "0.5.4"
         },
         "content-type": {
             "dev": true,
-            "integrity": "sha512-hIP3EEPs8tB9AT1L+NUqtwOAps4mk2Zob89MWXMHjHWg9milF/j4osnnQLXBCBFBk/tvIG/tUc9mOUJiPBhPXA==",
-            "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.4.tgz",
-            "version": "1.0.4"
+            "integrity": "sha512-nTjqfcBFEipKdXCv4YDQWCfmcLZKm81ldF0pAopTvyrFGVbcR6P/VAAd5G7N+0tTr8QqiU0tFadD6FK4NtJwOA==",
+            "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.5.tgz",
+            "version": "1.0.5"
         },
         "convert-source-map": {
             "dev": true,
             "integrity": "sha512-4FJkXzKXEDB1snCFZlLP4gpC3JILicCpGbzG9f9G7tGqGCzETQ2hWPrcinA9oU4wtf2biUaEH5065UnMeR33oA==",
             "requires": {
                 "safe-buffer": "~5.1.1"
             },
             "resolved": "https://registry.npmjs.org/convert-source-map/-/convert-source-map-1.7.0.tgz",
             "version": "1.7.0"
         },
         "cookie": {
             "dev": true,
-            "integrity": "sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==",
-            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.5.0.tgz",
-            "version": "0.5.0"
+            "integrity": "sha512-U71cyTamuh1CRNCfpGY6to28lxvNwPG4Guz/EVjgf3Jmzv0vlDp1atT9eS5dDjMYHucpHbWns6Lwf3BKz6svdw==",
+            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.6.0.tgz",
+            "version": "0.6.0"
         },
         "cookie-signature": {
             "dev": true,
             "integrity": "sha1-4wOogrNCzD7oylE6eZmXNNqzriw=",
             "resolved": "https://registry.npmjs.org/cookie-signature/-/cookie-signature-1.0.6.tgz",
             "version": "1.0.6"
         },
@@ -5884,22 +5884,22 @@
                     "dev": true,
                     "integrity": "sha512-RwNA9Z/7PrK06rYLIzFMlaF+l73iwpzsqRIFgbMLbTcLD6cOao82TaWefPXQvB2fOC4AjuYSEndS7N/mTCbkdQ==",
                     "resolved": "https://registry.npmjs.org/statuses/-/statuses-2.0.1.tgz",
                     "version": "2.0.1"
                 }
             },
             "dev": true,
-            "integrity": "sha512-5/PsL6iGPdfQ/lKM1UuielYgv3BUoJfz1aUwU9vHZ+J7gyvwdQXFEBIEIaxeGf0GIcreATNyBExtalisDbuMqQ==",
+            "integrity": "sha512-5T6nhjsT+EOMzuck8JjBHARTHfMht0POzlA60WV2pMD3gyXw2LZnZ+ueGdNxG+0calOJcWKbpFcuzLZ91YWq9Q==",
             "requires": {
                 "accepts": "~1.3.8",
                 "array-flatten": "1.1.1",
-                "body-parser": "1.20.1",
+                "body-parser": "1.20.2",
                 "content-disposition": "0.5.4",
                 "content-type": "~1.0.4",
-                "cookie": "0.5.0",
+                "cookie": "0.6.0",
                 "cookie-signature": "1.0.6",
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "encodeurl": "~1.0.2",
                 "escape-html": "~1.0.3",
                 "etag": "~1.8.1",
                 "finalhandler": "1.2.0",
@@ -5918,16 +5918,16 @@
                 "serve-static": "1.15.0",
                 "setprototypeof": "1.2.0",
                 "statuses": "2.0.1",
                 "type-is": "~1.6.18",
                 "utils-merge": "1.0.1",
                 "vary": "~1.1.2"
             },
-            "resolved": "https://registry.npmjs.org/express/-/express-4.18.2.tgz",
-            "version": "4.18.2"
+            "resolved": "https://registry.npmjs.org/express/-/express-4.19.2.tgz",
+            "version": "4.19.2"
         },
         "fast-deep-equal": {
             "integrity": "sha512-f3qQ9oQy9j2AhBe/H9VC91wLmKBCCU/gDOnKNAYG5hswO7BLKj09Hc5HYNz9cGI++xlpDCIgDaitVs03ATR84Q==",
             "resolved": "https://registry.npmjs.org/fast-deep-equal/-/fast-deep-equal-3.1.3.tgz",
             "version": "3.1.3"
         },
         "fast-glob": {
@@ -6193,17 +6193,17 @@
             "dev": true,
             "integrity": "sha512-8/sOawo8tJ4QOBX8YlQBMxL8+RLZfxMQOif9o0KUKTNTjMYElWPE0r/m5VNFxTRd0NSw8qSy8dajrwX4RYI1Hw==",
             "resolved": "https://registry.npmjs.org/flatted/-/flatted-3.2.4.tgz",
             "version": "3.2.4"
         },
         "follow-redirects": {
             "dev": true,
-            "integrity": "sha512-Cr4D/5wlrb0z9dgERpUL3LrmPKVDsETIJhaCMeDfuFYcqa5bldGV6wBsAN6X/vxlXQtFBMrXdXxdL8CbDTGniw==",
-            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.4.tgz",
-            "version": "1.15.4"
+            "integrity": "sha512-wWN62YITEaOpSK584EZXJafH1AGpO8RVgElfkuXbTOrPX4fIfOyEpW/CsiNd8JdYrAoOvafRTOEnvsO++qCqFA==",
+            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.6.tgz",
+            "version": "1.15.6"
         },
         "for-each": {
             "dev": true,
             "integrity": "sha512-jqYfLp7mo9vIyQf8ykW2v7A+2N4QjeCeI5+Dz9XraiO1ign81wjiH7Fb9vSOWvQfNtmSa4H2RoQTrrXivdUZmw==",
             "requires": {
                 "is-callable": "^1.1.3"
             },
@@ -6371,17 +6371,17 @@
                 "universalify": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-10.0.0.tgz",
             "version": "10.0.0"
         },
         "fs-monkey": {
             "dev": true,
-            "integrity": "sha512-cybjIfiiE+pTWicSCLFHSrXZ6EilF30oh91FDP9S2B051prEa7QWfrVTQm10/dDpswBDXZugPa1Ogu8Yh+HV0Q==",
-            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.3.tgz",
-            "version": "1.0.3"
+            "integrity": "sha512-8uMbBjrhzW76TYgEV27Y5E//W2f/lTFmx78P2w19FZSxarhI/798APGQyuGCwmkNxgwGRhrLfvWyLBvNtuOmew==",
+            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.5.tgz",
+            "version": "1.0.5"
         },
         "fs.realpath": {
             "dev": true,
             "integrity": "sha1-FQStJSMVjKpA20onh8sBQRmU6k8=",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
@@ -7184,17 +7184,17 @@
                 "side-channel": "^1.0.4"
             },
             "resolved": "https://registry.npmjs.org/internal-slot/-/internal-slot-1.0.5.tgz",
             "version": "1.0.5"
         },
         "ip": {
             "dev": true,
-            "integrity": "sha1-vd7XARQpCCjAoDnnLvJfWq7ENUo=",
-            "resolved": "https://registry.npmjs.org/ip/-/ip-1.1.5.tgz",
-            "version": "1.1.5"
+            "integrity": "sha512-cyRxvOEpNHNtchU3Ln9KC/auJgup87llfQpQ+t5ghoC/UhL16SWzbueiCsdTnWmqAWl7LadfuwhlqmtOaqMHdQ==",
+            "resolved": "https://registry.npmjs.org/ip/-/ip-1.1.9.tgz",
+            "version": "1.1.9"
         },
         "ipaddr.js": {
             "dev": true,
             "integrity": "sha512-1qTgH9NG+IIJ4yfKs2e6Pp1bZg8wbDbKHT21HrLIeYBTRLgMYKnMTPAuI3Lcs61nfx5h1xlXnbJtH1kX5/d/ng==",
             "resolved": "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-2.0.1.tgz",
             "version": "2.0.1"
         },
@@ -9551,20 +9551,20 @@
             "dev": true,
             "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
             "version": "0.3.0"
         },
         "memfs": {
             "dev": true,
-            "integrity": "sha512-1c9VPVvW5P7I85c35zAdEr1TD5+F11IToIHIlrVIcflfnzPkJa0ZoYEoEdYDP8KgPFoSZ/opDrUsAoZWym3mtw==",
+            "integrity": "sha512-UERzLsxzllchadvbPs5aolHh65ISpKpM+ccLbOJ8/vvpBKmAWf+la7dXFy7Mr0ySHbdHrFv5kGFCUHHe6GFEmw==",
             "requires": {
-                "fs-monkey": "1.0.3"
+                "fs-monkey": "^1.0.4"
             },
-            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.4.1.tgz",
-            "version": "3.4.1"
+            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.3.tgz",
+            "version": "3.5.3"
         },
         "merge-descriptors": {
             "dev": true,
             "integrity": "sha1-sAqqVW3YtEVoFQ7J0blT8/kMu2E=",
             "resolved": "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz",
             "version": "1.0.1"
         },
@@ -11226,23 +11226,23 @@
                         "safer-buffer": ">= 2.1.2 < 3"
                     },
                     "resolved": "https://registry.npmjs.org/iconv-lite/-/iconv-lite-0.4.24.tgz",
                     "version": "0.4.24"
                 }
             },
             "dev": true,
-            "integrity": "sha512-qqJBtEyVgS0ZmPGdCFPWJ3FreoqvG4MVQln/kCgF7Olq95IbOp0/BWyMwbdtn4VTvkM8Y7khCQ2Xgk/tcrCXig==",
+            "integrity": "sha512-8zGqypfENjCIqGhgXToC8aB2r7YrBX+AQAfIPs/Mlk+BtPTztOvTS01NRW/3Eh60J+a48lt8qsCzirQ6loCVfA==",
             "requires": {
                 "bytes": "3.1.2",
                 "http-errors": "2.0.0",
                 "iconv-lite": "0.4.24",
                 "unpipe": "1.0.0"
             },
-            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.5.1.tgz",
-            "version": "2.5.1"
+            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.5.2.tgz",
+            "version": "2.5.2"
         },
         "react": {
             "integrity": "sha512-lG9c9UuMHdcAexXtigOZLX8exLWkW0Ku29qPRU8uhF2R9BN96dLCt0psvzPLlHc5OWkgymP3qwTRgbnw5BKx3w==",
             "requires": {
                 "loose-envify": "^1.1.0",
                 "object-assign": "^4.1.1"
             },
@@ -13261,24 +13261,24 @@
                         "ajv-keywords": "^5.0.0"
                     },
                     "resolved": "https://registry.npmjs.org/schema-utils/-/schema-utils-4.0.0.tgz",
                     "version": "4.0.0"
                 }
             },
             "dev": true,
-            "integrity": "sha512-81EujCKkyles2wphtdrnPg/QqegC/AtqNH//mQkBYSMqwFVCQrxM6ktB2O/SPlZy7LqeEfTbV3cZARGQz6umhg==",
+            "integrity": "sha512-BVdTqhhs+0IfoeAf7EoH5WE+exCmqGerHfDM0IL096Px60Tq2Mn9MAbnaGUe6HiMa41KMCYF19gyzZmBcq/o4Q==",
             "requires": {
                 "colorette": "^2.0.10",
-                "memfs": "^3.4.1",
+                "memfs": "^3.4.3",
                 "mime-types": "^2.1.31",
                 "range-parser": "^1.2.1",
                 "schema-utils": "^4.0.0"
             },
-            "resolved": "https://registry.npmjs.org/webpack-dev-middleware/-/webpack-dev-middleware-5.3.1.tgz",
-            "version": "5.3.1"
+            "resolved": "https://registry.npmjs.org/webpack-dev-middleware/-/webpack-dev-middleware-5.3.4.tgz",
+            "version": "5.3.4"
         },
         "webpack-dev-server": {
             "dependencies": {
                 "ajv": {
                     "dev": true,
                     "integrity": "sha512-x9VuX+R/jcFj1DHo/fCp99esgGDWiHENrKxaCENuCxpoMCmAt/COCGVDwA7kleEpEzJjDnvh3yGoOuLu0Dtllw==",
                     "requires": {
@@ -13940,15 +13940,15 @@
             "devDependencies": {
                 "@babel/plugin-proposal-private-property-in-object": "^7.21.11",
                 "gh-pages": "^4.0.0",
                 "react-app-rewired": "^2.1.8",
                 "react-scripts": "^5.0.0"
             },
             "name": "sqllineagejs",
-            "version": "1.5.1"
+            "version": "1.5.2"
         },
         "node_modules/@aashutoshrathi/word-wrap": {
             "dev": true,
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-1Yjs2SvM8TflER/OD3cOjhWWOZb58A2t7wpE2S9XfBYTiIl+XFhQG2bjy4Pu1I+EAlCNUzRDYDdFwFYUKvXcIA==",
@@ -19317,34 +19317,34 @@
             "integrity": "sha512-XpNj6GDQzdfW+r2Wnn7xiSAd7TM3jzkxGXBGTtWKuSXv1xUV+azxAm8jdWZN06QTQk+2N2XB9jRDkvbmQmcRtg==",
             "resolved": "https://registry.npmjs.org/bluebird/-/bluebird-3.7.2.tgz",
             "version": "3.7.2"
         },
         "node_modules/body-parser": {
             "dependencies": {
                 "bytes": "3.1.2",
-                "content-type": "~1.0.4",
+                "content-type": "~1.0.5",
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "destroy": "1.2.0",
                 "http-errors": "2.0.0",
                 "iconv-lite": "0.4.24",
                 "on-finished": "2.4.1",
                 "qs": "6.11.0",
-                "raw-body": "2.5.1",
+                "raw-body": "2.5.2",
                 "type-is": "~1.6.18",
                 "unpipe": "1.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.8",
                 "npm": "1.2.8000 || >= 1.4.16"
             },
-            "integrity": "sha512-jWi7abTbYwajOytWCQc37VulmWiRae5RyTpaCyDcS5/lMdtwSz5lOpDE67srw/HYe35f1z3fDQw+3txg7gNtWw==",
-            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.20.1.tgz",
-            "version": "1.20.1"
+            "integrity": "sha512-ml9pReCu3M61kGlqoTm2umSXTlRTuGTx0bfYj+uIUKKYycG5NtSbeetV3faSU6R7ajOPw0g/J1PvK4qNy7s5bA==",
+            "resolved": "https://registry.npmjs.org/body-parser/-/body-parser-1.20.2.tgz",
+            "version": "1.20.2"
         },
         "node_modules/body-parser/node_modules/bytes": {
             "dev": true,
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-/Nf7TyzTx6S3yRJObOAV7956r8cr2+Oj8AC5dt8wSP3BQAoeX58NoHyCU8P8zGkNXStjTSi6fzO6F0pBdcYbEg==",
@@ -19935,17 +19935,17 @@
             "version": "5.2.1"
         },
         "node_modules/content-type": {
             "dev": true,
             "engines": {
                 "node": ">= 0.6"
             },
-            "integrity": "sha512-hIP3EEPs8tB9AT1L+NUqtwOAps4mk2Zob89MWXMHjHWg9milF/j4osnnQLXBCBFBk/tvIG/tUc9mOUJiPBhPXA==",
-            "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.4.tgz",
-            "version": "1.0.4"
+            "integrity": "sha512-nTjqfcBFEipKdXCv4YDQWCfmcLZKm81ldF0pAopTvyrFGVbcR6P/VAAd5G7N+0tTr8QqiU0tFadD6FK4NtJwOA==",
+            "resolved": "https://registry.npmjs.org/content-type/-/content-type-1.0.5.tgz",
+            "version": "1.0.5"
         },
         "node_modules/convert-source-map": {
             "dependencies": {
                 "safe-buffer": "~5.1.1"
             },
             "dev": true,
             "integrity": "sha512-4FJkXzKXEDB1snCFZlLP4gpC3JILicCpGbzG9f9G7tGqGCzETQ2hWPrcinA9oU4wtf2biUaEH5065UnMeR33oA==",
@@ -19953,17 +19953,17 @@
             "version": "1.7.0"
         },
         "node_modules/cookie": {
             "dev": true,
             "engines": {
                 "node": ">= 0.6"
             },
-            "integrity": "sha512-YZ3GUyn/o8gfKJlnlX7g7xq4gyO6OSuhGPKaaGssGB2qgDUS0gPgtTvoyZLTt9Ab6dC4hfc9dV5arkvc/OCmrw==",
-            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.5.0.tgz",
-            "version": "0.5.0"
+            "integrity": "sha512-U71cyTamuh1CRNCfpGY6to28lxvNwPG4Guz/EVjgf3Jmzv0vlDp1atT9eS5dDjMYHucpHbWns6Lwf3BKz6svdw==",
+            "resolved": "https://registry.npmjs.org/cookie/-/cookie-0.6.0.tgz",
+            "version": "0.6.0"
         },
         "node_modules/cookie-signature": {
             "dev": true,
             "integrity": "sha1-4wOogrNCzD7oylE6eZmXNNqzriw=",
             "resolved": "https://registry.npmjs.org/cookie-signature/-/cookie-signature-1.0.6.tgz",
             "version": "1.0.6"
         },
@@ -21916,18 +21916,18 @@
             "resolved": "https://registry.npmjs.org/expect/-/expect-27.5.1.tgz",
             "version": "27.5.1"
         },
         "node_modules/express": {
             "dependencies": {
                 "accepts": "~1.3.8",
                 "array-flatten": "1.1.1",
-                "body-parser": "1.20.1",
+                "body-parser": "1.20.2",
                 "content-disposition": "0.5.4",
                 "content-type": "~1.0.4",
-                "cookie": "0.5.0",
+                "cookie": "0.6.0",
                 "cookie-signature": "1.0.6",
                 "debug": "2.6.9",
                 "depd": "2.0.0",
                 "encodeurl": "~1.0.2",
                 "escape-html": "~1.0.3",
                 "etag": "~1.8.1",
                 "finalhandler": "1.2.0",
@@ -21950,17 +21950,17 @@
                 "utils-merge": "1.0.1",
                 "vary": "~1.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.10.0"
             },
-            "integrity": "sha512-5/PsL6iGPdfQ/lKM1UuielYgv3BUoJfz1aUwU9vHZ+J7gyvwdQXFEBIEIaxeGf0GIcreATNyBExtalisDbuMqQ==",
-            "resolved": "https://registry.npmjs.org/express/-/express-4.18.2.tgz",
-            "version": "4.18.2"
+            "integrity": "sha512-5T6nhjsT+EOMzuck8JjBHARTHfMht0POzlA60WV2pMD3gyXw2LZnZ+ueGdNxG+0calOJcWKbpFcuzLZ91YWq9Q==",
+            "resolved": "https://registry.npmjs.org/express/-/express-4.19.2.tgz",
+            "version": "4.19.2"
         },
         "node_modules/express/node_modules/array-flatten": {
             "dev": true,
             "integrity": "sha1-ml9pkFGx5wczKPKgCJaLZOopVdI=",
             "resolved": "https://registry.npmjs.org/array-flatten/-/array-flatten-1.1.1.tgz",
             "version": "1.1.1"
         },
@@ -22371,22 +22371,22 @@
             },
             "funding": [
                 {
                     "type": "individual",
                     "url": "https://github.com/sponsors/RubenVerborgh"
                 }
             ],
-            "integrity": "sha512-Cr4D/5wlrb0z9dgERpUL3LrmPKVDsETIJhaCMeDfuFYcqa5bldGV6wBsAN6X/vxlXQtFBMrXdXxdL8CbDTGniw==",
+            "integrity": "sha512-wWN62YITEaOpSK584EZXJafH1AGpO8RVgElfkuXbTOrPX4fIfOyEpW/CsiNd8JdYrAoOvafRTOEnvsO++qCqFA==",
             "peerDependenciesMeta": {
                 "debug": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.4.tgz",
-            "version": "1.15.4"
+            "resolved": "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.6.tgz",
+            "version": "1.15.6"
         },
         "node_modules/for-each": {
             "dependencies": {
                 "is-callable": "^1.1.3"
             },
             "dev": true,
             "integrity": "sha512-jqYfLp7mo9vIyQf8ykW2v7A+2N4QjeCeI5+Dz9XraiO1ign81wjiH7Fb9vSOWvQfNtmSa4H2RoQTrrXivdUZmw==",
@@ -22632,17 +22632,17 @@
             },
             "integrity": "sha512-C5owb14u9eJwizKGdchcDUQeFtlSHHthBk8pbX9Vc1PFZrLombudjDnNns88aYslCyF6IY5SUw3Roz6xShcEIQ==",
             "resolved": "https://registry.npmjs.org/fs-extra/-/fs-extra-10.0.0.tgz",
             "version": "10.0.0"
         },
         "node_modules/fs-monkey": {
             "dev": true,
-            "integrity": "sha512-cybjIfiiE+pTWicSCLFHSrXZ6EilF30oh91FDP9S2B051prEa7QWfrVTQm10/dDpswBDXZugPa1Ogu8Yh+HV0Q==",
-            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.3.tgz",
-            "version": "1.0.3"
+            "integrity": "sha512-8uMbBjrhzW76TYgEV27Y5E//W2f/lTFmx78P2w19FZSxarhI/798APGQyuGCwmkNxgwGRhrLfvWyLBvNtuOmew==",
+            "resolved": "https://registry.npmjs.org/fs-monkey/-/fs-monkey-1.0.5.tgz",
+            "version": "1.0.5"
         },
         "node_modules/fs.realpath": {
             "dev": true,
             "integrity": "sha1-FQStJSMVjKpA20onh8sBQRmU6k8=",
             "resolved": "https://registry.npmjs.org/fs.realpath/-/fs.realpath-1.0.0.tgz",
             "version": "1.0.0"
         },
@@ -23697,17 +23697,17 @@
             },
             "integrity": "sha512-Y+R5hJrzs52QCG2laLn4udYVnxsfny9CpOhNhUvk/SSSVyF6T27FzRbF0sroPidSu3X8oEAkOn2K804mjpt6UQ==",
             "resolved": "https://registry.npmjs.org/internal-slot/-/internal-slot-1.0.5.tgz",
             "version": "1.0.5"
         },
         "node_modules/ip": {
             "dev": true,
-            "integrity": "sha1-vd7XARQpCCjAoDnnLvJfWq7ENUo=",
-            "resolved": "https://registry.npmjs.org/ip/-/ip-1.1.5.tgz",
-            "version": "1.1.5"
+            "integrity": "sha512-cyRxvOEpNHNtchU3Ln9KC/auJgup87llfQpQ+t5ghoC/UhL16SWzbueiCsdTnWmqAWl7LadfuwhlqmtOaqMHdQ==",
+            "resolved": "https://registry.npmjs.org/ip/-/ip-1.1.9.tgz",
+            "version": "1.1.9"
         },
         "node_modules/ipaddr.js": {
             "dev": true,
             "engines": {
                 "node": ">= 10"
             },
             "integrity": "sha512-1qTgH9NG+IIJ4yfKs2e6Pp1bZg8wbDbKHT21HrLIeYBTRLgMYKnMTPAuI3Lcs61nfx5h1xlXnbJtH1kX5/d/ng==",
@@ -26849,23 +26849,23 @@
             },
             "integrity": "sha512-dq+qelQ9akHpcOl/gUVRTxVIOkAJ1wR3QAvb4RsVjS8oVoFjDGTc679wJYmUmknUF5HwMLOgb5O+a3KxfWapPQ==",
             "resolved": "https://registry.npmjs.org/media-typer/-/media-typer-0.3.0.tgz",
             "version": "0.3.0"
         },
         "node_modules/memfs": {
             "dependencies": {
-                "fs-monkey": "1.0.3"
+                "fs-monkey": "^1.0.4"
             },
             "dev": true,
             "engines": {
                 "node": ">= 4.0.0"
             },
-            "integrity": "sha512-1c9VPVvW5P7I85c35zAdEr1TD5+F11IToIHIlrVIcflfnzPkJa0ZoYEoEdYDP8KgPFoSZ/opDrUsAoZWym3mtw==",
-            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.4.1.tgz",
-            "version": "3.4.1"
+            "integrity": "sha512-UERzLsxzllchadvbPs5aolHh65ISpKpM+ccLbOJ8/vvpBKmAWf+la7dXFy7Mr0ySHbdHrFv5kGFCUHHe6GFEmw==",
+            "resolved": "https://registry.npmjs.org/memfs/-/memfs-3.5.3.tgz",
+            "version": "3.5.3"
         },
         "node_modules/merge-descriptors": {
             "dev": true,
             "integrity": "sha1-sAqqVW3YtEVoFQ7J0blT8/kMu2E=",
             "resolved": "https://registry.npmjs.org/merge-descriptors/-/merge-descriptors-1.0.1.tgz",
             "version": "1.0.1"
         },
@@ -29306,17 +29306,17 @@
                 "iconv-lite": "0.4.24",
                 "unpipe": "1.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.8"
             },
-            "integrity": "sha512-qqJBtEyVgS0ZmPGdCFPWJ3FreoqvG4MVQln/kCgF7Olq95IbOp0/BWyMwbdtn4VTvkM8Y7khCQ2Xgk/tcrCXig==",
-            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.5.1.tgz",
-            "version": "2.5.1"
+            "integrity": "sha512-8zGqypfENjCIqGhgXToC8aB2r7YrBX+AQAfIPs/Mlk+BtPTztOvTS01NRW/3Eh60J+a48lt8qsCzirQ6loCVfA==",
+            "resolved": "https://registry.npmjs.org/raw-body/-/raw-body-2.5.2.tgz",
+            "version": "2.5.2"
         },
         "node_modules/raw-body/node_modules/bytes": {
             "dev": true,
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-/Nf7TyzTx6S3yRJObOAV7956r8cr2+Oj8AC5dt8wSP3BQAoeX58NoHyCU8P8zGkNXStjTSi6fzO6F0pBdcYbEg==",
@@ -31947,33 +31947,33 @@
             },
             "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.76.1.tgz",
             "version": "5.76.1"
         },
         "node_modules/webpack-dev-middleware": {
             "dependencies": {
                 "colorette": "^2.0.10",
-                "memfs": "^3.4.1",
+                "memfs": "^3.4.3",
                 "mime-types": "^2.1.31",
                 "range-parser": "^1.2.1",
                 "schema-utils": "^4.0.0"
             },
             "dev": true,
             "engines": {
                 "node": ">= 12.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-81EujCKkyles2wphtdrnPg/QqegC/AtqNH//mQkBYSMqwFVCQrxM6ktB2O/SPlZy7LqeEfTbV3cZARGQz6umhg==",
+            "integrity": "sha512-BVdTqhhs+0IfoeAf7EoH5WE+exCmqGerHfDM0IL096Px60Tq2Mn9MAbnaGUe6HiMa41KMCYF19gyzZmBcq/o4Q==",
             "peerDependencies": {
                 "webpack": "^4.0.0 || ^5.0.0"
             },
-            "resolved": "https://registry.npmjs.org/webpack-dev-middleware/-/webpack-dev-middleware-5.3.1.tgz",
-            "version": "5.3.1"
+            "resolved": "https://registry.npmjs.org/webpack-dev-middleware/-/webpack-dev-middleware-5.3.4.tgz",
+            "version": "5.3.4"
         },
         "node_modules/webpack-dev-middleware/node_modules/ajv": {
             "dependencies": {
                 "fast-deep-equal": "^3.1.1",
                 "json-schema-traverse": "^1.0.0",
                 "require-from-string": "^2.0.2",
                 "uri-js": "^4.2.2"
@@ -32839,9 +32839,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "1.5.1"
+    "version": "1.5.2"
 }
```

### Comparing `sqllineage-1.5.1/sqllineagejs/package.json` & `sqllineage-1.5.2/sqllineagejs/package.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'1.5.2'"}*

```diff
@@ -43,9 +43,9 @@
     "private": true,
     "scripts": {
         "build": "react-app-rewired build",
         "deploy": "gh-pages -d build",
         "eject": "react-scripts eject",
         "start": "react-app-rewired start"
     },
-    "version": "1.5.1"
+    "version": "1.5.2"
 }
```

### Comparing `sqllineage-1.5.1/sqllineagejs/public/favicon.ico` & `sqllineage-1.5.2/sqllineagejs/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/public/index.html` & `sqllineage-1.5.2/sqllineagejs/public/index.html`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/public/logo192.png` & `sqllineage-1.5.2/sqllineagejs/public/logo192.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/public/logo512.png` & `sqllineage-1.5.2/sqllineagejs/public/logo512.png`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/App.js` & `sqllineage-1.5.2/sqllineagejs/src/App.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/api/client.js` & `sqllineage-1.5.2/sqllineagejs/src/api/client.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/directory/Directory.js` & `sqllineage-1.5.2/sqllineagejs/src/features/directory/Directory.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/directory/DirectoryTreeItem.js` & `sqllineage-1.5.2/sqllineagejs/src/features/directory/DirectoryTreeItem.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/directory/directorySlice.js` & `sqllineage-1.5.2/sqllineagejs/src/features/directory/directorySlice.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/editor/DAG.js` & `sqllineage-1.5.2/sqllineagejs/src/features/editor/DAG.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/editor/DAGDesc.js` & `sqllineage-1.5.2/sqllineagejs/src/features/editor/DAGDesc.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/editor/Editor.js` & `sqllineage-1.5.2/sqllineagejs/src/features/editor/Editor.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/editor/editorSlice.js` & `sqllineage-1.5.2/sqllineagejs/src/features/editor/editorSlice.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/widget/LoadError.js` & `sqllineage-1.5.2/sqllineagejs/src/features/widget/LoadError.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/features/widget/Loading.js` & `sqllineage-1.5.2/sqllineagejs/src/features/widget/Loading.js`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/sqllineagejs/src/index.css` & `sqllineage-1.5.2/sqllineagejs/src/index.css`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/core/test_cli.py` & `sqllineage-1.5.2/tests/core/test_cli.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/core/test_drawing.py` & `sqllineage-1.5.2/tests/core/test_drawing.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/core/test_exception.py` & `sqllineage-1.5.2/tests/core/test_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from unittest.mock import patch
 
 import pytest
 
 from sqllineage import SQLPARSE_DIALECT
 from sqllineage.exceptions import (
     InvalidSyntaxException,
@@ -52,14 +53,14 @@
         LineageRunner(
             """SELECT * FROM foo
 SELECT * FROM bar""",
             dialect="tsql",
         )._eval()
 
 
-@patch("os.environ", {"SQLLINEAGE_TSQL_NO_SEMICOLON": "TRUE"})
+@patch.dict(os.environ, {"SQLLINEAGE_TSQL_NO_SEMICOLON": "TRUE"})
 def test_user_warning_enable_tsql_no_semicolon_with_other_dialect():
     with pytest.warns(UserWarning):
         LineageRunner(
             """SELECT * FROM foo;
 SELECT * FROM bar""",
         )._eval()
```

### Comparing `sqllineage-1.5.1/tests/core/test_metadata_provider.py` & `sqllineage-1.5.2/tests/core/test_metadata_provider.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/core/test_models.py` & `sqllineage-1.5.2/tests/core/test_models.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_merge.py` & `sqllineage-1.5.2/tests/sql/column/test_column_merge.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_case_when.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_case_when.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_cast.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_cast.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_column.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_column.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_column_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_column_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_column_specified_in_dml.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_column_specified_in_dml.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_expression.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_expression.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_from_cte.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_from_cte.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_from_join.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_from_join.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_from_subquery.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_from_subquery.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_function.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_function.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_lateral_alias_ref.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_lateral_alias_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from unittest.mock import patch
 
 import pytest
 
 from sqllineage.core.metadata_provider import MetaDataProvider
 from sqllineage.utils.entities import ColumnQualifierTuple
 from ...helpers import assert_column_lineage_equal, generate_metadata_providers
@@ -10,15 +11,15 @@
     {
         "public.src_tbl1": ["id", "a", "b", "c"],
     }
 )
 
 
 @pytest.mark.parametrize("provider", providers)
-@patch("os.environ", {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
+@patch.dict(os.environ, {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
 def test_column_top_level_enable_lateral_ref(
     provider: MetaDataProvider,
 ):
     sql = """
     insert into public.tgt_tbl1
     select
         name               as user_name,
@@ -102,15 +103,15 @@
         ],
         test_sqlparse=False,
         metadata_provider=provider,
     )
 
 
 @pytest.mark.parametrize("provider", providers)
-@patch("os.environ", {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
+@patch.dict(os.environ, {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
 def test_column_top_level_enable_lateral_ref_with_metadata_from_table(
     provider: MetaDataProvider,
 ):
     sql = """
     insert into public.tgt_tbl1
     select
         a || b || c || id as id,
@@ -144,15 +145,15 @@
         ],
         test_sqlparse=False,
         metadata_provider=provider,
     )
 
 
 @pytest.mark.parametrize("provider", providers)
-@patch("os.environ", {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
+@patch.dict(os.environ, {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
 def test_column_top_level_enable_lateral_ref_with_metadata_from_subquery(
     provider: MetaDataProvider,
 ):
     sql = """
     insert into public.tgt_tbl1
     select
         a || b || c || id as id,
@@ -191,15 +192,15 @@
         ],
         test_sqlparse=False,
         metadata_provider=provider,
     )
 
 
 @pytest.mark.parametrize("provider", providers)
-@patch("os.environ", {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
+@patch.dict(os.environ, {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
 def test_column_top_level_enable_lateral_ref_with_metadata_from_nested_subquery(
     provider: MetaDataProvider,
 ):
     sql = """
     insert into public.tgt_tbl1
     select
         a || b || c || id as id,
@@ -243,15 +244,15 @@
         ],
         test_sqlparse=False,
         metadata_provider=provider,
     )
 
 
 @pytest.mark.parametrize("provider", providers)
-@patch("os.environ", {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
+@patch.dict(os.environ, {"SQLLINEAGE_LATERAL_COLUMN_ALIAS_REFERENCE": "1"})
 def test_column_enable_lateral_ref_within_subquery(
     provider: MetaDataProvider,
 ):
     sql = """
     insert into public.tgt_tbl1
     select
         sq.name
```

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_select_union.py` & `sqllineage-1.5.2/tests/sql/column/test_column_select_union.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_column_update.py` & `sqllineage-1.5.2/tests/sql/column/test_column_update.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_metadata_unqualified_column.py` & `sqllineage-1.5.2/tests/sql/column/test_metadata_unqualified_column.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/column/test_metadata_wildcard.py` & `sqllineage-1.5.2/tests/sql/column/test_metadata_wildcard.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/multiple_statements/test_split.py` & `sqllineage-1.5.2/tests/sql/table/multiple_statements/test_split.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/multiple_statements/test_tmp_table.py` & `sqllineage-1.5.2/tests/sql/table/multiple_statements/test_tmp_table.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_create.py` & `sqllineage-1.5.2/tests/sql/table/test_create.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_create_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_create_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_cte.py` & `sqllineage-1.5.2/tests/sql/table/test_cte.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_cte_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_cte_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_insert.py` & `sqllineage-1.5.2/tests/sql/table/test_insert.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_insert_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_insert_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_merge.py` & `sqllineage-1.5.2/tests/sql/table/test_merge.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_merge_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_merge_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_other_with_lineage_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_other_with_lineage_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_other_without_lineage.py` & `sqllineage-1.5.2/tests/sql/table/test_other_without_lineage.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_other_without_lineage_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_other_without_lineage_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_path_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_path_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `sqllineage-1.5.1/tests/sql/table/test_select.py` & `sqllineage-1.5.2/tests/sql/table/test_select.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,16 +103,41 @@
     assert_table_lineage_equal(sql, {"tab1", "tab2"})
 
 
 def test_select_parenthesized_from_table_join_recursive():
     sql = """SELECT tab1.id
 FROM ((tab1
     LEFT JOIN tab2 ON tab1.id = tab2.id)
-    LEFT JOIN tab3 ON tab1.id = tab3.id)"""
+    LEFT JOIN tab3 ON tab1.id = tab3.id)
+    """
     assert_table_lineage_equal(sql, {"tab1", "tab2", "tab3"})
+    sql = """SELECT tab1.id
+FROM (((tab1
+    LEFT JOIN tab2 ON tab1.id = tab2.id)
+    LEFT JOIN tab3 ON tab1.id = tab3.id)
+    LEFT JOIN tab4 ON tab1.id = tab4.id)
+    """
+    assert_table_lineage_equal(sql, {"tab1", "tab2", "tab3", "tab4"})
+    sql = """SELECT tab1.id
+FROM ((((tab1
+    LEFT JOIN tab2 ON tab1.id = tab2.id)
+    LEFT JOIN tab3 ON tab1.id = tab3.id)
+    LEFT JOIN tab4 ON tab1.id = tab4.id)
+    LEFT JOIN tab5 ON tab1.id = tab5.id)
+    """
+    assert_table_lineage_equal(sql, {"tab1", "tab2", "tab3", "tab4", "tab5"})
+    sql = """SELECT tab1.id
+FROM (((((tab1
+    LEFT JOIN tab2 ON tab1.id = tab2.id)
+    LEFT JOIN tab3 ON tab1.id = tab3.id)
+    LEFT JOIN tab4 ON tab1.id = tab4.id)
+    LEFT JOIN tab5 ON tab1.id = tab5.id)
+    LEFT JOIN tab6 ON tab1.id = tab6.id)
+        """
+    assert_table_lineage_equal(sql, {"tab1", "tab2", "tab3", "tab4", "tab5", "tab6"})
 
 
 def test_select_subquery():
     assert_table_lineage_equal("SELECT col1 FROM (SELECT col1 FROM tab1) dt", {"tab1"})
     # with an extra space
     assert_table_lineage_equal("SELECT col1 FROM ( SELECT col1 FROM tab1) dt", {"tab1"})
```

### Comparing `sqllineage-1.5.1/tests/sql/table/test_select_dialect_specific.py` & `sqllineage-1.5.2/tests/sql/table/test_select_dialect_specific.py`

 * *Files identical despite different names*

