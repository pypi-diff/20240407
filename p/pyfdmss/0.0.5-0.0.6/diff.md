# Comparing `tmp/pyfdmss-0.0.5.tar.gz` & `tmp/pyfdmss-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfdmss-0.0.5.tar", last modified: Thu Apr  4 17:10:00 2024, max compression
+gzip compressed data, was "pyfdmss-0.0.6.tar", last modified: Sun Apr  7 16:17:15 2024, max compression
```

## Comparing `pyfdmss-0.0.5.tar` & `pyfdmss-0.0.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/
--rw-r--r--   0 ananev    (1000) ananev    (1000)    35821 2023-10-30 16:40:18.000000 pyfdmss-0.0.5/LICENSE.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)      611 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/PKG-INFO
--rw-r--r--   0 ananev    (1000) ananev    (1000)       73 2024-03-30 10:52:38.000000 pyfdmss-0.0.5/README.md
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/pyfdmss.egg-info/
--rw-r--r--   0 ananev    (1000) ananev    (1000)      611 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/PKG-INFO
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1424 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/SOURCES.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)        1 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/dependency_links.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)       34 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/entry_points.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)        9 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/requires.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)       17 2024-04-04 17:10:00.000000 pyfdmss-0.0.5/pyfdmss.egg-info/top_level.txt
--rw-r--r--   0 ananev    (1000) ananev    (1000)       38 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/setup.cfg
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2273 2024-04-04 17:08:39.000000 pyfdmss-0.0.5/setup.py
-drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-04 17:10:00.646703 pyfdmss-0.0.5/src/
--rw-r--r--   0 ananev    (1000) ananev    (1000)      103 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/AccuracyOrder.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     3097 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Area3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      478 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/BoundaryArea3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1119 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CmdLineParameters.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25995 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Codegen.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1032 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Codegen.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncX.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncX.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncY.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncY.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncZ.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/CrtFuncZ.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      756 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/EnvCaseGenerator.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2221 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/EnvCaseGenerator.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     5592 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/FbcOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      732 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/FbcOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1214 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/FreeArea3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     8407 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      814 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     3823 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/InputParameters.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1086 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/InputParameters.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncX.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncX.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncY.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncY.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncZ.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/MouseFuncZ.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    10470 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1264 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    10371 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/OverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1685 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/OverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    63641 2024-03-30 12:41:45.000000 pyfdmss-0.0.5/src/OverdozenPermsolver.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     3918 2024-03-30 12:41:37.000000 pyfdmss-0.0.5/src/OverdozenPermsolver.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     8258 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/PbcOverdozenMicroperm.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1081 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/PbcOverdozenMicroperm.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1278 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/PeriodicArea3d.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2809 2024-03-30 10:24:05.000000 pyfdmss-0.0.5/src/Polynom.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      592 2024-03-30 10:20:01.000000 pyfdmss-0.0.5/src/Polynom.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     4168 2024-03-30 12:02:00.000000 pyfdmss-0.0.5/src/Slau.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      447 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/Slau.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      786 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/StuffedVoxel.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      460 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/StuffedVoxel.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)        0 2024-04-04 16:41:42.000000 pyfdmss-0.0.5/src/__init__.py
--rw-r--r--   0 ananev    (1000) ananev    (1000)      342 2024-04-04 17:04:10.000000 pyfdmss-0.0.5/src/main.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      298 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/stdafx.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)      269 2024-03-30 11:56:35.000000 pyfdmss-0.0.5/src/stdafx.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)      178 2024-04-04 15:13:08.000000 pyfdmss-0.0.5/src/testmodule.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)       45 2024-04-04 15:10:11.000000 pyfdmss-0.0.5/src/testmodule.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     2507 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinystr.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     8198 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinystr.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)    37621 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxml.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    64834 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxml.h
--rw-r--r--   0 ananev    (1000) ananev    (1000)     1791 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxmlerror.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)    37242 2024-03-30 09:57:44.000000 pyfdmss-0.0.5/src/tinyxmlparser.cpp
--rw-r--r--   0 ananev    (1000) ananev    (1000)     3306 2024-04-04 16:00:54.000000 pyfdmss-0.0.5/src/wrapper.h
+drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-07 16:17:15.848483 pyfdmss-0.0.6/
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    35821 2023-10-30 16:40:18.000000 pyfdmss-0.0.6/LICENSE.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      611 2024-04-07 16:17:15.848483 pyfdmss-0.0.6/PKG-INFO
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       73 2024-03-30 10:52:38.000000 pyfdmss-0.0.6/README.md
+drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-07 16:17:15.848483 pyfdmss-0.0.6/pyfdmss.egg-info/
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      611 2024-04-07 16:17:15.000000 pyfdmss-0.0.6/pyfdmss.egg-info/PKG-INFO
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1424 2024-04-07 16:17:15.000000 pyfdmss-0.0.6/pyfdmss.egg-info/SOURCES.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)        1 2024-04-07 16:17:15.000000 pyfdmss-0.0.6/pyfdmss.egg-info/dependency_links.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       34 2024-04-07 16:17:15.000000 pyfdmss-0.0.6/pyfdmss.egg-info/entry_points.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)        9 2024-04-07 16:17:15.000000 pyfdmss-0.0.6/pyfdmss.egg-info/requires.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       17 2024-04-07 16:17:15.000000 pyfdmss-0.0.6/pyfdmss.egg-info/top_level.txt
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       38 2024-04-07 16:17:15.848483 pyfdmss-0.0.6/setup.cfg
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1998 2024-04-07 16:17:13.000000 pyfdmss-0.0.6/setup.py
+drwxr-xr-x   0 ananev    (1000) ananev    (1000)        0 2024-04-07 16:17:15.848483 pyfdmss-0.0.6/src/
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      103 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/AccuracyOrder.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3097 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/Area3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      478 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/BoundaryArea3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1119 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/CmdLineParameters.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25995 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/Codegen.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1032 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/Codegen.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/CrtFuncX.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/CrtFuncX.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/CrtFuncY.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/CrtFuncY.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   151813 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/CrtFuncZ.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    25479 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/CrtFuncZ.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      756 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/EnvCaseGenerator.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     2221 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/EnvCaseGenerator.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     5592 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/FbcOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      732 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/FbcOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1214 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/FreeArea3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     8407 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/HorseBCOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      814 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/HorseBCOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3823 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/InputParameters.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1086 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/InputParameters.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/MouseFuncX.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/MouseFuncX.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/MouseFuncY.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/MouseFuncY.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)   170963 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/MouseFuncZ.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    34479 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/MouseFuncZ.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    10470 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/NfbcOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1264 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/NfbcOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    10371 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/OverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1685 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/OverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    63641 2024-03-30 12:41:45.000000 pyfdmss-0.0.6/src/OverdozenPermsolver.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3918 2024-03-30 12:41:37.000000 pyfdmss-0.0.6/src/OverdozenPermsolver.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     8258 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/PbcOverdozenMicroperm.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1081 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/PbcOverdozenMicroperm.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1278 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/PeriodicArea3d.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     2809 2024-03-30 10:24:05.000000 pyfdmss-0.0.6/src/Polynom.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      592 2024-03-30 10:20:01.000000 pyfdmss-0.0.6/src/Polynom.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     4168 2024-03-30 12:02:00.000000 pyfdmss-0.0.6/src/Slau.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      447 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/Slau.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      786 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/StuffedVoxel.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      460 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/StuffedVoxel.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)        0 2024-04-04 16:41:42.000000 pyfdmss-0.0.6/src/__init__.py
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      893 2024-04-07 16:13:07.000000 pyfdmss-0.0.6/src/main.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      298 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/stdafx.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      269 2024-03-30 11:56:35.000000 pyfdmss-0.0.6/src/stdafx.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)      178 2024-04-04 15:13:08.000000 pyfdmss-0.0.6/src/testmodule.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)       45 2024-04-04 15:10:11.000000 pyfdmss-0.0.6/src/testmodule.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     2507 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/tinystr.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     8198 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/tinystr.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    37621 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/tinyxml.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    64834 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/tinyxml.h
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     1791 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/tinyxmlerror.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)    37242 2024-03-30 09:57:44.000000 pyfdmss-0.0.6/src/tinyxmlparser.cpp
+-rw-r--r--   0 ananev    (1000) ananev    (1000)     3565 2024-04-07 16:02:45.000000 pyfdmss-0.0.6/src/wrapper.h
```

### Comparing `pyfdmss-0.0.5/LICENSE.txt` & `pyfdmss-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/PKG-INFO` & `pyfdmss-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfdmss
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev, Andrey Zubov
 Author-email: andrey.ananev@phystech.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyfdmss-0.0.5/pyfdmss.egg-info/PKG-INFO` & `pyfdmss-0.0.6/pyfdmss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfdmss
-Version: 0.0.5
+Version: 0.0.6
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Kirill M. Gerke, Marina V. Karsanina, Andrey A. Ananev, Andrey Zubov
 Author-email: andrey.ananev@phystech.edu
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyfdmss-0.0.5/pyfdmss.egg-info/SOURCES.txt` & `pyfdmss-0.0.6/pyfdmss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/setup.py` & `pyfdmss-0.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,35 +16,29 @@
 import sys
 
 is_64bits = sys.maxsize > 2**32
 
 from setuptools.command.build_ext import build_ext as build_ext_orig
 
 
-version = "0.0.5"
+version = "0.0.6"
 libName = "pyfdmss"
 
 file_dir_path = os.path.dirname(os.path.realpath(__file__))
 
 
 def package_files(directory):
     return [
         os.path.join(p, f)
         for p, d, files in os.walk(directory)
         for f in files
         if ".cpp" in f
     ]
 
 
-# extra_link_args=['-std=c++11','_GLIBCXX_USE_CXX11_ABI=0']
-# extraFlags=['-fpermissive','-std=c++11']
-# os.environ["CXX"] = "g++"
-# os.environ["CC"] = "gcc"
-# print("package_files = ", package_files("./pyfdmss/src/"))
-
 extra_compile_args = ["-O3", "-w", "-std=c++11", "-fopenmp"]
 installRequiresList = ["pybind11"]
 entry_points_Command = {"main_library": ["run = pyfdmss:run"]}
 
 pyfdmss_module = Extension(
     libName,
     sources=package_files("./src/"),
@@ -71,10 +65,9 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Education",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
         "Programming Language :: C++",
         "Programming Language :: Python :: 3 :: Only",
-        # 'Operating System :: OS Independent',
     ],
 )
