# Comparing `tmp/football_stats_scraper-0.1.5-py3-none-any.whl.zip` & `tmp/football_stats_scraper-0.1.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1958 bytes, number of entries: 5
--rw-rw-r--  2.0 unx     1416 b- defN 24-Apr-06 21:33 football_stats_scraper-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-06 21:33 football_stats_scraper-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx       65 b- defN 24-Apr-06 21:33 football_stats_scraper-0.1.5.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        1 b- defN 24-Apr-06 21:33 football_stats_scraper-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      467 b- defN 24-Apr-06 21:33 football_stats_scraper-0.1.5.dist-info/RECORD
-5 files, 2041 bytes uncompressed, 1070 bytes compressed:  47.6%
+Zip file size: 2090 bytes, number of entries: 5
+-rw-rw-r--  2.0 unx     1797 b- defN 24-Apr-06 22:18 football_stats_scraper-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-06 22:18 football_stats_scraper-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       57 b- defN 24-Apr-06 22:18 football_stats_scraper-0.1.6.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        1 b- defN 24-Apr-06 22:18 football_stats_scraper-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      467 b- defN 24-Apr-06 22:18 football_stats_scraper-0.1.6.dist-info/RECORD
+5 files, 2414 bytes uncompressed, 1202 bytes compressed:  50.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: football_stats_scraper-0.1.5.dist-info/METADATA
+Filename: football_stats_scraper-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: football_stats_scraper-0.1.5.dist-info/WHEEL
+Filename: football_stats_scraper-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: football_stats_scraper-0.1.5.dist-info/entry_points.txt
+Filename: football_stats_scraper-0.1.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: football_stats_scraper-0.1.5.dist-info/top_level.txt
+Filename: football_stats_scraper-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: football_stats_scraper-0.1.5.dist-info/RECORD
+Filename: football_stats_scraper-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `football_stats_scraper-0.1.5.dist-info/METADATA` & `football_stats_scraper-0.1.6.dist-info/METADATA`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: football-stats-scraper
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Python script to scrape football league tables and fixtures
 Home-page: https://github.com/yourusername/football-stats-scraper
 Author: John Murtagh
 Author-email: john90murtagh@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: requests
-Requires-Dist: beautifulsoup4
+Requires-Dist: beautifulsoup4 ==4.12.3
+Requires-Dist: certifi ==2024.2.2
+Requires-Dist: charset-normalizer ==3.3.2
+Requires-Dist: idna ==3.6
+Requires-Dist: lxml ==5.2.1
+Requires-Dist: numpy ==1.26.4
+Requires-Dist: pandas ==2.2.1
+Requires-Dist: python-dateutil ==2.9.0.post0
+Requires-Dist: pytz ==2024.1
+Requires-Dist: requests ==2.31.0
+Requires-Dist: six ==1.16.0
+Requires-Dist: soupsieve ==2.5
+Requires-Dist: tzdata ==2024.1
+Requires-Dist: urllib3 ==2.2.1
 
 # Football Stats Scraper
 
 A Python script to scrape football league tables and fixtures from a source website.
 
 ## Table of Contents
 - [Introduction](#introduction)
```

