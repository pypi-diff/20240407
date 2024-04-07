# Comparing `tmp/Mopidy-Jellyfin-1.0.4.tar.gz` & `tmp/Mopidy-Jellyfin-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mopidy-Jellyfin-1.0.4.tar", last modified: Fri Aug 12 22:51:10 2022, max compression
+gzip compressed data, was "Mopidy-Jellyfin-1.0.5.tar", last modified: Sun Apr  7 14:20:53 2024, max compression
```

## Comparing `Mopidy-Jellyfin-1.0.4.tar` & `Mopidy-Jellyfin-1.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2022-08-12 22:51:10.338333 Mopidy-Jellyfin-1.0.4/
--rw-r--r--   0 matt      (1000) matt      (1000)      263 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.4/.travis.yml
--rw-r--r--   0 matt      (1000) matt      (1000)    11358 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.4/LICENSE
--rw-r--r--   0 matt      (1000) matt      (1000)      154 2019-05-17 00:16:33.000000 Mopidy-Jellyfin-1.0.4/MANIFEST.in
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2022-08-12 22:51:10.335000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/
--rw-r--r--   0 matt      (1000) matt      (1000)     4275 2022-08-12 22:51:09.000000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)      789 2022-08-12 22:51:10.000000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/SOURCES.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2022-08-12 22:51:09.000000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/dependency_links.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       50 2022-08-12 22:51:10.000000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/entry_points.txt
--rw-r--r--   0 matt      (1000) matt      (1000)        1 2019-04-26 14:27:34.000000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/not-zip-safe
--rw-r--r--   0 matt      (1000) matt      (1000)       87 2022-08-12 22:51:10.000000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/requires.txt
--rw-r--r--   0 matt      (1000) matt      (1000)       16 2022-08-12 22:51:10.000000 Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/top_level.txt
--rw-r--r--   0 matt      (1000) matt      (1000)     4275 2022-08-12 22:51:10.338333 Mopidy-Jellyfin-1.0.4/PKG-INFO
--rw-r--r--   0 matt      (1000) matt      (1000)     3648 2022-08-12 22:46:11.000000 Mopidy-Jellyfin-1.0.4/README.rst
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2022-08-12 22:51:10.335000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/
--rw-r--r--   0 matt      (1000) matt      (1000)     1629 2022-08-12 22:50:31.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/__init__.py
--rw-r--r--   0 matt      (1000) matt      (1000)      807 2020-11-15 23:10:58.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/backend.py
--rw-r--r--   0 matt      (1000) matt      (1000)      366 2022-08-12 22:46:11.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/ext.conf
--rw-r--r--   0 matt      (1000) matt      (1000)     9412 2022-08-12 22:46:11.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/frontend.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4114 2022-02-26 15:08:47.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/http.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4240 2022-02-26 15:08:47.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/library.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1519 2020-07-18 14:54:46.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/playback.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4696 2020-10-17 17:05:53.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/playlists.py
--rw-r--r--   0 matt      (1000) matt      (1000)    31992 2022-08-12 22:46:11.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/remote.py
--rw-r--r--   0 matt      (1000) matt      (1000)     1021 2020-05-17 14:05:10.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/utils.py
--rw-r--r--   0 matt      (1000) matt      (1000)     4532 2022-06-15 21:32:11.000000 Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/ws_client.py
--rw-r--r--   0 matt      (1000) matt      (1000)      140 2022-08-12 22:51:10.338333 Mopidy-Jellyfin-1.0.4/setup.cfg
--rw-r--r--   0 matt      (1000) matt      (1000)     1395 2020-02-09 19:44:51.000000 Mopidy-Jellyfin-1.0.4/setup.py
-drwxr-xr-x   0 matt      (1000) matt      (1000)        0 2022-08-12 22:51:10.338333 Mopidy-Jellyfin-1.0.4/tests/
--rw-r--r--   0 matt      (1000) matt      (1000)     2472 2020-05-17 14:02:40.000000 Mopidy-Jellyfin-1.0.4/tests/conftest.py
--rw-r--r--   0 matt      (1000) matt      (1000)      554 2020-05-17 14:02:40.000000 Mopidy-Jellyfin-1.0.4/tests/test_backend.py
--rw-r--r--   0 matt      (1000) matt      (1000)      463 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.4/tests/test_extension.py
--rw-r--r--   0 matt      (1000) matt      (1000)     2188 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.4/tests/test_library.py
--rw-r--r--   0 matt      (1000) matt      (1000)      488 2020-05-17 14:02:40.000000 Mopidy-Jellyfin-1.0.4/tests/test_playback.py
--rw-r--r--   0 matt      (1000) matt      (1000)    17984 2020-05-17 14:02:40.000000 Mopidy-Jellyfin-1.0.4/tests/test_remote.py
--rw-r--r--   0 matt      (1000) matt      (1000)      631 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.4/tests/test_utils.py
--rw-r--r--   0 matt      (1000) matt      (1000)      391 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.4/tox.ini
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2024-04-07 14:20:53.921525 Mopidy-Jellyfin-1.0.5/
+-rw-r--r--   0 matt      (1000) users      (985)      263 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.5/.travis.yml
+-rw-r--r--   0 matt      (1000) users      (985)    11358 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.5/LICENSE
+-rw-r--r--   0 matt      (1000) users      (985)      154 2019-05-17 00:16:33.000000 Mopidy-Jellyfin-1.0.5/MANIFEST.in
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2024-04-07 14:20:53.921525 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/
+-rw-r--r--   0 matt      (1000) users      (985)     4432 2024-04-07 14:20:53.000000 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)      789 2024-04-07 14:20:53.000000 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/SOURCES.txt
+-rw-r--r--   0 matt      (1000) users      (985)        1 2024-04-07 14:20:53.000000 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/dependency_links.txt
+-rw-r--r--   0 matt      (1000) users      (985)       50 2024-04-07 14:20:53.000000 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/entry_points.txt
+-rw-r--r--   0 matt      (1000) users      (985)        1 2019-04-26 14:27:34.000000 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/not-zip-safe
+-rw-r--r--   0 matt      (1000) users      (985)       87 2024-04-07 14:20:53.000000 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/requires.txt
+-rw-r--r--   0 matt      (1000) users      (985)       16 2024-04-07 14:20:53.000000 Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/top_level.txt
+-rw-r--r--   0 matt      (1000) users      (985)     4432 2024-04-07 14:20:53.921525 Mopidy-Jellyfin-1.0.5/PKG-INFO
+-rw-r--r--   0 matt      (1000) users      (985)     3648 2022-12-22 21:39:10.000000 Mopidy-Jellyfin-1.0.5/README.rst
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2024-04-07 14:20:53.918192 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/
+-rw-r--r--   0 matt      (1000) users      (985)     1629 2024-04-07 14:20:31.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/__init__.py
+-rw-r--r--   0 matt      (1000) users      (985)      807 2020-08-28 03:21:27.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/backend.py
+-rw-r--r--   0 matt      (1000) users      (985)      366 2022-12-22 21:39:10.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/ext.conf
+-rw-r--r--   0 matt      (1000) users      (985)    10286 2024-04-07 14:20:31.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/frontend.py
+-rw-r--r--   0 matt      (1000) users      (985)     4114 2022-12-22 22:09:50.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/http.py
+-rw-r--r--   0 matt      (1000) users      (985)     4240 2022-12-22 21:39:10.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/library.py
+-rw-r--r--   0 matt      (1000) users      (985)     1519 2020-07-04 01:50:42.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/playback.py
+-rw-r--r--   0 matt      (1000) users      (985)     4696 2020-11-10 04:49:11.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/playlists.py
+-rw-r--r--   0 matt      (1000) users      (985)    31921 2022-12-22 22:09:50.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/remote.py
+-rw-r--r--   0 matt      (1000) users      (985)     1021 2019-04-25 23:15:29.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/utils.py
+-rw-r--r--   0 matt      (1000) users      (985)     4532 2022-12-22 22:09:50.000000 Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/ws_client.py
+-rw-r--r--   0 matt      (1000) users      (985)      140 2024-04-07 14:20:53.921525 Mopidy-Jellyfin-1.0.5/setup.cfg
+-rw-r--r--   0 matt      (1000) users      (985)     1395 2020-02-09 19:44:51.000000 Mopidy-Jellyfin-1.0.5/setup.py
+drwxr-xr-x   0 matt      (1000) users      (985)        0 2024-04-07 14:20:53.918192 Mopidy-Jellyfin-1.0.5/tests/
+-rw-r--r--   0 matt      (1000) users      (985)     2472 2020-07-03 21:30:08.000000 Mopidy-Jellyfin-1.0.5/tests/conftest.py
+-rw-r--r--   0 matt      (1000) users      (985)      554 2020-07-03 21:30:08.000000 Mopidy-Jellyfin-1.0.5/tests/test_backend.py
+-rw-r--r--   0 matt      (1000) users      (985)      463 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.5/tests/test_extension.py
+-rw-r--r--   0 matt      (1000) users      (985)     2188 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.5/tests/test_library.py
+-rw-r--r--   0 matt      (1000) users      (985)      488 2020-07-03 21:30:08.000000 Mopidy-Jellyfin-1.0.5/tests/test_playback.py
+-rw-r--r--   0 matt      (1000) users      (985)    17984 2020-07-03 21:30:08.000000 Mopidy-Jellyfin-1.0.5/tests/test_remote.py
+-rw-r--r--   0 matt      (1000) users      (985)      631 2019-04-26 13:50:35.000000 Mopidy-Jellyfin-1.0.5/tests/test_utils.py
+-rw-r--r--   0 matt      (1000) users      (985)      391 2022-12-22 22:03:22.000000 Mopidy-Jellyfin-1.0.5/tox.ini
```

### Comparing `Mopidy-Jellyfin-1.0.4/LICENSE` & `Mopidy-Jellyfin-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/PKG-INFO` & `Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: Mopidy-Jellyfin
-Version: 1.0.4
+Version: 1.0.5
 Summary: Mopidy extension for playing music from jellyfin
 Home-page: https://github.com/jellyfin/mopidy-jellyfin
 Author: Matt Carlton
 Author-email: mcarlton00@gmail.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: Mopidy>=2.0
