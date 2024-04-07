# Comparing `tmp/spotidex-0.0.3.tar.gz` & `tmp/spotidex-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotidex-0.0.3.tar", last modified: Sat Apr  6 12:59:27 2024, max compression
+gzip compressed data, was "spotidex-0.0.4.tar", last modified: Sun Apr  7 09:29:00 2024, max compression
```

## Comparing `spotidex-0.0.3.tar` & `spotidex-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.977004 spotidex-0.0.3/
--rw-rw-rw-   0        0        0     1110 2024-04-06 09:42:27.000000 spotidex-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1129 2024-04-06 12:59:27.975196 spotidex-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      499 2024-04-06 09:42:27.000000 spotidex-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-06 12:59:27.977004 spotidex-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-04-06 12:59:12.000000 spotidex-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.875929 spotidex-0.0.3/spotidex/
--rw-rw-rw-   0        0        0      121 2024-04-06 10:41:23.000000 spotidex-0.0.3/spotidex/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.915841 spotidex-0.0.3/spotidex/cli/
--rw-rw-rw-   0        0        0      616 2024-04-06 11:21:46.000000 spotidex-0.0.3/spotidex/cli/SpotidexApp.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:04:49.000000 spotidex-0.0.3/spotidex/cli/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.944958 spotidex-0.0.3/spotidex/cli/app_screens/
--rw-rw-rw-   0        0        0     6936 2024-04-06 10:26:07.000000 spotidex-0.0.3/spotidex/cli/app_screens/DownloadInterface.py
--rw-rw-rw-   0        0        0     4675 2024-04-06 10:26:15.000000 spotidex-0.0.3/spotidex/cli/app_screens/MainMenuInterface.py
--rw-rw-rw-   0        0        0     4123 2024-04-06 10:26:01.000000 spotidex-0.0.3/spotidex/cli/app_screens/SearchInterface.py
--rw-rw-rw-   0        0        0     4025 2024-04-06 10:25:55.000000 spotidex-0.0.3/spotidex/cli/app_screens/SelectDownloadInterface.py
--rw-rw-rw-   0        0        0     2430 2024-04-06 10:26:19.000000 spotidex-0.0.3/spotidex/cli/app_screens/SettingsInterface.py
--rw-rw-rw-   0        0        0        0 2024-03-25 10:54:48.000000 spotidex-0.0.3/spotidex/cli/app_screens/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.948008 spotidex-0.0.3/spotidex/cli/custom_widgets/
--rw-rw-rw-   0        0        0     4510 2024-04-06 08:18:54.000000 spotidex-0.0.3/spotidex/cli/custom_widgets/AppInterface.py
--rw-rw-rw-   0        0        0     1409 2024-04-06 10:25:36.000000 spotidex-0.0.3/spotidex/cli/custom_widgets/DownloadPathSelector.py
--rw-rw-rw-   0        0        0     1694 2024-03-26 11:07:37.000000 spotidex-0.0.3/spotidex/cli/custom_widgets/DownloadQualitySelection.py
--rw-rw-rw-   0        0        0     1933 2024-03-26 10:25:59.000000 spotidex-0.0.3/spotidex/cli/custom_widgets/MetadataCheckBox.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:19:37.000000 spotidex-0.0.3/spotidex/cli/custom_widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.952619 spotidex-0.0.3/spotidex/cli/popup_screens/
--rw-rw-rw-   0        0        0     4303 2024-04-06 09:28:28.000000 spotidex-0.0.3/spotidex/cli/popup_screens/DownloadPathPopup.py
--rw-rw-rw-   0        0        0     1126 2023-12-20 02:51:25.000000 spotidex-0.0.3/spotidex/cli/popup_screens/ExitScreenPopup.py
--rw-rw-rw-   0        0        0     1210 2024-03-26 12:20:40.000000 spotidex-0.0.3/spotidex/cli/popup_screens/GoBackSettingsPopup.py
--rw-rw-rw-   0        0        0     1389 2024-03-22 13:06:57.000000 spotidex-0.0.3/spotidex/cli/popup_screens/NetworkErrorPopup.py
--rw-rw-rw-   0        0        0        0 2024-04-06 10:19:46.000000 spotidex-0.0.3/spotidex/cli/popup_screens/__init__.py
--rw-rw-rw-   0        0        0     3880 2024-04-06 12:55:51.000000 spotidex-0.0.3/spotidex/cli/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.974198 spotidex-0.0.3/spotidex/src/
--rw-rw-rw-   0        0        0        0 2024-04-06 10:22:02.000000 spotidex-0.0.3/spotidex/src/__init__.py
--rw-rw-rw-   0        0        0     2308 2023-12-15 00:52:48.000000 spotidex-0.0.3/spotidex/src/content.py
--rw-rw-rw-   0        0        0     9579 2024-04-06 12:16:05.000000 spotidex-0.0.3/spotidex/src/download.py
--rw-rw-rw-   0        0        0     1049 2023-12-06 02:16:07.000000 spotidex-0.0.3/spotidex/src/static.py
--rw-rw-rw-   0        0        0     8260 2024-04-05 12:03:44.000000 spotidex-0.0.3/spotidex/src/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 12:59:27.909636 spotidex-0.0.3/spotidex.egg-info/
--rw-rw-rw-   0        0        0     1129 2024-04-06 12:59:27.000000 spotidex-0.0.3/spotidex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1181 2024-04-06 12:59:27.000000 spotidex-0.0.3/spotidex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 12:59:27.000000 spotidex-0.0.3/spotidex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2024-04-06 12:59:27.000000 spotidex-0.0.3/spotidex.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-04-06 12:59:27.000000 spotidex-0.0.3/spotidex.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-06 12:59:27.000000 spotidex-0.0.3/spotidex.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.420750 spotidex-0.0.4/
+-rw-rw-rw-   0        0        0     1110 2024-04-06 09:42:27.000000 spotidex-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1129 2024-04-07 09:29:00.417519 spotidex-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2024-04-06 09:42:27.000000 spotidex-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 09:29:00.420750 spotidex-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-07 09:27:38.000000 spotidex-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.295922 spotidex-0.0.4/spotidex/
+-rw-rw-rw-   0        0        0      121 2024-04-07 04:09:46.000000 spotidex-0.0.4/spotidex/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.356891 spotidex-0.0.4/spotidex/cli/
+-rw-rw-rw-   0        0        0      616 2024-04-07 04:09:10.000000 spotidex-0.0.4/spotidex/cli/SpotidexApp.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:04:49.000000 spotidex-0.0.4/spotidex/cli/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.362395 spotidex-0.0.4/spotidex/cli/app_screens/
+-rw-rw-rw-   0        0        0     6871 2024-04-07 04:25:26.000000 spotidex-0.0.4/spotidex/cli/app_screens/DownloadInterface.py
+-rw-rw-rw-   0        0        0     4675 2024-04-06 10:26:15.000000 spotidex-0.0.4/spotidex/cli/app_screens/MainMenuInterface.py
+-rw-rw-rw-   0        0        0     4360 2024-04-06 19:29:28.000000 spotidex-0.0.4/spotidex/cli/app_screens/SearchInterface.py
+-rw-rw-rw-   0        0        0     4025 2024-04-06 10:25:55.000000 spotidex-0.0.4/spotidex/cli/app_screens/SelectDownloadInterface.py
+-rw-rw-rw-   0        0        0     2430 2024-04-06 10:26:19.000000 spotidex-0.0.4/spotidex/cli/app_screens/SettingsInterface.py
+-rw-rw-rw-   0        0        0        0 2024-03-25 10:54:48.000000 spotidex-0.0.4/spotidex/cli/app_screens/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.378943 spotidex-0.0.4/spotidex/cli/custom_widgets/
+-rw-rw-rw-   0        0        0     4510 2024-04-06 08:18:54.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/AppInterface.py
+-rw-rw-rw-   0        0        0     1409 2024-04-06 10:25:36.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadPathSelector.py
+-rw-rw-rw-   0        0        0     1694 2024-03-26 11:07:37.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadQualitySelection.py
+-rw-rw-rw-   0        0        0     1933 2024-03-26 10:25:59.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/MetadataCheckBox.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:19:37.000000 spotidex-0.0.4/spotidex/cli/custom_widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.404431 spotidex-0.0.4/spotidex/cli/popup_screens/
+-rw-rw-rw-   0        0        0     4303 2024-04-06 09:28:28.000000 spotidex-0.0.4/spotidex/cli/popup_screens/DownloadPathPopup.py
+-rw-rw-rw-   0        0        0     1126 2023-12-20 02:51:25.000000 spotidex-0.0.4/spotidex/cli/popup_screens/ExitScreenPopup.py
+-rw-rw-rw-   0        0        0     1210 2024-03-26 12:20:40.000000 spotidex-0.0.4/spotidex/cli/popup_screens/GoBackSettingsPopup.py
+-rw-rw-rw-   0        0        0     1389 2024-03-22 13:06:57.000000 spotidex-0.0.4/spotidex/cli/popup_screens/NetworkErrorPopup.py
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:19:46.000000 spotidex-0.0.4/spotidex/cli/popup_screens/__init__.py
+-rw-rw-rw-   0        0        0     3880 2024-04-06 12:55:51.000000 spotidex-0.0.4/spotidex/cli/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.412477 spotidex-0.0.4/spotidex/src/
+-rw-rw-rw-   0        0        0        0 2024-04-06 10:22:02.000000 spotidex-0.0.4/spotidex/src/__init__.py
+-rw-rw-rw-   0        0        0     3043 2024-04-07 05:31:37.000000 spotidex-0.0.4/spotidex/src/content.py
+-rw-rw-rw-   0        0        0     6703 2024-04-07 06:26:09.000000 spotidex-0.0.4/spotidex/src/download.py
+-rw-rw-rw-   0        0        0     1049 2023-12-06 02:16:07.000000 spotidex-0.0.4/spotidex/src/static.py
+-rw-rw-rw-   0        0        0     5954 2024-04-07 06:30:44.000000 spotidex-0.0.4/spotidex/src/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 09:29:00.350367 spotidex-0.0.4/spotidex.egg-info/
+-rw-rw-rw-   0        0        0     1129 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1181 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      127 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 09:28:59.000000 spotidex-0.0.4/spotidex.egg-info/top_level.txt
```

### Comparing `spotidex-0.0.3/LICENSE.txt` & `spotidex-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/PKG-INFO` & `spotidex-0.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotidex
-Version: 0.0.3
+Version: 0.0.4
 Author: libin-codes
 Author-email: libinlalu000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotidex-0.0.3/setup.py` & `spotidex-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("README.md","r") as f:
     description = f.read()
 
 setup(
     name="spotidex",
-    version="0.0.3",
+    version="0.0.4",
     long_description=description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "mutagen==1.47.0",
         "Requests==2.31.0",
```

### Comparing `spotidex-0.0.3/spotidex/cli/SpotidexApp.py` & `spotidex-0.0.4/spotidex/cli/SpotidexApp.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/app_screens/DownloadInterface.py` & `spotidex-0.0.4/spotidex/cli/app_screens/DownloadInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,14 @@
             self.app.query_one("ProgressBar").update(total=100)
         self.app.query_one("ProgressBar",ProgressBar).update(progress=float(percent))
 
     def on_worker_state_changed(self, event) -> None:
         def eval(value):
             if value == "retry":
                 self.app.query_one("ProgressBar",ProgressBar).update(progress=0, total=None)
-                self.app.query_one("ProgressBar",ProgressBar).p
                 self.download_music()
 
         if str(event.state) == "WorkerState.CANCELLED":
             self.app.push_screen(NetworkErrorScreen(), eval)
 
     @work(thread=True, exclusive=True)
     def download_music(self):
```

### Comparing `spotidex-0.0.3/spotidex/cli/app_screens/MainMenuInterface.py` & `spotidex-0.0.4/spotidex/cli/app_screens/MainMenuInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/app_screens/SearchInterface.py` & `spotidex-0.0.4/spotidex/cli/app_screens/SearchInterface.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,24 +61,27 @@
         )
     
     @work(exclusive=True, thread=True)
     def get_link_info(self):
         self.app.query_one("LoadingIndicator").styles.background = "#1c1c1c"
         try:
             self.app.link_details = get_link_details(self.app.spotify_link)
