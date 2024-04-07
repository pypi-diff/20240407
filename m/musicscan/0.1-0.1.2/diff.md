# Comparing `tmp/musicscan-0.1.tar.gz` & `tmp/musicscan-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musicscan-0.1.tar", last modified: Thu Apr  4 11:05:17 2024, max compression
+gzip compressed data, was "musicscan-0.1.2.tar", last modified: Sun Apr  7 12:49:33 2024, max compression
```

## Comparing `musicscan-0.1.tar` & `musicscan-0.1.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.175122 musicscan-0.1/
--rw-r--r--   0 chrisj     (102) other        (1)     1071 2024-02-17 16:38:18.000000 musicscan-0.1/LICENSE
--rw-r--r--   0 chrisj     (102) other        (1)     4294 2024-04-04 11:05:17.175028 musicscan-0.1/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)     3240 2024-04-04 10:36:09.000000 musicscan-0.1/README.md
--rw-r--r--   0 chrisj     (102) other        (1)     1192 2024-04-04 11:04:53.000000 musicscan-0.1/pyproject.toml
--rw-r--r--   0 chrisj     (102) other        (1)      150 2024-04-04 11:05:17.175692 musicscan-0.1/setup.cfg
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.162533 musicscan-0.1/src/
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.165335 musicscan-0.1/src/musicscan/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:52.000000 musicscan-0.1/src/musicscan/__init__.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.170475 musicscan-0.1/src/musicscan/data/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:59.000000 musicscan-0.1/src/musicscan/data/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     5803 2024-04-03 01:25:41.000000 musicscan-0.1/src/musicscan/data/analyzer.py
--rw-r--r--   0 chrisj     (102) other        (1)     2199 2024-04-03 01:26:18.000000 musicscan-0.1/src/musicscan/data/artist.py
--rw-r--r--   0 chrisj     (102) other        (1)     5019 2024-04-03 01:41:03.000000 musicscan-0.1/src/musicscan/data/cd.py
--rw-r--r--   0 chrisj     (102) other        (1)     3463 2024-04-03 01:26:36.000000 musicscan-0.1/src/musicscan/data/flags.py
--rw-r--r--   0 chrisj     (102) other        (1)     4082 2024-04-03 01:26:06.000000 musicscan-0.1/src/musicscan/data/library.py
--rw-r--r--   0 chrisj     (102) other        (1)     2973 2024-04-03 01:26:55.000000 musicscan-0.1/src/musicscan/data/stringtools.py
--rw-r--r--   0 chrisj     (102) other        (1)     4124 2024-04-03 01:25:53.000000 musicscan-0.1/src/musicscan/data/titletools.py
--rw-r--r--   0 chrisj     (102) other        (1)     3954 2024-04-03 01:40:45.000000 musicscan-0.1/src/musicscan/data/track.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.171934 musicscan-0.1/src/musicscan/fileops/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:02.000000 musicscan-0.1/src/musicscan/fileops/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     1370 2024-04-03 01:27:53.000000 musicscan-0.1/src/musicscan/fileops/filenames.py
--rw-r--r--   0 chrisj     (102) other        (1)     3316 2024-04-03 01:27:23.000000 musicscan-0.1/src/musicscan/fileops/scanner.py
--rw-r--r--   0 chrisj     (102) other        (1)     5556 2024-04-04 03:19:55.000000 musicscan-0.1/src/musicscan/fileops/xmlwriter.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.172692 musicscan-0.1/src/musicscan/generic/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:05.000000 musicscan-0.1/src/musicscan/generic/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     2485 2024-02-25 01:18:01.000000 musicscan-0.1/src/musicscan/generic/stats.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.173442 musicscan-0.1/src/musicscan/tools/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:09.000000 musicscan-0.1/src/musicscan/tools/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)     5946 2024-04-04 03:21:05.000000 musicscan-0.1/src/musicscan/tools/id3scan.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.174220 musicscan-0.1/src/musicscan/xml/
--rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-04-03 01:29:17.000000 musicscan-0.1/src/musicscan/xml/__init__.py
--rw-r--r--   0 chrisj     (102) other        (1)    11776 2024-04-04 10:37:23.000000 musicscan-0.1/src/musicscan/xml/builder.py
-drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-04 11:05:17.174615 musicscan-0.1/src/musicscan.egg-info/
--rw-r--r--   0 chrisj     (102) other        (1)     4294 2024-04-04 11:05:17.000000 musicscan-0.1/src/musicscan.egg-info/PKG-INFO
--rw-r--r--   0 chrisj     (102) other        (1)      845 2024-04-04 11:05:17.000000 musicscan-0.1/src/musicscan.egg-info/SOURCES.txt
--rw-r--r--   0 chrisj     (102) other        (1)        1 2024-04-04 11:05:17.000000 musicscan-0.1/src/musicscan.egg-info/dependency_links.txt
--rw-r--r--   0 chrisj     (102) other        (1)        8 2024-04-04 11:05:17.000000 musicscan-0.1/src/musicscan.egg-info/requires.txt
--rw-r--r--   0 chrisj     (102) other        (1)       10 2024-04-04 11:05:17.000000 musicscan-0.1/src/musicscan.egg-info/top_level.txt
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.428525 musicscan-0.1.2/
+-rw-r--r--   0 chrisj     (102) other        (1)     1071 2024-02-17 16:38:18.000000 musicscan-0.1.2/LICENSE
+-rw-r--r--   0 chrisj     (102) other        (1)     6224 2024-04-07 12:49:33.428434 musicscan-0.1.2/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)     5168 2024-04-06 20:54:31.000000 musicscan-0.1.2/README.md
+-rw-r--r--   0 chrisj     (102) other        (1)     1194 2024-04-07 12:47:49.000000 musicscan-0.1.2/pyproject.toml
+-rw-r--r--   0 chrisj     (102) other        (1)      150 2024-04-07 12:49:33.429117 musicscan-0.1.2/setup.cfg
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.415646 musicscan-0.1.2/src/
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.418407 musicscan-0.1.2/src/musicscan/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:52.000000 musicscan-0.1.2/src/musicscan/__init__.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.423748 musicscan-0.1.2/src/musicscan/data/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:41:59.000000 musicscan-0.1.2/src/musicscan/data/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5803 2024-04-03 01:25:41.000000 musicscan-0.1.2/src/musicscan/data/analyzer.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2199 2024-04-03 01:26:18.000000 musicscan-0.1.2/src/musicscan/data/artist.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5019 2024-04-03 01:41:03.000000 musicscan-0.1.2/src/musicscan/data/cd.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3541 2024-04-06 21:04:19.000000 musicscan-0.1.2/src/musicscan/data/flags.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4082 2024-04-03 01:26:06.000000 musicscan-0.1.2/src/musicscan/data/library.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2973 2024-04-03 01:26:55.000000 musicscan-0.1.2/src/musicscan/data/stringtools.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4124 2024-04-03 01:25:53.000000 musicscan-0.1.2/src/musicscan/data/titletools.py
+-rw-r--r--   0 chrisj     (102) other        (1)     4084 2024-04-06 21:23:16.000000 musicscan-0.1.2/src/musicscan/data/track.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.425250 musicscan-0.1.2/src/musicscan/fileops/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:02.000000 musicscan-0.1.2/src/musicscan/fileops/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     1370 2024-04-03 01:27:53.000000 musicscan-0.1.2/src/musicscan/fileops/filenames.py
+-rw-r--r--   0 chrisj     (102) other        (1)     3316 2024-04-03 01:27:23.000000 musicscan-0.1.2/src/musicscan/fileops/scanner.py
+-rw-r--r--   0 chrisj     (102) other        (1)     5556 2024-04-04 03:19:55.000000 musicscan-0.1.2/src/musicscan/fileops/xmlwriter.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.426014 musicscan-0.1.2/src/musicscan/generic/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:05.000000 musicscan-0.1.2/src/musicscan/generic/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     2485 2024-02-25 01:18:01.000000 musicscan-0.1.2/src/musicscan/generic/stats.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.426774 musicscan-0.1.2/src/musicscan/tools/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-02-10 15:42:09.000000 musicscan-0.1.2/src/musicscan/tools/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)     6103 2024-04-07 12:41:49.000000 musicscan-0.1.2/src/musicscan/tools/id3scan.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.427606 musicscan-0.1.2/src/musicscan/xml/
+-rw-r--r--   0 chrisj     (102) other        (1)     1116 2024-04-03 01:29:17.000000 musicscan-0.1.2/src/musicscan/xml/__init__.py
+-rw-r--r--   0 chrisj     (102) other        (1)    12012 2024-04-06 21:20:18.000000 musicscan-0.1.2/src/musicscan/xml/builder.py
+drwxr-xr-x   0 chrisj     (102) other        (1)        0 2024-04-07 12:49:33.428011 musicscan-0.1.2/src/musicscan.egg-info/
+-rw-r--r--   0 chrisj     (102) other        (1)     6224 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/PKG-INFO
+-rw-r--r--   0 chrisj     (102) other        (1)      845 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/SOURCES.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        1 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/dependency_links.txt
+-rw-r--r--   0 chrisj     (102) other        (1)        8 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/requires.txt
+-rw-r--r--   0 chrisj     (102) other        (1)       10 2024-04-07 12:49:33.000000 musicscan-0.1.2/src/musicscan.egg-info/top_level.txt
```

### Comparing `musicscan-0.1/LICENSE` & `musicscan-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/pyproject.toml` & `musicscan-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "musicscan"
-version = "0.1"
+version = "0.1.2"
 description = "Package for converting music metadata to XML"
 readme = "README.md"
 requires-python = ">3.8"
 dependencies = [
   "tinytag"
 ]
