# Comparing `tmp/pyaffalddk-2.0.21.tar.gz` & `tmp/pyaffalddk-2.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaffalddk-2.0.21.tar", last modified: Fri Apr  5 04:02:57 2024, max compression
+gzip compressed data, was "pyaffalddk-2.0.22.tar", last modified: Sun Apr  7 11:55:53 2024, max compression
```

## Comparing `pyaffalddk-2.0.21.tar` & `pyaffalddk-2.0.22.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/pyaffalddk/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/pyaffalddk/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/pyaffalddk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-05 04:02:57.000000 pyaffalddk-2.0.21/pyaffalddk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 04:02:57.319516 pyaffalddk-2.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 04:02:53.000000 pyaffalddk-2.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/pyaffalddk/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11021 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/pyaffalddk/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/pyaffalddk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 11:55:53.000000 pyaffalddk-2.0.22/pyaffalddk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 11:55:53.192197 pyaffalddk-2.0.22/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-07 11:55:42.000000 pyaffalddk-2.0.22/setup.py
```

### Comparing `pyaffalddk-2.0.21/LICENSE` & `pyaffalddk-2.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.21/PKG-INFO` & `pyaffalddk-2.0.22/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.21
+Version: 2.0.22
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.21/pyaffalddk/api.py` & `pyaffalddk-2.0.22/pyaffalddk/api.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.21/pyaffalddk/const.py` & `pyaffalddk-2.0.22/pyaffalddk/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     ],
     "farligtaffald": [
         "",
     ],
     "farligtaffaldmiljoboks": [
         "Miljøkasse (1 stk.)",
         "Miljøboks",
+        "Rød kasse henteordning (1 stk.)",
     ],
     "flis": [""],
     "jern": [""],
     "genbrug": [
         "Tekstiler",
         "Genbrug",
         "Genbrugsøer",
@@ -219,20 +220,22 @@
     ],
     "storskrald": [
         "Storskrald - fortovsindsamling (1 stk.)",
     ],
     "storskraldogtekstilaffald": [""],
     "haveaffald": [
         "Gen-Skel 0-2 meter (1 stk.)",
+        "Haveaffald henteordning (1 stk.)",
     ],
     "papirglas": [
         "Papir/glas - 240 l. fortovsindsamling (1 stk.)",
     ],
     "plastmadkarton": [
         "Genbrugsbeholder PMDK/MG-240L/3uge (1 stk.)",
+        "Genbrug henteordning (1 stk.)",
     ],
     "papirglasdaaser": [
         "240 L 2-delt Papir/glas-dåser en-familie (1 stk.)",
     ],
     "pappapirglasmetal": [
         "240L metal, glas, plast/papir gl. (1 stk.)",
         "240 l genbrug 2-kammer (2023) (1 stk.)",
@@ -248,14 +251,15 @@
         "Tekstilpose tømning (1 stk.)",
     ],
     "glasplast": [""],
     "plastmetalpapir": [""],
     "papirglasmetalplast": [
         "4-kammer (370 l) (1 stk.)",
         "Pap og papir/metal, glas og hård plast - 240 L (1 stk.)",
+        "240 l genbrug låg i låg (1 stk.)"
     ],
 }
 
 ICON_LIST = {
     "batterier": "mdi:battery",
     "elektronik": "mdi:power-plug",
     "restaffaldmadaffald": "mdi:trash-can",
@@ -379,7 +383,8 @@
     "Vejen": "vejen",
     "Vordingborg": "vordingborg",
 }
 
 MUNICIPALITIES_ARRAY = list(MUNICIPALITIES_LIST.keys())
 
 WEEKDAYS = ["Mandag", "Tirsdag", "Onsdag", "Torsdag", "Fredag", "Lørdag", "Søndag"]
+WEEKDAYS_SHORT = ["Man", "Tir", "Ons", "Tor", "Fre", "Lør", "Søn"]
```

### Comparing `pyaffalddk-2.0.21/pyaffalddk/data.py` & `pyaffalddk-2.0.22/pyaffalddk/data.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.21/pyaffalddk/images.py` & `pyaffalddk-2.0.22/pyaffalddk/images.py`

 * *Files identical despite different names*

### Comparing `pyaffalddk-2.0.21/pyaffalddk.egg-info/PKG-INFO` & `pyaffalddk-2.0.22/pyaffalddk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaffalddk
-Version: 2.0.21
+Version: 2.0.22
 Summary: Gets garbage collection data from danish Municipalities
 Home-page: https://github.com/briis/pyaffalddk
 Author: briis
 Author-email: bjarne@briis.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyaffalddk-2.0.21/setup.py` & `pyaffalddk-2.0.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyaffalddk",
-    version="2.0.21",
+    version="2.0.22",
     author="briis",
     author_email="bjarne@briis.com",
     description="Gets garbage collection data from danish Municipalities",
     license="MIT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/briis/pyaffalddk",
```

