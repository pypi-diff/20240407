# Comparing `tmp/buildz-0.4.7.tar.gz` & `tmp/buildz-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.4.7.tar", last modified: Sun Apr  7 18:00:58 2024, max compression
+gzip compressed data, was "buildz-0.4.8.tar", last modified: Sun Apr  7 18:41:46 2024, max compression
```

## Comparing `buildz-0.4.7.tar` & `buildz-0.4.8.tar`

### file list

```diff
@@ -1,132 +1,132 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.7/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1896 2024-04-07 18:00:58.533121 buildz-0.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2024-04-07 18:00:18.000000 buildz-0.4.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.439089 buildz-0.4.7/buildz/
--rw-rw-rw-   0        0        0      139 2024-04-01 15:22:30.000000 buildz-0.4.7/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.7/buildz/__main__.py
--rw-rw-rw-   0        0        0     1771 2024-04-02 17:23:58.000000 buildz-0.4.7/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.4.7/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.4.7/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/myers/
--rw-rw-rw-   0        0        0     1770 2024-04-07 17:54:14.000000 buildz-0.4.7/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.7/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.7/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.4.7/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.4.7/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.4.7/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.7/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.4.7/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.4.7/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1116 2024-04-07 17:56:57.000000 buildz-0.4.7/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.4.7/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.4.7/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      542 2024-04-02 16:54:56.000000 buildz-0.4.7/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.4.7/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.7/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.4.7/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.4.7/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.4.7/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.488362 buildz-0.4.7/buildz/fz/
--rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.4.7/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.7/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.4.7/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.4.7/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.488362 buildz-0.4.7/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.4.7/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.7/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.488362 buildz-0.4.7/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     1010 2024-04-02 12:26:00.000000 buildz-0.4.7/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     5842 2024-04-02 16:11:02.000000 buildz-0.4.7/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    12673 2024-04-02 14:42:14.000000 buildz-0.4.7/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.501866 buildz-0.4.7/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     4828 2024-04-02 14:18:18.000000 buildz-0.4.7/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.4.7/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.4.7/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.501866 buildz-0.4.7/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0     1843 2024-04-02 15:59:22.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.7/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.7/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.4.7/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.4.7/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.4.7/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.4.7/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.4.7/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.4.7/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     5472 2024-04-02 15:07:54.000000 buildz-0.4.7/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.4.7/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.4.7/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.4.7/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.4.7/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1931 2024-04-07 16:41:32.000000 buildz-0.4.7/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.517496 buildz-0.4.7/buildz/tz/
--rw-rw-rw-   0        0        0      289 2024-04-07 16:06:13.000000 buildz-0.4.7/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     6379 2024-04-07 17:41:33.000000 buildz-0.4.7/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.517496 buildz-0.4.7/buildz/xf/
--rw-rw-rw-   0        0        0      209 2024-04-01 15:22:54.000000 buildz-0.4.7/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.7/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.517496 buildz-0.4.7/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.7/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.7/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.7/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.7/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.7/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.7/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.7/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.7/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.7/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.7/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.7/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3070 2024-04-01 16:46:08.000000 buildz-0.4.7/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.7/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.7/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.7/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.7/buildz/xf/loader/pos.py
--rw-rw-rw-   0        0        0     1921 2024-04-02 14:13:24.000000 buildz-0.4.7/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2591 2024-04-01 16:46:39.000000 buildz-0.4.7/buildz/xf/read.py
--rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.4.7/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.7/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.7/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.533121 buildz-0.4.7/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.7/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.7/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.7/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.7/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.4.7/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.7/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.7/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.7/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-07 18:00:58.470371 buildz-0.4.7/buildz.egg-info/
--rw-rw-rw-   0        0        0     1896 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2976 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-07 18:00:58.000000 buildz-0.4.7/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-07 18:00:58.533121 buildz-0.4.7/setup.cfg
--rw-rw-rw-   0        0        0      770 2024-04-07 18:00:49.000000 buildz-0.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.971928 buildz-0.4.8/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.8/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     1896 2024-04-07 18:41:46.971928 buildz-0.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2024-04-07 18:00:18.000000 buildz-0.4.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.892955 buildz-0.4.8/buildz/
+-rw-rw-rw-   0        0        0      139 2024-04-01 15:22:30.000000 buildz-0.4.8/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.8/buildz/__main__.py
+-rw-rw-rw-   0        0        0     1771 2024-04-02 17:23:58.000000 buildz-0.4.8/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.915842 buildz-0.4.8/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.919508 buildz-0.4.8/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.4.8/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.4.8/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.920208 buildz-0.4.8/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     1807 2024-04-07 18:37:57.000000 buildz-0.4.8/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.8/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.921674 buildz-0.4.8/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.924924 buildz-0.4.8/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.8/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.4.8/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.4.8/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.4.8/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.8/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.928710 buildz-0.4.8/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.4.8/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.4.8/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1116 2024-04-07 17:56:57.000000 buildz-0.4.8/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.4.8/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.4.8/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      542 2024-04-02 16:54:56.000000 buildz-0.4.8/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.928710 buildz-0.4.8/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.4.8/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.8/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.4.8/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.928710 buildz-0.4.8/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.4.8/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.4.8/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.933939 buildz-0.4.8/buildz/fz/
+-rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.4.8/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.8/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.4.8/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.4.8/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.933939 buildz-0.4.8/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.4.8/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.8/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.937518 buildz-0.4.8/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     1010 2024-04-02 12:26:00.000000 buildz-0.4.8/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     5842 2024-04-02 16:11:02.000000 buildz-0.4.8/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    12673 2024-04-02 14:42:14.000000 buildz-0.4.8/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.944146 buildz-0.4.8/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     4828 2024-04-02 14:18:18.000000 buildz-0.4.8/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.4.8/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.4.8/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.956925 buildz-0.4.8/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0     1843 2024-04-02 15:59:22.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.8/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.8/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.4.8/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.4.8/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.4.8/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.4.8/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.4.8/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.4.8/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     5472 2024-04-02 15:07:54.000000 buildz-0.4.8/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.4.8/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.4.8/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.4.8/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.4.8/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1931 2024-04-07 16:41:32.000000 buildz-0.4.8/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.956925 buildz-0.4.8/buildz/tz/
+-rw-rw-rw-   0        0        0      289 2024-04-07 16:06:13.000000 buildz-0.4.8/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7211 2024-04-07 18:39:24.000000 buildz-0.4.8/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.956925 buildz-0.4.8/buildz/xf/
+-rw-rw-rw-   0        0        0      209 2024-04-01 15:22:54.000000 buildz-0.4.8/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.8/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.971928 buildz-0.4.8/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1696 2024-03-01 16:40:46.000000 buildz-0.4.8/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     2456 2024-02-22 16:50:58.000000 buildz-0.4.8/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.971928 buildz-0.4.8/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.8/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2619 2024-03-31 10:34:46.000000 buildz-0.4.8/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.8/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.8/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.8/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1156 2024-03-01 16:45:20.000000 buildz-0.4.8/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-02-22 13:17:44.000000 buildz-0.4.8/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      390 2024-02-22 17:15:53.000000 buildz-0.4.8/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.8/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3070 2024-04-01 16:46:08.000000 buildz-0.4.8/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.8/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-02-22 16:35:35.000000 buildz-0.4.8/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     1693 2024-02-22 16:18:29.000000 buildz-0.4.8/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-02-22 12:37:04.000000 buildz-0.4.8/buildz/xf/loader/pos.py
+-rw-rw-rw-   0        0        0     1921 2024-04-02 14:13:24.000000 buildz-0.4.8/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2591 2024-04-01 16:46:39.000000 buildz-0.4.8/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.4.8/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.971928 buildz-0.4.8/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.8/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.8/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.971928 buildz-0.4.8/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.8/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.8/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.8/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.8/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.4.8/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.8/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.8/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      509 2024-04-01 13:44:50.000000 buildz-0.4.8/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-07 18:41:46.915842 buildz-0.4.8/buildz.egg-info/
+-rw-rw-rw-   0        0        0     1896 2024-04-07 18:41:46.000000 buildz-0.4.8/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2976 2024-04-07 18:41:46.000000 buildz-0.4.8/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 18:41:46.000000 buildz-0.4.8/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-07 18:41:46.000000 buildz-0.4.8/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 18:41:46.987558 buildz-0.4.8/setup.cfg
+-rw-rw-rw-   0        0        0      770 2024-04-07 18:41:15.000000 buildz-0.4.8/setup.py
```

### Comparing `buildz-0.4.7/LICENSE` & `buildz-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/PKG-INFO` & `buildz-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.7
+Version: 0.4.8
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.7/README.md` & `buildz-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/argx.py` & `buildz-0.4.8/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/ioc/deal.py` & `buildz-0.4.8/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/ioc/help.py` & `buildz-0.4.8/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/myers/deal.py` & `buildz-0.4.8/buildz/demo/myers/deal.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,14 @@
         mark_txt = argx.get(maps, 't', None)
         if mark_txt:
             mark_encode = 0
         spt = argx.get(maps, 's', 1)
         nspt = argx.get(maps, 'ns', 0)
         if nspt:
             spt = 0
