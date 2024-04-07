# Comparing `tmp/pystashlib-0.4.4.tar.gz` & `tmp/pystashlib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystashlib-0.4.4.tar", last modified: Mon Feb 12 02:24:12 2024, max compression
+gzip compressed data, was "pystashlib-0.5.0.tar", last modified: Sun Apr  7 14:37:36 2024, max compression
```

## Comparing `pystashlib-0.4.4.tar` & `pystashlib-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-02-12 02:24:12.338014 pystashlib-0.4.4/
--rw-rw-rw-   0        0        0     1915 2024-02-12 02:24:12.337013 pystashlib-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     1317 2024-02-09 14:15:36.000000 pystashlib-0.4.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-12 02:24:12.336012 pystashlib-0.4.4/pystashlib.egg-info/
--rw-rw-rw-   0        0        0     1915 2024-02-12 02:24:12.000000 pystashlib-0.4.4/pystashlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2024-02-12 02:24:12.000000 pystashlib-0.4.4/pystashlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-12 02:24:12.000000 pystashlib-0.4.4/pystashlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-02-12 02:24:12.000000 pystashlib-0.4.4/pystashlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-12 02:24:12.000000 pystashlib-0.4.4/pystashlib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-12 02:24:12.338014 pystashlib-0.4.4/setup.cfg
--rw-rw-rw-   0        0        0      971 2024-02-09 14:15:51.000000 pystashlib-0.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-12 02:24:12.334010 pystashlib-0.4.4/stashlib/
--rw-rw-rw-   0        0        0       23 2024-02-09 14:15:47.000000 pystashlib-0.4.4/stashlib/__init__.py
--rw-rw-rw-   0        0        0     8403 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/common.py
--rw-rw-rw-   0        0        0     1992 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/database.py
--rw-rw-rw-   0        0        0     1024 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/html.py
--rw-rw-rw-   0        0        0     1150 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/log.py
--rw-rw-rw-   0        0        0     1111 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/logger.py
--rw-rw-rw-   0        0        0     3848 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/scene_filename_parser.py
--rw-rw-rw-   0        0        0     2614 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/sqlite_wrapper.py
--rw-rw-rw-   0        0        0    14462 2024-02-09 13:02:41.000000 pystashlib-0.4.4/stashlib/stash_database.py
--rw-rw-rw-   0        0        0     2345 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/stash_database_base.py
--rw-rw-rw-   0        0        0    23018 2024-02-12 01:16:16.000000 pystashlib-0.4.4/stashlib/stash_interface.py
--rw-rw-rw-   0        0        0    60302 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/stash_models.py
--rw-rw-rw-   0        0        0   285285 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/stash_tables.py
--rw-rw-rw-   0        0        0     1838 2024-01-22 14:58:25.000000 pystashlib-0.4.4/stashlib/table.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:37:36.144064 pystashlib-0.5.0/
+-rw-rw-rw-   0        0        0     2086 2024-04-07 14:37:36.142061 pystashlib-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1463 2024-04-07 14:32:50.000000 pystashlib-0.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 14:37:36.141060 pystashlib-0.5.0/pystashlib.egg-info/
+-rw-rw-rw-   0        0        0     2086 2024-04-07 14:37:36.000000 pystashlib-0.5.0/pystashlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2024-04-07 14:37:36.000000 pystashlib-0.5.0/pystashlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 14:37:36.000000 pystashlib-0.5.0/pystashlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-04-07 14:37:36.000000 pystashlib-0.5.0/pystashlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 14:37:36.000000 pystashlib-0.5.0/pystashlib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 14:37:36.144064 pystashlib-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-04-07 14:32:09.000000 pystashlib-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:37:36.139061 pystashlib-0.5.0/stashlib/
+-rw-rw-rw-   0        0        0       23 2024-04-07 14:33:35.000000 pystashlib-0.5.0/stashlib/__init__.py
+-rw-rw-rw-   0        0        0     8403 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/common.py
+-rw-rw-rw-   0        0        0     1992 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/database.py
+-rw-rw-rw-   0        0        0     1024 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/html.py
+-rw-rw-rw-   0        0        0     1150 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/log.py
+-rw-rw-rw-   0        0        0     1111 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/logger.py
+-rw-rw-rw-   0        0        0     3848 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/scene_filename_parser.py
+-rw-rw-rw-   0        0        0     2614 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/sqlite_wrapper.py
+-rw-rw-rw-   0        0        0    14462 2024-02-09 13:02:41.000000 pystashlib-0.5.0/stashlib/stash_database.py
+-rw-rw-rw-   0        0        0     2449 2024-04-07 14:33:49.000000 pystashlib-0.5.0/stashlib/stash_database_base.py
+-rw-rw-rw-   0        0        0    23018 2024-02-12 01:16:16.000000 pystashlib-0.5.0/stashlib/stash_interface.py
+-rw-rw-rw-   0        0        0    61082 2024-04-07 14:33:49.000000 pystashlib-0.5.0/stashlib/stash_models.py
+-rw-rw-rw-   0        0        0   285173 2024-04-07 14:33:49.000000 pystashlib-0.5.0/stashlib/stash_tables.py
+-rw-rw-rw-   0        0        0     1838 2024-01-22 14:58:25.000000 pystashlib-0.5.0/stashlib/table.py
```

### Comparing `pystashlib-0.4.4/PKG-INFO` & `pystashlib-0.5.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: pystashlib
-Version: 0.4.4
+Version: 0.5.0
 Summary: A python library for manipulating a stash database
 Home-page: https://github.com/7dJx1qP/pystashlib
 Author: 7dJx1qP
 Author-email: 38586902+7dJx1qP@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cloudscraper
 Requires-Dist: pyyaml
 Requires-Dist: python-dateutil
+Requires-Dist: requests
 Provides-Extra: html
 Requires-Dist: lxml; extra == "html"
 
 A python library for querying and updating a stash sqlite database
 
 pystashlib and Stash compatibility table:
 | pystashlib | Stash version | Stash schema |
 | ------------- | ------------- | ------------- |
