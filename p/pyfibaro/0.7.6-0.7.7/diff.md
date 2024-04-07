# Comparing `tmp/pyfibaro-0.7.6.tar.gz` & `tmp/pyfibaro-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfibaro-0.7.6.tar", last modified: Sun Oct 22 15:12:03 2023, max compression
+gzip compressed data, was "pyfibaro-0.7.7.tar", last modified: Sun Apr  7 20:20:40 2024, max compression
```

## Comparing `pyfibaro-0.7.6.tar` & `pyfibaro-0.7.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 15:12:03.233589 pyfibaro-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2023-10-22 15:12:03.233589 pyfibaro-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 15:12:03.233589 pyfibaro-0.7.6/pyfibaro/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 15:12:03.233589 pyfibaro-0.7.6/pyfibaro/common/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/common/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/common/rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    18818 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_room.py
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_state_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyfibaro/fibaro_state_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 15:12:03.233589 pyfibaro-0.7.6/pyfibaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2023-10-22 15:12:03.000000 pyfibaro-0.7.6/pyfibaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-10-22 15:12:03.000000 pyfibaro-0.7.6/pyfibaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-22 15:12:03.000000 pyfibaro-0.7.6/pyfibaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-22 15:12:03.000000 pyfibaro-0.7.6/pyfibaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-22 15:12:03.000000 pyfibaro-0.7.6/pyfibaro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2023-10-22 15:12:03.237589 pyfibaro-0.7.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-22 15:12:03.233589 pyfibaro-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_device_armed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_device_hc3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_device_scene_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_device_scene_support_hc3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_room.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_scene_hc3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_fibaro_state_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_rest_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-10-22 15:11:42.000000 pyfibaro-0.7.6/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.553742 pyfibaro-0.7.7/pyfibaro/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.553742 pyfibaro-0.7.7/pyfibaro/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/common/rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3257 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18818 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_state_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyfibaro/fibaro_state_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/pyfibaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 20:20:40.000000 pyfibaro-0.7.7/pyfibaro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:20:40.557742 pyfibaro-0.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11151 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_armed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_hc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_scene_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_device_scene_support_hc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4008 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_room.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_scene_hc3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_fibaro_state_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_rest_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-07 20:20:27.000000 pyfibaro-0.7.7/tests/test_utils.py
```

### Comparing `pyfibaro-0.7.6/LICENSE` & `pyfibaro-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/PKG-INFO` & `pyfibaro-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.7.6
+Version: 0.7.7
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.7.6/README.md` & `pyfibaro-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/common/const.py` & `pyfibaro-0.7.7/pyfibaro/common/const.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/common/rest_client.py` & `pyfibaro-0.7.7/pyfibaro/common/rest_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/fibaro_client.py` & `pyfibaro-0.7.7/pyfibaro/fibaro_client.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/fibaro_device.py` & `pyfibaro-0.7.7/pyfibaro/fibaro_device.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/fibaro_info.py` & `pyfibaro-0.7.7/pyfibaro/fibaro_info.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/fibaro_room.py` & `pyfibaro-0.7.7/pyfibaro/fibaro_room.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/fibaro_scene.py` & `pyfibaro-0.7.7/pyfibaro/fibaro_scene.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/pyfibaro/fibaro_state_handler.py` & `pyfibaro-0.7.7/pyfibaro/fibaro_state_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,57 +16,59 @@
 
     def __init__(self, rest_client: RestClient, callback: callable) -> None:
         """Create the state handler and start the background thread."""
 
         super().__init__(name=f"Thread {__name__}")
 
         self._rest_client = rest_client
-        self.callback = callback
+        self._callback = callback
+        self._stop_flag = threading.Event()
+
         # stop unconditionally on exit
         self.daemon = True
 
-        self._stop_flag = threading.Event()
-
         self.start()
 
     def run(self) -> None:
         """State Handler main loop which runs in this thread."""
 
         _LOGGER.info("Starting the state change handler")
         last = 0
 
         while not self._is_stopped_flag():
             sleep_time = 1
             attempt = 1
             success = False
 
-            while not success:
-                if self._is_stopped_flag():
-                    break
-
+            while not success and not self._is_stopped_flag():
                 try:
                     state = self._rest_client.get(
                         f"refreshStates?last={last}", timeout=REFRESH_STATE_TIMEOUT
                     )
                     _LOGGER.debug(state)
 
                     last = state.get("last")