-        except Exception:
+        except Exception as spotidex_error:
+            if spotidex_error.message == "NetworkError":
+                self.app.notify("Network Connection Error",title="SPOTIDEX",severity="error")
+            elif spotidex_error.message == "InvalidSpotifyLink":
+                self.app.notify("Invalid Spotify Link",title="SPOTIDEX",severity="error")
             get_current_worker().cancel()
         self.app.query_one("#interface").loading = False
         self.app.query_one("#exit-button").disabled = False
         self.app.query_one("#interface").styles.padding = (2,3,0,3)
         
         
     def on_worker_state_changed(self, event: Worker.StateChanged) -> None:
         if str(event.state) == "WorkerState.CANCELLED":
-            self.app.notify("Network Connection Error",title="SPOTIDEX",severity="error")
             self.query_one('#search-input').visible = True
             self.query_one('#app-description').visible = True
             self.query_one('#search-button').visible = True
         elif str(event.state) == "WorkerState.SUCCESS":
             self.app.push_screen(MainMenuInterface())
             self.query_one('#search-input').visible = True
             self.query_one('#app-description').visible = True
```

### Comparing `spotidex-0.0.3/spotidex/cli/app_screens/SelectDownloadInterface.py` & `spotidex-0.0.4/spotidex/cli/app_screens/SelectDownloadInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/app_screens/SettingsInterface.py` & `spotidex-0.0.4/spotidex/cli/app_screens/SettingsInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/custom_widgets/AppInterface.py` & `spotidex-0.0.4/spotidex/cli/custom_widgets/AppInterface.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/custom_widgets/DownloadPathSelector.py` & `spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadPathSelector.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/custom_widgets/DownloadQualitySelection.py` & `spotidex-0.0.4/spotidex/cli/custom_widgets/DownloadQualitySelection.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/custom_widgets/MetadataCheckBox.py` & `spotidex-0.0.4/spotidex/cli/custom_widgets/MetadataCheckBox.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/popup_screens/DownloadPathPopup.py` & `spotidex-0.0.4/spotidex/cli/popup_screens/DownloadPathPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/popup_screens/ExitScreenPopup.py` & `spotidex-0.0.4/spotidex/cli/popup_screens/ExitScreenPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/popup_screens/GoBackSettingsPopup.py` & `spotidex-0.0.4/spotidex/cli/popup_screens/GoBackSettingsPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/popup_screens/NetworkErrorPopup.py` & `spotidex-0.0.4/spotidex/cli/popup_screens/NetworkErrorPopup.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/cli/utils.py` & `spotidex-0.0.4/spotidex/cli/utils.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex/src/content.py` & `spotidex-0.0.4/spotidex/src/content.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 from spotidex.src.utils import *
 from spotidex.src.static import *
 from spotipy import Spotify
 from spotipy.oauth2 import SpotifyClientCredentials