-        print(f"SPT:{spt}")
         if opt == 'diff':
             bs1 = fz.read(fp1).decode("utf-8")
             bs2 = fz.read(fp2).decode("utf-8")
             #bs1 = b"text z xxxyzijsa"
             #bs2 = b"test xxxx afzjcovijsax"
             stps = tz.m_steps(bs1, bs2,split=spt)
             if mark_encode:
@@ -32,23 +31,25 @@
                 for stp in stps:
                     c = stp[-1]
                     if type(c)==bytes:
                         stp[-1] = c.decode()
                 stps = "t"+xf.dumps(stps)
                 stps = stps.encode()
             fz.write(fp_step, stps)
+            print("done diff")
         elif opt == 'update':
             bs1 = fz.read(fp1).decode("utf-8")
             bs_step = fz.read(fp_step)
             mark_encode = bs_step[:1] == b'e'
             bs_step= bs_step[1:]
             if mark_encode:
                 stps = tz.m_decode(bs_step)
             else:
                 stps = xf.loads(bs_step.decode())
             bs2 = tz.m_update(bs1, stps,split=spt).encode("utf-8")
             fz.write(fp2, bs2)
+            print("done update")
         else:
             print(f"unexpect opt: {opt}")
     pass
 
 pass
```

### Comparing `buildz-0.4.7/buildz/demo/res/conf/main.js` & `buildz-0.4.8/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/res/help/ioc.js` & `buildz-0.4.8/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/res/help/myers.js` & `buildz-0.4.8/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/res/help/search.js` & `buildz-0.4.8/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/res/help/xf.js` & `buildz-0.4.8/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/res/test.js` & `buildz-0.4.8/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/search/deal.py` & `buildz-0.4.8/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/demo/test.py` & `buildz-0.4.8/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/fz/dirz.py` & `buildz-0.4.8/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/fz/fio.py` & `buildz-0.4.8/buildz/fz/fio.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/fz/lsf.py` & `buildz-0.4.8/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc/base.py` & `buildz-0.4.8/buildz/ioc/ioc/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc/conf.py` & `buildz-0.4.8/buildz/ioc/ioc/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc/confs.py` & `buildz-0.4.8/buildz/ioc/ioc/confs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/base.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/call.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/calls.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.4.8/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.4.8/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/env.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/join.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/list.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/map.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/obj.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/obj.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/ref.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/val.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/ioc/ioc_deal/var.py` & `buildz-0.4.8/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/pyz.py` & `buildz-0.4.8/buildz/pyz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/tz/myers_diff.py` & `buildz-0.4.8/buildz/tz/myers_diff.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,47 +7,71 @@
 ACT_DEL = "del_curr"
 import struct
 def encode(steps, as_str = False):
     """
         步骤列表转bytes/str
     """
     rst = b""
