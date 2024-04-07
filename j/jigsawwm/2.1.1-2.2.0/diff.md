# Comparing `tmp/jigsawwm-2.1.1.tar.gz` & `tmp/jigsawwm-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jigsawwm-2.1.1.tar", last modified: Tue Jan 23 12:07:32 2024, max compression
+gzip compressed data, was "jigsawwm-2.2.0.tar", last modified: Sun Apr  7 03:38:51 2024, max compression
```

## Comparing `jigsawwm-2.1.1.tar` & `jigsawwm-2.2.0.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.935245 jigsawwm-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-01-23 12:07:32.935245 jigsawwm-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 12:07:32.935245 jigsawwm-2.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.927245 jigsawwm-2.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.927245 jigsawwm-2.1.1/src/jigsawwm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.931245 jigsawwm-2.1.1/src/jigsawwm/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/assets/dark.css
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/assets/dwindle.png
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/assets/icons.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/assets/obs.png
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/assets/wide-dwindle.png
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/daemon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.931245 jigsawwm-2.1.1/src/jigsawwm/jmk/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/jmk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/jmk/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/jmk/hotkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/jmk/sysinout.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/smartstart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.931245 jigsawwm-2.1.1/src/jigsawwm/tiler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/tiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/tiler/layouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/tiler/tilers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.931245 jigsawwm-2.1.1/src/jigsawwm/ui/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/ui/dialog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/ui/windows_splash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.931245 jigsawwm-2.1.1/src/jigsawwm/w32/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/reg.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/sendinput.py
--rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/vk.py
--rw-r--r--   0 runner    (1001) docker     (127)    16951 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/window.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/window_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/w32/winevent.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.935245 jigsawwm-2.1.1/src/jigsawwm/wm/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/wm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15926 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/wm/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/wm/op_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/wm/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/src/jigsawwm/wm/theme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.935245 jigsawwm-2.1.1/src/jigsawwm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8090 2024-01-23 12:07:32.000000 jigsawwm-2.1.1/src/jigsawwm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-01-23 12:07:32.000000 jigsawwm-2.1.1/src/jigsawwm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 12:07:32.000000 jigsawwm-2.1.1/src/jigsawwm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-23 12:07:32.000000 jigsawwm-2.1.1/src/jigsawwm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-23 12:07:32.000000 jigsawwm-2.1.1/src/jigsawwm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 12:07:32.935245 jigsawwm-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/tests/test_jmk_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-01-23 12:07:25.000000 jigsawwm-2.1.1/tests/test_jmk_hotkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.906196 jigsawwm-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-07 03:38:51.906196 jigsawwm-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6995 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 03:38:51.906196 jigsawwm-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.898197 jigsawwm-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.898197 jigsawwm-2.2.0/src/jigsawwm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.902197 jigsawwm-2.2.0/src/jigsawwm/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/assets/dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/assets/dwindle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/assets/icons.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/assets/obs.png
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/assets/wide-dwindle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/daemon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.902197 jigsawwm-2.2.0/src/jigsawwm/jmk/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/jmk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11856 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/jmk/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/jmk/hotkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/jmk/sysinout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/smartstart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.902197 jigsawwm-2.2.0/src/jigsawwm/tiler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/tiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7804 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/tiler/layouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4991 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/tiler/tilers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.902197 jigsawwm-2.2.0/src/jigsawwm/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/ui/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/ui/windows_splash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.902197 jigsawwm-2.2.0/src/jigsawwm/w32/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/reg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/sendinput.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/virtdesk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10945 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/vk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17423 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/window.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/window_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/w32/winevent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.906196 jigsawwm-2.2.0/src/jigsawwm/wm/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/wm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/wm/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/wm/op_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/wm/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/src/jigsawwm/wm/theme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.906196 jigsawwm-2.2.0/src/jigsawwm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-07 03:38:51.000000 jigsawwm-2.2.0/src/jigsawwm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-07 03:38:51.000000 jigsawwm-2.2.0/src/jigsawwm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 03:38:51.000000 jigsawwm-2.2.0/src/jigsawwm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-07 03:38:51.000000 jigsawwm-2.2.0/src/jigsawwm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 03:38:51.000000 jigsawwm-2.2.0/src/jigsawwm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 03:38:51.906196 jigsawwm-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/tests/test_jmk_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-07 03:38:45.000000 jigsawwm-2.2.0/tests/test_jmk_hotkey.py
```

### Comparing `jigsawwm-2.1.1/LICENSE` & `jigsawwm-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/PKG-INFO` & `jigsawwm-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jigsawwm
-Version: 2.1.1
+Version: 2.2.0
 Summary: JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 Author-email: Klesh Wong <klesh@qq.com>
 Project-URL: Documentation, https://jigsawwm.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/klesh/JigsawWM
 Project-URL: Issue Tracker, https://github.com/klesh/JigsawWM/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,14 +14,16 @@
 Classifier: Operating System :: POSIX :: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: comtypes~=1.1.14
 Requires-Dist: pyside6~=6.5.2
 Requires-Dist: mailcalaid~=1.0.1
