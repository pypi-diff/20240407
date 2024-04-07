# Comparing `tmp/oru2xds-2.0.8.tar.gz` & `tmp/oru2xds-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oru2xds-2.0.8.tar", last modified: Sat Aug  6 21:13:51 2022, max compression
+gzip compressed data, was "oru2xds-2.0.9.tar", last modified: Sat Aug  6 21:15:32 2022, max compression
```

## Comparing `oru2xds-2.0.8.tar` & `oru2xds-2.0.9.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:13:51.753805 oru2xds-2.0.8/
--rw-rw-r--   0 antocm    (1000) antocm    (1000)    35150 2021-01-10 00:57:10.000000 oru2xds-2.0.8/LICENSE.md
--rw-rw-r--   0 antocm    (1000) antocm    (1000)    51351 2022-08-06 21:13:51.753805 oru2xds-2.0.8/PKG-INFO
--rw-rw-r--   0 antocm    (1000) antocm    (1000)    10297 2022-08-06 17:54:37.000000 oru2xds-2.0.8/README.md
--rw-r--r--   0 antocm    (1000) antocm    (1000)      804 2022-08-06 19:14:39.000000 oru2xds-2.0.8/pyproject.toml
--rw-rw-r--   0 antocm    (1000) antocm    (1000)       38 2022-08-06 21:13:51.753805 oru2xds-2.0.8/setup.cfg
-drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:13:51.753805 oru2xds-2.0.8/src/
-drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:13:51.753805 oru2xds-2.0.8/src/oru2xds/
--rw-rw-r--   0 antocm    (1000) antocm    (1000)        0 2022-08-06 19:22:23.000000 oru2xds-2.0.8/src/oru2xds/__init__.py
--rw-r--r--   0 antocm    (1000) antocm    (1000)       22 2022-08-06 21:13:30.000000 oru2xds-2.0.8/src/oru2xds/__version__.py
--rw-rw-r--   0 antocm    (1000) antocm    (1000)     1675 2022-07-10 20:44:47.000000 oru2xds-2.0.8/src/oru2xds/config.py
--rw-rw-r--   0 antocm    (1000) antocm    (1000)    50879 2022-07-12 21:46:43.000000 oru2xds-2.0.8/src/oru2xds/hl7_cda.py
--rw-rw-r--   0 antocm    (1000) antocm    (1000)     5668 2022-07-10 22:05:26.000000 oru2xds-2.0.8/src/oru2xds/hl7_v2x_receiver.py
--rw-rw-r--   0 antocm    (1000) antocm    (1000)   102065 2022-07-12 21:47:22.000000 oru2xds-2.0.8/src/oru2xds/ihe_xds.py
--rwxrw-r--   0 antocm    (1000) antocm    (1000)     4191 2022-08-06 19:21:57.000000 oru2xds-2.0.8/src/oru2xds/oru2xds.py
--rw-rw-r--   0 antocm    (1000) antocm    (1000)     9282 2022-07-12 21:47:56.000000 oru2xds-2.0.8/src/oru2xds/soap.py
-drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:13:51.753805 oru2xds-2.0.8/src/oru2xds.egg-info/
--rw-r--r--   0 antocm    (1000) antocm    (1000)    51351 2022-08-06 21:13:51.000000 oru2xds-2.0.8/src/oru2xds.egg-info/PKG-INFO
--rw-r--r--   0 antocm    (1000) antocm    (1000)      403 2022-08-06 21:13:51.000000 oru2xds-2.0.8/src/oru2xds.egg-info/SOURCES.txt
--rw-r--r--   0 antocm    (1000) antocm    (1000)        1 2022-08-06 21:13:51.000000 oru2xds-2.0.8/src/oru2xds.egg-info/dependency_links.txt
--rw-r--r--   0 antocm    (1000) antocm    (1000)       52 2022-08-06 21:13:51.000000 oru2xds-2.0.8/src/oru2xds.egg-info/requires.txt
--rw-r--r--   0 antocm    (1000) antocm    (1000)        8 2022-08-06 21:13:51.000000 oru2xds-2.0.8/src/oru2xds.egg-info/top_level.txt
+drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:15:32.950818 oru2xds-2.0.9/
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)    35150 2021-01-10 00:57:10.000000 oru2xds-2.0.9/LICENSE.md
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)    51351 2022-08-06 21:15:32.950818 oru2xds-2.0.9/PKG-INFO
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)    10297 2022-08-06 17:54:37.000000 oru2xds-2.0.9/README.md
+-rw-r--r--   0 antocm    (1000) antocm    (1000)      691 2022-08-06 21:15:26.000000 oru2xds-2.0.9/pyproject.toml
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)       38 2022-08-06 21:15:32.950818 oru2xds-2.0.9/setup.cfg
+drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:15:32.950818 oru2xds-2.0.9/src/
+drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:15:32.950818 oru2xds-2.0.9/src/oru2xds/
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)        0 2022-08-06 19:22:23.000000 oru2xds-2.0.9/src/oru2xds/__init__.py
+-rw-r--r--   0 antocm    (1000) antocm    (1000)       22 2022-08-06 21:14:00.000000 oru2xds-2.0.9/src/oru2xds/__version__.py
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)     1675 2022-07-10 20:44:47.000000 oru2xds-2.0.9/src/oru2xds/config.py
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)    50879 2022-07-12 21:46:43.000000 oru2xds-2.0.9/src/oru2xds/hl7_cda.py
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)     5668 2022-07-10 22:05:26.000000 oru2xds-2.0.9/src/oru2xds/hl7_v2x_receiver.py
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)   102065 2022-07-12 21:47:22.000000 oru2xds-2.0.9/src/oru2xds/ihe_xds.py
+-rwxrw-r--   0 antocm    (1000) antocm    (1000)     4191 2022-08-06 19:21:57.000000 oru2xds-2.0.9/src/oru2xds/oru2xds.py
+-rw-rw-r--   0 antocm    (1000) antocm    (1000)     9282 2022-07-12 21:47:56.000000 oru2xds-2.0.9/src/oru2xds/soap.py
+drwxrwxr-x   0 antocm    (1000) antocm    (1000)        0 2022-08-06 21:15:32.950818 oru2xds-2.0.9/src/oru2xds.egg-info/
+-rw-r--r--   0 antocm    (1000) antocm    (1000)    51351 2022-08-06 21:15:32.000000 oru2xds-2.0.9/src/oru2xds.egg-info/PKG-INFO
+-rw-r--r--   0 antocm    (1000) antocm    (1000)      369 2022-08-06 21:15:32.000000 oru2xds-2.0.9/src/oru2xds.egg-info/SOURCES.txt
+-rw-r--r--   0 antocm    (1000) antocm    (1000)        1 2022-08-06 21:15:32.000000 oru2xds-2.0.9/src/oru2xds.egg-info/dependency_links.txt
+-rw-r--r--   0 antocm    (1000) antocm    (1000)        8 2022-08-06 21:15:32.000000 oru2xds-2.0.9/src/oru2xds.egg-info/top_level.txt
```

### Comparing `oru2xds-2.0.8/LICENSE.md` & `oru2xds-2.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/PKG-INFO` & `oru2xds-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oru2xds
-Version: 2.0.8
+Version: 2.0.9
 Summary: Receive HL7 messages and send them to an XDS.b repository
 Author-email: Antonio Martins <digiplan.pt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `oru2xds-2.0.8/README.md` & `oru2xds-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/pyproject.toml` & `oru2xds-2.0.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -16,18 +16,10 @@
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
-dependencies = [
-    "lxml",
-    "aiorun",
-    "hl7",
-    "striprtf",
-    "requests",
-    "requests-toolbelt",
-]
 
 [tool.setuptools.dynamic]
 version = {attr = "oru2xds/__version__.__version__"}
```

### Comparing `oru2xds-2.0.8/src/oru2xds/config.py` & `oru2xds-2.0.9/src/oru2xds/config.py`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/src/oru2xds/hl7_cda.py` & `oru2xds-2.0.9/src/oru2xds/hl7_cda.py`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/src/oru2xds/hl7_v2x_receiver.py` & `oru2xds-2.0.9/src/oru2xds/hl7_v2x_receiver.py`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/src/oru2xds/ihe_xds.py` & `oru2xds-2.0.9/src/oru2xds/ihe_xds.py`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/src/oru2xds/oru2xds.py` & `oru2xds-2.0.9/src/oru2xds/oru2xds.py`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/src/oru2xds/soap.py` & `oru2xds-2.0.9/src/oru2xds/soap.py`

 * *Files identical despite different names*

### Comparing `oru2xds-2.0.8/src/oru2xds.egg-info/PKG-INFO` & `oru2xds-2.0.9/src/oru2xds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oru2xds
-Version: 2.0.8
+Version: 2.0.9
 Summary: Receive HL7 messages and send them to an XDS.b repository
 Author-email: Antonio Martins <digiplan.pt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

