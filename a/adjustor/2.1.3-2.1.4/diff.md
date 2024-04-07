# Comparing `tmp/adjustor-2.1.3.tar.gz` & `tmp/adjustor-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adjustor-2.1.3.tar", last modified: Thu Apr  4 16:58:01 2024, max compression
+gzip compressed data, was "adjustor-2.1.4.tar", last modified: Sun Apr  7 16:34:10 2024, max compression
```

## Comparing `adjustor-2.1.3.tar` & `adjustor-2.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-04 16:57:55.000000 adjustor-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-04 16:57:55.000000 adjustor-2.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-04 16:58:01.269585 adjustor-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-04 16:57:55.000000 adjustor-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-04 16:57:55.000000 adjustor-2.1.3/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 16:58:01.269585 adjustor-2.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.261585 adjustor-2.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.265585 adjustor-2.1.3/src/adjustor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/acpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/alib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/lenovo.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/core/platform.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/asus/
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/asus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/asus/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/lenovo/
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/lenovo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3629 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/lenovo/settings.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor/drivers/smu/
--rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/smu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/smu/qam.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/drivers/smu/smu.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/hhd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/settings.yml
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-04 16:57:55.000000 adjustor-2.1.3/src/adjustor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 16:58:01.269585 adjustor-2.1.3/src/adjustor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-04 16:58:01.000000 adjustor-2.1.3/src/adjustor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.368099 adjustor-2.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 16:34:04.000000 adjustor-2.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-07 16:34:04.000000 adjustor-2.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-07 16:34:10.364099 adjustor-2.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-07 16:34:04.000000 adjustor-2.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-07 16:34:04.000000 adjustor-2.1.4/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 16:34:10.368099 adjustor-2.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.360099 adjustor-2.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.360099 adjustor-2.1.4/src/adjustor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/acpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/alib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5753 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/lenovo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/core/platform.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/asus/
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/asus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/asus/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/lenovo/
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/lenovo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/lenovo/settings.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor/drivers/smu/
+-rw-r--r--   0 runner    (1001) docker     (127)    10254 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/smu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/smu/qam.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/drivers/smu/smu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7389 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/hhd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/settings.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-07 16:34:04.000000 adjustor-2.1.4/src/adjustor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 16:34:10.364099 adjustor-2.1.4/src/adjustor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 16:34:10.000000 adjustor-2.1.4/src/adjustor.egg-info/top_level.txt
```

### Comparing `adjustor-2.1.3/LICENSE` & `adjustor-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/PKG-INFO` & `adjustor-2.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adjustor
-Version: 2.1.3
+Version: 2.1.4
 Summary: Adjustor, a userspace program for managing the TDP of handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/adjustor
 Project-URL: Bug Tracker, https://github.com/hhd-dev/adjustor/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adjustor-2.1.3/pyproject.toml` & `adjustor-2.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "adjustor"
-version = "2.1.3"
+version = "2.1.4"
 authors = [
   { name="Kapenekakis Antheas", email="pypi@antheas.dev" },
 ]
 description = "Adjustor, a userspace program for managing the TDP of handheld devices."
 readme = "readme.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `adjustor-2.1.3/readme.md` & `adjustor-2.1.4/readme.md`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/core/acpi.py` & `adjustor-2.1.4/src/adjustor/core/acpi.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/core/alib.py` & `adjustor-2.1.4/src/adjustor/core/alib.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/core/const.py` & `adjustor-2.1.4/src/adjustor/core/const.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/core/lenovo.py` & `adjustor-2.1.4/src/adjustor/core/lenovo.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 def set_power_light(enabled: bool):
     logger.debug(f"Setting power light status.")
     return call(r"\_SB.GZFD.WMAF", [0, 0x02, bytes([0x03, int(enabled), 0x00])])
 
 
 def get_power_light():
-    logger.info(f"Getting power light status.")
+    logger.debug(f"Getting power light status.")
     if not call(r"\_SB.GZFD.WMAF", [0, 0x01, 0x03], risky=False):
         return None
     o = read()
     if isinstance(o, bytes) and len(o) == 2:
         return bool(o[0])
     return None
 
@@ -191,14 +191,24 @@
 
 
 def get_slow_tdp():
     logger.debug(f"Retrieving slow TDP.")
     return get_feature(0x0101FF00)
 
 
+def get_charge_limit():
+    logger.debug(f"Retrieving charge limit.")
+    return get_feature(0x03010001)
+
+
+def set_charge_limit(enable: bool):
+    logger.info(f"Setting charge limit (80 %) to {enable}.")
+    return set_feature(0x03010001, enable)
+
+
 def set_steady_tdp(val: int):
     logger.info(f"Setting steady TDP to {val}.")
     return set_feature(0x0102FF00, val)
 
 
 def set_fast_tdp(val: int):
     logger.info(f"Setting fast TDP to {val}.")