+Requires-Dist: pyvda~=0.4.3
+Requires-Dist: screeninfo~=0.8.1
 
 # JigsawWM
 
 JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 
 # What Can I Do?
```

### Comparing `jigsawwm-2.1.1/README.md` & `jigsawwm-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/pyproject.toml` & `jigsawwm-2.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="jigsawwm"
-version="2.1.1"
+version="2.2.0"
 authors=[
   { name="Klesh Wong", email="klesh@qq.com" },
 ]
 description = "JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/assets/dark.css` & `jigsawwm-2.2.0/src/jigsawwm/assets/dark.css`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/assets/icons.svg` & `jigsawwm-2.2.0/src/jigsawwm/assets/icons.svg`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/assets/logo.png` & `jigsawwm-2.2.0/src/jigsawwm/assets/logo.png`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/assets/obs.png` & `jigsawwm-2.2.0/src/jigsawwm/assets/obs.png`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/assets/wide-dwindle.png` & `jigsawwm-2.2.0/src/jigsawwm/assets/wide-dwindle.png`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/daemon.py` & `jigsawwm-2.2.0/src/jigsawwm/daemon.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import abc
 import logging
 import os
 import signal
 import multiprocessing.pool
 from subprocess import PIPE, Popen
-from threading import Lock, Thread
+from threading import Lock, Thread, Event
 from typing import Callable, List, Sequence, TextIO
 
 from PySide6.QtGui import QAction, QIcon
 from PySide6.QtWidgets import QMenu, QSystemTrayIcon
 
 from jigsawwm import ui
 
@@ -78,35 +78,44 @@
     @property
     def text(self):
         status = "running" if self.is_running else "stopped"
         return f"[{status}] {self.name}"
 
 
 class ThreadedService(Service):
+    interval_sec = 60
+
     def __init__(self):
         self._thread = None
+        self._stop_flag = Event()
 
     @property
     def is_running(self) -> bool:
         return self._thread is not None and self._thread.is_alive()
 
     def start(self):
         if self.is_running:
             raise ValueError(f"Service {self.name} is already running")
         self._thread = Thread(target=self.run, daemon=True)
+        self._stop_flag.clear()
         self._thread.start()
 
-    @abc.abstractmethod
     def run(self):
+        while not self._stop_flag.wait(self.interval_sec):
+            self.loop()
+
+    @abc.abstractmethod
+    def loop(self):
         pass
 
     def stop(self):
-        if self._thread is None:
-            raise ValueError(f"Service {self.name} is not running")
+        if not self.is_running:
+            return
         thread, self._thread = self._thread, None
+        self._stop_flag.set()
         thread.join()
 
 
 class ProcessService(Service):
     """ProcessService is a kind of specialized Service that run a CLI program in the
     background"""
 
@@ -166,28 +175,23 @@
 
     @abc.abstractmethod
     def run(self) -> bool:
         pass
 
     def launch(self):
         if self.condition():
-            if self.nonblocking:
-                self.pool.apply_async(self.run)
-            else:
-                self.run()
+            self.launch_anyway()
+
+    def launch_anyway(self):
+        self.pool.apply_async(self.run)
 
     @property
     def text(self):
         return self.name
 
-    @property
-    def nonblocking(self):
-        return False
-
-
 class Daemon:
     """JigsawWM Daemon serivce, you must inherite this class and override the `setup` function
     to configurate the Manager.
     """
 
     trayicon: QSystemTrayIcon = None
     traymenu: QMenu = None
@@ -216,15 +220,15 @@
         """Update traymenu"""
         self.traymenu.clear()
         self.menuitems.clear()
         # tasks
         for job in self.jobs:
             if isinstance(job, Task):
                 act = QAction(job.text)
-                act.triggered.connect(job.run)
+                act.triggered.connect(job.launch_anyway)
                 self.traymenu.addAction(act)
                 self.menuitems.append(act)
         self.traymenu.addSeparator()
         # services
         for job in self.jobs:
             if isinstance(job, Service):
                 act = QAction(job.text)
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/jmk/core.py` & `jigsawwm-2.2.0/src/jigsawwm/jmk/core.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/jmk/hotkey.py` & `jigsawwm-2.2.0/src/jigsawwm/jmk/hotkey.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/jmk/sysinout.py` & `jigsawwm-2.2.0/src/jigsawwm/jmk/sysinout.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from jigsawwm.w32 import hook
 from jigsawwm.w32.sendinput import is_synthesized, send_input, vk_to_input
 from jigsawwm.w32.window import Window, get_active_window
 
 from .core import *
 
 q = SimpleQueue()