-                    self.callback(state)
-
                     success = True
                 except Exception as ex:
                     _LOGGER.warning("Connection Error (%s). Error: %s", attempt, ex)
                     attempt += 1
 
                     if attempt == 3:
                         sleep_time = 30
-                        _LOGGER.warning("Fallback to 30-second connection retry timer.")
+                        _LOGGER.info("Fallback to 30-second connection retry timer.")
 
                     self._stop_flag.wait(sleep_time)
 
+                if success:
+                    try:
+                        self._callback(state)
+                    except Exception as ex:
+                        _LOGGER.warning("Error in state change callback: %s", ex)
+
+
         _LOGGER.info("State change handler stopped.")
 
     def _is_stopped_flag(self) -> bool:
         return self._stop_flag.is_set()
 
     def stop(self) -> None:
         """Stop the state handler."""
```

### Comparing `pyfibaro-0.7.6/pyfibaro/fibaro_state_resolver.py` & `pyfibaro-0.7.7/pyfibaro/fibaro_state_resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """State object resolver for fibaro home center."""
+from __future__ import annotations
 
 import logging
+
 from typing import Any
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class FibaroEvent:
     """A fibaro event returned by state handler."""
@@ -18,19 +20,22 @@
         """Returns the event type as string.
 
         Most known event is "CentralSceneEvent" which is used for button press events.
         """
         return self.raw_data.get("type", "")
 
     @property
-    def fibaro_id(self) -> int:
-        """The device id which throws the event."""
+    def fibaro_id(self) -> int | None:
+        """The device id which throws the event. Not all events are related to a device."""
         data = self.event_data
         # id is used by HC3, deviceId by HC2
-        return int(data.get("id", data.get("deviceId")))
+        fibaro_id = data.get("id", data.get("deviceId"))
+        if fibaro_id is None:
+            return None
+        return int(fibaro_id)
 
     @property
     def event_data(self) -> dict:
         """Returns the event data in raw format."""
         return self.raw_data.get("data", {})
 
     @property
```

### Comparing `pyfibaro-0.7.6/pyfibaro.egg-info/PKG-INFO` & `pyfibaro-0.7.7/pyfibaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfibaro
-Version: 0.7.6
+Version: 0.7.7
 Summary: Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 Home-page: https://github.com/rappenze/pyfibaro
 Author: Roman Appenzeller
 Author-email: 
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyfibaro-0.7.6/pyfibaro.egg-info/SOURCES.txt` & `pyfibaro-0.7.7/pyfibaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/setup.cfg` & `pyfibaro-0.7.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyfibaro
-version = 0.7.6
+version = 0.7.7
 description = Simple API to access fibaro home center from any Python 3 script. Designed for Home Assistant (but not only)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/rappenze/pyfibaro
 author = Roman Appenzeller
 author_email = 
 license = MIT
