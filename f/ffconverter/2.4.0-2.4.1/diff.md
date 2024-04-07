# Comparing `tmp/ffconverter-2.4.0.tar.gz` & `tmp/ffconverter-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffconverter-2.4.0.tar", last modified: Sat Apr  6 19:16:58 2024, max compression
+gzip compressed data, was "ffconverter-2.4.1.tar", last modified: Sat Apr  6 19:29:54 2024, max compression
```

## Comparing `ffconverter-2.4.0.tar` & `ffconverter-2.4.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.377552 ffconverter-2.4.0/
--rw-r--r--   0 luna      (1000) luna      (1000)       50 2024-03-02 10:15:40.000000 ffconverter-2.4.0/AUTHORS
--rw-r--r--   0 luna      (1000) luna      (1000)    34665 2024-03-02 10:15:40.000000 ffconverter-2.4.0/COPYING
--rw-r--r--   0 luna      (1000) luna      (1000)     6438 2024-04-06 19:15:18.000000 ffconverter-2.4.0/ChangeLog
--rw-r--r--   0 luna      (1000) luna      (1000)      211 2024-03-02 10:15:40.000000 ffconverter-2.4.0/MANIFEST.in
--rw-r--r--   0 luna      (1000) luna      (1000)     2511 2024-04-06 19:16:58.377552 ffconverter-2.4.0/PKG-INFO
--rw-r--r--   0 luna      (1000) luna      (1000)     3731 2024-04-06 19:16:14.000000 ffconverter-2.4.0/README.md
--rw-r--r--   0 luna      (1000) luna      (1000)      982 2024-03-02 10:15:40.000000 ffconverter-2.4.0/TRANSLATORS
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.370885 ffconverter-2.4.0/bin/
--rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.0/bin/ffconverter
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.370885 ffconverter-2.4.0/ffconverter/
--rw-r--r--   0 luna      (1000) luna      (1000)      602 2024-04-06 19:12:53.000000 ffconverter-2.4.0/ffconverter/__init__.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     3107 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/about_dlg.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)    23183 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/audiovideotab.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     5253 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/config.py
--rw-r--r--   0 luna      (1000) luna      (1000)     2403 2024-04-04 15:23:59.000000 ffconverter-2.4.0/ffconverter/dynamictab.py
--rw-r--r--   0 luna      (1000) luna      (1000)    29084 2024-04-04 20:10:23.000000 ffconverter-2.4.0/ffconverter/ffconverter.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)     4728 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/imagetab.py
--rw-r--r--   0 luna      (1000) luna      (1000)    16574 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/preferences_dlg.py
--rwxr-xr-x   0 luna      (1000) luna      (1000)    18633 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/presets_dlgs.py
--rw-r--r--   0 luna      (1000) luna      (1000)    26813 2024-04-04 19:50:46.000000 ffconverter-2.4.0/ffconverter/progress.py
--rw-r--r--   0 luna      (1000) luna      (1000)  1251243 2024-03-02 10:15:40.000000 ffconverter-2.4.0/ffconverter/qrc_resources.py
--rw-r--r--   0 luna      (1000) luna      (1000)    27171 2024-04-04 16:33:34.000000 ffconverter-2.4.0/ffconverter/utils.py
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/ffconverter.egg-info/
--rw-r--r--   0 luna      (1000) luna      (1000)     2511 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/PKG-INFO
--rw-r--r--   0 luna      (1000) luna      (1000)     1262 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/SOURCES.txt
--rw-r--r--   0 luna      (1000) luna      (1000)        1 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/dependency_links.txt
--rw-r--r--   0 luna      (1000) luna      (1000)       12 2024-04-06 19:16:58.000000 ffconverter-2.4.0/ffconverter.egg-info/top_level.txt
--rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.0/launcher
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/locale/
--rw-r--r--   0 luna      (1000) luna      (1000)      862 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter.pro
--rw-r--r--   0 luna      (1000) luna      (1000)    45600 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_bg.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35525 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ca.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35959 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_cs.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    36320 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_de_DE.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38690 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_el.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    33999 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_en.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    35421 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_es.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    43549 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_fr.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42403 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_gl.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42406 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_gl_ES.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    41592 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_hu.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42338 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_it.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    37555 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ms_MY.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    39570 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_pl_PL.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38218 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_pt.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    39782 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_pt_BR.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    38131 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ro_RO.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    45091 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_ru.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    40891 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_tr.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    43700 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_vi.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    42125 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_zh_CN.ts
--rw-r--r--   0 luna      (1000) luna      (1000)    41525 2024-03-02 10:15:40.000000 ffconverter-2.4.0/locale/ffconverter_zh_TW.ts
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/man/
--rw-r--r--   0 luna      (1000) luna      (1000)      730 2024-03-02 10:15:40.000000 ffconverter-2.4.0/man/ffconverter.1.gz
--rw-r--r--   0 luna      (1000) luna      (1000)     1517 2024-03-02 10:15:40.000000 ffconverter-2.4.0/resources.qrc
--rw-r--r--   0 luna      (1000) luna      (1000)       38 2024-04-06 19:16:58.377552 ffconverter-2.4.0/setup.cfg
--rwxr-xr-x   0 luna      (1000) luna      (1000)     3392 2024-03-02 10:15:40.000000 ffconverter-2.4.0/setup.py
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/share/
--rw-r--r--   0 luna      (1000) luna      (1000)      404 2024-04-06 19:12:59.000000 ffconverter-2.4.0/share/ffconverter.desktop
--rw-r--r--   0 luna      (1000) luna      (1000)    30976 2024-03-02 10:15:40.000000 ffconverter-2.4.0/share/ffconverter.png
--rw-r--r--   0 luna      (1000) luna      (1000)    39299 2024-03-02 10:15:40.000000 ffconverter-2.4.0/share/presets.xml
-drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:16:58.374218 ffconverter-2.4.0/test/
--rwxr-xr-x   0 luna      (1000) luna      (1000)      816 2024-03-02 10:15:40.000000 ffconverter-2.4.0/test/test_dialogs.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.490851 ffconverter-2.4.1/
+-rw-r--r--   0 luna      (1000) luna      (1000)       50 2024-03-02 10:15:40.000000 ffconverter-2.4.1/AUTHORS
+-rw-r--r--   0 luna      (1000) luna      (1000)    34665 2024-03-02 10:15:40.000000 ffconverter-2.4.1/COPYING
+-rw-r--r--   0 luna      (1000) luna      (1000)     6507 2024-04-06 19:28:31.000000 ffconverter-2.4.1/ChangeLog
+-rw-r--r--   0 luna      (1000) luna      (1000)      211 2024-03-02 10:15:40.000000 ffconverter-2.4.1/MANIFEST.in
+-rw-r--r--   0 luna      (1000) luna      (1000)     2511 2024-04-06 19:29:54.490851 ffconverter-2.4.1/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     3731 2024-04-06 19:16:14.000000 ffconverter-2.4.1/README.md
+-rw-r--r--   0 luna      (1000) luna      (1000)      982 2024-03-02 10:15:40.000000 ffconverter-2.4.1/TRANSLATORS
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.487517 ffconverter-2.4.1/bin/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.1/bin/ffconverter
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.487517 ffconverter-2.4.1/ffconverter/
+-rw-r--r--   0 luna      (1000) luna      (1000)      602 2024-04-06 19:28:02.000000 ffconverter-2.4.1/ffconverter/__init__.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3107 2024-03-02 10:15:40.000000 ffconverter-2.4.1/ffconverter/about_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    23183 2024-03-02 10:15:40.000000 ffconverter-2.4.1/ffconverter/audiovideotab.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     5253 2024-03-02 10:15:40.000000 ffconverter-2.4.1/ffconverter/config.py
+-rw-r--r--   0 luna      (1000) luna      (1000)     2403 2024-04-04 15:23:59.000000 ffconverter-2.4.1/ffconverter/dynamictab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    29255 2024-04-06 19:26:17.000000 ffconverter-2.4.1/ffconverter/ffconverter.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     4728 2024-03-02 10:15:40.000000 ffconverter-2.4.1/ffconverter/imagetab.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    16574 2024-03-02 10:15:40.000000 ffconverter-2.4.1/ffconverter/preferences_dlg.py
+-rwxr-xr-x   0 luna      (1000) luna      (1000)    18633 2024-03-02 10:15:40.000000 ffconverter-2.4.1/ffconverter/presets_dlgs.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    26813 2024-04-04 19:50:46.000000 ffconverter-2.4.1/ffconverter/progress.py
+-rw-r--r--   0 luna      (1000) luna      (1000)  1251243 2024-03-02 10:15:40.000000 ffconverter-2.4.1/ffconverter/qrc_resources.py
+-rw-r--r--   0 luna      (1000) luna      (1000)    27171 2024-04-04 16:33:34.000000 ffconverter-2.4.1/ffconverter/utils.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.490851 ffconverter-2.4.1/ffconverter.egg-info/
+-rw-r--r--   0 luna      (1000) luna      (1000)     2511 2024-04-06 19:29:54.000000 ffconverter-2.4.1/ffconverter.egg-info/PKG-INFO
+-rw-r--r--   0 luna      (1000) luna      (1000)     1262 2024-04-06 19:29:54.000000 ffconverter-2.4.1/ffconverter.egg-info/SOURCES.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)        1 2024-04-06 19:29:54.000000 ffconverter-2.4.1/ffconverter.egg-info/dependency_links.txt
+-rw-r--r--   0 luna      (1000) luna      (1000)       12 2024-04-06 19:29:54.000000 ffconverter-2.4.1/ffconverter.egg-info/top_level.txt
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      114 2024-03-02 10:15:40.000000 ffconverter-2.4.1/launcher
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.490851 ffconverter-2.4.1/locale/
+-rw-r--r--   0 luna      (1000) luna      (1000)      862 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter.pro
+-rw-r--r--   0 luna      (1000) luna      (1000)    45600 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_bg.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35525 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_ca.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35959 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_cs.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    36320 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_de_DE.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38690 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_el.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    33999 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_en.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    35421 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_es.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43549 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_fr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42403 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_gl.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42406 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_gl_ES.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41592 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_hu.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42338 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_it.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    37555 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_ms_MY.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39570 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_pl_PL.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38218 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_pt.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    39782 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_pt_BR.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    38131 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_ro_RO.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    45091 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_ru.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    40891 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_tr.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    43700 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_vi.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    42125 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_zh_CN.ts
+-rw-r--r--   0 luna      (1000) luna      (1000)    41525 2024-03-02 10:15:40.000000 ffconverter-2.4.1/locale/ffconverter_zh_TW.ts
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.490851 ffconverter-2.4.1/man/
+-rw-r--r--   0 luna      (1000) luna      (1000)      730 2024-03-02 10:15:40.000000 ffconverter-2.4.1/man/ffconverter.1.gz
+-rw-r--r--   0 luna      (1000) luna      (1000)     1517 2024-03-02 10:15:40.000000 ffconverter-2.4.1/resources.qrc
+-rw-r--r--   0 luna      (1000) luna      (1000)       38 2024-04-06 19:29:54.490851 ffconverter-2.4.1/setup.cfg
+-rwxr-xr-x   0 luna      (1000) luna      (1000)     3392 2024-03-02 10:15:40.000000 ffconverter-2.4.1/setup.py
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.490851 ffconverter-2.4.1/share/
+-rw-r--r--   0 luna      (1000) luna      (1000)      404 2024-04-06 19:12:59.000000 ffconverter-2.4.1/share/ffconverter.desktop
+-rw-r--r--   0 luna      (1000) luna      (1000)    30976 2024-03-02 10:15:40.000000 ffconverter-2.4.1/share/ffconverter.png
+-rw-r--r--   0 luna      (1000) luna      (1000)    39299 2024-03-02 10:15:40.000000 ffconverter-2.4.1/share/presets.xml
+drwxr-xr-x   0 luna      (1000) luna      (1000)        0 2024-04-06 19:29:54.490851 ffconverter-2.4.1/test/
+-rwxr-xr-x   0 luna      (1000) luna      (1000)      816 2024-03-02 10:15:40.000000 ffconverter-2.4.1/test/test_dialogs.py
```

### Comparing `ffconverter-2.4.0/COPYING` & `ffconverter-2.4.1/COPYING`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ChangeLog` & `ffconverter-2.4.1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+Version 2.4.1
+-------------
+
+* Fix icon on Wayland (Fix Issue #13)
+
+
 Version 2.4.0
 -------------
 
 * Added trimesh/gmsh to support 3D-Models (close #11)
 
 * Fixed crash when using drag-and-drop (close #12)
```

