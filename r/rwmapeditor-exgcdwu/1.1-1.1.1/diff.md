# Comparing `tmp/rwmapeditor_exgcdwu-1.1.tar.gz` & `tmp/rwmapeditor_exgcdwu-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwmapeditor_exgcdwu-1.1.tar", last modified: Sun Apr  7 13:53:04 2024, max compression
+gzip compressed data, was "rwmapeditor_exgcdwu-1.1.1.tar", last modified: Sun Apr  7 14:02:37 2024, max compression
```

## Comparing `rwmapeditor_exgcdwu-1.1.tar` & `rwmapeditor_exgcdwu-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/_case/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/_layer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/_objectgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_case/_tileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_default_data.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/_frame/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/_element_ori.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_frame/_element_property.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmap/_util/
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_class_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_etElement_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_png_rel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/rwmap/_util/_str_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:53:04.009264 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-07 13:53:03.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 13:53:04.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:53:03.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 13:53:03.000000 rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-07 13:53:04.013264 rwmapeditor_exgcdwu-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-07 13:52:47.000000 rwmapeditor_exgcdwu-1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/rwmap/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/rwmap/_case/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_case/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_case/_layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_case/_objectgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_case/_tileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_default_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/rwmap/_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_frame/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_frame/_element_ori.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_frame/_element_property.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/rwmap/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_util/_class_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_util/_etElement_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_util/_png_rel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/rwmap/_util/_str_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/rwmapeditor_exgcdwu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-07 14:02:37.000000 rwmapeditor_exgcdwu-1.1.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-07 14:02:37.000000 rwmapeditor_exgcdwu-1.1.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:02:37.000000 rwmapeditor_exgcdwu-1.1.1/rwmapeditor_exgcdwu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-07 14:02:37.000000 rwmapeditor_exgcdwu-1.1.1/rwmapeditor_exgcdwu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-07 14:02:37.519303 rwmapeditor_exgcdwu-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-07 14:02:18.000000 rwmapeditor_exgcdwu-1.1.1/setup.py
```

### Comparing `rwmapeditor_exgcdwu-1.1/LICENSE` & `rwmapeditor_exgcdwu-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/PKG-INFO` & `rwmapeditor_exgcdwu-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.1
+Version: 1.1.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rwmapeditor-exgcdwu
-___一个铁锈战争(Rusted Warfare)地图编辑python库___
+___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
-[![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)][pypi]
-[![license](https://img.shields.io/github/license/Gsllchb/rwmapeditor-exgcdwu.svg)][license]
+![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
 ## 安装
 
+```console
 pip install rwmapeditor-exgcdwu
+```
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
 map_name = 'example_mission.tmx'
```

### Comparing `rwmapeditor_exgcdwu-1.1/README.md` & `rwmapeditor_exgcdwu-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # rwmapeditor-exgcdwu
-___一个铁锈战争(Rusted Warfare)地图编辑python库___
+___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
-[![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)][pypi]
-[![license](https://img.shields.io/github/license/Gsllchb/rwmapeditor-exgcdwu.svg)][license]
+![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
 ## 安装
 
+```console
 pip install rwmapeditor-exgcdwu
+```
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
 map_name = 'example_mission.tmx'
```

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_case/_layer.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_case/_layer.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_case/_objectgroup.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_case/_objectgroup.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_case/_tileset.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_case/_tileset.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_core.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_core.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_frame/_coordinate.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_frame/_coordinate.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_frame/_element_property.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_frame/_element_property.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_util/__init__.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_util/__init__.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_util/_etElement_process.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_util/_etElement_process.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmap/_util/_str_util.py` & `rwmapeditor_exgcdwu-1.1.1/rwmap/_util/_str_util.py`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO` & `rwmapeditor_exgcdwu-1.1.1/rwmapeditor_exgcdwu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 Metadata-Version: 2.1
 Name: rwmapeditor_exgcdwu
-Version: 1.1
+Version: 1.1.1
 Home-page: https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-
 Author: exgcdwu
 Author-email: 1006605318@qq.com
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rwmapeditor-exgcdwu
-___一个铁锈战争(Rusted Warfare)地图编辑python库___
+___一个铁锈战争 (Rusted Warfare) 地图编辑 python 库___
 
-[![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)][pypi]
-[![license](https://img.shields.io/github/license/Gsllchb/rwmapeditor-exgcdwu.svg)][license]
+![released version](https://img.shields.io/pypi/v/rwmapeditor-exgcdwu.svg)
 
 ## 目标
 
 python实现铁锈地图文件地块编辑和宾语编辑。
 
 暂时不打算接触地块集。
 
 重点减轻城市争夺地图的宾语编辑工作量
 
 基本框架已完成。
 
 ## 安装
 
+```console
 pip install rwmapeditor-exgcdwu
+```
 
 ## 简易使用例子
 
 ```python
 # coding: utf-8
 map_dir = 'D:/Game/steam/steamapps/common/Rusted Warfare/mods/maps/'
 map_name = 'example_mission.tmx'
```

### Comparing `rwmapeditor_exgcdwu-1.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt` & `rwmapeditor_exgcdwu-1.1.1/rwmapeditor_exgcdwu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rwmapeditor_exgcdwu-1.1/setup.py` & `rwmapeditor_exgcdwu-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # setup.py
 
 #import os
 from setuptools import setup, find_packages
 
-__version__ = '1.1'
+__version__ = '1.1.1'
 #current_dir = os.path.dirname(__file__)
 #requirements = open(current_dir + '/requirements.txt').readlines()
 
 def readme():
     with open('README.md') as file:
         return file.read()
 
@@ -17,11 +17,11 @@
     name = 'rwmapeditor_exgcdwu',
     version = __version__,
     author = 'exgcdwu',
     author_email = '1006605318@qq.com',
     url = "https://github.com/exgcdwu/Rusted-Warfare-map-editor-for-city-occupation-play-",
     long_description = strreadme,
     long_description_content_type = "text/markdown",
-    packages = find_packages(exclude=["tests"]),
+    packages = find_packages(exclude=["tests", "rwmap_data"]),
     python_requires = '>=3.0.0'
     #,install_requires = requirements
 )
```