```

### Comparing `pyfdmss-0.0.5/src/Area3d.h` & `pyfdmss-0.0.6/src/Area3d.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/CmdLineParameters.h` & `pyfdmss-0.0.6/src/CmdLineParameters.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/Codegen.cpp` & `pyfdmss-0.0.6/src/Codegen.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/Codegen.h` & `pyfdmss-0.0.6/src/Codegen.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/CrtFuncX.cpp` & `pyfdmss-0.0.6/src/CrtFuncX.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/CrtFuncX.h` & `pyfdmss-0.0.6/src/CrtFuncX.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/CrtFuncY.cpp` & `pyfdmss-0.0.6/src/CrtFuncY.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/CrtFuncY.h` & `pyfdmss-0.0.6/src/CrtFuncY.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/CrtFuncZ.cpp` & `pyfdmss-0.0.6/src/CrtFuncZ.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/CrtFuncZ.h` & `pyfdmss-0.0.6/src/CrtFuncZ.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/EnvCaseGenerator.cpp` & `pyfdmss-0.0.6/src/EnvCaseGenerator.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/EnvCaseGenerator.h` & `pyfdmss-0.0.6/src/EnvCaseGenerator.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/FbcOverdozenMicroperm.cpp` & `pyfdmss-0.0.6/src/FbcOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/FbcOverdozenMicroperm.h` & `pyfdmss-0.0.6/src/FbcOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/FreeArea3d.h` & `pyfdmss-0.0.6/src/FreeArea3d.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.cpp` & `pyfdmss-0.0.6/src/HorseBCOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/HorseBCOverdozenMicroperm.h` & `pyfdmss-0.0.6/src/HorseBCOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/InputParameters.cpp` & `pyfdmss-0.0.6/src/InputParameters.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/InputParameters.h` & `pyfdmss-0.0.6/src/InputParameters.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/MouseFuncX.cpp` & `pyfdmss-0.0.6/src/MouseFuncX.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/MouseFuncX.h` & `pyfdmss-0.0.6/src/MouseFuncX.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/MouseFuncY.cpp` & `pyfdmss-0.0.6/src/MouseFuncY.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/MouseFuncY.h` & `pyfdmss-0.0.6/src/MouseFuncY.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/MouseFuncZ.cpp` & `pyfdmss-0.0.6/src/MouseFuncZ.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/MouseFuncZ.h` & `pyfdmss-0.0.6/src/MouseFuncZ.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.cpp` & `pyfdmss-0.0.6/src/NfbcOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/NfbcOverdozenMicroperm.h` & `pyfdmss-0.0.6/src/NfbcOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/OverdozenMicroperm.cpp` & `pyfdmss-0.0.6/src/OverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/OverdozenMicroperm.h` & `pyfdmss-0.0.6/src/OverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/OverdozenPermsolver.cpp` & `pyfdmss-0.0.6/src/OverdozenPermsolver.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/OverdozenPermsolver.h` & `pyfdmss-0.0.6/src/OverdozenPermsolver.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/PbcOverdozenMicroperm.cpp` & `pyfdmss-0.0.6/src/PbcOverdozenMicroperm.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/PbcOverdozenMicroperm.h` & `pyfdmss-0.0.6/src/PbcOverdozenMicroperm.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/PeriodicArea3d.h` & `pyfdmss-0.0.6/src/PeriodicArea3d.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/Polynom.cpp` & `pyfdmss-0.0.6/src/Polynom.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/Polynom.h` & `pyfdmss-0.0.6/src/Polynom.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/Slau.cpp` & `pyfdmss-0.0.6/src/Slau.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/StuffedVoxel.cpp` & `pyfdmss-0.0.6/src/StuffedVoxel.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/tinystr.cpp` & `pyfdmss-0.0.6/src/tinystr.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/tinystr.h` & `pyfdmss-0.0.6/src/tinystr.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/tinyxml.cpp` & `pyfdmss-0.0.6/src/tinyxml.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/tinyxml.h` & `pyfdmss-0.0.6/src/tinyxml.h`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/tinyxmlerror.cpp` & `pyfdmss-0.0.6/src/tinyxmlerror.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/tinyxmlparser.cpp` & `pyfdmss-0.0.6/src/tinyxmlparser.cpp`

 * *Files identical despite different names*