-| v0.4.0-v0.4.4 | v0.24.0-v0.24.3 | 54 |
+| v0.5.0 | v0.25.0-v0.25.1 | 55 |
+| v0.4.0-v0.4.5 | v0.24.0-v0.24.3 | 54 |
 | v0.3.0-v0.3.1 | v0.17.0-v0.17.2 | 36 |
 | v0.2.8 | v0.15.0-v0.16.1 | 31 |
 | v0.2.7 | v0.14.0 | 30 |
 | v0.2.5 | v0.12.0-v0.13.1 | 29 |
 | v0.2.4 | v0.11.0 | 28 |
 
 # Changelog
 
+## v0.5.0
+* Update to support Stash v0.25.0
+
+## v0.4.5
+* Add `requests` package to list of requirements
+
 ## v0.4.4
 * Updated StashInterface GQL client to support Stash v0.24.3
 
 ## v0.4.3
 *  Added support for performer name disambiguation
 
 ### Changed
```

### Comparing `pystashlib-0.4.4/pystashlib.egg-info/PKG-INFO` & `pystashlib-0.5.0/pystashlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 Metadata-Version: 2.1
 Name: pystashlib
-Version: 0.4.4
+Version: 0.5.0
 Summary: A python library for manipulating a stash database
 Home-page: https://github.com/7dJx1qP/pystashlib
 Author: 7dJx1qP
 Author-email: 38586902+7dJx1qP@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Requires-Dist: cloudscraper
 Requires-Dist: pyyaml
 Requires-Dist: python-dateutil
+Requires-Dist: requests
 Provides-Extra: html
 Requires-Dist: lxml; extra == "html"
 
 A python library for querying and updating a stash sqlite database
 
 pystashlib and Stash compatibility table:
 | pystashlib | Stash version | Stash schema |
 | ------------- | ------------- | ------------- |
-| v0.4.0-v0.4.4 | v0.24.0-v0.24.3 | 54 |
+| v0.5.0 | v0.25.0-v0.25.1 | 55 |
+| v0.4.0-v0.4.5 | v0.24.0-v0.24.3 | 54 |
 | v0.3.0-v0.3.1 | v0.17.0-v0.17.2 | 36 |
 | v0.2.8 | v0.15.0-v0.16.1 | 31 |
 | v0.2.7 | v0.14.0 | 30 |
 | v0.2.5 | v0.12.0-v0.13.1 | 29 |
 | v0.2.4 | v0.11.0 | 28 |
 
 # Changelog
 
+## v0.5.0
+* Update to support Stash v0.25.0
+
+## v0.4.5
+* Add `requests` package to list of requirements
+
 ## v0.4.4
 * Updated StashInterface GQL client to support Stash v0.24.3
 
 ## v0.4.3
 *  Added support for performer name disambiguation
 
 ### Changed
```

### Comparing `pystashlib-0.4.4/pystashlib.egg-info/SOURCES.txt` & `pystashlib-0.5.0/pystashlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/setup.py` & `pystashlib-0.5.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="pystashlib",
-    version="0.4.4",
+    version="0.5.0",
     description="A python library for manipulating a stash database",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/7dJx1qP/pystashlib",
     author="7dJx1qP",
     author_email="38586902+7dJx1qP@users.noreply.github.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.11",
     ],
     packages=["stashlib"],
     include_package_data=True,
-    install_requires=["cloudscraper", "pyyaml", "python-dateutil"],
+    install_requires=["cloudscraper", "pyyaml", "python-dateutil", "requests"],
     extras_require={
         "html": ["lxml"],
     },
 )
```

### Comparing `pystashlib-0.4.4/stashlib/common.py` & `pystashlib-0.5.0/stashlib/common.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/database.py` & `pystashlib-0.5.0/stashlib/database.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/html.py` & `pystashlib-0.5.0/stashlib/html.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/log.py` & `pystashlib-0.5.0/stashlib/log.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/logger.py` & `pystashlib-0.5.0/stashlib/logger.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/scene_filename_parser.py` & `pystashlib-0.5.0/stashlib/scene_filename_parser.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/sqlite_wrapper.py` & `pystashlib-0.5.0/stashlib/sqlite_wrapper.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/stash_database.py` & `pystashlib-0.5.0/stashlib/stash_database.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/stash_database_base.py` & `pystashlib-0.5.0/stashlib/stash_database_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from . import sqlite_wrapper as sq
 from .database import Database
 from .stash_tables import *
 
 class StashDatabaseBase(Database):
 
-	SCHEMA_VERSION = 54
+	SCHEMA_VERSION = 55
 
 	def __init__(self, db_path):
 		super().__init__(db_path)
 		self.schema_migrations = SchemaMigrations(self.conn)
 		self.tags = Tags(self.conn)
 		self.sqlite_sequence = SqliteSequence(self.conn)
 		self.performer_stash_ids = PerformerStashIds(self.conn)
@@ -40,16 +40,18 @@
 		self.tag_aliases = TagAliases(self.conn)
 		self.studio_aliases = StudioAliases(self.conn)
 		self.performer_aliases = PerformerAliases(self.conn)
 		self.performers = Performers(self.conn)
 		self.galleries_chapters = GalleriesChapters(self.conn)
 		self.blobs = Blobs(self.conn)
 		self.scene_urls = SceneUrls(self.conn)
-		self.scenes = Scenes(self.conn)
 		self.scene_markers = SceneMarkers(self.conn)
 		self.movies = Movies(self.conn)
 		self.studios = Studios(self.conn)
 		self.saved_filters = SavedFilters(self.conn)
 		self.image_urls = ImageUrls(self.conn)
 		self.images = Images(self.conn)
 		self.gallery_urls = GalleryUrls(self.conn)
 		self.galleries = Galleries(self.conn)
+		self.scenes_view_dates = ScenesViewDates(self.conn)
+		self.scenes_o_dates = ScenesODates(self.conn)
+		self.scenes = Scenes(self.conn)
```

### Comparing `pystashlib-0.4.4/stashlib/stash_interface.py` & `pystashlib-0.5.0/stashlib/stash_interface.py`

 * *Files identical despite different names*

### Comparing `pystashlib-0.4.4/stashlib/stash_models.py` & `pystashlib-0.5.0/stashlib/stash_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1922,184 +1922,14 @@
 
 	def values_list(self, include_id=False):
 		if include_id:
 			return [self.scene_id, self.position, self.url]
 		else:
 			return [self.scene_id, self.position, self.url]
 