-
+state = {}
 
 class SystemInput:
     """A handler that handles system input events.
 
     :param next_handler: the next handler in the chain, normally a JmkCore instance
     :param bypass_exe: a list of regular expression patterns that matches the exe path
         some applications (e.g. Windows 10's touch keyboard, emoji input) will not
@@ -190,11 +190,12 @@
         q.put(evt)
         return True
 
 
 def consume_queue():
     while True:
         evt = q.get()
+        state[evt.vk] = evt.pressed
         send_input(vk_to_input(evt.vk, evt.pressed, flags=evt.flags))
 
 
 executor.submit(consume_queue)
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/smartstart.py` & `jigsawwm-2.2.0/src/jigsawwm/smartstart.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     state = get_state_manager()
     last_date = state.getdate("daily", name)
     state.setdate("daily", name, today)
     state.save()
     return last_date != today
 
 
-def start_if_not_running(exe_path: str):
+def start_if_not_running(exe_path: str, name_only: bool=True):
     """Returns True if the given name has not been called today"""
-    if not is_exe_running(exe_path):
-        os.startfile(exe_path)
+    if not is_exe_running(exe_path, name_only):
+        os.startfile(exe_path)
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/state.py` & `jigsawwm-2.2.0/src/jigsawwm/state.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/tiler/layouts.py` & `jigsawwm-2.2.0/src/jigsawwm/tiler/layouts.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/tiler/tilers.py` & `jigsawwm-2.2.0/src/jigsawwm/tiler/tilers.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/ui/app.py` & `jigsawwm-2.2.0/src/jigsawwm/ui/app.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/ui/dialog.py` & `jigsawwm-2.2.0/src/jigsawwm/ui/dialog.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/ui/windows_splash.py` & `jigsawwm-2.2.0/src/jigsawwm/ui/windows_splash.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/hook.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/hook.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,14 +329,21 @@
         event: WinEvent,
         hwnd: HWND,
         id_obj: LONG,
         id_chd: LONG,
         id_evt_thread: DWORD,
         time: DWORD,
     ):
+        if event in (
+            WinEvent.EVENT_OBJECT_LOCATIONCHANGE,
+            WinEvent.EVENT_OBJECT_NAMECHANGE,
+            WinEvent.EVENT_SYSTEM_CAPTURESTART,
+            WinEvent.EVENT_SYSTEM_CAPTUREEND,
+        ):
+            return
         print("==================================")
         print(
             "[{now}] {event:30s} {hwnd:8d} ido: {id_obj:6d} idc: {id_chd:6d} {title}".format(
                 now=datetime.now().strftime("%M:%S.%f"),
                 event=event.name,
                 hwnd=hwnd or 0,
                 id_obj=id_obj,
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/monitor.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/monitor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import enum
 from ctypes import *
 from ctypes.wintypes import *
 from functools import cached_property
 from typing import Iterator, List, Tuple
+import screeninfo
+from dataclasses import dataclass
+import math
 
 user32 = WinDLL("user32", use_last_error=True)
 shcore = WinDLL("shcore", use_last_error=True)
 _current_pos_ptr = POINT()
 
 # Ref: https://learn.microsoft.com/en-us/windows/win32/gdi/multiple-display-monitors-functions
 
@@ -77,15 +80,15 @@
 
 
 class MONITORINFOEX(Structure):
     cbSize: int
     rcMonitor: RECT
     rcWork: RECT
     dwFlags: int
-    szDevice: CHAR * CCHDEVICENAME
+    szDevice: CHAR
 
     _fields_ = (
         ("cbSize", DWORD),
         ("rcMonitor", RECT),
         ("rcWork", RECT),
         ("dwFlags", DWORD),
         ("szDevice", CHAR * CCHDEVICENAME),
@@ -163,14 +166,36 @@
         :rtype: DEVICE_SCALE_FACTOR
         """
         scale_factor = ULONG()
         if shcore.GetScaleFactorForMonitor(self._hmon, byref(scale_factor)) != 0:
             raise WinError(get_last_error())
         return DEVICE_SCALE_FACTOR(scale_factor.value)
 
+    def get_screen_info(self) -> screeninfo.Monitor:
+        for monitor in screeninfo.get_monitors():
+            if monitor.name == self.name:
+                return ScreenInfo(
+                    monitor.width,
+                    monitor.height,
+                    monitor.width_mm,
+                    monitor.height_mm,
+                    ratio=max(monitor.width, monitor.height) / min(monitor.width, monitor.height),
+                    is_primary=monitor.is_primary,
+                    inch=round(math.sqrt(monitor.width_mm ** 2 + monitor.height_mm ** 2) / 25.4),
+                )
+
+@dataclass
+class ScreenInfo:
+    width_px: int
+    height_px: int
+    width_mm: int
+    height_mm: int
+    ratio: float
+    is_primary: bool
+    inch: int
 
 def get_monitors() -> Iterator[Monitor]:
     """Retrieves all display monitors(mirroring monitors are excluded)
 
     :returns: system monitors
     :rtype: Iterator[Monitor]
     """
