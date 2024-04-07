# Comparing `tmp/tidal-wave-2024.3.6.tar.gz` & `tmp/tidal-wave-2024.4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidal-wave-2024.3.6.tar", last modified: Fri Mar 29 23:01:07 2024, max compression
+gzip compressed data, was "tidal-wave-2024.4.1.1.tar", last modified: Sun Apr  7 20:08:35 2024, max compression
```

## Comparing `tidal-wave-2024.3.6.tar` & `tidal-wave-2024.4.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:01:07.828644 tidal-wave-2024.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    40115 2024-03-29 23:01:07.828644 tidal-wave-2024.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 23:01:07.828644 tidal-wave-2024.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:01:07.824644 tidal-wave-2024.3.6/tidal_wave/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/album.py
--rw-r--r--   0 runner    (1001) docker     (127)     6079 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/artist.py
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/dash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/hls.py
--rw-r--r--   0 runner    (1001) docker     (127)    12180 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/media.py
--rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/mix.py
--rw-r--r--   0 runner    (1001) docker     (127)    25876 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/oauth.py
--rw-r--r--   0 runner    (1001) docker     (127)    21241 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/playlist.py
--rw-r--r--   0 runner    (1001) docker     (127)    15168 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/requesting.py
--rw-r--r--   0 runner    (1001) docker     (127)    35280 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-03-29 23:01:01.000000 tidal-wave-2024.3.6/tidal_wave/video.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 23:01:07.824644 tidal-wave-2024.3.6/tidal_wave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    40115 2024-03-29 23:01:07.000000 tidal-wave-2024.3.6/tidal_wave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-29 23:01:07.000000 tidal-wave-2024.3.6/tidal_wave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 23:01:07.000000 tidal-wave-2024.3.6/tidal_wave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-29 23:01:07.000000 tidal-wave-2024.3.6/tidal_wave.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-03-29 23:01:07.000000 tidal-wave-2024.3.6/tidal_wave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-29 23:01:07.000000 tidal-wave-2024.3.6/tidal_wave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    40047 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:08:35.060119 tidal-wave-2024.4.1.1/tidal_wave/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7506 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/album.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/artist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/dash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/hls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12132 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16449 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/mix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26634 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11863 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21265 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15165 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/requesting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36001 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5420 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14842 2024-04-07 20:08:28.000000 tidal-wave-2024.4.1.1/tidal_wave/video.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 20:08:35.064118 tidal-wave-2024.4.1.1/tidal_wave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    40047 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-07 20:08:35.000000 tidal-wave-2024.4.1.1/tidal_wave.egg-info/top_level.txt
```

### Comparing `tidal-wave-2024.3.6/LICENSE` & `tidal-wave-2024.4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.3.6/PKG-INFO` & `tidal-wave-2024.4.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.3.6
+Version: 2024.4.1.1
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,21 +221,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff==2.2.1
 Requires-Dist: cachecontrol==0.14.0
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
-Requires-Dist: m3u8==4.0.0
+Requires-Dist: m3u8==4.1.0
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: requests[socks]==2.31.0
-Requires-Dist: typer==0.11.1
-Provides-Extra: all
-Requires-Dist: typer[all]==0.11.1; extra == "all"
+Requires-Dist: typer==0.12.1
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
```

### Comparing `tidal-wave-2024.3.6/README.md` & `tidal-wave-2024.4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.3.6/pyproject.toml` & `tidal-wave-2024.4.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 [bdist_wheel]
 universal = 0  # Make the generated wheels have "py3" tag
 [project]
 name = "tidal-wave"
-version = "2024.3.6"
+version = "2024.4.1.1"
 description = "A tool to wave at the TIDAL music service."
 authors = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
 maintainers = [
     {name = "colinho", email = "pypi@colin.technology"}
 ]
@@ -29,19 +29,17 @@
 ]
 dependencies = [
     "backoff==2.2.1",
     "cachecontrol==0.14.0",
     "dataclass-wizard==0.22.3",
     "ffmpeg-python==0.2.0",
     "mutagen==1.47.0",
-    "m3u8==4.0.0",
+    "m3u8==4.1.0",
     "platformdirs==4.2.0",
     "pycryptodome==3.20.0",
     "requests[socks]==2.31.0",
-    "typer==0.11.1"
+    "typer==0.12.1"
 ]
