# Comparing `tmp/eezo-0.1.6.tar.gz` & `tmp/eezo-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eezo-0.1.6.tar", last modified: Thu Apr  4 16:48:48 2024, max compression
+gzip compressed data, was "eezo-0.1.7.tar", last modified: Sun Apr  7 18:36:10 2024, max compression
```

## Comparing `eezo-0.1.6.tar` & `eezo-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.212256 eezo-0.1.6/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-04 16:48:48.212136 eezo-0.1.6/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.6/README.md
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.208804 eezo-0.1.6/eezo/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.6/eezo/async_client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-03-27 15:07:04.000000 eezo-0.1.6/eezo/client.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)    11051 2024-04-04 16:40:31.000000 eezo-0.1.6/eezo/connector.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.210222 eezo-0.1.6/eezo/interface/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       78 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/__init__.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.211944 eezo-0.1.6/eezo/interface/components/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/__init__.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/chart.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/component.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/image.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/text.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/components/youtube_video.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     3027 2024-03-19 14:09:37.000000 eezo-0.1.6/eezo/interface/interface.py
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.6/eezo/interface/message.py
-drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-04 16:48:48.209596 eezo-0.1.6/eezo.egg-info/
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/PKG-INFO
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      533 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/SOURCES.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/dependency_links.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)      353 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/requires.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-04 16:48:48.000000 eezo-0.1.6/eezo.egg-info/top_level.txt
--rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-04 16:48:48.212291 eezo-0.1.6/setup.cfg
--rw-r--r--   0 danielschonbohm   (501) staff       (20)     1921 2024-04-04 16:45:52.000000 eezo-0.1.6/setup.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.626244 eezo-0.1.7/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-07 18:36:10.626134 eezo-0.1.7/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1558 2024-03-19 14:53:56.000000 eezo-0.1.7/README.md
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.622838 eezo-0.1.7/eezo/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       86 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4495 2024-04-02 19:37:54.000000 eezo-0.1.7/eezo/async_client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     4542 2024-03-27 15:07:04.000000 eezo-0.1.7/eezo/client.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)    11110 2024-04-07 18:16:52.000000 eezo-0.1.7/eezo/connector.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.624104 eezo-0.1.7/eezo/interface/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       78 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/__init__.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.625959 eezo-0.1.7/eezo/interface/components/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      329 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/__init__.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1743 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/chart.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      159 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/component.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      243 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/image.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      246 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/text.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      283 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/components/youtube_video.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     3085 2024-04-07 18:22:55.000000 eezo-0.1.7/eezo/interface/interface.py
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1330 2024-03-19 12:03:08.000000 eezo-0.1.7/eezo/interface/message.py
+drwxr-xr-x   0 danielschonbohm   (501) staff       (20)        0 2024-04-07 18:36:10.623530 eezo-0.1.7/eezo.egg-info/
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1259 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/PKG-INFO
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      533 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/SOURCES.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        1 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/dependency_links.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)      353 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/requires.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)        5 2024-04-07 18:36:10.000000 eezo-0.1.7/eezo.egg-info/top_level.txt
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)       38 2024-04-07 18:36:10.626280 eezo-0.1.7/setup.cfg
+-rw-r--r--   0 danielschonbohm   (501) staff       (20)     1921 2024-04-07 18:26:49.000000 eezo-0.1.7/setup.py
```

### Comparing `eezo-0.1.6/PKG-INFO` & `eezo-0.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.6
+Version: 0.1.7
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.6/README.md` & `eezo-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `eezo-0.1.6/eezo/async_client.py` & `eezo-0.1.7/eezo/async_client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.6/eezo/client.py` & `eezo-0.1.7/eezo/client.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.6/eezo/connector.py` & `eezo-0.1.7/eezo/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         else:
             raise Exception(f"{response.status_code}: {response.json()['detail']}")
 
     def __get_job_result(self, job_id):
         while True:
             if job_id in self.job_responses:
                 response = self.job_responses.pop(job_id)
-                self.__log(f"<< Sub Job {job_id} completed")
+                self.__log(f"<< Sub Job {job_id} completed.")
 
                 if not response.get("success", True):
                     self.__log(
                         f" ✖ Sub Job {response['id']} failed:\n{response['traceback']}."
                     )
                     raise Exception(response["error"])
 
@@ -267,16 +267,19 @@
             lambda: self.__log(f" ✖ Connector {self.connector_id} disconnected"),
         )
 
         def auth_error(message: str):
             self.__log(f" ✖ Authentication failed: {message}")
             self.run_loop = False
 
+        def job_response(response):
+            self.job_responses[response["id"]] = response
+
         self.sio.on("job_request", lambda p: self.__execute_job(p))
-        self.sio.on("job_response", lambda p: self.job_responses.update({p["id"]: p}))
+        self.sio.on("job_response", job_response)
         self.sio.on("token_expired", lambda: self.__authenticate())
         self.sio.on("auth_error", auth_error)
 
         while self.run_loop:
             try:
                 self.sio.connect(SERVER)
                 self.sio.wait()
```

### Comparing `eezo-0.1.6/eezo/interface/components/chart.py` & `eezo-0.1.7/eezo/interface/components/chart.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.6/eezo/interface/interface.py` & `eezo-0.1.7/eezo/interface/interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,17 @@
                 "skill_id": skill_id,
                 "skill_payload": kwargs,
             }
         )
         return await self.get_result(job_id)
 
     async def get_thread(self, nr=5, to_string=False):
-        await self._run(skill_id="s_get_thread", nr_of_messages=nr, to_string=to_string)
+        return await self._run(
+            skill_id="s_get_thread", nr_of_messages=nr, to_string=to_string
+        )
 
     async def invoke(self, agent_id, **kwargs):
         return await self._run(skill_id=agent_id, **kwargs)
 
 
 class Interface:
     def __init__(
@@ -94,11 +96,13 @@
                 "skill_id": skill_id,
                 "skill_payload": kwargs,
             }
         )
         return self.get_result(job_id)
 
     def get_thread(self, nr=5, to_string=False):
-        self._run(skill_id="s_get_thread", nr_of_messages=nr, to_string=to_string)
+        return self._run(
+            skill_id="s_get_thread", nr_of_messages=nr, to_string=to_string
+        )
 
     def invoke(self, agent_id, **kwargs):
         return self._run(skill_id=agent_id, **kwargs)
```

### Comparing `eezo-0.1.6/eezo/interface/message.py` & `eezo-0.1.7/eezo/interface/message.py`

 * *Files identical despite different names*

### Comparing `eezo-0.1.6/eezo.egg-info/PKG-INFO` & `eezo-0.1.7/eezo.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eezo
-Version: 0.1.6
+Version: 0.1.7
 Summary: Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.
 Home-page: UNKNOWN
 Author: Daniel Schoenbohm
 Author-email: daniel@eezo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `eezo-0.1.6/eezo.egg-info/SOURCES.txt` & `eezo-0.1.7/eezo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eezo-0.1.6/setup.py` & `eezo-0.1.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="eezo",
-    version="0.1.6",
+    version="0.1.7",
     description="Eezo's Dashboard streamlines the management of AI agents via its API, offering a user-friendly interface that requires minimal coding. It enables easy access for all team members, fostering agent interaction and collaboration. The platform also features real-time data sharing with interactive charts, making it an ideal solution for developers and companies looking to centralize their AI tools and processes.",
     author="Daniel Schoenbohm",
     author_email="daniel@eezo.ai",
     packages=find_packages(),
     install_requires=[
         "aiohttp==3.9.3",
         "aiosignal==1.3.1",
```

