# Comparing `tmp/mimic_replay-1.1.3.tar.gz` & `tmp/mimic_replay-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimic_replay-1.1.3.tar", last modified: Thu Apr  4 18:23:33 2024, max compression
+gzip compressed data, was "mimic_replay-1.1.4.tar", last modified: Sun Apr  7 17:18:14 2024, max compression
```

## Comparing `mimic_replay-1.1.3.tar` & `mimic_replay-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:23:33.908422 mimic_replay-1.1.3/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-03-29 16:37:37.000000 mimic_replay-1.1.3/LICENSE
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 18:23:33.908422 mimic_replay-1.1.3/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      458 2024-04-04 17:55:01.000000 mimic_replay-1.1.3/README.md
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      869 2024-04-04 18:23:07.000000 mimic_replay-1.1.3/pyproject.toml
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-04 18:23:33.908422 mimic_replay-1.1.3/setup.cfg
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:23:33.908422 mimic_replay-1.1.3/src/
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:23:33.908422 mimic_replay-1.1.3/src/mimic_replay/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-03-29 16:39:06.000000 mimic_replay-1.1.3/src/mimic_replay/__init__.py
--rw-rw-r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-03-29 20:07:26.000000 mimic_replay-1.1.3/src/mimic_replay/config.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1202 2024-04-04 18:22:54.000000 mimic_replay-1.1.3/src/mimic_replay/injector.py
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     3041 2024-04-04 18:22:55.000000 mimic_replay-1.1.3/src/mimic_replay/install.py
-drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-04 18:23:33.908422 mimic_replay-1.1.3/src/mimic_replay.egg-info/
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-04 18:23:33.000000 mimic_replay-1.1.3/src/mimic_replay.egg-info/PKG-INFO
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-04 18:23:33.000000 mimic_replay-1.1.3/src/mimic_replay.egg-info/SOURCES.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-04 18:23:33.000000 mimic_replay-1.1.3/src/mimic_replay.egg-info/dependency_links.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       25 2024-04-04 18:23:33.000000 mimic_replay-1.1.3/src/mimic_replay.egg-info/requires.txt
--rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-04 18:23:33.000000 mimic_replay-1.1.3/src/mimic_replay.egg-info/top_level.txt
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1062 2024-03-29 16:37:37.000000 mimic_replay-1.1.4/LICENSE
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      458 2024-04-04 19:03:46.000000 mimic_replay-1.1.4/README.md
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      869 2024-04-07 17:18:05.000000 mimic_replay-1.1.4/pyproject.toml
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       38 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/setup.cfg
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.800368 mimic_replay-1.1.4/src/
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/src/mimic_replay/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-03-29 16:39:06.000000 mimic_replay-1.1.4/src/mimic_replay/__init__.py
+-rw-rw-r--   0 veronika_todd  (1000) veronika_todd  (1000)     9039 2024-03-29 20:07:26.000000 mimic_replay-1.1.4/src/mimic_replay/config.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1202 2024-04-04 19:06:47.000000 mimic_replay-1.1.4/src/mimic_replay/injector.py
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     3120 2024-04-07 17:13:30.000000 mimic_replay-1.1.4/src/mimic_replay/install.py
+drwxr-xr-x   0 veronika_todd  (1000) veronika_todd  (1000)        0 2024-04-07 17:18:14.810368 mimic_replay-1.1.4/src/mimic_replay.egg-info/
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)     1214 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/PKG-INFO
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)      344 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/SOURCES.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)        1 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/dependency_links.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       25 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/requires.txt
+-rw-r--r--   0 veronika_todd  (1000) veronika_todd  (1000)       13 2024-04-07 17:18:14.000000 mimic_replay-1.1.4/src/mimic_replay.egg-info/top_level.txt
```

### Comparing `mimic_replay-1.1.3/LICENSE` & `mimic_replay-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.3/PKG-INFO` & `mimic_replay-1.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimic_replay
-Version: 1.1.3
+Version: 1.1.4
 Summary: MIMIC installation script, which enables your application to communicate with your MIMIC server.
 Author-email: Veronika Todd <veronika.todd@gmail.com>, Lucas Sorribes <lucas.sorribes@gmail.com>, Erik Wiens <erik.wiens@gmail.com>, Louis Mascari <lmascari16@gmail.com>
 Project-URL: MIMIC, https://mimic-replay.com
 Project-URL: Github, https://github.com/2401-Team-4/capstone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mimic_replay-1.1.3/pyproject.toml` & `mimic_replay-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mimic_replay"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Veronika Todd", email="veronika.todd@gmail.com" },
   { name="Lucas Sorribes", email="lucas.sorribes@gmail.com" },
   { name="Erik Wiens", email="erik.wiens@gmail.com" },
   { name="Louis Mascari", email="lmascari16@gmail.com" }
 ]
 dependencies = [
```

### Comparing `mimic_replay-1.1.3/src/mimic_replay/config.py` & `mimic_replay-1.1.4/src/mimic_replay/config.py`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.3/src/mimic_replay/injector.py` & `mimic_replay-1.1.4/src/mimic_replay/injector.py`

 * *Files identical despite different names*

### Comparing `mimic_replay-1.1.3/src/mimic_replay/install.py` & `mimic_replay-1.1.4/src/mimic_replay/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,16 +24,19 @@
   print("🎉 Connection to MIMIC server successful 🎉")  
   return backendUrl  
 
 
 def send_project_info(name, password, backendUrl):
   r = requests.post(f'{backendUrl}/api/project/new', json={ 'projectId': UNIQUE_PROJECT_ID, "name": name, "password": password })
   print("🔹 Sending new project information to MIMIC server...")
-  print("🔹", r.status_code, r.reason)
-  print("🔥 MIMIC is successfully installed 🔥") if r.status_code == 200 else print("💔 There was an error installing MIMIC 💔")
+  if r.status_code == 200:
+    print("🔹 Credentials received by MIMIC server!")
+    print("🔥 MIMIC is successfully installed 🔥")
+  else:
+    print("💔 There was an error communicating with to your MIMIC server, installer unable to proceed 💔")
   
 def credentials(backendUrl):
   unique_name = False
   while unique_name == False:
     name = name_credentials()
     r = requests.post(f'{backendUrl}/api/project/validate', json={ "name": name })
     if r.status_code == 200:
```

### Comparing `mimic_replay-1.1.3/src/mimic_replay.egg-info/PKG-INFO` & `mimic_replay-1.1.4/src/mimic_replay.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimic_replay
-Version: 1.1.3
+Version: 1.1.4
 Summary: MIMIC installation script, which enables your application to communicate with your MIMIC server.
 Author-email: Veronika Todd <veronika.todd@gmail.com>, Lucas Sorribes <lucas.sorribes@gmail.com>, Erik Wiens <erik.wiens@gmail.com>, Louis Mascari <lmascari16@gmail.com>
 Project-URL: MIMIC, https://mimic-replay.com
 Project-URL: Github, https://github.com/2401-Team-4/capstone
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

