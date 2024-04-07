# Comparing `tmp/uiautomator2-3.0.5.tar.gz` & `tmp/uiautomator2-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uiautomator2-3.0.5.tar", max compression
+gzip compressed data, was "uiautomator2-3.0.6.tar", max compression
```

## Comparing `uiautomator2-3.0.5.tar` & `uiautomator2-3.0.6.tar`

### file list

```diff
@@ -1,43 +1,46 @@
--rw-r--r--   0        0        0     1064 2024-04-04 14:51:55.415653 uiautomator2-3.0.5/LICENSE
--rw-r--r--   0        0        0    53306 2024-04-04 14:51:55.419653 uiautomator2-3.0.5/README.md
--rw-r--r--   0        0        0     1032 2024-04-04 14:52:09.127554 uiautomator2-3.0.5/pyproject.toml
--rw-r--r--   0        0        0    68753 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/__init__.py
--rw-r--r--   0        0        0     7964 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/__main__.py
--rw-r--r--   0        0        0      289 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/_proto.py
--rw-r--r--   0        0        0    21287 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/_selector.py
--rw-r--r--   0        0        0      647 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/abcd.py
--rw-r--r--   0        0        0  1061950 2024-04-04 14:52:08.183558 uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator-test.apk
--rw-r--r--   0        0        0  2191186 2024-04-04 14:52:08.011560 uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator.apk
--rwxr-xr-x   0        0        0      570 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/assets/sync.sh
--rw-r--r--   0        0        0     2602 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/__init__.py
--rw-r--r--   0        0        0      405 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/README.md
--rw-r--r--   0        0        0     5574 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/__init__.py
--rw-r--r--   0        0        0     4802 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/index.html
--rw-r--r--   0        0        0    61137 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/pig.jpg
--rw-r--r--   0        0        0     1100 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
--rw-r--r--   0        0        0       29 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/start.bat
--rw-r--r--   0        0        0     2645 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/info/__init__.py
--rw-r--r--   0        0        0    28515 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/info/conf.py
--rw-r--r--   0        0        0     2852 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/README.md
--rw-r--r--   0        0        0    12384 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/__init__.py
--rw-r--r--   0        0        0    41467 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/net.png
--rw-r--r--   0        0        0    26928 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext/perf/summary.png
--rw-r--r--   0        0        0     4180 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/README.md
--rw-r--r--   0        0        0    18456 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/__init__.py
--rw-r--r--   0        0        0      947 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/README.md
--rw-r--r--   0        0        0     2495 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/__init__.py
--rw-r--r--   0        0        0     3308 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/baiduOCR.py
--rw-r--r--   0        0        0    10476 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/image.py
--rw-r--r--   0        0        0    14731 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/init.py
--rw-r--r--   0        0        0     1801 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/messagebox.py
--rw-r--r--   0        0        0     3776 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/screenrecord.py
--rw-r--r--   0        0        0     3342 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/settings.py
--rw-r--r--   0        0        0     1762 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/swipe.py
--rw-r--r--   0        0        0     5856 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/utils.py
--rw-r--r--   0        0        0     4780 2024-04-04 14:52:09.131554 uiautomator2-3.0.5/uiautomator2/version.py
--rw-r--r--   0        0        0     9456 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/watcher.py
--rw-r--r--   0        0        0     6710 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/webview.py
--rw-r--r--   0        0        0    14389 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/widget.py
--rw-r--r--   0        0        0    23845 2024-04-04 14:51:55.423653 uiautomator2-3.0.5/uiautomator2/xpath.py
--rw-r--r--   0        0        0    54208 1970-01-01 00:00:00.000000 uiautomator2-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 09:30:42.009248 uiautomator2-3.0.6/LICENSE
+-rw-r--r--   0        0        0    53306 2024-04-07 09:30:42.009248 uiautomator2-3.0.6/README.md
+-rw-r--r--   0        0        0     1028 2024-04-07 09:30:56.029267 uiautomator2-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0    68753 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/__init__.py
+-rw-r--r--   0        0        0     8063 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/__main__.py
+-rw-r--r--   0        0        0      289 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/_proto.py
+-rw-r--r--   0        0        0    21287 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/_selector.py
+-rw-r--r--   0        0        0      647 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/abcd.py
+-rw-r--r--   0        0        0       27 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/assets/.gitignore
+-rw-r--r--   0        0        0  1061950 2024-04-07 09:30:55.109266 uiautomator2-3.0.6/uiautomator2/assets/app-uiautomator-test.apk
+-rw-r--r--   0        0        0  2191186 2024-04-07 09:30:54.873265 uiautomator2-3.0.6/uiautomator2/assets/app-uiautomator.apk
+-rwxr-xr-x   0        0        0 10092696 2024-04-07 08:30:35.000000 uiautomator2-3.0.6/uiautomator2/assets/atx-agent
+-rwxr-xr-x   0        0        0      886 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/assets/sync.sh
+-rw-r--r--   0        0        0       80 2024-04-07 09:30:55.133266 uiautomator2-3.0.6/uiautomator2/assets/version.txt
+-rw-r--r--   0        0        0     2602 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/__init__.py
+-rw-r--r--   0        0        0      405 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/htmlreport/README.md
+-rw-r--r--   0        0        0     5574 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/htmlreport/__init__.py
+-rw-r--r--   0        0        0     4802 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/htmlreport/assets/index.html
+-rw-r--r--   0        0        0    61137 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/htmlreport/assets/pig.jpg
+-rw-r--r--   0        0        0     1100 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/htmlreport/assets/simplehttpserver.py
+-rw-r--r--   0        0        0       29 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/htmlreport/assets/start.bat
+-rw-r--r--   0        0        0     2645 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/info/__init__.py
+-rw-r--r--   0        0        0    28515 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/info/conf.py
+-rw-r--r--   0        0        0     2852 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/perf/README.md
+-rw-r--r--   0        0        0    12384 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/perf/__init__.py
+-rw-r--r--   0        0        0    41467 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/perf/net.png
+-rw-r--r--   0        0        0    26928 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext/perf/summary.png
+-rw-r--r--   0        0        0     4180 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext-archived/aircv/README.md
+-rw-r--r--   0        0        0    18456 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext-archived/aircv/__init__.py
+-rw-r--r--   0        0        0      947 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext-archived/ocr/README.md
+-rw-r--r--   0        0        0     2495 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext-archived/ocr/__init__.py
+-rw-r--r--   0        0        0     3308 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/ext-archived/ocr/baiduOCR.py
+-rw-r--r--   0        0        0    10476 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/image.py
+-rw-r--r--   0        0        0    15094 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/init.py
+-rw-r--r--   0        0        0     1801 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/messagebox.py
+-rw-r--r--   0        0        0     3776 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/screenrecord.py
+-rw-r--r--   0        0        0     3342 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/settings.py
+-rw-r--r--   0        0        0     1762 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/swipe.py
+-rw-r--r--   0        0        0     5856 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/utils.py
+-rw-r--r--   0        0        0     4908 2024-04-07 09:30:56.029267 uiautomator2-3.0.6/uiautomator2/version.py
+-rw-r--r--   0        0        0     9456 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/watcher.py
+-rw-r--r--   0        0        0     6710 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/webview.py
+-rw-r--r--   0        0        0    14389 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/widget.py
+-rw-r--r--   0        0        0    23845 2024-04-07 09:30:42.017248 uiautomator2-3.0.6/uiautomator2/xpath.py
+-rw-r--r--   0        0        0    54208 1970-01-01 00:00:00.000000 uiautomator2-3.0.6/PKG-INFO
```

### Comparing `uiautomator2-3.0.5/LICENSE` & `uiautomator2-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/README.md` & `uiautomator2-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/pyproject.toml` & `uiautomator2-3.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "uiautomator2"
-version = "3.0.5"
+version = "3.0.6"
 description = "automator for anroid device"
 homepage = "https://github.com/openatx/uiautomator2"
 authors = ["codeskyblue <codeskyblue@gmail.com>"]
 license = "MIT"
 readme = "README.md"