```

### Comparing `musicscan-0.1/src/musicscan/__init__.py` & `musicscan-0.1.2/src/musicscan/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/__init__.py` & `musicscan-0.1.2/src/musicscan/data/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/analyzer.py` & `musicscan-0.1.2/src/musicscan/data/analyzer.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/artist.py` & `musicscan-0.1.2/src/musicscan/data/artist.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/cd.py` & `musicscan-0.1.2/src/musicscan/data/cd.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/flags.py` & `musicscan-0.1.2/src/musicscan/data/flags.py`

 * *Files 7% similar despite different names*

```diff
@@ -72,14 +72,15 @@
     d_parenthesis = 11
     l_group = 20
     p_feat_artist = 30
     p_live = 31
     p_demo = 32
     p_blank_track = 40
     p_genre_country_folk = 50
+    m_year = 60
 
     @classmethod
     def to_str(cls, in_code):
         '''
         Convert a flag value to a usable string.
         '''
         matrix = {FlagCodes.p_greatest: 'possible_greatest_hits',
@@ -90,11 +91,12 @@
                   FlagCodes.d_parenthesis: 'detected_parenthesis',
                   FlagCodes.l_group: 'likely_group_artist',
                   FlagCodes.p_feat_artist: 'possible_featured_artist',
                   FlagCodes.p_live: 'possible_live_performance',
                   FlagCodes.p_demo: 'possible_demo_performance',
                   FlagCodes.p_blank_track: 'possible_blank_track',
                   FlagCodes.p_genre_country_folk:
-                  'country_and_folk_genre_is_too_vague'}
+                  'country_and_folk_genre_is_too_vague',
+                  FlagCodes.m_year: 'missing_copyright_year'}
         if in_code in matrix:
             return matrix[in_code]
         return ''
