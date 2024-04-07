# Comparing `tmp/nonebot_plugin_ghtiles-0.1.2.tar.gz` & `tmp/nonebot_plugin_ghtiles-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ghtiles-0.1.2.tar", last modified: Wed Apr  3 11:09:55 2024, max compression
+gzip compressed data, was "nonebot_plugin_ghtiles-0.1.3.tar", last modified: Sun Apr  7 09:32:20 2024, max compression
```

## Comparing `nonebot_plugin_ghtiles-0.1.2.tar` & `nonebot_plugin_ghtiles-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/LICENSE
--rw-r--r--   0        0        0     3002 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/README.md
--rw-r--r--   0        0        0     7242 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/__init__.py
--rw-r--r--   0        0        0      241 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/config.py
--rw-r--r--   0        0        0     2211 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/utils.py
--rw-r--r--   0        0        0     1172 2024-04-03 11:09:55.310957 nonebot_plugin_ghtiles-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3002 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/README.md
+-rw-r--r--   0        0        0     7248 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/config.py
+-rw-r--r--   0        0        0     2303 2024-04-07 09:32:07.684982 nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/utils.py
+-rw-r--r--   0        0        0     1172 2024-04-07 09:32:20.524912 nonebot_plugin_ghtiles-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.3/PKG-INFO
```

### Comparing `nonebot_plugin_ghtiles-0.1.2/LICENSE` & `nonebot_plugin_ghtiles-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.2/README.md` & `nonebot_plugin_ghtiles-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/__init__.py` & `nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 
 # messages
 def tile_msg(username: str, contributions: int):
     logger.debug(
         f"triggered tile_msg, username: {username}, contributions: {contributions}"
     )
     if contributions == 0:
-        return UniMessage(f"{username} 还没有贴瓷砖")
+        return UniMessage(f"{username} 今天还没有贴瓷砖")
     else:
         return UniMessage(f"{username} 在 {get_today()} 贴了 {contributions} 个瓷砖")
 
 
 def winner_msg(username: str, contributions: int):
     return UniMessage(f"今天的瓷砖王是 {username}，贴了 {contributions} 个瓷砖！")
```

### Comparing `nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/utils.py` & `nonebot_plugin_ghtiles-0.1.3/nonebot_plugin_ghtiles/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,19 @@
     soup = BeautifulSoup(gh_html, "html.parser")
     contributions = 0
     if soup.tbody is None:
         return contributions
     tt = soup.tbody("tool-tip")
     today_index = next((index for index, td in enumerate(soup.tbody("td", class_="ContributionCalendar-day")) if td.get('data-date') == get_today()), None)
     if today_index is not None:
-        search = re.search(r'\d+', tt[today_index].text)
-        if search is not None:
-            contributions = int(search.group())
+        search = re.compile(r"(\d+|No) contribution").search(tt[today_index].text)
+        if search:
+            if search.group(1) == "No":
+                return contributions
+            contributions = int(search.group(1))
     return contributions
 
 class AutoSave:
     def __init__(self, fileProxy: Path, proxy: dict = None, initial_data: dict = None): # type: ignore
         self._fileProxy = fileProxy
         if proxy is None:
             if fileProxy.exists():
```

### Comparing `nonebot_plugin_ghtiles-0.1.2/pyproject.toml` & `nonebot_plugin_ghtiles-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-ghtiles"
-version = "0.1.2"
+version = "0.1.3"
 description = "A nonebot2 plugin for show GitHub contributions"
 readme = "README.md"
 requires-python = ">=3.9, <4.0"
 dependencies = [
     "nonebot2>=2.2.0",
     "httpx~=0.27",
     "nonebot-plugin-alconna>=0.38.1",
```

### Comparing `nonebot_plugin_ghtiles-0.1.2/PKG-INFO` & `nonebot_plugin_ghtiles-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ghtiles
-Version: 0.1.2
+Version: 0.1.3
 Summary: A nonebot2 plugin for show GitHub contributions
 Home-page: https://github.com/Lipraty/nonebot-plugin-ghtiles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/Lipraty/nonebot-plugin-ghtiles
 Requires-Python: <4.0,>=3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.3 Summary: A
 nonebot2 plugin for show GitHub contributions Home-page: https://github.com/
 Lipraty/nonebot-plugin-ghtiles Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Project-URL: Homepage, https://github.com/Lipraty/nonebot-
 plugin-ghtiles Requires-Python: <4.0,>=3.9 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: httpx~=0.27 Requires-Dist: nonebot-plugin-alconna>=0.38.1
 Requires-Dist: nonebot-plugin-apscheduler~=0.4 Requires-Dist: nonebot-plugin-
```