+Requires-Dist: Pykka>=1.1
+Requires-Dist: requests>=2.20
+Requires-Dist: unidecode>=1.1
+Requires-Dist: websocket-client>=0.57
 
 ****************************
 Mopidy-Jellyfin
 ****************************
 
 .. image:: https://img.shields.io/pypi/v/Mopidy-Jellyfin.svg?style=flat
     :target: https://pypi.python.org/pypi/Mopidy-Jellyfin/
@@ -102,9 +107,7 @@
 
 Credits
 =======
 
 - Current maintainer: `Matt Carlton <https://github.com/mcarlton00>`_
 - Original author: `Marvin Steadfast <https://github.com/xsteadfastx>`_
 - `Contributors <https://github.com/jellyfin/mopidy-jellyfin/graphs/contributors>`_
-
-
```

### Comparing `Mopidy-Jellyfin-1.0.4/Mopidy_Jellyfin.egg-info/SOURCES.txt` & `Mopidy-Jellyfin-1.0.5/Mopidy_Jellyfin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/PKG-INFO` & `Mopidy-Jellyfin-1.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: Mopidy-Jellyfin
-Version: 1.0.4
+Version: 1.0.5
 Summary: Mopidy extension for playing music from jellyfin
 Home-page: https://github.com/jellyfin/mopidy-jellyfin
 Author: Matt Carlton
 Author-email: mcarlton00@gmail.com
 License: Apache License, Version 2.0