```

### Comparing `adjustor-2.1.3/src/adjustor/core/platform.py` & `adjustor-2.1.4/src/adjustor/core/platform.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/drivers/asus/__init__.py` & `adjustor-2.1.4/src/adjustor/drivers/asus/__init__.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/drivers/asus/settings.yml` & `adjustor-2.1.4/src/adjustor/drivers/asus/settings.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/drivers/lenovo/__init__.py` & `adjustor-2.1.4/src/adjustor/drivers/lenovo/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 from hhd.plugins import Context, HHDPlugin, HHDSettings, load_relative_yaml
 from hhd.plugins.conf import Config
 
 from adjustor.core.lenovo import (
     MIN_CURVE,
     TdpMode,
+    get_charge_limit,
     get_full_fan_speed,
     get_power_light,
     get_tdp_mode,
+    set_charge_limit,
     set_fan_curve,
     set_fast_tdp,
     set_full_fan_speed,
     set_power_light,
     set_slow_tdp,
     set_steady_tdp,
     set_tdp_mode,
@@ -80,14 +82,15 @@
         #
 
         # Initialize values so we do not query them all the time
         tdp_reset = self.startup
         if self.startup:
             conf["tdp.lenovo.ffss"] = get_full_fan_speed()
             conf["tdp.lenovo.power_light"] = get_power_light()
+            conf["tdp.lenovo.charge_limit"] = get_charge_limit()
 
         # If not old config, exit, as values can not be set
         if not self.old_conf:
             self.old_conf = conf["tdp.lenovo"]
             return
 
         curr = time.time()
@@ -101,14 +104,20 @@
 
         power_light = conf["tdp.lenovo.power_light"].to(bool)
         if power_light is not None and power_light != self.old_conf["power_light"].to(
             bool
         ):
             set_power_light(power_light)
 
+        charge_limit = conf["tdp.lenovo.charge_limit"].to(bool)
+        if charge_limit is not None and charge_limit != self.old_conf[
+            "charge_limit"
+        ].to(bool):
+            set_charge_limit(charge_limit)
+
         #
         # TDP
         #
 
         # Update tdp mode if user changed through the app
         mode = conf["tdp.lenovo.tdp.mode"].to(str)
         if mode is not None and mode != self.old_conf["tdp.mode"].to(str):
```

### Comparing `adjustor-2.1.3/src/adjustor/drivers/lenovo/settings.yml` & `adjustor-2.1.4/src/adjustor/drivers/lenovo/settings.yml`

 * *Files 9% similar despite different names*

```diff
@@ -130,11 +130,18 @@
             
           reset:
             title: Restore Default
             type: action
             hint: >-
               Reset to the original fan curve provided by Lenovo in BIOS V28.
 
+  charge_limit:
+    tags: [advanced]
+    type: bool
+    title: Enable Charge Limit (80%)
+    hint: >-
+      Limits device charging to 80%. Lenovo EC method. Available since BIOSv29.
+
   power_light:
     tags: [advanced]
     type: bool
     title: Enable Power Light
```

### Comparing `adjustor-2.1.3/src/adjustor/drivers/smu/__init__.py` & `adjustor-2.1.4/src/adjustor/drivers/smu/__init__.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/drivers/smu/smu.yml` & `adjustor-2.1.4/src/adjustor/drivers/smu/smu.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/events.py` & `adjustor-2.1.4/src/adjustor/events.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/hhd.py` & `adjustor-2.1.4/src/adjustor/hhd.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/settings.yml` & `adjustor-2.1.4/src/adjustor/settings.yml`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor/utils.py` & `adjustor-2.1.4/src/adjustor/utils.py`

 * *Files identical despite different names*

### Comparing `adjustor-2.1.3/src/adjustor.egg-info/PKG-INFO` & `adjustor-2.1.4/src/adjustor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adjustor
-Version: 2.1.3
+Version: 2.1.4
 Summary: Adjustor, a userspace program for managing the TDP of handheld devices.
 Author-email: Kapenekakis Antheas <pypi@antheas.dev>
 Project-URL: Homepage, https://github.com/hhd-dev/adjustor
 Project-URL: Bug Tracker, https://github.com/hhd-dev/adjustor/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `adjustor-2.1.3/src/adjustor.egg-info/SOURCES.txt` & `adjustor-2.1.4/src/adjustor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