+from spotipy import SpotifyException
+from requests import ConnectionError,ReadTimeout
+
 
 class SpotifyContent:
     def __init__(self) -> None:
         client_cred_manager = SpotifyClientCredentials(client_id, client_secret)
         self.sp = Spotify(client_credentials_manager=client_cred_manager)
 
     def album_details(self, link):
         album_id = link.split("/")[-1].split("?")[0]
-        album_data = self.sp.album(album_id)
-        track_links = extract_track_links(self.sp,link)
+        try:
+            album_data = self.sp.album(album_id)
+            track_links = extract_track_links(self.sp,link)
+        except (ConnectionError,ReadTimeout):
+            raise SpotidexError("NetworkError")
+        except SpotifyException:
+            raise SpotidexError("InvalidSpotifyLink")
+        
 
         details = {
             "album_name": album_data["name"],
             "album_type": album_data["album_type"],
             "total_tracks": album_data["tracks"]["total"],
             "release_date": album_data["release_date"],
             "label": album_data["label"],
@@ -23,32 +32,43 @@
             "track_details":  parallel_searches(self,track_links),
         }
 
         return details
 
     def playlist_details(self, link):
         playlist_id = link.split("/")[-1].split("?")[0]
-        playlist_data = self.sp.playlist(playlist_id)
-        track_links = extract_track_links(self.sp, link)
+        try:
+            playlist_data = self.sp.playlist(playlist_id)
+            track_links = extract_track_links(self.sp, link)
+        except (ConnectionError,ReadTimeout):
+            raise SpotidexError("NetworkError")
+        except SpotifyException:
+            raise SpotidexError("InvalidSpotifyLink")
+        
+        
 
         details = {
             "playlist_name": playlist_data["name"],
             "description": playlist_data["description"],
             "creator": playlist_data["owner"]["display_name"],
             "followers": playlist_data["followers"]["total"],
             "total_tracks": playlist_data["tracks"]["total"],
             "image_url": playlist_data["images"][0]["url"],
             "track_details": parallel_searches(self,track_links),
         }
 
         return details
 
     def track_details(self, link):
