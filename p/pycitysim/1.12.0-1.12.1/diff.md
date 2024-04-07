# Comparing `tmp/pycitysim-1.12.0.tar.gz` & `tmp/pycitysim-1.12.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycitysim-1.12.0.tar", last modified: Tue Mar 26 08:08:39 2024, max compression
+gzip compressed data, was "pycitysim-1.12.1.tar", last modified: Sun Apr  7 14:04:27 2024, max compression
```

## Comparing `pycitysim-1.12.0.tar` & `pycitysim-1.12.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.328617 pycitysim-1.12.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-26 08:08:34.000000 pycitysim-1.12.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-03-26 08:08:39.328617 pycitysim-1.12.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-26 08:08:34.000000 pycitysim-1.12.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.320618 pycitysim-1.12.0/pycitysim/
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.324617 pycitysim-1.12.0/pycitysim/apphub/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/apphub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/apphub/apphub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.324617 pycitysim-1.12.0/pycitysim/map/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/map/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/map/map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.324617 pycitysim-1.12.0/pycitysim/routing/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/routing/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.324617 pycitysim-1.12.0/pycitysim/sidecar/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sidecar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sidecar/sidecar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.324617 pycitysim-1.12.0/pycitysim/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/aoi_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/clock_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/economy_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/event_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/lane_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/light_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/person_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/road_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/sim/social_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.324617 pycitysim-1.12.0/pycitysim/urbankg/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/urbankg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/urbankg/kg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.324617 pycitysim-1.12.0/pycitysim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/utils/geojson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/utils/grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pycitysim/utils/protobuf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 08:08:39.328617 pycitysim-1.12.0/pycitysim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-03-26 08:08:39.000000 pycitysim-1.12.0/pycitysim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-03-26 08:08:39.000000 pycitysim-1.12.0/pycitysim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 08:08:39.000000 pycitysim-1.12.0/pycitysim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-26 08:08:39.000000 pycitysim-1.12.0/pycitysim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-26 08:08:39.000000 pycitysim-1.12.0/pycitysim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-26 08:08:34.000000 pycitysim-1.12.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 08:08:39.328617 pycitysim-1.12.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-07 14:04:19.000000 pycitysim-1.12.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-07 14:04:27.887297 pycitysim-1.12.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-07 14:04:19.000000 pycitysim-1.12.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.879298 pycitysim-1.12.1/pycitysim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/apphub/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/apphub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9986 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/apphub/apphub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/map/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/map/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35545 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/map/map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/routing/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/routing/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.883298 pycitysim-1.12.1/pycitysim/sidecar/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sidecar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sidecar/sidecar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/aoi_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/clock_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7093 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/economy_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/event_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/lane_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/light_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/person_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/road_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/sim/social_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim/urbankg/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/urbankg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/urbankg/kg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/geojson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pycitysim/utils/protobuf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:04:27.887297 pycitysim-1.12.1/pycitysim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 14:04:27.000000 pycitysim-1.12.1/pycitysim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-07 14:04:19.000000 pycitysim-1.12.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:04:27.887297 pycitysim-1.12.1/setup.cfg
```

### Comparing `pycitysim-1.12.0/LICENSE` & `pycitysim-1.12.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/PKG-INFO` & `pycitysim-1.12.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.12.0
+Version: 1.12.1
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycitysim-1.12.0/README.md` & `pycitysim-1.12.1/README.md`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/__init__.py` & `pycitysim-1.12.1/pycitysim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/apphub/apphub.py` & `pycitysim-1.12.1/pycitysim/apphub/apphub.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,15 @@
             "foreignID": foreign_id,
         }
         res = requests.post(
             self.app_hub_url + "/agents",
             json=body,
             auth=self._auth,
             proxies=self.proxies,
+            timeout=5000
         )
         if res.status_code != 200:
             raise Exception(f"[{res.status_code}] AppHub bind failed: " + res.text)
         data = res.json()
         agent_id = data["data"]["id"]
         self.agents[agent_id] = body
         return agent_id
@@ -166,30 +167,41 @@
         Returns:
         - agent_id: 绑定后的agent ID。the bound agent ID.
 
         Raises:
         - Exception: 绑定失败。Binding failed.
         """
         return self._bind(org_id, "org", name, avatar)
+    
+    def bind_func(self, name:str, avatar:Image):
+        """
+        插入非模拟器相关的智能体——func类型智能体
+
+        Args:
+        - name (str): 该智能体的名字
+        - avatar (Image): 该智能体的头像
+        """
+        return self._bind(-1, "func", name, avatar)
 
     def release_agent(self, agent_id: int) -> bool:
         """
-        释放agent(person/org)，释放后agent将不再被访问并允许其他app绑定
+        释放agent(person/org), 释放后agent将不再被访问并允许其他app绑定
         Release the agent (person/org). After the release, the agent will no longer be accessed and allows other apps to bind.
 
         Args:
         - agent_id: agent的ID。ID of the agent.
 
         Returns:
         - bool: 是否成功。whether succeed.
         """
         res = requests.delete(
             self.app_hub_url + "/agents/" + str(agent_id),
             auth=self._auth,
             proxies=self.proxies,
+            timeout=5000
         )
         return res.status_code == 200
 
     def update_agent_map(
         self,
         agent_id: int,
         lnglat: List[float],
@@ -223,14 +235,15 @@
             body["popup"] = popup
 
         res = requests.put(
             self.app_hub_url + "/agents/" + str(agent_id) + "/map",
             json=body,
             auth=self._auth,
             proxies=self.proxies,
+            timeout=5000
         )
         if res.status_code != 200:
             raise Exception(
                 f"[{res.status_code}] AppHub update map failed: " + res.text
             )
 
     def update_agent_messages(self, agent_id: int, messages: List[AgentMessage]):
@@ -246,14 +259,15 @@
         - Exception: 更新失败。Updating failed.
         """
         res = requests.put(
             self.app_hub_url + "/agents/" + str(agent_id) + "/messages",
             json={"messages": [message.to_dict() for message in messages]},
             auth=self._auth,
             proxies=self.proxies,
+            timeout=5000
         )
         if res.status_code != 200:
             raise Exception(
                 f"[{res.status_code}] AppHub update messages failed: " + res.text
             )
 
     def fetch_user_messages(
@@ -273,14 +287,15 @@
         Raises:
         - Exception: 获取失败。Fetching failed.
         """
         res = requests.post(
             self.app_hub_url + "/agents/" + str(agent_id) + "/fetch-user-messages",
             auth=self._auth,
             proxies=self.proxies,
+            timeout=5000
         )
         if res.status_code != 200:
             raise Exception(
                 f"[{res.status_code}] AppHub fetch messages failed: " + res.text
             )
         data = res.json()
         return [UserMessage(**message) for message in data["data"]]
```

