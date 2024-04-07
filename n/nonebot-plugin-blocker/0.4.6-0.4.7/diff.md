# Comparing `tmp/nonebot_plugin_blocker-0.4.6.tar.gz` & `tmp/nonebot_plugin_blocker-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_blocker-0.4.6.tar", last modified: Thu Mar 28 19:30:11 2024, max compression
+gzip compressed data, was "nonebot_plugin_blocker-0.4.7.tar", last modified: Sun Apr  7 06:00:35 2024, max compression
```

## Comparing `nonebot_plugin_blocker-0.4.6.tar` & `nonebot_plugin_blocker-0.4.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/LICENSE
--rw-r--r--   0        0        0     2479 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/README.md
--rw-r--r--   0        0        0      494 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/__init__.py
--rw-r--r--   0        0        0     3609 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/__main__.py
--rw-r--r--   0        0        0     3848 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/config.py
--rw-r--r--   0        0        0     2687 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/web/__init__.py
--rw-r--r--   0        0        0     3154 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/web/webpage/main.html
--rw-r--r--   0        0        0     6189 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/web/webpage/main.js
--rw-r--r--   0        0        0     2297 2024-03-28 19:29:52.773811 nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/web/webpage/style.css
--rw-r--r--   0        0        0      687 2024-03-28 19:30:11.413871 nonebot_plugin_blocker-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/LICENSE
+-rw-r--r--   0        0        0     2479 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/README.md
+-rw-r--r--   0        0        0      494 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/__init__.py
+-rw-r--r--   0        0        0     3609 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/__main__.py
+-rw-r--r--   0        0        0     3848 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/config.py
+-rw-r--r--   0        0        0     2671 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/web/__init__.py
+-rw-r--r--   0        0        0     3154 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/web/webpage/main.html
+-rw-r--r--   0        0        0     4399 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/web/webpage/main.js
+-rw-r--r--   0        0        0     2297 2024-04-07 06:00:20.273700 nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/web/webpage/style.css
+-rw-r--r--   0        0        0      687 2024-04-07 06:00:35.529711 nonebot_plugin_blocker-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 nonebot_plugin_blocker-0.4.7/PKG-INFO
```

### Comparing `nonebot_plugin_blocker-0.4.6/LICENSE` & `nonebot_plugin_blocker-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.4.6/README.md` & `nonebot_plugin_blocker-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/__main__.py` & `nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/config.py` & `nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/web/__init__.py` & `nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/web/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,38 +58,38 @@
     try:
         reply_config.config.update({uin: form.model_dump()})
         await reply_config.save_config()
         await blockerlist.change_blocker_type(
             uin, form.model_dump().get("blocker_list", False)
         )
         return {"result": "success"}
-    except:  # noqa: E722
+    except Exception:
         return {"result": "failed"}
 
 
 @app.get("/query_reply_list")
 async def __get_reply_list__():
     try:
         bot_list : set = set(get_bots().keys())
         bot_list.update(reply_config.config.keys())
         return {"result": "success", "data": list(bot_list)}
-    except:  # noqa: E722
+    except Exception:
         return {"result": "failed"}
 
 
 @app.get("/query_reply")
 async def __get_reply_config__(uin: str):
     try:
         return {"result": "success", "data": reply_config.config.get(uin)}
-    except:  # noqa: E722
+    except Exception:
         return {"result": "failed"}
 
 
 @app.get("/delete")
 async def __delete_reply_config__(uin: str):
     try:
         reply_config.config.pop(uin)
         await reply_config.save_config()
         await blockerlist.change_blocker_type(uin)
         return {"result": "success"}
-    except:  # noqa: E722
+    except Exception:
         return {"result": "failed"}
```

### Comparing `nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/web/webpage/main.html` & `nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/web/webpage/main.html`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.4.6/nonebot_plugin_blocker/web/webpage/style.css` & `nonebot_plugin_blocker-0.4.7/nonebot_plugin_blocker/web/webpage/style.css`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_blocker-0.4.6/pyproject.toml` & `nonebot_plugin_blocker-0.4.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-blocker"
-version = "0.4.6"
+version = "0.4.7"
 description = "Message Blocker"
 authors = [
     { name = "MerCuJerry", email = "mercujerry@gmail.com" },
 ]
 keywords = [
     "nonebot",
     "nonebot2",
```

### Comparing `nonebot_plugin_blocker-0.4.6/PKG-INFO` & `nonebot_plugin_blocker-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-blocker
-Version: 0.4.6
+Version: 0.4.7
 Summary: Message Blocker
 Keywords: nonebot nonebot2 qqbot bot
 Home-page: https://github.com/MerCuJerry/nonebot-plugin-blocker
 Author-Email: MerCuJerry <mercujerry@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 MerCuJerry
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.4.6 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-blocker Version: 0.4.7 Summary:
 Message Blocker Keywords: nonebot nonebot2 qqbot bot Home-page: https://
 github.com/MerCuJerry/nonebot-plugin-blocker Author-Email: MerCuJerry
 gmail.com> License: MIT License Copyright (c) 2023 MerCuJerry Permission is
 hereby granted, free of charge, to any person obtaining a copy of this software
 and associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