-        track_data = self.sp.track(link.split("/")[-1].split("?")[0])
-
+        try:
+            track_data = self.sp.track(link.split("/")[-1].split("?")[0])
+        except (ConnectionError,ReadTimeout):
+            raise SpotidexError("NetworkError")
+        except SpotifyException:
+            raise SpotidexError("InvalidSpotifyLink")
         details = {
             "track_name": track_data["name"],
             "track_number": track_data["track_number"],
             "disc_number": track_data["disc_number"],
             "album": track_data["album"]["name"],
             "artist": ", ".join([artist["name"] for artist in track_data["artists"]]),
             "cover_image_url": track_data["album"]["images"][0]["url"],
```

### Comparing `spotidex-0.0.3/spotidex/src/download.py` & `spotidex-0.0.4/spotidex/src/download.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,259 +1,195 @@
 from spotidex.src.utils import *
 from spotidex.src.static import *
 
-import re, logging
 from pathlib import Path
 
 from tempfile import TemporaryDirectory
 import shutil
 import yt_dlp.YoutubeDL
-from spotipy import Spotify
+import spotipy
 from spotipy.oauth2 import SpotifyClientCredentials
+from spotipy import SpotifyException
+from requests import ConnectionError,ReadTimeout
+
+
 
 class SpotifyDownloader:
     def __init__(self) -> None:
         self.spotidex_path = get_spotidex_data_directory()
         self.ffmpeg_path = get_ffmpeg()
-        self.is_library = False
-        self.progress_dict = {}
-        self.total_tracks = 1
-   
-
-        client_cred_manager = SpotifyClientCredentials(
-            client_id,
-            client_secret,
-        )
-        self.sp = Spotify(client_credentials_manager=client_cred_manager)
+        self.total_tracks = None
+        self.sp = spotipy.Spotify(
+            client_credentials_manager=
+                SpotifyClientCredentials(
+                    client_id,
+                    client_secret,
+            )
+                )
+        
+    def _download_with_temp_directory(
+        self,
+        links,
+        folder_name,
+        custom_hook=None,
+        download_path=Path.cwd(),
+        quality="high",
+        metadata=True,
+        make_folder=True,
+    ):
+        with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
+            if make_folder:
+                folder_name = get_valid_name(download_path, folder_name)
+                temp_path = Path(temp_folder).joinpath(folder_name)
+            else:
+                temp_path = Path(temp_folder)
+
+            done, not_done = pool_download(
+                self, list(set(links)), custom_hook, temp_path, quality, metadata
+            )
+            if len(not_done) != 0:
+                raise SpotidexError("NetworkError")
+            progress_hook(self, {"status": "downloaded"}, custom_hook)
+            for file_path in Path(temp_folder).iterdir():
+                shutil.move(str(file_path), str(download_path))
+            progress_hook(self, {"status": "transfered"}, custom_hook)
         
 
     def download_track(
         self,
         link,
         custom_hook=None,
-        path=None,
+        download_path=Path.cwd(),
         quality="high",
         metadata=True,
     ):
-        logging.getLogger("pytube").setLevel(logging.ERROR)
+        try:
+            data = self.sp.track(link.split("/")[-1].split("?")[0])
+        except SpotifyException:
+            raise SpotidexError("InvalidSpotifyLink")
+        except (ConnectionError,ReadTimeout):
+            raise SpotidexError("NetworkError")
 
-        data = self.sp.track(link.split("/")[-1].split("?")[0])
+        
         track_artist = ",".join([artist["name"] for artist in data["artists"]])
-        track_name = data["name"]
-        query = f"{track_name} song by {track_artist} official lyrics "
-
-        file_name = re.sub(r"[^\w\d(),.\- ]", "", data["name"])
-        download_path = Path.cwd() if path == None else path
-        for i in range(1,1000000):
-            if Path(download_path,file_name+".mp3").exists():
-                file_name = file_name.split(" (")[0]+f" ({i})"
-            else:
-                break
-        if self.is_library:
+        query = f"{data["name"]} song by {track_artist} official lyrics "
+        file_name = get_valid_name(download_path,data["name"]+".mp3")
+    
+        with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
             options = {
-            "format": "bestaudio/best",
-            "outtmpl": str(download_path)+'\\'+file_name,
-            "quiet": True,
-            "noprogress": True,
-            "progress": "false",
-            "ffmpeg_location": str(self.ffmpeg_path),
-            "postprocessors": [
-                {
-                    "key": "FFmpegExtractAudio",
-                    "preferredcodec": "mp3",
-                    "preferredquality": bitrate[quality],
-                }
-            ],
-            "retries": 20,
-            "progress_hooks": [lambda d: progress_hook(self, d, custom_hook)]
-            if custom_hook != None
-            else [],
-        }
-
+                "format": "bestaudio/best",
+                "outtmpl": str(download_path)+'\\'+file_name,
+                "quiet": True,
+                "noprogress": True,
+                "progress": "false",
+                "ffmpeg_location": str(self.ffmpeg_path),
+                "postprocessors": [
+                    {
+                        "key": "FFmpegExtractAudio",
+                        "preferredcodec": "mp3",
+                        "preferredquality": bitrate[quality],
+                    }
+                ],
+                "retries": 20,
+                "progress_hooks": [lambda d: progress_hook(self, d, custom_hook)]
+                if custom_hook != None
+                else [],
+            }
+                
+            if self.total_tracks == None:
+                options['outtmpl'] = str(Path(temp_folder))+'\\'+file_name
             ydl = yt_dlp.YoutubeDL(options)
             yt_video_result = ydl.extract_info(f"ytsearch:{query}", download=False)
             first_yt_video_link = yt_video_result["entries"][0]["webpage_url"]
             yt_video_download = ydl.extract_info(first_yt_video_link, download=True)
             downloaded_path = ydl.prepare_filename(yt_video_download)
 
             if metadata:
                 add_metadata(data, Path(downloaded_path + ".mp3").resolve())
