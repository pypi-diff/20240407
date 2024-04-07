# Comparing `tmp/Mopidy-SevenSegmentDisplay-0.7.4.tar.gz` & `tmp/Mopidy-SevenSegmentDisplay-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Mopidy-SevenSegmentDisplay-0.7.4.tar", last modified: Sat Apr  6 16:47:18 2024, max compression
+gzip compressed data, was "Mopidy-SevenSegmentDisplay-0.7.5.tar", last modified: Sun Apr  7 08:48:13 2024, max compression
```

## Comparing `Mopidy-SevenSegmentDisplay-0.7.4.tar` & `Mopidy-SevenSegmentDisplay-0.7.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-06 16:47:18.000000 Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.896524 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/alert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/animation.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/cava.config
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/equalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ext.conf
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/http.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ir.py
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/led.py
--rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/lib_nrf24.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/light_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/max7219.py
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/music.py
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/jquery.js
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/threader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-06 16:47:18.900524 Mopidy-SevenSegmentDisplay-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-06 16:47:15.000000 Mopidy-SevenSegmentDisplay-0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 08:48:13.000000 Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.248488 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/alert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/animation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/cava.config
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/equalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ext.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/led.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25861 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/lib_nrf24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/light_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/max7219.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14070 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/music.py
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7867 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    11556 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18860 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   109518 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)    31819 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95786 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/jquery.js
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3506 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/threader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7045 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13576 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-07 08:48:13.252488 Mopidy-SevenSegmentDisplay-0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-04-07 08:48:05.000000 Mopidy-SevenSegmentDisplay-0.7.5/setup.py
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/LICENSE` & `Mopidy-SevenSegmentDisplay-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO` & `Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt` & `Mopidy-SevenSegmentDisplay-0.7.5/Mopidy_SevenSegmentDisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/PKG-INFO` & `Mopidy-SevenSegmentDisplay-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopidy-SevenSegmentDisplay
-Version: 0.7.4
+Version: 0.7.5
 Summary: A Mopidy extension for using it with seven segment display.
 Home-page: https://github.com/JumalIO/mopidy-sevensegmentdisplay
 Author: Julius
 Author-email: spamjulius@mail.com
 Maintainer: Julius
 Maintainer-email: spamjulius@mail.com
 License: Apache License, Version 2.0
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/README.md` & `Mopidy-SevenSegmentDisplay-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/__init__.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from mopidy import config, ext
 from .http import factory_decorator
 from .actor import Frontend
 
-__version__ = '0.7.4'
+__version__ = '0.7.5'
 
 
 class Extension(ext.Extension):
     dist_name = 'Mopidy-SevenSegmentDisplay'
     ext_name = 'sevensegmentdisplay'
     version = __version__
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/actor.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/actor.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/alert.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/alert.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/animation.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/animation.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/clock.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/clock.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/display.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/display.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/equalizer.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/equalizer.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ext.conf` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ext.conf`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/gpio.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/gpio.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/http.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,19 +77,19 @@
         elif (alert == 'run'):
             self.worker.run_alert()
 
         preset = str(self.get_argument('preset', ''))
         if (preset != ''):
             self.worker.set_preset(preset)
 
-        red = int(self.get_argument('red', None))
-        green = int(self.get_argument('green', None))
-        blue = int(self.get_argument('blue', None))
+        red = self.get_argument('red', None)
+        green = self.get_argument('green', None)
+        blue = self.get_argument('blue', None)
         if (red is not None and green is not None and blue is not None):
-            self.worker.set_led_color(red, green, blue)
+            self.worker.set_led_color(int(red), int(green), int(blue))
 
         self.write(str(self.worker.get_volume()))
         self.write(self.worker.get_state())
 
 
 def factory_decorator(worker):
     def app_factory(config, core):
```

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/ir.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/ir.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/led.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/led.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/lib_nrf24.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/lib_nrf24.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/light_sensor.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/light_sensor.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/max7219.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/max7219.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/menu.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/menu.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/music.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/music.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.css` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/alwan.min.js` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/alwan.min.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap-theme.css` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.css` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/bootstrap.js` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/static/jquery.js` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/static/jquery.js`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/base.html` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/base.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/templates/index.html` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/templates/index.html`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/timer.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/timer.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/mopidy_sevensegmentdisplay/worker.py` & `Mopidy-SevenSegmentDisplay-0.7.5/mopidy_sevensegmentdisplay/worker.py`

 * *Files identical despite different names*

### Comparing `Mopidy-SevenSegmentDisplay-0.7.4/setup.py` & `Mopidy-SevenSegmentDisplay-0.7.5/setup.py`

 * *Files identical despite different names*