### Comparing `pycitysim-1.12.0/pycitysim/map/map.py` & `pycitysim-1.12.1/pycitysim/map/map.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/routing/client.py` & `pycitysim-1.12.1/pycitysim/routing/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sidecar/sidecar.py` & `pycitysim-1.12.1/pycitysim/sidecar/sidecar.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/__init__.py` & `pycitysim-1.12.1/pycitysim/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/aoi_service.py` & `pycitysim-1.12.1/pycitysim/sim/aoi_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/client.py` & `pycitysim-1.12.1/pycitysim/sim/client.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/clock_service.py` & `pycitysim-1.12.1/pycitysim/sim/clock_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/economy_services.py` & `pycitysim-1.12.1/pycitysim/sim/economy_services.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/event_service.py` & `pycitysim-1.12.1/pycitysim/sim/event_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/lane_service.py` & `pycitysim-1.12.1/pycitysim/sim/lane_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/light_service.py` & `pycitysim-1.12.1/pycitysim/sim/light_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/person_service.py` & `pycitysim-1.12.1/pycitysim/sim/person_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/road_service.py` & `pycitysim-1.12.1/pycitysim/sim/road_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/sim/social_service.py` & `pycitysim-1.12.1/pycitysim/sim/social_service.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/urbankg/kg.py` & `pycitysim-1.12.1/pycitysim/urbankg/kg.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/utils/geojson.py` & `pycitysim-1.12.1/pycitysim/utils/geojson.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/utils/grpc.py` & `pycitysim-1.12.1/pycitysim/utils/grpc.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim/utils/protobuf.py` & `pycitysim-1.12.1/pycitysim/utils/protobuf.py`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pycitysim.egg-info/PKG-INFO` & `pycitysim-1.12.1/pycitysim.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycitysim
-Version: 1.12.0
+Version: 1.12.1
 Summary: City Simulator and OpenCity Databases Python SDK
 Author-email: Jun Zhang <zhangjun990222@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycitysim-1.12.0/pycitysim.egg-info/SOURCES.txt` & `pycitysim-1.12.1/pycitysim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycitysim-1.12.0/pyproject.toml` & `pycitysim-1.12.1/pyproject.toml`

 * *Files identical despite different names*

