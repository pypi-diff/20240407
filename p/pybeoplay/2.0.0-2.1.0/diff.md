# Comparing `tmp/pybeoplay-2.0.0.tar.gz` & `tmp/pybeoplay-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybeoplay-2.0.0.tar", last modified: Sat Mar 16 20:35:27 2024, max compression
+gzip compressed data, was "pybeoplay-2.1.0.tar", last modified: Sun Apr  7 00:21:14 2024, max compression
```

## Comparing `pybeoplay-2.0.0.tar` & `pybeoplay-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-16 20:35:27.984582 pybeoplay-2.0.0/
--rw-rw-rw-   0        0        0     1074 2021-01-23 16:53:58.000000 pybeoplay-2.0.0/LICENSE
--rw-rw-rw-   0        0        0     1960 2024-03-16 20:35:27.984582 pybeoplay-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1296 2023-01-07 03:41:34.000000 pybeoplay-2.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-16 20:35:27.958930 pybeoplay-2.0.0/pybeoplay/
--rw-rw-rw-   0        0        0    30046 2024-03-16 15:39:51.000000 pybeoplay-2.0.0/pybeoplay/__init__.py
--rw-rw-rw-   0        0        0     2315 2023-04-16 01:28:12.000000 pybeoplay-2.0.0/pybeoplay/const.py
-drwxrwxrwx   0        0        0        0 2024-03-16 20:35:27.982613 pybeoplay-2.0.0/pybeoplay.egg-info/
--rw-rw-rw-   0        0        0     1960 2024-03-16 20:35:27.000000 pybeoplay-2.0.0/pybeoplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-03-16 20:35:27.000000 pybeoplay-2.0.0/pybeoplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-16 20:35:27.000000 pybeoplay-2.0.0/pybeoplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-01-24 04:42:02.000000 pybeoplay-2.0.0/pybeoplay.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2024-03-16 20:35:27.000000 pybeoplay-2.0.0/pybeoplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-03-16 20:35:27.991563 pybeoplay-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1285 2024-03-16 15:40:24.000000 pybeoplay-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:21:14.364873 pybeoplay-2.1.0/
+-rw-rw-rw-   0        0        0     1074 2021-01-23 16:53:58.000000 pybeoplay-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2705 2024-04-07 00:21:14.364223 pybeoplay-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2037 2024-04-07 00:19:50.000000 pybeoplay-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 00:21:14.337259 pybeoplay-2.1.0/pybeoplay/
+-rw-rw-rw-   0        0        0    30451 2024-04-07 00:18:56.000000 pybeoplay-2.1.0/pybeoplay/__init__.py
+-rw-rw-rw-   0        0        0     2462 2024-04-07 00:15:59.000000 pybeoplay-2.1.0/pybeoplay/const.py
+drwxrwxrwx   0        0        0        0 2024-04-07 00:21:14.362365 pybeoplay-2.1.0/pybeoplay.egg-info/
+-rw-rw-rw-   0        0        0     2705 2024-04-07 00:21:14.000000 pybeoplay-2.1.0/pybeoplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-04-07 00:21:14.000000 pybeoplay-2.1.0/pybeoplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 00:21:14.000000 pybeoplay-2.1.0/pybeoplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-01-24 04:42:02.000000 pybeoplay-2.1.0/pybeoplay.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2024-04-07 00:21:14.000000 pybeoplay-2.1.0/pybeoplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-07 00:21:14.367919 pybeoplay-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1285 2024-04-07 00:17:58.000000 pybeoplay-2.1.0/setup.py
```

### Comparing `pybeoplay-2.0.0/LICENSE` & `pybeoplay-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pybeoplay-2.0.0/PKG-INFO` & `pybeoplay-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pybeoplay
-Version: 2.0.0
+Version: 2.1.0
 Summary: BeoPlay API for Python
 Home-page: https://github.com/giachello/pybeoplay
-Download-URL: https://github.com/giachello/pybeoplay/tarball/2.0.0
+Download-URL: https://github.com/giachello/pybeoplay/tarball/2.1.0
 Author: Giovanni Iachello
 Author-email: giovanni.iachello@gmail.com
 License: MIT License
 Keywords: beoplay,pybeoplay,B&O,Bang & Olufsen
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -51,7 +51,11 @@
 - previous
 - standby
 - set source
 - join experience
 - leave experience
 - play queue item
 - set stand position
+
+The following key presses are available:
+```Cursor/Select, Cursor/Up, Cursor/Down, Cursor/Left, Cursor/Right, Cursor/Exit, Cursor/Back, Cursor/PageUp, Cursor/PageDown, Cursor/Clear, Stream/Play, Stream/Stop, Stream/Pause, Stream/Wind, Stream/Rewind, Stream/Forward, Stream/Backward, List/StepUp, List/StepDown, List/PreviousElement, List/Shuffle, List/Repeat, Menu/Root, Menu/Option, Menu/Setup, Menu/Contents, Menu/Favorites, Menu/ElectronicProgramGuide, Menu/VideoOnDemand, Menu/Text, Menu/HbbTV,Menu/HomeControl, Device/Information, Device/Eject, Device/TogglePower, Device/Languages, Device/Subtitles, Device/OneWayJoin, Device/Mots, Record/Record, Generic/Blue, Generic/Red, Generic/Green, Generic/Yellow,``` and the digits ```0-9```
+
```

### Comparing `pybeoplay-2.0.0/pybeoplay/__init__.py` & `pybeoplay-2.1.0/pybeoplay/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,19 @@
         return self._hardwareVersion
 
     @property
     def remote_commands(self):
         """Get the list of available remote commands"""
         return BEOPLAY_REMOTE_COMMANDS
 