### Comparing `pyfdmss-0.0.5/src/wrapper.h` & `pyfdmss-0.0.6/src/wrapper.h`

 * *Files 22% similar despite different names*

```diff
@@ -65,26 +65,32 @@
 
 	ps.printVelPrsFieldsCustom(output_fnames);
 
 	doc.LinkEndChild(rootElem);
 	doc.SaveFile(io_filenames->summaryFileName);
 }
 
-void run(std::string config_path, std::string image_path, std::string summary_path,
-         std::string velx_path, std::string vely_path, std::string velz_path,
-         std::string pressure_path, std::string full_vel_path, std::string comp_vel_path,
-         std::string log_path) {
+void run(std::string config_path = std::string("config.xml"), 
+		 std::string image_path = std::string("image3d.raw"),
+		 std::string summary_path = std::string("output.txt"),
+         std::string velx_path = std::string("/dev/null"), 
+		 std::string vely_path = std::string("/dev/null"), 
+		 std::string velz_path = std::string("/dev/null"),
+         std::string pressure_path = std::string("/dev/null"),
+		 std::string full_vel_path = std::string("/dev/null"), 
+		 std::string comp_vel_path = std::string("/dev/null"),
+         std::string log_path = std::string("/dev/null")) {
 
-  CmdLineParameters io_filenames (
-      config_path.data(),
-      image_path.data(),
-      summary_path.data(),
-      velx_path.data(),
-      vely_path.data(),
-      velz_path.data(),
-      pressure_path.data(),
-      full_vel_path.data(),
-      comp_vel_path.data(),
-      log_path.data());
-  SolveImpl(&io_filenames);
-  return;
+	CmdLineParameters io_filenames (
+		config_path.data(),
+		image_path.data(),
+		summary_path.data(),
+		velx_path.data(),
+		vely_path.data(),
+		velz_path.data(),
+		pressure_path.data(),
+		full_vel_path.data(),
+		comp_vel_path.data(),
+		log_path.data());
+	SolveImpl(&io_filenames);
+	return;
 }
```