-Platform: UNKNOWN
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: Mopidy>=2.0
+Requires-Dist: Pykka>=1.1
+Requires-Dist: requests>=2.20
+Requires-Dist: unidecode>=1.1
+Requires-Dist: websocket-client>=0.57
 
 ****************************
 Mopidy-Jellyfin
 ****************************
 
 .. image:: https://img.shields.io/pypi/v/Mopidy-Jellyfin.svg?style=flat
     :target: https://pypi.python.org/pypi/Mopidy-Jellyfin/
@@ -102,9 +107,7 @@
 
 Credits
 =======
 
 - Current maintainer: `Matt Carlton <https://github.com/mcarlton00>`_
 - Original author: `Marvin Steadfast <https://github.com/xsteadfastx>`_
 - `Contributors <https://github.com/jellyfin/mopidy-jellyfin/graphs/contributors>`_
-
-
```

### Comparing `Mopidy-Jellyfin-1.0.4/README.rst` & `Mopidy-Jellyfin-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/__init__.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import os
 import socket
 
 from mopidy import config, ext
 
 
-__version__ = '1.0.4'
+__version__ = '1.0.5'
 
 logger = logging.getLogger(__name__)
 
 
 class Extension(ext.Extension):
 
     dist_name = 'Mopidy-Jellyfin'
