# Comparing `tmp/Mopidy-SevenSegmentDisplay-0.7.5.tar.gz` & `tmp/Mopidy-SevenSegmentDisplay-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mopidy-SevenSegmentDisplay-0.7.5.tar", last modified: Sun Apr  7 08:48:13 2024, max compression
+gzip compressed data, was "Mopidy-SevenSegmentDisplay-0.7.6.tar", last modified: Sun Apr  7 18:19:39 2024, max compression
```

## Comparing `Mopidy-SevenSegmentDisplay-0.7.5.tar` & `Mopidy-SevenSegmentDisplay-0.7.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.248488 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/cava.config
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ext.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/led.py
--rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/lib_nrf24.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/max7219.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/music.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:19:39.125246 Mopidy-SevenSegmentDisplay-0.7.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:19:39.125246 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 18:19:39.000000 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 18:19:39.000000 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:19:39.000000 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 18:19:39.000000 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:19:38.000000 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 18:19:39.000000 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 18:19:39.000000 Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 18:19:39.125246 Mopidy-SevenSegmentDisplay-0.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:19:39.125246 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/cava.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/ext.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/lib_nrf24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3567 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/max7219.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:19:39.125246 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/alwan.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/alwan.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:19:39.125246 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13591 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-07 18:19:39.129246 Mopidy-SevenSegmentDisplay-0.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-07 18:19:23.000000 Mopidy-SevenSegmentDisplay-0.7.6/setup.py
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/LICENSE` & `Mopidy-SevenSegmentDisplay-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO` & `Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt` & `Mopidy-SevenSegmentDisplay-0.7.6/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/PKG-INFO` & `Mopidy-SevenSegmentDisplay-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.5
+Version: 0.7.6
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/README.md` & `Mopidy-SevenSegmentDisplay-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/__init__.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from mopidy import config, ext
 from .http import factory_decorator
 from .actor import Frontend
 
-__version__ = '0.7.5'
+__version__ = '0.7.6'
 
 
 class Extension(ext.Extension):
     dist_name = 'Mopidy-SevenSegmentDisplay'
     ext_name = 'sevensegmentdisplay'
     version = __version__
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/actor.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/actor.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/alert.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/alert.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/animation.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/animation.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/clock.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/clock.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/display.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/display.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,12 +111,12 @@
     def __init__(self, display_enabled, light_sensor, display_min_brightness, display_max_brightness):
         super(DisplayWithPowerSaving, self).__init__(display_enabled)
         self._light_sensor = light_sensor
         self._display_min_brightness = display_min_brightness
         self._display_max_brightness = display_max_brightness
 
     def update_brightness(self):
-        value = self._light_sensor.getValue()
+        value = self._light_sensor.get_value()
 
         brightness = int(round(self._display_min_brightness + (self._display_max_brightness - self._display_min_brightness) * value))
         
         super(DisplayWithPowerSaving, self).set_brightness(brightness)
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/equalizer.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/equalizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,19 +67,19 @@
             self._process = None
 
     def _get_draw_buffer(self):
         if (self._source is not None):
             data = self._source.read(self._chunk)
             if (len(data) < self._chunk):
                 return self._sample
-            self._sample = [self._getSymbol(i / self._bytenorm) for i in struct.unpack(self._fmt, data)]
+            self._sample = [self._get_symbol(i / self._bytenorm) for i in struct.unpack(self._fmt, data)]
 
         return self._sample
 
-    def _getSymbol(self, ratio):
+    def _get_symbol(self, ratio):
         if (ratio > 0.8):
             return Symbols.TOP | Symbols.MIDDLE | Symbols.BOTTOM
         elif (ratio > 0.4):
             return Symbols.MIDDLE | Symbols.BOTTOM
         elif (ratio > 0.1):
             return Symbols.BOTTOM
         return Symbols.NONE
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ext.conf` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/ext.conf`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/gpio.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/gpio.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/http.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/http.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ir.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/ir.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/led.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/led.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import random
 import logging
 import RPi.GPIO as GPIO
 from .lib_nrf24 import NRF24
 
 
 class Led:
-    
+
     def __init__(self, led_enabled):
         self._radio = None
         self._pipes = []
         self._size = 8
 
         if (not led_enabled):
             return
 
         GPIO.setmode(GPIO.BCM)
-        
+
         readingPipe = [0xF0, 0xF0, 0xF0, 0xF0, 0xE1]
 
         import spidev
         spi = spidev.SpiDev()
         spi.open(0, 1)
         spi.cshigh = False
         spi.max_speed_hz = 500000
@@ -31,15 +31,14 @@
 
         self._radio.setPayloadSize(self._size)
         self._radio.setChannel(0x76)
         self._radio.setDataRate(NRF24.BR_1MBPS)
         self._radio.setPALevel(NRF24.PA_MAX)
         self._radio.setAutoAck(True)
         self._radio.openReadingPipe(1, readingPipe)
-        self._radio.printDetails()
 
         self._radio.startListening()
 
     def run(self):
         if self._radio.available():
             r = []
 
@@ -56,16 +55,15 @@
                     pipe[2] == r[3] and
                     pipe[3] == r[4] and
                     pipe[4] == r[5]):
                     return
 
             self._pipes.append([r[1], r[2], r[3], r[4], r[5]])
 
-
-    def setColor(self, red, green, blue):
+    def set_color(self, red, green, blue):
         try:
             if self._radio is None:
                 return
 
             self._radio.stopListening()
 
             for pipe in self._pipes:
@@ -81,17 +79,17 @@
                 else:
                     logging.info("Received: Ack only, no payload")
 
             self._radio.startListening()
         except Exception as inst:
             logging.error(inst)
         
-    def setColorHsv(self, hue, sat = 1, val = 1):
+    def set_color_hsv(self, hue, sat = 1, val = 1):
         c = colorsys.hsv_to_rgb(hue / 360.0, sat, val)
             
-        self.setColor(int(c[0] * 255), int(c[1] * 255), int(c[2] * 255))
+        self.set_color(int(c[0] * 255), int(c[1] * 255), int(c[2] * 255))
 
-    def setRandomColor(self):
-        self.setColorHsv(random.random() * 360)
+    def set_random_color(self):
+        self.set_color_hsv(random.random() * 360)
 
-    def setNoneColor(self):
-        self.setColor(0, 0, 0)
+    def set_none_color(self):
+        self.set_color(0, 0, 0)
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/lib_nrf24.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/lib_nrf24.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/light_sensor.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/light_sensor.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,14 +43,15 @@
             [0, 0, 0, 0, 0, 0, 0, 0],
             [0, 0, S, L, E, E, P, 0]
         ]
     }
 
     _max_value = 26000
     _channel = None
+    _value = 0.5
 
     def __init__(self, enabled, timeout, sudden_change_callback, sudden_change_timeout_callback):
         super(LightSensor, self).__init__()
         
         self._timeout = timeout
         self._sudden_change_callback = sudden_change_callback
         self._sudden_change_timeout_callback = sudden_change_timeout_callback
@@ -71,49 +72,54 @@
 
         # Define the analog input channel
         self._channel = AnalogIn(self._ads, ADS.P0)
 
         super(LightSensor, self).start()
 
     def run(self):
-        previous_value = self.getValue()
+        previous_value = self.read_value()
         timeout = -1
         min_value = 200 / self._max_value
         max_value = 500 / self._max_value
 
         while (True):
             if (self.stopped()):
                 break
 
-            value = self.getValue()
+            self._value = self.read_value()
 
-            if (value < min_value and previous_value > max_value):
+            if (self._value < min_value and previous_value > max_value):
                 self._sudden_change_callback(datetime.now(), True)
                 timeout = 0
-            elif (value > max_value and previous_value < min_value):
+            elif (self._value > max_value and previous_value < min_value):
                 self._sudden_change_callback(datetime.now(), False)
                 timeout = 0
 
             if (timeout > self._timeout * 60 * 10):
                 self._sudden_change_timeout_callback()
                 timeout = -1
 
-            previous_value = value
+            previous_value = self._value
 
             if (timeout >= 0):
                 timeout += 1
 
             time.sleep(0.1)
 
         self._i2c.deinit()
 
-    def getValue(self):
+    def read_value(self):
         if (self._channel is None):
             return 0.5