-        else:
-            with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
-
-                options = {
-                    "format": "bestaudio/best",
-                    "outtmpl": str(Path(temp_folder))+'\\'+file_name,
-                    "quiet": True,
-                    "noprogress": True,
-                    "progress": "false",
-                    "ffmpeg_location": str(self.ffmpeg_path),
-                    "postprocessors": [
-                        {
-                            "key": "FFmpegExtractAudio",
-                            "preferredcodec": "mp3",
-                            "preferredquality": bitrate[quality],
-                        }
-                    ],
-                    "retries": 20,
-                    "progress_hooks": [lambda d: progress_hook(self, d, custom_hook)]
-                    if custom_hook != None
-                    else [],
-                }
-
-                ydl = yt_dlp.YoutubeDL(options)
-                yt_video_result = ydl.extract_info(f"ytsearch:{query}", download=False)
-                first_yt_video_link = yt_video_result["entries"][0]["webpage_url"]
-                yt_video_download = ydl.extract_info(first_yt_video_link, download=True)
-                downloaded_path = ydl.prepare_filename(yt_video_download)
-
-                if metadata:
-                    add_metadata(data, Path(downloaded_path + ".mp3").resolve())
-
-                if not self.is_library and custom_hook is not None:
-                    progress_hook(self, {"status": "downloaded"}, custom_hook)
-
-                if not self.is_library:
-                    for file_path in Path(temp_folder).iterdir():
-                        shutil.move(file_path, download_path)
-
-                    if custom_hook is not None:
-                        progress_hook(self, {"status": "transfered"}, custom_hook)
-        
-        
 