-class ScenesRow(TableRow):
-	def __init__(self):
-		super().__init__('scenes')
-		self._id = None
-		self._title = None
-		self._details = None
-		self._date = None
-		self._rating = None
-		self._studio_id = None
-		self._o_counter = None
-		self._organized = None
-		self._created_at = None
-		self._updated_at = None
-		self._code = None
-		self._director = None
-		self._resume_time = None
-		self._last_played_at = None
-		self._play_count = None
-		self._play_duration = None
-		self._cover_blob = None
-
-	@property
-	def table_name(self):
-		return self._table_name
-
-	@property
-	def id(self):
-		return self._id
-
-	@id.setter
-	def id(self, id):
-		self._id = id
-
-	@property
-	def title(self):
-		return self._title
-
-	@title.setter
-	def title(self, title):
-		self._title = title
-
-	@property
-	def details(self):
-		return self._details
-
-	@details.setter
-	def details(self, details):
-		self._details = details
-
-	@property
-	def date(self):
-		return self._date
-
-	@date.setter
-	def date(self, date):
-		self._date = date
-
-	@property
-	def rating(self):
-		return self._rating
-
-	@rating.setter
-	def rating(self, rating):
-		self._rating = rating
-
-	@property
-	def studio_id(self):
-		return self._studio_id
-
-	@studio_id.setter
-	def studio_id(self, studio_id):
-		self._studio_id = studio_id
-
-	@property
-	def o_counter(self):
-		return self._o_counter
-
-	@o_counter.setter
-	def o_counter(self, o_counter):
-		self._o_counter = o_counter
-
-	@property
-	def organized(self):
-		return self._organized
-
-	@organized.setter
-	def organized(self, organized):
-		self._organized = organized
-
-	@property
-	def created_at(self):
-		return self._created_at
-
-	@created_at.setter
-	def created_at(self, created_at):
-		self._created_at = created_at
-
-	@property
-	def updated_at(self):
-		return self._updated_at
-
-	@updated_at.setter
-	def updated_at(self, updated_at):
-		self._updated_at = updated_at
-
-	@property
-	def code(self):
-		return self._code
-
-	@code.setter
-	def code(self, code):
-		self._code = code
-
-	@property
-	def director(self):
-		return self._director
-
-	@director.setter
-	def director(self, director):
-		self._director = director
-
-	@property
-	def resume_time(self):
-		return self._resume_time
-
-	@resume_time.setter
-	def resume_time(self, resume_time):
-		self._resume_time = resume_time
-
-	@property
-	def last_played_at(self):
-		return self._last_played_at
-
-	@last_played_at.setter
-	def last_played_at(self, last_played_at):
-		self._last_played_at = last_played_at
-
-	@property
-	def play_count(self):
-		return self._play_count
-
-	@play_count.setter
-	def play_count(self, play_count):
-		self._play_count = play_count
-
-	@property
-	def play_duration(self):
-		return self._play_duration
-
-	@play_duration.setter
-	def play_duration(self, play_duration):
-		self._play_duration = play_duration
-
-	@property
-	def cover_blob(self):
-		return self._cover_blob
-
-	@cover_blob.setter
-	def cover_blob(self, cover_blob):
-		self._cover_blob = cover_blob
-
-	def __str__(self):
-		return str(self.__class__) + ": " + str(self.__dict__)
-
-	def values_list(self, include_id=False):
-		if include_id:
-			return [self.id, self.title, self.details, self.date, self.rating, self.studio_id, self.o_counter, self.organized, self.created_at, self.updated_at, self.code, self.director, self.resume_time, self.last_played_at, self.play_count, self.play_duration, self.cover_blob]
-		else:
-			return [self.title, self.details, self.date, self.rating, self.studio_id, self.o_counter, self.organized, self.created_at, self.updated_at, self.code, self.director, self.resume_time, self.last_played_at, self.play_count, self.play_duration, self.cover_blob]
-
 class SceneMarkersRow(TableRow):
 	def __init__(self):
 		super().__init__('scene_markers')
 		self._id = None
 		self._title = None
 		self._seconds = None
 		self._primary_tag_id = None
@@ -2831,7 +2661,220 @@
 
 	def values_list(self, include_id=False):
 		if include_id:
 			return [self.id, self.folder_id, self.title, self.date, self.details, self.studio_id, self.rating, self.organized, self.created_at, self.updated_at, self.code, self.photographer]
 		else:
 			return [self.folder_id, self.title, self.date, self.details, self.studio_id, self.rating, self.organized, self.created_at, self.updated_at, self.code, self.photographer]
 
