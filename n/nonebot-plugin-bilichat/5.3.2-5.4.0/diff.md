# Comparing `tmp/nonebot_plugin_bilichat-5.3.2.tar.gz` & `tmp/nonebot_plugin_bilichat-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_bilichat-5.3.2.tar", last modified: Sat Apr  6 17:23:17 2024, max compression
+gzip compressed data, was "nonebot_plugin_bilichat-5.4.0.tar", last modified: Sun Apr  7 17:19:20 2024, max compression
```

## Comparing `nonebot_plugin_bilichat-5.3.2.tar` & `nonebot_plugin_bilichat-5.4.0.tar`

### file list

```diff
@@ -1,80 +1,92 @@
--rw-r--r--   0        0        0    34523 2024-04-06 17:23:14.558272 nonebot_plugin_bilichat-5.3.2/LICENSE
--rw-r--r--   0        0        0    17886 2024-04-06 17:23:14.558272 nonebot_plugin_bilichat-5.3.2/README.md
--rw-r--r--   0        0        0     2799 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/__init__.py
--rw-r--r--   0        0        0     1120 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/__init__.py
--rw-r--r--   0        0        0      740 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/base.py
--rw-r--r--   0        0        0     2232 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/bilibili_auth.py
--rw-r--r--   0        0        0     1647 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/subs_config.py
--rw-r--r--   0        0        0     2686 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/webui.py
--rw-r--r--   0        0        0     7742 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/base_content_parsing.py
--rw-r--r--   0        0        0       60 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/__init__.py
--rw-r--r--   0        0        0     1300 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/auto_delete_subs.py
--rw-r--r--   0        0        0      996 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/base.py
--rw-r--r--   0        0        0      892 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/functions.py
--rw-r--r--   0        0        0     3845 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/login.py
--rw-r--r--   0        0        0     5230 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs.py
--rw-r--r--   0        0        0     4996 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs_cfg.py
--rw-r--r--   0        0        0     9273 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/config.py
--rw-r--r--   0        0        0       81 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/__init__.py
--rw-r--r--   0        0        0     3166 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/column.py
--rw-r--r--   0        0        0     4233 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/dynamic.py
--rw-r--r--   0        0        0     3942 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/video.py
--rw-r--r--   0        0        0      518 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/b23_extract.py
--rw-r--r--   0        0        0     6192 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bcut_asr.py
--rw-r--r--   0        0        0      506 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
--rw-r--r--   0        0        0     2406 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
--rw-r--r--   0        0        0      966 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
--rw-r--r--   0        0        0     2653 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
--rw-r--r--   0        0        0     2657 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/browser.py
--rw-r--r--   0        0        0      456 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/__init__.py
--rw-r--r--   0        0        0      437 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/cache.py
--rw-r--r--   0        0        0      871 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/json_cache.py
--rw-r--r--   0        0        0      531 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
--rw-r--r--   0        0        0      521 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/__init__.py
--rw-r--r--   0        0        0      217 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/column/__init__.py
--rw-r--r--   0        0        0     3262 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
--rw-r--r--   0        0        0      220 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
--rw-r--r--   0        0        0     5145 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
--rw-r--r--   0        0        0     1160 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
--rw-r--r--   0        0        0     7333 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py
--rw-r--r--   0        0        0     6326 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
--rw-r--r--   0        0        0     3040 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
--rw-r--r--   0        0        0     3796 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py
--rw-r--r--   0        0        0     3376 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fonts_provider.py
--rw-r--r--   0        0        0      525 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/store.py
--rw-r--r--   0        0        0     3115 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/strings.py
--rw-r--r--   0        0        0     3329 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/text_to_image.py
--rw-r--r--   0        0        0     1732 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/tools.py
--rw-r--r--   0        0        0     1788 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/uid_extract.py
--rw-r--r--   0        0        0     4033 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/video_subtitle.py
--rw-r--r--   0        0        0      568 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/__init__.py
--rw-r--r--   0        0        0      184 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/bilibili_auth.py
--rw-r--r--   0        0        0      824 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/subs_config.py
--rw-r--r--   0        0        0      341 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/arguments.py
--rw-r--r--   0        0        0     3019 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bcut_asr.py
--rw-r--r--   0        0        0     1326 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/live.py
--rw-r--r--   0        0        0     1040 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/summary.py
--rw-r--r--   0        0        0     1163 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/exception.py
--rw-r--r--   0        0        0      323 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/openai.py
--rw-r--r--   0        0        0      270 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/optional.py
--rw-r--r--   0        0        0     9390 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/browser/mobile_style.js
--rw-r--r--   0        0        0     1187 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png
--rw-r--r--   0        0        0     1200 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
--rw-r--r--   0        0        0    93905 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
--rw-r--r--   0        0        0     7545 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/video-details.html
--rw-r--r--   0        0        0     5777 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/bilibili.png
--rw-r--r--   0        0        0     2098 2024-04-06 17:23:14.578272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/index.html
--rw-r--r--   0        0        0    47433 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/marked.min.js
--rw-r--r--   0        0        0    59199 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/openai.png
--rw-r--r--   0        0        0     9556 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/upload-webui.html
--rw-r--r--   0        0        0   300664 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/webui.tar.gz
--rw-r--r--   0        0        0     2623 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/__init__.py
--rw-r--r--   0        0        0     7217 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/dynamic.py
--rw-r--r--   0        0        0     4023 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/live.py
--rw-r--r--   0        0        0    14427 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/manager.py
--rw-r--r--   0        0        0      478 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/__init__.py
--rw-r--r--   0        0        0     4931 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai.py
--rw-r--r--   0        0        0     2268 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai_summarise.py
--rw-r--r--   0        0        0     1655 2024-04-06 17:23:14.582272 nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/wordcloud.py
--rw-r--r--   0        0        0     1780 2024-04-06 17:23:17.694267 nonebot_plugin_bilichat-5.3.2/pyproject.toml
--rw-r--r--   0        0        0    19586 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.3.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-07 17:19:17.022463 nonebot_plugin_bilichat-5.4.0/LICENSE
+-rw-r--r--   0        0        0    17759 2024-04-07 17:19:17.026463 nonebot_plugin_bilichat-5.4.0/README.md
+-rw-r--r--   0        0        0     2674 2024-04-07 17:19:17.042463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-07 17:19:17.042463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/__init__.py
+-rw-r--r--   0        0        0      740 2024-04-07 17:19:17.042463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/base.py
+-rw-r--r--   0        0        0     2232 2024-04-07 17:19:17.042463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/bilibili_auth.py
+-rw-r--r--   0        0        0     1636 2024-04-07 17:19:17.042463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/subs_config.py
+-rw-r--r--   0        0        0     2686 2024-04-07 17:19:17.042463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/webui.py
+-rw-r--r--   0        0        0     7793 2024-04-07 17:19:17.042463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/base_content_parsing.py
+-rw-r--r--   0        0        0     1350 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/__init__.py
+-rw-r--r--   0        0        0      219 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/__init__.py
+-rw-r--r--   0        0        0      862 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/dodo.py
+-rw-r--r--   0        0        0     1951 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/kaiheila.py
+-rw-r--r--   0        0        0     1837 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/onebot_v11.py
+-rw-r--r--   0        0        0     3865 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/onebot_v12.py
+-rw-r--r--   0        0        0      872 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/qq.py
+-rw-r--r--   0        0        0     1165 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/red.py
+-rw-r--r--   0        0        0     3458 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/adapters/satori.py
+-rw-r--r--   0        0        0      396 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/expection.py
+-rw-r--r--   0        0        0     1745 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/registries.py
+-rw-r--r--   0        0        0     5797 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/bot_select/target.py
+-rw-r--r--   0        0        0       60 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/__init__.py
+-rw-r--r--   0        0        0     1311 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/auto_delete_subs.py
+-rw-r--r--   0        0        0     1063 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/base.py
+-rw-r--r--   0        0        0      942 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/functions.py
+-rw-r--r--   0        0        0     3895 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/login.py
+-rw-r--r--   0        0        0     5230 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/subs.py
+-rw-r--r--   0        0        0     4996 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/subs_cfg.py
+-rw-r--r--   0        0        0     9273 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/config.py
+-rw-r--r--   0        0        0       81 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/content/__init__.py
+-rw-r--r--   0        0        0     3166 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/content/column.py
+-rw-r--r--   0        0        0     4233 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/content/dynamic.py
+-rw-r--r--   0        0        0     3942 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/content/video.py
+-rw-r--r--   0        0        0      518 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/b23_extract.py
+-rw-r--r--   0        0        0     6192 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py
+-rw-r--r--   0        0        0      506 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bilibili_request/__init__.py
+-rw-r--r--   0        0        0     2406 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py
+-rw-r--r--   0        0        0      966 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py
+-rw-r--r--   0        0        0     2653 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py
+-rw-r--r--   0        0        0     2657 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/browser.py
+-rw-r--r--   0        0        0      456 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/cache/__init__.py
+-rw-r--r--   0        0        0      437 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/cache/cache.py
+-rw-r--r--   0        0        0      871 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/cache/json_cache.py
+-rw-r--r--   0        0        0      531 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py
+-rw-r--r--   0        0        0      521 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/__init__.py
+-rw-r--r--   0        0        0      217 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/column/__init__.py
+-rw-r--r--   0        0        0     3262 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py
+-rw-r--r--   0        0        0      220 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/dynamic/__init__.py
+-rw-r--r--   0        0        0     5145 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py
+-rw-r--r--   0        0        0     1160 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py
+-rw-r--r--   0        0        0     7333 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py
+-rw-r--r--   0        0        0     6326 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py
+-rw-r--r--   0        0        0     3040 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py
+-rw-r--r--   0        0        0     3796 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py
+-rw-r--r--   0        0        0     3376 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py
+-rw-r--r--   0        0        0      525 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/store.py
+-rw-r--r--   0        0        0     3115 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/strings.py
+-rw-r--r--   0        0        0     3329 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/text_to_image.py
+-rw-r--r--   0        0        0     1732 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/tools.py
+-rw-r--r--   0        0        0     1788 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/uid_extract.py
+-rw-r--r--   0        0        0     4033 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py
+-rw-r--r--   0        0        0      568 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/api/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/api/bilibili_auth.py
+-rw-r--r--   0        0        0      815 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/api/subs_config.py
+-rw-r--r--   0        0        0      341 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/arguments.py
+-rw-r--r--   0        0        0     3019 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/bcut_asr.py
+-rw-r--r--   0        0        0     1326 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/bilibili/live.py
+-rw-r--r--   0        0        0     1040 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/bilibili/summary.py
+-rw-r--r--   0        0        0     1163 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/exception.py
+-rw-r--r--   0        0        0      323 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/openai.py
+-rw-r--r--   0        0        0      270 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/optional.py
+-rw-r--r--   0        0        0     9390 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/browser/mobile_style.js
+-rw-r--r--   0        0        0     1187 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png
+-rw-r--r--   0        0        0     1200 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png
+-rw-r--r--   0        0        0    93905 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png
+-rw-r--r--   0        0        0     7545 2024-04-07 17:19:17.046463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/video-details.html
+-rw-r--r--   0        0        0     5777 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/bilibili.png
+-rw-r--r--   0        0        0     2098 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/index.html
+-rw-r--r--   0        0        0    47433 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/marked.min.js
+-rw-r--r--   0        0        0    59199 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/openai.png
+-rw-r--r--   0        0        0     9556 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/upload-webui.html
+-rw-r--r--   0        0        0   300664 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/webui.tar.gz
+-rw-r--r--   0        0        0     2623 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/__init__.py
+-rw-r--r--   0        0        0     7217 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/dynamic.py
+-rw-r--r--   0        0        0     4023 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/live.py
+-rw-r--r--   0        0        0    15971 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/manager.py
+-rw-r--r--   0        0        0      478 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/summary/__init__.py
+-rw-r--r--   0        0        0     4931 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/summary/openai.py
+-rw-r--r--   0        0        0     2268 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py
+-rw-r--r--   0        0        0     1615 2024-04-07 17:19:17.050463 nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/wordcloud.py
+-rw-r--r--   0        0        0     1707 2024-04-07 17:19:20.242417 nonebot_plugin_bilichat-5.4.0/pyproject.toml
+-rw-r--r--   0        0        0    19399 1970-01-01 00:00:00.000000 nonebot_plugin_bilichat-5.4.0/PKG-INFO
```

### Comparing `nonebot_plugin_bilichat-5.3.2/LICENSE` & `nonebot_plugin_bilichat-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/README.md` & `nonebot_plugin_bilichat-5.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -340,13 +340,12 @@
 -   [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 -   [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 -   [bilireq](https://github.com/SK-415/bilireq) 项目使用的 bilibili 请求库
 -   [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 -   [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项 BUG 修复和代码参考
 -   [hamo-reid](https://github.com/hamo-reid) 为 style_blue 绘制了界面
 -   [dynamicrender](https://pypi.org/project/dynrender-skia/) 提供 t2i 和动态渲染
--   [SAA](https://github.com/MountainDash/nonebot-plugin-send-anything-anywhere) 提供指令及订阅部分的跨平台支持
 -   [ALC](https://github.com/nonebot/plugin-alconna) 提供跨平台支持
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -182,12 +182,11 @@
 djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [bilireq](https://
 github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili è¯·æ±åº - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://github.com/Misaka-
 Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG ä¿®å¤åä»£ç åè - [hamo-
 reid](https://github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ -
 [dynamicrender](https://pypi.org/project/dynrender-skia/) æä¾ t2i
-åå¨ææ¸²æ - [SAA](https://github.com/MountainDash/nonebot-plugin-send-
-anything-anywhere) æä¾æä»¤åè®¢éé¨åçè·¨å¹³å°æ¯æ - [ALC](https:
-//github.com/nonebot/plugin-alconna) æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿
-[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
+åå¨ææ¸²æ - [ALC](https://github.com/nonebot/plugin-alconna)
+æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿ [![Stargazers over time](https://
+starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/
+nonebot-plugin-bilichat)
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/__init__.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 from nonebot import require
 from nonebot.plugin import PluginMetadata
 
 from .config import __version__, plugin_config, raw_config
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_alconna")
-require("nonebot_plugin_saa")
-
-from nonebot_plugin_saa import enable_auto_select_bot  # noqa: E402
-
-enable_auto_select_bot()
 
 cmd_perfix = f"{raw_config.command_start}{plugin_config.bilichat_cmd_start}{raw_config.command_sep}"
 
 __plugin_meta__ = PluginMetadata(
     name="nonebot-plugin-bilichat",
     description="多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat",
     usage="视频、专栏、动态解析直接发送链接、小程序、xml卡片即可，指令请参考 https://github.com/Well2333/nonebot-plugin-bilichat",
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/__init__.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/base.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/base.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/bilibili_auth.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/bilibili_auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/subs_config.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/subs_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict, List, Union
 
 import nonebot
 from nonebot.compat import model_dump
 from nonebot.log import logger
-from nonebot_plugin_saa.utils.const import SupportedPlatform
 from pydantic import ValidationError
 
+from ..bot_select.target import SupportedPlatform
 from ..model.api import FaildResponse, Response
 from ..model.api.subs_config import Subs
 from ..subscribe.manager import SubscriptionSystem
 from .base import app
 
 config = nonebot.get_driver().config
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/api/webui.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/api/webui.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/base_content_parsing.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/base_content_parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,14 +136,16 @@
         else:
             raise AbortError(f"查询 {bililink} 返回内容为空")
 
         return True
     except AbortError as e:
         logger.info(e)
         return False
+    except FinishedException:
+        return False
 
 
 async def _pre_check(state: T_State, event: Event, bot: Bot, msg: UniMsg, target: MsgTarget):
     return await _permission_check(bot, event, target, state) and await _bili_check(state, event, bot, msg)
 
 
 bilichat = on_message(
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/base.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import asyncio
 from asyncio import Lock
 
+from nonebot.log import logger
 from nonebot.matcher import Matcher
 from nonebot.params import Depends
 from nonebot.plugin import CommandGroup
 from nonebot.rule import to_me
-from nonebot_plugin_saa import SaaTarget
+from nonebot_plugin_alconna.uniseg import MsgTarget
 
 from ..config import plugin_config
 from ..subscribe.manager import CONFIG_LOCK, SubscriptionSystem, User
 
 bilichat = CommandGroup(
     plugin_config.bilichat_cmd_start,
     rule=to_me() if plugin_config.bilichat_command_to_me else None,
@@ -18,13 +19,14 @@
 
 async def check_lock(matcher: Matcher) -> Lock:
     while CONFIG_LOCK.locked():
         await asyncio.sleep(0)
     return CONFIG_LOCK
 
 
-async def get_user(matcher: Matcher, target: SaaTarget, lock: Lock = Depends(check_lock)):
+async def get_user(matcher: Matcher, target: MsgTarget, lock: Lock = Depends(check_lock)):
+    logger.debug(target)
     async with lock:
-        platform, user_id = User.extract_saa_target(target)
+        platform, user_id = User.extract_alc_target(target)
         if not user_id:
             await matcher.finish("暂时还不支持当前会话呢\n`(*>﹏<*)′")
         return SubscriptionSystem.users.get(f"{platform}-_-{user_id}", User(user_id=user_id, platform=platform))
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/login.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from asyncio import Lock
 
 from bilireq.login import Login
 from nonebot.adapters import Message
 from nonebot.log import logger
 from nonebot.params import CommandArg, Depends
 from nonebot.permission import SUPERUSER
-from nonebot_plugin_saa import Image, MessageFactory
+from nonebot_plugin_alconna.uniseg import Image, MsgTarget, UniMessage
 
 from ..config import plugin_config
 from ..lib.bilibili_request.auth import AuthManager
 from ..lib.tools import calc_time_total
 from .base import bilichat, check_lock
 
 # bili_login_sms = bilichat.command(
@@ -78,21 +78,21 @@
                 for auth in AuthManager.grpc_auths
             ]
         )
     )
 
 
 @bili_login_qrcode.handle()
-async def bili_qrcode_login(lock: Lock = Depends(check_lock)):
+async def bili_qrcode_login(target: MsgTarget, lock: Lock = Depends(check_lock)):
     async with lock:
         login = Login()
         qr_url = await login.get_qrcode_url()
         logger.debug(f"qrcode login url: {qr_url}")
         data = "base64://" + await login.get_qrcode(qr_url, base64=True)  # type: ignore
-        await MessageFactory(Image(data)).send()
+        await UniMessage(Image(raw=data)).send(target=target)
         try:
             auth = await login.qrcode_login(interval=5)
             assert auth, "登录失败，返回数据为空"
             logger.debug(auth.data)
             AuthManager.add_auth(auth)
             AuthManager.dump_grpc_auths()
         except Exception as e:
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/subs.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/commands/subs_cfg.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/commands/subs_cfg.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/config.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/column.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/content/column.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/dynamic.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/content/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/content/video.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/content/video.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/b23_extract.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/b23_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bcut_asr.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/auth.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bilibili_request/auth.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bilibili_request/gRPC.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/bilibili_request/restAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/browser.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/browser.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/json_cache.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/cache/json_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/cache/mongo_cache.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/cache/mongo_cache.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/__init__.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/column/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/dynamic/browser_shot.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/dynamic/dynamicrender.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/__init__.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/video/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/video/bbot_default.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/draw/video/style_blue.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/draw/video/style_blue.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fetch_dynamic.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/fetch_dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/fonts_provider.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/fonts_provider.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/store.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/store.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/strings.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/strings.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/text_to_image.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/text_to_image.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/tools.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/tools.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/uid_extract.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/uid_extract.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/lib/video_subtitle.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/lib/video_subtitle.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/__init__.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/api/subs_config.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/api/subs_config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import List
 
-from nonebot_plugin_saa.utils.const import SupportedPlatform
 from pydantic import BaseModel, Field
 
+from ...bot_select.target import SupportedPlatform
+
 
 class SubsConfig(BaseModel):
     subs_limit: int = Field(5, ge=0, le=50)
     dynamic_interval: int = Field(90, ge=60)
     live_interval: int = Field(30, ge=10)
     push_delay: int = Field(3, ge=0)
     dynamic_grpc: bool = False
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bcut_asr.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/bcut_asr.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/live.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/bilibili/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/bilibili/summary.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/bilibili/summary.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/model/exception.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/model/exception.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/browser/mobile_style.js` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/browser/mobile_style.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/business.png` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/assets/business.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/personal.png` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/assets/personal.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/assets/video_bottom.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/style_blue/video-details.html` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/style_blue/video-details.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/bilibili.png` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/bilibili.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/index.html` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/index.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/marked.min.js` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/marked.min.js`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/summary/openai.png` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/summary/openai.png`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/upload-webui.html` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/upload-webui.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/static/webui.tar.gz` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/static/webui.tar.gz`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/__init__.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/dynamic.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/dynamic.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/live.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/live.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/subscribe/manager.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/subscribe/manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 import asyncio
 import json
+import random
 import time
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 from apscheduler.job import Job
 from nonebot import get_driver
 from nonebot.adapters import Bot
 from nonebot.compat import PYDANTIC_V2
 from nonebot.log import logger
+from nonebot_plugin_alconna.uniseg import AtAll, Image, SupportScope, Target, UniMessage
 from nonebot_plugin_apscheduler import scheduler
-from nonebot_plugin_saa import (
-    Image,
-    Mention,
-    MessageFactory,
-    PlatformTarget,
-    TargetQQGroup,
-    TargetQQGuildChannel,
-    TargetQQPrivate,
-)
-from nonebot_plugin_saa.auto_select_bot import BOT_CACHE, get_bot
-from nonebot_plugin_saa.utils.const import SupportedPlatform
-from nonebot_plugin_saa.utils.exceptions import NoBotFound
 from pydantic import BaseModel, Field, validator
 
+from ..bot_select import get_bots
+from ..bot_select.expection import NoBotFoundError
+from ..bot_select.registries import BOT_CACHE, BOT_CACHE_LOCK
+from ..bot_select.target import PlatformTarget, SupportedPlatform, TargetQQGroup, TargetQQGuildChannel, TargetQQPrivate
 from ..lib.store import data_dir
 from ..lib.tools import calc_time_total
 from ..lib.uid_extract import uid_extract_sync
 from ..optional import capture_exception
 
 # 临时解决方案
 try:
@@ -148,34 +142,46 @@
             except (ValueError, TypeError):
                 # 处理 uid 转换为 int 时可能发生的错误
                 continue
 
         return validated_subs
 
     @classmethod
-    def extract_saa_target(cls, target: PlatformTarget):
-        if isinstance(target, TargetQQGroup):
-            user_id = target.group_id
-        elif isinstance(target, TargetQQPrivate):
-            user_id = target.user_id
-        elif isinstance(target, TargetQQGuildChannel):
-            user_id = target.channel_id
+    def extract_alc_target(cls, target: Target) -> Tuple[str, str]:
+
+        if target.scope == SupportScope.qq_client:
+            user_id = target.id
+            if target.private:
+                return SupportedPlatform.qq_private, user_id
+            else:
+                return SupportedPlatform.qq_group, user_id
+        elif target.scope == SupportScope.qq_guild:
+            return SupportedPlatform.qq_guild_channel, target.id
         else:
-            raise NotImplementedError("Unsupported target type")
-        return str(target.platform_type), str(user_id)
+            raise NotImplementedError(f"Unsupported target type {target.scope}")
 
-    def create_saa_target(self):
+    def create_saa_target(self) -> PlatformTarget:
         if self.platform == SupportedPlatform.qq_group:
             return TargetQQGroup(group_id=int(self.user_id))
         elif self.platform == SupportedPlatform.qq_private:
             return TargetQQPrivate(user_id=int(self.user_id))
         elif self.platform == SupportedPlatform.qq_guild_channel:
             return TargetQQGuildChannel(channel_id=int(self.user_id))
         else:
             raise NotImplementedError("Unsupported platform type")
+    
+    def create_alc_target(self) -> Target:
+        if self.platform == SupportedPlatform.qq_group:
+            return Target(id=self.user_id, scope=SupportScope.qq_client, private=False)
+        elif self.platform == SupportedPlatform.qq_private:
+            return Target(id=self.user_id, scope=SupportScope.qq_client, private=True)
+        elif self.platform == SupportedPlatform.qq_guild_channel:
+            return Target(id=self.user_id, scope=SupportScope.qq_guild)
+        else:
+            raise NotImplementedError("Unsupported platform type")
 
     def dict(self, **kwargs) -> Dict[str, Any]:
         exclude_properties = {name for name, value in type(self).__dict__.items() if isinstance(value, property)}
         exclude_properties.add("subscriptions")
         if PYDANTIC_V2:
             dict_ = super().model_dump(**{**kwargs, "exclude": exclude_properties})  # type: ignore
         else:
@@ -194,32 +200,42 @@
         return uplist
 
     @property
     def _id(self) -> str:
         return f"{self.platform}-_-{self.user_id}"
 
     async def push_to_user(self, content: List[Union[str, bytes]], at_all: Optional[bool] = None):
-        target = self.create_saa_target()
         if not at_all:
             at = ""
         elif self.platform == SupportedPlatform.qq_group:
-            at = Mention("all")
+            at = AtAll()
         elif self.platform == SupportedPlatform.qq_guild_channel:
             at = "@everyone"
         else:
             at = ""
-        msg = MessageFactory(at)
-        msg.extend([Image(x) if isinstance(x, bytes) else x for x in content])  # type: ignore
+        msg = UniMessage(at)
+        msg.extend([Image(raw=x) if isinstance(x, bytes) else x for x in content])  # type: ignore
+
         try:
-            await msg.send_to(target)
-        except NoBotFound:
-            pass
-        except Exception as e:
-            logger.exception(f"无法为用户 {self.user_id} 推送消息")
-            capture_exception(e)
+            bots = get_bots(target=self.create_saa_target())
+        except NoBotFoundError:
+            logger.warning(f"用户 {self.user_id} 无可用的推送Bot")
+            return
+        random.shuffle(bots)
+        logger.info(f"向 {self.user_id} 推送消息，可用的bots： {bots}")
+        for bot in bots:
+            logger.debug(f"开始推送 -> {bot}")
+            try:
+                await msg.send(bot=bot,target=self.create_alc_target())
+                logger.debug(f"推送成功 -> {bot}")
+                return
+            except Exception as e:
+                capture_exception(e)
+                logger.exception(f"推送失败 -> {bot}")
+        logger.error(f"无法为用户 {self.user_id} 推送消息")
 
         await asyncio.sleep(SubscriptionSystem.config.push_delay)
 
     def add_subscription(self, uploader: Uploader) -> Union[None, str]:
         """Add a subscription for a user to an uploader."""
 
         if len(self.subscriptions) > SubscriptionSystem.config.subs_limit:
@@ -367,35 +383,44 @@
         at_ups = "\n".join([str(up) for up in cls.activate_uploaders.values()])
         logger.debug("已激活的UP:\n" + (at_ups or "无已激活的UP"))
         return at_ups
 
     @classmethod
     def refresh_activate_uploaders(cls):
         """通过当前 Bot 覆盖的平台，激活需要推送的UP"""
-        logger.debug("刷新已激活的UP")
+        logger.info("正在刷新激活的UP列表")
         cls.activate_uploaders = {}
         for user in cls.users.values():
+            logger.debug(f"正在尝试激活用户 {user._id} 订阅的 UP")
             target = user.create_saa_target()
             try:
-                get_bot(target)
+                get_bots(target)
                 cls.activate_uploaders.update({int(up): cls.uploaders[int(up)] for up in user.subscriptions.keys()})
-            except NoBotFound:
+            except NoBotFoundError:
                 logger.debug(f"用户 {user._id} 无可用推送 Bot")
                 continue
         cls.get_activate_uploaders()
 
 
 driver.on_startup(SubscriptionSystem.load_from_file)
 
 
 @driver.on_bot_connect
 async def _(bot: Bot):
-    while bot not in BOT_CACHE.keys():
+    logger.info("重新检查可推送的用户")
+    while True:
+        if bot in BOT_CACHE.keys():
+            SubscriptionSystem.refresh_activate_uploaders()
+            logger.info("检查可推送的用户完成")
+            return
         await asyncio.sleep(0.5)
-    SubscriptionSystem.refresh_activate_uploaders()
 
 
 @driver.on_bot_disconnect
 async def _(bot: Bot):
-    while bot in BOT_CACHE.keys():
+    logger.info("重新检查可推送的用户")
+    while True:
+        if bot not in BOT_CACHE.keys():
+            SubscriptionSystem.refresh_activate_uploaders()
+            logger.info("检查可推送的用户完成")
+            return
         await asyncio.sleep(0.5)
-    SubscriptionSystem.refresh_activate_uploaders()
```

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/summary/openai.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/summary/openai_summarise.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/summary/openai_summarise.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_bilichat-5.3.2/nonebot_plugin_bilichat/wordcloud.py` & `nonebot_plugin_bilichat-5.4.0/nonebot_plugin_bilichat/wordcloud.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from jieba.analyse.tfidf import TFIDF
 from nonebot.log import logger
 from wordcloud import WordCloud
 
 from .config import plugin_config
 from .lib.cache import BaseCache
 from .lib.fonts_provider import get_font_async
-from .model.exception import AbortError
 from .optional import capture_exception  # type: ignore
 
 tfidf = TFIDF()
 
 
 async def wordcloud(cache: BaseCache) -> Optional[bytes]:
     try:
```

### Comparing `nonebot_plugin_bilichat-5.3.2/pyproject.toml` & `nonebot_plugin_bilichat-5.4.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-bilichat"
-version = "5.3.2"
+version = "5.4.0"
 description = "多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat"
 authors = [
     { name = "djkcyl", email = "cyl@cyllive.cn" },
     { name = "Well404", email = "well_404@outlook.com" },
 ]
 dependencies = [
     "bilireq>=0.2.8",
@@ -12,18 +12,17 @@
     "pillow>=9.5.0",
     "lxml>=4.9.2",
     "nonebot-plugin-localstore>=0.4.1",
     "nonebot2[fastapi,websockets]>=2.0.0",
     "httpx>=0.24.1",
     "dynrender-skia-opt>=0.3.8",
     "nonebot-plugin-apscheduler>=0.3.0",
-    "nonebot-plugin-send-anything-anywhere>=0.4.0",
     "packaging>=23.2",
     "python-multipart>=0.0.6",
-    "nonebot-plugin-alconna>=0.42.0",
+    "nonebot-plugin-alconna>=0.42.3",
 ]
 requires-python = ">=3.8,<4.0"
 readme = "README.md"
 
 [project.license]
 text = "AGPL3.0"
 
@@ -65,15 +64,14 @@
 [tool.pdm.dev-dependencies]
 dev = [
     "black>=23.3.0",
     "nonebot-adapter-onebot>=2.2.4",
     "nonebot-adapter-mirai2>=0.0.22",
     "nonebot-adapter-qq>=1.0.1",
     "viztracer>=0.16.1",
-    "nb-cli>=1.2.8",
     "nonebot-adapter-satori>=0.10.3",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
```

### Comparing `nonebot_plugin_bilichat-5.3.2/PKG-INFO` & `nonebot_plugin_bilichat-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-bilichat
-Version: 5.3.2
+Version: 5.4.0
 Summary: 多种B站链接解析，视频词云，AI总结，你想要的都在 bilichat
 Author-Email: djkcyl <cyl@cyllive.cn>, Well404 <well_404@outlook.com>
 License: AGPL3.0
 Requires-Python: <4.0,>=3.8
 Requires-Dist: bilireq>=0.2.8
 Requires-Dist: qrcode>=7.4.2
 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2
 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0
 Requires-Dist: httpx>=0.24.1
 Requires-Dist: dynrender-skia-opt>=0.3.8
 Requires-Dist: nonebot-plugin-apscheduler>=0.3.0
-Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.4.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: python-multipart>=0.0.6
-Requires-Dist: nonebot-plugin-alconna>=0.42.0
+Requires-Dist: nonebot-plugin-alconna>=0.42.3
 Requires-Dist: numpy<1.25.0,>=1.20.1; extra == "extra"
 Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
 Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra"
 Requires-Dist: nonebot-plugin-mongodb>=0.1.0; extra == "extra"
 Requires-Dist: jieba>=0.42.1; extra == "wordcloud"
 Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud"
 Requires-Dist: tiktoken>=0.6.0; extra == "summary"
@@ -380,13 +379,12 @@
 -   [BBot-Graia](https://github.com/djkcyl/BBot-Graia) 功能来源 ~~(我 牛 我 自 己)~~
 -   [ABot-Graia](https://github.com/djkcyl/ABot-Graia) 永远怀念最好的 ABot 🙏
 -   [bilireq](https://github.com/SK-415/bilireq) 项目使用的 bilibili 请求库
 -   [nonebot-plugin-template](https://github.com/A-kirami/nonebot-plugin-template): 项目的 README 模板
 -   [Misaka-Mikoto-Tech](https://github.com/Misaka-Mikoto-Tech) 为本项目提交了多项 BUG 修复和代码参考
 -   [hamo-reid](https://github.com/hamo-reid) 为 style_blue 绘制了界面
 -   [dynamicrender](https://pypi.org/project/dynrender-skia/) 提供 t2i 和动态渲染
--   [SAA](https://github.com/MountainDash/nonebot-plugin-send-anything-anywhere) 提供指令及订阅部分的跨平台支持
 -   [ALC](https://github.com/nonebot/plugin-alconna) 提供跨平台支持
 
 ## ⏳ Star 趋势
 
 [![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.3.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-bilichat Version: 5.4.0 Summary:
 å¤ç§Bç«é¾æ¥è§£æï¼è§é¢è¯äºï¼AIæ»ç»ï¼ä½ æ³è¦çé½å¨ bilichat
 Author-Email: djkcyl
 cyllive.cn>, Well404
 outlook.com> License: AGPL3.0 Requires-Python: <4.0,>=3.8 Requires-Dist:
 bilireq>=0.2.8 Requires-Dist: qrcode>=7.4.2 Requires-Dist: pillow>=9.5.0
 Requires-Dist: lxml>=4.9.2 Requires-Dist: nonebot-plugin-localstore>=0.4.1
 Requires-Dist: nonebot2[fastapi,websockets]>=2.0.0 Requires-Dist: httpx>=0.24.1
 Requires-Dist: dynrender-skia-opt>=0.3.8 Requires-Dist: nonebot-plugin-
-apscheduler>=0.3.0 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.4.0
-Requires-Dist: packaging>=23.2 Requires-Dist: python-multipart>=0.0.6 Requires-
-Dist: nonebot-plugin-alconna>=0.42.0 Requires-Dist: numpy<1.25.0,>=1.20.1;
-extra == "extra" Requires-Dist: nonebot-plugin-sentry>=0.2.2; extra == "extra"
-Requires-Dist: nonebot-plugin-htmlrender>=0.2.0.3; extra == "extra" Requires-
-Dist: nonebot-plugin-mongodb>=0.1.0; extra == "extra" Requires-Dist:
-jieba>=0.42.1; extra == "wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra ==
-"wordcloud" Requires-Dist: tiktoken>=0.6.0; extra == "summary" Requires-Dist:
-numpy<1.25.0,>=1.20.1; extra == "all" Requires-Dist: jieba>=0.42.1; extra ==
-"all" Requires-Dist: wordcloud>=1.8.2.2; extra == "all" Requires-Dist: nonebot-
-plugin-htmlrender>=0.2.0.3; extra == "all" Requires-Dist: nonebot-plugin-
+apscheduler>=0.3.0 Requires-Dist: packaging>=23.2 Requires-Dist: python-
+multipart>=0.0.6 Requires-Dist: nonebot-plugin-alconna>=0.42.3 Requires-Dist:
+numpy<1.25.0,>=1.20.1; extra == "extra" Requires-Dist: nonebot-plugin-
+sentry>=0.2.2; extra == "extra" Requires-Dist: nonebot-plugin-
+htmlrender>=0.2.0.3; extra == "extra" Requires-Dist: nonebot-plugin-
+mongodb>=0.1.0; extra == "extra" Requires-Dist: jieba>=0.42.1; extra ==
+"wordcloud" Requires-Dist: wordcloud>=1.8.2.2; extra == "wordcloud" Requires-
+Dist: tiktoken>=0.6.0; extra == "summary" Requires-Dist: numpy<1.25.0,>=1.20.1;
+extra == "all" Requires-Dist: jieba>=0.42.1; extra == "all" Requires-Dist:
+wordcloud>=1.8.2.2; extra == "all" Requires-Dist: nonebot-plugin-
+htmlrender>=0.2.0.3; extra == "all" Requires-Dist: nonebot-plugin-
 mongodb>=0.1.0; extra == "all" Requires-Dist: nonebot-plugin-sentry>=0.4.1;
 extra == "all" Requires-Dist: tiktoken>=0.6.0; extra == "all" Provides-Extra:
 extra Provides-Extra: wordcloud Provides-Extra: summary Provides-Extra: all
 Description-Content-Type: text/markdown
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
    # nonebot-plugin-bilichat _â¨ å¤åè½ç B ç«è§é¢è§£æå·¥å· â¨_
@@ -206,12 +206,11 @@
 djkcyl/ABot-Graia) æ°¸è¿æå¿µæå¥½ç ABot ð - [bilireq](https://
 github.com/SK-415/bilireq) é¡¹ç®ä½¿ç¨ç bilibili è¯·æ±åº - [nonebot-
 plugin-template](https://github.com/A-kirami/nonebot-plugin-template):
 é¡¹ç®ç README æ¨¡æ¿ - [Misaka-Mikoto-Tech](https://github.com/Misaka-
 Mikoto-Tech) ä¸ºæ¬é¡¹ç®æäº¤äºå¤é¡¹ BUG ä¿®å¤åä»£ç åè - [hamo-
 reid](https://github.com/hamo-reid) ä¸º style_blue ç»å¶äºçé¢ -
 [dynamicrender](https://pypi.org/project/dynrender-skia/) æä¾ t2i
-åå¨ææ¸²æ - [SAA](https://github.com/MountainDash/nonebot-plugin-send-
-anything-anywhere) æä¾æä»¤åè®¢éé¨åçè·¨å¹³å°æ¯æ - [ALC](https:
-//github.com/nonebot/plugin-alconna) æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿
-[![Stargazers over time](https://starchart.cc/djkcyl/nonebot-plugin-
-bilichat.svg)](https://starchart.cc/djkcyl/nonebot-plugin-bilichat)
+åå¨ææ¸²æ - [ALC](https://github.com/nonebot/plugin-alconna)
+æä¾è·¨å¹³å°æ¯æ ## â³ Star è¶å¿ [![Stargazers over time](https://
+starchart.cc/djkcyl/nonebot-plugin-bilichat.svg)](https://starchart.cc/djkcyl/
+nonebot-plugin-bilichat)
```

