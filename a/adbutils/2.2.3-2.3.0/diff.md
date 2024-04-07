# Comparing `tmp/adbutils-2.2.3.tar.gz` & `tmp/adbutils-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.2.3.tar", last modified: Sun Mar 24 11:25:18 2024, max compression
+gzip compressed data, was "adbutils-2.3.0.tar", last modified: Sun Apr  7 12:31:00 2024, max compression
```

## Comparing `adbutils-2.2.3.tar` & `adbutils-2.3.0.tar`

### file list

```diff
@@ -1,50 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.150401 adbutils-2.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.146402 adbutils-2.2.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-24 11:25:12.000000 adbutils-2.2.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.146402 adbutils-2.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-24 11:25:12.000000 adbutils-2.2.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-03-24 11:25:12.000000 adbutils-2.2.3/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-24 11:25:18.000000 adbutils-2.2.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-03-24 11:25:18.000000 adbutils-2.2.3/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-24 11:25:12.000000 adbutils-2.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-24 11:25:18.150401 adbutils-2.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14311 2024-03-24 11:25:12.000000 adbutils-2.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.150401 adbutils-2.2.3/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3396 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11931 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    51160 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7372 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.150401 adbutils-2.2.3/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12871 2024-03-24 11:25:12.000000 adbutils-2.2.3/adbutils/pidcat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.150401 adbutils-2.2.3/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-03-24 11:25:18.000000 adbutils-2.2.3/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-03-24 11:25:18.000000 adbutils-2.2.3/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 11:25:18.000000 adbutils-2.2.3/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 11:25:18.000000 adbutils-2.2.3/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-24 11:25:18.000000 adbutils-2.2.3/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-24 11:25:18.000000 adbutils-2.2.3/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-24 11:25:18.000000 adbutils-2.2.3/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.146402 adbutils-2.2.3/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.150401 adbutils-2.2.3/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-03-24 11:25:12.000000 adbutils-2.2.3/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-03-24 11:25:12.000000 adbutils-2.2.3/build_wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.150401 adbutils-2.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-24 11:25:12.000000 adbutils-2.2.3/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-24 11:25:12.000000 adbutils-2.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-24 11:25:18.150401 adbutils-2.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-24 11:25:12.000000 adbutils-2.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 11:25:18.150401 adbutils-2.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-24 11:25:12.000000 adbutils-2.2.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.760258 adbutils-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-07 12:30:54.000000 adbutils-2.3.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.752258 adbutils-2.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-07 12:30:54.000000 adbutils-2.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.752258 adbutils-2.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-07 12:30:54.000000 adbutils-2.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-07 12:30:54.000000 adbutils-2.3.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-07 12:30:54.000000 adbutils-2.3.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 12:31:00.000000 adbutils-2.3.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-07 12:31:00.000000 adbutils-2.3.0/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-07 12:30:54.000000 adbutils-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-07 12:31:00.760258 adbutils-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14687 2024-04-07 12:30:54.000000 adbutils-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12748 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14732 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13794 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-07 12:30:54.000000 adbutils-2.3.0/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 12:31:00.000000 adbutils-2.3.0/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.752258 adbutils-2.3.0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-04-07 12:30:54.000000 adbutils-2.3.0/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-04-07 12:30:54.000000 adbutils-2.3.0/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 12:30:54.000000 adbutils-2.3.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-07 12:30:54.000000 adbutils-2.3.0/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 12:30:54.000000 adbutils-2.3.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-07 12:30:54.000000 adbutils-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-07 12:31:00.760258 adbutils-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-07 12:30:54.000000 adbutils-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.756258 adbutils-2.3.0/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8160 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-07 12:30:54.000000 adbutils-2.3.0/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:31:00.760258 adbutils-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-07 12:30:54.000000 adbutils-2.3.0/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-07 12:30:54.000000 adbutils-2.3.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-07 12:30:54.000000 adbutils-2.3.0/tests/test_adb_server.py
```

### Comparing `adbutils-2.2.3/.github/workflows/publish-to-pypi.yml` & `adbutils-2.3.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/.travis.yml` & `adbutils-2.3.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/LICENSE` & `adbutils-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/PKG-INFO` & `adbutils-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.2.3
+Version: 2.3.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.2.3/README.md` & `adbutils-2.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # adbutils
 [![PyPI](https://img.shields.io/pypi/v/adbutils.svg?color=blue)](https://pypi.org/project/adbutils/#history)
+[![codecov](https://codecov.io/gh/openatx/adbutils/graph/badge.svg?token=OuGOMZUkmi)](https://codecov.io/gh/openatx/adbutils)
 
-Python adb library for adb service (Only support Python3.6+)
+Python adb library for adb service (Only support Python3.6+), Recommend 3.8+
 
 **Table of Contents**
 
 <!--ts-->
    * [adbutils](#adbutils)
    * [Install](#install)
    * [Usage](#usage)
@@ -222,15 +223,15 @@
 output = d.sync.read_bytes("/data/local/tmp/hi.txt")
 # Expect output: b"Hello world"
 
 # 拷贝到本地
 d.sync.pull("/data/local/tmp/hi.txt", "hi.txt")
 
 # 获取包的信息
-info = d.package_info("com.example.demo")
+info = d.app_info("com.example.demo")
 if info:
     print(info) 
 	# output example:
     # {
 	# "version_name": "1.2.3", "version_code": "12", "signature": "0xff132", 
     # "first_install_time": datetime-object, "last_update_time": datetime-object,
     # }
@@ -271,18 +272,21 @@
 d.window_size()
 # example output: (1080, 1920)
 
 d.rotation()
 # example output: 1
 # other possible valus: 0, 1, 2, 3
 
-d.package_info("com.github.uiautomator")
+d.app_info("com.github.uiautomator")
 # example output: {"version_name": "1.1.7", "version_code": "1007"}
 
 d.keyevent("HOME")
+d.volume_up()
+d.volume_down()
+d.volume_mute()
 
 d.send_keys("hello world$%^&*") # simulate: adb shell input text "hello%sworld\%\^\&\*"
 
 d.open_browser("https://www.baidu.com") # 打开百度
 # There still too many functions, please see source codes
 
 # check if screen is on
@@ -508,25 +512,34 @@
 open another terminal, type the following command then you will see the socket data
 
 ```bash
 $ export ANDROID_ADB_SERVER_PORT=5577
 $ adb devices
 ```
 
+## Changes from 1.x to 2.x
+
+### Remove
+- current_app removed, use app_current instead
+- package_info removed, use app_info instead
+
+### Add
+- add volume_up, volume_down, volume_mute
+
 ## Generate TOC
 ```bash
 gh-md-toc --insert README.md
 ```
 
 <https://github.com/ekalinin/github-markdown-toc>
 
 # Thanks
 - [swind pure-python-adb](https://github.com/Swind/pure-python-adb)
 - [openstf/adbkit](https://github.com/openstf/adbkit)
-- [ADB Source Code](https://github.com/aosp-mirror/platform_system_core/blob/master/adb)
+- [ADB Source Code](https://android.googlesource.com/platform/system/core/+/android-4.4_r1/adb/adb.c)
 - ADB Protocols [OVERVIEW.TXT](https://cs.android.com/android/platform/superproject/+/master:packages/modules/adb/OVERVIEW.TXT) [SERVICES.TXT](https://cs.android.com/android/platform/superproject/+/master:packages/modules/adb/SERVICES.TXT) [SYNC.TXT](https://cs.android.com/android/platform/superproject/+/master:packages/modules/adb/SYNC.TXT)
 - [Awesome ADB](https://github.com/mzlogin/awesome-adb)
 - [JakeWharton/pidcat](https://github.com/JakeWharton/pidcat)
 
 # Alternative
 - https://github.com/Swind/pure-python-adb
```

### Comparing `adbutils-2.2.3/adbutils/__init__.py` & `adbutils-2.3.0/adbutils/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,17 +72,17 @@
         if transport_id:
             return AdbDevice(self, transport_id=transport_id)
 
         serial = os.environ.get("ANDROID_SERIAL")
         if not serial:
             ds = self.device_list()
             if len(ds) == 0:
-                raise RuntimeError("Can't find any android device/emulator")
+                raise AdbError("Can't find any android device/emulator")
             if len(ds) > 1:
-                raise RuntimeError(
+                raise AdbError(
                     "more than one device/emulator, please specify the serial number"
                 )
             return ds[0]
         return AdbDevice(self, serial)
```

### Comparing `adbutils-2.2.3/adbutils/__main__.py` & `adbutils-2.3.0/adbutils/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,18 +319,18 @@
             print(f"{remote_path} pulled to {target_path}")
 
     elif args.browser:
         d.open_browser(args.browser)
 
     elif args.current:
         package_name = d.app_current().package
-        info = d.package_info(package_name)
+        info = d.app_info(package_name)
         print(json.dumps(info, indent=4, default=str))
 
     elif args.package:
-        info = d.package_info(args.package)
+        info = d.app_info(args.package)
         print(json.dumps(info, indent=4, default=str))
 
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `adbutils-2.2.3/adbutils/_adb.py` & `adbutils-2.3.0/adbutils/_adb.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,60 +12,63 @@
 import typing
 import weakref
 from typing import Iterator, Union
 
 from deprecation import deprecated
 
 from adbutils._utils import adb_path
-from adbutils.errors import AdbError, AdbTimeout
+from adbutils.errors import AdbConnectionError, AdbError, AdbTimeout
 
 from adbutils._proto import *
-from adbutils._utils import list2cmdline
 from adbutils._version import __version__
 
 _OKAY = "OKAY"
 _FAIL = "FAIL"
 
 
 def _check_server(host: str, port: int) -> bool:
     """ Returns if server is running """
     s = socket.socket()
     try:
+        s.settimeout(.1)
         s.connect((host, port))
         return True
-    except socket.error as e:
+    except (socket.timeout, socket.error) as e:
         return False
     finally:
         s.close()
 
 
-
 class AdbConnection(object):
     def __init__(self, host: str, port: int):
         self.__host = host
         self.__port = port
         self.__conn = self._safe_connect()
 
         self._finalizer = weakref.finalize(self, self.conn.close)
 
     def _create_socket(self):
         adb_host = self.__host
         adb_port = self.__port
         s = socket.socket()
         try:
+            s.settimeout(.1) # prevent socket hang
             s.connect((adb_host, adb_port))
+            s.settimeout(None)
             return s
-        except:
-            s.close()
-            raise
+        except socket.timeout as e:
+            raise AdbTimeout("connect to adb server timeout")
+        except socket.error as e:
+            raise AdbConnectionError("connect to adb server failed: %s" % e)
+
 
     def _safe_connect(self):
         try:
             return self._create_socket()
-        except ConnectionRefusedError:
+        except AdbConnectionError:
             subprocess.run([adb_path(), "start-server"], timeout=20.0)  # 20s should enough for adb start
             return self._create_socket()
 
     @property
     def closed(self) -> bool:
         return not self._finalizer.alive
```

### Comparing `adbutils-2.2.3/adbutils/_proto.py` & `adbutils-2.3.0/adbutils/_proto.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # -*- coding: utf-8 -*-
 """Created on Fri May 06 2022 11:39:40 by codeskyblue
 """
 from __future__ import annotations
 
 __all__ = [
     "Network", "DeviceEvent", "ForwardItem", "ReverseItem", "FileInfo",
-    "WindowSize", "RunningAppInfo", "ShellReturn", "AdbDeviceInfo"
+    "WindowSize", "RunningAppInfo", "ShellReturn", "AdbDeviceInfo", "AppInfo"
 ]
 
 import enum
 import datetime
 import pathlib
 import typing
 from dataclasses import dataclass
```

### Comparing `adbutils-2.2.3/adbutils/_utils.py` & `adbutils-2.3.0/adbutils/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,18 +10,20 @@
 import threading
 import time
 import typing
 import zipfile
 import typing
 import pathlib
 
-import whichcraft
+from shutil import which
 from apkutils2.axml.axmlparser import AXML
 from apkutils2.manifest import Manifest
 
+from adbutils.errors import AdbError
+
 
 MB = 1024 * 1024
 
 
 def append_path(base: typing.Union[str, pathlib.Path], addition: str) -> str:
     if isinstance(base, pathlib.Path):
         return (base / addition).as_posix()
@@ -48,15 +50,15 @@
     except OSError:
         # bind 0 will fail on Manjaro, fallback to random port
         # https://github.com/openatx/adbutils/issues/85
         for _ in range(20):
             port = random.randint(10000, 20000)
             if not is_port_in_use(port):
                 return port
-        raise RuntimeError("No free port found")
+        raise AdbError("No free port found")
 
 
 def list2cmdline(args: typing.Union[list, tuple]):
     """ do not use subprocess.list2cmdline, use this instead
 
     Reason:
         subprocess.list2cmdline(['echo', '&']) --> "a &", but what I expect should be "a '&'"
@@ -89,25 +91,25 @@
 
 def adb_path():
     # 0. check env: ADBUTILS_ADB_PATH
     if os.getenv("ADBUTILS_ADB_PATH"):
         return os.getenv("ADBUTILS_ADB_PATH")
         
     # 1. find in $PATH
-    exe = whichcraft.which("adb")
+    exe = which("adb")
     if exe and _is_valid_exe(exe):
         return exe
     
     # 2. use buildin adb
     bin_dir = _get_bin_dir()
     exe = os.path.join(bin_dir, "adb.exe" if os.name == 'nt' else 'adb')
     if os.path.isfile(exe) and _is_valid_exe(exe):
         return exe
 
-    raise RuntimeError("No adb exe could be found. Install adb on your system")
+    raise AdbError("No adb exe could be found. Install adb on your system")
 
 
 def _popen_kwargs(prevent_sigint=False):
     startupinfo = None
     preexec_fn = None
     creationflags = 0
     if sys.platform.startswith("win"):
@@ -247,8 +249,54 @@
     
     def is_done(self) -> bool:
         """ check if background worker has stopped """
         return self.__done.is_set()
     
     def reset(self):
         self.__stop.clear()
-        self.__done.clear()
+        self.__done.clear()
+
+
+def escape_special_characters(text: str) -> str:
+    """
+    A helper that escape special characters
+
+    Args:
+        text: str
+    """
+    escaped = text.translate(
+        str.maketrans({
+            "-": r"\-",
+            "+": r"\+",
+            "[": r"\[",
+            "]": r"\]",
+            "(": r"\(",
+            ")": r"\)",
+            "{": r"\{",
+            "}": r"\}",
+            "\\": r"\\\\",
+            "^": r"\^",
+            "$": r"\$",
+            "*": r"\*",
+            ".": r"\.",
+            ",": r"\,",
+            ":": r"\:",
+            "~": r"\~",
+            ";": r"\;",
+            ">": r"\>",
+            "<": r"\<",
+            "%": r"\%",
+            "#": r"\#",
+            "\'": r"\\'",
+            "\"": r'\\"',
+            "`": r"\`",
+            "!": r"\!",
+            "?": r"\?",
+            "|": r"\|",
+            "=": r"\=",
+            "@": r"\@",
+            "/": r"\/",
+            "_": r"\_",
+            " ": r"%s",  # special
+            "&": r"\&"
+        }))
+    return escaped
```

### Comparing `adbutils-2.2.3/adbutils/errors.py` & `adbutils-2.3.0/adbutils/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     """ adb error """
 
 
 class AdbTimeout(AdbError):
     """ timeout when communicate to adb-server """
 
 
+class AdbConnectionError(AdbError):
+    """ connection error """
+
+
 class AdbInstallError(AdbError):
     def __init__(self, output: str):
         """
         Errors examples:
         Failure [INSTALL_FAILED_ALREADY_EXISTS: Attempt to re-install io.appium.android.apis without first uninstalling.]
         Error: Failed to parse APK file: android.content.pm.PackageParser$PackageParserException: Failed to parse /data/local/tmp/tmp-29649242.apk
```

### Comparing `adbutils-2.2.3/adbutils/pidcat.py` & `adbutils-2.3.0/adbutils/pidcat.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # Originally written by Jeff Sharkey, http://jsharkey.org/
 # Piping detection and popen() added by other Android team members
 # Package filtering and output improvements by Jake Wharton, http://jakewharton.com
 
 import argparse
 import sys
 import re
-import subprocess
 from subprocess import PIPE
 
 import adbutils
 
 __version__ = '2.1.0'
 
 # yapf: disable
```

### Comparing `adbutils-2.2.3/adbutils.egg-info/PKG-INFO` & `adbutils-2.3.0/adbutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.2.3
+Version: 2.3.0
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.2.3/adbutils.egg-info/SOURCES.txt` & `adbutils-2.3.0/adbutils.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,51 @@
+.coveragerc
 .travis.yml
 AUTHORS
 ChangeLog
 LICENSE
 README.md
 build_wheel.py
+codecov.yml
+pytest.ini
 requirements.txt
 setup.cfg
 setup.py
 .github/dependabot.yml
+.github/workflows/main.yml
 .github/workflows/publish-to-pypi.yml
 adbutils/__init__.py
 adbutils/__main__.py
 adbutils/_adb.py
 adbutils/_device.py
 adbutils/_proto.py
 adbutils/_utils.py
 adbutils/_version.py
 adbutils/errors.py
+adbutils/install.py
 adbutils/pidcat.py
+adbutils/screenrecord.py
+adbutils/screenshot.py
+adbutils/shell.py
+adbutils/sync.py
 adbutils.egg-info/PKG-INFO
 adbutils.egg-info/SOURCES.txt
 adbutils.egg-info/dependency_links.txt
 adbutils.egg-info/not-zip-safe
 adbutils.egg-info/pbr.json
 adbutils.egg-info/requires.txt
 adbutils.egg-info/top_level.txt
 adbutils/binaries/README.md
 adbutils/binaries/__init__.py
 assets/images/pidcat.png
 examples/reset-offline.py
+test_real_device/conftest.py
+test_real_device/test_adb.py
+test_real_device/test_deprecated.py
+test_real_device/test_device.py
+test_real_device/test_forward_reverse.py
+test_real_device/test_import.py
+test_real_device/test_record.py
+test_real_device/test_utils.py
+tests/adb_server.py
 tests/conftest.py
-tests/test_adb.py
-tests/test_deprecated.py
-tests/test_device.py
-tests/test_forward_reverse.py
-tests/test_import.py
-tests/test_record.py
-tests/test_utils.py
+tests/test_adb_server.py
```

### Comparing `adbutils-2.2.3/assets/images/pidcat.png` & `adbutils-2.3.0/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/build_wheel.py` & `adbutils-2.3.0/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/examples/reset-offline.py` & `adbutils-2.3.0/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/setup.cfg` & `adbutils-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/tests/conftest.py` & `adbutils-2.3.0/test_real_device/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/tests/test_adb.py` & `adbutils-2.3.0/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/tests/test_device.py` & `adbutils-2.3.0/test_real_device/test_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     # adb connect device devpath is "unknown"
     # assert device.get_devpath().startswith("usb:")
 
 
 def test_keyevent(device: AdbDevice):
     # make sure no error raised
     device.keyevent(4)
+    device.volume_up()
+    device.volume_down()
+    device.volume_mute()
 
 
 def test_switch_screen(device: AdbDevice):
     device.switch_screen(False)
     device.switch_screen(True)
 
 
@@ -157,23 +160,14 @@
         data += chunk
     assert b"Hello Android" == data
 
 
 def test_screenshot(device: AdbDevice):
     im = device.screenshot()
     assert im.mode == "RGB"
-
-
-@pytest.mark.skip("huawei is not supported")
-def test_screenrecord(device: AdbDevice, tmp_path: pathlib.Path):
-    r = device.screenrecord()
-    time.sleep(5)
-    target_path = tmp_path.joinpath("video.mp4")
-    r.stop_and_pull(target_path)
-    assert target_path.exists()
     
 
 def test_app_info(device: AdbDevice):
     pinfo = device.app_current()
     app_info = device.app_info(pinfo.package)
     assert app_info.package_name is not None
```

### Comparing `adbutils-2.2.3/tests/test_forward_reverse.py` & `adbutils-2.3.0/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.2.3/tests/test_utils.py` & `adbutils-2.3.0/test_real_device/test_utils.py`

 * *Files identical despite different names*