```

### Comparing `musicscan-0.1/src/musicscan/data/library.py` & `musicscan-0.1.2/src/musicscan/data/library.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/stringtools.py` & `musicscan-0.1.2/src/musicscan/data/stringtools.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/titletools.py` & `musicscan-0.1.2/src/musicscan/data/titletools.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/data/track.py` & `musicscan-0.1.2/src/musicscan/data/track.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 '''
 Data objects for music.
 '''
 
 # pylint: disable=too-many-instance-attributes
 
 from datetime import timedelta
-from musicscan.data.flags import Flags
+from musicscan.data.flags import Flags, FlagCodes
 from musicscan.data.stringtools import sanitize_year
 
 
 class Track():
     '''
     A track identifies a single musical track on an album,
     created through ID3 data.
@@ -44,14 +44,15 @@
         self.album = ''
         self.album_o = None
         self.track_no = 0
         self.bpm = 0
         self.short_title = ''
         self.album_artist = ''
         self.composer = ''
+        self.year = '0000'
         self.flags = Flags()
         self.indices = []
         self._process(in_tag)
 
     def _process(self, in_tag):
         self.title = in_tag.title
         self.genre = in_tag.genre
@@ -72,15 +73,18 @@
         if in_tag.composer:
             self.composer = in_tag.composer
         # self.disc_count = int(in_tag.disc_total)
         self.duration_r = in_tag.duration
         self.duration_f = self.duration_r * 100 / int(100)
         self.duration_t = timedelta(seconds=float(self.duration_f))
         self.duration_s = Track._make_iso_interval(self.duration_t)
-        self.year = sanitize_year(in_tag.year)
+        if in_tag.year:
+            self.year = sanitize_year(in_tag.year)
+        else:
+            self.flags.add_flag(FlagCodes.m_year)
 
     def set_album_object(self, in_album_object):
         '''
         The album object is a reference back to the object that
         contains the track.
         '''
         self.album_o = in_album_object
```

### Comparing `musicscan-0.1/src/musicscan/fileops/__init__.py` & `musicscan-0.1.2/src/musicscan/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/fileops/filenames.py` & `musicscan-0.1.2/src/musicscan/fileops/filenames.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/fileops/scanner.py` & `musicscan-0.1.2/src/musicscan/fileops/scanner.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/fileops/xmlwriter.py` & `musicscan-0.1.2/src/musicscan/fileops/xmlwriter.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/generic/__init__.py` & `musicscan-0.1.2/src/musicscan/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/generic/stats.py` & `musicscan-0.1.2/src/musicscan/generic/stats.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/tools/__init__.py` & `musicscan-0.1.2/src/musicscan/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/tools/id3scan.py` & `musicscan-0.1.2/src/musicscan/tools/id3scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 parse the data, and then generate XML files for
 each musical album.
 
 (Assuming each album is a musical CD)
 
 '''
 