-        
-        if (self._channel.value > self._max_value):
+
+        value = self._channel.value
+
+        if (value > self._max_value):
             return 1
 
-        return self._channel.value / self._max_value
+        return value / self._max_value
+    
+    def get_value(self):
+        return self._value
     
     def get_draw_sleep_animation(self):
         return self.ANIMATION_SLEEP
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/max7219.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/max7219.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/menu.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/menu.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/music.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/music.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.css` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/alwan.min.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.js` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/alwan.min.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap-theme.css` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.css` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.js` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/jquery.js` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/static/jquery.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/base.html` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/templates/base.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/index.html` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/templates/index.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/timer.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/timer.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/worker.py` & `Mopidy-SevenSegmentDisplay-0.7.6/mopidy_sevensegmentdisplay/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                     sleep(1)
 
         except Exception as inst:
             logging.error(inst)
         finally:
             self.equalizer.stop()
             self.ir_sender.stop()
-            self.led.setNoneColor()
+            self.led.set_none_color()
             self.gpio.cleanup()
             self.display.stop()
             self.light_sensor.stop()
 
     def _init_menu(self):
         self.MENU = {
             "get_sub_menu": lambda: [
@@ -252,21 +252,21 @@
                     self.timer_off.increase()
                     self.timer_off.increase()
                     self.menu.draw_sub_menu_animation(self.light_sensor.get_draw_sleep_animation())
                 else:
                     self.timer_off.reset()
         else:
             if (is_dark):
-                self.led.setRandomColor()
+                self.led.set_random_color()
             else:
-                self.led.setNoneColor()
+                self.led.set_none_color()
 
     def _on_light_sensor_sudden_change_timeout(self):
         if (not self.music.is_playing()):
-            self.led.setNoneColor()
+            self.led.set_none_color()
 
     def _on_change_preset(self, value):
         self.music.set_preset(value)
         if (value < 0):
             self.menu.click_left(self.MENU_STYLE)
         else:
             self.menu.click_right(self.MENU_STYLE)
@@ -284,15 +284,15 @@
             self.timer_off.decrease()
             self.menu.draw_sub_menu(self.MENU_TIMER_OFF)
         else:
             self.timer_on.decrease()
             self.menu.draw_sub_menu(self.MENU_TIMER_ON)
 
     def set_led_color(self, red, green, blue):
-        self.led.setColor(red, green, blue)
+        self.led.set_color(red, green, blue)
 
     def run_alert(self):
         self.menu.draw_sub_menu_animation(self.alert.get_draw_alert_animation())
         self.alert.run()
 
     def get_presets(self):
         return self.music.get_presets()
@@ -332,20 +332,20 @@
     def on_started(self):
         self.menu.draw_sub_menu_animation(self.music.get_draw_start_animation())
 
     def on_stopped(self):
         self.menu.draw_sub_menu_animation(self.music.get_draw_stop_animation())
         self.timer_off.reset()
         self.ir_sender.power(False)
-        self.led.setNoneColor()
+        self.led.set_none_color()
 
     def on_playing(self):
         self.menu.draw_sub_menu_animation(self.music.get_draw_play_animation())
         self.timer_on.reset()
-        self.led.setRandomColor()
+        self.led.set_random_color()
 
         if (self.music.is_playing()):
             self.ir_sender.power(True)
 
     def on_paused(self):
         self.menu.draw_sub_menu_animation(self.music.get_draw_pause_animation())
 
@@ -355,15 +355,15 @@
     def on_mute(self, mute):
         if mute:
             self.on_volume_changed(0)
         else:
             self.on_volume_changed()
 
     def on_new_track_playing(self):
-        self.led.setRandomColor()
+        self.led.set_random_color()
 
     def on_volume_changed(self, volume=None):
         if (self.menu is not None and self.music is not None and self.music.is_volume_changed(volume)):
             self.menu.draw_sub_menu(self.MENU_VOLUME)
 
     def on_playback_state_changed(self, old_state, new_state):
         if (old_state != new_state):
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.5/setup.py` & `Mopidy-SevenSegmentDisplay-0.7.6/setup.py`

 * *Files identical despite different names*