@@ -236,15 +261,20 @@
     p = get_cursor_pos()
     print(f"cursor pos       :  x {p.x} y {p.y}")
     for monitor in get_topo_sorted_monitors():
         print()
         print("scale factor     :", monitor.get_scale_factor())
         monitor_info = monitor.get_info()
         print("device           :", monitor_info.szDevice)
+        print("screen info    :", monitor.get_screen_info())
         m = monitor_info.rcWork
         print(
             f"monitor workarea : left {m.left} top {m.top}  right {m.right}  bottom {m.bottom}"
         )
         m = monitor_info.rcMonitor
         print(
             f"monitor react    : left {m.left} top {m.top}  right {m.right}  bottom {m.bottom}"
         )
+
+    # import screeninfo
+    # for monitor in screeninfo.get_monitors():
+    #     print(monitor)
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/process.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/process.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 from ctypes import *
 from ctypes.wintypes import *
 from typing import List
+from enum import IntEnum
 
 kernel32 = WinDLL("kernel32", use_last_error=True)
 advapi32 = WinDLL("advapi32", use_last_error=True)
 psapi = WinDLL("psapi", use_last_error=True)
+shcore  = WinDLL("shcore", use_last_error=True)
 
 TOKEN_QUERY = DWORD(8)
 
 
 def open_process_for_limited_query(pid: int) -> HANDLE:
     """Opens an existing local process object with permission to query limited information
 
@@ -121,13 +123,25 @@
     :return: session id
     :rtype: int
     """
     session_id = DWORD()
     kernel32.ProcessIdToSessionId(kernel32.GetCurrentProcessId(), byref(session_id))
     return kernel32.WTSGetActiveConsoleSessionId()
 
+class ProcessDpiAwareness(IntEnum):
+  PROCESS_DPI_UNAWARE = 0,
+  PROCESS_SYSTEM_DPI_AWARE = 1,
+  PROCESS_PER_MONITOR_DPI_AWARE = 2
+
+def get_process_dpi_awareness(pid: int) -> ProcessDpiAwareness:
+    """Retrieves the DPI awareness of the process"""
+    hprc = open_process_for_limited_query(pid)
+    awareness = c_int()
+    if shcore.GetProcessDpiAwareness(hprc, pointer(awareness)):
+        raise WinError(get_last_error())
+    return ProcessDpiAwareness(awareness.value) 
 
 if __name__ == "__main__":
     # import sys
 
     # print(is_exe_running(sys.argv[1], bool(sys.argv[2])))
     print(get_session_id())
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/reg.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/reg.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def read_reg_key(key, subkey, value):
     """
     Reads a value from the registry
     """
     try:
         with winreg.OpenKey(key, subkey) as handle:
-            return winreg.QueryValueEx(handle, value)[0]
+            return winreg.QueryValueEx(handle, value)[0].hex()
     except FileNotFoundError:
         return None
 
 
 def get_current_desktop_id():
     """
     Returns the GUID of the current virtual desktop
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/sendinput.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/sendinput.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/vk.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/vk.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/window.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/window.py`

 * *Files 1% similar despite different names*

```diff
@@ -332,25 +332,35 @@
     def restore(self):
         """Activates and displays the window. If the window is minimized or maximized,
         the system restores it to its original size and position."""
         restore_window(self._hwnd)
 
     def toggle_maximize(self):
         """Toggle maximize style"""
-        if self.get_style() & WindowStyle.MAXIMIZE:
+        if self.is_maximized:
             self.restore()
         else:
             self.maximize()
 
     @property
+    def is_maximized(self) -> bool:
+        """Check if window is maximized"""
+        return self.get_style() & WindowStyle.MAXIMIZE
+
+    @property
     def is_evelated(self):
         """Check if window is elevated (Administrator)"""
         return process.is_elevated(self.pid)
 
     @property
+    def dpi_awareness(self):
+        """Check if window is api aware"""
+        return process.get_process_dpi_awareness(self.pid)
+
+    @property
     def is_cloaked(self) -> bool:
         """Check if window is cloaked (DWM)
 
         Ref: https://learn.microsoft.com/en-us/windows/win32/api/dwmapi/ne-dwmapi-dwmwindowattribute
         """
         return is_window_cloaked(self._hwnd)
 
@@ -379,25 +389,29 @@
     def set_rect(self, rect: RECT):
         """Sets the dimensions of the bounding rectangle (Call SetWindowPos with RECT)
 
         Ref: https://learn.microsoft.com/en-us/windows/win32/api/winuser/nf-winuser-setwindowpos
 
         :param rect: RECT with top/left/bottom/right properties
         """
+        if self.is_maximized:
+            self.restore()
         set_window_rect(self._hwnd, rect)
         self._restricted_rect = rect
         logger.debug("set_rect %s for %s", rect, self.title)
 
     def restrict(self):
         if self._restricted_rect:
             set_window_rect(self._hwnd, self._restricted_rect)
             logger.debug("restricted %s for %s", self._restricted_rect, self.title)
 
     def activate(self) -> bool:
         """Brings the thread that created current window into the foreground and activates the window"""
+        print("activate")
+        import traceback; traceback.print_stack()
         return set_active_window(self)
 
     @property
     def icon_handle(self) -> HANDLE:
         return get_window_icon(self._hwnd)
 
 
@@ -534,14 +548,15 @@
     rect = window.get_rect()
     print("rect         :", rect.left, rect.top, rect.right, rect.bottom, file=file)
     bound = window.get_extended_frame_bounds()
     print("bound        :", bound.left, bound.top, bound.right, bound.bottom, file=file)
     print("is_app_window:", is_app_window(hwnd), file=file)
     print("is_manageable:", is_manageable_window(hwnd), file=file)
     print("is_evelated  :", window.is_evelated, file=file)
+    print("dpi_awareness:", window.dpi_awareness.name, file=file)
 
 
 def inspect_active_window():
     text = sprint_window(get_foreground_window())
     print(text)
     messagebox.showinfo("JigsawWM", text)
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/window_structs.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/window_structs.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/w32/winevent.py` & `jigsawwm-2.2.0/src/jigsawwm/w32/winevent.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/src/jigsawwm/wm/manager.py` & `jigsawwm-2.2.0/src/jigsawwm/wm/manager.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import logging
-from functools import partial
 from os import path
 from typing import Dict, List, Optional, Set
+from threading import Thread
+from queue import SimpleQueue
+import multiprocessing.pool
+import time
 
 from jigsawwm import ui
 from jigsawwm.tiler.tilers import *
 from jigsawwm.w32 import hook
 from jigsawwm.w32.monitor import (
     Monitor,
     get_monitor_from_cursor,
@@ -18,19 +21,20 @@
     DWORD,
     HWND,
     LONG,
     Window,
     get_foreground_window,
     get_manageable_windows,
     get_window_from_pos,
+    is_top_level_window,
     get_window_title,
     is_app_window,
-    is_window,
 )
 from jigsawwm.w32.winevent import WinEvent
+from jigsawwm.jmk import sysinout, Vk
 
 from .op_mixin import OpMixin
 from .state import MonitorState, VirtDeskState
 from .theme import Theme
 
 logger = logging.getLogger(__name__)
 
@@ -82,26 +86,29 @@
                 layout_tiler=dwindle_layout_tiler,
                 icon_name="dwindle.png",
             ),
         ]
         self.ignore_exe_names = set(ignore_exe_names or [])
         self.force_managed_exe_names = set(force_managed_exe_names or [])
         self.init_exe_sequence = init_exe_sequence or []
-        self.theme = self.themes[0].name
+        self.wait_mouse_released = False
+        self._sync_queue = SimpleQueue()
+        self._sync_pool = multiprocessing.pool.ThreadPool()
+        self.start_sync_thread()
         self.sync(init=True)
 
     @property
     def virtdesk_state(self) -> Optional[VirtDeskState]:
         """Retrieve virtual desktop state"""
         desktop_id = get_current_desktop_id()
         virtdesk_state = self._state.get(desktop_id)
         if virtdesk_state is None:
             # make sure monitor_state for current virtual desktop exists
             virtdesk_state = VirtDeskState(
-                lambda theme: self.themes[self.get_theme_index(theme)], desktop_id
+                lambda theme: self.themes[self.get_theme_index(theme)], desktop_id, self.themes
             )
             self._state[desktop_id] = virtdesk_state
         return virtdesk_state
 
     def check_window_ignored(self, window: Window) -> bool:
         exepath = window.exe
         return not exepath or path.basename(exepath) in self.ignore_exe_names
@@ -109,84 +116,72 @@
     def check_force_managed(self, hwnd: HWND) -> bool:
         try:
             exepath = Window(hwnd).exe
             return exepath and path.basename(exepath) in self.force_managed_exe_names
         except:
             return False
 
-    def sync(self, init=False, restrict=False) -> bool:
-        """Update manager state(monitors, windows) to match OS's and arrange windows if it is changed"""
+    def sync(self, init=False, restrict=False, delay=0.2) -> bool:
+        self._sync_queue.put_nowait((init, restrict, delay))
 
-        virtdesk_state = self.virtdesk_state
+    def start_sync_thread(self):
+        """Start a thread to watch for the queue and manage windows accordingly"""
+        self._thread = Thread(
+            target=self._consume_sync_queue,
+            name="sync_queue_consumer",
+        )
+        self._thread.start()
 