+    # 加减的长度设置最多2**15-1，保留1位当作“加/减”，4位整数当字符串位置索引
+    max16 = 2**15-1
     for step in steps:
         if step[0] == ACT_ADD:
             bs = step[2]
             if type(bs) == str:
                 bs = bs.encode("utf-8")
-            obj = struct.pack(">BII", 1, step[1], len(bs))+bs
+            bs_arr = []
+            while len(bs)>max16:
+                cut = bs[:max16]
+                bs = bs[max16:]
+                bs_arr.append(cut)
+            if len(bs)>0:
+                bs_arr.append(bs)
+            for bs in bs_arr:
+                obj = struct.pack(">HI", len(bs)*2+1, step[1])+bs
+                rst+=obj
         else:
-            obj = struct.pack(">BII", 0, step[1], step[2])
-        rst+=obj
+            s1 = step[1]
+            s2 = step[2]
+            nexts = [s1]
+            while (s2-s1)>max16:
+                nexts.append(s1+max16)
+                s1+=max16+1
+            if s1<=s2:
+                nexts.append(s2)
+            for i in range(1,len(nexts)):
+                obj = struct.pack(">HI", (nexts[i]-nexts[i-1])*2, nexts[i-1])
+                rst+=obj
+        #rst+=obj
     if as_str:
         rst = base64.b64encode(rst).decode()
     return rst
 
 pass
 def decode(obj):
     """
         bytes/str转步骤列表
     """
     if type(obj) == str:
         obj = base64.b64decode(obj)