-
 import argparse
 import os
 import os.path
 import sys
 from tinytag import TinyTag
 from musicscan.fileops.scanner import Walker
 from musicscan.fileops.filenames import FilenameMatches
@@ -98,15 +97,15 @@
 
 
 def write_xml_files(in_organizer, in_args, in_stats):
     '''
     Write out the XML files with the accumulated ID3 data.
     '''
     if not os.path.isdir(in_args.outdir):
-        print(F"FAILURE: Cannot write to output path {in_args.outdir}\n")
+        print("\nFAILURE: Cannot write to output path {in_args.outdir}\n")
         sys.exit(1)
     writer = XMLFileWriter(in_args.outdir)
     writer.set_debug(in_args.debug)
     writer.set_overwrite(in_args.overwrite)
     writer.set_split_xml(in_args.splitxml)
     for alb_i in in_organizer.albums:
         writer.write_xml(alb_i)
@@ -143,19 +142,23 @@
                         default=True,
                         help='Add edit flags to output XML')
     parser.add_argument('--debug', action='store_true',
                         default=False,
                         help='write debug info in XML files')
 
     args = parser.parse_args()
-    musicpath = args.musicpath or os.environ['MUSICPATH']
-    stats = Stats()
+    musicpath = args.musicpath
     if not musicpath:
-        parser.print_help()
-        sys.exit(2)
+        if 'MUSICPATH' in os.environ:
+            musicpath = os.environ['MUSICPATH']
+        else:
+            print("\nFAILURE: Can't find a source path for music files.\n")
+            parser.print_help()
+            sys.exit(2)
+    stats = Stats()
     all_files = get_files(musicpath, stats)
     data = scan_files(all_files)
     library = Library()
     organizer = Organizer(library)
     if args.debug:
         show_debug_data(data)
     for entry in data:
```

### Comparing `musicscan-0.1/src/musicscan/xml/__init__.py` & `musicscan-0.1.2/src/musicscan/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `musicscan-0.1/src/musicscan/xml/builder.py` & `musicscan-0.1.2/src/musicscan/xml/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,18 +254,23 @@
         output = f"  <xi:include href='{f_str}'/>\n"
         return output
 
     def build_chunk_catalog(self, in_album):
         '''
         Write out the album catalog element.
         '''
+        first_track = in_album.first_track()
         output = " <catalog>\n"
         output += "  <artists>\n"
-        output += f"  {in_album.artist.to_xml()}\n"
+        output += f"   {in_album.artist.to_xml()}\n"
         output += "  </artists>\n"
+        if first_track.year != '0000':
+            output += "  <copyright>\n" +\
+                      f"   <year>{first_track.year}</year>\n" +\
+                      "  </copyright>\n"
         output += " </catalog>\n"
         return output
 
     def build_chunk_classification(self, in_album):
         '''
         Write out the album classification element.
         '''
@@ -334,15 +339,15 @@
                           f"{sanitize_for_xml(in_track.artist)}" +\
                           "</unkn></artist>\n" +\
                           "   </artists>\n"
             if in_track.composer:
                 output += "   <composers>\n" +\
                           "    <composer><unkn>" +\
                           f"{sanitize_for_xml(in_track.composer)}" +\
-                          "</unkn></composer>" +\
+                          "</unkn></composer>\n" +\
                           "   </composers>\n"
             output += "   </catalog>\n"
         return output
 
     def build_technical(self, in_track):
         '''
         Output the XML technical element for the song.
```

### Comparing `musicscan-0.1/src/musicscan.egg-info/SOURCES.txt` & `musicscan-0.1.2/src/musicscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