```

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/backend.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/backend.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/frontend.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/frontend.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,14 +144,18 @@
             now_playing_queue = []
             for index, track in enumerate(tracklist):
                 track_id = track.uri.split(':')[-1]
                 now_playing_queue.append({
                     'Id': track_id,
                     'PlaylistItemId': f'playlistItem{index}'
                 })
+                # Max json body in the server for play queue is 1000
+                # This gives us a little wiggle room
+                if index >= 950:
+                    break
             playlist_item_id = f'playlistItem{track_index}'
 
             # json payload to server
             data = {
                 "VolumeLevel": volume,
                 "IsMuted": mute_state,
                 "IsPaused": pause_state,
@@ -206,29 +210,45 @@
                 self.core.mixer.set_mute(False)
             else:
                 self.core.mixer.set_mute(True)
 
     def play_tracks(self, data):
         # Receives the "Play To" commands from the Jellyfin server
         items = data.get('ItemIds')
-        playcommand = data.get('PlayCommand', '')
+        play_command = data.get('PlayCommand', '')
         start_ticks = data.get('StartPositionTicks')
         if start_ticks:
             start_position = int(start_ticks / 10000)
         else:
             start_position = 0
 
         uris = ['jellyfin:track:{}'.format(item_id) for item_id in items]
-        tracks = self.core.tracklist.add(uris=uris).get()
-        # Allows adding to play queue without changing currently playing track
-        if playcommand == 'PlayNow':
+
+        if play_command == 'PlayNow':
+            # Play what the server tells us to
+            self.core.tracklist.clear()
+            tracks = self.core.tracklist.add(uris=uris).get()
             start_index = data.get('StartIndex')
+            # If specified, start at a specific track.  otherwise, start at 0
             if not start_index:
                 start_index = 0
             self.core.playback.play(tlid=tracks[start_index].tlid)
+        elif play_command == 'PlayLast':
+            # This maps to the "Play Next" button in JF-Web
+            curr_index = self.core.tracklist.index().get()
+            if curr_index is not None:
+                add_index = curr_index + 1
+            else:
+                # Fall back to position 0 if no tracks currently exist
+                add_index = 0
+            self.core.tracklist.add(uris=uris, at_position=add_index).get()
+        elif play_command == 'PlayNext':
+            # This maps to the "Add to play queue" button in JF-Web
+            self.core.tracklist.add(uris=uris).get()
+
         # If playing a track that already has playback progress, start at that
         # progress point, not the beginning
         if start_position:
             # Needs to wait a short time before seeking or else we lose
             # all control
             time.sleep(.5)
             self.core.playback.seek(int(start_position))
```

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/http.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/http.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/library.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/library.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/playback.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/playback.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/playlists.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/playlists.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/remote.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,33 +185,28 @@
             models.Ref.directory(
                 uri='jellyfin:directory:{}'.format(i.get('Id')),
                 name=i.get('Name')
             ) for i in libraries if i
         ]
 
     def get_playlists(self):
-        url = self.api_url(
-            '/Users/{}/Views'.format(self.user_id)
-        )
-
-        data = self.http.get(url)
-
-        library_id = [
-            library.get('Id') for library in data.get('Items')
-            if library.get('Name') == 'Playlists'
-        ]
-
-        if library_id:
-            library_id = library_id[0]
-        else:
-            return []
+        '''
+        Queries the server for any playlist objects
+        '''
+        url_params = {
+            'UserId': self.user_id,
+            'IncludeItemTypes': 'Playlist',
+            'Recursive': 'true',
+            'fields': 'MediaSources'
+        }
 
-        raw_playlists = self.get_directory(library_id)
+        url = self.api_url('/Users/{}/Items'.format(self.user_id), url_params)
+        playlists = self.http.get(url)
 
-        return raw_playlists.get('Items')
+        return playlists.get('Items', [])
 
     def get_playlist_contents(self, playlist_id):
         url_params = {
             'UserId': self.user_id,
             'fields': 'MediaSources'
         }
         url = self.api_url('/Playlists/{}/Items'.format(playlist_id), url_params)
@@ -679,15 +674,15 @@
             search_query = 'MusicAlbum'
         elif itemtype == 'track_name':
             search_query = 'Audio'
         else:
             raise Exception('Jellyfin search: no itemtype {}'.format(itemtype))
 
         url_params = {
-            'SearchTerm': quote(term.encode('utf-8')),
+            'SearchTerm': term,
             'IncludeItemTypes': search_query
         }
 
         url = self.api_url('/Search/Hints', url_params)
         data = self.http.get(url)
 
         return [i for i in data.get('SearchHints', [])]
```

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/utils.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/utils.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/mopidy_jellyfin/ws_client.py` & `Mopidy-Jellyfin-1.0.5/mopidy_jellyfin/ws_client.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/setup.py` & `Mopidy-Jellyfin-1.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/tests/conftest.py` & `Mopidy-Jellyfin-1.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/tests/test_backend.py` & `Mopidy-Jellyfin-1.0.5/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/tests/test_library.py` & `Mopidy-Jellyfin-1.0.5/tests/test_library.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/tests/test_remote.py` & `Mopidy-Jellyfin-1.0.5/tests/test_remote.py`

 * *Files identical despite different names*

### Comparing `Mopidy-Jellyfin-1.0.4/tests/test_utils.py` & `Mopidy-Jellyfin-1.0.5/tests/test_utils.py`

 * *Files identical despite different names*