+    @property
+    def digits(self):
+        """Get the list of available digits"""
+        return BEOPLAY_DIGITS
+
     ###############################################################
     # ASYNC BASED NETWORK CALLS
     ###############################################################
 
     async def async_getReq(self, path):
         """Non blocking GET call to the speaker, with a given path."""
         if self._clientsession is None:
@@ -426,14 +431,23 @@
         await self.async_postReq("POST", BEOPLAY_REMOTE_PREFIX + command, {"toBeReleased": toBeReleased})
 
     async def async_remote_release(self, command : str):
         if (command not in BEOPLAY_REMOTE_COMMANDS):
             return
         await self.async_postReq("POST", BEOPLAY_REMOTE_PREFIX + command + BEOPLAY_URL_RELEASE, {})
 
+    async def async_digits(self, digit : str):
+        """
+        Send a digit keypress to the device. Digits are 0-9  
+
+        """
+        if (digit not in BEOPLAY_DIGITS):
+            return
+        await self.async_postReq("POST", BEOPLAY_DIGITS_URL, {BEOPLAY_DIGITS_KEY: int(digit)})
+
 
     ###############################################################
     # REQUESTS (BLOCKING) NETWORK CALLS
     ###############################################################
 
     def _getReq(self, path):
         try:
```

### Comparing `pybeoplay-2.0.0/pybeoplay/const.py` & `pybeoplay-2.1.0/pybeoplay/const.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,7 +34,11 @@
 BEOPLAY_URL_LEAVE_EXPERIENCE = 'BeoZone/Zone/ActiveSources/primaryExperience'
 BEOPLAY_URL_PLAYQUEUE = 'BeoZone/Zone/PlayQueue'
 BEOPLAY_URL_PLAYQUEUE_INSTANT = '?instantplay'
 
 
 BEOPLAY_REMOTE_COMMANDS = ['Cursor/Select', 'Cursor/Up', 'Cursor/Down', 'Cursor/Left', 'Cursor/Right', 'Cursor/Exit', 'Cursor/Back', 'Cursor/PageUp', 'Cursor/PageDown', 'Cursor/Clear', 'Stream/Play', 'Stream/Stop', 'Stream/Pause', 'Stream/Wind', 'Stream/Rewind', 'Stream/Forward', 'Stream/Backward', 'List/StepUp', 'List/StepDown', 'List/PreviousElement', 'List/Shuffle', 'List/Repeat', 'Menu/Root', 'Menu/Option', 'Menu/Setup', 'Menu/Contents', 'Menu/Favorites', 'Menu/ElectronicProgramGuide', 'Menu/VideoOnDemand', 'Menu/Text', 'Menu/HbbTV,Menu/HomeControl', 'Device/Information', 'Device/Eject', 'Device/TogglePower', 'Device/Languages', 'Device/Subtitles', 'Device/OneWayJoin', 'Device/Mots', 'Record/Record', 'Generic/Blue', 'Generic/Red', 'Generic/Green', 'Generic/Yellow']
 BEOPLAY_REMOTE_PREFIX = 'BeoZone/Zone/'
+
+BEOPLAY_DIGITS = [ '0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
+BEOPLAY_DIGITS_URL = 'BeoZone/Zone/Digits'
+BEOPLAY_DIGITS_KEY = 'digits'
```

### Comparing `pybeoplay-2.0.0/pybeoplay.egg-info/PKG-INFO` & `pybeoplay-2.1.0/pybeoplay.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pybeoplay
-Version: 2.0.0
+Version: 2.1.0
 Summary: BeoPlay API for Python
 Home-page: https://github.com/giachello/pybeoplay
-Download-URL: https://github.com/giachello/pybeoplay/tarball/2.0.0
+Download-URL: https://github.com/giachello/pybeoplay/tarball/2.1.0
 Author: Giovanni Iachello
 Author-email: giovanni.iachello@gmail.com
 License: MIT License
 Keywords: beoplay,pybeoplay,B&O,Bang & Olufsen
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -51,7 +51,11 @@
 - previous
 - standby
 - set source
 - join experience
 - leave experience
 - play queue item
 - set stand position
+
+The following key presses are available:
+```Cursor/Select, Cursor/Up, Cursor/Down, Cursor/Left, Cursor/Right, Cursor/Exit, Cursor/Back, Cursor/PageUp, Cursor/PageDown, Cursor/Clear, Stream/Play, Stream/Stop, Stream/Pause, Stream/Wind, Stream/Rewind, Stream/Forward, Stream/Backward, List/StepUp, List/StepDown, List/PreviousElement, List/Shuffle, List/Repeat, Menu/Root, Menu/Option, Menu/Setup, Menu/Contents, Menu/Favorites, Menu/ElectronicProgramGuide, Menu/VideoOnDemand, Menu/Text, Menu/HbbTV,Menu/HomeControl, Device/Information, Device/Eject, Device/TogglePower, Device/Languages, Device/Subtitles, Device/OneWayJoin, Device/Mots, Record/Record, Generic/Blue, Generic/Red, Generic/Green, Generic/Yellow,``` and the digits ```0-9```
+
```

### Comparing `pybeoplay-2.0.0/setup.py` & `pybeoplay-2.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 PACKAGE_NAME = 'pybeoplay'
 HERE = os.path.abspath(os.path.dirname(__file__))
-VERSION = '2.0.0'
+VERSION = '2.1.0'
 
 PACKAGES = find_packages(exclude=['tests', 'tests.*', 'dist', 'ccu', 'build'])
 
 REQUIRES = []
 
 long_description = readme()
```