-[project.optional-dependencies]
-all = ["typer[all]==0.11.1"]
 [project.scripts]
 tidal-wave = "tidal_wave.main:app"
 [project.urls]
 Homepage = "https://github.com/ebb-earl-co/tidal-wave"
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/album.py` & `tidal-wave-2024.4.1.1/tidal_wave/album.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,44 +72,52 @@
         self.album_dir"""
         self.album_credits: Optional[AlbumsCreditsResponseJSON] = (
             request_albums_credits(
                 session=session, album_id=self.album_id, transparent=self.transparent
             )
         )
         if self.album_credits is not None:
-            f: str = str((self.album_dir / "AlbumCredits.json").absolute())
-            with open(f, "w") as fp:
-                json.dump(obj=self.album_credits.credit, fp=fp)
+            num_credit: int = len(self.album_credits.credit)
+            if num_credit == 0:
+                logger.warning(
+                    f"No album credits returned from TIDAL API for album {self.album_id}"
+                )
+            else:
+                ac_file: str = str((self.album_dir / "AlbumCredits.json").absolute())
+                with open(ac_file, "w") as fp:
+                    json.dump(obj=self.album_credits.credit, fp=fp)
 
     def set_album_dir(self, out_dir: Path):
         """This method populates self.album_dir as a sub-subdirectory of
         out_dir: its parent directory is the name of the (main) artist of
         the album"""
         artist_substring: str = self.metadata.artist.name.replace("..", "")
         album_substring: str = (
             f"{self.metadata.name.replace('..', '')} "
             f"[{self.metadata.id}] [{self.metadata.release_date.year}]"
         )
         self.album_dir = out_dir / artist_substring / album_substring
         self.album_dir.mkdir(parents=True, exist_ok=True)
+        # Create cover_path here, even if the API
+        # does not return a cover, to avoid AttributeError later
+        self.cover_path: Path = self.album_dir / "cover.jpg"
 
         if self.metadata.number_of_volumes > 1:
             for v in range(1, self.metadata.number_of_volumes + 1):
                 volume_substring: str = f"Volume {v}"
                 (out_dir / artist_substring / album_substring / volume_substring).mkdir(
                     parents=True, exist_ok=True
                 )
 
     def save_cover_image(self, session: Session, out_dir: Path):
         """This method writes cover.jpg in self.album_dir via the
         utils.download_cover_image() function. If successful,
         then self.album_cover_saved takes the value True"""
         if self.album_dir is None:
             self.set_album_dir(out_dir=out_dir)
-        self.cover_path: Path = self.album_dir / "cover.jpg"
         if not self.cover_path.exists():
             download_cover_image(
                 session=session,
                 cover_uuid=self.metadata.cover,
                 output_dir=self.album_dir,
             )
         else:
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/artist.py` & `tidal-wave-2024.4.1.1/tidal_wave/artist.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         /artists/albums?filter=EPSANDSINGLES and stores the results in self.albums"""
         self.albums: Optional[ArtistsAlbumsResponseJSON] = request_artists_audio_works(
             session=session, artist_id=self.artist_id, transparent=self.transparent
         )
 
     def set_videos(self, session: Session):
         """This method requests from TIDAL API endpoint /artists/videos and
-        stores the results in self.albums"""
+        stores the results in self.videos"""
         self.videos: Optional[ArtistsVideosResponseJSON] = request_artists_videos(
             session=session, artist_id=self.artist_id, transparent=self.transparent
         )
 
     def set_artist_dir(self, out_dir: Path):
         """This method sets self.artist_dir and creates the directory on the file system
         if it does not exist"""
@@ -111,23 +111,23 @@
             )
 
     def get_videos(
         self,
         session: Session,
         out_dir: Path,
     ) -> List[Optional[str]]:
-        """This method sets self.videos by calling self.set_videos()
+        """This method sets self.videos by calling self.set_videos() and
         then, for each video, instantiates a Video object and executes
-        video.get()"""
+        the object's .get() method"""
         self.set_videos(session)
         logger.info(
             f"Starting attempt to get {self.videos.total_number_of_items} videos "
             f"for artist with ID {self.metadata.id}, '{self.name}'"
         )