+    def _consume_sync_queue(self):
+        while True:
+            try:
+                init, restrict, delay = self._sync_queue.get()
+                if delay:
+                    time.sleep(delay)
+                    while not self._sync_queue.empty(): # ignore sync requests during the time
+                        self._sync_queue.get_nowait()
+                self._sync(init, restrict)
+            except:
+                import traceback
+                traceback.print_exc()
 
-        #
+    def _sync(self, init=False, restrict=False) -> bool:
+        # logger.warning("_sync")
+        virtdesk_state = self.virtdesk_state
         # gather all manageable windows
-        #
-
         manageable_windows = list(get_manageable_windows(self.check_force_managed))
         if not manageable_windows:
             return
-
-
-        #
         # group manageable windows by their current monitor
-        #
-
         group_wins_by_mons: Dict[Monitor, Set[Window]] = {}
         managed_windows = set()
         for window in manageable_windows:
-
-
-            #
             # skip this window if to be ignored
-            #
-
             if self.check_window_ignored(window):
                 continue
-
-
-            #
             # determine relevant monitor
-            #
-
             if init or window in virtdesk_state.managed_windows:
-
                 # use previous monitor
                 monitor = get_monitor_from_window(window.handle)
-
             else:
                 # use the monitor currently showing the cursor
                 monitor = get_monitor_from_cursor()
-
-
-            #
             # build list of windows for each monitor
-            #
-
             # get current list of windows for relevant monitor
             windows = group_wins_by_mons.get(monitor)
-
             # init list if not yet existing
             if windows is None:
                 windows = set()
                 group_wins_by_mons[monitor] = windows
-
             # add window to lists
             windows.add(window)
             managed_windows.add(window)
             logger.debug("%s is managed by monitor %s", window, monitor)
-
-
-        #
         # synchronize windows on each monitor
-        #
-
         virtdesk_state.managed_windows = managed_windows
-
         # pass down to monitor_state for further synchronization
         for monitor, windows in group_wins_by_mons.items():
             monitor_state = virtdesk_state.get_monitor(monitor)
             monitor_state.sync(
                     windows,
                     restrict=restrict,
                     #window_sort_order=self.init_exe_sequence if init else [],
@@ -386,59 +381,86 @@
         event: WinEvent,
         hwnd: HWND,
         id_obj: LONG,
         id_chd: LONG,
         id_evt_thread: DWORD,
         evt_time: DWORD,
         restrict: bool = False,
+        delay: float = 0.1,
     ):
