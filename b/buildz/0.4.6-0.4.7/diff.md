# Comparing `tmp/buildz-0.4.6.tar.gz` & `tmp/buildz-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.4.6.tar", last modified: Tue Apr  2 17:39:22 2024, max compression
+gzip compressed data, was "buildz-0.4.7.tar", last modified: Sun Apr  7 18:00:58 2024, max compression
```

## Comparing `buildz-0.4.6.tar` & `buildz-0.4.7.tar`

### file list

```diff
@@ -1,124 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.293768 buildz-0.4.6/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.6/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.6/MANIFEST.in
--rw-rw-rw-   0        0        0     1386 2024-04-02 17:39:22.293768 buildz-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      971 2024-04-02 16:51:43.000000 buildz-0.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.231186 buildz-0.4.6/buildz/
--rw-rw-rw-   0        0        0      139 2024-04-01 15:22:30.000000 buildz-0.4.6/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.6/buildz/__main__.py
--rw-rw-rw-   0        0        0     1771 2024-04-02 17:23:58.000000 buildz-0.4.6/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.231186 buildz-0.4.6/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.231186 buildz-0.4.6/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.4.6/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.4.6/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.231186 buildz-0.4.6/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.246811 buildz-0.4.6/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.6/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1760 2024-04-02 16:24:31.000000 buildz-0.4.6/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.4.6/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.6/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.246811 buildz-0.4.6/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      307 2024-04-02 17:24:33.000000 buildz-0.4.6/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.4.6/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.4.6/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.4.6/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      542 2024-04-02 16:54:56.000000 buildz-0.4.6/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.246811 buildz-0.4.6/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.4.6/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.6/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.4.6/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.246811 buildz-0.4.6/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.4.6/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.4.6/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.246811 buildz-0.4.6/buildz/fz/
--rw-rw-rw-   0        0        0      159 2024-04-01 15:24:04.000000 buildz-0.4.6/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.6/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.4.6/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.246811 buildz-0.4.6/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.4.6/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.6/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.246811 buildz-0.4.6/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     1010 2024-04-02 12:26:00.000000 buildz-0.4.6/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     5842 2024-04-02 16:11:02.000000 buildz-0.4.6/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    12673 2024-04-02 14:42:14.000000 buildz-0.4.6/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.263134 buildz-0.4.6/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     4828 2024-04-02 14:18:18.000000 buildz-0.4.6/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.4.6/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.4.6/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.278138 buildz-0.4.6/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0     1843 2024-04-02 15:59:22.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.6/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.6/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.4.6/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.4.6/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.4.6/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.4.6/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.4.6/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.4.6/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     5472 2024-04-02 15:07:54.000000 buildz-0.4.6/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.4.6/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.4.6/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.4.6/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.4.6/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1112 2024-03-31 02:32:18.000000 buildz-0.4.6/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.278138 buildz-0.4.6/buildz/xf/
--rw-rw-rw-   0        0        0      209 2024-04-01 15:22:54.000000 buildz-0.4.6/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.6/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.278138 buildz-0.4.6/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.6/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.6/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.293768 buildz-0.4.6/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.6/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.6/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.6/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.6/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.6/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.6/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.6/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.6/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.6/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3070 2024-04-01 16:46:08.000000 buildz-0.4.6/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.6/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.6/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.6/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.6/buildz/xf/loader/pos.py
--rw-rw-rw-   0        0        0     1921 2024-04-02 14:13:24.000000 buildz-0.4.6/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2591 2024-04-01 16:46:39.000000 buildz-0.4.6/buildz/xf/read.py
--rw-rw-rw-   0        0        0     1314 2024-02-24 09:19:50.000000 buildz-0.4.6/buildz/xf/test_write.py
--rw-rw-rw-   0        0        0     1203 2024-03-01 16:51:07.000000 buildz-0.4.6/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.293768 buildz-0.4.6/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.6/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.6/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.293768 buildz-0.4.6/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.6/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.6/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.6/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.6/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1377 2024-02-24 09:43:55.000000 buildz-0.4.6/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.6/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.6/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.6/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:39:22.231186 buildz-0.4.6/buildz.egg-info/
--rw-rw-rw-   0        0        0     1386 2024-04-02 17:39:22.000000 buildz-0.4.6/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2825 2024-04-02 17:39:22.000000 buildz-0.4.6/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 17:39:22.000000 buildz-0.4.6/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 17:39:22.000000 buildz-0.4.6/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 17:39:22.293768 buildz-0.4.6/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-04-02 16:50:44.000000 buildz-0.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.7/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     1896 2024-04-07 18:00:58.533121 buildz-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2024-04-07 18:00:18.000000 buildz-0.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.439089 buildz-0.4.7/buildz/
+-rw-rw-rw-   0        0        0      139 2024-04-01 15:22:30.000000 buildz-0.4.7/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.7/buildz/__main__.py
+-rw-rw-rw-   0        0        0     1771 2024-04-02 17:23:58.000000 buildz-0.4.7/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.4.7/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.4.7/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     1770 2024-04-07 17:54:14.000000 buildz-0.4.7/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.7/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.7/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.4.7/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.4.7/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.4.7/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.7/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.4.7/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.4.7/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1116 2024-04-07 17:56:57.000000 buildz-0.4.7/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.4.7/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.4.7/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      542 2024-04-02 16:54:56.000000 buildz-0.4.7/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.4.7/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.7/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.4.7/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.4.7/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.4.7/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.488362 buildz-0.4.7/buildz/fz/
+-rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.4.7/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.7/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.4.7/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.4.7/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.488362 buildz-0.4.7/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.4.7/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.7/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.488362 buildz-0.4.7/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     1010 2024-04-02 12:26:00.000000 buildz-0.4.7/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     5842 2024-04-02 16:11:02.000000 buildz-0.4.7/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    12673 2024-04-02 14:42:14.000000 buildz-0.4.7/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.501866 buildz-0.4.7/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     4828 2024-04-02 14:18:18.000000 buildz-0.4.7/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.4.7/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.4.7/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.501866 buildz-0.4.7/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0     1843 2024-04-02 15:59:22.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.7/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.4.7/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.4.7/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.4.7/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.4.7/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.4.7/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.4.7/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     5472 2024-04-02 15:07:54.000000 buildz-0.4.7/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.4.7/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.4.7/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.4.7/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.4.7/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1931 2024-04-07 16:41:32.000000 buildz-0.4.7/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.517496 buildz-0.4.7/buildz/tz/
+-rw-rw-rw-   0        0        0      289 2024-04-07 16:06:13.000000 buildz-0.4.7/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     6379 2024-04-07 17:41:33.000000 buildz-0.4.7/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.517496 buildz-0.4.7/buildz/xf/
+-rw-rw-rw-   0        0        0      209 2024-04-01 15:22:54.000000 buildz-0.4.7/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.7/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.517496 buildz-0.4.7/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.7/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.7/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.7/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.7/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.7/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.7/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.7/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.7/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.7/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.7/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.7/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3070 2024-04-01 16:46:08.000000 buildz-0.4.7/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.7/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.7/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.7/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.7/buildz/xf/loader/pos.py
+-rw-rw-rw-   0        0        0     1921 2024-04-02 14:13:24.000000 buildz-0.4.7/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2591 2024-04-01 16:46:39.000000 buildz-0.4.7/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.4.7/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.7/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.7/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.7/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.7/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.7/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.7/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.4.7/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.7/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.7/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.7/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz.egg-info/
+-rw-rw-rw-   0        0        0     1896 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2976 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 18:00:58.533121 buildz-0.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      770 2024-04-07 18:00:49.000000 buildz-0.4.7/setup.py
```

### Comparing `buildz-0.4.6/LICENSE` & `buildz-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/PKG-INFO` & `buildz-0.4.7/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.6
+Version: 0.4.7
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
@@ -15,21 +15,31 @@
 ```
 1，在json格式基础上加了点东西，让配置文件写起来更简单，模块在buildz.xf下
 2，基于xf格式写了个ioc控制反转配置文件读取的程序，模块在buildz.ioc下
 3，其他工具模块：
     buildz.fz: 文件夹查找
     buildz.pyz: 简化python __import__调用
     buildz.argx: 按格式读命令行参数
+    buildz.tz: 加些工具，目前只有myerse diff字符串比较算法
     buildz.demo: 使用参考，运行"python -m buildz"会用这个模块
+代码关系:
+    buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
+    buildz.ioc需要buildz.xf和buildz.pyz
+    buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
     buildz.argx: read command argument in special format
     buildz.demo: example codes to use buildz, run "python -m buildz" will use this module
+code relationship:
+    buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
+    buildz.ioc use buildz.xf and buildz.pyz
+    buildz.tz: some tools, only contains "myerse diff algorithm" now
+    buildz.demo use all other modules
 
 run python -m buildz to see help
 ```