-        for i, v in enumerate(self.videos.items):
+        for v in self.videos.items:
             video: Video = Video(video_id=v.id, transparent=self.transparent)
             video.get(
                 session=session,
                 out_dir=out_dir,
                 metadata=v,
             )
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/dash.py` & `tidal-wave-2024.4.1.1/tidal_wave/dash.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.3.6/tidal_wave/hls.py` & `tidal-wave-2024.4.1.1/tidal_wave/hls.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.3.6/tidal_wave/login.py` & `tidal-wave-2024.4.1.1/tidal_wave/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,20 @@
                 return sess
 
         serj = SessionsEndpointResponseJSON.from_dict(r.json())
         logger.debug("Adding data from API reponse to session object:")
         logger.debug(serj)
 
     sess: requests.Session = requests.Session()
-    sess.headers: Dict[str, str] = headers
-    sess.auth: BearerAuth = BearerAuth(token=token)
-    sess.user_id: str = serj.user_id
-    sess.session_id: str = serj.session_id
-    sess.client_id: str = serj.client.id
-    sess.client_name: str = serj.client.name
+    sess.headers = headers
+    sess.auth = BearerAuth(token=token)
+    sess.user_id = serj.user_id
+    sess.session_id = serj.session_id
+    sess.client_id = serj.client.id
+    sess.client_name = serj.client.name
     if serj.country_code == "US":
         sess.params["countryCode"] = "US"
         sess.params["locale"] = "en_US"
         sess.headers["Accept-Language"] = "en-US"
     elif (len(serj.country_code) == 2) and (serj.country_code.isupper()):
         sess.params["countryCode"] = serj.country_code
     return sess
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/main.py` & `tidal-wave-2024.4.1.1/tidal_wave/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from contextlib import closing
 import logging
 from pathlib import Path
 from typing import Optional, Union
 
-from .login import login, AudioFormat, LogLevel
 from .album import Album
 from .artist import Artist
+from .login import login, AudioFormat, LogLevel
 from .mix import Mix
-from .playlist import Playlist
-from .track import Track
-from .video import Video
 from .models import (
     match_tidal_url,
     TidalAlbum,
     TidalArtist,
     TidalMix,
     TidalPlaylist,
     TidalTrack,
     TidalVideo,
 )
+from .playlist import Playlist
+from .track import Track
+from .video import Video
+from .utils import is_tidal_api_reachable
 
 from cachecontrol import CacheControl
 from platformdirs import user_music_path
 import typer
 from typing_extensions import Annotated
 
 app = typer.Typer()
@@ -90,14 +91,23 @@
 
     if tidal_resource is None:
         logger.critical(
             f"Cannot parse '{tidal_url}' as a TIDAL album, artist, mix, playlist, track, or video URL"
         )
         raise typer.Exit(code=1)
 
+    # Check Internet connectivity, and whether api.tidal.com is up
+    if not is_tidal_api_reachable():
+        user_wishes_to_continue: bool = typer.confirm(
+            "\nEven though tidal-wave cannot seem to connect to the Internet, "
+            "would you like program execution to continue?"
+        )
+        if not user_wishes_to_continue:
+            raise typer.Exit(code=1)
+
     s, audio_format = login(audio_format=audio_format)
     if s is None:
         raise typer.Exit(code=1)
 
     with closing(CacheControl(s)) as session:
         if isinstance(tidal_resource, TidalTrack):
             track = Track(track_id=tidal_resource.tidal_id, transparent=transparent)
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/media.py` & `tidal-wave-2024.4.1.1/tidal_wave/media.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,21 +18,27 @@
     "artist": {"flac": "ARTIST", "m4a": "\xa9ART"},
     "artists": {"flac": "ARTISTS", "m4a": "----:com.apple.iTunes:ARTISTS"},
     "barcode": {"flac": "BARCODE", "m4a": "----:com.apple.iTunes:BARCODE"},
     "comment": {"flac": "COMMENT", "m4a": "\xa9cmt"},
     "composer": {"flac": "COMPOSER", "m4a": "\xa9wrt"},
     "copyright": {"flac": "COPYRIGHT", "m4a": "cprt"},
     "date": {"flac": "DATE", "m4a": "\xa9day"},