+class ScenesViewDatesRow(TableRow):
+	def __init__(self):
+		super().__init__('scenes_view_dates')
+		self._scene_id = None
+		self._view_date = None
+
+	@property
+	def table_name(self):
+		return self._table_name
+
+	@property
+	def scene_id(self):
+		return self._scene_id
+
+	@scene_id.setter
+	def scene_id(self, scene_id):
+		self._scene_id = scene_id
+
+	@property
+	def view_date(self):
+		return self._view_date
+
+	@view_date.setter
+	def view_date(self, view_date):
+		self._view_date = view_date
+
+	def __str__(self):
+		return str(self.__class__) + ": " + str(self.__dict__)
+
+	def values_list(self, include_id=False):
+		if include_id:
+			return [self.scene_id, self.view_date]
+		else:
+			return [self.scene_id, self.view_date]
+
+class ScenesODatesRow(TableRow):
+	def __init__(self):
+		super().__init__('scenes_o_dates')
+		self._scene_id = None
+		self._o_date = None
+
+	@property
+	def table_name(self):
+		return self._table_name
+
+	@property
+	def scene_id(self):
+		return self._scene_id
+
+	@scene_id.setter
+	def scene_id(self, scene_id):
+		self._scene_id = scene_id
+
+	@property
+	def o_date(self):
+		return self._o_date
+
+	@o_date.setter
+	def o_date(self, o_date):
+		self._o_date = o_date
+
+	def __str__(self):
+		return str(self.__class__) + ": " + str(self.__dict__)
+
+	def values_list(self, include_id=False):
+		if include_id:
+			return [self.scene_id, self.o_date]
+		else:
+			return [self.scene_id, self.o_date]
+
+class ScenesRow(TableRow):
+	def __init__(self):
+		super().__init__('scenes')
+		self._id = None
+		self._title = None
+		self._details = None
+		self._date = None
+		self._rating = None
+		self._studio_id = None
+		self._organized = None
+		self._created_at = None
+		self._updated_at = None
+		self._code = None
+		self._director = None
+		self._resume_time = None
+		self._play_duration = None
+		self._cover_blob = None
+
+	@property
+	def table_name(self):
+		return self._table_name
+
+	@property
+	def id(self):
+		return self._id
+
+	@id.setter
+	def id(self, id):
+		self._id = id
+
+	@property
+	def title(self):
+		return self._title
+
+	@title.setter
+	def title(self, title):
+		self._title = title
+
+	@property
+	def details(self):
+		return self._details
+
+	@details.setter
+	def details(self, details):
+		self._details = details
+
+	@property
+	def date(self):
+		return self._date
+
+	@date.setter
+	def date(self, date):
+		self._date = date
+
+	@property
+	def rating(self):
+		return self._rating
+
+	@rating.setter
+	def rating(self, rating):
+		self._rating = rating
+
+	@property
+	def studio_id(self):
+		return self._studio_id
+
+	@studio_id.setter
+	def studio_id(self, studio_id):
+		self._studio_id = studio_id
+
+	@property
+	def organized(self):
+		return self._organized
+
+	@organized.setter
+	def organized(self, organized):
+		self._organized = organized
+
+	@property
+	def created_at(self):
+		return self._created_at
+
+	@created_at.setter
+	def created_at(self, created_at):
+		self._created_at = created_at
+
+	@property
+	def updated_at(self):
+		return self._updated_at
+
+	@updated_at.setter
+	def updated_at(self, updated_at):
+		self._updated_at = updated_at
+
+	@property
+	def code(self):
+		return self._code
+
+	@code.setter
+	def code(self, code):
+		self._code = code
+
+	@property
+	def director(self):
+		return self._director
+
+	@director.setter
+	def director(self, director):
+		self._director = director
+
+	@property
+	def resume_time(self):
+		return self._resume_time
+
+	@resume_time.setter
+	def resume_time(self, resume_time):
+		self._resume_time = resume_time
+
+	@property
+	def play_duration(self):
+		return self._play_duration
+
+	@play_duration.setter
+	def play_duration(self, play_duration):
+		self._play_duration = play_duration
+
+	@property
+	def cover_blob(self):
+		return self._cover_blob
+
+	@cover_blob.setter
+	def cover_blob(self, cover_blob):
+		self._cover_blob = cover_blob
+
+	def __str__(self):
+		return str(self.__class__) + ": " + str(self.__dict__)
+
+	def values_list(self, include_id=False):
+		if include_id:
+			return [self.id, self.title, self.details, self.date, self.rating, self.studio_id, self.organized, self.created_at, self.updated_at, self.code, self.director, self.resume_time, self.play_duration, self.cover_blob]
+		else:
+			return [self.title, self.details, self.date, self.rating, self.studio_id, self.organized, self.created_at, self.updated_at, self.code, self.director, self.resume_time, self.play_duration, self.cover_blob]
+
```

### Comparing `pystashlib-0.4.4/stashlib/stash_tables.py` & `pystashlib-0.5.0/stashlib/stash_tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -3397,420 +3397,14 @@
 
 	def update_url_by_scene_id(self, scene_id, value, commit=True):
 		return self.execute("UPDATE scene_urls SET url = ? WHERE scene_id = ?", [value, scene_id], commit)
 
 	def update_empty_url_by_scene_id(self, scene_id, value, commit=True):
 		return self.execute("UPDATE scene_urls SET url = ? WHERE scene_id = ? AND (url IS NULL OR url = '' OR url = 0)", [value, scene_id], commit)
 