```

### Comparing `buildz-0.4.6/README.md` & `buildz-0.4.7/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,21 +2,31 @@
 ```
 1，在json格式基础上加了点东西，让配置文件写起来更简单，模块在buildz.xf下
 2，基于xf格式写了个ioc控制反转配置文件读取的程序，模块在buildz.ioc下
 3，其他工具模块：
     buildz.fz: 文件夹查找
     buildz.pyz: 简化python __import__调用
     buildz.argx: 按格式读命令行参数
+    buildz.tz: 加些工具，目前只有myerse diff字符串比较算法
     buildz.demo: 使用参考，运行"python -m buildz"会用这个模块
+代码关系:
+    buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
+    buildz.ioc需要buildz.xf和buildz.pyz
+    buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
     buildz.argx: read command argument in special format
     buildz.demo: example codes to use buildz, run "python -m buildz" will use this module
+code relationship:
+    buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
+    buildz.ioc use buildz.xf and buildz.pyz
+    buildz.tz: some tools, only contains "myerse diff algorithm" now
+    buildz.demo use all other modules
 
 run python -m buildz to see help
 ```
```

### Comparing `buildz-0.4.6/buildz/argx.py` & `buildz-0.4.7/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/ioc/deal.py` & `buildz-0.4.7/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/ioc/help.py` & `buildz-0.4.7/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/res/conf/main.js` & `buildz-0.4.7/buildz/demo/res/conf/main.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -37,14 +37,18 @@
                         xf: {
                             deal: deal.xf
                             help: help.xf
                         },
                         search: {
                             deal: deal.search
                             help: help.search
+                        },
+                        myers: {
+                            deal: deal.myers
+                            help: help.myers
                         }
                     }
                 }
                 default: {
                     type: ref
                     key: help.default
                 }
