# Comparing `tmp/LyPythonToolbox-0.1.2.tar.gz` & `tmp/LyPythonToolbox-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LyPythonToolbox-0.1.2.tar", last modified: Fri Apr  5 12:04:55 2024, max compression
+gzip compressed data, was "LyPythonToolbox-0.1.3.tar", last modified: Sun Apr  7 10:39:25 2024, max compression
```

## Comparing `LyPythonToolbox-0.1.2.tar` & `LyPythonToolbox-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-05 12:04:55.629965 LyPythonToolbox-0.1.2/
--rw-rw-r--   0 luna       (501) staff       (20)     1098 2024-03-31 18:06:51.000000 LyPythonToolbox-0.1.2/LICENSE
--rw-r--r--   0 luna       (501) staff       (20)      514 2024-04-05 12:04:55.629783 LyPythonToolbox-0.1.2/PKG-INFO
--rw-rw-r--   0 luna       (501) staff       (20)       64 2024-04-05 10:28:08.000000 LyPythonToolbox-0.1.2/README.md
--rw-r--r--   0 luna       (501) staff       (20)       38 2024-04-05 12:04:55.630034 LyPythonToolbox-0.1.2/setup.cfg
--rw-r--r--   0 luna       (501) staff       (20)     1350 2024-04-05 12:04:41.000000 LyPythonToolbox-0.1.2/setup.py
-drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-05 12:04:55.627517 LyPythonToolbox-0.1.2/src/
-drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-05 12:04:55.628842 LyPythonToolbox-0.1.2/src/LyPythonToolbox/
--rw-------   0 luna       (501) staff       (20)     2289 2024-04-05 10:38:54.000000 LyPythonToolbox-0.1.2/src/LyPythonToolbox/Util_configdict.py
--rw-rw-r--   0 luna       (501) staff       (20)       82 2024-04-05 10:39:15.000000 LyPythonToolbox-0.1.2/src/LyPythonToolbox/__init__.py
--rw-r--r--   0 luna       (501) staff       (20)      134 2024-04-05 10:34:43.000000 LyPythonToolbox-0.1.2/src/LyPythonToolbox/print_tricks.py
-drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-05 12:04:55.629547 LyPythonToolbox-0.1.2/src/LyPythonToolbox.egg-info/
--rw-r--r--   0 luna       (501) staff       (20)      514 2024-04-05 12:04:55.000000 LyPythonToolbox-0.1.2/src/LyPythonToolbox.egg-info/PKG-INFO
--rw-r--r--   0 luna       (501) staff       (20)      305 2024-04-05 12:04:55.000000 LyPythonToolbox-0.1.2/src/LyPythonToolbox.egg-info/SOURCES.txt
--rw-r--r--   0 luna       (501) staff       (20)        1 2024-04-05 12:04:55.000000 LyPythonToolbox-0.1.2/src/LyPythonToolbox.egg-info/dependency_links.txt
--rw-r--r--   0 luna       (501) staff       (20)       16 2024-04-05 12:04:55.000000 LyPythonToolbox-0.1.2/src/LyPythonToolbox.egg-info/top_level.txt
+drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-07 10:39:25.886237 LyPythonToolbox-0.1.3/
+-rw-rw-r--   0 luna       (501) staff       (20)     1098 2024-03-31 18:06:51.000000 LyPythonToolbox-0.1.3/LICENSE
+-rw-r--r--   0 luna       (501) staff       (20)      515 2024-04-07 10:39:25.886075 LyPythonToolbox-0.1.3/PKG-INFO
+-rw-rw-r--   0 luna       (501) staff       (20)       65 2024-04-05 12:13:31.000000 LyPythonToolbox-0.1.3/README.md
+-rw-r--r--   0 luna       (501) staff       (20)       38 2024-04-07 10:39:25.886303 LyPythonToolbox-0.1.3/setup.cfg
+-rw-r--r--   0 luna       (501) staff       (20)     1350 2024-04-07 10:39:19.000000 LyPythonToolbox-0.1.3/setup.py
+drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-07 10:39:25.883920 LyPythonToolbox-0.1.3/src/
+drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-07 10:39:25.885177 LyPythonToolbox-0.1.3/src/LyPythonToolbox/
+-rw-------   0 luna       (501) staff       (20)     2289 2024-04-05 10:38:54.000000 LyPythonToolbox-0.1.3/src/LyPythonToolbox/Util_configdict.py
+-rw-rw-r--   0 luna       (501) staff       (20)       82 2024-04-05 10:39:15.000000 LyPythonToolbox-0.1.3/src/LyPythonToolbox/__init__.py
+-rw-r--r--   0 luna       (501) staff       (20)     1341 2024-04-07 10:38:04.000000 LyPythonToolbox-0.1.3/src/LyPythonToolbox/print_tricks.py
+drwxr-xr-x   0 luna       (501) staff       (20)        0 2024-04-07 10:39:25.885818 LyPythonToolbox-0.1.3/src/LyPythonToolbox.egg-info/
+-rw-r--r--   0 luna       (501) staff       (20)      515 2024-04-07 10:39:25.000000 LyPythonToolbox-0.1.3/src/LyPythonToolbox.egg-info/PKG-INFO
+-rw-r--r--   0 luna       (501) staff       (20)      305 2024-04-07 10:39:25.000000 LyPythonToolbox-0.1.3/src/LyPythonToolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 luna       (501) staff       (20)        1 2024-04-07 10:39:25.000000 LyPythonToolbox-0.1.3/src/LyPythonToolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 luna       (501) staff       (20)       16 2024-04-07 10:39:25.000000 LyPythonToolbox-0.1.3/src/LyPythonToolbox.egg-info/top_level.txt
```

### Comparing `LyPythonToolbox-0.1.2/LICENSE` & `LyPythonToolbox-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LyPythonToolbox-0.1.2/PKG-INFO` & `LyPythonToolbox-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: LyPythonToolbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ly's personal python toolbox.
 Home-page: https://github.com/YueLin301/LyPythonToolbox
 Author: Yue Lin
 Author-email: linyue3h1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-See [my blog](https://yuelin301.github.io/posts/Python-Toolbox).
+See [my blog](https://yuelin301.github.io/posts/LyPythonToolbox).
```

### Comparing `LyPythonToolbox-0.1.2/setup.py` & `LyPythonToolbox-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name                          = "LyPythonToolbox",                              # 包名
-    version                       = "0.1.2",                                        # 版本号
+    version                       = "0.1.3",                                        # 版本号
     author                        = "Yue Lin",                                      # 作者名字
     author_email                  = "linyue3h1@gmail.com",                          # 作者邮箱
     description                   = "Ly's personal python toolbox.",                # 简短描述
     long_description              = open("README.md").read(),                       # 长描述，通常是README文件
     long_description_content_type = "text/markdown",                                # 长描述内容的格式，这里为Markdown
     url                           = "https://github.com/YueLin301/LyPythonToolbox", # 项目的URL，通常是GitHub的URL
     packages                      = find_packages(where='src'),
```

### Comparing `LyPythonToolbox-0.1.2/src/LyPythonToolbox/Util_configdict.py` & `LyPythonToolbox-0.1.3/src/LyPythonToolbox/Util_configdict.py`

 * *Files identical despite different names*

### Comparing `LyPythonToolbox-0.1.2/src/LyPythonToolbox.egg-info/PKG-INFO` & `LyPythonToolbox-0.1.3/src/LyPythonToolbox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: LyPythonToolbox
-Version: 0.1.2
+Version: 0.1.3
 Summary: Ly's personal python toolbox.
 Home-page: https://github.com/YueLin301/LyPythonToolbox
 Author: Yue Lin
 Author-email: linyue3h1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-See [my blog](https://yuelin301.github.io/posts/Python-Toolbox).
+See [my blog](https://yuelin301.github.io/posts/LyPythonToolbox).
```