-    "director": {"flac": None, "m4a": "\xa9dir"},
+    "director": {"flac": "DIRECTOR", "m4a": "\xa9dir"},
     "engineer": {"flac": "ENGINEER", "m4a": "----:com.apple.iTunes:ENGINEER"},
     "isrc": {"flac": "ISRC", "m4a": "----:com.apple.iTunes:ISRC"},
+    "language": {"flac": "LANGUAGE", "m4a": "----:com.apple.iTunes:LANGUAGE"},
+    "location": {"flac": "LOCATION", "m4a": "\xa9xyz"},
     "lyrics": {"flac": "LYRICS", "m4a": "\xa9lyr"},
     "lyricist": {"flac": "LYRICIST", "m4a": "----:com.apple.iTunes:LYRICIST"},
+    "media": {"flac": "MEDIA", "m4a": "----:com.apple.iTunes:MEDIA"},
     "mixer": {"flac": "MIXER", "m4a": "----:com.apple.iTunes:MIXER"},
-    "producer": {"flac": "PRODUCER", "m4a": "----:com.apple.iTunes:PRODUCER"},
+    "performer": {"flac": "PERFORMER", "m4a": "perf"},
+    "producer": {"flac": "PRODUCER", "m4a": "\xa9prd"},
+    "publisher": {"flac": "PUBLISHER", "m4a": "\xa9pub"},
+    "rating": {"flac": None, "m4a": "rtng"},  # 0 if None; 1 if clean; 2 if explicit
     "remixer": {"flac": "REMIXER", "m4a": "----:com.apple.iTunes:REMIXER"},
     "album_peak_amplitude": {
         "flac": "REPLAYGAIN_ALBUM_PEAK",
         "m4a": "----:com.apple.iTunes:REPLAYGAIN_ALBUM_PEAK",
     },
     "album_replay_gain": {
         "flac": "REPLAYGAIN_ALBUM_GAIN",
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/mix.py` & `tidal-wave-2024.4.1.1/tidal_wave/mix.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.3.6/tidal_wave/models.py` & `tidal-wave-2024.4.1.1/tidal_wave/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,16 +207,16 @@
         _credit: Optional["Credit"] = self.get_credit(type_)
         if _credit is not None:
             return [c.name for c in _credit.contributors]
         else:
             return
 
     def __post_init__(self):
-        """Try to parse the various Contributors into a dict
-        that will be JSON-format amenable"""
+        """Try to parse the various Contributors into a dict,
+        self.credit, that will be JSON-format amenable"""
 
         _credit: Dict[str, Union[str, List[str]]] = {
             c: self.get_contributors(c)
             for c in (
                 "Cover Design",
                 "Creative Director",
                 "Design",
@@ -526,30 +526,47 @@
             return tuple(vc.name for vc in vcs)
         else:
             return
 
     def __post_init__(self):
         """Try to parse the various Contributors to top-level
         attributes of this class"""
+        self.associated_performer: Optional[Tuple[str]] = self.get_contributors(
+            "Associated Performer"
+        )
         self.composer: Optional[Tuple[str]] = self.get_contributors("Composer")
         self.director: Optional[Tuple[str]] = self.get_contributors("Director")
+        self.engineer: Optional[Tuple[str]] = self.get_contributors("Engineer")
         self.film_director: Optional[Tuple[str]] = self.get_contributors(
             "Film Director"
         )
         self.film_producer: Optional[Tuple[str]] = self.get_contributors(
             "Film Producer"
         )
+        self.location: Optional[Tuple[str]] = self.get_contributors("Studio")
         self.lyricist: Optional[Tuple[str]] = self.get_contributors("Lyricist")
         self.mastering_engineer: Optional[Tuple[str]] = self.get_contributors(
             "Mastering Engineer"
         )
+        self.mixing_engineer: Optional[Tuple[str]] = self.get_contributors(
+            "Mixing Engineer"
+        )
+        self.music_publisher: Optional[Tuple[str]] = self.get_contributors(
+            "Music Publisher"
+        )
         self.producer: Optional[Tuple[str]] = self.get_contributors("Producer")
+        self.video_director: Optional[Tuple[str]] = self.get_contributors(
+            "Video Director"
+        )
         self.video_producer: Optional[Tuple[str]] = self.get_contributors(
             "Video Producer"
         )
+        self.vocal_engineer: Optional[Tuple[str]] = self.get_contributors(
+            "Vocal Engineer"
+        )
 
 
 @dataclass
 class PlaylistsEndpointResponseJSON(dataclass_wizard.JSONWizard):
     """Response from the TIDAL API, videos/<VIDEOID> endpoint.If the params and
     headers are correctly specified, the API returns metadata of the available
     version of the (music) video, including video quality, video title, date,
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/oauth.py` & `tidal-wave-2024.4.1.1/tidal_wave/oauth.py`

 * *Files identical despite different names*

### Comparing `tidal-wave-2024.3.6/tidal_wave/playlist.py` & `tidal-wave-2024.4.1.1/tidal_wave/playlist.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,15 +242,17 @@
 
     def craft_m3u8_text(self):
         """This method creates a file called playlist.m3u8 in self.playlist_dir
         that is a standard M3U. Needs to be called after self.flatten_playlist_dir
         in order to be able to access self.files
         N.b. the already-written file is temporarily copied to a .mp4 version in a
         temporary directory because .m4a files cannot be read with mutagen."""
-        m3u_text: str = f"#EXTM3U\n#EXTENC:UTF-8\n#EXTIMG:{str(self.cover_path.absolute())}\n#PLAYLIST:{self.name}\n"
+        m3u_text: str = (
+            f"#EXTM3U\n#EXTENC:UTF-8\n#EXTIMG:{str(self.cover_path.absolute())}\n#PLAYLIST:{self.name}\n"
+        )
 
         logger.info(
             f"Creating .m3u8 playlist file for Playlist with ID '{self.playlist_id}'"
         )
         for d in self.files:
             file: str = next(iter(d.values()))
             if file is None:
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/requesting.py` & `tidal-wave-2024.4.1.1/tidal_wave/requesting.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 json.dumps(resp.json(), ensure_ascii=True, indent=4, sort_keys=True)
             )
 
         if cf:
             data = sc.from_dict({"credits": resp.json()})
         else:
             data = sc.from_dict(resp.json())
-        
+
         return data
 
     return function(
         s=session,
         e=endpoint,
         i=identifier,
         u=url_end,
@@ -335,44 +335,44 @@
         parameters={
             "audioquality": audio_quality,
             "playbackmode": "STREAM",
             "assetpresentation": "FULL",
         },
         url_end="/playbackinfopostpaywall",
         subclass=TracksEndpointStreamResponseJSON,
-        transparent=transparent
+        transparent=transparent,
     )
     return func()
 
 
 def request_videos(
     session: Session, video_id: int, transparent: bool = False
 ) -> Optional[VideosEndpointResponseJSON]:
     return requester_maker(
         session=session,
         endpoint="videos",
         identifier=video_id,
         headers={"Accept": "application/json"},
         subclass=VideosEndpointResponseJSON,
-        transparent=transparent
+        transparent=transparent,
     )
 
 
 def request_video_contributors(
     session: Session, video_id: int, transparent: bool = False
 ) -> Optional[VideosContributorsResponseJSON]:
     return requester_maker(
         session=session,
         endpoint="videos",
         identifier=video_id,
         headers={"Accept": "application/json"},
         parameters={"limit": 100},
         url_end="/contributors",
         subclass=VideosContributorsResponseJSON,
-        transparent=transparent
+        transparent=transparent,
     )
 
 
 def request_video_stream(
     session: Session, video_id: int, video_quality: str, transparent: bool = False
 ) -> Optional[VideosEndpointStreamResponseJSON]:
     func = partial(
@@ -384,29 +384,29 @@
         parameters={
             "videoquality": video_quality,
             "playbackmode": "STREAM",
             "assetpresentation": "FULL",
         },
         url_end="/playbackinfopostpaywall",
         subclass=VideosEndpointStreamResponseJSON,
-        transparent=transparent
+        transparent=transparent,
     )
     return func()
 
 
 def request_playlists(
     session: Session, playlist_id: int, transparent: bool = False
 ) -> Optional[PlaylistsEndpointResponseJSON]:
     return requester_maker(
         session=session,
         endpoint="playlists",
         identifier=playlist_id,
         headers={"Accept": "application/json"},
         subclass=PlaylistsEndpointResponseJSON,
-        transparent=transparent
+        transparent=transparent,
     )
 
 
 def get_album_id(session: Session, track_id: int) -> Optional[int]:
     """Given the Tidal ID to a track, query the Tidal API in order to retrieve
     the Tidal ID of the album to which the track belongs"""
     terj: Optional[TracksEndpointResponseJSON] = request_tracks(session, track_id)
```

### Comparing `tidal-wave-2024.3.6/tidal_wave/track.py` & `tidal-wave-2024.4.1.1/tidal_wave/track.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,14 +155,18 @@
         artist_substring: str = self.album.artist.name.replace("..", "")
         album_substring: str = (
             f"{self.album.name} " f"[{self.album.id}] [{self.album.release_date.year}]"
         )
         self.album_dir: Path = out_dir / artist_substring / album_substring
         self.album_dir.mkdir(parents=True, exist_ok=True)
 
+        # Create cover_path here, even if the API
+        # does not return a cover, to avoid AttributeError later
+        self.cover_path: Path = self.album_dir / "cover.jpg"
+
         if self.album.number_of_volumes > 1:
             volume_substring: str = f"Volume {self.metadata.volume_number}"
             (self.album_dir / volume_substring).mkdir(parents=True, exist_ok=True)
 
     def set_filename(self, audio_format: AudioFormat):
         """This method sets self.filename, which is based on self.metadata
         as well as audio_format. Additionally, if the available codecs in
@@ -280,15 +284,14 @@
                         f"'{str(track_artist_bio_json.absolute())}"
                     )
                     track_artist_bio_json.write_text(artist_bio.to_json())
 
     def save_album_cover(self, session: Session):
         """This method saves cover.jpg to self.album_dir; the bytes for cover.jpg
         come from self.album.cover"""
-        self.cover_path: Path = self.album_dir / "cover.jpg"
         if not self.cover_path.exists():
             download_cover_image(
                 session=session, cover_uuid=self.album.cover, output_dir=self.album_dir
             )
 
     def set_urls(self, session: Session):
         """This method sets self.urls based on self.manifest"""
@@ -519,18 +522,18 @@
             f"{self.stream.album_replay_gain}"
             if self.stream.album_replay_gain is not None
             else None
         )
         tags[tag_map["artist"]] = ";".join((a.name for a in self.metadata.artists))
         tags[tag_map["artists"]] = [a.name for a in self.metadata.artists]
         tags[tag_map["barcode"]] = self.album.upc
-        tags[tag_map["comment"]] = self.metadata.url
         tags[tag_map["copyright"]] = self.metadata.copyright
         tags[tag_map["date"]] = str(self.album.release_date)
         tags[tag_map["isrc"]] = self.metadata.isrc
+        tags[tag_map["media"]] = "Digital Media"
         tags[tag_map["title"]] = self.metadata.name
         tags[tag_map["track_peak_amplitude"]] = f"{self.metadata.peak}"
         tags[tag_map["track_peak_amplitude"]] = (
             f"{self.metadata.peak}" if self.metadata.peak is not None else None
         )
         tags[tag_map["track_replay_gain"]] = (
             f"{self.metadata.replay_gain}"
@@ -550,38 +553,51 @@
             _lyrics = self.lyrics.subtitles
         except (TypeError, AttributeError):  # NoneType problems
             pass
         else:
             tags[tag_map["lyrics"]] = _lyrics
 
         if self.codec == "flac":
+            tags[tag_map["comment"]] = self.metadata.url
             # track and disk
             tags["DISCTOTAL"] = f"{self.album.number_of_volumes}"
             tags["DISC"] = f"{self.metadata.volume_number}"
             tags["TRACKTOTAL"] = f"{self.album.number_of_tracks}"
             tags["TRACKNUMBER"] = f"{self.metadata.track_number}"
             # instrument-specific
             #     piano
             try:
                 piano_credits: List[str] = [
-                    f"{pc} (piano)" for pc in self.credits.piano
+                    f"{{{pc}}} (piano)" for pc in self.credits.piano
                 ]
             except (TypeError, AttributeError):  # NoneType problems
                 pass
             else:
                 tags["PERFORMER"] = piano_credits
 
         elif self.codec == "m4a":
+            tags["\xa9url"] = self.metadata.url
+            # Whether explicit field, 'rtng', does not have a FLAC counterpart
+            if self.metadata.explicit is None:
+                tags["rtng"] = (0,)
+            elif not self.metadata.explicit:
+                tags["rtng"] = (1,)
+            elif self.metadata.explicit:
+                tags["rtng"] = (2,)
+
+            tags["pcst"] = 0  # I.e. False because we are not working with podcasts here
+            tags["stik"] = (1,)  # Music (https://exiftool.org/TagNames/QuickTime.html)
+
             # Have to convert to bytes the values of the tags starting with '----'
             for k, v in tags.copy().items():
                 if k.startswith("----"):
                     if isinstance(v, str):
-                        tags[k]: bytes = v.encode("UTF-8")
+                        tags[k] = v.encode("UTF-8")
                     elif isinstance(v, list):
-                        tags[k]: List[bytes] = [s.encode("UTF-8") for s in v]
+                        tags[k] = [s.encode("UTF-8") for s in v]
 
             tags["trkn"] = [(self.metadata.track_number, self.album.number_of_tracks)]
             tags["disk"] = [(self.metadata.volume_number, self.album.number_of_volumes)]
 
         self.tags: dict = {k: v for k, v in tags.items() if v is not None}
 
     def set_mutagen(self):
@@ -639,15 +655,15 @@
                         with temporary_file(suffix=".flac") as tf:
                             shutil.move(self.absolute_outfile, tf.name)
                             cmd: List[str] = shlex.split(_cmd % tf.name)
                             subprocess.run(cmd)
 
         elif self.codec == "m4a":
             _cmd: str = f"""ffmpeg -hide_banner -loglevel quiet -y -i "{self.absolute_outfile}"
-                -map 0:a:0 -map 0:v:0 -map_metadata 0 -c:a copy -c:v copy "%s" """
+                -map 0:a:0 -map 0:v:0 -map_metadata 0 -c:a copy -c:v copy -movflags +faststart "%s" """
             if self.mutagen.get("covr") is not None:
                 if isinstance(self.mutagen["covr"], list):
                     if len(self.mutagen["covr"]) == 1:
                         if isinstance(self.mutagen["covr"][0], MP4Cover):
                             with temporary_file(suffix=".mp4") as tf:
                                 cmd: List[str] = shlex.split(_cmd % tf.name)
                                 subprocess.run(cmd)
```

### Comparing `tidal-wave-2024.3.6/tidal_wave.egg-info/PKG-INFO` & `tidal-wave-2024.4.1.1/tidal_wave.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidal-wave
-Version: 2024.3.6
+Version: 2024.4.1.1
 Summary: A tool to wave at the TIDAL music service.
 Author-email: colinho <pypi@colin.technology>
 Maintainer-email: colinho <pypi@colin.technology>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,21 +221,19 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: backoff==2.2.1
 Requires-Dist: cachecontrol==0.14.0
 Requires-Dist: dataclass-wizard==0.22.3
 Requires-Dist: ffmpeg-python==0.2.0
 Requires-Dist: mutagen==1.47.0
-Requires-Dist: m3u8==4.0.0
+Requires-Dist: m3u8==4.1.0
 Requires-Dist: platformdirs==4.2.0
 Requires-Dist: pycryptodome==3.20.0
 Requires-Dist: requests[socks]==2.31.0
-Requires-Dist: typer==0.11.1
-Provides-Extra: all
-Requires-Dist: typer[all]==0.11.1; extra == "all"
+Requires-Dist: typer==0.12.1
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Version](https://img.shields.io/pypi/v/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/tidal-wave)](https://pypi.org/project/tidal-wave/)
 [![Build Python package](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml/badge.svg?branch=trunk&event=release)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/python-build.yml)
 [![Docker Image CI](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml/badge.svg?branch=trunk)](https://github.com/ebb-earl-co/tidal-wave/actions/workflows/docker-image.yml)
```

### Comparing `tidal-wave-2024.3.6/tidal_wave.egg-info/SOURCES.txt` & `tidal-wave-2024.4.1.1/tidal_wave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