### Comparing `ffconverter-2.4.0/PKG-INFO` & `ffconverter-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.4.0
+Version: 2.4.1
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
```

### Comparing `ffconverter-2.4.0/README.md` & `ffconverter-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/TRANSLATORS` & `ffconverter-2.4.1/TRANSLATORS`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/__init__.py` & `ffconverter-2.4.1/ffconverter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 GUI File Format Converter
 """
 
 # version
 __major__ = 2
 __minor__ = 4
-__patch__ = 0
+__patch__ = 1
 __prerelease__ = "" # alpha, beta, rc etc.
 
 # package information
 __name__ = "ffconverter"
 __version__ = "{0}.{1}.{2}".format(__major__, __minor__, __patch__)
 __version__ += __prerelease__
 __description__ = "File Format Converter with Qt GUI"
```

### Comparing `ffconverter-2.4.0/ffconverter/about_dlg.py` & `ffconverter-2.4.1/ffconverter/about_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/audiovideotab.py` & `ffconverter-2.4.1/ffconverter/audiovideotab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/config.py` & `ffconverter-2.4.1/ffconverter/config.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/dynamictab.py` & `ffconverter-2.4.1/ffconverter/dynamictab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/ffconverter.py` & `ffconverter-2.4.1/ffconverter/ffconverter.py`

 * *Files 1% similar despite different names*