+            if self.total_tracks == None:
+                progress_hook(self, {"status": "downloaded"}, custom_hook)
+                for file_path in Path(temp_folder).iterdir():
+                    shutil.move(file_path, download_path)
+                progress_hook(self, {"status": "transfered"}, custom_hook)
+    
     def download_playlist(
         self,
         link,
         custom_hook=None,
         download_path=Path.cwd(),
         quality="high",
         metadata=True,
         make_folder=True,
     ):
         playlist_id = link.split("/")[-1].split("?")[0]
-        playlist_data = self.sp.playlist(playlist_id)
-        track_links = extract_track_links(self.sp, link)
-
-        self.is_library = True
-        self.total_tracks = len(track_links)
-
-        folder_name = re.sub(r"[^\w\d(),.\- ]", "", playlist_data["name"])
-        for i in range(1,1000000):
-            if Path(download_path,folder_name).exists():
-                folder_name = folder_name.split(" (")[0]+f" ({i})"
-            else:
-                break
-        with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
-            if make_folder == True:
-                temp_path = Path(temp_folder).joinpath(folder_name)
-            else:
-                temp_path = Path(temp_folder)   
-
-            done,not_done = pool_download(
-                    self,
-                    list(set(track_links)),
-                    custom_hook,
-                    temp_path,
-                    quality,
-                    metadata,
-                )
-            if len(not_done) != 0:
-                raise ConnectionError
+        try:
+            playlist_data = self.sp.playlist(playlist_id)
+            track_links = extract_track_links(self.sp, link)
+        except SpotifyException:
+            raise SpotidexError("InvalidSpotifyLink")
+        except (ConnectionError,ReadTimeout):
+            raise SpotidexError("NetworkError")
+        
+        folder_name = get_valid_name(download_path,playlist_data['name'])
+
+        self._download_with_temp_directory(
+                track_links,
+                folder_name,
+                custom_hook,
+                download_path,
+                quality,
+                metadata,
+                make_folder,
+            )
             