```

### Comparing `buildz-0.4.6/buildz/demo/res/help/ioc.js` & `buildz-0.4.7/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/res/help/search.js` & `buildz-0.4.7/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/res/help/xf.js` & `buildz-0.4.7/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/res/test.js` & `buildz-0.4.7/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/search/deal.py` & `buildz-0.4.7/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/demo/test.py` & `buildz-0.4.7/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/fz/dirz.py` & `buildz-0.4.7/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/fz/lsf.py` & `buildz-0.4.7/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc/base.py` & `buildz-0.4.7/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc/conf.py` & `buildz-0.4.7/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc/confs.py` & `buildz-0.4.7/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/base.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/call.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/calls.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.4.7/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/env.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/join.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/list.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/map.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/obj.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/ref.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/val.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/ioc/ioc_deal/var.py` & `buildz-0.4.7/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/pyz.py` & `buildz-0.4.7/buildz/pyz.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 
+import sys
+import os
 def load(md, fc = None):
     """
         import object(whether module or others) from md(or md.fc)
         exp:
             load("buildz.xf") = package xf
             load("buildz.xf", "loads") = function loads from package buildz.xf
             load("buildz.xf.loads") = function loads from package buildz.xf
@@ -22,26 +24,58 @@
     if fc is not None:
         fc = getattr(md, fc)
     else:
         fc = md
     return fc
 
 pass
-import sys
 def pyexe():
     return sys.executable
 
 pass
+exe=pyexe
 is_windows = sys.platform.lower()=='win32'
 def pypkg():
     """
         return python package path, test on linux and windows
     """
     import site
     sites = site.getsitepackages()
     if is_windows:
         fpath = sites[-1]
     else:
         fpath = sites[0]
     return fpath
 
 pass
+pkg = pypkg
+pth = pypkg
+
+class Pth:
+    def __init__(self, fp = "build.pth"):
+        self.fp = os.path.join(pth(), fp)
+    def read(self):
+        fp = self.fp
+        if not os.path.isfile(fp):
+            return []
+        with open(fp, 'rb') as f:
+            s = f.read().decode()
+        return s.split("\n")
+    def add(self, path):
+        arr = self.read()
+        if path in arr:
+            print("alread add")
+            return
+        arr.append(path)
+        self.write(arr)
+    def write(self, paths = []):
+        if type(paths) not in [list, tuple]:
+            paths = [paths]
+        s = "\n".join(paths)
+        with open(self.fp, 'wb') as f:
+            f.write(s.encode())
+    def remove(self):
+        os.remove(self.fp)
+
+pass
+
+_pth = Pth()
```

### Comparing `buildz-0.4.6/buildz/xf/file.py` & `buildz-0.4.7/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/base.py` & `buildz-0.4.7/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/buffer.py` & `buildz-0.4.7/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/listz.py` & `buildz-0.4.7/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/lr.py` & `buildz-0.4.7/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/lrval.py` & `buildz-0.4.7/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/mapz.py` & `buildz-0.4.7/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/nextz.py` & `buildz-0.4.7/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/reval.py` & `buildz-0.4.7/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/setz.py` & `buildz-0.4.7/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/spt.py` & `buildz-0.4.7/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/deal/strz.py` & `buildz-0.4.7/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/item.py` & `buildz-0.4.7/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/mg.py` & `buildz-0.4.7/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/loader/pos.py` & `buildz-0.4.7/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/mapz.py` & `buildz-0.4.7/buildz/xf/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/read.py` & `buildz-0.4.7/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/write.py` & `buildz-0.4.7/buildz/xf/write.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 pts = [
     "[\+\-]?\d+",
     "[\+\-]?\d+\.\d+",
     "[\+\-]?\d+e[\+\-]?\d+",
     "null",
     "true",
     "false",
-    "[\s\S]*[\n\r\t\:\[\]\{\}][\s\S]*"
+    "[\s\S]*[\n\r\t\:\[\]\{\}\(\)\,\:\=\'\<\>\" \|\#\;\/][\s\S]*"
 ]
 def build(json_format=False):
     mgs = mg.Manager()
     if not json_format:
         mgs.add(strz.StrDeal('"','"', pts))
         mgs.add(reval.ValDeal(float, lambda x:str(x)))
         mgs.add(reval.ValDeal(int, lambda x:str(x)))
```

### Comparing `buildz-0.4.6/buildz/xf/writer/base.py` & `buildz-0.4.7/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/writer/conf.py` & `buildz-0.4.7/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/writer/deal/listz.py` & `buildz-0.4.7/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/writer/deal/mapz.py` & `buildz-0.4.7/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/writer/deal/strz.py` & `buildz-0.4.7/buildz/xf/writer/deal/strz.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,17 @@
         self.pts = [self.rpt(pt) for pt in pts]
     def deal(self, obj, conf):
         val = obj.val
         if type(val) not in [bytes, str]:
             return None
         et = self.like("\n", val)
         need_ep = 0
-        if val.find(et)>=0:
+        if len(val)==0:
+            need_ep = 1
+        elif val.find(et)>=0:
             need_ep = 1
         else:
             for pt in self.pts:
                 rpt = self.like(pt, val)
                 if re.match(rpt, val) is not None:
                     need_ep = 1
                     break
```

### Comparing `buildz-0.4.6/buildz/xf/writer/itemz.py` & `buildz-0.4.7/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz/xf/writer/mg.py` & `buildz-0.4.7/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.6/buildz.egg-info/PKG-INFO` & `buildz-0.4.7/buildz.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.6
+Version: 0.4.7
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
@@ -15,21 +15,31 @@
 ```
 1，在json格式基础上加了点东西，让配置文件写起来更简单，模块在buildz.xf下
 2，基于xf格式写了个ioc控制反转配置文件读取的程序，模块在buildz.ioc下
 3，其他工具模块：
     buildz.fz: 文件夹查找
     buildz.pyz: 简化python __import__调用
     buildz.argx: 按格式读命令行参数
+    buildz.tz: 加些工具，目前只有myerse diff字符串比较算法
     buildz.demo: 使用参考，运行"python -m buildz"会用这个模块
+代码关系:
+    buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz都是独立的模块
+    buildz.ioc需要buildz.xf和buildz.pyz
+    buildz.demo需要其他全部模块
 
 运行python -m buildz查看帮助
 
 1, a profile file format base on json, make it easy to write profile file, module is in buildz.xf
 2, a ioc profile file read function base on xf format, module is in buildz.ioc
 3, other tools module:
     buildz.fz: file search
     buildz.pyz: make it easier to use python's __import__ function
     buildz.argx: read command argument in special format
     buildz.demo: example codes to use buildz, run "python -m buildz" will use this module
+code relationship:
+    buildz.xf, buildz.pyz, buildz.argx, buildz.fz, buildz.tz is independent
+    buildz.ioc use buildz.xf and buildz.pyz
+    buildz.tz: some tools, only contains "myerse diff algorithm" now
+    buildz.demo use all other modules
 
 run python -m buildz to see help
 ```
```

### Comparing `buildz-0.4.6/buildz.egg-info/SOURCES.txt` & `buildz-0.4.7/buildz.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,29 +9,34 @@
 buildz.egg-info/PKG-INFO
 buildz.egg-info/SOURCES.txt
 buildz.egg-info/dependency_links.txt
 buildz.egg-info/top_level.txt
 buildz/demo/test.py
 buildz/demo/ioc/deal.py
 buildz/demo/ioc/help.py
+buildz/demo/myers/deal.py
+buildz/demo/myers/help.py
 buildz/demo/res/test.js
 buildz/demo/res/conf/ioc.js
 buildz/demo/res/conf/main.js
+buildz/demo/res/conf/myers.js
 buildz/demo/res/conf/search.js
 buildz/demo/res/conf/xf.js
 buildz/demo/res/help/default.js
 buildz/demo/res/help/ioc.js
+buildz/demo/res/help/myers.js
 buildz/demo/res/help/search.js
 buildz/demo/res/help/xf.js
 buildz/demo/search/deal.py
 buildz/demo/search/help.py
 buildz/demo/xf/deal.py
 buildz/demo/xf/help.py
 buildz/fz/__init__.py
 buildz/fz/dirz.py
+buildz/fz/fio.py
 buildz/fz/lsf.py
 buildz/ioc/__init__.py
 buildz/ioc/init.py
 buildz/ioc/ioc/base.py
 buildz/ioc/ioc/conf.py
 buildz/ioc/ioc/confs.py
 buildz/ioc/ioc_deal/base.py
@@ -64,19 +69,20 @@
 buildz/ioc/ioc_deal/conf/obj_cst_lists.js
 buildz/ioc/ioc_deal/conf/obj_defaults.js
 buildz/ioc/ioc_deal/conf/obj_lists.js
 buildz/ioc/ioc_deal/conf/obj_set_lists.js
 buildz/ioc/ioc_deal/conf/ovar_lists.js
 buildz/ioc/ioc_deal/conf/ref_lists.js
 buildz/ioc/ioc_deal/conf/var_lists.js
+buildz/tz/__init__.py
+buildz/tz/myers_diff.py
 buildz/xf/__init__.py
 buildz/xf/file.py
 buildz/xf/mapz.py
 buildz/xf/read.py
-buildz/xf/test_write.py
 buildz/xf/write.py
 buildz/xf/xargs.py
 buildz/xf/loader/base.py
 buildz/xf/loader/buffer.py
 buildz/xf/loader/exp.py
 buildz/xf/loader/item.py
 buildz/xf/loader/mg.py
```

### Comparing `buildz-0.4.6/setup.py` & `buildz-0.4.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.4.6',
+    version = '0.4.7',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-base file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