```diff
@@ -660,14 +660,19 @@
 
 def main():
     app = QApplication([i.encode('utf-8') for i in sys.argv])
     app.setOrganizationName(ffmc.__name__)
     app.setOrganizationDomain(ffmc.__url__)
     app.setApplicationName('FF Multi Converter')
     app.setWindowIcon(QIcon(':/ffconverter.png'))
+    try:
+        # Qt 5.7+ needed
+        app.setDesktopFileName("ffconverter")
+    except AttributeError:
+        print("Using PyQt below 5.7, cannot set Wayland Icon!")
 
     locale = QLocale.system().name()
 
     qtTranslator = QTranslator()
     if qtTranslator.load('qt_' + locale, ':/'):
         app.installTranslator(qtTranslator)
     appTranslator = QTranslator()
```

### Comparing `ffconverter-2.4.0/ffconverter/imagetab.py` & `ffconverter-2.4.1/ffconverter/imagetab.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/preferences_dlg.py` & `ffconverter-2.4.1/ffconverter/preferences_dlg.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/presets_dlgs.py` & `ffconverter-2.4.1/ffconverter/presets_dlgs.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/progress.py` & `ffconverter-2.4.1/ffconverter/progress.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/qrc_resources.py` & `ffconverter-2.4.1/ffconverter/qrc_resources.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter/utils.py` & `ffconverter-2.4.1/ffconverter/utils.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/ffconverter.egg-info/PKG-INFO` & `ffconverter-2.4.1/ffconverter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffconverter
-Version: 2.4.0
+Version: 2.4.1
 Summary: File Format Converter with Qt GUI
 Home-page: https://github.com/l-koehler/FF-converter
 Author: Ilias Stamatis
 Author-email: stamatis.iliass@gmail.com
 Maintainer: l-koehler
 Maintainer-email: lorenz.koehler@posteo.de
 License: GNU GPL3