-            if custom_hook != None:
-                progress_hook(self, {"status": "downloaded"}, custom_hook)
-
-            for file_path in Path(temp_folder).iterdir():
-                shutil.move(str(file_path), str(download_path))
-
-            if custom_hook != None:
-                progress_hook(self, {"status": "transfered"}, custom_hook)
-            
-        
-
-
     def download_album(
         self,
         link,
         custom_hook=None,
         download_path=Path.cwd(),
         quality="high",
         metadata=True,
         make_folder=True,
     ):
         album_id = link.split("/")[-1].split("?")[0]
-        album_data = self.sp.album(album_id)
-        track_links = extract_track_links(self.sp, link)
-
-        self.is_library = True
-        self.total_tracks = len(track_links)
-        
-        folder_name,i = re.sub(r"[^\w\d(),.\-\[\] ]", "", folder_name),1
-        while Path(download_path, folder_name).exists():
-            folder_name,i = folder_name.split(" (")[0] + f" ({i})",i+1
-        folder_name = re.sub(r"[^\w\d(),.\- ]", "", album_data["name"])
-        for i in range(1,1000000):
-            if Path(download_path,folder_name).exists():
-                folder_name = folder_name.split(" (")[0]+f" ({i})"
-            else:
-                break
-        with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
-            if make_folder == True:
-                temp_path = Path(temp_folder).joinpath(folder_name)
-            else:
-                temp_path = Path(temp_folder)   
-
-            done,not_done = pool_download(
-                    self,
-                    list(set(track_links)),
-                    custom_hook,
-                    temp_path,
-                    quality,
-                    metadata,
-                )
-            if len(not_done) != 0:
-                raise ConnectionError
-
-            progress_hook(self, {"status": "downloaded"}, custom_hook)
-            with self.temp_folder:
-                for file_path in Path(temp_folder).iterdir():
-                    shutil.move(str(file_path), str(download_path))
-            progress_hook(self, {"status": "transfered"}, custom_hook)
-        
-
-
+        try:
+            album_data = self.sp.album(album_id)
+            track_links = extract_track_links(self.sp, link)
+        except SpotifyException:
+            raise SpotidexError("InvalidSpotifyLink")
+        except (ConnectionError,ReadTimeout):
+            raise SpotidexError("NetworkError")
+        
+        
+        folder_name = get_valid_name(download_path,album_data['name'])
+        
+        self._download_with_temp_directory(
+                track_links,
+                folder_name,
+                custom_hook,
+                download_path,
+                quality,
+                metadata,
+                make_folder,
+            )
+            
     def download_multiple_songs(
         self,
         links,
         folder_name,
         custom_hook=None,
         download_path=Path.cwd(),
         quality="high",
         metadata=True,
         make_folder=True,
     ):
