# Comparing `tmp/isobar_ext-0.5.1.tar.gz` & `tmp/isobar_ext-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isobar_ext-0.5.1.tar", last modified: Sat Feb  3 22:34:37 2024, max compression
+gzip compressed data, was "isobar_ext-0.9.0.tar", max compression
```

## Comparing `isobar_ext-0.5.1.tar` & `isobar_ext-0.9.0.tar`

### file list

```diff
@@ -1,111 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.895951 isobar_ext-0.5.1/
--rw-rw-rw-   0        0        0     1184 2024-02-03 21:06:21.000000 isobar_ext-0.5.1/LICENSE.md
--rw-rw-rw-   0        0        0    13441 2024-02-03 22:34:37.895951 isobar_ext-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0    12887 2024-02-03 21:06:21.000000 isobar_ext-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.836344 isobar_ext-0.5.1/isobar_ext/
--rw-rw-rw-   0        0        0      608 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/__init__.py
--rw-rw-rw-   0        0        0     1660 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/chord.py
--rw-rw-rw-   0        0        0     5174 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/constants.py
--rw-rw-rw-   0        0        0     1185 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.843346 isobar_ext-0.5.1/isobar_ext/io/
--rw-rw-rw-   0        0        0      993 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.845344 isobar_ext-0.5.1/isobar_ext/io/cv/
--rw-rw-rw-   0        0        0      116 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/cv/__init__.py
--rw-rw-rw-   0        0        0     2940 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/cv/output.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.846345 isobar_ext-0.5.1/isobar_ext/io/dummy/
--rw-rw-rw-   0        0        0       74 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/dummy/__init__.py
--rw-rw-rw-   0        0        0     1002 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/dummy/output.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.848345 isobar_ext-0.5.1/isobar_ext/io/midi/
--rw-rw-rw-   0        0        0      768 2024-02-03 21:59:22.000000 isobar_ext-0.5.1/isobar_ext/io/midi/__init__.py
--rw-rw-rw-   0        0        0     4914 2024-02-03 21:59:22.000000 isobar_ext-0.5.1/isobar_ext/io/midi/input.py
--rw-rw-rw-   0        0        0     3938 2024-02-03 21:59:22.000000 isobar_ext-0.5.1/isobar_ext/io/midi/output.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.850346 isobar_ext-0.5.1/isobar_ext/io/midifile/
--rw-rw-rw-   0        0        0      268 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/midifile/__init__.py
--rw-rw-rw-   0        0        0     6725 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/midifile/input.py
--rw-rw-rw-   0        0        0     4140 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/midifile/output.py
--rw-rw-rw-   0        0        0      349 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/midinote.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.852556 isobar_ext-0.5.1/isobar_ext/io/netclock/
--rw-rw-rw-   0        0        0      112 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/netclock/__init__.py
--rw-rw-rw-   0        0        0     1782 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/netclock/receiver.py
--rw-rw-rw-   0        0        0     1032 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/netclock/sender.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.855562 isobar_ext-0.5.1/isobar_ext/io/netglobals/
--rw-rw-rw-   0        0        0      116 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/netglobals/__init__.py
--rw-rw-rw-   0        0        0     1433 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/netglobals/receiver.py
--rw-rw-rw-   0        0        0     1271 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/netglobals/sender.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.856562 isobar_ext-0.5.1/isobar_ext/io/osc/
--rw-rw-rw-   0        0        0       70 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/osc/__init__.py
--rw-rw-rw-   0        0        0     1249 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/osc/output.py
--rw-rw-rw-   0        0        0      770 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/output.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.857610 isobar_ext-0.5.1/isobar_ext/io/signalflow/
--rw-rw-rw-   0        0        0       84 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/signalflow/__init__.py
--rw-rw-rw-   0        0        0     2278 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/signalflow/output.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.859610 isobar_ext-0.5.1/isobar_ext/io/socketio/
--rw-rw-rw-   0        0        0       80 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/socketio/__init__.py
--rw-rw-rw-   0        0        0     1076 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/socketio/output.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.860568 isobar_ext-0.5.1/isobar_ext/io/supercollider/
--rw-rw-rw-   0        0        0       90 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/supercollider/__init__.py
--rw-rw-rw-   0        0        0     1454 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/io/supercollider/output.py
--rw-rw-rw-   0        0        0     7852 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/key.py
--rw-rw-rw-   0        0        0      539 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/note.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.870562 isobar_ext-0.5.1/isobar_ext/pattern/
--rw-rw-rw-   0        0        0      592 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/__init__.py
--rw-rw-rw-   0        0        0    20774 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/chance.py
--rw-rw-rw-   0        0        0    22106 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/core.py
--rw-rw-rw-   0        0        0     6139 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/fade.py
--rw-rw-rw-   0        0        0     2317 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/lsystem.py
--rw-rw-rw-   0        0        0     7935 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/markov.py
--rw-rw-rw-   0        0        0     2157 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/midi.py
--rw-rw-rw-   0        0        0     1906 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/oscillator.py
--rw-rw-rw-   0        0        0     9666 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/scalar.py
--rw-rw-rw-   0        0        0    40414 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/sequence.py
--rw-rw-rw-   0        0        0     4118 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/static.py
--rw-rw-rw-   0        0        0     4136 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/tonal.py
--rw-rw-rw-   0        0        0     3995 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/pattern/warp.py
--rw-rw-rw-   0        0        0     7622 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/scale.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.874802 isobar_ext-0.5.1/isobar_ext/shorthand/
--rw-rw-rw-   0        0        0      342 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/shorthand/__init__.py
--rw-rw-rw-   0        0        0     5918 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/shorthand/abbreviations.py
--rw-rw-rw-   0        0        0     2471 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/shorthand/notation.py
--rw-rw-rw-   0        0        0     1404 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/shorthand/patches.py
--rw-rw-rw-   0        0        0     2568 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/shorthand/setup.py
--rw-rw-rw-   0        0        0      753 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/shorthand/sync.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.878803 isobar_ext-0.5.1/isobar_ext/timelines/
--rw-rw-rw-   0        0        0      216 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/timelines/__init__.py
--rw-rw-rw-   0        0        0     6032 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/timelines/clock.py
--rw-rw-rw-   0        0        0     3291 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/timelines/clock_link.py
--rw-rw-rw-   0        0        0    10744 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/timelines/event.py
--rw-rw-rw-   0        0        0    25826 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/timelines/timeline.py
--rw-rw-rw-   0        0        0    27346 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/timelines/track.py
--rw-rw-rw-   0        0        0     7992 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/isobar_ext/util.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.841344 isobar_ext-0.5.1/isobar_ext.egg-info/
--rw-rw-rw-   0        0        0    13441 2024-02-03 22:34:37.000000 isobar_ext-0.5.1/isobar_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2641 2024-02-03 22:34:37.000000 isobar_ext-0.5.1/isobar_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-03 22:34:37.000000 isobar_ext-0.5.1/isobar_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-02-03 22:34:37.000000 isobar_ext-0.5.1/isobar_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-02-03 22:34:37.000000 isobar_ext-0.5.1/isobar_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2024-02-03 22:34:37.896951 isobar_ext-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      906 2024-02-03 22:31:47.000000 isobar_ext-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-03 22:34:37.894951 isobar_ext-0.5.1/tests/
--rw-rw-rw-   0        0        0      242 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/__init__.py
--rw-rw-rw-   0        0        0      388 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_chord.py
--rw-rw-rw-   0        0        0     1799 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_io_midi.py
--rw-rw-rw-   0        0        0     1501 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_io_midifile.py
--rw-rw-rw-   0        0        0     2706 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_key.py
--rw-rw-rw-   0        0        0     2480 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern.py
--rw-rw-rw-   0        0        0     4631 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_chance.py
--rw-rw-rw-   0        0        0     2253 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_core.py
--rw-rw-rw-   0        0        0      253 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_lsystem.py
--rw-rw-rw-   0        0        0      418 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_markov.py
--rw-rw-rw-   0        0        0     3247 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_operators.py
--rw-rw-rw-   0        0        0     2554 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_scalar.py
--rw-rw-rw-   0        0        0     5837 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_sequence.py
--rw-rw-rw-   0        0        0     1572 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_static.py
--rw-rw-rw-   0        0        0      864 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_pattern_tonal.py
--rw-rw-rw-   0        0        0      531 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_shorthand_notation.py
--rw-rw-rw-   0        0        0    12397 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_timeline.py
--rw-rw-rw-   0        0        0     2111 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_timeline_clock.py
--rw-rw-rw-   0        0        0     7463 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_timeline_event.py
--rw-rw-rw-   0        0        0     3177 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_timeline_event_control.py
--rw-rw-rw-   0        0        0      952 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_timeline_event_supercollider.py
--rw-rw-rw-   0        0        0     2313 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_timeline_track.py
--rw-rw-rw-   0        0        0     1758 2024-02-03 21:14:19.000000 isobar_ext-0.5.1/tests/test_util.py
+-rw-r--r--   0        0        0     1907 2024-03-16 16:39:22.219516 isobar_ext-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      588 2024-04-07 17:17:41.659548 isobar_ext-0.9.0/isobar_ext/__init__.py
+-rw-r--r--   0        0        0     1683 2024-04-07 18:08:46.888561 isobar_ext-0.9.0/isobar_ext/chord.py
+-rw-r--r--   0        0        0     5174 2024-02-03 21:14:19.101336 isobar_ext-0.9.0/isobar_ext/constants.py
+-rw-r--r--   0        0        0     1185 2024-02-03 21:14:19.101336 isobar_ext-0.9.0/isobar_ext/exceptions.py
+-rw-r--r--   0        0        0     1013 2024-04-07 16:23:39.121473 isobar_ext-0.9.0/isobar_ext/io/__init__.py
+-rw-r--r--   0        0        0      116 2024-02-03 21:14:19.102352 isobar_ext-0.9.0/isobar_ext/io/cv/__init__.py
+-rw-r--r--   0        0        0     2940 2024-02-03 21:14:19.103787 isobar_ext-0.9.0/isobar_ext/io/cv/output.py
+-rw-r--r--   0        0        0       74 2024-02-03 21:14:19.103787 isobar_ext-0.9.0/isobar_ext/io/dummy/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-07 16:23:39.451331 isobar_ext-0.9.0/isobar_ext/io/dummy/output.py
+-rw-r--r--   0        0        0      774 2024-04-07 16:26:19.459909 isobar_ext-0.9.0/isobar_ext/io/midi/__init__.py
+-rw-r--r--   0        0        0     4888 2024-04-07 16:36:48.471196 isobar_ext-0.9.0/isobar_ext/io/midi/input.py
+-rw-r--r--   0        0        0     4003 2024-04-07 16:37:38.660752 isobar_ext-0.9.0/isobar_ext/io/midi/output.py
+-rw-r--r--   0        0        0      288 2024-03-16 18:10:06.535531 isobar_ext-0.9.0/isobar_ext/io/midifile/__init__.py
+-rw-r--r--   0        0        0    23116 2024-04-07 16:42:37.403590 isobar_ext-0.9.0/isobar_ext/io/midifile/input.py
+-rw-r--r--   0        0        0    13362 2024-04-07 16:56:43.886312 isobar_ext-0.9.0/isobar_ext/io/midifile/output.py
+-rw-r--r--   0        0        0    17404 2024-04-07 16:26:19.482425 isobar_ext-0.9.0/isobar_ext/io/midimessages.py
+-rw-r--r--   0        0        0     1559 2024-04-07 16:26:19.595543 isobar_ext-0.9.0/isobar_ext/io/midinote.py
+-rw-r--r--   0        0        0      112 2024-02-03 21:14:19.108167 isobar_ext-0.9.0/isobar_ext/io/netclock/__init__.py
+-rw-r--r--   0        0        0     1790 2024-04-07 16:26:19.563564 isobar_ext-0.9.0/isobar_ext/io/netclock/receiver.py
+-rw-r--r--   0        0        0     1034 2024-04-07 16:23:39.302169 isobar_ext-0.9.0/isobar_ext/io/netclock/sender.py
+-rw-r--r--   0        0        0      116 2024-02-03 21:14:19.111319 isobar_ext-0.9.0/isobar_ext/io/netglobals/__init__.py
+-rw-r--r--   0        0        0     1435 2024-04-07 16:23:39.389134 isobar_ext-0.9.0/isobar_ext/io/netglobals/receiver.py
+-rw-r--r--   0        0        0     1275 2024-04-07 16:23:39.468337 isobar_ext-0.9.0/isobar_ext/io/netglobals/sender.py
+-rw-r--r--   0        0        0       70 2024-02-03 21:14:19.112803 isobar_ext-0.9.0/isobar_ext/io/osc/__init__.py
+-rw-r--r--   0        0        0     1440 2024-04-07 16:59:29.475319 isobar_ext-0.9.0/isobar_ext/io/osc/output.py
+-rw-r--r--   0        0        0      914 2024-04-07 17:00:35.790821 isobar_ext-0.9.0/isobar_ext/io/output.py
+-rw-r--r--   0        0        0       84 2024-02-03 21:14:19.114815 isobar_ext-0.9.0/isobar_ext/io/signalflow/__init__.py
+-rw-r--r--   0        0        0     2278 2024-04-07 16:23:39.344327 isobar_ext-0.9.0/isobar_ext/io/signalflow/output.py
+-rw-r--r--   0        0        0       80 2024-02-03 21:14:19.115814 isobar_ext-0.9.0/isobar_ext/io/socketio/__init__.py
+-rw-r--r--   0        0        0     1076 2024-02-03 21:14:19.115814 isobar_ext-0.9.0/isobar_ext/io/socketio/output.py
+-rw-r--r--   0        0        0       90 2024-02-03 21:14:19.116814 isobar_ext-0.9.0/isobar_ext/io/supercollider/__init__.py
+-rw-r--r--   0        0        0     1454 2024-04-07 16:23:39.140895 isobar_ext-0.9.0/isobar_ext/io/supercollider/output.py
+-rw-r--r--   0        0        0     7840 2024-04-07 18:10:18.806665 isobar_ext-0.9.0/isobar_ext/key.py
+-rw-r--r--   0        0        0       38 2024-04-07 16:26:19.413878 isobar_ext-0.9.0/isobar_ext/notation/__init__.py
+-rw-r--r--   0        0        0     2434 2024-04-07 17:06:35.088895 isobar_ext-0.9.0/isobar_ext/notation/notation.py
+-rw-r--r--   0        0        0      569 2024-04-07 18:12:15.445044 isobar_ext-0.9.0/isobar_ext/note.py
+-rw-r--r--   0        0        0      592 2024-04-07 16:23:39.410584 isobar_ext-0.9.0/isobar_ext/pattern/__init__.py
+-rw-r--r--   0        0        0    20163 2024-04-07 17:42:51.820318 isobar_ext-0.9.0/isobar_ext/pattern/chance.py
+-rw-r--r--   0        0        0    23356 2024-04-07 16:26:19.505789 isobar_ext-0.9.0/isobar_ext/pattern/core.py
+-rw-r--r--   0        0        0     6143 2024-04-07 16:23:39.173671 isobar_ext-0.9.0/isobar_ext/pattern/fade.py
+-rw-r--r--   0        0        0     2321 2024-04-07 16:23:39.440711 isobar_ext-0.9.0/isobar_ext/pattern/lsystem.py
+-rw-r--r--   0        0        0     7937 2024-04-07 16:23:39.336698 isobar_ext-0.9.0/isobar_ext/pattern/markov.py
+-rw-r--r--   0        0        0     2163 2024-04-07 16:26:19.571353 isobar_ext-0.9.0/isobar_ext/pattern/midi.py
+-rw-r--r--   0        0        0     1908 2024-04-07 16:23:39.182226 isobar_ext-0.9.0/isobar_ext/pattern/oscillator.py
+-rw-r--r--   0        0        0     9657 2024-04-07 17:42:51.821322 isobar_ext-0.9.0/isobar_ext/pattern/scalar.py
+-rw-r--r--   0        0        0    38364 2024-04-07 18:17:33.310983 isobar_ext-0.9.0/isobar_ext/pattern/sequence.py
+-rw-r--r--   0        0        0     1126 2024-04-07 18:17:33.335696 isobar_ext-0.9.0/isobar_ext/pattern/series.py
+-rw-r--r--   0        0        0     3718 2024-04-07 17:35:09.888006 isobar_ext-0.9.0/isobar_ext/pattern/static.py
+-rw-r--r--   0        0        0     4122 2024-04-07 17:48:33.537064 isobar_ext-0.9.0/isobar_ext/pattern/tonal.py
+-rw-r--r--   0        0        0     4022 2024-04-07 18:17:33.295837 isobar_ext-0.9.0/isobar_ext/pattern/warp.py
+-rw-r--r--   0        0        0     7591 2024-04-07 18:14:34.259628 isobar_ext-0.9.0/isobar_ext/scale.py
+-rw-r--r--   0        0        0    13073 2024-04-07 16:26:19.472638 isobar_ext-0.9.0/isobar_ext/scales.json
+-rw-r--r--   0        0        0      342 2024-04-07 16:23:39.427968 isobar_ext-0.9.0/isobar_ext/shorthand/__init__.py
+-rw-r--r--   0        0        0     5862 2024-04-07 18:17:33.274178 isobar_ext-0.9.0/isobar_ext/shorthand/abbreviations.py
+-rw-r--r--   0        0        0     1450 2024-04-07 18:17:33.304410 isobar_ext-0.9.0/isobar_ext/shorthand/patches.py
+-rw-r--r--   0        0        0     3163 2024-04-07 16:26:19.600320 isobar_ext-0.9.0/isobar_ext/shorthand/setup.py
+-rw-r--r--   0        0        0      755 2024-04-07 16:23:39.076742 isobar_ext-0.9.0/isobar_ext/shorthand/sync.py
+-rw-r--r--   0        0        0      216 2024-04-07 16:23:39.135584 isobar_ext-0.9.0/isobar_ext/timelines/__init__.py
+-rw-r--r--   0        0        0     6048 2024-04-07 16:26:19.617816 isobar_ext-0.9.0/isobar_ext/timelines/clock.py
+-rw-r--r--   0        0        0     3307 2024-04-07 17:54:07.927014 isobar_ext-0.9.0/isobar_ext/timelines/clock_link.py
+-rw-r--r--   0        0        0    10766 2024-04-07 17:58:09.038529 isobar_ext-0.9.0/isobar_ext/timelines/event.py
+-rw-r--r--   0        0        0    30453 2024-04-07 17:58:09.049053 isobar_ext-0.9.0/isobar_ext/timelines/timeline.py
+-rw-r--r--   0        0        0    39776 2024-04-07 18:17:33.281191 isobar_ext-0.9.0/isobar_ext/timelines/track.py
+-rw-r--r--   0        0        0     7967 2024-04-07 18:16:20.273303 isobar_ext-0.9.0/isobar_ext/util.py
+-rw-r--r--   0        0        0     1184 2024-02-03 21:06:21.964400 isobar_ext-0.9.0/LICENSE.md
+-rw-r--r--   0        0        0      897 2024-04-07 18:49:27.377156 isobar_ext-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    12953 2024-04-07 17:42:51.818949 isobar_ext-0.9.0/README.md
+-rw-r--r--   0        0        0    13817 1970-01-01 00:00:00.000000 isobar_ext-0.9.0/PKG-INFO
```

### Comparing `isobar_ext-0.5.1/LICENSE.md` & `isobar_ext-0.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `isobar_ext-0.5.1/PKG-INFO` & `isobar_ext-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: isobar_ext
-Version: 0.5.1
-Summary: A Python library to express and manipulate musical patterns extending original isobar library.
-Home-page: https://github.com/piotereks/isobar-ext
-Author: Piotr Sakowski
-Author-email: piotereks@gmail.com
-Keywords: sound,music,composition
-Classifier: Topic :: Multimedia :: Sound/Audio
-Classifier: Topic :: Artistic Software
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # isobar-ext
    <span class="text-small lh-condensed-ultra no-wrap mt-1" data-repository-hovercards-enabled="">
       forked from <a data-hovercard-type="repository" data-hovercard-url="/piotereks/isobar-ext/hovercard" class="Link--inTextBlock" href="https://github.com/ideoforms/isobar">ideoforms/isobar</a>
     </span>
 
 ![ci](https://github.com/piotereks/isobar-ext/workflows/ci/badge.svg) [![stability-mature](https://img.shields.io/badge/stability-mature-008000.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#mature)
 
@@ -25,51 +10,52 @@
 The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://piotereks.github.io/isobar-ext/#flow-diagram).)
 
 isobar-ext includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
 
 ## Usage
 
 ```python
+import isobar_ext.pattern.series
 import isobar_ext as iso
 
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # Create a geometric series on a minor scale.
 # PingPong plays the series forward then backward. PLoop loops forever.
-#------------------------------------------------------------------------
-arpeggio = iso.PSeries(0, 2, 6)
+# ------------------------------------------------------------------------
+arpeggio = isobar_ext.pattern.series.PSeries(0, 2, 6)
 arpeggio = iso.PDegree(arpeggio, iso.Scale.minor) + 72
 arpeggio = iso.PPingPong(arpeggio)
 arpeggio = iso.PLoop(arpeggio)
 
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # Create a velocity sequence, with emphasis every 4th note,
 # plus a random walk to create gradual dynamic changes.
 # Amplitudes are in the MIDI velocity range (0..127).
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 amplitude = iso.PSequence([50, 35, 25, 35]) + iso.PBrown(0, 1, -20, 20)
 
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # A Timeline schedules events at a specified tempo. By default, events
 # are send to the system's default MIDI output.
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 timeline = iso.Timeline(120)
 
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # Schedule events, with properties generated by the Pattern objects.
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 timeline.schedule({
     "note": arpeggio,
     "duration": 0.25,
     "amplitude": amplitude
 })
 
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 # Run the timeline.
 # Call timeline.background() to run in a separate thread.
-#------------------------------------------------------------------------
+# ------------------------------------------------------------------------
 timeline.run()
 ```
 
 ## Installation
 
 The short answer: `pip3 install isobar-ext` (not yet on PyPl)
```

