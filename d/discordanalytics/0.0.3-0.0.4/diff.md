# Comparing `tmp/discordanalytics-0.0.3.tar.gz` & `tmp/discordanalytics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discordanalytics-0.0.3.tar", last modified: Sat Apr  6 18:41:14 2024, max compression
+gzip compressed data, was "discordanalytics-0.0.4.tar", last modified: Sun Apr  7 14:42:11 2024, max compression
```

## Comparing `discordanalytics-0.0.3.tar` & `discordanalytics-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:41:14.413436 discordanalytics-0.0.3/discordanalytics/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/discordanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/discordanalytics/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/discordanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-06 18:41:14.000000 discordanalytics-0.0.3/discordanalytics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-06 18:41:09.000000 discordanalytics-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:41:14.417436 discordanalytics-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:42:11.865636 discordanalytics-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-07 14:42:11.861636 discordanalytics-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:42:11.861636 discordanalytics-0.0.4/discordanalytics/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/discordanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/discordanalytics/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:42:11.861636 discordanalytics-0.0.4/discordanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-07 14:42:11.000000 discordanalytics-0.0.4/discordanalytics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-07 14:42:07.000000 discordanalytics-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:42:11.865636 discordanalytics-0.0.4/setup.cfg
```

### Comparing `discordanalytics-0.0.3/LICENSE` & `discordanalytics-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `discordanalytics-0.0.3/PKG-INFO` & `discordanalytics-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordanalytics
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for interacting with Discord Analytics API
 Author-email: ValDesign <valdesign.dev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Discord Analytics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `discordanalytics-0.0.3/README.md` & `discordanalytics-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `discordanalytics-0.0.3/discordanalytics/client.py` & `discordanalytics-0.0.4/discordanalytics/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,17 @@
       "Content-Type": "application/json",
       "Authorization": f"Bot {api_key}"
     }
     self.stats = {
       "date": datetime.today().strftime("%Y-%m-%d"),
       "guilds": 0,
       "users": 0,
-      "interactions": [],
-      "locales": [],
-      "guildsLocales": [],
+      "interactions": [], # {name:str, number:int, type:int}[]
+      "locales": [], # {locale:str, number:int}[]
+      "guildsLocales": [], # {locale:str, number:int}[]
       "guildMembers": {
         "little": 0,
         "medium": 0,
         "big": 0,
         "huge": 0
       }
     }
@@ -159,55 +159,55 @@
     
     guilds = []
     for guild in self.client.guilds:
       if guild.preferred_locale is not None:
         found = False
         for g in guilds:
           if g["locale"] == guild.preferred_locale.value:
-            g["count"] += 1
+            g["number"] += 1
             found = True
             break
         if not found:
           guilds.append({
             "locale": guild.preferred_locale.value,
-            "count": 1
+            "number": 1
           })
     self.stats["guildsLocales"] = guilds
     
     found = False
     for data in self.stats["locales"]:
       if data["locale"] == interaction.locale.value:
-        data["count"] += 1
+        data["number"] += 1
         found = True
         break
     if not found:
       self.stats["locales"].append({
         "locale": interaction.locale.value,
-        "count": 1
+        "number": 1
       })
 
     if interaction.type == InteractionType.application_command or interaction.type == InteractionType.autocomplete:
       found = False
       for data in self.stats["interactions"]:
         if data["name"] == interaction.data["name"] and data["type"] == interaction.type.value:
-          data["count"] += 1
+          data["number"] += 1
           found = True
           break
       if not found:
         self.stats["interactions"].append({
           "name": interaction.data["name"],
-          "count": 1,
+          "number": 1,
           "type": interaction.type.value
         })
     elif interaction.type == InteractionType.component or interaction.type == InteractionType.modal_submit:
       found = False
       for data in self.stats["interactions"]:
         if data["name"] == interaction.data["custom_id"] and data["type"] == interaction.type.value:
-          data["count"] += 1
+          data["number"] += 1
           found = True
           break
       if not found:
         self.stats["interactions"].append({
           "name": interaction.data["custom_id"],
-          "count": 1,
+          "number": 1,
           "type": interaction.type.value
         })
```

### Comparing `discordanalytics-0.0.3/discordanalytics.egg-info/PKG-INFO` & `discordanalytics-0.0.4/discordanalytics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discordanalytics
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for interacting with Discord Analytics API
 Author-email: ValDesign <valdesign.dev@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Discord Analytics
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