-        self.is_library = True
-        self.total_tracks = len(links)
-        with TemporaryDirectory(dir=str(self.spotidex_path)) as temp_folder:
-            if make_folder == True:
-                folder_name,i = re.sub(r"[^\w\d(),.\-\[\] ]", "", folder_name),1
-                while Path(download_path, folder_name).exists():
-                    folder_name,i = folder_name.split(" (")[0] + f" ({i})",i+1
-                temp_path = Path(temp_folder).joinpath(folder_name)
-            else:
-                temp_path = Path(temp_folder)   
-
-
-            done,not_done = pool_download(
-                    self, list(set(links)), custom_hook, temp_path, quality, metadata
-                )
-            if len(not_done) != 0:
-                raise ConnectionError
+        self._download_with_temp_directory(
+                links,
+                folder_name,
+                custom_hook,
+                download_path,
+                quality,
+                metadata,
+                make_folder,
+            )
             
-
-            progress_hook(self, {"status": "downloaded"}, custom_hook)
-            for file_path in Path(temp_folder).iterdir():
-                shutil.move(str(file_path), str(download_path))
-            progress_hook(self, {"status": "transfered"}, custom_hook)
-        
-
```

### Comparing `spotidex-0.0.3/spotidex/src/static.py` & `spotidex-0.0.4/spotidex/src/static.py`

 * *Files identical despite different names*

### Comparing `spotidex-0.0.3/spotidex.egg-info/PKG-INFO` & `spotidex-0.0.4/spotidex.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotidex
-Version: 0.0.3
+Version: 0.0.4
 Author: libin-codes
 Author-email: libinlalu000@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `spotidex-0.0.3/spotidex.egg-info/SOURCES.txt` & `spotidex-0.0.4/spotidex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