-    ni = 1+4+4
+    ni = 2+4
     rst = []
     while len(obj)>0:
         bs = obj[:ni]
         obj = obj[ni:]
-        act, base, c = struct.unpack(">BII", bs)
+        v2, base = struct.unpack(">HI", bs)
+        act = v2%2
+        c = v2//2
+        #act, base, c = struct.unpack(">HI", bs)
         if act == 1:
             bs = obj[:c]
             obj = obj[c:]
             s = bs.decode("utf-8")
             tmp = [ACT_ADD, base, s]
         else:
-            tmp = [ACT_DEL, base, c]
+            tmp = [ACT_DEL, base, base+c]
         rst.append(tmp)
     return rst
 
 pass
 def steps(vs, n, m, d, stra, strb):
     k = n-m
     rst = []
```

### Comparing `buildz-0.4.7/buildz/xf/file.py` & `buildz-0.4.8/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/base.py` & `buildz-0.4.8/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/buffer.py` & `buildz-0.4.8/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/listz.py` & `buildz-0.4.8/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/lr.py` & `buildz-0.4.8/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/lrval.py` & `buildz-0.4.8/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/mapz.py` & `buildz-0.4.8/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/nextz.py` & `buildz-0.4.8/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/reval.py` & `buildz-0.4.8/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/setz.py` & `buildz-0.4.8/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/spt.py` & `buildz-0.4.8/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/deal/strz.py` & `buildz-0.4.8/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/item.py` & `buildz-0.4.8/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/mg.py` & `buildz-0.4.8/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/loader/pos.py` & `buildz-0.4.8/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/mapz.py` & `buildz-0.4.8/buildz/xf/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/read.py` & `buildz-0.4.8/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/write.py` & `buildz-0.4.8/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/writer/base.py` & `buildz-0.4.8/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/writer/conf.py` & `buildz-0.4.8/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/writer/deal/listz.py` & `buildz-0.4.8/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/writer/deal/mapz.py` & `buildz-0.4.8/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/writer/deal/strz.py` & `buildz-0.4.8/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/writer/itemz.py` & `buildz-0.4.8/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz/xf/writer/mg.py` & `buildz-0.4.8/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/buildz.egg-info/PKG-INFO` & `buildz-0.4.8/buildz.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.7
+Version: 0.4.8
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.7/buildz.egg-info/SOURCES.txt` & `buildz-0.4.8/buildz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildz-0.4.7/setup.py` & `buildz-0.4.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.4.7',
+    version = '0.4.8',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-base file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