### Comparing `isobar_ext-0.5.1/README.md` & `isobar_ext-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,203 +1,232 @@
-# isobar-ext
-   <span class="text-small lh-condensed-ultra no-wrap mt-1" data-repository-hovercards-enabled="">
-      forked from <a data-hovercard-type="repository" data-hovercard-url="/piotereks/isobar-ext/hovercard" class="Link--inTextBlock" href="https://github.com/ideoforms/isobar">ideoforms/isobar</a>
-    </span>
-
-![ci](https://github.com/piotereks/isobar-ext/workflows/ci/badge.svg) [![stability-mature](https://img.shields.io/badge/stability-mature-008000.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#mature)
-
-isobar-ext is a Python library for creating and manipulating musical patterns, designed for use in algorithmic composition, generative music and sonification. It makes it quick and easy to express complex musical ideas, and can send and receive events from various different sources including MIDI, MIDI files, and OSC.
-
-The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://piotereks.github.io/isobar-ext/#flow-diagram).)
-
-isobar-ext includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
-
-## Usage
-
-```python
-import isobar_ext as iso
-
-#------------------------------------------------------------------------
-# Create a geometric series on a minor scale.
-# PingPong plays the series forward then backward. PLoop loops forever.
-#------------------------------------------------------------------------
-arpeggio = iso.PSeries(0, 2, 6)
-arpeggio = iso.PDegree(arpeggio, iso.Scale.minor) + 72
-arpeggio = iso.PPingPong(arpeggio)
-arpeggio = iso.PLoop(arpeggio)
-
-#------------------------------------------------------------------------
-# Create a velocity sequence, with emphasis every 4th note,
-# plus a random walk to create gradual dynamic changes.
-# Amplitudes are in the MIDI velocity range (0..127).
-#------------------------------------------------------------------------
-amplitude = iso.PSequence([50, 35, 25, 35]) + iso.PBrown(0, 1, -20, 20)
-
-#------------------------------------------------------------------------
-# A Timeline schedules events at a specified tempo. By default, events
-# are send to the system's default MIDI output.
-#------------------------------------------------------------------------
-timeline = iso.Timeline(120)
-
-#------------------------------------------------------------------------
-# Schedule events, with properties generated by the Pattern objects.
-#------------------------------------------------------------------------
-timeline.schedule({
-    "note": arpeggio,
-    "duration": 0.25,
-    "amplitude": amplitude
-})
-
-#------------------------------------------------------------------------
-# Run the timeline.
-# Call timeline.background() to run in a separate thread.
-#------------------------------------------------------------------------
-timeline.run()
-```
-
-## Installation
-
-The short answer: `pip3 install isobar-ext` (not yet on PyPl)
-
-The long answer: [isobar-ext Getting Started guide](http://piotereks.github.io/isobar-ext/getting-started/)
-
-## Documentation
-
-For complete documentation, see [piotereks.github.io/isobar-ext](http://piotereks.github.io/isobar-ext/).
-
-## Examples
-
-Examples are available in the [examples](examples) directory with this
-distribution:
-
-* [00.ex-hello-world.py](examples/00.ex-hello-world.py)
-* [01.ex-basics.py](examples/01.ex-basics.py)
-* [02.ex-subsequence.py](examples/02.ex-subsequence.py)
-* [03.ex-euclidean.py](examples/03.ex-euclidean.py)
-* [04.ex-permutations.py](examples/04.ex-permutations.py)
-* [05.ex-piano-phase.py](examples/05.ex-piano-phase.py)
-* [06.ex-walk.py](examples/06.ex-walk.py)
-* [07.ex-static-pattern.py](examples/07.ex-static-pattern.py)
-* [10.ex-lsystem-stochastic.py](examples/10.ex-lsystem-stochastic.py)
-* [11.ex-lsystem-rhythm.py](examples/11.ex-lsystem-rhythm.py)
-* [12.ex-lsystem-grapher.py](examples/12.ex-lsystem-grapher.py)
-* [20.ex-midi-input.py](examples/20.ex-midi-input.py)
-* [21.ex-midi-clock-sync-in.py](examples/21.ex-midi-clock-sync-in.py)
-* [22.ex-midi-markov-learner.py](examples/22.ex-midi-markov-learner.py)
-* [23.ex-midi-monitor.py](examples/23.ex-midi-monitor.py)
-* [30.ex-midifile-read.py](examples/30.ex-midifile-read.py)
-* [31.ex-midifile-write.py](examples/31.ex-midifile-write.py)
-* [32.ex-midifile-markov.py](examples/32.ex-midifile-markov.py)
-* [40.ex-osc-send.py](examples/40.ex-osc-send.py)
-
-### Pattern classes
-
-    CORE (core.py)
-    Pattern                  - Abstract superclass of all pattern generators.
-    PConstant                - Returns a fixed value.
-    PRef                     - Contains a reference to another pattern, which can be replaced dynamically.
-    PFunc                    - Returns the value generated by a function.
-    PArrayIndex              - Request a specified index from an array.
-    PDict                    - Construct a pattern from a dict of arrays, or an array of dicts.
-    PDictKey                 - Request a specified key from a dictionary.
-    PConcatenate             - Concatenate the output of multiple sequences.
-    PAbs                     - Absolute value of `input`
-    PInt                     - Integer value of `input`
-    PAdd                     - Add elements of two patterns (shorthand: patternA + patternB)
-    PSub                     - Subtract elements of two patterns (shorthand: patternA - patternB)
-    PMul                     - Multiply elements of two patterns (shorthand: patternA * patternB)
-    PDiv                     - Divide elements of two patterns (shorthand: patternA / patternB)
-    PFloorDiv                - Integer division (shorthand: patternA // patternB)
-    PMod                     - Modulo elements of two patterns (shorthand: patternA % patternB)
-    PPow                     - One pattern to the power of another (shorthand: patternA ** patternB)
-    PLShift                  - Binary left-shift (shorthand: patternA << patternB)
-    PRShift                  - Binary right-shift (shorthand: patternA << patternB)
-    PEqual                   - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
-    PGreaterThanOrEqual      - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
-    PGreaterThan             - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
-    PGreaterThanOrEqual      - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
-    PLessThan                - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
-    PLessThanOrEqual         - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
-
-    SCALAR (scalar.py)
-    PChanged                 - Outputs a 1 if the value of the input pattern has changed,
-    PDiff                    - Outputs the difference between the current and previous values of an input pattern
-    PSkipIf                  - If `skip` is false, returns `input`; otherwise, returns None.
-    PNormalise               - Adaptively normalise `input` to [0..1] over a linear scale.
-    PMap                     - Apply an arbitrary function to an input pattern.
-    PMapEnumerated           - Apply arbitrary function to input, passing a counter.
-    PScaleLinLin             - Map `input` from linear range [a,b] to linear range [c,d].
-    PScaleLinExp             - Map `input` from linear range [a,b] to exponential range [c,d].
-    PRound                   - Round `input` to N decimal places.
-    PScalar                  - Reduce tuples and lists into single scalar values,
-    PWrap                    - Wrap input note values within <min>, <max>.
-    PIndexOf                 - Find index of items from `pattern` in <list>
-
-    SEQUENCE (sequence.py)
-    PSeries                  - Arithmetic series, beginning at `start`, increment by `step`
-    PRange                   - Similar to PSeries, but specify a max/step value.
-    PGeom                    - Geometric series, beginning at `start`, multiplied by `step`
-    PImpulse                 - Outputs a 1 every <period> events, otherwise 0.
-    PLoop                    - Repeats a finite `pattern` for `n` repeats.
-    PPingPong                - Ping-pong input pattern back and forth N times.
-    PCreep                   - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
-    PStutter                 - Play each note of `pattern` `count` times.
-    PSubsequence             - Returns a finite subsequence of an input pattern.
-    PReverse                 - Reverses a finite sequence.
-    PReset                   - Resets `pattern` whenever `trigger` is true
-    PCounter                 - Increments a counter by 1 for each zero-crossing in `trigger`.
-    PCollapse                - Skip over any rests in `input`
-    PNoRepeats               - Skip over repeated values in `input`
-    PPad                     - Pad `pattern` with rests until it reaches length `length`.
-    PPadToMultiple           - Pad `pattern` with rests until its length is divisible by `multiple`.
-    PArpeggiator             - Arpeggiator.
-    PEuclidean               - Generate Euclidean rhythms.
-    PPermut                  - Generate every permutation of `count` input items.
-    PPatternGeneratorAction  - Each time its pattern is exhausted, request a new pattern by calling <fn>.
-    PSequenceAction          - Iterate over an array, perform a function, and repeat.
-
-    CHANCE (chance.py)
-    PWhite                   - White noise between `min` and `max`.
-    PBrown                   - Brownian noise.
-    PCoin                    - Coin toss, returning either 0 or 1 given some `probability`.
-    PWalk                    - Random walk around list.
-    PChoice                  - Pick a random element from `values`, weighted by optional `weights`.
-    PSample                  - Pick multiple random elements from `values`, weighted by optional `weights`,
-    PShuffle                 - Shuffled list.
-    PShuffleInput            - Every `n` steps, take `n` values from `pattern` and reorder.
-    PSkip                    - Skip events with some probability, 1 - `play`.
-    PFlipFlop                - flip a binary bit with some probability.
-    PSwitchOne               - Capture `length` input values; loop, repeatedly switching two adjacent values.
-    PRandomExponential       - Random uniform on exponential curve between `min` and `max`,
-    PRandomImpulseSequence   - Random sequence of impulses with probability `probability`.
-
-    TONAL (tonal.py)
-    PDegree                  - Map scale index <degree> to MIDI notes in <scale>.
-    PFilterByKey             - Filter notes based on their presence in <key>.
-    PNearestNoteInKey        - Return the nearest note in <key>.
-    PMidiNoteToFrequency     - Map MIDI note to frequency value.
-
-    STATIC (static.py)
-    PGlobals                 - Static global value identified by a string.
-    PCurrentTime             - Returns the position (in beats) of the current timeline.
-
-    FADE (fade.py)
-    PFadeNotewise            - Fade a pattern in/out by introducing notes at a gradual rate.
-    PFadeNotewiseRandom      - Fade a pattern in/out by gradually introducing random notes.
-
-    MARKOV (markov.py)
-    PMarkov                  - First-order Markov chain generator.
-
-    LSYSTEM (lsystem.py)
-    PLSystem                 - integer sequence derived from Lindenmayer systems
-
-    WARP (warp.py)
-    PWInterpolate            - Requests a new target warp value from `pattern` every `length` beats
-    PWSine                   - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
-    PWRallantando            - Exponential deceleration to <amp> times the current tempo over `length` beats.
-
-## Background
-
-isobar was first designed for the generative sound installation [Variable 4](http://www.variable4.org.uk), in which it was used to generate musical structures in response to changing weather conditions. It was more recently used in [The Listening Machine](http://www.thelisteningmachine.org/), taking live input from Twitter and generating musical output from language patterns, streamed live over the internet.
-
-Many of the concepts behind Pattern and its subclasses are inspired by the brilliant pattern library of the [SuperCollider](http://supercollider.sf.net) synthesis language.
-
+Metadata-Version: 2.1
+Name: isobar_ext
+Version: 0.9.0
+Summary: A Python library to express and manipulate musical patterns extending the original isobar library.
+Home-page: https://github.com/piotereks/isobar-ext
+License: MIT
+Keywords: sound,music,composition
+Author: Piotr Sakowski
+Author-email: piotereks@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Artistic Software
+Classifier: Topic :: Multimedia :: Sound/Audio
+Requires-Dist: mido
+Requires-Dist: python-osc
+Requires-Dist: python-rtmidi
+Project-URL: Documentation, http://piotereks.github.io/isobar-ext
+Project-URL: Repository, https://github.com/piotereks/isobar-ext
+Description-Content-Type: text/markdown
+
+# isobar-ext
+   <span class="text-small lh-condensed-ultra no-wrap mt-1" data-repository-hovercards-enabled="">
+      forked from <a data-hovercard-type="repository" data-hovercard-url="/piotereks/isobar-ext/hovercard" class="Link--inTextBlock" href="https://github.com/ideoforms/isobar">ideoforms/isobar</a>
+    </span>
+
+![ci](https://github.com/piotereks/isobar-ext/workflows/ci/badge.svg) [![stability-mature](https://img.shields.io/badge/stability-mature-008000.svg)](https://github.com/mkenney/software-guides/blob/master/STABILITY-BADGES.md#mature)
+
+isobar-ext is a Python library for creating and manipulating musical patterns, designed for use in algorithmic composition, generative music and sonification. It makes it quick and easy to express complex musical ideas, and can send and receive events from various different sources including MIDI, MIDI files, and OSC.
+
+The core element is a Timeline, which can control its own tempo or sync to an external clock. Onto this, you can schedule Patterns, which can be note sequences, control events, program changes, or other arbitrary events via lambda functions. Pattern are used as templates to generate Events, which trigger notes or control changes on an OutputDevice (Check out a [diagrammatic overview](http://piotereks.github.io/isobar-ext/#flow-diagram).)
+
+isobar-ext includes a large array of basic compositional building blocks (see [Pattern Classes](#pattern-classes)), plus some advanced pattern generators for more sophisticated operations (arpeggiators, Euclidean rhythms, L-systems, Markov chains).
+
+## Usage
+
+```python
+import isobar_ext.pattern.series
+import isobar_ext as iso
+
+# ------------------------------------------------------------------------
+# Create a geometric series on a minor scale.
+# PingPong plays the series forward then backward. PLoop loops forever.
+# ------------------------------------------------------------------------
+arpeggio = isobar_ext.pattern.series.PSeries(0, 2, 6)
+arpeggio = iso.PDegree(arpeggio, iso.Scale.minor) + 72
+arpeggio = iso.PPingPong(arpeggio)
+arpeggio = iso.PLoop(arpeggio)
+
+# ------------------------------------------------------------------------
+# Create a velocity sequence, with emphasis every 4th note,
+# plus a random walk to create gradual dynamic changes.
+# Amplitudes are in the MIDI velocity range (0..127).
+# ------------------------------------------------------------------------
+amplitude = iso.PSequence([50, 35, 25, 35]) + iso.PBrown(0, 1, -20, 20)
+
+# ------------------------------------------------------------------------
+# A Timeline schedules events at a specified tempo. By default, events
+# are send to the system's default MIDI output.
+# ------------------------------------------------------------------------
+timeline = iso.Timeline(120)
+
+# ------------------------------------------------------------------------
+# Schedule events, with properties generated by the Pattern objects.
+# ------------------------------------------------------------------------
+timeline.schedule({
+    "note": arpeggio,
+    "duration": 0.25,
+    "amplitude": amplitude
+})
+
+# ------------------------------------------------------------------------
+# Run the timeline.
+# Call timeline.background() to run in a separate thread.
+# ------------------------------------------------------------------------
+timeline.run()
+```
+
+## Installation
+
+The short answer: `pip3 install isobar-ext` (not yet on PyPl)
+
+The long answer: [isobar-ext Getting Started guide](http://piotereks.github.io/isobar-ext/getting-started/)
+
+## Documentation
+
+For complete documentation, see [piotereks.github.io/isobar-ext](http://piotereks.github.io/isobar-ext/).
+
+## Examples
+
+Examples are available in the [examples](examples) directory with this
+distribution:
+
+* [00.ex-hello-world.py](examples/00.ex-hello-world.py)
+* [01.ex-basics.py](examples/01.ex-basics.py)
+* [02.ex-subsequence.py](examples/02.ex-subsequence.py)
+* [03.ex-euclidean.py](examples/03.ex-euclidean.py)
+* [04.ex-permutations.py](examples/04.ex-permutations.py)
+* [05.ex-piano-phase.py](examples/05.ex-piano-phase.py)
+* [06.ex-walk.py](examples/06.ex-walk.py)
+* [07.ex-static-pattern.py](examples/07.ex-static-pattern.py)
+* [10.ex-lsystem-stochastic.py](examples/10.ex-lsystem-stochastic.py)
+* [11.ex-lsystem-rhythm.py](examples/11.ex-lsystem-rhythm.py)
+* [12.ex-lsystem-grapher.py](examples/12.ex-lsystem-grapher.py)
+* [20.ex-midi-input.py](examples/20.ex-midi-input.py)
+* [21.ex-midi-clock-sync-in.py](examples/21.ex-midi-clock-sync-in.py)
+* [22.ex-midi-markov-learner.py](examples/22.ex-midi-markov-learner.py)
+* [23.ex-midi-monitor.py](examples/23.ex-midi-monitor.py)
+* [30.ex-midifile-read.py](examples/30.ex-midifile-read.py)
+* [31.ex-midifile-write.py](examples/31.ex-midifile-write.py)
+* [32.ex-midifile-markov.py](examples/32.ex-midifile-markov.py)
+* [40.ex-osc-send.py](examples/40.ex-osc-send.py)
+
+### Pattern classes
+
+    CORE (core.py)
+    Pattern                  - Abstract superclass of all pattern generators.
+    PConstant                - Returns a fixed value.
+    PRef                     - Contains a reference to another pattern, which can be replaced dynamically.
+    PFunc                    - Returns the value generated by a function.
+    PArrayIndex              - Request a specified index from an array.
+    PDict                    - Construct a pattern from a dict of arrays, or an array of dicts.
+    PDictKey                 - Request a specified key from a dictionary.
+    PConcatenate             - Concatenate the output of multiple sequences.
+    PAbs                     - Absolute value of `input`
+    PInt                     - Integer value of `input`
+    PAdd                     - Add elements of two patterns (shorthand: patternA + patternB)
+    PSub                     - Subtract elements of two patterns (shorthand: patternA - patternB)
+    PMul                     - Multiply elements of two patterns (shorthand: patternA * patternB)
+    PDiv                     - Divide elements of two patterns (shorthand: patternA / patternB)
+    PFloorDiv                - Integer division (shorthand: patternA // patternB)
+    PMod                     - Modulo elements of two patterns (shorthand: patternA % patternB)
+    PPow                     - One pattern to the power of another (shorthand: patternA ** patternB)
+    PLShift                  - Binary left-shift (shorthand: patternA << patternB)
+    PRShift                  - Binary right-shift (shorthand: patternA << patternB)
+    PEqual                   - Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)
+    PGreaterThanOrEqual      - Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)
+    PGreaterThan             - Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)
+    PGreaterThanOrEqual      - Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)
+    PLessThan                - Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)
+    PLessThanOrEqual         - Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)
+
+    SCALAR (scalar.py)
+    PChanged                 - Outputs a 1 if the value of the input pattern has changed,
+    PDiff                    - Outputs the difference between the current and previous values of an input pattern
+    PSkipIf                  - If `skip` is false, returns `input`; otherwise, returns None.
+    PNormalise               - Adaptively normalise `input` to [0..1] over a linear scale.
+    PMap                     - Apply an arbitrary function to an input pattern.
+    PMapEnumerated           - Apply arbitrary function to input, passing a counter.
+    PScaleLinLin             - Map `input` from linear range [a,b] to linear range [c,d].
+    PScaleLinExp             - Map `input` from linear range [a,b] to exponential range [c,d].
+    PRound                   - Round `input` to N decimal places.
+    PScalar                  - Reduce tuples and lists into single scalar values,
+    PWrap                    - Wrap input note values within <min>, <max>.
+    PIndexOf                 - Find index of items from `pattern` in <list>
+
+    SEQUENCE (sequence.py)
+    PSeries                  - Arithmetic series, beginning at `start`, increment by `step`
+    PRange                   - Similar to PSeries, but specify a max/step value.
+    PGeom                    - Geometric series, beginning at `start`, multiplied by `step`
+    PImpulse                 - Outputs a 1 every <period> events, otherwise 0.
+    PLoop                    - Repeats a finite `pattern` for `n` repeats.
+    PPingPong                - Ping-pong input pattern back and forth N times.
+    PCreep                   - Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
+    PStutter                 - Play each note of `pattern` `count` times.
+    PSubsequence             - Returns a finite subsequence of an input pattern.
+    PReverse                 - Reverses a finite sequence.
+    PReset                   - Resets `pattern` whenever `trigger` is true
+    PCounter                 - Increments a counter by 1 for each zero-crossing in `trigger`.
+    PCollapse                - Skip over any rests in `input`
+    PNoRepeats               - Skip over repeated values in `input`
+    PPad                     - Pad `pattern` with rests until it reaches length `length`.
+    PPadToMultiple           - Pad `pattern` with rests until its length is divisible by `multiple`.
+    PArpeggiator             - Arpeggiator.
+    PEuclidean               - Generate Euclidean rhythms.
+    PPermut                  - Generate every permutation of `count` input items.
+    PPatternGeneratorAction  - Each time its pattern is exhausted, request a new pattern by calling <fn>.
+    PSequenceAction          - Iterate over an array, perform a function, and repeat.
+
+    CHANCE (chance.py)
+    PWhite                   - White noise between `min` and `max`.
+    PBrown                   - Brownian noise.
+    PCoin                    - Coin toss, returning either 0 or 1 given some `probability`.
+    PWalk                    - Random walk around list.
+    PChoice                  - Pick a random element from `values`, weighted by optional `weights`.
+    PSample                  - Pick multiple random elements from `values`, weighted by optional `weights`,
+    PShuffle                 - Shuffled list.
+    PShuffleInput            - Every `n` steps, take `n` values from `pattern` and reorder.
+    PSkip                    - Skip events with some probability, 1 - `play`.
+    PFlipFlop                - flip a binary bit with some probability.
+    PSwitchOne               - Capture `length` input values; loop, repeatedly switching two adjacent values.
+    PRandomExponential       - Random uniform on exponential curve between `min` and `max`,
+    PRandomImpulseSequence   - Random sequence of impulses with probability `probability`.
+
+    TONAL (tonal.py)
+    PDegree                  - Map scale index <degree> to MIDI notes in <scale>.
+    PFilterByKey             - Filter notes based on their presence in <key>.
+    PNearestNoteInKey        - Return the nearest note in <key>.
+    PMidiNoteToFrequency     - Map MIDI note to frequency value.
+
+    STATIC (static.py)
+    PGlobals                 - Static global value identified by a string.
+    PCurrentTime             - Returns the position (in beats) of the current timeline.
+
+    FADE (fade.py)
+    PFadeNotewise            - Fade a pattern in/out by introducing notes at a gradual rate.
+    PFadeNotewiseRandom      - Fade a pattern in/out by gradually introducing random notes.
+
+    MARKOV (markov.py)
+    PMarkov                  - First-order Markov chain generator.
+
+    LSYSTEM (lsystem.py)
+    PLSystem                 - integer sequence derived from Lindenmayer systems
+
+    WARP (warp.py)
+    PWInterpolate            - Requests a new target warp value from `pattern` every `length` beats
+    PWSine                   - Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
+    PWRallantando            - Exponential deceleration to <amp> times the current tempo over `length` beats.
+
+## Background
+
+isobar was first designed for the generative sound installation [Variable 4](http://www.variable4.org.uk), in which it was used to generate musical structures in response to changing weather conditions. It was more recently used in [The Listening Machine](http://www.thelisteningmachine.org/), taking live input from Twitter and generating musical output from language patterns, streamed live over the internet.
+
+Many of the concepts behind Pattern and its subclasses are inspired by the brilliant pattern library of the [SuperCollider](http://supercollider.sf.net) synthesis language.
+
+
```

### Comparing `isobar_ext-0.5.1/isobar_ext/__init__.py` & `isobar_ext-0.9.0/isobar_ext/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,28 +4,29 @@
 
 A Python library for algorithmic composition by expressing and constructing musical patterns.
 
 For documentation, please see:
 
     https://github.com/piotereks/isobar-ext
 
+
 For a full list of all Pattern classes:
 
     pydoc3 isobar_ext.pattern
 
 """
 
 # flake8: noqa
 
 __version__ = "0"
-__author__ = "Daniel Jones <http://www.erase.net/>"
+__author__ = "Piotr Sakowski"
 
-from .note import *
-from .scale import *
 from .chord import *
-from .key import *
-from .util import *
-from .timelines import *
-from .pattern import *
 from .constants import *
 from .exceptions import *
 from .io import *
+from .key import *
+from .note import *
+from .pattern import *
+from .scale import *
+from .timelines import *
+from .util import *
```

### Comparing `isobar_ext-0.5.1/isobar_ext/chord.py` & `isobar_ext-0.9.0/isobar_ext/chord.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-import random
 import copy
+import random
 
 
 class Chord:
     """Represents a chord made up of 1 or more note intervals."""
 
     dict = {}
 
-    def __init__(self, intervals=[], root=0, name="unnamed chord"):
+    def __init__(self, intervals=None, root=0, name="unnamed chord"):
+        if intervals is None:
+            intervals = []
         self.intervals = intervals
         self.name = name
         self.root = root
         if name not in Chord.dict:
             Chord.dict[name] = self
 
     def __str__(self):
-        return "%s [%s]" % (self.name, ",".join(str(n) for n in self.semitones))
+        return f'{self.name} [{",".join(str(n) for n in self.semitones)}]'
 
     @property
     def semitones(self):
-        semitones = [self.root] + [
-            sum(self.intervals[0: n + 1], self.root)
+        return [self.root] + [
+            sum(self.intervals[: n + 1], self.root)
             for n in range(len(self.intervals))
         ]
-        return semitones
 
     @staticmethod
     def byname(name):
         return Chord.dict[name]
 
     @staticmethod
     def random():
```

### Comparing `isobar_ext-0.5.1/isobar_ext/constants.py` & `isobar_ext-0.9.0/isobar_ext/constants.py`

 * *Files identical despite different names*

### Comparing `isobar_ext-0.5.1/isobar_ext/exceptions.py` & `isobar_ext-0.9.0/isobar_ext/exceptions.py`

 * *Files identical despite different names*

### Comparing `isobar_ext-0.5.1/isobar_ext/io/__init__.py` & `isobar_ext-0.9.0/isobar_ext/io/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from .output import OutputDevice
+from .cv import CVOutputDevice, get_cv_output_devices
 from .dummy import DummyOutputDevice
 from .midi import (
     MidiInputDevice,
     MidiOutputDevice,
     get_midi_output_names,
     get_midi_input_names,
 )
-from .midifile import MidiFileInputDevice, MidiFileOutputDevice, PatternWriterMIDI
+from .midifile import MidiFileInputDevice, MidiFileOutputDevice, PatternWriterMIDI, FileOut
+from .midinote import MidiNote
 from .osc import OSCOutputDevice
-from .cv import CVOutputDevice, get_cv_output_devices
-from .socketio import SocketIOOutputDevice
+from .output import OutputDevice
 from .signalflow import SignalFlowOutputDevice
-from .midinote import MidiNote
+from .socketio import SocketIOOutputDevice
 from .supercollider import SuperColliderOutputDevice
 
 __all__ = ["OutputDevice", "DummyOutputDevice", "MidiInputDevice", "MidiOutputDevice"]
 __all__ += ["get_midi_output_names", "get_midi_input_names"]
-__all__ += ["MidiFileInputDevice", "MidiFileOutputDevice", "PatternWriterMIDI"]
+__all__ += ["MidiFileInputDevice", "MidiFileOutputDevice", "PatternWriterMIDI", "FileOut"]
 __all__ += [
     "OSCOutputDevice",
     "SocketIOOutputDevice",
     "SignalFlowOutputDevice",
     "MidiNote",
     "SuperColliderOutputDevice",
     "CVOutputDevice",
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/cv/output.py` & `isobar_ext-0.9.0/isobar_ext/io/cv/output.py`

 * *Files identical despite different names*

### Comparing `isobar_ext-0.5.1/isobar_ext/io/dummy/output.py` & `isobar_ext-0.9.0/isobar_ext/io/dummy/output.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from ..output import OutputDevice
 from ...constants import DEFAULT_TICKS_PER_BEAT
 
 log = logging.getLogger(__name__)
 
 
 class DummyOutputDevice(OutputDevice):
@@ -17,19 +18,19 @@
     @property
     def ticks_per_beat(self):
         return DEFAULT_TICKS_PER_BEAT
 
     def tick(self):
         self.current_time += 1.0 / self.ticks_per_beat
 
-    def note_on(self, note=60, velocity=64, channel=0):
+    def note_on(self, note=60, velocity=64, channel=0, track_idx=0):
         self.events.append(
-            [round(self.current_time, 8), "note_on", note, velocity, channel]
+            [round(self.current_time, 8), "note_on", note, velocity, channel, track_idx]
         )
 
-    def note_off(self, note=60, channel=0):
-        self.events.append([round(self.current_time, 8), "note_off", note, channel])
+    def note_off(self, note=60, channel=0, track_idx=0):
+        self.events.append([round(self.current_time, 8), "note_off", note, channel, track_idx])
 
-    def control(self, control=0, value=0, channel=0):
+    def control(self, control=0, value=0, channel=0, track_idx=0):
         self.events.append(
-            [round(self.current_time, 8), "control", control, value, channel]
+            [round(self.current_time, 8), "control", control, value, channel, track_idx]
         )
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/midi/__init__.py` & `isobar_ext-0.9.0/isobar_ext/io/midi/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+import mido
+
 from .input import MidiInputDevice
 from .output import MidiOutputDevice
 
-import mido
 
 def get_midi_output_names():
     """
     Query MIDI output device names.
 
     Returns:
         List[str]: A list of all possible MIDI output device names.
     """
     output_names = mido.get_output_names()
     return output_names
 
+
 def get_midi_input_names():
     """
     Query MIDI input device names.
 
     Returns:
         List[str]: A list of all possible MIDI input device names.
     """
     input_names = mido.get_input_names()
     return input_names
 
+
 __all__ = ["MidiInputDevice", "MidiOutputDevice", "get_midi_input_names", "get_midi_output_names"]
 
 # Class aliases for backwards-compatibility
 MidiOut = MidiOutputDevice
 MidiIn = MidiInputDevice
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/midi/input.py` & `isobar_ext-0.9.0/isobar_ext/io/midi/input.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import mido
-
+import contextlib
+import logging
 import os
-import time
 import queue
-import logging
-from ...exceptions import DeviceNotFoundException
+import time
+
+import mido
+
 from ...constants import MIDI_CLOCK_TICKS_PER_BEAT
+from ...exceptions import DeviceNotFoundException
 
 log = logging.getLogger(__name__)
 
+
 class MidiInputDevice:
     def __init__(self, device_name=None, clock_target=None, virtual=False):
         """
         Create a MIDI input device.
         Use `isobar_ext.get_midi_input_names()` to query all available devices.
 
         Args:
@@ -24,49 +27,46 @@
                                `timeline.clock_source = midi_in`.
             virtual (bool):    Whether to create a "virtual" rtmidi device.
         """
         if device_name is None:
             device_name = os.getenv("isobar_ext_DEFAULT_MIDI_IN")
         try:
             self.midi = mido.open_input(device_name, callback=self._callback, virtual=virtual)
-        except (RuntimeError, SystemError, OSError):
-            raise DeviceNotFoundException("Could not find MIDI device")
+        except (RuntimeError, SystemError, OSError) as e:
+            raise DeviceNotFoundException("Could not find MIDI device") from e
 
         self.clock_target = clock_target
         self.queue = queue.Queue()
         self.callback = None
         self.estimated_tempo = None
         self.last_clock_time = None
-        log.info("Opened MIDI input: %s" % self.midi.name)
+        log.info(f"Opened MIDI input: {self.midi.name}")
 
     @property
     def device_name(self):
         return self.midi.name
 
     def _callback(self, message):
         """
         Callback used by mido.
         Args:
             message: A mido.Message.
         """
-        log.debug(" - MIDI message received: %s" % message)
+        log.debug(f" - MIDI message received: {message}")
 
         if message.type == 'clock':
             if self.last_clock_time is not None:
                 dt = time.time() - self.last_clock_time
                 tick_estimate = (120 / 48) * 1.0 / dt
                 if self.estimated_tempo is None:
                     self.estimated_tempo = tick_estimate
                 else:
                     smoothing = 0.95
                     self.estimated_tempo = (smoothing * self.estimated_tempo) + ((1.0 - smoothing) * tick_estimate)
-                self.last_clock_time = time.time()
-            else:
-                self.last_clock_time = time.time()
-
+            self.last_clock_time = time.time()
             if self.clock_target is not None:
                 self.clock_target.tick()
 
         elif message.type == 'start':
             log.info(" - MIDI: Received start message")
             if self.clock_target is not None:
                 self.clock_target.start()
@@ -80,24 +80,25 @@
             log.info(" - MIDI: Received songpos message")
             if message.pos == 0:
                 if self.clock_target is not None:
                     self.clock_target.reset()
             else:
                 log.warning("MIDI song position message received, but MIDI input cannot seek to arbitrary position")
 
-        elif message.type in ['note_on', 'note_off', 'control_change', 'pitchwheel']:
+        elif message.type in ['note_on', 'note_off', 'control_change', 'pitchwheel', 'program_change']:
             if self.callback:
                 self.callback(message)
             else:
                 self.queue.put(message)
 
     def stop(self):
         pass
 
-    def run(self):
+    @staticmethod
+    def run():
         """
         Run indefinitely.
         """
         while True:
             time.sleep(0.1)
 
     def get_tempo(self):
@@ -131,15 +132,13 @@
         Similar to `receive`, but does not block. If an event has been received,
         it returns the mido Message immediately. Otherwise, returns None.
 
         Returns:
             Message: The event received, or None.
         """
         rv = None
-        try:
+        with contextlib.suppress(queue.Empty):
             rv = self.queue.get_nowait()
-        except queue.Empty:
-            pass
         return rv
 
     def close(self):
         del self.midi
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/midi/output.py` & `isobar_ext-0.9.0/isobar_ext/io/midi/output.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+import itertools
+import logging
 import os
+
 import mido
-import logging
+
 from ..output import OutputDevice
-from ...exceptions import DeviceNotFoundException
 from ...constants import MIDI_CLOCK_TICKS_PER_BEAT
+from ...exceptions import DeviceNotFoundException
 
 log = logging.getLogger(__name__)
 
-class MidiOutputDevice (OutputDevice):
+
+class MidiOutputDevice(OutputDevice):
     def __init__(self, device_name=None, send_clock=False, virtual=False):
         """
         Create a MIDI output device.
         Use `isobar_ext.get_midi_output_names()` to query all available devices.
 
         Args:
             device_name (str): The name of the target device to use.
@@ -21,18 +25,18 @@
             virtual (bool):    Whether to create a "virtual" rtmidi device.
         """
         super().__init__()
         try:
             if device_name is None:
                 device_name = os.getenv("isobar_ext_DEFAULT_MIDI_OUT")
             self.midi = mido.open_output(device_name, virtual=virtual)
-        except (RuntimeError, SystemError, OSError):
-            raise DeviceNotFoundException("Could not find MIDI device")
+        except (RuntimeError, SystemError, OSError) as e:
+            raise DeviceNotFoundException("Could not find MIDI device") from e
         self.send_clock = send_clock
-        log.info("Opened MIDI output: %s" % self.midi.name)
+        log.info(f"Opened MIDI output: {self.midi.name}")
 
     def start(self):
         """
         Sends a MIDI start message to the output device.
         """
         if self.send_clock:
             msg = mido.Message("start")
@@ -55,37 +59,36 @@
         return MIDI_CLOCK_TICKS_PER_BEAT
 
     def tick(self):
         if self.send_clock:
             msg = mido.Message("clock")
             self.midi.send(msg)
 
-    def note_on(self, note=60, velocity=64, channel=0):
+    def note_on(self, note=60, velocity=64, channel=0, **kwargs):
         log.debug("[midi] Note on  (channel = %d, note = %d, velocity = %d)" % (channel, note, velocity))
         msg = mido.Message('note_on', note=int(note), velocity=int(velocity), channel=int(channel))
         self.midi.send(msg)
 
-    def note_off(self, note=60, channel=0):
+    def note_off(self, note=60, channel=0, **kwargs):
         log.debug("[midi] Note off (channel = %d, note = %d)" % (channel, note))
         msg = mido.Message('note_off', note=int(note), channel=int(channel))
         self.midi.send(msg)
 
     def all_notes_off(self):
         log.debug("[midi] All notes off")
-        for channel in range(16):
-            for note in range(128):
-                msg = mido.Message('note_off', note=int(note), channel=int(channel))
-                self.midi.send(msg)
+        for channel, note in itertools.product(range(16), range(128)):
+            msg = mido.Message('note_off', note=int(note), channel=int(channel))
+            self.midi.send(msg)
 
-    def control(self, control=0, value=0, channel=0):
+    def control(self, control=0, value=0, channel=0, **kwargs):
         log.debug("[midi] Control (channel %d, control %d, value %d)" % (channel, control, value))
         msg = mido.Message('control_change', control=int(control), value=int(value), channel=int(channel))
         self.midi.send(msg)
 
-    def program_change(self, program=0, channel=0):
+    def program_change(self, program=0, channel=0, **kwargs):
         log.debug("[midi] Program change (channel %d, program_change %d)" % (channel, program))
         msg = mido.Message('program_change', program=int(program), channel=int(channel))
         self.midi.send(msg)
 
     def pitch_bend(self, pitch=0, channel=0):
         log.debug("[midi] Pitch bend (channel %d, pitch %d)" % (channel, pitch))
         msg = mido.Message('pitchwheel', pitch=int(pitch), channel=int(channel))
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/netclock/receiver.py` & `isobar_ext-0.9.0/isobar_ext/io/netclock/receiver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-from pythonosc.dispatcher import Dispatcher
-from pythonosc.osc_server import BlockingOSCUDPServer
 import threading
 import time
 
+from pythonosc.dispatcher import Dispatcher
+from pythonosc.osc_server import BlockingOSCUDPServer
+
 from ...constants import DEFAULT_TICKS_PER_BEAT
 
 
 class NetworkClockReceiver:
     """
     Naive interface to send clock signals over a network.
     Currently assumes virtually no network latency or jitter, so is only suitable
     for Ethernet connections!
 
     TODO: Implement round-trip latency estimation and jitter smoothing.
     """
 
     def __init__(
-        self, clock_target=None, port=8192, ticks_per_beat=DEFAULT_TICKS_PER_BEAT
+            self, clock_target=None, port=8192, ticks_per_beat=DEFAULT_TICKS_PER_BEAT
     ):
         self.clock_target = clock_target
 
         dispatcher = Dispatcher()
         dispatcher.map("/clock/tick", self.on_clock_tick)
         dispatcher.map("/clock/reset", self.on_clock_reset)
         dispatcher.map("/clock/sync/beat", self.on_clock_sync_beat)
@@ -51,10 +52,11 @@
 
 if __name__ == "__main__":
 
     class DummyClockTarget:
         def tick(self):
             print("tick")
 
+
     receiver = NetworkClockReceiver(clock_target=DummyClockTarget())
     while True:
         time.sleep(0.1)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/netclock/sender.py` & `isobar_ext-0.9.0/isobar_ext/io/netclock/sender.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from pythonosc.udp_client import SimpleUDPClient
 import time
 
+from pythonosc.udp_client import SimpleUDPClient
+
 
 class NetworkClockSender:
     """
     Naive interface to send clock signals over a network.
     Currently assumes virtually no network latency or jitter, so is only suitable
     for Ethernet connections!
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/netglobals/receiver.py` & `isobar_ext-0.9.0/isobar_ext/io/netglobals/receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from pythonosc.dispatcher import Dispatcher
-from pythonosc.osc_server import BlockingOSCUDPServer
-import threading
 import pickle
+import threading
 import time
 
-from isobar_ext.pattern.static import Globals
+from pythonosc.dispatcher import Dispatcher
+from pythonosc.osc_server import BlockingOSCUDPServer
+
 from isobar_ext.constants import DEFAULT_TICKS_PER_BEAT  # noqa: F401
+from isobar_ext.pattern.static import Globals
 
 
 class NetworkGlobalsReceiver:
     """
     Simple interface to receive Globals over a network.
 
     TODO: Integrate with NetworkClockReceiver
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/netglobals/sender.py` & `isobar_ext-0.9.0/isobar_ext/io/netglobals/sender.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from pythonosc.udp_client import SimpleUDPClient
-import time
 import pickle
+import time
+
+from pythonosc.udp_client import SimpleUDPClient
+
 from isobar_ext.pattern.static import Globals
 
 
 class NetworkGlobalsSender:
     """
     Simple interface to send globals over a network.
     Currently assumes virtually no network latency or jitter, so is only suitable
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/osc/output.py` & `isobar_ext-0.9.0/isobar_ext/io/supercollider/output.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,51 @@
+import logging
+
 from ..output import OutputDevice
-from ...pattern import Pattern
+
+log = logging.getLogger(__name__)
 
 try:
-    from pythonosc.udp_client import SimpleUDPClient
+    import supercollider
 except ModuleNotFoundError:
     pass
 
 
-class OSCOutputDevice(OutputDevice):
+class SuperColliderOutputDevice(OutputDevice):
     """
-    OSCOutputDevice: Wraps MIDI messages in OSC.
+    SuperColliderOutputDevice: Wraps MIDI messages in OSC.
     /note [ note, velocity, channel ]
     /control [ control, value, channel ]
     """
 
-    def __init__(self, host, port):
+    def __init__(self, host="127.0.0.1", port=57110):
         """
         Args:
             host: Hostname to send OSC messages to
             port: Port number to send OSC messages to
         """
         super().__init__()
         try:
-            self.osc = SimpleUDPClient(host, port)
+            self.server = supercollider.Server()
 
         except NameError:
-            raise Exception("python-osc must be installed")
+            raise Exception(
+                "The supercollider package must be installed: pip3 install supercollider"
+            )
+
+        self.default_synth_name = "sine"
+        self.synths = {}
 
     def note_on(self, note=60, velocity=64, channel=0):
-        self.osc.send_message("/note", velocity, channel)
+        synth_params = {"note": note, "velocity": velocity}
+        synth = supercollider.Synth(self.server, self.default_synth_name, synth_params)
+        self.synths[note] = synth
 
     def note_off(self, note=60, channel=0):
-        self.osc.send_message("/note", 0, channel)
+        pass
 
     def control(self, control, value, channel=0):
-        self.osc.send_message("/control", value, channel)
+        pass
 
-    def send(self, address, params=None):
-        if params is not None:
-            params = [Pattern.value(param) for param in params]
-        self.osc.send_message(address, params)
+    def create(self, name, params=None):
+        log.debug("Creating SuperCollider Synth: %s, %s" % (name, params))
+        supercollider.Synth(self.server, name, params)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/signalflow/output.py` & `isobar_ext-0.9.0/isobar_ext/io/signalflow/output.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from ..output import OutputDevice
-
-import logging
 import inspect
+import logging
+
+from ..output import OutputDevice
 
 log = logging.getLogger(__name__)
 
 try:
     import signalflow as sf
 except ModuleNotFoundError:
     # No SignalFlow support available
```

### Comparing `isobar_ext-0.5.1/isobar_ext/io/socketio/output.py` & `isobar_ext-0.9.0/isobar_ext/io/socketio/output.py`

 * *Files identical despite different names*

### Comparing `isobar_ext-0.5.1/isobar_ext/key.py` & `isobar_ext-0.9.0/isobar_ext/key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from .scale import Scale
+import random
+
 from .note import Note
+from .scale import Scale
 from .util import midi_note_to_note_name, note_name_to_midi_note
 
-import random
-
 
 class Key:
     """Represents a harmonic structure, containing a tonic and scale."""
 
     def __init__(self, tonic=0, scale=Scale.major):
         if isinstance(tonic, str):
             # --------------------------------------------------------------------------------
@@ -26,18 +26,18 @@
         self.tonic = tonic
         self.scale = scale
 
     def __eq__(self, other):
         return self.tonic == other.tonic and self.scale == other.scale
 
     def __str__(self):
-        return "Key: %s %s" % (midi_note_to_note_name(self.tonic)[:], self.scale.name)
+        return f"Key: {midi_note_to_note_name(self.tonic)[:]} {self.scale.name}"
 
     def __repr__(self):
-        return 'Key(%s, "%s")' % (self.tonic, self.scale.name)
+        return f'Key({self.tonic}, "{self.scale.name}")'
 
     def __hash__(self):
         return hash((self.tonic, hash(self.scale)))
 
     def get(self, *args, **kwargs):
         """Returns the <degree>th semitone within this key."""
         params = {"degree": None, "scale_down": False}
@@ -66,17 +66,17 @@
         if kwargs is not None:
             params |= kwargs
 
         semitone = params.get("semitone")
         # semitone -= self.tonic
         scale_down = params.get("scale_down")
         if (
-            scale_down and
-            hasattr(self.scale, "semitones_down") and
-            self.scale.semitones_down
+                scale_down and
+                hasattr(self.scale, "semitones_down") and
+                self.scale.semitones_down
         ):
             semitones = self.semitones_down
         else:
             semitones = self.semitones
         # Always return true if None (rest) is queried.
         if semitone is None:
             return True
@@ -108,17 +108,17 @@
         if kwargs is not None:
             parms |= kwargs
 
         note = parms.get("note")
 
         scale_down = parms.get("scale_down")
         if (
-            scale_down and
-            hasattr(self.scale, "semitones_down") and
-            self.scale.semitones_down
+                scale_down and
+                hasattr(self.scale, "semitones_down") and
+                self.scale.semitones_down
         ):
             semitones = self.scale.semitones_down
         else:
             semitones = self.scale.semitones
         if self.__contains__(semitone=note, scale_down=scale_down):
             return note
         else:
@@ -153,57 +153,56 @@
     def voiceleading(self, other):
         """Returns the most parsimonious voice leading between this key
         and <other>, as a list of N tuples (semiA, semiB) where N is the
         maximal length of (this, other), and semiA and semiB are members
         of each. May not be bijective."""
 
         if len(self.semitones) > len(other.semitones):
-            semisA = self.semitones
-            semisB = other.semitones
+            semis_a = self.semitones
+            semis_b = other.semitones
         else:
-            semisA = other.semitones
-            semisB = self.semitones
-        semisB = list(reversed(semisB))
+            semis_a = other.semitones
+            semis_b = self.semitones
+        semis_b = list(reversed(semis_b))
 
         leading = []
-        for semiA in semisA:
+        for semiA in semis_a:
             distances = []
-            for semiB in semisB:
+            for semiB in semis_b:
                 distance = abs(semiA - semiB)
                 if distance > self.scale.octave_size / 2:
                     distance = self.scale.octave_size - distance
                 distances.append(distance)
             index = distances.index(min(distances))
-            leading.append((semiA, semisB[index]))
+            leading.append((semiA, semis_b[index]))
 
         return leading
 
     def distance(self, other):
         leading = self.voiceleading(other)
-        distance = sum([abs(a_b[0] - a_b[1]) for a_b in leading])
-        return distance
+        return sum(abs(a_b[0] - a_b[1]) for a_b in leading)
 
     def fadeto(self, other, level):
         """level between 0..1"""
         semitones_a = self.semitones
         semitones_b = other.semitones
         semitones_shared = [n for n in semitones_b if n in semitones_a]
         semitones_a_only = [n for n in semitones_a if n not in semitones_b]
         semitones_b_only = [n for n in semitones_b if n not in semitones_a]
 
         if level < 0.5:
             # scale from 1..0
             level = 1.0 - (level * 2)
             count_from_a = int(round(level * len(semitones_a_only)))
-            return semitones_shared + semitones_a_only[0:count_from_a]
+            return semitones_shared + semitones_a_only[:count_from_a]
         else:
             # scale from 0..1
             level = 2 * (level - 0.5)
             count_from_b = int(round(level * len(semitones_b_only)))
-            return semitones_shared + semitones_b_only[0:count_from_b]
+            return semitones_shared + semitones_b_only[:count_from_b]
 
     @staticmethod
     def random():
         t = random.randint(0, 11)
         s = Scale.random()
         return Key(t, s)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/note.py` & `isobar_ext-0.9.0/isobar_ext/note.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from .util import midi_note_to_note_name
 
 
 class Note(object):
     names = ["C", "C#", "D", "D#", "E", "F", "F#", "G", "G#", "A", "A#", "B"]
 
     def __init__(self, note=60, velocity=64, duration=1.0):
+        self.midinote = None
         self.note = note
         self.velocity = velocity
         self.duration = duration
 
     def __str__(self):
         if self.velocity == 0:
             return "rest"
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/__init__.py` & `isobar_ext-0.9.0/isobar_ext/pattern/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # flake8: noqa
 
 __version__ = "0"
 __author__ = "Daniel Jones <http://www.erase.net/>"
 
+from .chance import *
 from .core import *
+from .fade import *
+from .lsystem import *
+from .markov import *
+from .midi import *
 from .oscillator import *
 from .scalar import *
 from .sequence import *
-from .chance import *
-from .lsystem import *
-from .markov import *
-from .warp import *
 from .static import *
 from .tonal import *
-from .fade import *
-from .midi import *
+from .warp import *
 
 __all__ = []
 key = value = None
 for key, value in vars().items():
     try:
         # Add every class to pydoc
         if issubclass(value, object):
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/chance.py` & `isobar_ext-0.9.0/isobar_ext/pattern/chance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
-import sys
+
 import copy
 import random
+import sys
 
 from .core import Pattern
+from .series import PSeries
 from ..util import wnchoice, scale_lin_exp
 
 
 class PStochasticPattern(Pattern):
     """
     PStochasticPattern is the superclass of all chance-based patterns.
     It contains its own random number generator and state, so that it can be
@@ -52,78 +54,67 @@
     >>> PWhite(0, 10).nextn(16)
     [8, 10, 8, 1, 7, 3, 1, 9, 9, 3, 2, 10, 7, 5, 10, 4]
 
     >>> PWhite(0.0, 10.0).nextn(16)
     [3.6747936220022082, 0.61313530428271923, 9.1515368696591555, ... 6.2963694390145974 ]
     """
 
-    def __init__(self, min: float = 0.0, max: float = 1.0):
+    def __init__(self, v_min: float = 0.0, v_max: float = 1.0):
         super().__init__()
 
-        self.min = min
-        self.max = max
+        self.min = v_min
+        self.max = v_max
 
     def __repr__(self):
-        return "PWhite(%s,%s)" % (self.min, self.max)
+        return f"PWhite({self.min},{self.max})"
 
     def __next__(self):
-        min = Pattern.value(self.min)
-        max = Pattern.value(self.max)
+        v_min = Pattern.value(self.min)
+        v_max = Pattern.value(self.max)
 
-        if isinstance(min, float):
-            return self.rng.uniform(min, max)
+        if isinstance(v_min, float):
+            return self.rng.uniform(v_min, v_max)
         else:
-            # --------------------------------------------------------------------------------
-            # rng.randint does not spread values across the range proportionately with
-            # varying values of [min, max]. Use rng.uniform() and do our own scaling to ensure
-            # that the output is controllable.
-            # --------------------------------------------------------------------------------
-            rv = int(self.rng.uniform(min, max))
-            return rv
+            return int(self.rng.uniform(v_min, v_max))
 
 
 class PBrown(PStochasticPattern):
     """PBrown: Brownian noise.
     Output begins at `initial_value`, and steps up/down
     by uniform random values from [-`step`, `step`]
     inclusive.
 
     If step is a float, the output is a float pattern.
     If step is an int, the output is an int pattern,
     with min <= values <= max.
     """
 
     def __init__(
-        self,
-        initial_value: float = 0,
-        step: float = 0.1,
-        min: float = -sys.maxsize,
-        max: float = sys.maxsize,
+            self,
+            initial_value: float = 0,
+            step: float = 0.1,
+            v_min: float = -sys.maxsize,
+            v_max: float = sys.maxsize,
     ):
         """
         Args:
             initial_value (float or int): Initial value
             step (float or int): Maximum value to increase or decrease by each step
-            min (float or int): Minimum permitted value
-            min (float or int): Maximum permitted value
+            v_min (float or int): Minimum permitted value
+            v_min (float or int): Maximum permitted value
         """
         super().__init__()
         self.initial_value = initial_value
         self.value = initial_value
         self.step = step
-        self.min = min
-        self.max = max
+        self.min = v_min
+        self.max = v_max
 
     def __repr__(self):
-        return "PBrown(%s, %s, %s, %s)" % (
-            self.initial_value,
-            self.step,
-            self.min,
-            self.max,
-        )
+        return f"PBrown({self.initial_value}, {self.step}, {self.min}, {self.max})"
 
     def reset(self):
         super().reset()
         self.value = self.initial_value
 
     def __next__(self):
         vstep = Pattern.value(self.step)
@@ -154,75 +145,64 @@
     """
 
     def __init__(self, probability: float = 0.5, regular: bool = False):
         super().__init__()
         self.probability = Pattern.pattern(probability)
         self.regular = regular
 
-        self.current_value = 0.0
-        if regular:
-            # Initialise current_value to 1 in order to immediately trigger
-            # coin() if regular is True
-            self.current_value = 1.0
+        self.current_value = 1.0 if regular else 0.0
 
     def __repr__(self):
-        return "PCoin(%s)" % self.probability
+        return f"PCoin({self.probability})"
 
     def __next__(self):
         probability = Pattern.value(self.probability)
-        regular = Pattern.value(self.regular)
-
-        if regular:
-            if self.current_value >= 1:
-                self.current_value -= 1
-                rv = 1
-            else:
-                rv = 0
-            self.current_value += probability
-            return rv
+        # if not (regular := Pattern.value(self.regular)):
+        if not (Pattern.value(self.regular)):
+            return 1 if self.rng.uniform(0, 1) < probability else 0
+        if self.current_value >= 1:
+            self.current_value -= 1
+            rv = 1
         else:
-            if self.rng.uniform(0, 1) < probability:
-                return 1
-            else:
-                return 0
+            rv = 0
+        self.current_value += probability
+        return rv
 
 
 class PRandomWalk(PStochasticPattern):
     """PWalk: Random walk around list.
            Jumps between `min` and `max` steps inclusive.
 
-    >>> PRandomWalk([ 0, 2, 5, 8, 11 ], min=1, max=2).nextn(16)
+    >>> PRandomWalk([ 0, 2, 5, 8, 11 ], v_min=1, v_max=2).nextn(16)
     [8, 11, 0, 8, 0, 11, 2, 11, 2, 0, 5, 8, 11, 8, 5, 8]
     """
 
     def __init__(
-        self, values: list = [], min: int = 1, max: int = 1, wrap: bool = True
+            self, values=None, v_min: int = 1, v_max: int = 1, wrap: bool = True
     ):
         """
 
         Args:
             values (list): Array of values to walk around
-            min (int): Minimum number of steps to move
-            max (int): Maximum number of steps to move
+            v_min (int): Minimum number of steps to move
+            v_max (int): Maximum number of steps to move
             wrap (bool): Whether to wrap around the start/end of the array
         """
         super().__init__()
+        self.pos = None
+        if values is None:
+            values = []
         self.values = values
-        self.min = min
-        self.max = max
+        self.min = v_min
+        self.max = v_max
         self.wrap = wrap
         self.reset()
 
     def __repr__(self):
-        return "PRandomWalk(%s, %s, %s, %s)" % (
-            repr(self.values),
-            self.min,
-            self.max,
-            self.wrap,
-        )
+        return f"PRandomWalk({repr(self.values)}, {self.min}, {self.max}, {self.wrap})"
 
     def reset(self):
         super().reset()
         self.pos = 0
 
     def __next__(self):
         vvalues = Pattern.value(self.values)
@@ -263,15 +243,15 @@
             weights: An optional list of weights, of the same length as values
         """
         super().__init__()
         self.values = values
         self.weights = weights
 
     def __repr__(self):
-        return "PChoice(%s, %s)" % (repr(self.values), repr(self.weights))
+        return f"PChoice({repr(self.values)}, {repr(self.weights)})"
 
     def __next__(self):
         vvalues = Pattern.value(self.values)
         vweights = Pattern.value(self.weights)
         if vweights is not None:
             return wnchoice(vvalues, vweights, rng=self.rng)
         else:
@@ -299,32 +279,28 @@
         """
         super().__init__()
         self.values = values
         self.count = count
         self.weights = weights
 
     def __repr__(self):
-        return "PSample(%s, %s, %s)" % (
-            repr(self.values),
-            self.count,
-            repr(self.weights),
-        )
+        return f"PSample({repr(self.values)}, {self.count}, {repr(self.weights)})"
 
     def __next__(self):
         vvalues = copy.copy(Pattern.value(self.values))
         vcount = copy.copy(Pattern.value(self.count))
         vweights = copy.copy(Pattern.value(self.weights))
 
         if vcount > len(vvalues):
             raise ValueError(
                 "Count cannot be larger than the number of available values"
             )
 
         rv = []
-        for n in range(vcount):
+        for _ in range(vcount):
             if vweights:
                 index = wnchoice(list(range(len(vvalues))), vweights, rng=self.rng)
                 vweights.pop(index)
             else:
                 index = self.rng.randrange(0, len(vvalues))
 
             rv.append(vvalues.pop(index))
@@ -336,30 +312,32 @@
     """PShuffle: Shuffled list.
 
     >>> p = PShuffle([ 1, 2, 3 ])
     >>> p.nextn(16)
     [1, 3, 2, 3, 2, 1, 2, 3, 1, 2, 3, 1, 1, 2, 3, 1]
     """
 
-    def __init__(self, values: list = [], repeats: int = sys.maxsize):
+    def __init__(self, values: list = None, repeats: int = sys.maxsize):
         """
         Args:
             values (list): List of values
             repeats (int): Number of times to re-shuffle and iterate
         """
+        if values is None:
+            values = []
         super().__init__()
         self.values_orig = copy.copy(values)
         self.repeats = repeats
 
         self.pos = 0
         self.rcount = 1
         self.values = copy.copy(self.values_orig)
 
     def __repr__(self):
-        return "PShuffle(%s, %s)" % (repr(self.values_orig), self.repeats)
+        return f"PShuffle({repr(self.values_orig)}, {self.repeats})"
 
     def reset(self):
         super().reset()
         self.pos = 0
         self.rcount = 0
         self.values = copy.copy(self.values_orig)
 
@@ -392,15 +370,15 @@
         super().__init__()
         self.pattern = pattern
         self.every = every
         self.values = []
         self.pos = 0
 
     def __repr__(self):
-        return "PShuffleInput(%s, %s)" % (repr(self.pattern), self.every)
+        return f"PShuffleInput({repr(self.pattern)}, {self.every})"
 
     def __next__(self):
         if self.pos >= len(self.values):
             self.pos = 0
 
         if self.pos == 0:
             kevery = Pattern.value(self.every)
@@ -421,28 +399,27 @@
         super().__init__()
         self.pattern = pattern
         self.play = play
         self.regular = regular
         self.pos = 0.0
 
     def __repr__(self):
-        return "PSkip(%s, %s, %s)" % (repr(self.pattern), self.play, self.regular)
+        return f"PSkip({repr(self.pattern)}, {self.play}, {self.regular})"
 
     def __next__(self):
         value = Pattern.value(self.pattern)
         play = Pattern.value(self.play)
 
         if self.regular:
             self.pos += play
             if self.pos >= 1:
                 self.pos -= 1
                 return value
-        else:
-            if self.rng.uniform(0, 1) < play:
-                return value
+        elif self.rng.uniform(0, 1) < play:
+            return value
 
         return None
 
 
 class PFlipFlop(PStochasticPattern):
     """PFlipFlop: flip a binary bit with some probability.
                <initial> is initial value (0 or 1)
@@ -458,46 +435,47 @@
         super().__init__()
         self.initial = initial
         self.value = initial
         self.p_on = p_on
         self.p_off = p_off
 
     def __repr__(self):
-        return "PFlipFlop(%s, %s, %s)" % (self.initial, self.p_on, self.p_off)
+        return f"PFlipFlop({self.initial}, {self.p_on}, {self.p_off})"
 
     def reset(self):
         super().reset()
         self.value = self.initial
 
     def __next__(self):
         self.value = Pattern.value(self.value)
         self.p_on = Pattern.value(self.p_on)
         self.p_off = Pattern.value(self.p_off)
 
         if self.value == 0:
             if self.rng.uniform(0, 1) < self.p_on:
                 self.value = 1
-        else:
-            if self.rng.uniform(0, 1) < self.p_off:
-                self.value = 0
+        elif self.rng.uniform(0, 1) < self.p_off:
+            self.value = 0
 
         return self.value
 
 
 class PSwitchOne(PStochasticPattern):
     """PSwitchOne: Capture `length` input values; loop, repeatedly switching two adjacent values."""
 
     def __init__(self, pattern: Pattern, length: int = 4):
         super().__init__()
+        self.pos = None
+        self.values = None
         self.pattern = pattern
         self.length = length
         self.reset()
 
     def __repr__(self):
-        return "PSwitchOne(%s, %s)" % (repr(self.pattern), self.length)
+        return f"PSwitchOne({repr(self.pattern)}, {self.length})"
 
     def reset(self):
         super().reset()
         self.values = []
         self.pos = 0
 
     def __next__(self):
@@ -507,17 +485,17 @@
             value = next(self.pattern)
             self.values.append(value)
             self.pos += 1
             return value
 
         if self.pos >= len(self.values):
             index = self.rng.randint(0, len(self.values)) - 1
-            indexP = (index + 1) % len(self.values)
-            self.values[index], self.values[indexP] = (
-                self.values[indexP],
+            index_p = (index + 1) % len(self.values)
+            self.values[index], self.values[index_p] = (
+                self.values[index_p],
                 self.values[index],
             )
             self.pos = 0
 
         rv = self.values[self.pos]
         self.pos += 1
         return rv
@@ -534,33 +512,30 @@
 
     >>> PRandomExponential(1.0, 100.0).nextn(16)
     [54.84880471711992, 89.53150541306805, 2.4077905492103318, ... ]
     """
 
     abbreviation = "prandexp"
 
-    def __init__(self, min: float = 1.0, max: float = 10.0):
+    def __init__(self, v_min: float = 1.0, v_max: float = 10.0):
         super().__init__()
 
-        self.min = min
-        self.max = max
+        self.min = v_min
+        self.max = v_max
 
     def __repr__(self):
-        return "PRandomExponential(%s, %s)" % (self.min, self.max)
+        return f"PRandomExponential({self.min}, {self.max})"
 
     def __next__(self):
-        min = Pattern.value(self.min)
-        max = Pattern.value(self.max)
+        v_min = Pattern.value(self.min)
+        v_max = Pattern.value(self.max)
 
         norm = self.rng.uniform(0, 1)
-        rv = scale_lin_exp(norm, 0, 1, min, max)
-        if isinstance(min, float):
-            return rv
-        else:
-            return int(rv)
+        rv = scale_lin_exp(norm, 0, 1, v_min, v_max)
+        return rv if isinstance(v_min, float) else int(rv)
 
 
 class PRandomImpulseSequence(PStochasticPattern):
     """PRandomImpulseSequence: Random sequence of impulses with probability `probability`.
 
     >>> PRandomImpulseSequence(0.3, 16).nextn(16)
     [...]
@@ -568,23 +543,26 @@
     """
 
     abbreviation = "prandimpseq"
 
     def __init__(self, probability: float = 0.0, length: int = 8):
         super().__init__()
 
+        self.every_index = None
+        self.every_count = None
+        self.every_action = None
         self.probability = probability
         self.length = length
         self.current_length = 0
         self.values = []
         self.pos = 0
         self.every(0)
 
     def __repr__(self):
-        return "PRandomImpulseSequence(%s, %s)" % (self.probability, self.length)
+        return f"PRandomImpulseSequence({self.probability}, {self.length})"
 
     def generate(self):
         probability = Pattern.value(self.probability)
         self.current_length = Pattern.value(self.length)
         self.values = [
             int(self.rng.uniform(0, 1) < probability)
             for _ in range(self.current_length)
@@ -605,29 +583,29 @@
 
         # return self so this can be used in scheduling:
         # "active": PRandomImpulseSequence(0.3, 8).every(8, "explore"),
         return self
 
     def explore(self):
         # TODO: Merge function with PExplorer
-        P_SWITCH = 0
-        P_MUTATE = 1
-        P_ROTATE = 2
-        op = self.rng.choice([P_SWITCH, P_MUTATE, P_ROTATE])
-        if op == P_SWITCH:
+        p_switch = 0
+        p_mutate = 1
+        p_rotate = 2
+        op = self.rng.choice([p_switch, p_mutate, p_rotate])
+        if op == p_switch:
             indices = list(range(len(self.values)))
             self.rng.shuffle(indices)
             self.values[indices[0]], self.values[indices[1]] = (
                 self.values[indices[1]],
                 self.values[indices[0]],
             )
-        elif op == P_MUTATE:
+        elif op == p_mutate:
             index = random.randrange(len(self.values))
             self.values[index] = 1 - self.values[index]
-        elif op == P_ROTATE:
+        elif op == p_rotate:
             direction_right = self.rng.uniform(0, 1) < 0.5
             if direction_right:
                 self.values = [self.values[-1]] + self.values[:-1]
             else:
                 self.values = self.values[1:] + [self.values[0]]
 
     def __next__(self):
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/core.py` & `isobar_ext-0.9.0/isobar_ext/pattern/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # -------------------------------------------------------------------------------
 # isobar_ext: a python library for expressing and manipulating musical patterns.
 # -------------------------------------------------------------------------------
 
 from __future__ import annotations
+
 import copy
 import inspect
 from typing import Iterable, Callable
 
 import isobar_ext
 
 
 class Pattern:
-    """Pattern: Abstract superclass of all pattern generators.
+    """ Pattern: Abstract superclass of all pattern generators.
 
-    Patterns are at the core of isobar_ext. A Pattern implements the iterator
-    protocol, representing a sequence of values which are iteratively
-    returned by the next() method. A pattern may be finite, after which
-    point it raises a StopIteration exception. Call reset() to return
-    a pattern to its initial state.
+        Patterns are at the core of isobar_ext. A Pattern implements the iterator
+        protocol, representing a sequence of values which are iteratively
+        returned by the next() method. A pattern may be finite, after which
+        point it raises a StopIteration exception. Call reset() to return
+        a pattern to its initial state.
 
-    Patterns can be subject to standard arithmetic operators as expected.
-    """
+        Patterns can be subject to standard arithmetic operators as expected.
+        """
 
     LENGTH_MAX = 65536
 
     def __repr__(self):
         # Used in place of a common string representation
         return "Pattern()"
 
@@ -34,15 +35,15 @@
         items = self.all()
         return len(items)
 
     def __neg__(self):
         return 0 - self
 
     def __abs__(self):
-        """Absolute value."""
+        """ Absolute value. """
         return PAbs(self)
 
     def __add__(self, operand):
         """Binary op: add two patterns"""
         return PAdd(self, operand)
 
     def __radd__(self, operand):
@@ -112,44 +113,75 @@
         return PRShift(self, operand)
 
     def __rrshift__(self, operand):
         """Right bitshift"""
         return PRShift(operand, self)
 
     def __eq__(self, operand):
-        """Equal"""
+        """ Equal """
         return PEqual(self, operand)
 
     def __ne__(self, operand):
-        """Not equal"""
+        """ Not equal """
         return PNotEqual(self, operand)
 
     def __gt__(self, operand):
-        """Greater than"""
+        """ Greater than """
         return PGreaterThan(self, operand)
 
     def __ge__(self, operand):
-        """Greater than or equal"""
+        """ Greater than or equal """
         return PGreaterThanOrEqual(self, operand)
 
     def __lt__(self, operand):
-        """Less than"""
+        """ Less than """
         return PLessThan(self, operand)
 
     def __le__(self, operand):
-        """Less than or equal"""
+        """ Less than or equal """
         return PLessThanOrEqual(self, operand)
 
     def __and__(self, operand):
-        """And"""
+        """ And """
         return PAnd(self, operand)
 
     def __iter__(self):
         return self
 
+    def poll(self, on: bool = True) -> object:
+        """
+        If set, causes the Pattern object to output its value to stdout each time
+        its __next__() method is called.
+
+        Returns the Pattern object, useful when scheduling like so:
+
+        timeline.schedule({
+            "note": pattern.poll(),
+            ...
+        })
+
+        Args:
+            on: Whether to poll the Pattern's output.
+
+        Returns:
+            The Pattern.
+        """
+        if not hasattr(self.__class__, "__next_orig__"):
+            self.__class__.__next_orig__ = self.__class__.__next__
+
+        def _get_and_print_next(self):
+            value = self.__next_orig__()
+            if hasattr(self, "_poll") and self._poll:
+                print("%s: %s" % (self.__class__.__name__, value))
+            return value
+
+        self.__class__.__next__ = _get_and_print_next
+        self._poll = on
+        return self
+
     def nextn(self, count: int) -> list:
         """
         Returns the next `count` output values.
         If fewer than `count` values are generated, return all output values.
         """
         rv = []
         try:
@@ -178,19 +210,19 @@
         except StopIteration:
             pass
 
         self.reset()
         return values
 
     def reset(self):
-        """Calling reset() should always reset a Pattern back to its initial state
-        immediately after construction.
+        """ Calling reset() should always reset a Pattern back to its initial state
+            immediately after construction.
 
-        When implementing new Patterns, this may require storing some state variables
-        to be stored.
+            When implementing new Patterns, this may require storing some state variables
+            to be stored.
         """
         fields = vars(self)
         for name, field in list(fields.items()):
             if isinstance(field, Pattern):
                 field.reset()
             # ------------------------------------------------------------------------
             # look through list items and reset anything in here too
@@ -216,16 +248,16 @@
         """
         Returns the timeline that this Pattern is embedded in, if any.
         """
         stack = inspect.stack()
         for frame in stack:
             frameobj = frame[0]
             args, _, _, value_dict = inspect.getargvalues(frameobj)
-            if len(args) and args[0] == "self":
-                instance = value_dict.get("self", None)
+            if len(args) and args[0] == 'self':
+                instance = value_dict.get('self', None)
                 classname = instance.__class__.__name__
                 if classname == "Timeline":
                     return instance
 
     def copy(self) -> Pattern:
         """
         Returns a copy of this Pattern.
@@ -246,102 +278,101 @@
     @staticmethod
     def pattern(v):
         """
         Patternify a value, turning it into an object with a next() method
         to obtain its next value.
 
         Pattern subclasses remain untouched.
-        Scalars and other objects are turned into PConstant objects."""
+        Scalars and other objects are turned into PConstant objects. """
 
         if isinstance(v, Pattern):
             return v
         elif isinstance(v, dict):
             return isobar_ext.PDict(v)
         elif isinstance(v, str):
-            from isobar_ext.shorthand.notation import parse_notation
-
+            from isobar_ext.notation import parse_notation
             try:
                 return parse_notation(v)
             except ValueError:
                 return isobar_ext.PConstant(v)
         else:
             return isobar_ext.PConstant(v)
 
 
 class PConstant(Pattern):
-    """PConstant: Returns a fixed value.
+    """ PConstant: Returns a fixed value.
 
-    >>> p = PConstant(4)
-    >>> p.nextn(16)
-    [4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4]
-    """
+        >>> p = PConstant(4)
+        >>> p.nextn(16)
+        [4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4, 4]
+        """
 
     def __init__(self, constant: float):
         self.constant = constant
 
     def __repr__(self):
-        return "PConstant(%s)" % repr(self.constant)
+        return ("PConstant(%s)" % repr(self.constant))
 
     def __next__(self):
         return self.constant
 
     def __float__(self):
         return float(self.constant)
 
 
 class PRef(Pattern):
-    """PRef: Contains a reference to another pattern, which can be replaced dynamically.
-    Returns the next value of the pattern contained.
-    Useful to change an inner pattern in real time.
-    """
+    """ PRef: Contains a reference to another pattern, which can be replaced dynamically.
+        Returns the next value of the pattern contained.
+        Useful to change an inner pattern in real time.
+        """
 
     def __init__(self, pattern: Pattern):
         self.pattern = pattern
 
     def __repr__(self):
-        return "PRef(%s)" % repr(self.pattern)
+        return ("PRef(%s)" % repr(self.pattern))
 
     def set_pattern(self, pattern: Pattern):
-        """Replace the referenced pattern with another."""
+        """ Replace the referenced pattern with another. """
         self.pattern = pattern
 
     def __next__(self):
         return next(self.pattern)
 
 
 class PFunc(Pattern):
-    """PFunc: Returns the value generated by a function.
-    Useful to incorporate additional logic into a pattern.
+    """ PFunc: Returns the value generated by a function.
+        Useful to incorporate additional logic into a pattern.
 
-    >>> seconds = PFunc(lambda: datetime.datetime.now().second)
-    >>> p.nextn(16)
-    [19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19]"""
+        >>> seconds = PFunc(lambda: datetime.datetime.now().second)
+        >>> p.nextn(16)
+        [19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19, 19]"""
 
     def __init__(self, function: Callable):
         self.function = function
 
     def __repr__(self):
-        return "PFunc(%s)" % repr(self.function)
+        return ("PFunc(%s)" % repr(self.function))
 
     def __next__(self):
         function = Pattern.value(self.function)
         return function()
 
 
 class PArrayIndex(Pattern):
-    """PArrayIndex: Request a specified index from an array.
-    If the item is a Pattern, the next value from that pattern is returned.
-    """
+    """ PArrayIndex: Request a specified index from an array.
+        If the item is a Pattern, the next value from that pattern is returned.
+        """
 
     def __init__(self, list: Iterable, index: int):
         self.list = list
         self.index = index
 
     def __repr__(self):
-        return "PArrayIndex(%s, %s)" % (self.list, self.index)
+        return ("PArrayIndex(%s, %s)" % (self.list, self.index))
 
     def __next__(self):
         list = Pattern.value(self.list)
         index = Pattern.value(self.index)
 
         # ------------------------------------------------------------------
         # null indices denote a rest -- so return a null value.
@@ -351,47 +382,47 @@
             return None
         else:
             index = int(index)
             return Pattern.value(list[index])
 
 
 class PDict(Pattern):
-    """PDict: Construct a pattern from a dict of arrays, or an array of dicts.
-    The below are equivalent:
+    """ PDict: Construct a pattern from a dict of arrays, or an array of dicts.
+        The below are equivalent:
 
-        PDict([ { "note" : 60, "velocity" : 64 }, { "note" : 67, "velocity" : 32 }, ... ])
-        PDict({ "note" : [ 60, 67 ], "velocity" : [ 64, 32 ]})
+            PDict([ { "note" : 60, "velocity" : 64 }, { "note" : 67, "velocity" : 32 }, ... ])
+            PDict({ "note" : [ 60, 67 ], "velocity" : [ 64, 32 ]})
 
-    Thanks to Dan Stowell <http://www.mcld.co.uk/>
-    """
+        Thanks to Dan Stowell <http://www.mcld.co.uk/>
+        """
 
     def __init__(self, value: dict = None):
         from .sequence import PSequence
 
         self.dict = {}
 
-        if isinstance(value, dict):
+        if type(value) == dict:
             # ------------------------------------------------------------------------
             # Value is a dict of arrays.
             # ------------------------------------------------------------------------
             self.dict = dict([(k, Pattern.pattern(v)) for k, v in value.items()])
-        elif isinstance(value, list):
+        elif type(value) == list:
             # ------------------------------------------------------------------------
             # Value is an array of dicts.
             # ------------------------------------------------------------------------
             self.dict = {}
             try:
                 keys = list(value[0].keys())
                 for key in keys:
                     self.dict[key] = PSequence([item[key] for item in value], 1)
             except IndexError:
                 pass
 
     def __repr__(self):
-        return "PDict(%s)" % repr(self.dict)
+        return ("PDict(%s)" % repr(self.dict))
 
     def __getitem__(self, key):
         return self.dict[key]
 
     def __setitem__(self, key, value):
         self.dict[key] = value
 
@@ -405,28 +436,26 @@
         """
         Load pattern data from a MIDI file.
 
         Args:
             filename (str): Filename to read from (.mid)
         """
         from isobar_ext.io.midifile import MidiFileInputDevice
-
         reader = MidiFileInputDevice(filename)
         self.dict = reader.read(quantize=quantize)
 
     def save(self, filename: str):
         """
         Save pattern data to a MIDI file.
 
         Args:
             filename (str): Filename to write to (.mid)
             quantize (float): Quantization level. 1.0 = quantize to beat, 0.25 = quantize to quarter-beat, etc.
         """
         from isobar_ext.io.midifile import MidiFileOutputDevice
-
         writer = MidiFileOutputDevice(filename)
         clock = isobar_ext.DummyClock()
         timeline = isobar_ext.Timeline(self, output_device=writer, clock_source=clock)
         timeline.schedule(self)
         timeline.stop_when_done = True
         try:
             clock.run()
@@ -458,44 +487,49 @@
         # for some reason, doing a list comprehension without the surrounding square
         # brackets causes an inner StopIteration to be suppressed -- we want to
         # explicitly raise it.
         rv = dict([(k, Pattern.value(vdict[k])) for k in vdict])
 
         return rv
 
+    def get(self, key, default=None):
+
+        return self.__getitem__(key) if key in self else default
+
 
 class PDictKey(Pattern):
-    """PDictKey: Request a specified key from a dictionary."""
+    """ PDictKey: Request a specified key from a dictionary.
+        """
 
     def __init__(self, dict: dict, key):
         self.dict = dict
         self.key = key
 
     def __repr__(self):
-        return "PDictKey(%s, %s)" % (repr(self.dict), repr(self.key))
+        return ("PDictKey(%s, %s)" % (repr(self.dict), repr(self.key)))
 
     def __next__(self):
         vdict = Pattern.value(self.dict)
         vkey = Pattern.value(self.key)
         return vdict[vkey]
 
 
 class PConcatenate(Pattern):
-    """PConcatenate: Concatenate the output of multiple sequences.
+    """ PConcatenate: Concatenate the output of multiple sequences.
 
-    >>> PConcatenate([ PSequence([ 1, 2, 3 ], 2), PSequence([ 9, 8, 7 ], 2) ]).nextn(16)
-    [1, 2, 3, 1, 2, 3, 9, 8, 7, 9, 8, 7]
-    """
+        >>> PConcatenate([ PSequence([ 1, 2, 3 ], 2), PSequence([ 9, 8, 7 ], 2) ]).nextn(16)
+        [1, 2, 3, 1, 2, 3, 9, 8, 7, 9, 8, 7]
+        """
 
     def __init__(self, inputs: list):
         self.inputs = inputs
         self.pos = 0
 
     def __repr__(self):
-        return "PConcatenate(%s)" % self.inputs
+        return ("PConcatenate(%s)" % self.inputs)
 
     def __next__(self):
         try:
             return next(self.inputs[self.pos])
         except StopIteration:
             if self.pos < len(self.inputs) - 1:
                 self.pos += 1
@@ -506,238 +540,237 @@
 
     def reset(self):
         super().reset()
         self.pos = 0
 
 
 class PAbs(Pattern):
-    """PAbs: Absolute value of `input`"""
+    """ PAbs: Absolute value of `input` """
 
     def __init__(self, input):
         self.input = input
 
     def __repr__(self):
-        return "PAbs(%s)" % repr(self.input)
+        return ("PAbs(%s)" % repr(self.input))
 
     def __next__(self):
         next = Pattern.value(self.input)
         if next is not None:
             return abs(next)
         return next
 
 
 class PInt(Pattern):
-    """PInt: Integer value of `input`"""
+    """ PInt: Integer value of `input` """
 
     def __init__(self, input: int):
         self.input = input
 
     def __repr__(self):
-        return "PInt(%s)" % self.input
+        return ("PInt(%s)" % self.input)
 
     def __next__(self):
         next = Pattern.value(self.input)
         if next is not None:
             return int(next)
         return next
 
 
 # ------------------------------------------------------------------
 # Binary operators
 # ------------------------------------------------------------------
 
-
 class PBinOp(Pattern):
     def __init__(self, a, b):
         self.a = a
         self.b = b
 
 
 class PAdd(PBinOp):
-    """PAdd: Add elements of two patterns (shorthand: patternA + patternB)"""
+    """ PAdd: Add elements of two patterns (shorthand: patternA + patternB) """
 
     def __str__(self):
         return "%s + %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a + b
 
 
 class PSub(PBinOp):
-    """PSub: Subtract elements of two patterns (shorthand: patternA - patternB)"""
+    """ PSub: Subtract elements of two patterns (shorthand: patternA - patternB) """
 
     def __str__(self):
         return "%s - %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a - b
 
 
 class PMul(PBinOp):
-    """PMul: Multiply elements of two patterns (shorthand: patternA * patternB)"""
+    """ PMul: Multiply elements of two patterns (shorthand: patternA * patternB) """
 
     def __str__(self):
         return "(%s) * (%s)" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a * b
 
 
 class PDiv(PBinOp):
-    """PDiv: Divide elements of two patterns (shorthand: patternA / patternB)"""
+    """ PDiv: Divide elements of two patterns (shorthand: patternA / patternB) """
 
     def __str__(self):
         return "(%s) / (%s)" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a / b
 
 
 class PFloorDiv(PBinOp):
-    """PFloorDiv: Integer division (shorthand: patternA // patternB)"""
+    """ PFloorDiv: Integer division (shorthand: patternA // patternB) """
 
     def __str__(self):
         return "(%s) // (%s)" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a // b
 
 
 class PMod(PBinOp):
-    """PMod: Modulo elements of two patterns (shorthand: patternA % patternB)"""
+    """ PMod: Modulo elements of two patterns (shorthand: patternA % patternB) """
 
     def __str__(self):
         return "(%s) %% (%s)" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a % b
 
 
 class PPow(PBinOp):
-    """PPow: One pattern to the power of another (shorthand: patternA ** patternB)"""
+    """ PPow: One pattern to the power of another (shorthand: patternA ** patternB) """
 
     def __str__(self):
         return "pow(%s, %s)" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else pow(a, b)
 
 
 class PLShift(PBinOp):
-    """PLShift: Binary left-shift (shorthand: patternA << patternB)"""
+    """ PLShift: Binary left-shift (shorthand: patternA << patternB) """
 
     def __str__(self):
         return "(%s << %s)" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a << b
 
 
 class PRShift(PBinOp):
-    """PRShift: Binary right-shift (shorthand: patternA << patternB)"""
+    """ PRShift: Binary right-shift (shorthand: patternA << patternB) """
 
     def __str__(self):
         return "(%s >> %s)" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a >> b
 
 
 class PEqual(PBinOp):
-    """PEqual: Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB)"""
+    """ PEqual: Return 1 if a == b, 0 otherwise (shorthand: patternA == patternB) """
 
     def __str__(self):
         return "%s == %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a == b
 
 
 class PNotEqual(PBinOp):
-    """PGreaterThanOrEqual: Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB)"""
+    """ PGreaterThanOrEqual: Return 1 if a != b, 0 otherwise (shorthand: patternA != patternB) """
 
     def __str__(self):
         return "%s != %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a != b
 
 
 class PGreaterThan(PBinOp):
-    """PGreaterThan: Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB)"""
+    """ PGreaterThan: Return 1 if a > b, 0 otherwise (shorthand: patternA > patternB) """
 
     def __str__(self):
         return "%s > %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a > b
 
 
 class PGreaterThanOrEqual(PBinOp):
-    """PGreaterThanOrEqual: Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB)"""
+    """ PGreaterThanOrEqual: Return 1 if a >= b, 0 otherwise (shorthand: patternA >= patternB) """
 
     def __str__(self):
         return "%s >= %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a >= b
 
 
 class PLessThan(PBinOp):
-    """PLessThan: Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB)"""
+    """ PLessThan: Return 1 if a < b, 0 otherwise (shorthand: patternA < patternB) """
 
     def __str__(self):
         return "%s < %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a < b
 
 
 class PLessThanOrEqual(PBinOp):
-    """PLessThanOrEqual: Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB)"""
+    """ PLessThanOrEqual: Return 1 if a <= b, 0 otherwise (shorthand: patternA <= patternB) """
 
     def __str__(self):
         return "%s <= %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
         return None if a is None or b is None else a <= b
 
 
 class PAnd(PBinOp):
-    """PAnd: Return True if a and b, False otherwise (shorthand: patternA & patternB)"""
+    """ PAnd: Return True if a and b, False otherwise (shorthand: patternA & patternB) """
 
     def __str__(self):
         return "%s & %s" % (self.a, self.b)
 
     def __next__(self):
         a = Pattern.value(self.a)
         b = Pattern.value(self.b)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/fade.py` & `isobar_ext-0.9.0/isobar_ext/pattern/fade.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """ isobar_ext.pattern.fade: Unary pattern operators to fade a pattern in or out.
 
     Rather than simply beginning a pattern, we may want to start by playing a
     single note, introducing the rest gradually.
     """
 
 from __future__ import annotations
+
 import random
+
 from .core import Pattern
 
 
 class PFade(Pattern):
     IN = 1
     PEAK = 0
     OUT = -1
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/lsystem.py` & `isobar_ext-0.9.0/isobar_ext/pattern/lsystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
-from .core import Pattern
+
 import random
 
+from .core import Pattern
+
 
 class LSystem:
     def __init__(self, rule: str = "N[-N++N]-N", seed="N"):
         self.rule = rule
         self.seed = seed
         self.string = seed
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/markov.py` & `isobar_ext-0.9.0/isobar_ext/pattern/markov.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
-from .chance import PStochasticPattern
-from .core import Pattern
 
 import os
 from typing import Iterable
 
+from .chance import PStochasticPattern
+from .core import Pattern
+
 
 class PMarkov(PStochasticPattern):
     """PMarkov: First-order Markov chain generator."""
 
     def __init__(self, nodes: Iterable = None):
         """Create a new Markov chain. 'nodes' can be either be:
         * an ordered sequence of notes (which will be used to infer the
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/midi.py` & `isobar_ext-0.9.0/isobar_ext/pattern/midi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 MIDI control: Patterns which generate their outputs based on MIDI devices.
 """
 
-from .core import Pattern
-
+import os
 from typing import Optional
+
 import mido
-import os
+
+from .core import Pattern
 
 
 class isobar_extMIDIManager:
     shared_manager = None
 
     def __init__(self, device_name: str = None):
         if device_name is None:
@@ -40,15 +41,15 @@
     def on_control_change(self, control, value):
         for handler in self.control_handlers[control]:
             handler.on_change(value)
 
 
 class PMIDIControl(Pattern):
     def __init__(
-        self, control_index: int = 0, normalized: bool = False, default: int = None
+            self, control_index: int = 0, normalized: bool = False, default: int = None
     ):
         self.control_index: int = control_index
         self.value: Optional[int] = default
         self.normalized: bool = normalized
 
         manager = isobar_extMIDIManager.get_shared_manager()
         manager.add_control_handler(self.control_index, self)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/oscillator.py` & `isobar_ext-0.9.0/isobar_ext/pattern/oscillator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """ oscillator.py: Regular waveforms as pattern generators. """
 
 from __future__ import annotations
+
 from .core import Pattern
 
 
 class PTri(Pattern):
     """PTri: Generates a triangle waveform of period `length`.
 
     >>> p = PTri(10)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/scalar.py` & `isobar_ext-0.9.0/isobar_ext/pattern/scalar.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
-from .core import Pattern
-from .sequence import PSeries
-from ..util import scale_lin_exp, scale_lin_lin
 
 from typing import Callable
 
+from .core import Pattern
+from .series import PSeries
+from ..util import scale_lin_exp, scale_lin_lin
+
 
 class PChanged(Pattern):
     """PChanged: Outputs a 1 if the value of the input pattern has changed,
     or 0 otherwise.
 
     >>> a = PSequence([1, 0, 1, 2, 2, 2, 1, 0, 0, 1], repeats=1)
     >>> b = PChanged(a)
@@ -300,20 +301,20 @@
     """PIndexOf: Find index of items from `pattern` in <list>
 
     >>> p = PIndexOf([ chr(ord("a") + n) for n in range(26) ], PSeq("isobar_ext"))
     >>> p.nextn(16)
     [8, 18, 14, 1, 0, 17, 8, 18, 14, 1, 0, 17, 8, 18, 14, 1]
     """
 
-    def __init__(self, list: Pattern, item):
-        self.list = list
+    def __init__(self, lst: Pattern, item):
+        self.lst = lst
         self.item = item
 
     def __repr__(self):
-        return "PIndexOf(%s, %s)" % (repr(self.list), repr(self.item))
+        return "PIndexOf(%s, %s)" % (repr(self.lst), repr(self.item))
 
     def __next__(self):
-        list = Pattern.value(self.list)
+        lst = Pattern.value(self.lst)
         item = Pattern.value(self.item)
-        if list is None or item is None or item not in list:
+        if lst is None or item is None or item not in lst:
             return None
-        return list.index(item)
+        return lst.index(item)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/sequence.py` & `isobar_ext-0.9.0/isobar_ext/pattern/sequence.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 from __future__ import annotations
-import sys
-import math
+
 import copy  # noqa: F401
-import random
 import itertools
-from typing import Iterable, Callable
+import logging
+import math
+import random
+import sys
+from functools import reduce
+from typing import Iterable, Callable, List
 
+from .chance import PStochasticPattern
 from .core import Pattern
 from ..chord import Chord
 from ..constants import INTERPOLATION_NONE, INTERPOLATION_LINEAR, INTERPOLATION_COSINE
-from functools import reduce
-from .chance import PStochasticPattern
-
-import logging
 
 log = logging.getLogger(__name__)
 
 
 class PSequence(Pattern):
-    """Sequence: Sequence of values based on an array
-    Takes an input list, and repeats the items in this list.
+    """ Sequence: Sequence of values based on an array
+        Takes an input list, and repeats the items in this list.
 
-    >>> p = PSeq([ 1, 2, 3, 5 ])
-    >>> p.nextn(10)
-    [1, 2, 3, 5, 1, 2, 3, 5, 1, 2, 3, 5, 1, 2, 3, 5]
-    """
+        >>> p = PSeq([ 1, 2, 3, 5 ])
+        >>> p.nextn(10)
+        [1, 2, 3, 5, 1, 2, 3, 5, 1, 2, 3, 5, 1, 2, 3, 5]
+        """
 
     abbreviation = "pseq"
 
     def __init__(self, sequence: Iterable = None, repeats: int = sys.maxsize):
         # ------------------------------------------------------------------------
         # take a copy of the list to avoid changing the original
         # ------------------------------------------------------------------------
         if not hasattr(sequence, "__getitem__"):
             raise ValueError("Sequence must take a list argument")
         if sequence is None:
             sequence = []
         elif isinstance(sequence, str):
             sequence = Pattern.pattern(sequence).sequence
-        self.sequence = sequence
+        self.sequence: List = list(sequence)
         self.repeats = repeats
 
         self.reset()
 
     def __repr__(self):
-        return "PSequence(%s, %s)" % (repr(self.sequence), self.repeats)
+        return ("PSequence(%s, %s)" % (repr(self.sequence), self.repeats))
 
     def reset(self):
         super().reset()
         self.rcount = 0
         self.pos = 0
 
     def __next__(self):
@@ -81,72 +81,36 @@
         return self.sequence[item]
 
 
 # Backwards-compatbility
 PSeq = PSequence
 
 
-class PSeries(Pattern):
-    """PSeries: Arithmetic series, beginning at `start`, increment by `step`
-
-    >>> p = PSeries(3, 9)
-    >>> p.nextn(16)
-    [3, 12, 21, 30, 39, 48, 57, 66, 75, 84, 93, 102, 111, 120, 129, 138]
-    """
-
-    def __init__(self, start: float = 0, step: float = 1, length: int = sys.maxsize):
-        self.start = start
-        self.value = start
-        self.step = step
-        self.length = length
-        self.count = 0
-
-    def __repr__(self):
-        return "PSeries(%s, %s, %s)" % (self.start, self.step, self.length)
-
-    def reset(self):
-        super().reset()
-
-        self.value = self.start
-        self.count = 0
-
-    def __next__(self):
-        length = Pattern.value(self.length)
-        if self.count >= length:
-            # return None
-            raise StopIteration
-        step = Pattern.value(self.step)
-        n = self.value
-        self.value += step
-        self.count += 1
-        return n
-
-
 class PRange(Pattern):
-    """PRange: Similar to PSeries, but specify a max/step value.
+    """ PRange: Similar to PSeries, but specify a max/step value.
 
-    >>> p = PRange(0, 20, 2)
-    >>> p.nextn(16)
-    [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
-    """
+        >>> p = PRange(0, 20, 2)
+        >>> p.nextn(16)
+        [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
+        """
 
     def __init__(self, start: float = 0, end: float = 128, step=1):
         """
         Args:
             start (int or float): Start value
             end (int, float or Pattern): End value
             step (int, float or Pattern): Step value
         """
         self.start = start
         self.end = end
         self.step = step
         self.reset()
 
     def __repr__(self):
-        return "PRange(%s, %s, %s)" % (self.start, self.end, repr(self.step))
+        return ("PRange(%s, %s, %s)" % (self.start, self.end, repr(self.step)))
 
     def reset(self):
         super().reset()
         self.value = self.start
 
     def __next__(self):
         end = Pattern.value(self.end)
@@ -157,32 +121,30 @@
             raise StopIteration
         rv = self.value
         self.value += step
         return rv
 
 
 class PGeom(Pattern):
-    """PGeom: Geometric series, beginning at `start`, multiplied by `step`
+    """ PGeom: Geometric series, beginning at `start`, multiplied by `step`
+
+        >>> p = PGeom(1, 2)
+        >>> p.nextn(16)
+        [1, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768]
+        """
 
-    >>> p = PGeom(1, 2)
-    >>> p.nextn(16)
-    [1, 2, 4, 8, 16, 32, 64, 128, 256, 512, 1024, 2048, 4096, 8192, 16384, 32768]
-    """
-
-    def __init__(
-        self, start: float = 1, multiply: float = 2, length: int = sys.maxsize
-    ):
+    def __init__(self, start: float = 1, multiply: float = 2, length: int = sys.maxsize):
         self.start = start
         self.value = start
         self.multiply = multiply
         self.length = length
         self.count = 0
 
     def __repr__(self):
-        return "PGeom(%s, %s, %s)" % (self.start, self.multiply, self.length)
+        return ("PGeom(%s, %s, %s)" % (self.start, self.multiply, self.length))
 
     def reset(self):
         super().reset()
         self.value = self.start
         self.count = 0
 
     def __next__(self):
@@ -194,27 +156,27 @@
         rv = self.value
         self.value *= multiply
         self.count += 1
         return rv
 
 
 class PImpulse(Pattern):
-    """PImpulse: Outputs a 1 every <period> events, otherwise 0.
+    """ PImpulse: Outputs a 1 every <period> events, otherwise 0.
 
-    >>> p = PImpulse(4)
-    >>> p.nextn(16)
-    [1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0]
-    """
+        >>> p = PImpulse(4)
+        >>> p.nextn(16)
+        [1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0, 1, 0, 0, 0]
+        """
 
     def __init__(self, period: int):
         self.period = period
         self.pos = 0
 
     def __repr__(self):
-        return "PImpulse(%s)" % self.period
+        return ("PImpulse(%s)" % self.period)
 
     def reset(self):
         super().reset()
         self.pos = 0
 
     def __next__(self):
         period = Pattern.value(self.period)
@@ -228,34 +190,34 @@
             rv = 0
         self.pos += 1
 
         return rv
 
 
 class PLoop(Pattern):
-    """PLoop: Repeats a finite `pattern` for `n` repeats.
-    Useful for pattern generators which don't natively loop.
+    """ PLoop: Repeats a finite `pattern` for `n` repeats.
+        Useful for pattern generators which don't natively loop.
 
-    Input must be finite or results may vary.
+        Input must be finite or results may vary.
 
-    >>> p = PLoop(PSeq([ 1, 4, 9 ], 1))
-    >>> p.nextn(16)
-    [1, 4, 9, 1, 4, 9, 1, 4, 9, 1, 4, 9, 1, 4, 9, 1]
-    """
+        >>> p = PLoop(PSeq([ 1, 4, 9 ], 1))
+        >>> p.nextn(16)
+        [1, 4, 9, 1, 4, 9, 1, 4, 9, 1, 4, 9, 1, 4, 9, 1]
+        """
 
     def __init__(self, pattern: Pattern, count: int = sys.maxsize):
         self.pattern = pattern
         self.count = count
         self.pos = 0
         self.loop_index = 0
         self.read_all = False
         self.values = []
 
     def __repr__(self):
-        return "PLoop(%s, %s)" % (repr(self.pattern), self.count)
+        return ("PLoop(%s, %s)" % (repr(self.pattern), self.count))
 
     def reset(self):
         super().reset()
         self.pos = 0
         self.loop_index = 0
         self.read_all = False
         self.values = []
@@ -277,28 +239,28 @@
 
         rv = self.values[self.pos]
         self.pos += 1
         return rv
 
 
 class PPingPong(Pattern):
-    """PPingPong: Ping-pong input pattern back and forth N times.
+    """ PPingPong: Ping-pong input pattern back and forth N times.
 
-    >>> p = PPingPong(PSeq([ 1, 4, 9 ], 1), 10)
-    >>> p.nextn(16)
-    [1, 4, 9, 4, 1, 4, 9, 4, 1, 4, 9, 4, 1, 4, 9, 4]
-    """
+        >>> p = PPingPong(PSeq([ 1, 4, 9 ], 1), 10)
+        >>> p.nextn(16)
+        [1, 4, 9, 4, 1, 4, 9, 4, 1, 4, 9, 4, 1, 4, 9, 4]
+        """
 
     def __init__(self, pattern: Pattern, count: int = 1):
         self.pattern = pattern
         self.count = count
         self.reset()
 
     def __repr__(self):
-        return "PPingPong(%s, %s)" % (repr(self.pattern), self.count)
+        return ("PPingPong(%s, %s)" % (repr(self.pattern), self.count))
 
     def reset(self):
         super().reset()
         self.pattern.reset()
         self.values = self.pattern.all()
         self.pos = 0
         self.dir = 1
@@ -316,44 +278,31 @@
             self.dir = 1
             self.rpos += 1
 
         return rv
 
 
 class PCreep(Pattern):
-    """PCreep: Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
+    """ PCreep: Loop `length`-note segment, progressing `creep` notes after `repeats` repeats.
 
-    >>> p = PCreep(PSeries(), 3, 1, 2)
-    >>> p.nextn(16)
-    [0, 1, 2, 0, 1, 2, 1, 2, 3, 1, 2, 3, 2, 3, 4, 2]
-    """
-
-    def __init__(
-        self,
-        pattern: Pattern,
-        length: int = 4,
-        creep: int = 1,
-        repeats: int = 1,
-        prob: float = 1,
-    ):
+        >>> p = PCreep(PSeries(), 3, 1, 2)
+        >>> p.nextn(16)
+        [0, 1, 2, 0, 1, 2, 1, 2, 3, 1, 2, 3, 2, 3, 4, 2]
+        """
+
+    def __init__(self, pattern: Pattern, length: int = 4, creep: int = 1, repeats: int = 1, prob: float = 1):
         self.pattern = pattern
         self.length = length
         self.creep = creep
         self.repeats = repeats
         self.prob = prob
         self.reset()
 
     def __repr__(self):
-        return "PCreep(%s, %s, %s, %s, %s)" % (
-            repr(self.pattern),
-            self.length,
-            self.creep,
-            self.repeats,
-            self.prob,
-        )
+        return ("PCreep(%s, %s, %s, %s, %s)" % (repr(self.pattern), self.length, self.creep, self.repeats, self.prob))
 
     def reset(self):
         super().reset()
         self.buffer = []
         self.pos = 0
         self.rcount = 1
         while len(self.buffer) < self.length:
@@ -396,63 +345,60 @@
                 self.pos = 0
 
         self.pos += 1
         return self.buffer[self.pos - 1]
 
 
 class PStutter(Pattern):
-    """PStutter: Play each note of `pattern` `count` times.
-    Is really a more convenient way to do:
+    """ PStutter: Play each note of `pattern` `count` times.
+        Is really a more convenient way to do:
 
-        PCreep(pattern, 1, 1, count)
+            PCreep(pattern, 1, 1, count)
 
-    >>> p = PStutter(PSeries(), 2)
-    >>> p.nextn(16)
-    [0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5, 6, 6, 7, 7]
-    """
+        >>> p = PStutter(PSeries(), 2)
+        >>> p.nextn(16)
+        [0, 0, 1, 1, 2, 2, 3, 3, 4, 4, 5, 5, 6, 6, 7, 7]
+        """
 
     def __init__(self, pattern: Pattern, count: int = 2):
         self.pattern = Pattern.pattern(pattern)
         self.count = count
         self.count_current = 0
         self.pos = 0
         self.value = 0
 
     def __repr__(self):
-        return "PStutter(%s, %s)" % (repr(self.pattern), self.count)
+        return ("PStutter(%s, %s)" % (repr(self.pattern), self.count))
 
     def __next__(self):
         if self.pos >= self.count_current:
             self.count_current = Pattern.value(self.count)
             self.value = next(self.pattern)
             self.pos = 0
         self.pos += 1
         return self.value
 
 
 class PSubsequence(Pattern):
-    """PSubsequence: Returns a finite subsequence of an input pattern.
+    """ PSubsequence: Returns a finite subsequence of an input pattern.
 
-    >>> p = PSubsequence(...)
-    >>> p.nextn(16)
-    """
+        >>> p = PSubsequence(PSeries(0, 1), 2, 4)
+        >>> p.nextn(16)
+        [2, 3, 4, 5]
+        """
 
     def __init__(self, pattern: Pattern, offset: int, length: int):
         self.pattern = pattern
         self.offset = offset
         self.length = length
         self.pos = 0
         self.values = []
 
     def __repr__(self):
-        return "PSubsequence(%s, %s, %s)" % (
-            repr(self.pattern),
-            self.offset,
-            self.length,
-        )
+        return ("PSubsequence(%s, %s, %s)" % (repr(self.pattern), self.offset, self.length))
 
     def reset(self):
         super().reset()
         self.pos = 0
 
     def __next__(self):
         offset = Pattern.value(self.offset)
@@ -467,28 +413,22 @@
         rv = self.values[offset + self.pos]
         self.pos += 1
 
         return rv
 
 
 class PInterpolate(Pattern):
-    def __init__(
-        self, pattern: Pattern, steps: int, interpolation: str = INTERPOLATION_LINEAR
-    ):
+    def __init__(self, pattern: Pattern, steps: int, interpolation: str = INTERPOLATION_LINEAR):
         self.pattern = pattern
         self.steps = steps
         self.interpolation = interpolation
         self.reset()
 
     def __repr__(self):
-        return "PInterpolate(%s, %s, %s)" % (
-            repr(self.pattern),
-            self.steps,
-            repr(self.interpolation),
-        )
+        return ("PInterpolate(%s, %s, %s)" % (repr(self.pattern), self.steps, repr(self.interpolation)))
 
     def reset(self):
         super().reset()
         self.value = next(self.pattern)
         self.step_values = [self.value]
         self.pos = 0
 
@@ -505,149 +445,144 @@
                 vsteps = int(Pattern.value(self.steps))
             target = next(self.pattern)
 
             # --------------------------------------------------------------------------------
             # Calculate interpolated values.
             # --------------------------------------------------------------------------------
             if self.interpolation == INTERPOLATION_NONE:
-                self.step_values = list(self.value for n in range(vsteps - 1)) + [
-                    target
-                ]
+                self.step_values = list(self.value for n in range(vsteps - 1)) + [target]
             elif self.interpolation == INTERPOLATION_LINEAR:
                 dt = target - self.value
-                self.step_values = list(
-                    self.value + dt * (n + 1) / vsteps for n in range(vsteps)
-                )
+                self.step_values = list(self.value + dt * (n + 1) / vsteps for n in range(vsteps))
             elif self.interpolation == INTERPOLATION_COSINE:
                 dt = target - self.value
-                self.step_values = list(
-                    self.value + dt * 0.5 * (1.0 - math.cos(math.pi * (n + 1) / vsteps))
-                    for n in range(vsteps)
-                )
+                self.step_values = list(self.value + dt * 0.5 * (1.0 - math.cos(math.pi * (n + 1) / vsteps))
+                                        for n in range(vsteps))
             else:
                 raise ValueError("Interpolation type not recognised")
             self.pos = 0
 
         self.value = self.step_values[self.pos]
         self.pos += 1
         return self.value
 
 
 class PReverse(Pattern):
-    """PReverse: Reverses a finite sequence."""
+    """ PReverse: Reverses a finite sequence. """
 
     def __init__(self, input: Pattern):
         self.input = input
         self.reset()
 
     def __repr__(self):
-        return "PReverse(%s)" % repr(self.input)
+        return ("PReverse(%s)" % repr(self.input))
 
     def reset(self):
         super().reset()
         self.values = reversed(list(self.input))
 
     def __next__(self):
         return next(self.values)
 
 
 class PReset(Pattern):
-    """PReset: Resets `pattern` whenever `trigger` is true
+    """ PReset: Resets `pattern` whenever `trigger` is true
 
-    >>> p = PReset(PSeries(0, 1), PImpulse(4))
-    >>> p.nextn(16)
-    [0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3]
-    """
+        >>> p = PReset(PSeries(0, 1), PImpulse(4))
+        >>> p.nextn(16)
+        [0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3]
+        """
 
     def __init__(self, pattern: Pattern, trigger):
         self.pattern = pattern
         self.trigger = trigger
 
     def __repr__(self):
-        return "PReset(%s, %s)" % (repr(self.pattern), repr(self.trigger))
+        return ("PReset(%s, %s)" % (repr(self.pattern), repr(self.trigger)))
 
     def __next__(self):
         trigger_input = next(self.trigger)
         if trigger_input is not None and trigger_input > 0:
             self.pattern.reset()
 
         return next(self.pattern)
 
 
 class PCounter(Pattern):
-    """PCounter: Increments a counter by 1 for each zero-crossing in `trigger`.
+    """ PCounter: Increments a counter by 1 for each zero-crossing in `trigger`.
 
-    >>> p = PCounter(PImpulse(4))
-    >>> p.nextn(16)
-    [1, 1, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4]
-    """
+        >>> p = PCounter(PImpulse(4))
+        >>> p.nextn(16)
+        [1, 1, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3, 4, 4, 4, 4]
+        """
 
     def __init__(self, trigger):
         self.trigger = trigger
         self.value = 0
         self.count = 0
 
     def __repr__(self):
-        return "PCounter(%s)" % repr(self.trigger)
+        return ("PCounter(%s)" % repr(self.trigger))
 
     def __next__(self):
         value = next(self.trigger)
         if value > 0 and self.value <= 0:
             self.count += 1
             self.value = value
         elif value <= 0 and self.value > 0:
             self.value = value
 
         return self.count
 
 
 class PCollapse(Pattern):
-    """PCollapse: Skip over any rests in `input`"""
+    """ PCollapse: Skip over any rests in `input` """
 
     def __init__(self, input):
         self.input = input
 
     def __repr__(self):
-        return "PCollapse(%s)" % repr(self.input)
+        return ("PCollapse(%s)" % repr(self.input))
 
     def __next__(self):
         rv = None
         while rv is None:
             rv = Pattern.value(self.input)
         return rv
 
 
 class PNoRepeats(Pattern):
-    """PNoRepeats: Skip over repeated values in `input`"""
+    """ PNoRepeats: Skip over repeated values in `input` """
 
     def __init__(self, input):
         self.input = input
         self.value = sys.maxsize
 
     def __repr__(self):
-        return "PNoRepeats(%s)" % repr(self.input)
+        return ("PNoRepeats(%s)" % repr(self.input))
 
     def __next__(self):
         rv = sys.maxsize
         while rv == self.value or rv == sys.maxsize:
             rv = Pattern.value(self.input)
         self.value = rv
         return rv
 
 
 class PPad(Pattern):
-    """PPad: Pad `pattern` with rests until it reaches length `length`."""
+    """ PPad: Pad `pattern` with rests until it reaches length `length`.
+        """
 
     def __init__(self, pattern: Pattern, length: int):
         self.pattern = pattern
         self.length = length
         self.reset()
 
     def __repr__(self):
-        return "PPad(%s, %s)" % (repr(self.pattern), self.length)
+        return ("PPad(%s, %s)" % (repr(self.pattern), self.length))
 
     def reset(self):
         super().reset()
         self.count = 0
 
     def __next__(self):
         try:
@@ -658,34 +593,30 @@
             rv = None
 
         self.count += 1
         return rv
 
 
 class PPadToMultiple(Pattern):
-    """PPadToMultiple: Pad `pattern` with rests until its length is divisible by `multiple`.
-    Enforces a minimum padding of `minimum_pad`.
+    """ PPadToMultiple: Pad `pattern` with rests until its length is divisible by `multiple`.
+        Enforces a minimum padding of `minimum_pad`.
 
-    Useful to create patterns which occupy a whole number of bars.
-    """
+        Useful to create patterns which occupy a whole number of bars.
+        """
 
     def __init__(self, pattern: Pattern, multiple: float, minimum_pad: int = 0):
         self.pattern = pattern
         self.multiple = multiple
         self.minimum_pad = minimum_pad
         self.count = 0
         self.padcount = 0
         self.terminated = False
 
     def __repr__(self):
-        return "PPadToMultiple(%s, %s, %s)" % (
-            repr(self.pattern),
-            self.multiple,
-            self.minimum_pad,
-        )
+        return ("PPadToMultiple(%s, %s, %s)" % (repr(self.pattern), self.multiple, self.minimum_pad))
 
     def __next__(self):
         try:
             rv = next(self.pattern)
         except StopIteration:
             if self.padcount >= self.minimum_pad and (self.count % self.multiple == 0):
                 raise StopIteration
@@ -694,29 +625,28 @@
                 self.padcount += 1
 
         self.count += 1
         return rv
 
 
 class PArpeggiator(PStochasticPattern):
-    """PArpeggiator: Arpeggiator.
-
-    <type> can be one of:
-        PArp.UP
-        PArp.DOWN
-        PArp.UPDOWN
-        PArp.CONVERGE
-        PArp.DIVERGE
-        PArp.RANDOM
-
-    >>> p = PLoop(PArpeggiator(Chord.major, PArpeggiator.CONVERGE))
-    >>> p.nextn(16)
-    [0, 12, 4, 7, 0, 12, 4, 7, 0, 12, 4, 7, 0, 12, 4, 7]
-    """
+    """ PArpeggiator: Arpeggiator.
 
+        <type> can be one of:
+            PArp.UP
+            PArp.DOWN
+            PArp.UPDOWN
+            PArp.CONVERGE
+            PArp.DIVERGE
+            PArp.RANDOM
+
+        >>> p = PLoop(PArpeggiator(Chord.major, PArpeggiator.CONVERGE))
+        >>> p.nextn(16)
+        [0, 12, 4, 7, 0, 12, 4, 7, 0, 12, 4, 7, 0, 12, 4, 7]
+        """
     UP = 0
     DOWN = 1
     CONVERGE = 2
     DIVERGE = 3
     RANDOM = 4
     # Abnormal length patterns
     __LONGPATTERNS = 5
@@ -747,15 +677,15 @@
             # can alternatively specify a list of notes
             # ------------------------------------------------------------------------
             self._notes = self.chord
 
         self.restart()
 
     def __repr__(self):
-        return "PArpeggiator(%s, %s)" % (repr(self.chord), repr(self.type))
+        return ("PArpeggiator(%s, %s)" % (repr(self.chord), repr(self.type)))
 
     def get_notes(self):
         return self._notes
 
     def set_notes(self, notes: Iterable):
         self._notes = list(sorted(notes))
 
@@ -765,93 +695,61 @@
         self._notes = list(sorted(self._notes))
 
         if self.type == PArpeggiator.UP:
             self.offsets = list(range(len(self._notes)))
         elif self.type == PArpeggiator.DOWN:
             self.offsets = list(reversed(list(range(len(self._notes)))))
         elif self.type == PArpeggiator.CONVERGE:
-            self.offsets = [
-                (n // 2) if (n % 2 == 0) else (0 - (n + 1) // 2)
-                for n in range(len(self._notes))
-            ]
+            self.offsets = [(n // 2) if (n % 2 == 0) else (0 - (n + 1) // 2) for n in range(len(self._notes))]
         elif self.type == PArpeggiator.DIVERGE:
             if len(self._notes) % 2 == 0:
-                self.offsets = [
-                    (
-                        (len(self._notes) // 2 - 1) - (n // 2)
-                        if (n % 2 == 0)
-                        else (len(self._notes) // 2 + n // 2)
-                    )
-                    for n in range(len(self.notes))
-                ]
+                self.offsets = [(len(self._notes) // 2 - 1) - (n // 2) if (n % 2 == 0) else
+                                (len(self._notes) // 2 + n // 2) for n in range(len(self.notes))]
             else:
-                self.offsets = [
-                    (
-                        (len(self._notes) // 2 - 1) - (n // 2)
-                        if (n % 2 == 1)
-                        else (len(self._notes) // 2 + n // 2)
-                    )
-                    for n in range(len(self.notes))
-                ]
+                self.offsets = [(len(self._notes) // 2 - 1) - (n // 2) if (n % 2 == 1) else
+                                (len(self._notes) // 2 + n // 2) for n in range(len(self.notes))]
         elif self.type == PArpeggiator.RANDOM:
             self.offsets = list(range(len(self._notes)))
             self.rng.shuffle(self.offsets)
         # ------------------------------------------------------------------------
         # Abnormal length patterns
         # ------------------------------------------------------------------------
         elif self.type == PArpeggiator.UPDOWN:
             # Min length (for loop): 2
-            self.offsets = list(range(len(self._notes)))[:-1] + list(
-                reversed(list(range(len(self._notes))))
-            )
-            if self.loop and len(self._notes) > 1:
+            self.offsets = list(range(len(self._notes)))[:-1] + list(reversed(list(range(len(self._notes)))))
+            if (self.loop and len(self._notes) > 1):
                 # Remove the last element to prevent double notes
                 self.offsets = self.offsets[:-1]
         elif self.type == PArpeggiator.DOWNUP:
             # Min length (for loop): 2
-            self.offsets = list(reversed(list(range(len(self._notes)))))[:-1] + list(
-                range(len(self._notes))
-            )
-            if self.loop and len(self._notes) > 1:
+            self.offsets = list(reversed(list(range(len(self._notes)))))[:-1] + list(range(len(self._notes)))
+            if (self.loop and len(self._notes) > 1):
                 self.offsets = self.offsets[:-1]
         elif self.type == PArpeggiator.BUILD:
             # 0, 0, 1, 0, 1, 2, 0, 1, 2, 3, ...
             # Min length: 2
-            if len(self._notes) < 2:
+            if (len(self._notes) < 2):
                 raise ValueError("Arpeggiator type BUILD requires at least 2 notes")
-            self.offsets = list(
-                itertools.chain.from_iterable(
-                    [range(0, n + 1) for n in range(len(self._notes))]
-                )
-            )
+            self.offsets = list(itertools.chain.from_iterable([range(0, n + 1) for n in range(len(self._notes))]))
         elif self.type == PArpeggiator.BREAK:
             # n, n, n-1, n, n-1, n-2, n, n-1, n-2, n-3, ...
             # Min length: 2
-            if len(self._notes) < 2:
+            if (len(self._notes) < 2):
                 raise ValueError("Arpeggiator type BREAK requires at least 2 notes")
             self.offsets = list(
-                itertools.chain.from_iterable(
-                    [range(n - 1, -1, -1) for n in range(len(self._notes), -1, -1)]
-                )
-            )
+                itertools.chain.from_iterable([range(n - 1, -1, -1) for n in range(len(self._notes), -1, -1)]))
         elif self.type == PArpeggiator.ROOTBOUNCE:
             # 0, 1, 0, 2, ..., 0, n, 0, n - 1, ..., 0, 2, 0, 1, 0
             # Min length: 3
-            if len(self._notes) < 3:
-                raise ValueError(
-                    "Arpeggiator type ROOTBOUNCE requires at least 3 notes"
-                )
-            self.offsets = (
-                list(range(len(self._notes)))[1:-1] +
-                list(reversed(list(range(len(self._notes)))))[:-1]
-            )
+            if (len(self._notes) < 3):
+                raise ValueError("Arpeggiator type ROOTBOUNCE requires at least 3 notes")
+            self.offsets = list(range(len(self._notes)))[1:-1] + list(reversed(list(range(len(self._notes)))))[:-1]
             # Put a 0 in between every element of an UPDOWN pattern
-            for n in range(0, len(self.offsets) * 2 + 1, 2):
-                self.offsets.insert(n, 0)
-            if self.loop:
+            for n in range(0, len(self.offsets) * 2 + 1, 2): self.offsets.insert(n, 0)
+            if (self.loop):
                 # Remove the last three elements for a smooth loop
                 self.offsets = self.offsets[:-3]
         else:
             raise ValueError("Invalid Arpeggiator type: %s" % self.type)
 
     def reset(self):
         super().reset()
@@ -860,47 +758,45 @@
     def __next__(self):
         if len(self._notes) == 0:
             self.pos = 0
             return None
 
         pos = self.value(self.pos)
 
-        if pos < len(self.offsets) and (
-            pos < len(self._notes) or self.type > self.__LONGPATTERNS
-        ):
+        if pos < len(self.offsets) and (pos < len(self._notes) or self.type > self.__LONGPATTERNS):
             offset = self.offsets[pos]
             rv = self._notes[offset]
             self.pos = pos + 1
             return rv
         elif self.loop:
             self.pos = 0
             self.reset()
             return next(self)
         else:
             raise StopIteration
 
 
 class PEuclidean(Pattern):
-    """PEuclidean: Generate Euclidean rhythms.
-    Effectively tries to space <mod> events out evenly over `length` beats.
-    Events returned are either 1 or None (rest)
-
-    >>> p = PEuclidean(5, 8)
-    >>> p.nextn(8)
-    [1, None, 1, 1, None, 1, 1, None]
-    """
+    """ PEuclidean: Generate Euclidean rhythms.
+        Effectively tries to space <mod> events out evenly over `length` beats.
+        Events returned are either 1 or None (rest)
+
+        >>> p = PEuclidean(5, 8)
+        >>> p.nextn(8)
+        [1, None, 1, 1, None, 1, 1, None]
+        """
 
     def __init__(self, mod: int, length: int, phase: int = 0):
         self.mod = mod
         self.length = length
         self.sequence = []
         self.pos = phase
 
     def __repr__(self):
-        return "PEuclidean(%s, %s, %s)" % (self.mod, self.length, self.phase)
+        return ("PEuclidean(%s, %s, %s)" % (self.mod, self.length, self.phase))
 
     def __next__(self):
         length = self.value(self.length)
         mod = self.value(self.mod)
         sequence = self._euclidean(length, mod)
         if self.pos >= len(sequence):
             self.pos = 0
@@ -935,15 +831,15 @@
             return [a[n] + b[n] for n in range(len(a))] + b[len(a) - len(b):]
         elif len(b) < len(a):
             return [a[n] + b[n] for n in range(len(b))] + a[len(b) - len(a):]
         else:
             return [a[n] + b[n] for n in range(len(b))]
 
     def _euclidean(self, length, mod):
-        """Implements Bjorklund's algorithm, described in Toussaint (2005):
+        """ Implements Bjorklund's algorithm, described in Toussaint (2005):
         http://cgm.cs.mcgill.ca/~godfried/publications/banff.pdf
         """
 
         seqs = [(1,)] * mod + [(None,)] * (length - mod)
         seqs, remainder = self._split_remainder(seqs)
         while True:
             if len(remainder) <= 1:
@@ -951,43 +847,28 @@
             seqs = self._interleave(seqs, remainder)
             seqs, remainder = self._split_remainder(seqs)
 
         return reduce(lambda a, b: a + b, seqs + remainder)
 
 
 class PExplorer(Pattern):
-    def __init__(
-        self,
-        density: float = 0.5,
-        length: int = 4,
-        length_min: int = 2,
-        length_max: int = 6,
-        value_max: int = 12,
-        jump_max: int = 4,
-        loop: float = None,
-    ):
+    def __init__(self, density: float = 0.5, length: int = 4, length_min: int = 2, length_max: int = 6,
+                 value_max: int = 12, jump_max: int = 4, loop: float = None):
         self.density = density
         self.length = length
         self.length_min = length_min
         self.length_max = length_max
         self.value_max = value_max
         self.jump_max = jump_max
         self.loop = loop
         self.reset()
 
     def __repr__(self):
-        return "PExplorer(%s, %s, %s, %s, %s, %s, %s)" % (
-            self.density,
-            self.length,
-            self.length_min,
-            self.length_max,
-            self.value_max,
-            self.jump_max,
-            self.loop,
-        )
+        return ("PExplorer(%s, %s, %s, %s, %s, %s, %s)" % (
+            self.density, self.length, self.length_min, self.length_max, self.value_max, self.jump_max, self.loop))
 
     def reset(self):
         super().reset()
         self.counter = 0
         self.loop_pos = 0
         self.values = []
         self._generate_values()
@@ -1016,54 +897,33 @@
         OP_SWAP = 2
         OP_SPLIT = 3
         OP_REVERSE = 4
         OP_DELETE = 5
         OP_INSERT = 6
         OP_COPY = 7
 
-        OPERATION_NAMES = [
-            "mutate",
-            "rotate",
-            "swap",
-            "split",
-            "reverse",
-            "delete",
-            "insert",
-            "copy",
-        ]
+        OPERATION_NAMES = ["mutate", "rotate", "swap", "split", "reverse", "delete", "insert", "copy"]
 
         log.debug("PExplorer: Exploring: %s" % self.values)
-        operations = [
-            OP_MUTATE,
-            OP_ROTATE,
-            OP_SWAP,
-            OP_SPLIT,
-            OP_REVERSE,
-            OP_DELETE,
-            OP_INSERT,
-            OP_COPY,
-        ]
+        operations = [OP_MUTATE, OP_ROTATE, OP_SWAP, OP_SPLIT, OP_REVERSE, OP_DELETE, OP_INSERT, OP_COPY]
 
         values = self.values
         if len(values) >= self.length_max:
             operations.remove(OP_INSERT)
             operations.remove(OP_COPY)
         if len(values) <= self.length_min:
             operations.remove(OP_DELETE)
         operation = random.choice(operations)
         log.debug("PExplorer: Selected operation: %s" % OPERATION_NAMES[operation])
 
         # ------------------------------------------------------------------------
         # MUTATE: Replace a note with another note found within the sequence.
         # ------------------------------------------------------------------------
         if operation == OP_MUTATE:
-            filled_indices = [
-                n[0]
-                for n in filter(lambda n: n[1] is not None, list(enumerate(values)))
-            ]
+            filled_indices = [n[0] for n in filter(lambda n: n[1] is not None, list(enumerate(values)))]
             if len(filled_indices) > 0:
                 index = random.choice(filled_indices)
                 values[index] = random.randint(0, self.value_max)
 
         # ------------------------------------------------------------------------
         # ROTATE: Rotate the sequence forwards or backwards one slot.
         # ------------------------------------------------------------------------
@@ -1095,15 +955,15 @@
             values = list(reversed(values))
 
         # ------------------------------------------------------------------------
         # DELETE: Remove an item.
         # ------------------------------------------------------------------------
         elif operation == OP_DELETE:
             index = random.randrange(len(values))
-            del values[index]
+            del (values[index])
 
         # ------------------------------------------------------------------------
         # INSERT: Insert a new value at random.
         # ------------------------------------------------------------------------
         elif operation == OP_INSERT:
             index = random.randint(0, len(values))
             value = random.choice(list(range(self.value_max + 1)) + [None])
@@ -1135,32 +995,32 @@
 
         rv = self.values[self.counter]
         self.counter += 1
         return rv
 
 
 class PPermut(Pattern):
-    """PPermut: Generate every permutation of `count` input items.
+    """ PPermut: Generate every permutation of `count` input items.
 
-    >>> p = PPermut(PSeq([ 1, 11, 111, 1111 ]), 4)
-    >>> p.nextn(16)
-    [1, 11, 111, 1111, 1, 11, 1111, 111, 1, 111, 11, 1111, 1, 111, 1111, 11]
-    """
+        >>> p = PPermut(PSeq([ 1, 11, 111, 1111 ]), 4)
+        >>> p.nextn(16)
+        [1, 11, 111, 1111, 1, 11, 1111, 111, 1, 111, 11, 1111, 1, 111, 1111, 11]
+        """
 
     def __init__(self, input: Pattern, count: int = 8):
         if not hasattr(input, "__next__"):
             raise ValueError("Input to PPermut must be a Pattern or other iterator")
         self.input = input
         self.count = count
         self.pos = sys.maxsize
         self.permindex = sys.maxsize
         self.permutations = []
 
     def __repr__(self):
-        return "PPermut(%s, %s)" % (repr(self.input), self.count)
+        return ("PPermut(%s, %s)" % (repr(self.input), self.count))
 
     def reset(self):
         super().reset()
         self.pos = sys.maxsize
         self.permindex = sys.maxsize
         self.permutations = []
 
@@ -1189,26 +1049,26 @@
 
         rv = self.permutations[self.permindex][self.pos]
         self.pos += 1
         return rv
 
 
 class PPatternGeneratorAction(Pattern):
-    """PPatternGeneratorAction: Each time its pattern is exhausted, request a new pattern by calling <fn>.
+    """ PPatternGeneratorAction: Each time its pattern is exhausted, request a new pattern by calling <fn>.
 
-    >>>
-    >>>
-    """
+        >>>
+        >>>
+        """
 
     def __init__(self, fn: Callable):
         self.fn = fn
         self.pattern = self.fn()
 
     def __repr__(self):
-        return "PPatternGeneratorAction(%s)" % repr(self.fn)
+        return ("PPatternGeneratorAction(%s)" % repr(self.fn))
 
     def __next__(self):
         try:
             return next(self.pattern)
         except StopIteration:
             self.pattern = self.fn()
             # if not self.pattern:
@@ -1219,34 +1079,30 @@
             return next(self)
 
 
 PDecisionPoint = PPatternGeneratorAction
 
 
 class PSequenceAction(Pattern):
-    """PSequenceAction: Iterate over an array, perform a function, and repeat.
+    """ PSequenceAction: Iterate over an array, perform a function, and repeat.
 
-    >>>
-    >>>
-    """
+        >>>
+        >>>
+        """
 
     def __init__(self, list: Iterable, fn: Callable, repeats: int = sys.maxsize):
         self.list = list
         self.list_orig = list
         self.sequence = PSequence(self.list, 1)
         self.fn = fn
         self.repeats = repeats
         self.repeat_counter = 0
 
     def __repr__(self):
-        return "PSequenceAction(%s, %s, %s)" % (
-            repr(self.list),
-            repr(self.fn),
-            self.repeats,
-        )
+        return ("PSequenceAction(%s, %s, %s)" % (repr(self.list), repr(self.fn), self.repeats))
 
     def reset(self):
         super().reset()
         self.list = self.list_orig
         self.sequence = PSequence(self.list, 1)
         self.repeat_counter = 0
 
@@ -1268,15 +1124,15 @@
         self.notes = notes
         self.repeats = repeats
         self.rests = rests
         self.note_index = 0
         self.note_offset = 0
 
     def __repr__(self):
-        return "PMetropolis(%s, %s, %s)" % (repr(self.notes), self.repeats, self.rests)
+        return ("PMetropolis(%s, %s, %s)" % (repr(self.notes), self.repeats, self.rests))
 
     def __next__(self):
         repeats = self.repeats
         if len(repeats) < len(self.notes):
             repeats = repeats * int(math.ceil(len(self.notes) / len(repeats)))
         rests = self.rests
         if len(rests) < len(self.notes):
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/static.py` & `isobar_ext-0.9.0/isobar_ext/pattern/static.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 from . import Pattern
 
 
 class Globals:
     """
     The Globals class encapsulates a namespace of global variables that can be accessed
     throughout isobar_ext. This is particularly useful to alter parameters shared across the
@@ -22,15 +23,15 @@
         Returns:
             The value, which can be of any type.
 
         Raises:
             KeyError: If the key does not exist in the globals dict.
         """
         if key not in Globals.dict:
-            raise KeyError("Global variable does not exist: %s" % key)
+            raise KeyError(f"Global variable does not exist: {key}")
         value = Globals.dict[key]
         return Pattern.value(value)
 
     @classmethod
     def set(cls, key, value=None):
         """
         Set global parameters.
@@ -48,26 +49,26 @@
                     callback(key, value)
         else:
             Globals.dict[key] = value
             for callback in Globals.on_change_callbacks:
                 callback(key, value)
 
     @classmethod
-    def add_on_change_callback(self, callback):
+    def add_on_change_callback(cls, callback):
         Globals.on_change_callbacks.append(callback)
 
 
 class PGlobals(Pattern):
     """PGlobals: Static global value identified by a string."""
 
     def __init__(self, name: str):
         self.name = name
 
     def __repr__(self):
-        return "PGlobals(%s)" % repr(self.name)
+        return f"PGlobals({repr(self.name)})"
 
     def __next__(self):
         name = Pattern.value(self.name)
         value = Globals.get(name)
         return Pattern.value(value)
 
 
@@ -76,31 +77,28 @@
         self.pattern = pattern
         self.value = None
         self.element_duration = element_duration
         self.current_element_start_time = None
         self.current_element_duration = None
 
     def __repr__(self):
-        return "PStaticPattern(%s, %s)" % (
-            repr(self.pattern),
-            repr(self.element_duration),
-        )
+        return f"PStaticPattern({repr(self.pattern)}, {repr(self.element_duration)})"
 
     def __next__(self):
         timeline = self.timeline
         if timeline is None:
             raise Exception(
                 "Cannot query current timeline outside of a scheduled event context"
             )
         current_time = round(timeline.current_time, 5)
 
         while (
-            self.current_element_start_time is None or
-            current_time - self.current_element_start_time >=
-            self.current_element_duration
+                self.current_element_start_time is None or
+                current_time - self.current_element_start_time >=
+                self.current_element_duration
         ):
             self.value = Pattern.value(self.pattern)
             self.current_element_start_time = round(timeline.current_time, 5)
             self.current_element_duration = Pattern.value(self.element_duration)
 
         return self.value
 
@@ -115,16 +113,8 @@
         return "PCurrentTime()"
 
     def __next__(self):
         beats = self.get_beats()
         return round(beats, 5)
 
     def get_beats(self):
-        # ------------------------------------------------------------------------
-        # using the specified timeline (if given) or the currently-embedded
-        # timeline (otherwise), return the current position in current_time.
-        # ------------------------------------------------------------------------
-        timeline = self.timeline
-        if timeline:
-            return timeline.current_time
-
-        return 0
+        return timeline.current_time if (timeline := self.timeline) else 0
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/tonal.py` & `isobar_ext-0.9.0/isobar_ext/pattern/tonal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from __future__ import annotations
-from .core import Pattern
-from ..scale import Scale
-from ..util import midi_note_to_frequency, midi_semitones_to_frequency_ratio
 
 import typing
 from typing import Iterable
 
+from .core import Pattern
+from .series import PSeries
+from ..key import Key
+from ..scale import Scale
+from ..util import midi_note_to_frequency, midi_semitones_to_frequency_ratio
+
 
 class PDegree(Pattern):
     """PDegree: Map scale index <degree> to MIDI notes in <scale>.
 
     >>> p = PDegree(PSeries(0, 1), Scale.major)
     >>> p.nextn(16)
     [0, 2, 4, 5, 7, 9, 11, 12, 14, 16, 17, 19, 21, 23, 24, 26]
@@ -36,15 +39,15 @@
                 if isinstance(item, list)
                 else 0 if item is None else item
             )
             for item in lst
         ]
 
     def __repr__(self):
-        return "PDegree(%s, %s)" % (repr(self.degree), repr(self.scale))
+        return f"PDegree({repr(self.degree)}, {repr(self.scale)})"
 
     def __next__(self):
         degree = Pattern.value(self.degree)
         scale = Pattern.value(self.scale)
         if degree is None:
             return None
 
@@ -67,23 +70,24 @@
     """
 
     def __init__(self, pattern: Pattern, key: Iterable):
         self.pattern = pattern
         self.key = key
 
     def __repr__(self):
-        return "PFilterByKey(%s, %s)" % (repr(self.pattern), repr(self.key))
+        return f"PFilterByKey({repr(self.pattern)}, {repr(self.key)})"
 
     def __next__(self):
         note = Pattern.value(self.pattern)
         key = Pattern.value(self.key)
-        if note in key:
-            return note
-        else:
-            return None
+        return note if note in key else None
+
+
+class PNearestNoteKey:
+    pass
 
 
 class PNearestNoteInKey(Pattern):
     """PNearestNoteInKey: Return the nearest note in <key>.
 
     >>> p = PNearestNoteKey(PSeries(0, 1), Key("C", "major"))
     >>> p.nextn(16)
@@ -93,50 +97,46 @@
     abbreviation = "pnearestnote"
 
     def __init__(self, pattern: Pattern, key: Iterable):
         self.pattern = pattern
         self.key = key
 
     def __repr__(self):
-        return "PNearestNoteInKey(%s, %s)" % (repr(self.pattern), repr(self.key))
+        return f"PNearestNoteInKey({repr(self.pattern)}, {repr(self.key)})"
 
     def __next__(self):
         note = Pattern.value(self.pattern)
         key = Pattern.value(self.key)
         return key.nearest_note(note)
 
 
 class PMidiNoteToFrequency(Pattern):
     """PMidiNoteToFrequency: Map MIDI note to frequency value."""
 
     abbreviation = "pnotetofreq"
 
-    def __init__(self, input):
-        self.input = input
+    def __init__(self, v_input):
+        self.input = v_input
 
     def __repr__(self):
-        return "PMidiNoteToFrequency(%s)" % repr(self.input)
+        return f"PMidiNoteToFrequency({repr(self.input)})"
 
     def __next__(self):
         note = Pattern.value(self.input)
-        if note is None:
-            return None
-        return midi_note_to_frequency(note)
+        return None if note is None else midi_note_to_frequency(note)
 
 
 class PMidiSemitonesToFrequencyRatio(Pattern):
     """PMidiSemitonesToFrequencyRatio: Map a MIDI offet in semitones to a frequency ratio.
     e.g. 0 -> 1.0
          12 -> 2.0
          7 -> 1.5
     """
 
     abbreviation = "psemistofreq"
 
-    def __init__(self, input):
-        self.input = input
+    def __init__(self, v_input):
+        self.input = v_input
 
     def __next__(self):
         note = Pattern.value(self.input)
-        if note is None:
-            return None
-        return midi_semitones_to_frequency_ratio(note)
+        return None if note is None else midi_semitones_to_frequency_ratio(note)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/pattern/warp.py` & `isobar_ext-0.9.0/isobar_ext/pattern/warp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
-from .core import Pattern
 
 import math
 
+from .chance import PWhite
+from .core import Pattern
+
 
 class PWarp(Pattern):
     pass
 
 
 class PWInterpolate(PWarp):
     """PWInterpolate: Requests a new target warp value from `pattern` every `length` beats
@@ -21,15 +23,15 @@
         self.length = length
         self.pattern = pattern
         self.pos = self.length
         self.value = 0.0
         self.dv = 0.0
 
     def __repr__(self):
-        return "PWInterpolate(%s, %s)" % (repr(self.pattern), self.length)
+        return f"PWInterpolate({repr(self.pattern)}, {self.length})"
 
     def __next__(self):
         rv = self.value
 
         # ------------------------------------------------------------------------
         # keep ticking until we have reached our period (length, in beats)
         # TODO: querying self.timeline is very inefficient, find a better way
@@ -41,35 +43,39 @@
 
             # ------------------------------------------------------------------------
             # in case our length parameter is also a pattern: obtain a scalar value.
             # dv is used for linear interpolation until the next target reached.
             # ------------------------------------------------------------------------
             length = Pattern.value(self.length)
             self.dv = (self.target - self.value) / (
-                self.timeline.ticks_per_beat * length
+                    self.timeline.ticks_per_beat * length
             )
 
         self.value = self.value + self.dv
 
         return rv
 
 
+class PWAmp:
+    pass
+
+
 class PWSine(PWarp):
     """PWSine: Sinosoidal warp, period `length` beats, amplitude +/-<amp>.
 
     >>> p = PWAmp(8, 0.5)
     """
 
     def __init__(self, length: int = 1, amp: float = 0.5):
         self.length = length
         self.amp = amp
         self.pos = 0.0
 
     def __repr__(self):
-        return "PWSine(%s, %s)" % (self.length, self.amp)
+        return f"PWSine({self.length}, {self.amp})"
 
     def __next__(self):
         self.pos += self.timeline.tick_duration
         if self.pos > self.length:
             self.pos -= self.length
 
         # normalize to [0, 1]
@@ -91,15 +97,15 @@
         self.amp = amp
         self.pos = 0.0
         self.value = 1.0
         self.length_cur = -1.0
         self.dv = None
 
     def __repr__(self):
-        return "PWRallantando(%s, %s)" % (self.length, self.amp)
+        return f"PWRallantando({self.length}, {self.amp})"
 
     def __next__(self):
         rv = self.value
 
         # ------------------------------------------------------------------------
         # Need to round to avoid Python rounding errors
         # (eg 0.99999 < 1 when multiplying 1/24.0 by 24)
@@ -114,9 +120,8 @@
             rate_end = 1.0 + amp_cur
             steps = self.timeline.ticks_per_beat * self.length_cur
             self.dv = math.exp(math.log(rate_end / rate_start) / steps)
 
         self.pos += self.timeline.tick_duration
         self.value = self.value * self.dv
 
-        rv = math.log(rv, 2)
-        return rv
+        return math.log(rv, 2)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/scale.py` & `isobar_ext-0.9.0/isobar_ext/scale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from .util import normalize
-from .exceptions import UnknownScaleName
-import random
 import json
+import random
 from pathlib import Path
 
+from .exceptions import UnknownScaleName
+from .util import normalize
+
 
 class Scale(object):
     dict = {}
+
     # _scales = []
 
     def __init__(
-        self, semitones=None, name="unnamed scale", octave_size=12, semitones_down=None
+            self, semitones=None, name="unnamed scale", octave_size=12, semitones_down=None
     ):
         self.scale_down = False
 
         if semitones is None:
             semitones = [0, 2, 4, 5, 7, 9, 11]
         self.semitones = semitones
         self.semitones_down = semitones_down
@@ -30,36 +32,34 @@
         scale_instance = cls(semitones=semitones, name=name, octave_size=octave_size, semitones_down=semitones_down)
         # cls._scales.append(scale_instance)
         setattr(cls, name, scale_instance)
         cls.dict[name] = scale_instance
         return scale_instance
 
     def __str__(self):
-        return "%s %s" % (self.name, self.semitones)
+        return f"{self.name} {self.semitones}"
 
     def __getitem__(self, key):
         return self.get(key)
 
     def __eq__(self, other):
         return (
-            self.semitones == other.semitones and self.octave_size == other.octave_size
+                self.semitones == other.semitones and self.octave_size == other.octave_size
         )
 
     def __contains__(self, semitone):
         return (semitone % self.scale.octave_size) in self.semitones
 
     def __hash__(self):
         return hash(
-            tuple(
-                (
-                    tuple(self.semitones),
-                    tuple(self.weights),
-                    self.name,
-                    self.octave_size,
-                )
+            (
+                tuple(self.semitones),
+                tuple(self.weights),
+                self.name,
+                self.octave_size,
             )
         )
 
     def get(self, *args, **kwargs):
         """Retrieve the n'th degree of this scale."""
         parameters = {"n": None, "scale_down": False}
         if hasattr(self, "scale_down"):
@@ -83,16 +83,15 @@
         )
         octave = n // len(semitones)
         degree = n % len(semitones)
         semitone = semitones[degree]
         return (self.octave_size * octave) + semitone
 
     def copy(self):
-        other = Scale(self.semitones, self.name)
-        return other
+        return Scale(self.semitones, self.name)
 
     def change(self):
         """Exchange two random elements of this scale."""
         i = random.randint(0, len(self.semitones) - 1)
         j = random.randint(0, len(self.semitones) - 1)
         if i != j:
             tmp = self.semitones[i]
@@ -132,18 +131,17 @@
 
         index += degree
         return index
 
     @staticmethod
     def fromnotes(notes, name="unnamed scale", octave_size=12):
         notes = [note % octave_size for note in notes]
-        notes = list(dict((k, k) for k in notes).keys())
+        notes = list({k: k for k in notes}.keys())
         notes = sorted(notes)
-        scale = Scale(notes, name=name, octave_size=octave_size)
-        return scale
+        return Scale(notes, name=name, octave_size=octave_size)
 
     @staticmethod
     def all():
         return list(Scale.dict.values())
 
     @staticmethod
     def byname(name):
@@ -153,14 +151,15 @@
             raise UnknownScaleName()
 
     @staticmethod
     def random():
         key = random.choice(list(Scale.dict.keys()))
         return Scale.dict[key]
 
+
 # ------------------------------------------------------------------------
 current_directory = Path(__file__).resolve().parent
 config_file = current_directory / "scales.json"
 
 with open(config_file, "r") as file:
     scales = json.load(file)
 
@@ -178,47 +177,47 @@
 Scale.chromatic = Scale([0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11], "chromatic")
 Scale.major = Scale([0, 2, 4, 5, 7, 9, 11], "major")
 Scale.default = Scale.major
 
 
 class WeightedScale(Scale):
     def __init__(
-        self,
-        semitones=[0, 2, 4, 5, 7, 9, 11],
-        weights=[1 / 7.0] * 7,
-        name="major",
-        octave_size=12,
+            self,
+            semitones=None,
+            weights=None,
+            name="major",
+            octave_size=12,
     ):
         Scale.__init__(self, semitones, name=name, octave_size=octave_size)
+        if weights is None:
+            weights = [1 / 7.0] * 7
+        if semitones is None:
+            semitones = [0, 2, 4, 5, 7, 9, 11]
         self.weights = weights
+        self.semitones = semitones
         if name not in Scale.dict:
             Scale.dict[name] = self
 
     def __str__(self):
-        return "%s %s weights = %s" % (self.name, self.semitones, self.weights)
+        return f"{self.name} {self.semitones} weights = {self.weights}"
 
     @staticmethod
     def fromnotes(notes, name="unnamed scale", octave_size=12):
         note_sequence = [note % octave_size for note in notes]
         notes_dict = {}
         for note in note_sequence:
             if note not in notes_dict:
                 notes_dict[note] = 0
             notes_dict[note] += 1.0 / len(note_sequence)
 
-        notes_unique = list(dict((k, k) for k in note_sequence).keys())
+        notes_unique = list({k: k for k in note_sequence}.keys())
         notes_unique = sorted(notes_unique)
-        weights = []
-        for note in notes_unique:
-            weights.append(notes_dict[note])
-
-        scale = WeightedScale(notes_unique, weights, name=name, octave_size=octave_size)
-        return scale
+        weights = [notes_dict[note] for note in notes_unique]
+        return WeightedScale(notes_unique, weights, name=name, octave_size=octave_size)
 
     @staticmethod
     def fromorder(notes, name="unnamed scale", octave_size=12):
         notes = [note % octave_size for note in notes]
         weights = [len(notes) - n for n in range(len(notes))]
         weights = normalize(weights)
 
-        scale = WeightedScale(notes, weights, name=name, octave_size=octave_size)
-        return scale
+        return WeightedScale(notes, weights, name=name, octave_size=octave_size)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/shorthand/abbreviations.py` & `isobar_ext-0.9.0/isobar_ext/shorthand/abbreviations.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
 from ..pattern import PSaw as psaw  # noqa: F401
 from ..pattern import PScalar as pscalar  # noqa: F401
 from ..pattern import PScaleLinExp as pscalelinexp  # noqa: F401
 from ..pattern import PScaleLinLin as pscalelinlin  # noqa: F401
 from ..pattern import PSeq as pseq  # noqa: F401
 from ..pattern import PSequence as pseq  # noqa: F401
 from ..pattern import PSequenceAction as psequenceaction  # noqa: F401
-from ..pattern import PSeries as pseries  # noqa: F401
 from ..pattern import PShuffle as pshuffle  # noqa: F401
 from ..pattern import PShuffleInput as pshuffleinput  # noqa: F401
 from ..pattern import PSkip as pskip  # noqa: F401
 from ..pattern import PSkipIf as pskipif  # noqa: F401
 from ..pattern import PStaticPattern as pstaticpattern  # noqa: F401
 from ..pattern import PStochasticPattern as pstochasticpattern  # noqa: F401
 from ..pattern import PStutter as pstutter  # noqa: F401
```

### Comparing `isobar_ext-0.5.1/isobar_ext/shorthand/notation.py` & `isobar_ext-0.9.0/isobar_ext/notation/notation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+
 from ..pattern.sequence import PSequence
 
 
 def _parser_push(obj, sequence: PSequence, depth: int):
     """
     Append an item to the (possibly nested) PSequence.
     """
@@ -15,23 +16,21 @@
 
 
 def _parser_get_next_token(string: str):
     """
     Return the next token in the string.
     This may be a number (integer/float) or a note name (e.g. c#4).
     """
-    note_pattern = r"(-?[0-9]+(\.[0-9]+)?|[a-g]#?[0-9])\b"
     if string[0] in "[]":
         return string[0]
+    note_pattern = r"(-?[0-9]+(\.[0-9]+)?|[a-g]#?[0-9])\b"
+    if match := re.match(note_pattern, string):
+        return match[1]
     else:
-        match = re.match(note_pattern, string)
-        if match:
-            return match.group(1)
-        else:
-            raise ValueError("Invalid character in notation: %s" % string)
+        raise ValueError(f"Invalid character in notation: {string}")
 
 
 def _parser_token_to_value(token: str):
     try:
         return int(token)
     except ValueError:
         try:
@@ -45,15 +44,15 @@
     Parses a string into a (possibly nested) PSequence.
     For example:
 
         parse_notation('1 2 [10 11] [20 [30 31 32]]')
 
     results in
 
-        seq([1, 2, seq([10, 11]), seq([20, seq([30, 31, 32])])])])
+        seq([1, 2, seq([10, 11]), seq([20, seq([30, 31, 32])])])
 
     Implementation of a push-down automaton, thanks to:
     Source: https://stackoverflow.com/questions/4284991/parsing-nested-parentheses-in-python-grab-content-by-level
     """
     groups = PSequence([])
     depth = 0
 
@@ -70,16 +69,16 @@
                 _parser_push(value, groups, depth)
 
             string = string[len(token):]
             string = string.lstrip()
 
             if len(string) == 0:
                 break
-    except IndexError:
-        raise ValueError("Notation error: parenthesis mismatch")
+    except IndexError as e:
+        raise ValueError("Notation error: parenthesis mismatch") from e
 
     if depth > 0:
         raise ValueError("Notation error: parenthesis mismatch")
     else:
         return groups
```

### Comparing `isobar_ext-0.5.1/isobar_ext/shorthand/patches.py` & `isobar_ext-0.9.0/isobar_ext/shorthand/patches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from signalflow import *  # noqa: F403
 import os
 
+from signalflow import *  # noqa: F403
+
 
 class SegmentPlayerPatch(Patch):
     def __init__(
-        self,
-        buf,
-        onsets,
-        volume=0.5,
-        hpf=10,
-        lpf=20000,
-        delay=0.0,
-        feedback=0.0,
-        pan=0.0,
-        index=0,
-        rate=1.0,
+            self,
+            buf,
+            onsets,
+            volume=0.5,
+            hpf=10,
+            lpf=20000,
+            delay=0.0,
+            feedback=0.0,
+            pan=0.0,
+            index=0,
+            rate=1.0,
     ):
         super().__init__()
         index = self.add_input("index", index)
         rate = self.add_input("rate", rate)
         pan = self.add_input("pan", pan)
         volume = self.add_input("volume", volume)
         hpf = self.add_input("hpf", hpf)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/shorthand/sync.py` & `isobar_ext-0.9.0/isobar_ext/shorthand/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from signalflow import *  # noqa: F403
+
 from .setup import track, timeline
 
 
 def start_sync_test():
     """
     Play metronome audio from SignalFlow and MIDI outputs, to help with
     establishing audio sync between the two. Latency of the SignalFlow output
```

### Comparing `isobar_ext-0.5.1/isobar_ext/timelines/clock.py` & `isobar_ext-0.9.0/isobar_ext/timelines/clock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
+import logging
+import random
+import threading
+import time
+from typing import Any
+
 from ..constants import (
     DEFAULT_TEMPO,
     DEFAULT_TICKS_PER_BEAT,
     MIN_CLOCK_DELAY_WARNING_TIME,
 )
 from ..util import make_clock_multiplier
 
-import time
-import random
-import logging
-import threading
-from typing import Any
-
 logger = logging.getLogger(__name__)
 
 
 class Clock:
     def __init__(
-        self,
-        clock_target: Any = None,
-        tempo: float = DEFAULT_TEMPO,
-        ticks_per_beat: int = DEFAULT_TICKS_PER_BEAT,
+            self,
+            clock_target: Any = None,
+            tempo: float = DEFAULT_TEMPO,
+            ticks_per_beat: int = DEFAULT_TICKS_PER_BEAT,
     ):
         """
         A Clock generates tick events at a regular interval, defined by the `ticks_per_beat` property.
         The higher the number of ticks per beat, the finer the granularity events can be triggered.
 
         Different clocking systems vary in their granularity, typically specified in ticks per beat (crotchet),
         aka "pulses per quarter note", PPQN:
```

### Comparing `isobar_ext-0.5.1/isobar_ext/timelines/clock_link.py` & `isobar_ext-0.9.0/isobar_ext/timelines/clock_link.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-from ..constants import (   # noqa: F401
+import os
+import sys
+import time
+from typing import Any
+
+from .clock import Clock
+from ..constants import (  # noqa: F401
     DEFAULT_TEMPO,
     DEFAULT_TICKS_PER_BEAT,
     MIN_CLOCK_DELAY_WARNING_TIME,
 )
-from .clock import Clock
-import time
-import sys
-import os
-from typing import Any
 
 try:
     lib_dir = "auxiliary/lib"
     current_dir = os.path.dirname(os.path.abspath(__file__))
     lib_dir_abs = os.path.normpath(
         os.path.join(current_dir, os.path.pardir, os.path.pardir, lib_dir)
     )
     sys.path.insert(0, lib_dir)
     sys.path.insert(0, lib_dir_abs)
     import link
 except ModuleNotFoundError as e:
-    print(e)
     pass
 
 
 class AbletonLinkClock(Clock):
     def __init__(
-        self,
-        clock_target: Any = None,
-        tempo: float = DEFAULT_TEMPO,
-        ticks_per_beat: int = DEFAULT_TICKS_PER_BEAT,
+            self,
+            clock_target: Any = None,
+            tempo: float = DEFAULT_TEMPO,
+            ticks_per_beat: int = DEFAULT_TICKS_PER_BEAT,
     ):
         self.link_client = link.Link(120)
         self.link_client.enabled = True
         self.link_client.startStopSyncEnabled = True
         self.link_client.setTempoCallback(self.tempo_changed_callback)
 
         super().__init__(clock_target, tempo, ticks_per_beat)
 
-    def tempo_changed_callback(self, tempo):
+    @staticmethod
+    def tempo_changed_callback(tempo):
         print("tempo changed: %.2f" % tempo)
 
     def run(self):
         ticks_previous = None
         got_sync = False
 
         while True:
```

### Comparing `isobar_ext-0.5.1/isobar_ext/timelines/event.py` & `isobar_ext-0.9.0/isobar_ext/timelines/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from ..pattern import Pattern
-from ..scale import Scale
-from ..key import Key
-from ..constants import *  # noqa: F403
-from ..exceptions import InvalidEventException
 import logging
-from typing import Iterable
 import warnings
+from typing import Iterable
+
+from ..constants import *  # noqa: F403
+from ..exceptions import InvalidEventException
+from ..key import Key
+from ..pattern import Pattern
+from ..scale import Scale
 
 log = logging.getLogger(__name__)
 
 
 class EventDefaults:
     def __init__(self):
         default_values = {
@@ -36,19 +37,19 @@
         for key in event_values.keys():
             if key not in ALL_EVENT_PARAMETERS:
                 raise ValueError(f"Invalid key for event: {key}")
 
         parm = list({EVENT_NOTE, EVENT_ACTION, EVENT_DEGREE} & set(event_values))
         if len(parm) >= 2:
             warning_msg = f"Cannot specify both '{parm[0]}' and '{parm[1]}.'"
-            if EVENT_ACTION in (parm):
+            if EVENT_ACTION in parm:
                 warning_msg += (
-                    "\nEVENT_ACTION disables EVENT_NOTE and EVENT_DEGREE.\n" +
-                    "Use separate timeline.schedule for EVENT_ACTION" +
-                    " and separate for EVENT_NOTE or EVENT_DEGREE"
+                        "\nEVENT_ACTION disables EVENT_NOTE and EVENT_DEGREE.\n" +
+                        "Use separate timeline.schedule for EVENT_ACTION" +
+                        " and separate for EVENT_NOTE or EVENT_DEGREE"
                 )
             warnings.warn(warning_msg, Warning)
 
         if EVENT_DURATION_LEGACY in event_values:
             event_values[EVENT_DURATION] = event_values[EVENT_DURATION_LEGACY]
         if EVENT_AMPLITUDE_LEGACY in event_values:
             event_values[EVENT_AMPLITUDE] = event_values[EVENT_AMPLITUDE_LEGACY]
@@ -144,20 +145,20 @@
             # ----------------------------------------------------------------------
             self.patch = event_values[EVENT_PATCH]
             self.output = None
 
             if EVENT_TYPE in event_values:
                 self.type = event_values[EVENT_TYPE]
             elif type(self.patch).__name__ == "PatchSpec" or isinstance(
-                self.patch, type
+                    self.patch, type
             ):
                 self.type = EVENT_TYPE_PATCH_CREATE
             elif (
-                hasattr(self.patch, "trigger_node") and
-                self.patch.trigger_node is not None
+                    hasattr(self.patch, "trigger_node") and
+                    self.patch.trigger_node is not None
             ):
                 self.type = EVENT_TYPE_PATCH_TRIGGER
             else:
                 self.type = EVENT_TYPE_PATCH_SET
 
             if EVENT_PATCH_OUTPUT in event_values:
                 self.output = event_values[EVENT_PATCH_OUTPUT]
@@ -229,8 +230,8 @@
             )
 
         self.duration = event_values[EVENT_DURATION]
         self.active = event_values[EVENT_ACTIVE]
         self.fields = event_values
 
     def __str__(self):
-        return "Event (%s)" % self.fields
+        return f"Event ({self.fields})"
```

### Comparing `isobar_ext-0.5.1/isobar_ext/timelines/timeline.py` & `isobar_ext-0.9.0/isobar_ext/timelines/timeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,48 @@
-import math
 import copy
-import time
 import logging
+import math
 import threading
+import time
 import traceback
-from typing import Callable, Any, Optional, Union
+from collections.abc import Iterable
 from dataclasses import dataclass
+from functools import partial
+from typing import Callable, Any, Optional, Union
 
-from .track import Track
 from .clock import Clock
 from .event import EventDefaults
-from ..io import MidiOutputDevice, OutputDevice
-from ..constants import DEFAULT_TICKS_PER_BEAT, DEFAULT_TEMPO
+from .track import Track
+from ..constants import (DEFAULT_TICKS_PER_BEAT, DEFAULT_TEMPO, EVENT_ACTION, EVENT_ACTION_ARGS, EVENT_DURATION)
 from ..constants import INTERPOLATION_NONE
 from ..exceptions import (
     TrackLimitReachedException,
     TrackNotFoundException,
     MultipleOutputDevicesException,
 )
+from ..io import MidiOutputDevice, OutputDevice
+from ..pattern import PSequence
 from ..util import make_clock_multiplier
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class Action:
     time: float
     function: Callable
 
 
 class Timeline:
-    def __init__(
-        self,
-        tempo: float = DEFAULT_TEMPO,
-        output_device: Any = None,
-        clock_source: Any = None,
-        ticks_per_beat: int = DEFAULT_TICKS_PER_BEAT,
-    ):
+    def __init__(self,
+                 tempo: float = DEFAULT_TEMPO,
+                 output_device: Any = None,
+                 clock_source: Any = None,
+                 ticks_per_beat: int = DEFAULT_TICKS_PER_BEAT,
+                 ):
         """
         A Timeline object encapsulates a number of Tracks, each of which
         represents a sequence of note or control events.
 
         Timing is driven by a `clock_source`, which can be a real-time Clock object, or an
         external source such as a `MidiInputDevice` clock.
 
@@ -139,18 +141,15 @@
         """
         Query how many ticks are expected per beat.
         This varies based on the resolution of the clock source.
 
         Returns:
             The number of ticks per beat.
         """
-        if self.clock_source:
-            return self.clock_source.ticks_per_beat
-        else:
-            return None
+        return self.clock_source.ticks_per_beat if self.clock_source else None
 
     def set_ticks_per_beat(self, ticks_per_beat: int):
         """
         Set the number of ticks per beat.
 
         Args:
             ticks_per_beat: The new number of ticks per beat. This can be set for internal clocks, but \
@@ -252,89 +251,91 @@
 
         # --------------------------------------------------------------------------------
         # Copy self.actions because removing from it whilst using it = bad idea.
         # Perform actions before tracks are executed because an event might
         # include scheduling a quantized track, which should then be
         # immediately evaluated.
         # --------------------------------------------------------------------------------
-        for action in self.actions[:]:
+        aligned_actions = []
+        for idx, action in enumerate(self.actions[:]):
             # --------------------------------------------------------------------------------
             # The only event we currently get in a Timeline are add_track events
             #  -- which have a function object associated with them.
             #
             # Round to work around rounding errors.
             # http://docs.python.org/tutorial/floatingpoint.html
             # --------------------------------------------------------------------------------
+            if isinstance(action, dict):
+                action = Action(*action.values())
+                # self.actions[idx] = action
             if round(action.time, 8) <= round(self.current_time, 8):
                 action.function()
                 self.actions.remove(action)
-
+            else:
+                aligned_actions.append(action)
+                # self.actions.remove(action)
+        self.actions = aligned_actions
         # --------------------------------------------------------------------------------
         # Copy self.tracks because removing from it whilst using it = bad idea
         # --------------------------------------------------------------------------------
         for track in self.tracks[:]:
             try:
                 track.tick()
             except Exception as e:  # noqa: F841 (but we don't care if it's not used)
-                if self.ignore_exceptions:
-                    tb = traceback.format_exc()
-                    log.warning("*** Exception in track: %s" % tb)
-                    self.tracks.remove(track)
-                else:
+                if not self.ignore_exceptions:
                     raise
+                tb = traceback.format_exc()
+                log.warning(f"*** Exception in track: {tb}")
+                self.tracks.remove(track)
             if track.is_finished and track.remove_when_done:
                 self.tracks.remove(track)
                 log.info(
                     "Timeline: Track finished, removing from scheduler (total tracks: %d)"
                     % len(self.tracks)
                 )
 
         # --------------------------------------------------------------------------------
         # If we've run out of notes, raise a StopIteration.
         # --------------------------------------------------------------------------------
-        if len(self.tracks) == 0 and len(self.actions) == 0 and self.stop_when_done:
+        if len(self.tracks) == 0 and not self.actions and self.stop_when_done:
             # TODO: Don't do this if we've never played any events, e.g.
             #       right after calling timeline.start(). Should at least
             #       wait for some events to happen first.
             raise StopIteration
 
         # --------------------------------------------------------------------------------
         # Tell our output devices to move forward a step.
         # --------------------------------------------------------------------------------
         for device in self.output_devices:
             clock_multiplier = self.clock_multipliers[device]
             ticks = next(clock_multiplier)
 
-            for tick in range(ticks):
+            for _ in range(ticks):
                 device.tick()
 
         # --------------------------------------------------------------------------------
         # Increment beat count according to our current tick_length.
         # --------------------------------------------------------------------------------
         self.current_time += self.tick_duration
 
     def dump(self):
         """
         Output a summary of this Timeline object to stdout.
         """
         print(
-            "Timeline (clock: %s, tempo %s)"
-            % (
-                self.clock_source,
-                self.clock_source.tempo if self.clock_source.tempo else "unknown",
-            )
+            f'Timeline (clock: {self.clock_source}, tempo {self.clock_source.tempo or "unknown"})'
         )
 
         print((" - %d devices" % len(self.output_devices)))
         for device in self.output_devices:
-            print(("   - %s" % device))
+            print(f"   - {device}")
 
         print((" - %d tracks" % len(self.tracks)))
         for tracks in self.tracks:
-            print(("   - %s" % tracks))
+            print(f"   - {tracks}")
 
     def reset_to_beat(self):
         """
         Reset the timer to the last beat.
         Useful when a MIDI Stop/Reset message is received, or otherwise to re-establish beat sync.
         """
 
@@ -365,14 +366,15 @@
         """
         Run this Timeline in the foreground.
 
         Args:
             stop_when_done: If set, returns when no tracks are currently \
                             scheduled; otherwise, keeps running indefinitely.
         """
+
         if stop_when_done is not None:
             self.stop_when_done = stop_when_done
 
         try:
             # --------------------------------------------------------------------------------
             # Start the clock. This might internal (eg a Clock object, running on
             # an independent thread), or external (eg a MIDI clock).
@@ -386,15 +388,15 @@
             # --------------------------------------------------------------------------------
             # This will be hit if every Pattern in a timeline is exhausted.
             # --------------------------------------------------------------------------------
             log.info("Timeline: Finished")
             self.running = False
 
         except Exception as e:
-            print((" *** Exception in Timeline thread: %s" % e))
+            print(f" *** Exception in Timeline thread: {e}")
             if not self.ignore_exceptions:
                 raise e
 
     def start(self) -> None:
         """
         Starts the timeline running in the background.
         """
@@ -454,31 +456,29 @@
     """ The device that events are sent to. """
 
     def add_output_device(self, output_device: OutputDevice) -> None:
         """
         Append a new output device to the timeline's device list.
         """
         self.output_devices.append(output_device)
-        self.clock_multipliers[output_device] = make_clock_multiplier(
-            output_device.ticks_per_beat, self.ticks_per_beat
-        )
+        self.clock_multipliers[output_device] = make_clock_multiplier(output_device.ticks_per_beat, self.ticks_per_beat)
 
-    def schedule(
-        self,
-        params: dict = None,
-        quantize: float = None,
-        delay: float = 0,
-        count: Optional[int] = None,
-        interpolate: str = INTERPOLATION_NONE,
-        output_device: Any = None,
-        remove_when_done: bool = True,
-        name: Optional[str] = None,
-        replace: bool = False,
-        track_index: Optional[int] = None,
-    ) -> Track:
+    def schedule(self,
+                 params: dict = None,
+                 quantize: float = None,
+                 delay: float = 0,
+                 count: Optional[int] = None,
+                 interpolate: str = INTERPOLATION_NONE,
+                 output_device: Any = None,
+                 remove_when_done: bool = True,
+                 name: Optional[str] = None,
+                 replace: bool = False,
+                 track_index: Optional[int] = None,
+                 sel_track_idx: Optional[int] = None
+                 ) -> Track:
         """
         Schedule a new track within this Timeline.
 
         Args:
             params (dict):           Event dictionary. Keys are generally EVENT_* values, defined in constants.py. \
                                      If params is None, a new empty Track will be scheduled and returned. \
                                      This can be updated with Track.update(). \
@@ -498,15 +498,16 @@
             name (str):              Optional name to identify the Track. If given, can be used to update the track's
                                      parameters in future calls to schedule() by specifying replace=True.
             replace (bool):          Must be used in conjunction with the `name` parameter. Instead of scheduling a \
                                      new Track, this updates the parameters of an existing track with the same name.
             track_index (int):       When specified, inserts the Track at the given index.
                                      This can be used to set the priority of an event and ensure that it happens
                                      before another Track is evaluted, used in (e.g.) Track.update().
-
+            sel_track_idx (int):     Track index to use for event arguments (default: None). This says about midinote
+                                    track schedule us assigned to
         Returns:
             The new `Track` object.
 
         Raises:
             TrackLimitReachedException: If `max_tracks` has been reached.
         """
         if output_device is None:
@@ -514,65 +515,147 @@
             # If no output device exists, send to the system default MIDI output.
             # --------------------------------------------------------------------------------
             if len(self.output_devices) == 0:
                 self.add_output_device(MidiOutputDevice())
             output_device = self.output_devices[0]
 
         # --------------------------------------------------------------------------------
+        # This is to ensure EVENT_ACTION split 1 element [1:]
+        # --------------------------------------------------------------------------------
+        if not params:
+            params_list = [{}]
+        elif isinstance(params, list):
+            params_list = params
+        else:
+            params_list = [params]
+
+        tracks_list = []
+        params_list2 = []
+        event_args = {}
+        for param in params_list:
+            if not isinstance(param, dict) and not isinstance(param, Iterable):
+                param = dict(param)
+            if isinstance(param, dict):
+                action_fun = param.get(EVENT_ACTION, None)
+                event_args = param.get(EVENT_ACTION_ARGS, {})
+            else:
+                action_fun, event_args = None, {}
+
+            if action_fun and isinstance(action_fun, Iterable):
+                attributes1 = vars(action_fun)
+                # Get the attributes used by the class constructor
+                constructor_attributes = list(PSequence.__init__.__code__.co_varnames[1:])
+
+                # Filter the modified attributes to include only those used by the constructor
+                attributes = {k: v for k, v in attributes1.copy().items() if
+                              k in constructor_attributes}
+                attributes2 = {k: v for k, v in attributes1.copy().items() if
+                               k in constructor_attributes}
+                action_fun2 = [
+                                  partial(f, self) if isinstance(f, partial) else f
+                                  for f in copy.copy(action_fun)
+                              ][:1]
+                attributes2['sequence'] = action_fun2
+                action_fun2 = PSequence(**attributes2)
+                params2 = copy.copy(param)
+                params2[EVENT_ACTION] = action_fun2
+                if bool(event_args):
+                    params2[EVENT_ACTION_ARGS] = event_args
+                dur2 = list(params2.pop(EVENT_DURATION, None))
+
+                if dur2:
+                    params2[EVENT_DURATION] = PSequence(dur2[:1], repeats=1)
+                params_list2.append(params2)
+
+                action_fun = [partial(f, self) if isinstance(f, partial) else f for f in copy.copy(action_fun)][1:]
+                attributes['sequence'] = action_fun
+                action_fun = PSequence(**attributes)
+                param[EVENT_ACTION] = action_fun
+                if event_args:
+                    param[EVENT_ACTION_ARGS] = event_args
+
+                dur = list(param.pop(EVENT_DURATION, None))
+
+                if dur:
+                    param["delay"] = dur[0]
+                    param[EVENT_DURATION] = PSequence(dur[1:], repeats=1)
+
+            elif action_fun:
+                param[EVENT_ACTION] = action_fun
+                if bool(event_args):
+                    param[EVENT_ACTION_ARGS] = event_args
+
+            params_list2.append(param)
+
+        # --------------------------------------------------------------------------------
         # If replace=True is specified, updated the params of any existing track
         # with the same name. If none exists, proceed to create it as usual.
         # --------------------------------------------------------------------------------
-        if replace:
-            if name is None:
-                raise ValueError("Must specify a track name if `replace` is specified")
-            for existing_track in self.tracks:
-                if existing_track.name == name:
-                    existing_track.update(params, quantize=quantize, delay=delay)
-                    # TODO: Add unit test around this
+        for param in params_list2:
+            extra_delay = param.pop("delay", None) if isinstance(param, dict) else None
+            if replace:
+                if name is None:
+                    raise ValueError("Must specify a track name if `replace` is specified")
+                for existing_track in self.tracks:
+                    if existing_track.name == name:
+                        existing_track.update(param,
+                                              quantize=quantize,
+                                              delay=delay,
+                                              interpolate=interpolate)
+                    # TODO: Add unit test for update interpolate
+                    # TODO: Add unit test around this (returning the track?)
                     return existing_track
 
-        if self.max_tracks and len(self.tracks) >= self.max_tracks:
-            raise TrackLimitReachedException(
-                "Timeline: Refusing to schedule track (hit limit of %d)"
-                % self.max_tracks
-            )
-
-        if isinstance(params, Track):
-            track = params
-            track.reset()
-        else:
-            # --------------------------------------------------------------------------------
-            # Take a copy of params to avoid modifying the original
-            # --------------------------------------------------------------------------------
-            track = Track(
-                self,
-                max_event_count=count,
-                interpolate=interpolate,
-                output_device=output_device,
-                remove_when_done=remove_when_done,
-                name=name,
-            )
-
-            track.update(copy.copy(params), quantize=quantize, delay=delay)
+            if self.max_tracks and len(self.tracks) >= self.max_tracks:
+                raise TrackLimitReachedException(
+                    "Timeline: Refusing to schedule track (hit limit of %d)" % self.max_tracks)
+
+            def start_track(track_int):
+                # --------------------------------------------------------------------------------
+                # Add a new track.
+                # --------------------------------------------------------------------------------
+                if track_index is not None:
+                    self.tracks.insert(track_index, track_int)
+                else:
+                    self.tracks.append(track_int)
+                log.info("Timeline: Scheduled new track (total tracks: %d)" % len(self.tracks))
 
-            # --------------------------------------------------------------------------------
-            # Add a new track.
-            # --------------------------------------------------------------------------------
-            if track_index is not None:
-                self.tracks.insert(track_index, track)
+            if not bool(event_args) and sel_track_idx is not None:
+                # if not bool(event_args):
+                event_args = {"track_idx": sel_track_idx}
+                if not bool(param.get(EVENT_ACTION_ARGS, {})):
+                    param[EVENT_ACTION_ARGS] = event_args
+
+            if isinstance(param, Track):
+                track = param
+                track.reset()
             else:
-                self.tracks.append(track)
+                # --------------------------------------------------------------------------------
+                # Take a copy of params to avoid modifying the original
+                # --------------------------------------------------------------------------------
+                track = Track(
+                    self,
+                    max_event_count=count,
+                    interpolate=interpolate,
+                    output_device=output_device,
+                    remove_when_done=remove_when_done,
+                    name=name
+                )
 
-            log.info(
-                "Timeline: Scheduled new track (total tracks: %d)" % len(self.tracks)
-            )
+                track.update(copy.copy(param), quantize=quantize, delay=delay or extra_delay)
+            tracks_list.append(track)
 
-            # TODO:
-            #  - Add test for added_latency_seconds
-            #  - Add test for defaults
+            start_track(track)
+
+        if len(tracks_list) > 1:
+            track = tracks_list
+        elif len(tracks_list) == 1:
+            track = tracks_list[0]
+        else:
+            track = None
 
         return track
 
     # --------------------------------------------------------------------------------
     # Backwards-compatibility
     # --------------------------------------------------------------------------------
     sched = schedule
@@ -588,15 +671,15 @@
             TrackNotFoundException: If the track is not playing.
         """
         if track not in self.tracks:
             raise TrackNotFoundException("Track is not currently scheduled")
         self.tracks.remove(track)
 
     def _schedule_action(
-        self, function: Callable, quantize: float = 0.0, delay: float = 0.0
+            self, function: Callable, quantize: float = 0.0, delay: float = 0.0
     ) -> None:
         """
         Schedule a function to be called at the given time offset.
 
         Args:
             function: The function to call
             quantize: The quantization level, in beats
@@ -619,18 +702,15 @@
 
         Returns:
             The Track object, or None if not found.
         """
         if isinstance(track_id, int):
             return self.tracks[track_id]
         elif isinstance(track_id, str):
-            for track in self.tracks:
-                if track.name == track_id:
-                    return track
-            return None
+            return next((track for track in self.tracks if track.name == track_id), None)
         else:
             raise TypeError("Invalid type for track_id (must be an int or str)")
 
     def clear(self) -> None:
         """
         Remove all tracks.
         """
```

### Comparing `isobar_ext-0.5.1/isobar_ext/timelines/track.py` & `isobar_ext-0.9.0/isobar_ext/timelines/track.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 from __future__ import annotations
 
+import contextlib
 import copy
 import inspect
 from dataclasses import dataclass
 from typing import Union, Optional, Callable, TYPE_CHECKING
 
 from .event import Event
 
 if TYPE_CHECKING:
     from .timeline import Timeline
-from ..pattern import Pattern, PSequence, PDict, PInterpolate
+from ..pattern import Pattern, PSequence, PDict, PInterpolate, PConstant
 from ..constants import *  # noqa: F403
 from ..exceptions import InvalidEventException
 from ..util import midi_note_to_frequency
 from ..io.output import OutputDevice
 import logging
 
 log = logging.getLogger(__name__)
 
 
 @dataclass
 class NoteOffEvent:
     timestamp: float
     note: int
     channel: int
+    track_idx: int
+
+
+def get_track_idx(event_obj):
+    if isinstance(event_obj, (dict, PDict)):
+        if trk_idx := event_obj.get('args', {}).get('track_idx', None):
+            return trk_idx.constant if isinstance(trk_idx, PConstant) else trk_idx
+    return 0
 
 
 class Track:
     def __init__(
             self,
             timeline: Timeline,
             max_event_count: Optional[int] = None,
@@ -35,26 +44,27 @@
             output_device: Optional[OutputDevice] = None,
             remove_when_done: bool = True,
             name: Optional[str] = None,
     ):
         """
         Args:
             timeline: The Timeline object that the track inhabits
-            events: A dict, a PDict, or a Pattern that generates dicts.
             max_event_count: Optionally, the maximum number of events that will be executed. \
                              The Track will finish automatically once this number of events is complete.
             interpolate: Optional interpolation to impose on values, particularly for control tracks.
             output_device: Optional output device. Defaults to the Timeline's default_output_device.
             remove_when_done: If True, removes the Track from the Timeline when it finishes.
             name: Optional name for the track. If specified, can be used to update tracks in place by specifying \
                   its name when scheduling events on the Timeline.
         """
         # --------------------------------------------------------------------------------
         # Ensure that events is a pattern that generates a dict when it is iterated.
         # --------------------------------------------------------------------------------
+        # self.ss_track_idx = None
+        # self.track_idx = None
         self.event_stream: Pattern = PDict({})
         self.timeline: Timeline = timeline
         self.current_time: float = 0.0
         self.next_event_time: float = sys.maxsize
         self.max_event_count: int = max_event_count
         self.current_event_count: int = 0
         self.name: str = name
@@ -69,16 +79,17 @@
         self.note_offs: list[NoteOffEvent] = []
         self.is_muted: bool = False
         self.is_started: bool = False
         self.is_finished: bool = False
         self.remove_when_done: bool = remove_when_done
         self.on_event_callbacks: list[Callable] = []
 
-    def __getattr__(self, item):
-        return self.event_stream[item]
+    def __getattr__(self, item, default=None):
+        # return self.event_stream[item]
+        return getattr(self.event_stream, 'item', default)
 
     def __setattr__(self, item, value):
         # --------------------------------------------------------------------------------
         # Benign magic so that you can do things like
         #
         #    track.note = 64
         #
@@ -113,14 +124,15 @@
             events: A dict, a PDict, or a Pattern that generates dicts.
         """
         if events is None:
             events = {}
         if isinstance(events, dict):
             events = PDict(events)
         self.event_stream = events
+        # self.ss_track_idx = get_track_idx(self.event_stream)
 
         self.is_started = True
         self.current_time = 0.0
         self.next_event_time = self.current_time
 
     def update(
             self,
@@ -179,27 +191,71 @@
     def process_note_offs(self):
         # ----------------------------------------------------------------------
         # Process note_offs before we play the next note, else a repeated note
         # with gate = 1.0 will immediately be cancelled.
         #
         # Use round() to avoid scheduling issues arising from rounding errors.
         # ----------------------------------------------------------------------
+        # if self.event_stream['args']['track_idx'].constant is not None:
+        # if isinstance(self.event_stream, dict) and self.event_stream.get('args', {}).get('track_idx', None) is not None:
+        #
+        #     track_idx = self.event_stream['args']['track_idx'].constant
+        # else:
+        #     track_idx = 0
+        # if getattr(self, 'track_idx', None) is None:
+        if (
+                not hasattr(self, 'track_idx')
+                or getattr(self, 'track_idx', None) is None
+        ):
+            track_idx = get_track_idx(self.event_stream)
+            self.track_idx = track_idx
+        else:
+            track_idx = self.track_idx
+        # track_idx = self.ss_track_idx
+
         for note_off in self.note_offs[:]:
             if round(note_off.timestamp, 8) <= round(self.current_time, 8):
-                self.output_device.note_off(note_off.note, note_off.channel)
+                self.output_device.note_off(note_off.note, note_off.channel, track_idx=track_idx)
                 self.note_offs.remove(note_off)
 
     def tick(self):
         """
         Step forward one tick.
         """
 
         if not self.is_started:
             return
+        # ----------------------------------------------------------------------
+        # Process note_offs before we play the next note, else a repeated note
+        # with gate = 1.0 will immediately be cancelled.
+        # ----------------------------------------------------------------------
+        # if self.event_stream['args']['track_idx'].constant is not None:
+
+        # track_idx = 0
+        # if isinstance(self.event_stream, PDict):
+        #     # if self.event_stream.get('args', {}).get('track_idx', {}).get('constant', None) is not None:
+        #     if self.event_stream.get('args', {}).get('track_idx', None) is not None:
+        #         track_idx = self.event_stream['args']['track_idx'].constant
+        # if getattr(self, 'track_idx', None) is None:
+        if (
+                not hasattr(self, 'track_idx')
+                or getattr(self, 'track_idx', None) is None
+        ):
+            track_idx = get_track_idx(self.event_stream)
+            self.track_idx = track_idx
+        else:
+            track_idx = self.track_idx
 
+        for note in self.note_offs[:]:
+            if round(note.timestamp, 8) <= round(self.current_time, 8):
+                index = note.note
+                channel = note.channel
+                self.output_device.note_off(index, channel, track_idx=track_idx)
+                # if self.note_offs:
+                self.note_offs.remove(note)
         try:
             if self.interpolate is INTERPOLATION_NONE:
                 if round(self.current_time, 8) >= round(self.next_event_time, 8):
                     while round(self.current_time, 8) >= round(self.next_event_time, 8):
                         # --------------------------------------------------------------------------------
                         # Retrieve the next event.
                         # If no more events are available, this raises StopIteration.
@@ -221,85 +277,88 @@
                 try:
                     interpolated_values = next(self.interpolating_event)
                     interpolated_event = Event(
                         interpolated_values, self.timeline.defaults, track=self
                     )
                     self.perform_event(interpolated_event)
                 except StopIteration:
-                    is_first_event = False
-                    if self.next_event is None:
-                        # --------------------------------------------------------------------------------
-                        # The current and next events are needed to perform interpolation.
-                        # No events have yet been obtained, so query the current and next events off
-                        # the stack.
-                        # --------------------------------------------------------------------------------
-                        self.next_event = self.get_next_event()
-                        is_first_event = True
+                    self._extracted_from_tick_65()
+        except StopIteration:
+            if len(self.note_offs) == 0:
+                self.is_finished = True
 
-                    self.current_event = self.next_event
-                    self.next_event = self.get_next_event()
+        self.current_time += self.tick_duration
 
-                    # --------------------------------------------------------------------------------
-                    # Special case to handle zero-duration events: continue to pop new
-                    # events from the pattern.
-                    # --------------------------------------------------------------------------------
-                    while (
-                            int(self.current_event.duration * self.timeline.ticks_per_beat) <=
-                            0
-                    ):
-                        self.current_event = self.next_event
-                        self.next_event = self.get_next_event()
-
-                    if (
-                            self.current_event.type != EVENT_TYPE_CONTROL or
-                            self.next_event.type != EVENT_TYPE_CONTROL
-                    ):
-                        raise InvalidEventException(
-                            "Interpolation is only valid for control event"
-                        )
+    # TODO Rename this here and in `tick`
+    def _extracted_from_tick_65(self):
+        is_first_event = False
+        if self.next_event is None:
+            # --------------------------------------------------------------------------------
+            # The current and next events are needed to perform interpolation.
+            # No events have yet been obtained, so query the current and next events off
+            # the stack.
+            # --------------------------------------------------------------------------------
+            self.next_event = self.get_next_event()
+            is_first_event = True
 
-                    interpolating_event_fields = copy.copy(self.current_event.fields)
-                    duration = self.current_event.duration
-                    duration_ticks = duration * self.timeline.ticks_per_beat
-                    for key, value in self.current_event.fields.items():
-                        # --------------------------------------------------------------------------------
-                        # Create a new interpolating_event with patterns for each parameter to
-                        # interpolate.
-                        # --------------------------------------------------------------------------------
-                        if key == EVENT_TYPE or key == EVENT_DURATION:
-                            continue
-                        if type(value) is not float and type(value) is not int:
-                            continue
-                        interpolating_event_fields[key] = PInterpolate(
-                            PSequence(
-                                [
-                                    self.current_event.fields[key],
-                                    self.next_event.fields[key],
-                                ],
-                                1,
-                            ),
-                            duration_ticks,
-                            self.interpolate,
-                        )
+        self.current_event = self.next_event
+        self.next_event = self.get_next_event()
 
-                    self.interpolating_event = PDict(interpolating_event_fields)
-                    if not is_first_event:
-                        next(self.interpolating_event)
-                    event = Event(
-                        next(self.interpolating_event),
-                        self.timeline.defaults,
-                        track=self,
-                    )
-                    self.perform_event(event)
+        # --------------------------------------------------------------------------------
+        # Special case to handle zero-duration events: continue to pop new
+        # events from the pattern.
+        # --------------------------------------------------------------------------------
+        while (
+                int(self.current_event.duration * self.timeline.ticks_per_beat) <=
+                0
+        ):
+            self.current_event = self.next_event
+            self.next_event = self.get_next_event()
 
-        except StopIteration:
-            if len(self.note_offs) == 0:
-                self.is_finished = True
+        if (
+                self.current_event.type != EVENT_TYPE_CONTROL or
+                self.next_event.type != EVENT_TYPE_CONTROL
+        ):
+            raise InvalidEventException(
+                "Interpolation is only valid for control event"
+            )
 
-        self.current_time += self.tick_duration
+        interpolating_event_fields = copy.copy(self.current_event.fields)
+        duration = self.current_event.duration
+        duration_ticks = duration * self.timeline.ticks_per_beat
+        for key, value in self.current_event.fields.items():
+            # --------------------------------------------------------------------------------
+            # Create a new interpolating_event with patterns for each parameter to
+            # interpolate.
+            # --------------------------------------------------------------------------------
+            if key in [EVENT_TYPE, EVENT_DURATION]:
+                continue
+            if type(value) is not float and type(value) is not int:
+                continue
+            interpolating_event_fields[key] = PInterpolate(
+                PSequence(
+                    [
+                        self.current_event.fields[key],
+                        self.next_event.fields[key],
+                    ],
+                    1,
+                ),
+                duration_ticks,
+                self.interpolate,
+            )
+
+        self.interpolating_event = PDict(interpolating_event_fields)
+        if not is_first_event:
+            next(self.interpolating_event)
+        event = Event(
+            next(self.interpolating_event),
+            self.timeline.defaults,
+            track=self,
+        )
+        self.perform_event(event)
 
     def reset_to_beat(self):
         """
         Reset the track's time to the nearest integer.
         """
         self.current_time = round(self.current_time)
 
@@ -307,19 +366,16 @@
         """
         Rewind to the beginning of the pattern.
         """
         self.current_time = 0
         self.next_event_time = self.current_time
 
         for pattern in self.event_stream.values():
-            try:
+            with contextlib.suppress(AttributeError):
                 pattern.reset()
-            except AttributeError:
-                # Event stream may contain constant values, in which case no reset is needed.
-                pass
 
     def get_next_event(self) -> Event:
         """
         Retrieve the next event from the event stream dict.
 
         Returns:
             The next Event object
@@ -349,115 +405,320 @@
         event_values = copy.copy(event_values)
 
         event = Event(event_values, self.timeline.defaults, track=self)
         self.current_event_count += 1
 
         return event
 
+    # def perform_event(self, event: Event):
+    #     if not event.active:
+    #         return
+    #     if self.is_muted:
+    #         return
+    #
+    #     # ------------------------------------------------------------------------
+    #     # Action: Carry out an action each time this event is triggered
+    #     # ------------------------------------------------------------------------
+    #     if event.type == EVENT_TYPE_ACTION:
+    #         try:
+    #             fn = event.action
+    #             try:
+    #                 fn_params = inspect.signature(fn).parameters
+    #                 for key in event.args.keys():
+    #                     if key not in fn_params:
+    #                         raise Exception(
+    #                             "Named argument not found in callback args: %s" % key
+    #                         )
+    #             except ValueError:
+    #                 # ------------------------------------------------------------------------
+    #                 # inspect.signature does not work on cython/pybind11 bindings, and
+    #                 # raises a ValueError. In these cases, simply pass the arguments
+    #                 # without validation.
+    #                 # ------------------------------------------------------------------------
+    #                 pass
+    #             event.action(**event.args)
+    #         except StopIteration:
+    #             raise StopIteration()
+    #         except Exception as e:
+    #             print("Exception when handling scheduled action: %s" % e)
+    #             import traceback
+    #
+    #             traceback.print_exc()
+    #             pass
+    #
+    #     # ------------------------------------------------------------------------
+    #     # Control: Send a control value
+    #     # ------------------------------------------------------------------------
+    #     elif event.type == EVENT_TYPE_CONTROL:
+    #         log.debug(
+    #             "Control (channel %d, control %d, value %d)",
+    #             event.channel,
+    #             event.control,
+    #             event.value,
+    #         )
+    #         self.output_device.control(event.control, event.value, event.channel)
+    #
+    #     # ------------------------------------------------------------------------
+    #     # Program change
+    #     # ------------------------------------------------------------------------
+    #     elif event.type == EVENT_TYPE_PROGRAM_CHANGE:
+    #         log.debug(
+    #             "Program change (channel %d, program %d)",
+    #             event.channel,
+    #             event.program_change,
+    #         )
+    #         self.output_device.program_change(event.program_change, event.channel)
+    #
+    #     # ------------------------------------------------------------------------
+    #     # address: Send a value to an OSC endpoint
+    #     # ------------------------------------------------------------------------
+    #     elif event.type == EVENT_TYPE_OSC:
+    #         self.output_device.send(event.osc_address, event.osc_params)
+    #
+    #     # ------------------------------------------------------------------------
+    #     # SuperCollider synth
+    #     # ------------------------------------------------------------------------
+    #     elif event.type == EVENT_TYPE_SUPERCOLLIDER:
+    #         self.output_device.create(event.synth_name, event.synth_params)
+    #
+    #     # ------------------------------------------------------------------------
+    #     # SignalFlow patch
+    #     # ------------------------------------------------------------------------
+    #     elif event.type == EVENT_TYPE_PATCH_CREATE:
+    #         # ------------------------------------------------------------------------
+    #         # Action: Create patch
+    #         # ------------------------------------------------------------------------
+    #         if not hasattr(self.output_device, "create"):
+    #             raise InvalidEventException(
+    #                 "Device %s does not support this kind of event" % self.output_device
+    #             )
+    #         params = dict(
+    #             (key, Pattern.value(value)) for key, value in event.params.items()
+    #         )
+    #         if hasattr(event, "note"):
+    #             notes = event.note if hasattr(event.note, "__iter__") else [event.note]
+    #
+    #             for note in notes:
+    #                 if note > 0:
+    #                     # TODO: Should use None to denote rests
+    #                     params["frequency"] = midi_note_to_frequency(note)
+    #                     self.output_device.create(
+    #                         event.patch, params, output=event.output
+    #                     )
+    #         else:
+    #             self.output_device.create(event.patch, params, output=event.output)
+    #
+    #     elif (
+    #             event.type == EVENT_TYPE_PATCH_SET or event.type == EVENT_TYPE_PATCH_TRIGGER
+    #     ):
+    #         # ------------------------------------------------------------------------
+    #         # Action: Set patch's input(s) and/or trigger an event
+    #         # ------------------------------------------------------------------------
+    #         for key, value in event.params.items():
+    #             value = Pattern.value(value)
+    #             event.patch.set_input(key, value)
+    #
+    #         if hasattr(event, "note"):
+    #             event.patch.set_input("frequency", midi_note_to_frequency(event.note))
+    #
+    #         if event.type == EVENT_TYPE_PATCH_TRIGGER:
+    #             # ------------------------------------------------------------------------
+    #             # Action: Trigger a patch
+    #             # ------------------------------------------------------------------------
+    #             if not hasattr(self.output_device, "trigger"):
+    #                 raise InvalidEventException(
+    #                     "Device %s does not support this kind of event"
+    #                     % self.output_device
+    #                 )
+    #             params = dict(
+    #                 (key, Pattern.value(value)) for key, value in event.params.items()
+    #             )
+    #             self.output_device.trigger(
+    #                 event.patch, event.trigger_name, event.trigger_value
+    #             )
+    #
+    #     # ------------------------------------------------------------------------
+    #     # Note: Classic MIDI note
+    #     # ------------------------------------------------------------------------
+    #     elif event.type == EVENT_TYPE_NOTE:
+    #         # ----------------------------------------------------------------------
+    #         # event: Certain devices (eg Socket IO) handle generic events,
+    #         #        rather than note_on/note_off. (Should probably have to
+    #         #        register for this behaviour rather than happening magically...)
+    #         # ----------------------------------------------------------------------
+    #         if hasattr(self.output_device, "event") and callable(
+    #                 getattr(self.output_device, "event")
+    #         ):
+    #             d = copy.copy(event)
+    #             for key, value in list(d.items()):
+    #                 # ------------------------------------------------------------------------
+    #                 # Turn non-builtin objects into their string representations.
+    #                 # We don't want to call repr() on numbers as it turns them into strings,
+    #                 # which we don't want to happen in our resultant JSON.
+    #                 # TODO: There absolutely must be a way to do this for all objects which are
+    #                 #       non-builtins... ie, who are "class" instances rather than "type".
+    #                 #
+    #                 #       We could check dir(__builtins__), but for some reason, __builtins__ is
+    #                 #       different here than it is outside of a module!?
+    #                 #
+    #                 #       Instead, go with the lame option of listing "primitive" types.
+    #                 # ------------------------------------------------------------------------
+    #                 if type(value) not in (int, float, bool, str, list, dict, tuple):
+    #                     value = repr(value)
+    #                     d[key] = value
+    #
+    #             self.output_device.event(d)
+    #             return
+    #
+    #         # ----------------------------------------------------------------------
+    #         # note_on: Standard (MIDI) type of device
+    #         # ----------------------------------------------------------------------
+    #         # if type(event.amplitude) is tuple or event.amplitude > 0:
+    #         if type(event.amplitude) is tuple or True:
+    #             # TODO: pythonic duck-typing approach might be better
+    #             # TODO: doesn't handle arrays of amp, channel event, etc
+    #             notes = event.note if hasattr(event.note, "__iter__") else [event.note]
+    #
+    #             # ----------------------------------------------------------------------
+    #             # Allow for arrays of amp, gate etc, to handle chords properly.
+    #             # Caveat: Things will go horribly wrong for an array of amp/gate event
+    #             # shorter than the number of notes.
+    #             # ----------------------------------------------------------------------
+    #             for index, note in enumerate(notes):
+    #                 amp = (
+    #                     event.amplitude[index]
+    #                     if isinstance(event.amplitude, tuple)
+    #                     else event.amplitude
+    #                 )
+    #                 channel = (
+    #                     event.channel[index]
+    #                     if isinstance(event.channel, tuple)
+    #                     else event.channel
+    #                 )
+    #                 gate = (
+    #                     event.gate[index]
+    #                     if isinstance(event.gate, tuple)
+    #                     else event.gate
+    #                 )
+    #                 # TODO: Add an EVENT_SUSTAIN that allows absolute note lengths to be specified
+    #
+    #                 # if (amp is not None and amp > 0) and (gate is not None and gate > 0):
+    #                 if (amp is not None) and (gate is not None):
+    #                     self.output_device.note_on(note, amp, channel)
+    #
+    #                     note_dur = event.duration * gate
+    #                     note_off_time = self.current_time + note_dur
+    #                     note_off = NoteOffEvent(note_off_time, note, channel)
+    #                     self.note_offs.append(note_off)
+    #             if event.pitchbend is not None:
+    #                 self.output_device.pitch_bend(event.pitchbend, channel)
+    #     else:
+    #         raise InvalidEventException("Invalid event type: %s" % event.type)
+    #
+    #     if self.timeline.on_event_callback:
+    #         self.timeline.on_event_callback(self, event)
+    #
+    #     if self.on_event_callbacks:
+    #         for callback in self.on_event_callbacks:
+    #             callback(event)
+
     def perform_event(self, event: Event):
+
+        # if isinstance(self.event_stream, PDict) and self.event_stream.get('args', {}).get('track_idx', {'constant': None}).constant is not None:
+        # if getattr(isinstance(self.event_stream, PDict) and self.event_stream.get('args', {}).get('track_idx'), 'constant', None) is not None:
+        # if getattr(isinstance(self.event_stream, PDict) and self.event_stream.get('args', {}).get('track_idx', None), 'constant', None) is not None:
+        #
+        #     track_idx = self.event_stream['args']['track_idx'].constant
+        # if getattr(self, 'track_idx', None) is None:
+        if (
+                not hasattr(self, 'track_idx')
+                or getattr(self, 'track_idx', None) is None
+        ):
+            track_idx = get_track_idx(self.event_stream)
+            self.track_idx = track_idx
+        else:
+            track_idx = self.track_idx
+        # if not (track_idx := get_track_idx(self.event_stream)):
+        if track_idx is None and getattr(event, 'fields', {}).get('args', {}).get('track_idx') is not None:
+            track_idx = event.fields['args']['track_idx']
+            self.track_idx = track_idx
+        # else:
+        #     track_idx = 0
+
         if not event.active:
             return
         if self.is_muted:
             return
 
         # ------------------------------------------------------------------------
         # Action: Carry out an action each time this event is triggered
         # ------------------------------------------------------------------------
         if event.type == EVENT_TYPE_ACTION:
             try:
                 fn = event.action
-                try:
+                with contextlib.suppress(ValueError):
                     fn_params = inspect.signature(fn).parameters
                     for key in event.args.keys():
                         if key not in fn_params:
-                            raise Exception(
-                                "Named argument not found in callback args: %s" % key
-                            )
-                except ValueError:
-                    # ------------------------------------------------------------------------
-                    # inspect.signature does not work on cython/pybind11 bindings, and
-                    # raises a ValueError. In these cases, simply pass the arguments
-                    # without validation.
-                    # ------------------------------------------------------------------------
-                    pass
+                            raise Exception(f"Named argument not found in callback args: {key}")
                 event.action(**event.args)
             except StopIteration:
                 raise StopIteration()
             except Exception as e:
-                print("Exception when handling scheduled action: %s" % e)
+                print(f"Exception when handling scheduled action: {e}")
                 import traceback
 
                 traceback.print_exc()
-                pass
-
-        # ------------------------------------------------------------------------
-        # Control: Send a control value
-        # ------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_CONTROL:
             log.debug(
                 "Control (channel %d, control %d, value %d)",
                 event.channel,
                 event.control,
                 event.value,
             )
-            self.output_device.control(event.control, event.value, event.channel)
+            self.output_device.control(event.control, event.value, event.channel, track_idx=track_idx)
 
-        # ------------------------------------------------------------------------
-        # Program change
-        # ------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_PROGRAM_CHANGE:
             log.debug(
                 "Program change (channel %d, program %d)",
                 event.channel,
                 event.program_change,
             )
-            self.output_device.program_change(event.program_change, event.channel)
+            self.output_device.program_change(event.program_change, event.channel, track_idx=track_idx)
 
-        # ------------------------------------------------------------------------
-        # address: Send a value to an OSC endpoint
-        # ------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_OSC:
-            self.output_device.send(event.osc_address, event.osc_params)
+            self.output_device.send(event.osc_address, event.osc_params, track_idx=track_idx)
 
-        # ------------------------------------------------------------------------
-        # SuperCollider synth
-        # ------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_SUPERCOLLIDER:
             self.output_device.create(event.synth_name, event.synth_params)
 
-        # ------------------------------------------------------------------------
-        # SignalFlow patch
-        # ------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_PATCH_CREATE:
             # ------------------------------------------------------------------------
             # Action: Create patch
             # ------------------------------------------------------------------------
             if not hasattr(self.output_device, "create"):
                 raise InvalidEventException(
-                    "Device %s does not support this kind of event" % self.output_device
+                    f"Device {self.output_device} does not support this kind of event"
                 )
-            params = dict(
-                (key, Pattern.value(value)) for key, value in event.params.items()
-            )
+            params = {key: Pattern.value(value) for key, value in event.params.items()}
             if hasattr(event, "note"):
                 notes = event.note if hasattr(event.note, "__iter__") else [event.note]
 
                 for note in notes:
                     if note > 0:
                         # TODO: Should use None to denote rests
                         params["frequency"] = midi_note_to_frequency(note)
                         self.output_device.create(
+                            # event.patch, params, output=event.output, track_idx=track_idx
                             event.patch, params, output=event.output
                         )
             else:
-                self.output_device.create(event.patch, params, output=event.output)
+                self.output_device.create(event.patch, params, output=event.output, track_idx=track_idx)
 
-        elif (
-                event.type == EVENT_TYPE_PATCH_SET or event.type == EVENT_TYPE_PATCH_TRIGGER
-        ):
+        elif event.type in [EVENT_TYPE_PATCH_SET, EVENT_TYPE_PATCH_TRIGGER]:
             # ------------------------------------------------------------------------
             # Action: Set patch's input(s) and/or trigger an event
             # ------------------------------------------------------------------------
             for key, value in event.params.items():
                 value = Pattern.value(value)
                 event.patch.set_input(key, value)
 
@@ -466,27 +727,21 @@
 
             if event.type == EVENT_TYPE_PATCH_TRIGGER:
                 # ------------------------------------------------------------------------
                 # Action: Trigger a patch
                 # ------------------------------------------------------------------------
                 if not hasattr(self.output_device, "trigger"):
                     raise InvalidEventException(
-                        "Device %s does not support this kind of event"
-                        % self.output_device
+                        f"Device {self.output_device} does not support this kind of event"
                     )
-                params = dict(
-                    (key, Pattern.value(value)) for key, value in event.params.items()
-                )
+                params = {key: Pattern.value(value) for key, value in event.params.items()}
                 self.output_device.trigger(
-                    event.patch, event.trigger_name, event.trigger_value
+                    event.patch, event.trigger_name, event.trigger_value, track_idx=track_idx
                 )
 
-        # ------------------------------------------------------------------------
-        # Note: Classic MIDI note
-        # ------------------------------------------------------------------------
         elif event.type == EVENT_TYPE_NOTE:
             # ----------------------------------------------------------------------
             # event: Certain devices (eg Socket IO) handle generic events,
             #        rather than note_on/note_off. (Should probably have to
             #        register for this behaviour rather than happening magically...)
             # ----------------------------------------------------------------------
             if hasattr(self.output_device, "event") and callable(
@@ -509,58 +764,53 @@
                     if type(value) not in (int, float, bool, str, list, dict, tuple):
                         value = repr(value)
                         d[key] = value
 
                 self.output_device.event(d)
                 return
 
+            # TODO: pythonic duck-typing approach might be better
+            # TODO: doesn't handle arrays of amp, channel event, etc
+            notes = event.note if hasattr(event.note, "__iter__") else [event.note]
+
             # ----------------------------------------------------------------------
-            # note_on: Standard (MIDI) type of device
+            # Allow for arrays of amp, gate etc, to handle chords properly.
+            # Caveat: Things will go horribly wrong for an array of amp/gate event
+            # shorter than the number of notes.
             # ----------------------------------------------------------------------
-            # if type(event.amplitude) is tuple or event.amplitude > 0:
-            if type(event.amplitude) is tuple or True:
-                # TODO: pythonic duck-typing approach might be better
-                # TODO: doesn't handle arrays of amp, channel event, etc
-                notes = event.note if hasattr(event.note, "__iter__") else [event.note]
-
-                # ----------------------------------------------------------------------
-                # Allow for arrays of amp, gate etc, to handle chords properly.
-                # Caveat: Things will go horribly wrong for an array of amp/gate event
-                # shorter than the number of notes.
-                # ----------------------------------------------------------------------
-                for index, note in enumerate(notes):
-                    amp = (
-                        event.amplitude[index]
-                        if isinstance(event.amplitude, tuple)
-                        else event.amplitude
-                    )
-                    channel = (
-                        event.channel[index]
-                        if isinstance(event.channel, tuple)
-                        else event.channel
-                    )
-                    gate = (
-                        event.gate[index]
-                        if isinstance(event.gate, tuple)
-                        else event.gate
-                    )
-                    # TODO: Add an EVENT_SUSTAIN that allows absolute note lengths to be specified
+            for index, note in enumerate(notes):
+                amp = (
+                    event.amplitude[index]
+                    if isinstance(event.amplitude, tuple)
+                    else event.amplitude
+                )
+                channel = (
+                    event.channel[index]
+                    if isinstance(event.channel, tuple)
+                    else event.channel
+                )
+                gate = (
+                    event.gate[index]
+                    if isinstance(event.gate, tuple)
+                    else event.gate
+                )
+                # TODO: Add an EVENT_SUSTAIN that allows absolute note lengths to be specified
 
-                    # if (amp is not None and amp > 0) and (gate is not None and gate > 0):
-                    if (amp is not None) and (gate is not None):
-                        self.output_device.note_on(note, amp, channel)
-
-                        note_dur = event.duration * gate
-                        note_off_time = self.current_time + note_dur
-                        note_off = NoteOffEvent(note_off_time, note, channel)
-                        self.note_offs.append(note_off)
-                if event.pitchbend is not None:
-                    self.output_device.pitch_bend(event.pitchbend, channel)
+                # if (amp is not None and amp > 0) and (gate is not None and gate > 0):
+                if (amp is not None) and (gate is not None):
+                    self.output_device.note_on(note, amp, channel, track_idx=track_idx)
+
+                    note_dur = event.duration * gate
+                    note_off_time = self.current_time + note_dur
+                    note_off = NoteOffEvent(note_off_time, note, channel, track_idx=track_idx)
+                    self.note_offs.append(note_off)
+            if event.pitchbend is not None:
+                self.output_device.pitch_bend(event.pitchbend, channel)
         else:
-            raise InvalidEventException("Invalid event type: %s" % event.type)
+            raise InvalidEventException(f"Invalid event type: {event.type}")
 
         if self.timeline.on_event_callback:
             self.timeline.on_event_callback(self, event)
 
         if self.on_event_callbacks:
             for callback in self.on_event_callbacks:
                 callback(event)
```

### Comparing `isobar_ext-0.5.1/isobar_ext/util.py` & `isobar_ext-0.9.0/isobar_ext/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import random
 import math
+import random
 from typing import Any, Generator
+
 from .exceptions import InvalidMIDIPitch, UnknownNoteName, ClockException
 
 note_names = [
     ["C"],
     ["C#", "Db"],
     ["D"],
     ["D#", "Eb"],
@@ -19,17 +20,15 @@
 ]
 
 
 def normalize(array: list[float]) -> list[float]:
     """
     Normalise an array to sum to 1.0.
     """
-    if sum(array) == 0:
-        return array
-    return [float(n) / sum(array) for n in array]
+    return array if sum(array) == 0 else [float(n) / sum(array) for n in array]
 
 
 def windex(weights: list[float], rng=random) -> float:
     """
     Return a random index based on a list of weights, from 0..(len(weights) - 1).
     Assumes that weights is already normalised.
     """
@@ -72,57 +71,52 @@
     If no octave is given, octave 0 is considered
     so e.g. C->C0, E->E0
     a note value between 12..23 is returned.
     """
     if name[-1].isdigit():
         sign = -1 if name[-2] == "-" else 1
         octave = sign * int(name[-1])
-        if sign == 1:
-            name = name[:-1]
-        else:
-            name = name[:-2]
+        name = name[:-1] if sign == 1 else name[:-2]
     else:
         octave = -1
 
     try:
         # TODO: Fix such that note names can be lowercase (must also work with e.g. Bb)
         index = note_names.index(
             [nameset for nameset in note_names if name in nameset][0]
         )
-    except IndexError:
-        raise UnknownNoteName("Unknown note name: %s" % name)
+    except IndexError as e:
+        raise UnknownNoteName(f"Unknown note name: {name}") from e
 
     return (octave + 1) * 12 + index
 
 
 def midi_note_to_note_name(note: float) -> str:
     """
     Maps a MIDI note index to a note name.
     Supports fractional pitches.
     """
     if (type(note) is not int and type(note) is not float) or (note < 0 or note > 127):
         raise InvalidMIDIPitch()
 
     degree = int(note) % len(note_names)
     octave = int(note / len(note_names)) - 1
-    str = "%s%d" % (note_names[degree][0], octave)
+    v_str = "%s%d" % (note_names[degree][0], octave)
     frac = math.modf(note)[0]
     if frac > 0:
-        str = str + " + %2f" % frac
+        v_str = v_str + " + %2f" % frac
 
-    return str
+    return v_str
 
 
 def midi_note_to_frequency(note: float) -> float:
     """
     Maps a MIDI note index to a frequency.
     """
-    if note is None:
-        return None
-    return 440.0 * pow(2, (note - 69.0) / 12)
+    return None if note is None else 440.0 * pow(2, (note - 69.0) / 12)
 
 
 def midi_note_to_frequency_just_intonation(note):
     note_ratios = [
         1 / 1,
         256 / 243,
         9 / 8,
@@ -135,16 +129,15 @@
         27 / 16,
         16 / 9,
         243 / 128,
     ]
     octave = note // 12
     octave_note = note % 12
     octave_base_frequency = midi_note_to_frequency(octave * 12)
-    octave_note_frequency = octave_base_frequency * note_ratios[octave_note]
-    return octave_note_frequency
+    return octave_base_frequency * note_ratios[octave_note]
 
 
 def note_name_to_frequency(note_name: str) -> float:
     """
     Returns the frequency corresponding to the given MIDI note name.
 
     Args:
@@ -180,19 +173,19 @@
     Returns:
         float: The ratio, in semitones
     """
     return math.log2(frequency_ratio) * 12
 
 
 def scale_lin_exp(
-    value: float,
-    from_min: float = 0,
-    from_max: float = 1,
-    to_min: float = 1,
-    to_max: float = 10,
+        value: float,
+        from_min: float = 0,
+        from_max: float = 1,
+        to_min: float = 1,
+        to_max: float = 10,
 ) -> float:
     """
     Map a value on a linear scale to an exponential scale.
 
     Args:
         value: The value
         from_min: The lower bound of the input range
@@ -207,19 +200,19 @@
         return to_min
     if value > from_max:
         return to_max
     return ((to_max / to_min) ** ((value - from_min) / (from_max - from_min))) * to_min
 
 
 def scale_lin_lin(
-    value: float,
-    from_min: float = 0,
-    from_max: float = 1,
-    to_min: float = 0,
-    to_max: float = 1,
+        value: float,
+        from_min: float = 0,
+        from_max: float = 1,
+        to_min: float = 0,
+        to_max: float = 1,
 ) -> float:
     """
     Map a value on a linear scale to a linear scale.
 
     Args:
         value: The value
         from_min: The lower bound of the input range
@@ -242,25 +235,29 @@
         sum(list(zip(list(range(maximum + 1)), list(range(0, -maximum - 1, -1)))), ())
     )
     sequence.pop(0)
     return sequence
 
 
 def filter_tone_row(
-    source: list[int], target: list[int], bend_limit: int = 7
+        source: list[int], target: list[int], bend_limit: int = 7
 ) -> list[int]:
     """
     Filters the notes in <source> by the permitted notes in <target>.
     returns a tuple (<bool> acceptable, <int> pitch_bend)
     """
     bends = bipolar_diverge(bend_limit)
-    for bend in bends:
-        if all(((note + bend) % 12) in target for note in source):
-            return (True, bend)
-    return (False, 0)
+    return next(
+        (
+            (True, bend)
+            for bend in bends
+            if all(((note + bend) % 12) in target for note in source)
+        ),
+        (False, 0),
+    )
 
 
 def random_seed(seed: int) -> None:
     """
     Set the random number generator seed.
 
     Args:
@@ -279,16 +276,16 @@
 
     Returns:
         int: The multiplier
     """
     multiple = 1.0
     if output_clock_rate and input_clock_rate:
         multiple = output_clock_rate / input_clock_rate
-    if (multiple > 1 and int(multiple) != multiple) or (
-        multiple < 1 and 1 / multiple != int(1 / multiple)
+    if (1 < multiple != int(multiple)) or (
+            multiple < 1 and 1 / multiple != int(1 / multiple)
     ):
         raise ClockException(
             "Cannot sync output device (clock rates must integer multiples of each other)"
         )
 
     pos = 1
     while True:
```