-include = ["*/assets/*.apk"]
+include = ["*/assets/*"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "*"
 lxml = "*"
 adbutils = "^2.2.3"
 retry = ">=0,<1"
```

### Comparing `uiautomator2-3.0.5/uiautomator2/__init__.py` & `uiautomator2-3.0.6/uiautomator2/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/__main__.py` & `uiautomator2-3.0.6/uiautomator2/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 import json
 import logging
 
 import adbutils
 
 import uiautomator2 as u2
 
-from .init import Initer
-from .version import __version__
+from uiautomator2.init import Initer
+from uiautomator2.version import __version__
+from uiautomator2 import enable_pretty_logging
 
 
 logger = logging.getLogger(__name__)
 
 def cmd_init(args):
     serial = args.serial or args.serial_optional
     if serial:
@@ -134,14 +135,15 @@
 def cmd_version(args):
     print("uiautomator2 version: %s" % __version__)
 
 
 def cmd_console(args):
     import code
     import platform
+    enable_pretty_logging()
 
     d = u2.connect(args.serial)
     model = d.shell("getprop ro.product.model").output.strip()
     serial = d.serial
     try:
         import IPython
         from traitlets.config import get_config
```

### Comparing `uiautomator2-3.0.5/uiautomator2/_selector.py` & `uiautomator2-3.0.6/uiautomator2/_selector.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/abcd.py` & `uiautomator2-3.0.6/uiautomator2/abcd.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator-test.apk` & `uiautomator2-3.0.6/uiautomator2/assets/app-uiautomator-test.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/assets/app-uiautomator.apk` & `uiautomator2-3.0.6/uiautomator2/assets/app-uiautomator.apk`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/exceptions.py` & `uiautomator2-3.0.6/uiautomator2/exceptions.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/__init__.py` & `uiautomator2-3.0.6/uiautomator2/ext/htmlreport/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/index.html` & `uiautomator2-3.0.6/uiautomator2/ext/htmlreport/assets/index.html`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/pig.jpg` & `uiautomator2-3.0.6/uiautomator2/ext/htmlreport/assets/pig.jpg`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/htmlreport/assets/simplehttpserver.py` & `uiautomator2-3.0.6/uiautomator2/ext/htmlreport/assets/simplehttpserver.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/info/__init__.py` & `uiautomator2-3.0.6/uiautomator2/ext/info/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/info/conf.py` & `uiautomator2-3.0.6/uiautomator2/ext/info/conf.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/perf/README.md` & `uiautomator2-3.0.6/uiautomator2/ext/perf/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/perf/__init__.py` & `uiautomator2-3.0.6/uiautomator2/ext/perf/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/perf/net.png` & `uiautomator2-3.0.6/uiautomator2/ext/perf/net.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext/perf/summary.png` & `uiautomator2-3.0.6/uiautomator2/ext/perf/summary.png`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/README.md` & `uiautomator2-3.0.6/uiautomator2/ext-archived/aircv/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext-archived/aircv/__init__.py` & `uiautomator2-3.0.6/uiautomator2/ext-archived/aircv/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/README.md` & `uiautomator2-3.0.6/uiautomator2/ext-archived/ocr/README.md`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/__init__.py` & `uiautomator2-3.0.6/uiautomator2/ext-archived/ocr/__init__.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/ext-archived/ocr/baiduOCR.py` & `uiautomator2-3.0.6/uiautomator2/ext-archived/ocr/baiduOCR.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/image.py` & `uiautomator2-3.0.6/uiautomator2/image.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/init.py` & `uiautomator2-3.0.6/uiautomator2/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # coding: utf-8
 #
 
 import datetime
 import hashlib
 import logging
 import os
+from pathlib import Path
 import shutil
 import tarfile
 
 import adbutils
 import progress.bar
 import requests
 from retry import retry
@@ -18,14 +19,15 @@
 
 appdir = os.path.join(os.path.expanduser("~"), '.uiautomator2')
 
 GITHUB_BASEURL = "https://github.com/openatx"
 
 
 logger = logging.getLogger(__name__)
+assets_dir = Path(__file__).absolute().parent.joinpath("assets")
 
 class DownloadBar(progress.bar.PixelBar):
     message = "Downloading"
     suffix = '%(current_size)s/%(total_size)s'
     width = 10
 
     @property
@@ -329,22 +331,28 @@
     def _install_jars(self):
         """ use uiautomator 1.0 to run uiautomator test """
         for (name, url) in self.jar_urls:
             self.push_url(url, "/data/local/tmp/" + name, mode=0o644)
 
     def _install_atx_agent(self):
         logger.info("Install atx-agent %s", __atx_agent_version__)
+        if 'armeabi' in self.abis:
+            local_atx_agent_path = assets_dir.joinpath("atx-agent")
+            if local_atx_agent_path.exists():
+                logger.info("Use local atx-agent[armeabi]: %s", local_atx_agent_path)
+                dest = '/data/local/tmp/atx-agent'
+                self._device.sync.push(local_atx_agent_path, dest, mode=0o755)
+                return
         self.push_url(self.atx_agent_url, tgz=True, extract_name="atx-agent")
 
     def setup_atx_agent(self):
         # stop atx-agent first
         self.shell(self.atx_agent_path, "server", "--stop")
         if self.is_atx_agent_outdated():
-            logger.info("Install atx-agent %s", __atx_agent_version__)
-            self.push_url(self.atx_agent_url, tgz=True, extract_name="atx-agent")
+            self._install_atx_agent()
         
         self.shell(self.atx_agent_path, 'server', '--nouia', '-d', "--addr", self.__atx_listen_addr)
         logger.info("Check atx-agent version")
         self.check_atx_agent_version()
 
     @retry(
         (requests.ConnectionError, requests.ReadTimeout, requests.HTTPError),
```

### Comparing `uiautomator2-3.0.5/uiautomator2/messagebox.py` & `uiautomator2-3.0.6/uiautomator2/messagebox.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/screenrecord.py` & `uiautomator2-3.0.6/uiautomator2/screenrecord.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/settings.py` & `uiautomator2-3.0.6/uiautomator2/settings.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/swipe.py` & `uiautomator2-3.0.6/uiautomator2/swipe.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/utils.py` & `uiautomator2-3.0.6/uiautomator2/utils.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/version.py` & `uiautomator2-3.0.6/uiautomator2/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 #
 
 # version managed by poetry
-__version__ = "3.0.5"
+__version__ = "3.0.6"
 
 # See ChangeLog for details
 
 __apk_version__ = '2.3.3'
 # 2.3.3 make float windows smaller
 # 2.3.2 merge pull requests # require atx-agent>=0.10.0
 # 2.3.1 support minicapagent, rotationagent, minitouchagent
@@ -35,15 +35,16 @@
 # 1.0.9 fix apk version code and version name
 # ERR: 1.0.8 bad version number. show ip on notification
 # ERR: 1.0.7 bad version number. new input method, some bug fix
 
 __jar_version__ = 'v0.1.6'  # no useless for now.
 # v0.1.6 first release version
 
-__atx_agent_version__ = '0.10.0'
+__atx_agent_version__ = '0.10.1' # sync.sh verison should also be updated
+# 0.10.1 update androidbinary version, https://github.com/openatx/atx-agent/issues/115
 # 0.10.0 remove tunnel code, use androidx.test.runner
 # 0.9.6 fix security reason for remote control device
 # 0.9.5 log support rotate, prevent log too large
 # 0.9.4 test travis push to qiniu-cdn
 # 0.9.3 fix atx-agent version output too many output
 # 0.9.2 fix when /sdcard/atx-agent.log can't create, atx-agent can't start error
 # 0.9.1 update /minicap to use apkagent and minicap
```

### Comparing `uiautomator2-3.0.5/uiautomator2/watcher.py` & `uiautomator2-3.0.6/uiautomator2/watcher.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/webview.py` & `uiautomator2-3.0.6/uiautomator2/webview.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/widget.py` & `uiautomator2-3.0.6/uiautomator2/widget.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/uiautomator2/xpath.py` & `uiautomator2-3.0.6/uiautomator2/xpath.py`

 * *Files identical despite different names*

### Comparing `uiautomator2-3.0.5/PKG-INFO` & `uiautomator2-3.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uiautomator2
-Version: 3.0.5
+Version: 3.0.6
 Summary: automator for anroid device
 Home-page: https://github.com/openatx/uiautomator2
 License: MIT
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