```

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_device.py` & `pyfibaro-0.7.7/tests/test_fibaro_device.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_device_armed.py` & `pyfibaro-0.7.7/tests/test_fibaro_device_armed.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_device_hc3.py` & `pyfibaro-0.7.7/tests/test_fibaro_device_hc3.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_device_scene_support.py` & `pyfibaro-0.7.7/tests/test_fibaro_device_scene_support.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_device_scene_support_hc3.py` & `pyfibaro-0.7.7/tests/test_fibaro_device_scene_support_hc3.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_info.py` & `pyfibaro-0.7.7/tests/test_fibaro_info.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_login.py` & `pyfibaro-0.7.7/tests/test_fibaro_login.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_refresh.py` & `pyfibaro-0.7.7/tests/test_fibaro_scene_hc3.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,78 @@
-"""Test FibaroStateHandler class."""
+"""Test SceneModel class."""
 
-import time
-
-import pytest
 import requests_mock
 
 from pyfibaro.fibaro_client import FibaroClient
 
 from .test_utils import TEST_BASE_URL, TEST_PASSWORD, TEST_USERNAME, load_fixture
 
-refresh_payload = load_fixture("refresh.json")
+scene_payload = load_fixture("scene-hc3.json")
 login_payload = load_fixture("login_success.json")
 info_payload = load_fixture("info.json")
+info_payload["serialNumber"] = "HC3-111111"
+
+
+def test_fibaro_scene() -> None:
+    """Test get request"""
+    with requests_mock.Mocker() as mock:
+        assert isinstance(mock, requests_mock.Mocker)
+
+        mock.register_uri("GET", f"{TEST_BASE_URL}scenes", json=scene_payload)
+        mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
+        mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
+
+        client = FibaroClient(TEST_BASE_URL)
+        client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
+        client.connect()
+
+        scenes = client.read_scenes()
+        assert scenes is not None
+
+        assert len(scenes) == 2
+        assert scenes[0].fibaro_id == 1
+        assert scenes[0].name == "Morning Scenario"
+        assert scenes[0].room_id == 219
+        assert scenes[0].visible is True
+        assert mock.call_count == 3
+
+
+def test_fibaro_scene_start() -> None:
+    """Test get request"""
+    with requests_mock.Mocker() as mock:
+        assert isinstance(mock, requests_mock.Mocker)
+
+        mock.register_uri("GET", f"{TEST_BASE_URL}scenes", json=scene_payload)
+        mock.register_uri("POST", f"{TEST_BASE_URL}scenes/1/execute")
+        mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
+        mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
+
+        client = FibaroClient(TEST_BASE_URL)
+        client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
+        client.connect()
+
+        scenes = client.read_scenes()
+
+        assert mock.call_count == 3
+        scenes[0].start("1234")
+        assert mock.call_count == 4
+
+
+def test_fibaro_scene_stop() -> None:
+    """Test get request"""
+    with requests_mock.Mocker() as mock:
+        assert isinstance(mock, requests_mock.Mocker)
 
+        mock.register_uri("GET", f"{TEST_BASE_URL}scenes", json=scene_payload)
+        mock.register_uri("POST", f"{TEST_BASE_URL}scenes/1/kill")
+        mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
+        mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
 
-class TestRefresh:
-    """Use a test class to get async state."""
+        client = FibaroClient(TEST_BASE_URL)
+        client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
+        client.connect()
 
-    callback_result = None
+        scenes = client.read_scenes()
 
-    def callback_function(self, event) -> None:
-        """The callback handler for this test."""
-        self.callback_result = event
-
-    def test_fibaro_refresh(self) -> None:
-        """Test get request"""
-        with requests_mock.Mocker() as mock:
-            assert isinstance(mock, requests_mock.Mocker)
-
-            mock.register_uri(
-                "GET", f"{TEST_BASE_URL}refreshStates", json=refresh_payload
-            )
-            mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
-            mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
-
-            client = FibaroClient(TEST_BASE_URL)
-            client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
-            client.connect()
-
-            client.register_update_handler(self.callback_function)
-            time.sleep(0.2)
-            client.unregister_update_handler()
-
-            assert self.callback_result is not None
-            assert mock.call_count > 2
-
-    def test_fibaro_refresh_fail(self) -> None:
-        """Test get request"""
-        with requests_mock.Mocker() as mock:
-            assert isinstance(mock, requests_mock.Mocker)
-
-            mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
-            mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
-
-            client = FibaroClient(TEST_BASE_URL)
-            client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
-            client.connect()
-
-            client.register_update_handler(self.callback_function)
-            time.sleep(1.2)
-            client.unregister_update_handler()
-
-            assert mock.call_count > 2
-
-    def test_fibaro_refresh_double_register(self) -> None:
-        """Test get request"""
-        with requests_mock.Mocker() as mock:
-            assert isinstance(mock, requests_mock.Mocker)
-
-            mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
-            mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
-
-            client = FibaroClient(TEST_BASE_URL)
-            client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
-            client.connect()
-
-            with pytest.raises(Exception):
-                client.register_update_handler(self.callback_function)
-                client.register_update_handler(self.callback_function)
+        assert mock.call_count == 3
+        scenes[0].stop()
+        assert mock.call_count == 4
```

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_room.py` & `pyfibaro-0.7.7/tests/test_fibaro_room.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_scene.py` & `pyfibaro-0.7.7/tests/test_fibaro_scene.py`

 * *Files identical despite different names*

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_scene_hc3.py` & `pyfibaro-0.7.7/tests/test_rest_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,78 +1,46 @@
-"""Test SceneModel class."""
+"""Test rest client."""
 
 import requests_mock
 
-from pyfibaro.fibaro_client import FibaroClient
+from pyfibaro.common.rest_client import RestClient
 
 from .test_utils import TEST_BASE_URL, TEST_PASSWORD, TEST_USERNAME, load_fixture
 
-scene_payload = load_fixture("scene-hc3.json")
-login_payload = load_fixture("login_success.json")
 info_payload = load_fixture("info.json")
-info_payload["serialNumber"] = "HC3-111111"
 
 
-def test_fibaro_scene() -> None:
+def test_get_request() -> None:
     """Test get request"""
     with requests_mock.Mocker() as mock:
         assert isinstance(mock, requests_mock.Mocker)
-
-        mock.register_uri("GET", f"{TEST_BASE_URL}scenes", json=scene_payload)
-        mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
         mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
+        client = RestClient(TEST_BASE_URL, False, TEST_USERNAME, TEST_PASSWORD)
+        response = client.get("settings/info")
 
-        client = FibaroClient(TEST_BASE_URL)
-        client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
-        client.connect()
-
-        scenes = client.read_scenes()
-        assert scenes is not None
-
-        assert len(scenes) == 2
-        assert scenes[0].fibaro_id == 1
-        assert scenes[0].name == "Morning Scenario"
-        assert scenes[0].room_id == 219
-        assert scenes[0].visible is True
-        assert mock.call_count == 3
+        assert mock.call_count == 1
+        assert response == info_payload
 
 
-def test_fibaro_scene_start() -> None:
+def test_https_get_request() -> None:
     """Test get request"""
     with requests_mock.Mocker() as mock:
         assert isinstance(mock, requests_mock.Mocker)
+        url = "https://192.169.1.40/api/"
+        mock.register_uri("GET", f"{url}settings/info", json=info_payload)
+        client = RestClient(url, True, TEST_USERNAME, TEST_PASSWORD)
+        response = client.get("settings/info")
 
-        mock.register_uri("GET", f"{TEST_BASE_URL}scenes", json=scene_payload)
-        mock.register_uri("POST", f"{TEST_BASE_URL}scenes/1/execute")
-        mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
-        mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
-
-        client = FibaroClient(TEST_BASE_URL)
-        client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
-        client.connect()
-
-        scenes = client.read_scenes()
+        assert mock.call_count == 1
+        assert response == info_payload
 
-        assert mock.call_count == 3
-        scenes[0].start("1234")
-        assert mock.call_count == 4
 
-
-def test_fibaro_scene_stop() -> None:
-    """Test get request"""
+def test_post_request() -> None:
+    """Test post request"""
     with requests_mock.Mocker() as mock:
         assert isinstance(mock, requests_mock.Mocker)
+        mock.register_uri("POST", f"{TEST_BASE_URL}settings/info", json=info_payload)
+        client = RestClient(TEST_BASE_URL, False, TEST_USERNAME, TEST_PASSWORD)
+        response = client.post("settings/info", info_payload)
 
-        mock.register_uri("GET", f"{TEST_BASE_URL}scenes", json=scene_payload)
-        mock.register_uri("POST", f"{TEST_BASE_URL}scenes/1/kill")
-        mock.register_uri("GET", f"{TEST_BASE_URL}loginStatus", json=login_payload)
-        mock.register_uri("GET", f"{TEST_BASE_URL}settings/info", json=info_payload)
-
-        client = FibaroClient(TEST_BASE_URL)
-        client.set_authentication(TEST_USERNAME, TEST_PASSWORD)
-        client.connect()
-
-        scenes = client.read_scenes()
-
-        assert mock.call_count == 3
-        scenes[0].stop()
-        assert mock.call_count == 4
+        assert mock.call_count == 1
+        assert response == info_payload
```

### Comparing `pyfibaro-0.7.6/tests/test_fibaro_state_resolver.py` & `pyfibaro-0.7.7/tests/test_fibaro_state_resolver.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,20 +10,25 @@
 
 
 def test_fibaro_state_resolver_event() -> None:
     """Test event resolver"""
     resolver = FibaroStateResolver(refresh_payload)
     events = resolver.get_events()
     assert events is not None
-    assert len(events) == 1
+    assert len(events) == 2
     assert events[0].event_type == "DevicePropertyUpdatedEvent"
     assert events[0].fibaro_id == 28
     assert events[0].key_event_type == ""
     assert events[0].key_id == 0
 
+    assert events[1].event_type == "PowerMetricsChangedEvent"
+    assert events[1].fibaro_id is None
+    assert events[1].key_event_type == ""
+    assert events[1].key_id == 0
+
 
 def test_fibaro_state_resolver_state_update() -> None:
     """Test event resolver"""
     resolver = FibaroStateResolver(refresh_payload)
     changes = resolver.get_state_updates()
     assert changes is not None
     assert len(changes) == 1
```