-        if (
-            id_obj
-            or id_chd
-            or not is_window(hwnd)
-            or not is_app_window(hwnd)
-            or self.check_window_ignored(Window(hwnd))
+        # ignore if left mouse button is pressed in case of dragging
+        force_sync = False
+        if sysinout.state.get( Vk.LBUTTON ) and event == WinEvent.EVENT_SYSTEM_MOVESIZEEND:
+            # delay the sync until button released to avoid flickering
+            self.wait_mouse_released = True
+            return
+        elif self.wait_mouse_released:
+            if not sysinout.state.get( Vk.LBUTTON ):
+                self.wait_mouse_released = False
+                force_sync = True
+            else:
+                return
+        if force_sync:
+            logger.debug("force sync")
+            self.sync(restrict=restrict, delay=delay)
+            return
+        # # filter by event
+        # if event not in (
+        #     WinEvent.EVENT_OBJECT_LOCATIONCHANGE,
+        #     WinEvent.EVENT_OBJECT_NAMECHANGE,
+        # ):
+        #     logger.warning(
+        #         "[A] event: %30s hwnd: %8s id_obj: %8x id_chd: %8x id_evt_thread: %8d title: %s",
+        #         event.name, hwnd, id_obj, id_chd, id_evt_thread, get_window_title(hwnd)
+        #     )
+        window = Window(hwnd)
+        def manageable(hwnd):
+            return (
+                is_top_level_window(hwnd)
+                and is_app_window(hwnd)
+                and get_window_title(hwnd)
+                and not self.check_window_ignored(window)
+            )
+        if event == WinEvent.EVENT_OBJECT_SHOW: # for app that minimized to tray, show event is the only way to detect
+            if not manageable(hwnd):
+                return
+        elif event == WinEvent.EVENT_OBJECT_HIDE: # same as above
+            if window not in self.virtdesk_state.managed_windows:
+                return
+        elif event == WinEvent.EVENT_SYSTEM_MOVESIZEEND:
+            restrict = True
+        # elif event == WinEvent.EVENT_OBJECT_STATECHANGE:
+        #     if not manageable(hwnd):
+        #         return
+        #     delay = 0.2
+        elif event not in (
+            WinEvent.EVENT_SYSTEM_MINIMIZESTART,
+            WinEvent.EVENT_SYSTEM_MINIMIZEEND,
         ):
+            # if event not in (WinEvent.EVENT_OBJECT_LOCATIONCHANGE, WinEvent.EVENT_OBJECT_NAMECHANGE):
+            #     logger.warning(
+            #         "[B] event: %30s hwnd: %8s id_obj: %8x id_chd: %8x thread %8x top_level: %1s app_window: %1s ignored: %1s title: %s",
+            #         event.name, hwnd, id_obj, id_chd,id_evt_thread, is_top_level_window(hwnd),is_app_window(hwnd), self.check_window_ignored(Window(hwnd)), get_window_title(hwnd)
+            #     )
             return
-        logger.debug(
-            "_winevent_callback: event %s restrict %s %s",
-            event.name,
-            restrict,
-            get_window_title(hwnd),
-        )
-        self.sync(restrict=restrict)
+
+        # logger.warning(
+        #     "[C] event: %30s hwnd: %8s title: %s",
+        #     event.name, hwnd,  get_window_title(hwnd)
+        # )
+        self.sync(restrict=restrict, delay=delay)
 
     def install_hooks(self):
         """Install hooks for window events"""
         self.hook_ids = [
             hook.hook_winevent(
-                WinEvent.EVENT_OBJECT_SHOW,
-                WinEvent.EVENT_OBJECT_HIDE,
+                WinEvent.EVENT_MIN,
+                WinEvent.EVENT_MAX,
                 self._winevent_callback,
             ),
-            hook.hook_winevent(
-                WinEvent.EVENT_OBJECT_CLOAKED,
-                WinEvent.EVENT_OBJECT_UNCLOAKED,
-                self._winevent_callback,
-            ),
-            hook.hook_winevent(
-                WinEvent.EVENT_SYSTEM_MINIMIZESTART,
-                WinEvent.EVENT_SYSTEM_MINIMIZEEND,
-                self._winevent_callback,
-            ),
-            hook.hook_winevent(
-                WinEvent.EVENT_SYSTEM_MOVESIZEEND,
-                WinEvent.EVENT_SYSTEM_MOVESIZEEND,
-                partial(self._winevent_callback, restrict=True),
-            ),
-            # hook.hook_winevent(
-            #     WinEvent.EVENT_SYSTEM_FOREGROUND,
-            #     WinEvent.EVENT_SYSTEM_FOREGROUND,
-            #     partial(self._winevent_callback, restrict=True),
-            # ),
         ]
 
     def uninstall_hooks(self):
         for hook_id in self.hook_ids:
             hook.unhook_winevent(hook_id)
         self.hook_ids = []
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/wm/state.py` & `jigsawwm-2.2.0/src/jigsawwm/wm/state.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from typing import Dict, List, Optional, Set
 from os import path
 
 from jigsawwm.tiler.tilers import *
 from jigsawwm.w32.monitor import Monitor, get_monitor_from_window
 from jigsawwm.w32.window import RECT, Window, get_active_window
+from jigsawwm.w32.process import ProcessDpiAwareness
 
 from .theme import Theme
 
 logger = logging.getLogger(__name__)
 
 
 class MonitorState:
@@ -118,15 +119,14 @@
 
     def arrange(self, theme: Optional[Theme] = None):
         """Arrange windows based on the theme
 
         :param str theme: optional, fallback to theme of the instance
         """
         theme = theme or self.virtdesk_state.get_theme(self.theme)
-        print("arrange", self.theme, theme.name)
         wr = self.monitor.get_info().rcWork
         work_area = (wr.left, wr.top, wr.right, wr.bottom)
         windows = self.get_existing_windows()
         i = 0
         gap = theme.gap
         for left, top, right, bottom in theme.layout_tiler(work_area, len(windows)):
             window = windows[i]
@@ -143,25 +143,30 @@
             left += gap
             top += gap
             right -= gap
             bottom -= gap
             rect = RECT(left, top, right, bottom)
             logger.debug("arrange %s %s", window, rect)
             window.set_rect(rect)
+            i += 1
+            if window.dpi_awareness == ProcessDpiAwareness.PROCESS_DPI_UNAWARE:
+                # seems like the `get_extended_frame_bounds` would return physical size 
+                # for DPI unware window, skip them for now
+                # TODO: convert physical size to logical size for DPI unware window
+                continue
             # compensation
             r = window.get_rect()
             b = window.get_extended_frame_bounds()
             compensated_rect = (
                 round(left + r.left - b.left),
                 round(top + r.top - b.top),
                 round(right + r.right - b.right),
                 round(bottom + r.bottom - b.bottom),
             )
             window.set_rect(RECT(*compensated_rect))
-            i += 1
 
     def restrict(self, theme: Optional[Theme] = None):
         """Restrict all managed windows to their specified rect"""
         theme = theme or self.get_theme()
         if not theme.strict:
             return
         for window in self.windows:
@@ -175,32 +180,36 @@
     :param bytearray desktop_id: virtual desktop id
     """
 
     desktop_id: bytearray
     managed_windows: Set[Window]
     monitors: Dict[Monitor, MonitorState]
     last_active_window: Optional[Window] = None
+    themes: List[Theme]
 
-    def __init__(self, get_theme: Callable[[str], Theme], desktop_id: bytearray):
+    def __init__(self, get_theme: Callable[[str], Theme], desktop_id: bytearray, themes: List[Theme]):
         self.desktop_id = desktop_id
         self.managed_windows = set()
         self.monitors = {}
         self.last_active_window = None
         self.get_theme = get_theme
+        self.themes = themes
 
     def get_monitor(self, monitor: Monitor) -> MonitorState:
         """Retrieves the monitor state for the specified monitor in the virtual desktop
 
         :param Monitor monitor: monitor
         :returns: monitor state
         :rtype: MonitorState
         """
         monitor_state = self.monitors.get(monitor)
         if monitor_state is None:
-            monitor_state = MonitorState(self, monitor)
+            theme = sorted(self.themes, key=lambda x: x.affinity_index(monitor.get_screen_info()), reverse=True)[0]
+            logger.info("default to theme %s for monito %s", theme.name, monitor.name)
+            monitor_state = MonitorState(self, monitor, theme=theme.name)
             self.monitors[monitor] = monitor_state
         return monitor_state
 
     def get_managed_active_window(self) -> Optional[Window]:
         """Retrieves the managed forground window if any"""
         window = get_active_window()
         logger.debug("get_managed_active_window: active window %s", window)
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm/wm/theme.py` & `jigsawwm-2.2.0/src/jigsawwm/wm/theme.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 from typing import List, Optional
 
 from jigsawwm.tiler.tilers import *
+from jigsawwm.w32.monitor import Monitor
 
 
 @dataclass
 class Theme:
     """Theme is a set of preference packed together for users to switch easily,
     typically, it consists of a LayoutTiler, Gap between windows and
     other options.
@@ -22,7 +23,8 @@
     # new appeared window would be prepended to the list if the option was set to True
     new_window_as_master: Optional[bool] = None
     # gap between windows / monitor edges
     gap: Optional[int] = 0
     # forbid
     strict: Optional[bool] = None
     hook_ids: List[int] = None
+    affinity_index: Optional[Callable[[Monitor], int]] = None
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm.egg-info/PKG-INFO` & `jigsawwm-2.2.0/src/jigsawwm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jigsawwm
-Version: 2.1.1
+Version: 2.2.0
 Summary: JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 Author-email: Klesh Wong <klesh@qq.com>
 Project-URL: Documentation, https://jigsawwm.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/klesh/JigsawWM
 Project-URL: Issue Tracker, https://github.com/klesh/JigsawWM/issues
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: Microsoft :: Windows
@@ -14,14 +14,16 @@
 Classifier: Operating System :: POSIX :: BSD
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: comtypes~=1.1.14
 Requires-Dist: pyside6~=6.5.2
 Requires-Dist: mailcalaid~=1.0.1
+Requires-Dist: pyvda~=0.4.3
+Requires-Dist: screeninfo~=0.8.1
 
 # JigsawWM
 
 JigsawWM is a free and open-source project that aims to increase your productivity by offering a set of automation facilities, including the jmk module as an AHK alternative, a Tiling Window Manager to free you from managing windows manually and the Daemon to support any customization you may have in mind.
 
 # What Can I Do?
```

### Comparing `jigsawwm-2.1.1/src/jigsawwm.egg-info/SOURCES.txt` & `jigsawwm-2.2.0/src/jigsawwm.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 src/jigsawwm/ui/windows_splash.py
 src/jigsawwm/w32/__init__.py
 src/jigsawwm/w32/hook.py
 src/jigsawwm/w32/monitor.py
 src/jigsawwm/w32/process.py
 src/jigsawwm/w32/reg.py
 src/jigsawwm/w32/sendinput.py
+src/jigsawwm/w32/virtdesk.py
 src/jigsawwm/w32/vk.py
 src/jigsawwm/w32/window.py
 src/jigsawwm/w32/window_structs.py
 src/jigsawwm/w32/winevent.py
 src/jigsawwm/wm/__init__.py
 src/jigsawwm/wm/manager.py
 src/jigsawwm/wm/op_mixin.py
```

### Comparing `jigsawwm-2.1.1/tests/test_jmk_core.py` & `jigsawwm-2.2.0/tests/test_jmk_core.py`

 * *Files identical despite different names*

### Comparing `jigsawwm-2.1.1/tests/test_jmk_hotkey.py` & `jigsawwm-2.2.0/tests/test_jmk_hotkey.py`

 * *Files identical despite different names*