```

### Comparing `ffconverter-2.4.0/ffconverter.egg-info/SOURCES.txt` & `ffconverter-2.4.1/ffconverter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter.pro` & `ffconverter-2.4.1/locale/ffconverter.pro`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_bg.ts` & `ffconverter-2.4.1/locale/ffconverter_bg.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_ca.ts` & `ffconverter-2.4.1/locale/ffconverter_ca.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_cs.ts` & `ffconverter-2.4.1/locale/ffconverter_cs.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_de_DE.ts` & `ffconverter-2.4.1/locale/ffconverter_de_DE.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_el.ts` & `ffconverter-2.4.1/locale/ffconverter_el.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_en.ts` & `ffconverter-2.4.1/locale/ffconverter_en.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_es.ts` & `ffconverter-2.4.1/locale/ffconverter_es.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_fr.ts` & `ffconverter-2.4.1/locale/ffconverter_fr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_gl.ts` & `ffconverter-2.4.1/locale/ffconverter_gl.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_gl_ES.ts` & `ffconverter-2.4.1/locale/ffconverter_gl_ES.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_hu.ts` & `ffconverter-2.4.1/locale/ffconverter_hu.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_it.ts` & `ffconverter-2.4.1/locale/ffconverter_it.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_ms_MY.ts` & `ffconverter-2.4.1/locale/ffconverter_ms_MY.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_pl_PL.ts` & `ffconverter-2.4.1/locale/ffconverter_pl_PL.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_pt.ts` & `ffconverter-2.4.1/locale/ffconverter_pt.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_pt_BR.ts` & `ffconverter-2.4.1/locale/ffconverter_pt_BR.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_ro_RO.ts` & `ffconverter-2.4.1/locale/ffconverter_ro_RO.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_ru.ts` & `ffconverter-2.4.1/locale/ffconverter_ru.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_tr.ts` & `ffconverter-2.4.1/locale/ffconverter_tr.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_vi.ts` & `ffconverter-2.4.1/locale/ffconverter_vi.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_zh_CN.ts` & `ffconverter-2.4.1/locale/ffconverter_zh_CN.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/locale/ffconverter_zh_TW.ts` & `ffconverter-2.4.1/locale/ffconverter_zh_TW.ts`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/man/ffconverter.1.gz` & `ffconverter-2.4.1/man/ffconverter.1.gz`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/resources.qrc` & `ffconverter-2.4.1/resources.qrc`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/setup.py` & `ffconverter-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/share/ffconverter.png` & `ffconverter-2.4.1/share/ffconverter.png`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/share/presets.xml` & `ffconverter-2.4.1/share/presets.xml`

 * *Files identical despite different names*

### Comparing `ffconverter-2.4.0/test/test_dialogs.py` & `ffconverter-2.4.1/test/test_dialogs.py`

 * *Files identical despite different names*