-class Scenes(Table):
-	def __init__(self, conn: sqlite3.Connection):
-		super().__init__(conn, 'scenes')
-
-	def select_id(self, id, colvalues={}, selectcols=['*']):
-		colvalues['id'] = id
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_title(self, title, colvalues={}, selectcols=['*']):
-		colvalues['title'] = title
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_details(self, details, colvalues={}, selectcols=['*']):
-		colvalues['details'] = details
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_date(self, date, colvalues={}, selectcols=['*']):
-		colvalues['date'] = date
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_rating(self, rating, colvalues={}, selectcols=['*']):
-		colvalues['rating'] = rating
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_studio_id(self, studio_id, colvalues={}, selectcols=['*']):
-		colvalues['studio_id'] = studio_id
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_o_counter(self, o_counter, colvalues={}, selectcols=['*']):
-		colvalues['o_counter'] = o_counter
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_organized(self, organized, colvalues={}, selectcols=['*']):
-		colvalues['organized'] = organized
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_created_at(self, created_at, colvalues={}, selectcols=['*']):
-		colvalues['created_at'] = created_at
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_updated_at(self, updated_at, colvalues={}, selectcols=['*']):
-		colvalues['updated_at'] = updated_at
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_code(self, code, colvalues={}, selectcols=['*']):
-		colvalues['code'] = code
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_director(self, director, colvalues={}, selectcols=['*']):
-		colvalues['director'] = director
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_resume_time(self, resume_time, colvalues={}, selectcols=['*']):
-		colvalues['resume_time'] = resume_time
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_last_played_at(self, last_played_at, colvalues={}, selectcols=['*']):
-		colvalues['last_played_at'] = last_played_at
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_play_count(self, play_count, colvalues={}, selectcols=['*']):
-		colvalues['play_count'] = play_count
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_play_duration(self, play_duration, colvalues={}, selectcols=['*']):
-		colvalues['play_duration'] = play_duration
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def select_cover_blob(self, cover_blob, colvalues={}, selectcols=['*']):
-		colvalues['cover_blob'] = cover_blob
-		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
-
-	def selectone_id(self, id, colvalues={}, selectcols=['*']):
-		colvalues['id'] = id
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_title(self, title, colvalues={}, selectcols=['*']):
-		colvalues['title'] = title
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_details(self, details, colvalues={}, selectcols=['*']):
-		colvalues['details'] = details
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_date(self, date, colvalues={}, selectcols=['*']):
-		colvalues['date'] = date
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_rating(self, rating, colvalues={}, selectcols=['*']):
-		colvalues['rating'] = rating
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_studio_id(self, studio_id, colvalues={}, selectcols=['*']):
-		colvalues['studio_id'] = studio_id
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_o_counter(self, o_counter, colvalues={}, selectcols=['*']):
-		colvalues['o_counter'] = o_counter
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_organized(self, organized, colvalues={}, selectcols=['*']):
-		colvalues['organized'] = organized
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_created_at(self, created_at, colvalues={}, selectcols=['*']):
-		colvalues['created_at'] = created_at
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_updated_at(self, updated_at, colvalues={}, selectcols=['*']):
-		colvalues['updated_at'] = updated_at
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_code(self, code, colvalues={}, selectcols=['*']):
-		colvalues['code'] = code
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_director(self, director, colvalues={}, selectcols=['*']):
-		colvalues['director'] = director
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_resume_time(self, resume_time, colvalues={}, selectcols=['*']):
-		colvalues['resume_time'] = resume_time
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_last_played_at(self, last_played_at, colvalues={}, selectcols=['*']):
-		colvalues['last_played_at'] = last_played_at
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_play_count(self, play_count, colvalues={}, selectcols=['*']):
-		colvalues['play_count'] = play_count
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_play_duration(self, play_duration, colvalues={}, selectcols=['*']):
-		colvalues['play_duration'] = play_duration
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def selectone_cover_blob(self, cover_blob, colvalues={}, selectcols=['*']):
-		colvalues['cover_blob'] = cover_blob
-		row = self.selectone(colvalues, selectcols)
-		if row:
-			return ScenesRow().from_sqliterow(row)
-		else:
-			return None
-
-	def insert(self, title, details, date, rating, studio_id, o_counter, organized, created_at, updated_at, code, director, resume_time, last_played_at, play_count, play_duration, cover_blob, commit=True):
-		return self.execute("INSERT INTO scenes (title, details, date, rating, studio_id, o_counter, organized, created_at, updated_at, code, director, resume_time, last_played_at, play_count, play_duration, cover_blob) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", [title, details, date, rating, studio_id, o_counter, organized, created_at, updated_at, code, director, resume_time, last_played_at, play_count, play_duration, cover_blob], commit)
-
-	def insert_model(self, model: ScenesRow, commit=True):
-		return self.execute("INSERT INTO scenes (title, details, date, rating, studio_id, o_counter, organized, created_at, updated_at, code, director, resume_time, last_played_at, play_count, play_duration, cover_blob) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", model.values_list(False), commit)
-
-	def delete_by_id(self, id, commit=True):
-		return self.execute("DELETE FROM scenes WHERE id = ?", [id, ], commit)
-
-	def delete_by_studio_id(self, studio_id, commit=True):
-		return self.execute("DELETE FROM scenes WHERE studio_id = ?", [studio_id, ], commit)
-
-	def update_title_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET title = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_title_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET title = ? WHERE id = ? AND (title IS NULL OR title = '' OR title = 0)", [value, id], commit)
-
-	def update_details_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET details = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_details_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET details = ? WHERE id = ? AND (details IS NULL OR details = '' OR details = 0)", [value, id], commit)
-
-	def update_date_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET date = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_date_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET date = ? WHERE id = ? AND (date IS NULL OR date = '' OR date = 0)", [value, id], commit)
-
-	def update_rating_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET rating = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_rating_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET rating = ? WHERE id = ? AND (rating IS NULL OR rating = '' OR rating = 0)", [value, id], commit)
-
-	def update_studio_id_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET studio_id = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_studio_id_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET studio_id = ? WHERE id = ? AND (studio_id IS NULL OR studio_id = '' OR studio_id = 0)", [value, id], commit)
-
-	def update_o_counter_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET o_counter = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_o_counter_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET o_counter = ? WHERE id = ? AND (o_counter IS NULL OR o_counter = '' OR o_counter = 0)", [value, id], commit)
-
-	def update_organized_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET organized = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_organized_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET organized = ? WHERE id = ? AND (organized IS NULL OR organized = '' OR organized = 0)", [value, id], commit)
-
-	def update_created_at_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET created_at = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_created_at_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET created_at = ? WHERE id = ? AND (created_at IS NULL OR created_at = '' OR created_at = 0)", [value, id], commit)
-
-	def update_updated_at_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET updated_at = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_updated_at_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET updated_at = ? WHERE id = ? AND (updated_at IS NULL OR updated_at = '' OR updated_at = 0)", [value, id], commit)
-
-	def update_code_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET code = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_code_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET code = ? WHERE id = ? AND (code IS NULL OR code = '' OR code = 0)", [value, id], commit)
-
-	def update_director_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET director = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_director_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET director = ? WHERE id = ? AND (director IS NULL OR director = '' OR director = 0)", [value, id], commit)
-
-	def update_resume_time_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET resume_time = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_resume_time_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET resume_time = ? WHERE id = ? AND (resume_time IS NULL OR resume_time = '' OR resume_time = 0)", [value, id], commit)
-
-	def update_last_played_at_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET last_played_at = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_last_played_at_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET last_played_at = ? WHERE id = ? AND (last_played_at IS NULL OR last_played_at = '' OR last_played_at = 0)", [value, id], commit)
-
-	def update_play_count_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_count = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_play_count_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_count = ? WHERE id = ? AND (play_count IS NULL OR play_count = '' OR play_count = 0)", [value, id], commit)
-
-	def update_play_duration_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_duration = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_play_duration_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_duration = ? WHERE id = ? AND (play_duration IS NULL OR play_duration = '' OR play_duration = 0)", [value, id], commit)
-
-	def update_cover_blob_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET cover_blob = ? WHERE id = ?", [value, id], commit)
-
-	def update_empty_cover_blob_by_id(self, id, value, commit=True):
-		return self.execute("UPDATE scenes SET cover_blob = ? WHERE id = ? AND (cover_blob IS NULL OR cover_blob = '' OR cover_blob = 0)", [value, id], commit)
-
-	def update_title_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET title = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_title_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET title = ? WHERE studio_id = ? AND (title IS NULL OR title = '' OR title = 0)", [value, studio_id], commit)
-
-	def update_details_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET details = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_details_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET details = ? WHERE studio_id = ? AND (details IS NULL OR details = '' OR details = 0)", [value, studio_id], commit)
-
-	def update_date_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET date = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_date_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET date = ? WHERE studio_id = ? AND (date IS NULL OR date = '' OR date = 0)", [value, studio_id], commit)
-
-	def update_rating_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET rating = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_rating_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET rating = ? WHERE studio_id = ? AND (rating IS NULL OR rating = '' OR rating = 0)", [value, studio_id], commit)
-
-	def update_o_counter_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET o_counter = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_o_counter_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET o_counter = ? WHERE studio_id = ? AND (o_counter IS NULL OR o_counter = '' OR o_counter = 0)", [value, studio_id], commit)
-
-	def update_organized_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET organized = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_organized_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET organized = ? WHERE studio_id = ? AND (organized IS NULL OR organized = '' OR organized = 0)", [value, studio_id], commit)
-
-	def update_created_at_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET created_at = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_created_at_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET created_at = ? WHERE studio_id = ? AND (created_at IS NULL OR created_at = '' OR created_at = 0)", [value, studio_id], commit)
-
-	def update_updated_at_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET updated_at = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_updated_at_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET updated_at = ? WHERE studio_id = ? AND (updated_at IS NULL OR updated_at = '' OR updated_at = 0)", [value, studio_id], commit)
-
-	def update_code_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET code = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_code_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET code = ? WHERE studio_id = ? AND (code IS NULL OR code = '' OR code = 0)", [value, studio_id], commit)
-
-	def update_director_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET director = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_director_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET director = ? WHERE studio_id = ? AND (director IS NULL OR director = '' OR director = 0)", [value, studio_id], commit)
-
-	def update_resume_time_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET resume_time = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_resume_time_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET resume_time = ? WHERE studio_id = ? AND (resume_time IS NULL OR resume_time = '' OR resume_time = 0)", [value, studio_id], commit)
-
-	def update_last_played_at_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET last_played_at = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_last_played_at_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET last_played_at = ? WHERE studio_id = ? AND (last_played_at IS NULL OR last_played_at = '' OR last_played_at = 0)", [value, studio_id], commit)
-
-	def update_play_count_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_count = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_play_count_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_count = ? WHERE studio_id = ? AND (play_count IS NULL OR play_count = '' OR play_count = 0)", [value, studio_id], commit)
-
-	def update_play_duration_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_duration = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_play_duration_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET play_duration = ? WHERE studio_id = ? AND (play_duration IS NULL OR play_duration = '' OR play_duration = 0)", [value, studio_id], commit)
-
-	def update_cover_blob_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET cover_blob = ? WHERE studio_id = ?", [value, studio_id], commit)
-
-	def update_empty_cover_blob_by_studio_id(self, studio_id, value, commit=True):
-		return self.execute("UPDATE scenes SET cover_blob = ? WHERE studio_id = ? AND (cover_blob IS NULL OR cover_blob = '' OR cover_blob = 0)", [value, studio_id], commit)
-
 class SceneMarkers(Table):
 	def __init__(self, conn: sqlite3.Connection):
 		super().__init__(conn, 'scene_markers')
 
 	def select_id(self, id, colvalues={}, selectcols=['*']):
 		colvalues['id'] = id
 		return [SceneMarkersRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
@@ -5569,7 +5163,427 @@
 
 	def update_photographer_by_studio_id(self, studio_id, value, commit=True):
 		return self.execute("UPDATE galleries SET photographer = ? WHERE studio_id = ?", [value, studio_id], commit)
 
 	def update_empty_photographer_by_studio_id(self, studio_id, value, commit=True):
 		return self.execute("UPDATE galleries SET photographer = ? WHERE studio_id = ? AND (photographer IS NULL OR photographer = '' OR photographer = 0)", [value, studio_id], commit)
 
+class ScenesViewDates(Table):
+	def __init__(self, conn: sqlite3.Connection):
+		super().__init__(conn, 'scenes_view_dates')
+
+	def select_scene_id(self, scene_id, colvalues={}, selectcols=['*']):
+		colvalues['scene_id'] = scene_id
+		return [ScenesViewDatesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_view_date(self, view_date, colvalues={}, selectcols=['*']):
+		colvalues['view_date'] = view_date
+		return [ScenesViewDatesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def selectone_scene_id(self, scene_id, colvalues={}, selectcols=['*']):
+		colvalues['scene_id'] = scene_id
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesViewDatesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_view_date(self, view_date, colvalues={}, selectcols=['*']):
+		colvalues['view_date'] = view_date
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesViewDatesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def insert(self, scene_id, view_date, commit=True):
+		return self.execute("INSERT INTO scenes_view_dates (scene_id, view_date) VALUES (?, ?)", [scene_id, view_date], commit)
+
+	def insert_model(self, model: ScenesViewDatesRow, commit=True):
+		return self.execute("INSERT INTO scenes_view_dates (scene_id, view_date) VALUES (?, ?)", model.values_list(False), commit)
+
+	def delete_by_scene_id(self, scene_id, commit=True):
+		return self.execute("DELETE FROM scenes_view_dates WHERE scene_id = ?", [scene_id, ], commit)
+
+	def update_view_date_by_scene_id(self, scene_id, value, commit=True):
+		return self.execute("UPDATE scenes_view_dates SET view_date = ? WHERE scene_id = ?", [value, scene_id], commit)
+
+	def update_empty_view_date_by_scene_id(self, scene_id, value, commit=True):
+		return self.execute("UPDATE scenes_view_dates SET view_date = ? WHERE scene_id = ? AND (view_date IS NULL OR view_date = '' OR view_date = 0)", [value, scene_id], commit)
+
+class ScenesODates(Table):
+	def __init__(self, conn: sqlite3.Connection):
+		super().__init__(conn, 'scenes_o_dates')
+
+	def select_scene_id(self, scene_id, colvalues={}, selectcols=['*']):
+		colvalues['scene_id'] = scene_id
+		return [ScenesODatesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_o_date(self, o_date, colvalues={}, selectcols=['*']):
+		colvalues['o_date'] = o_date
+		return [ScenesODatesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def selectone_scene_id(self, scene_id, colvalues={}, selectcols=['*']):
+		colvalues['scene_id'] = scene_id
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesODatesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_o_date(self, o_date, colvalues={}, selectcols=['*']):
+		colvalues['o_date'] = o_date
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesODatesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def insert(self, scene_id, o_date, commit=True):
+		return self.execute("INSERT INTO scenes_o_dates (scene_id, o_date) VALUES (?, ?)", [scene_id, o_date], commit)
+
+	def insert_model(self, model: ScenesODatesRow, commit=True):
+		return self.execute("INSERT INTO scenes_o_dates (scene_id, o_date) VALUES (?, ?)", model.values_list(False), commit)
+
+	def delete_by_scene_id(self, scene_id, commit=True):
+		return self.execute("DELETE FROM scenes_o_dates WHERE scene_id = ?", [scene_id, ], commit)
+
+	def update_o_date_by_scene_id(self, scene_id, value, commit=True):
+		return self.execute("UPDATE scenes_o_dates SET o_date = ? WHERE scene_id = ?", [value, scene_id], commit)
+
+	def update_empty_o_date_by_scene_id(self, scene_id, value, commit=True):
+		return self.execute("UPDATE scenes_o_dates SET o_date = ? WHERE scene_id = ? AND (o_date IS NULL OR o_date = '' OR o_date = 0)", [value, scene_id], commit)
+
+class Scenes(Table):
+	def __init__(self, conn: sqlite3.Connection):
+		super().__init__(conn, 'scenes')
+
+	def select_id(self, id, colvalues={}, selectcols=['*']):
+		colvalues['id'] = id
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_title(self, title, colvalues={}, selectcols=['*']):
+		colvalues['title'] = title
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_details(self, details, colvalues={}, selectcols=['*']):
+		colvalues['details'] = details
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_date(self, date, colvalues={}, selectcols=['*']):
+		colvalues['date'] = date
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_rating(self, rating, colvalues={}, selectcols=['*']):
+		colvalues['rating'] = rating
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_studio_id(self, studio_id, colvalues={}, selectcols=['*']):
+		colvalues['studio_id'] = studio_id
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_organized(self, organized, colvalues={}, selectcols=['*']):
+		colvalues['organized'] = organized
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_created_at(self, created_at, colvalues={}, selectcols=['*']):
+		colvalues['created_at'] = created_at
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_updated_at(self, updated_at, colvalues={}, selectcols=['*']):
+		colvalues['updated_at'] = updated_at
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_code(self, code, colvalues={}, selectcols=['*']):
+		colvalues['code'] = code
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_director(self, director, colvalues={}, selectcols=['*']):
+		colvalues['director'] = director
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_resume_time(self, resume_time, colvalues={}, selectcols=['*']):
+		colvalues['resume_time'] = resume_time
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_play_duration(self, play_duration, colvalues={}, selectcols=['*']):
+		colvalues['play_duration'] = play_duration
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def select_cover_blob(self, cover_blob, colvalues={}, selectcols=['*']):
+		colvalues['cover_blob'] = cover_blob
+		return [ScenesRow().from_sqliterow(x) for x in self.select(colvalues, selectcols)]
+
+	def selectone_id(self, id, colvalues={}, selectcols=['*']):
+		colvalues['id'] = id
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_title(self, title, colvalues={}, selectcols=['*']):
+		colvalues['title'] = title
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_details(self, details, colvalues={}, selectcols=['*']):
+		colvalues['details'] = details
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_date(self, date, colvalues={}, selectcols=['*']):
+		colvalues['date'] = date
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_rating(self, rating, colvalues={}, selectcols=['*']):
+		colvalues['rating'] = rating
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_studio_id(self, studio_id, colvalues={}, selectcols=['*']):
+		colvalues['studio_id'] = studio_id
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_organized(self, organized, colvalues={}, selectcols=['*']):
+		colvalues['organized'] = organized
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_created_at(self, created_at, colvalues={}, selectcols=['*']):
+		colvalues['created_at'] = created_at
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_updated_at(self, updated_at, colvalues={}, selectcols=['*']):
+		colvalues['updated_at'] = updated_at
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_code(self, code, colvalues={}, selectcols=['*']):
+		colvalues['code'] = code
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_director(self, director, colvalues={}, selectcols=['*']):
+		colvalues['director'] = director
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_resume_time(self, resume_time, colvalues={}, selectcols=['*']):
+		colvalues['resume_time'] = resume_time
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_play_duration(self, play_duration, colvalues={}, selectcols=['*']):
+		colvalues['play_duration'] = play_duration
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def selectone_cover_blob(self, cover_blob, colvalues={}, selectcols=['*']):
+		colvalues['cover_blob'] = cover_blob
+		row = self.selectone(colvalues, selectcols)
+		if row:
+			return ScenesRow().from_sqliterow(row)
+		else:
+			return None
+
+	def insert(self, title, details, date, rating, studio_id, organized, created_at, updated_at, code, director, resume_time, play_duration, cover_blob, commit=True):
+		return self.execute("INSERT INTO scenes (title, details, date, rating, studio_id, organized, created_at, updated_at, code, director, resume_time, play_duration, cover_blob) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", [title, details, date, rating, studio_id, organized, created_at, updated_at, code, director, resume_time, play_duration, cover_blob], commit)
+
+	def insert_model(self, model: ScenesRow, commit=True):
+		return self.execute("INSERT INTO scenes (title, details, date, rating, studio_id, organized, created_at, updated_at, code, director, resume_time, play_duration, cover_blob) VALUES (?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?, ?)", model.values_list(False), commit)
+
+	def delete_by_id(self, id, commit=True):
+		return self.execute("DELETE FROM scenes WHERE id = ?", [id, ], commit)
+
+	def delete_by_studio_id(self, studio_id, commit=True):
+		return self.execute("DELETE FROM scenes WHERE studio_id = ?", [studio_id, ], commit)
+
+	def update_title_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET title = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_title_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET title = ? WHERE id = ? AND (title IS NULL OR title = '' OR title = 0)", [value, id], commit)
+
+	def update_details_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET details = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_details_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET details = ? WHERE id = ? AND (details IS NULL OR details = '' OR details = 0)", [value, id], commit)
+
+	def update_date_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET date = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_date_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET date = ? WHERE id = ? AND (date IS NULL OR date = '' OR date = 0)", [value, id], commit)
+
+	def update_rating_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET rating = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_rating_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET rating = ? WHERE id = ? AND (rating IS NULL OR rating = '' OR rating = 0)", [value, id], commit)
+
+	def update_studio_id_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET studio_id = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_studio_id_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET studio_id = ? WHERE id = ? AND (studio_id IS NULL OR studio_id = '' OR studio_id = 0)", [value, id], commit)
+
+	def update_organized_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET organized = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_organized_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET organized = ? WHERE id = ? AND (organized IS NULL OR organized = '' OR organized = 0)", [value, id], commit)
+
+	def update_created_at_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET created_at = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_created_at_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET created_at = ? WHERE id = ? AND (created_at IS NULL OR created_at = '' OR created_at = 0)", [value, id], commit)
+
+	def update_updated_at_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET updated_at = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_updated_at_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET updated_at = ? WHERE id = ? AND (updated_at IS NULL OR updated_at = '' OR updated_at = 0)", [value, id], commit)
+
+	def update_code_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET code = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_code_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET code = ? WHERE id = ? AND (code IS NULL OR code = '' OR code = 0)", [value, id], commit)
+
+	def update_director_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET director = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_director_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET director = ? WHERE id = ? AND (director IS NULL OR director = '' OR director = 0)", [value, id], commit)
+
+	def update_resume_time_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET resume_time = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_resume_time_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET resume_time = ? WHERE id = ? AND (resume_time IS NULL OR resume_time = '' OR resume_time = 0)", [value, id], commit)
+
+	def update_play_duration_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET play_duration = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_play_duration_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET play_duration = ? WHERE id = ? AND (play_duration IS NULL OR play_duration = '' OR play_duration = 0)", [value, id], commit)
+
+	def update_cover_blob_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET cover_blob = ? WHERE id = ?", [value, id], commit)
+
+	def update_empty_cover_blob_by_id(self, id, value, commit=True):
+		return self.execute("UPDATE scenes SET cover_blob = ? WHERE id = ? AND (cover_blob IS NULL OR cover_blob = '' OR cover_blob = 0)", [value, id], commit)
+
+	def update_title_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET title = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_title_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET title = ? WHERE studio_id = ? AND (title IS NULL OR title = '' OR title = 0)", [value, studio_id], commit)
+
+	def update_details_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET details = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_details_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET details = ? WHERE studio_id = ? AND (details IS NULL OR details = '' OR details = 0)", [value, studio_id], commit)
+
+	def update_date_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET date = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_date_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET date = ? WHERE studio_id = ? AND (date IS NULL OR date = '' OR date = 0)", [value, studio_id], commit)
+
+	def update_rating_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET rating = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_rating_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET rating = ? WHERE studio_id = ? AND (rating IS NULL OR rating = '' OR rating = 0)", [value, studio_id], commit)
+
+	def update_organized_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET organized = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_organized_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET organized = ? WHERE studio_id = ? AND (organized IS NULL OR organized = '' OR organized = 0)", [value, studio_id], commit)
+
+	def update_created_at_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET created_at = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_created_at_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET created_at = ? WHERE studio_id = ? AND (created_at IS NULL OR created_at = '' OR created_at = 0)", [value, studio_id], commit)
+
+	def update_updated_at_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET updated_at = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_updated_at_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET updated_at = ? WHERE studio_id = ? AND (updated_at IS NULL OR updated_at = '' OR updated_at = 0)", [value, studio_id], commit)
+
+	def update_code_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET code = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_code_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET code = ? WHERE studio_id = ? AND (code IS NULL OR code = '' OR code = 0)", [value, studio_id], commit)
+
+	def update_director_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET director = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_director_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET director = ? WHERE studio_id = ? AND (director IS NULL OR director = '' OR director = 0)", [value, studio_id], commit)
+
+	def update_resume_time_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET resume_time = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_resume_time_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET resume_time = ? WHERE studio_id = ? AND (resume_time IS NULL OR resume_time = '' OR resume_time = 0)", [value, studio_id], commit)
+
+	def update_play_duration_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET play_duration = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_play_duration_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET play_duration = ? WHERE studio_id = ? AND (play_duration IS NULL OR play_duration = '' OR play_duration = 0)", [value, studio_id], commit)
+
+	def update_cover_blob_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET cover_blob = ? WHERE studio_id = ?", [value, studio_id], commit)
+
+	def update_empty_cover_blob_by_studio_id(self, studio_id, value, commit=True):
+		return self.execute("UPDATE scenes SET cover_blob = ? WHERE studio_id = ? AND (cover_blob IS NULL OR cover_blob = '' OR cover_blob = 0)", [value, studio_id], commit)
+
```

### Comparing `pystashlib-0.4.4/stashlib/table.py` & `pystashlib-0.5.0/stashlib/table.py`

 * *Files identical despite different names*

