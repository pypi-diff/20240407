# Comparing `tmp/f5_sphinx_theme-2.5.0.tar.gz` & `tmp/f5_sphinx_theme-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/f5-sphinx-theme/f5-sphinx-theme/dist/.tmp-al4jn3k3/f5_sphinx_theme-2.5.0.tar", last modified: Thu Apr  4 22:26:23 2024, max compression
+gzip compressed data, was "/home/runner/work/f5-sphinx-theme/f5-sphinx-theme/dist/.tmp-i5vj4as7/f5_sphinx_theme-2.5.2.tar", last modified: Sun Apr  7 06:37:00 2024, max compression
```

## Comparing `f5_sphinx_theme-2.5.0.tar` & `f5_sphinx_theme-2.5.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/breadcrumb.html
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/extralinks.html
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/globaltoc.html
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/head.html
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/localtoc.html
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/
--rwxr-xr-x   0 runner    (1001) docker     (127)   453169 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/CoveoFullSearch.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    25897 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap-theme.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    24167 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap-theme.min.css
--rwxr-xr-x   0 runner    (1001) docker     (127)   108100 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap.css
--rwxr-xr-x   0 runner    (1001) docker     (127)    89501 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)    19559 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/f5-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)   121080 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/f5.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaBold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaBold.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    25620 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaThin.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaThin.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/
--rwxr-xr-x   0 runner    (1001) docker     (127)   548426 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    56583 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/bootstrap.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    58072 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/bootstrap.min.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    12128 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/clouddocs.js
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/feedback.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     2417 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/jquery.appear.js
--rwxr-xr-x   0 runner    (1001) docker     (127)    13945 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/printThis.js
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme/theme.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 22:26:07.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-04 22:26:23.000000 f5_sphinx_theme-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-04 22:26:02.000000 f5_sphinx_theme-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/breadcrumb.html
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/extralinks.html
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/globaltoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/head.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/localtoc.html
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   453169 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/CoveoFullSearch.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25897 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap-theme.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24167 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap-theme.min.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)   108100 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap.css
+-rwxr-xr-x   0 runner    (1001) docker     (127)    89501 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    20941 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/f5-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)   122826 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/f5.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    25336 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaBold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19040 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaBold.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25452 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19068 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25620 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaThin.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaThin.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   548426 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    56583 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/bootstrap.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    58072 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/bootstrap.min.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12128 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/clouddocs.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/feedback.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2417 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/jquery.appear.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13945 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/printThis.js
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme/theme.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:36:40.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-07 06:37:00.000000 f5_sphinx_theme-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-07 06:36:34.000000 f5_sphinx_theme-2.5.2/setup.py
```

### Comparing `f5_sphinx_theme-2.5.0/LICENSE` & `f5_sphinx_theme-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/PKG-INFO` & `f5_sphinx_theme-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5_sphinx_theme
-Version: 2.5.0
+Version: 2.5.2
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `f5_sphinx_theme-2.5.0/README.rst` & `f5_sphinx_theme-2.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/__init__.py` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from os import path
 
 
-__version__ = "2.5.0"
+__version__ = "2.5.2"
 
 
 def get_html_theme_path():
     """Return the html theme path for this template library.
 
     :returns: List of directories to find template files in
     """
```

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/globaltoc.html` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/globaltoc.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/head.html` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/head.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/layout.html` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/localtoc.html` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/localtoc.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/searchbox.html` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/CoveoFullSearch.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/CoveoFullSearch.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap-theme.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap-theme.min.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/bootstrap.min.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/custom.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/custom.css`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/f5-theme.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/f5-theme.css`

 * *Files 5% similar despite different names*

```diff
@@ -31,28 +31,29 @@
 a.copybtn {
   width: 28px;
   height: 28px;
   padding: 8px;
 }
 
 #clouddocs-header {
-  position: fixed;
+  position: static;
+  /* Below is the original, but Eric Lafleur changed this because of Bug 19098 */
+  /* position: fixed;  */
   width: 100%;
   background-color: white;
   z-index: 20;
 }
 
 #clouddocs-footer {
   position: relative;
   max-height: 20vh
 }
 
 #content {
   padding: 20px;
-  padding-top: 152px;
   transition: all 0.3s;
 }
 
 #content.active {
   margin-left: 6px;
 }
 
@@ -204,15 +205,15 @@
   float: left;
   /* margin-top: 22px; */
   margin-left: 12px;
   overflow-x: auto;
   overflow-y: scroll;
   padding: 24px 12px 16px 16px;
   font-size: 14px;
-  margin-top: 10px;
+  margin-top: 15px;
 }
 
 #sidebar.active {
   margin-left: -35%;
 }
 
 :target:before {
@@ -1135,14 +1136,18 @@
 }
 
 .pageHeader {
   height: 80px;
   border-bottom: 14px solid #0186be;
 }
 
+.pageHeader .stat:first-of-type {
+  height: 50px;
+}
+
 @media (max-width: 768px) {
 
   .row.pageHeader,
   .pageHeader,
   #MainMenu {
     display: none;
   }
@@ -1303,7 +1308,63 @@
 }
 
 .version_list dd a {
   padding: 0;
   padding-right: 8px;
   color: black;
 }
+
+/*********************************************************
+This section here is the css styling for the dropdown menu
+**********************************************************/
+
+/* Dropdown Button */
+.dropbtn {
+  background-color: #0186BE;
+  color: white;
+  padding-left: 12px;
+  padding-right: 12px;
+  padding-top: 6px;
+  padding-bottom: 6px;
+  font-size: 16px;
+  border: none;
+  margin-bottom: 12px;
+}
+
+/* The container <div> - needed to position the dropdown content */
+.dropdown {
+  position: relative;
+  display: inline-block;
+}
+
+/* Dropdown Content (Hidden by Default) */
+.dropdown-content {
+  display: none;
+  position: absolute;
+  background-color: #f1f1f1;
+  min-width: 160px;
+  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
+  z-index: 1;
+}
+
+/* Links inside the dropdown */
+.dropdown-content a {
+  color: black;
+  padding: 12px 16px;
+  text-decoration: none;
+  display: block;
+}
+
+/* Change color of dropdown links on hover */
+.dropdown-content a:hover {
+  background-color: #ddd;
+}
+
+/* Show the dropdown menu on hover */
+.dropdown:hover .dropdown-content {
+  display: block;
+}
+
+/* Change the background color of the dropdown button when the dropdown content is shown */
+.dropdown:hover .dropbtn {
+  background-color: #002e63;
+}
```

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/css/f5.css` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/css/f5.css`

 * *Files 6% similar despite different names*

```diff
@@ -1,180 +1,201 @@
 /* Start of grid layout for CONTAINER AND CLOUD SOLUTIONS page  */
 
-.panel-body > .list-group {
+.panel-body>.list-group {
   display: flex;
   flex-wrap: wrap;
   justify-content: center;
 }
 
 
-.panel-body > .list-group .btn {
+.panel-body>.list-group .btn {
   white-space: normal;
 }
 
-.panel-body > .list-group .list-group-item:nth-child(4n+1) {
+.panel-body>.list-group .list-group-item:nth-child(4n+1) {
   margin-left: 0;
 }
 
-.panel-body > .list-group .list-group-item {
+.panel-body>.list-group .list-group-item {
   margin-top: 10px;
   width: calc(25% - 20px);
   margin-left: 20px;
   overflow: hidden;
   background-color: #f7f7f7;
   border: none;
   text-align: center;
   padding: 25px;
 }
 
-.panel-body > .list-group-item *:last-child{
+.panel-body>.list-group-item *:last-child {
   margin-bottom: 0;
 }
 
-.panel-body > .list-group-item *:first-child  {
+.panel-body>.list-group-item *:first-child {
   margin-top: 0;
 }
 
-.panel-body > .list-group .list-group-item p {
+.panel-body>.list-group .list-group-item p {
   margin-top: 12px;
   font-size: 14px;
 }
 
-.panel-heading > .panel-title {
+.panel-heading>.panel-title {
   text-align: center;
 }
 
 /* Responsive for smaller screens */
 
 @media all and (max-width: 1024px) {
-  .panel-body > .list-group .list-group-item {
+  .panel-body>.list-group .list-group-item {
     width: calc(33% - 20px);
   }
 }
 
 @media all and (max-width: 839px) {
-  .panel-body > .list-group .list-group-item {
+  .panel-body>.list-group .list-group-item {
     width: calc(50% - 20px);
   }
 }
 
 @media all and (max-width: 480px) {
-  .panel-body > .list-group .list-group-item {
+  .panel-body>.list-group .list-group-item {
     width: calc(100% - 20px);
   }
 }
 
 /* End of grid layout for CONTAINER AND CLOUD SOLUTIONS page */
 
 body.newstyles {
   margin: 0;
   padding: 0;
   overflow: auto;
 }
+
 .left {
   float: left;
 }
+
 .right {
   float: right;
 }
+
 .bold {
   font-weight: bold;
 }
+
 .spaced {
   margin: 0 4px;
 }
+
 .centred {
   margin: 0 auto;
   display: table !important;
 }
+
 .remove {
   background-color: #4F8D97;
   color: white;
 }
+
 @font-face {
   font-family: 'Colaborate';
   src: url('https://cdn.f5.com/websites/support/assets/fonts/ColabThi-webfont.eot');
   src: url('https://cdn.f5.com/websites/support/assets/fonts/ColabThi-webfont.eot?iefix') format('eot'), url('https://cdn.f5.com/websites/support/assets/fonts/ColabThi-webfont.woff') format('woff'), url('https://cdn.f5.com/websites/support/assets/fonts/ColabThi-webfont.ttf') format('truetype'), url('https://cdn.f5.com/websites/support/assets/fonts/ColabThi-webfont.svg#webfont') format('svg');
 }
+
 @font-face {
   font-family: "TabletGothic";
   src: url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothic.eot?f5v=2');
   src: url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothic.eot?f5v=2#iefix') format('embedded-opentype'), url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothic.woff?f5v=2') format('woff'), url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothic.ttf?f5v=2') format('truetype'), url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothic.svg?f5v=2#TabletGothic') format('svg');
   font-weight: normal;
   font-style: normal;
 }
+
 @font-face {
   font-family: "TabletGothicSemiBold";
   src: url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothicSemiBold.eot?f5v=2');
   src: url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothicSemiBold.eot?f5v=2#iefix') format('embedded-opentype'), url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothicSemiBold.woff?f5v=2') format('woff'), url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothicSemiBold.ttf?f5v=2') format('truetype'), url('https://cdn.f5.com/websites/support/assets/fonts/TabletGothicSemiBold.svg?f5v=2#TabletGothicSemiBold') format('svg');
   font-weight: normal;
   font-style: normal;
 }
+
 @font-face {
   font-family: "f5";
   src: url('https://cdn.f5.com/websites/support/assets/fonts/f5.eot?f5v=2');
   src: url('https://cdn.f5.com/websites/support/assets/fonts/f5.eot?f5v=2#iefix') format('embedded-opentype'), url('https://cdn.f5.com/websites/support/assets/fonts/f5.svg?f5v=2#f5') format('svg'), url('https://cdn.f5.com/websites/support/assets/fonts/f5.woff?f5v=2') format('woff');
   font-weight: normal;
   font-style: normal;
 }
+
 h1,
 h2,
 h3 {
-  font-family: Proxima,-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
+  font-family: Proxima, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
   font-weight: normal !important;
   color: #333;
 }
+
 h4 {
   font-weight: normal !important;
   color: #000;
 }
+
 h1 {
   font-size: 25px;
 }
+
 h2 {
   font-size: 22px;
   line-height: 26px;
   margin-bottom: 20px;
   width: 100%;
 }
+
 h3 {
   font-size: 20px;
 }
+
 h4 {
   font-size: 22px;
   margin: 18px 0 10px 0;
   width: 100%;
 }
+
 h5,
 .h5 {
   font-size: 16px;
   font-weight: bold;
 }
+
 h6,
 .h6 {
   font-size: 15px;
   font-style: italic;
   font-weight: bold;
 }
+
 a:hover {
   cursor: pointer;
 }
+
 h5.knownissue,
 h5.manual,
 h5.howto,
 h5.policy,
 h5.security,
 h5.diagnostic,
 h5.non-diagnostic {
   background-size: 45px 45px !important;
   padding: 16px 0 14px 55px;
   font-size: 18px;
   float: left;
   width: 100%;
 }
+
 .content-cont.diagnostic,
 .content-cont.howto,
 .content-cont.knownissue,
 .content-cont.manual,
 .content-cont.non-diagnostic,
 .content-cont.policy,
 .content-cont.releasenote,
@@ -182,92 +203,114 @@
 .content-cont.security {
   background-size: 30px 30px !important;
   padding: 0 0 0 30px;
   font-size: 14px;
   float: left;
   width: 100%;
 }
+
 i.knownissue,
 i.manual,
 i.howto,
 i.policy,
 i.diagnostic,
 i.non-diagnostic,
 i.security {
   background-size: 45px 45px !important;
   width: 45px;
   height: 45px;
   display: block;
   margin: auto;
 }
+
 i.knownissue {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-knownissue.svg') no-repeat center left;
 }
+
 i.security {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-security.svg') no-repeat center left;
 }
+
 i.policy {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-policy.svg') no-repeat center left;
 }
+
 i.manual {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-manual.svg') no-repeat center left;
 }
+
 i.howto {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-howto.svg') no-repeat center left;
 }
+
 h5.knownissue {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-knownissue.svg') no-repeat center left;
 }
+
 h5.security {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-security.svg') no-repeat center left;
 }
+
 h5.policy {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-policy.svg') no-repeat center left;
 }
+
 h5.non-diagnostic {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-releasenote.svg') no-repeat center left;
 }
+
 h5.manual {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-manual.svg') no-repeat center left;
 }
+
 h5.howto {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-howto.svg') no-repeat center left;
 }
+
 .content-cont.knownissue {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-knownissue-bw.svg') no-repeat top left;
 }
+
 .content-cont.security {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-security-bw.svg') no-repeat top left;
 }
+
 .content-cont.policy {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-policy-bw.svg') no-repeat top left;
 }
+
 .content-cont.manual {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-manual-bw.svg') no-repeat top left;
 }
+
 .content-cont.howto {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-howto-bw.svg') no-repeat top left;
 }
+
 .content-cont.diagnostic,
 .content-cont.non-diagnostic,
 .content-cont.releasenote,
 .content-cont.supplementaldocuments {
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/icon-releasenote-bw.svg') no-repeat top left;
 }
+
 .icon-inverse-circle:before {
   width: 1.65em;
   height: 1.65em;
 }
+
 .icon-inverse-circle:before {
   background: #7c7d7d;
   color: #FFF;
 }
+
 a:hover .icon-inverse-circle:before {
   background: #4d4f53;
 }
+
 .ext-rounded-icon:before,
 .icon-inverse-circle:before,
 .icon-white-round:before,
 .icon-round:before,
 .article .social i:before {
   border-width: .1em;
   border-color: transparent;
@@ -276,133 +319,171 @@
   text-align: center;
   display: table-cell;
   vertical-align: middle;
   -webkit-transition: all 0.4s ease;
   transition: all 0.4s ease;
   font-family: 'f5';
 }
+
 .icon-inverse-circle {
   height: 1.65em;
   width: 1.65em;
   color: #fff;
 }
+
 .icon-twitter:before {
   content: "\f099";
 }
+
 .icon-linkedin:before {
   content: "\e00f";
 }
+
 .icon-facebook:before {
   content: "\f09a";
 }
+
 .icon-youtube:before {
   content: "\f167";
 }
+
 .icon-dc-pos:before {
   content: "\e60e";
 }
+
 .icon-cloud:before {
   content: "\e612";
 }
+
 .icon-servers:before {
   content: "\e622";
 }
+
 .icon-computer-on:before {
   content: "\e624";
 }
+
 .icon-print:before {
   content: "\e600";
 }
+
 .icon-share:before {
   content: "\e005";
 }
+
 .icon-pdf:before {
   content: "\e609";
 }
+
 .icon-mail:before,
 .icon-envelope:before {
   content: "\f0e0";
 }
+
 .icon-star:before,
 .icon-favorite:before,
 .icon-star-empty:before {
   content: "\f006";
 }
+
 .icon-star-full:before,
 .icon-favorited:before {
   content: "\f005";
 }
+
 .icon-plus:before {
   content: "\f116";
 }
+
 .icon-minus:before {
   content: "\f117";
 }
+
 .icon-refresh:before {
   content: "\e60d";
 }
+
 .icon-clear:before,
 .icon-clear-left:before {
   content: "\e60b";
 }
+
 .icon-down:before {
   content: "\f107";
 }
+
 .icon-up:before {
   content: "\f106";
 }
+
 .icon-download:before {
   content: "\f0ed";
 }
+
 .icon-f5:before {
   content: "\e008";
 }
+
 .icon-graduate:before {
   content: "\e615";
 }
+
 .icon-edit:before,
 .icon-pencil:before {
   content: "\e603";
 }
+
 .icon-bin:before {
   content: "\e24f";
 }
+
 .icon-new-window:before {
   content: "\f08e";
 }
+
 .icon-people:before {
   content: "\f0c0";
 }
+
 .icon-question:before {
   content: "\f128";
 }
+
 .icon-speedometer:before {
   content: "\e619";
 }
+
 .icon-unlocked:before {
   content: "\f13e";
 }
+
 .icon-locked:before {
   content: "\f023";
 }
+
 .icon-doc:before {
   content: "\e608";
 }
+
 .icon-file:before {
   content: "\e00b";
 }
+
 .icon-pdf:before {
   content: "\e609";
 }
+
 .icon-image:before {
   content: "\e00c";
 }
+
 .icon-phone:before {
   content: "\f095";
 }
+
 [class^="icon-"],
 [class*=" icon-"],
 a.more:after,
 .ext-icon,
 [class*="bullet-"] li:before,
 #sb-nav a {
   speak: none;
@@ -413,62 +494,75 @@
   font-variant: normal;
   font-size: inherit;
   line-height: 1;
   text-rendering: auto;
   -webkit-font-smoothing: antialiased;
   -moz-osx-font-smoothing: grayscale;
 }
+
 .icon-1x {
   font-size: 1.1em !important;
   margin: 0 2px 0 0;
   float: left;
   padding: 0;
   line-height: 18px;
 }
+
 .icon-1x-right {
   font-size: 1.1em !important;
   margin: 0 2px 0 0;
   padding: 0;
   line-height: 18px;
 }
+
 .icon-1-5x {
   font-size: 1.5em !important;
 }
+
 .icon-2x {
   font-size: 2em !important;
 }
+
 .icon-3x {
   font-size: 3em !important;
 }
+
 .icon-5x {
   font-size: 5em !important;
 }
+
 .intitle {
   margin: 0 10px 0 0;
   background-color: #fff;
   padding: 6px;
   border-radius: 50px;
   border: 1px solid #dddddd;
 }
+
 .share {
   margin: 1px 0 0 5px;
 }
+
 .glyphicon {
   top: 2px;
   margin-right: 5px;
 }
+
 .glyphicon.spacer {
   margin-right: 5px;
 }
+
 .glyphicon.no-space {
   margin-right: 0;
 }
+
 ul.filters {
   margin: 10px -6px 0 0;
 }
+
 ul.filters li {
   font-size: 11px;
   line-height: 1;
   list-style: none;
   float: left;
   margin: 0 6px 6px 0;
   padding: 2px 6px 4px 6px;
@@ -478,284 +572,383 @@
   color: #777777;
   border: 1px solid #ccc;
   background: rgba(0, 0, 0, 0.08);
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
 }
+
 ul.filters li:hover {
   text-decoration: none;
   color: #555;
   border-color: #bbb;
   background-color: rgba(0, 0, 0, 0.1);
   cursor: pointer;
 }
+
 ul.filters li .glyphicon {
   margin-left: 2px;
   margin-right: 0px;
   font-size: 13px;
   top: 2px;
   color: #9D9D9D;
 }
+
 ul.filters li:hover .glyphicon {
   color: #000;
 }
+
 .use-filters {
   float: left;
   font-size: 12px;
   margin: 4px 4px 0 0;
 }
+
 .alert-pagination .pagination {
   float: right;
 }
+
 .panel.alert-panel {
   margin-bottom: 0px;
 }
+
 .content {
   width: 100%;
   float: left;
 }
+
 .title-bg h3 {
   background: #F5F5F5;
   padding: 4px 4px 7px 8px;
   margin: 20px 20px 0 0;
 }
+
 .nobanner .row.support-header {
   display: none;
 }
+
 .nobanner.guided-search .search {
   margin: 14px auto 24px auto;
 }
+
 .nobanner .pageHeader {
   border-bottom: 14px solid #2270B3;
 }
+
 /*  ------------- My Support button ------------- */
 a.mysupport {
   background-color: #e6e6e6;
   color: #003c78;
   text-decoration: none;
   padding: 5px 26px;
   line-height: 22px;
   font-size: 14px;
   font-weight: bold;
   border-radius: 4px;
   margin: 12px 0px 0 0;
   float: right;
 }
+
 a.mysupport:hover {
   background-color: rgba(230, 230, 230, 0.96);
 }
+
 .support-menu ul {
   float: right;
   width: auto;
 }
+
 .support-menu ul li {
   float: left;
   display: inline;
   margin: 10px 8px 0px 8px;
 }
+
 .support-menu ul li a {
   padding: 6px 0 6px 22px;
   color: #000;
   font-weight: bold;
   opacity: 0.6;
   transition: opacity 1s ease-in-out;
   -moz-transition: opacity 1s ease-in-out;
   -webkit-transition: opacity 1s ease-in-out;
 }
+
 .support-menu ul li a:hover {
   padding: 6px 0 6px 22px;
   opacity: 1;
 }
+
 .support-menu ul li a.current {
   color: #000;
   opacity: 1;
   cursor: default;
 }
+
 .csp-bread-crumbs ul {
   float: left;
   width: 100%;
   margin: 10px 0 0 0 !important;
   padding: 0;
 }
+
 .csp-bread-crumbs ul li {
   display: inline;
   font-size: 85%;
 }
+
 .csp-bread-crumbs ul li:before {
   content: "/ ";
   padding-right: 4px;
 }
+
 .csp-bread-crumbs ul li:first-child:before {
   content: "";
 }
+
 .csp-bread-crumbs ul li a:hover {
   cursor: pointer !important;
 }
+
 .footer {
-  background: #4c4e52;
+  background: black;
   color: #fff;
   margin-top: 80px;
   position: sticky;
 }
+
+.contact-container {
+  display: flex;
+  justify-content: center;
+  text-align: center;
+}
+
+.contact-header {
+  margin: 6px 0 0 0 !important;
+  width: revert;
+  font-size: 16px !important;
+  font-weight: bold !important;
+}
+
+.social-container {
+  display: flex;
+  justify-content: center;
+  text-align: center;
+}
+
+.social-link-header {
+  margin: 6px 0 0 0 !important;
+  width: revert;
+  font-size: 16px !important;
+  font-weight: bold !important;
+}
+
+.social-links {
+  display: flex;
+  font-size: 0;
+  margin-top: 2px !important;
+  margin-bottom: 0 !important;
+  padding-left: 0 !important;
+  width: 300px;
+}
+
+.spacer {
+  margin: 3px 25px 0 25px;
+}
+
+.links {
+  padding-left: 40px;
+}
+
 .footer p,
 footer p a {
-  font-size: 11px;
-  color: #ABA9A9;
+  font-size: 14px;
+  /* color: #ABA9A9; */
   font-family: Arial, Helvetica, sans-serif;
   letter-spacing: 1px;
   font-weight: normal;
-  margin: 10px 0 30px 0;
+  /* margin: 10px 0 30px 0; */
 }
+
 .footer h4 {
-  font-size: 18px;
+  font-size: 16px;
+  font-weight: bold !important;
   margin: 34px 0 10px 0;
   color: white;
   text-transform: uppercase;
 }
+
 .footer a,
 .footer a:visited {
   color: #ffffff;
   line-height: 26px;
 }
+
 .footer a:hover,
 .footer a:active {
   color: #e6e6e6;
   text-decoration: none;
 }
+
 .footer ul {
   padding: 0;
   margin: 0 0 20px 2px;
 }
+
 .footer ul li {
   list-style: none;
 }
+
 .footer .social_icons li {
   display: inline-block !important;
   margin-left: 5px;
 }
+
 .footer .social_icons li:first-child {
   margin-left: 0;
 }
+
 .footer .icon-inverse-circle,
 .footer .article .social i {
   font-size: 19px;
   font-style: normal;
 }
+
 .footer .icon-inverse-circle:before,
 .footer .article .social i:before {
   background-color: #aeb0b0;
 }
+
 .footer .icon-inverse-circle:hover:before,
 .footer .article .social i:hover:before {
   background-color: #7c7d7d;
 }
+
 .footer .revision {
   color: #4c4e4e;
 }
-#MainMenu .submenu > li:not(.divider) {
+
+#MainMenu .submenu>li:not(.divider) {
   padding: 15px;
   background: #efefef;
 }
-#MainMenu > li {
+
+#MainMenu>li {
   height: 40px;
   padding-top: 10px;
 }
-#MainMenu > li:first-of-type {
+
+#MainMenu>li:first-of-type {
   border-left: 1px solid #ccc;
   padding-left: 10px;
 }
-#MainMenu > li:hover::after {
+
+#MainMenu>li:hover::after {
   content: " ";
   display: block;
   border-top: 3px solid #e21d38;
   height: 20px;
 }
+
 .main-menu {
   float: left;
   margin: 0 0 0 0;
   padding: 0;
   padding-top: 10px;
   margin-left: 10px;
 }
+
 .main-menu .message {
   padding: 15px;
   background: #FFF;
   min-height: 150px;
 }
+
 .main-menu .message img {
   min-width: 100%;
 }
+
 .main-menu .message figcaption {
   margin-top: 10px;
 }
+
 .main-menu .message figcaption a {
   padding-top: 10px !important;
   line-height: 20px;
   font-weight: normal;
   float: left;
 }
-.main-menu > li > ul {
+
+.main-menu>li>ul {
   width: 100%;
 }
-.main-menu > li > a {
+
+.main-menu>li>a {
   display: inline-block;
   position: relative;
 }
+
 .main-menu li {
   float: left;
   display: inline;
   list-style: none;
   margin: 0px 26px 0 4px;
   line-height: 21px;
   vertical-align: text-top;
   font-size: 18px;
 }
+
 .main-menu li a {
   color: #555;
   font-weight: 700;
   padding-top: 10px;
   text-decoration: none;
 }
+
 .main-menu li a:hover {
   color: #0075b8;
   text-decoration: none;
 }
+
 .main-menu li .menu-panel {
   display: none;
   position: absolute;
   z-index: 1000;
   left: 0;
   background: #e4e7eb;
   width: 100%;
   box-shadow: 0px 2px 5px 0px rgba(0, 0, 0, 0.25);
   padding: 30px 0;
   min-height: 244px;
 }
+
 .main-menu li .menu-panel li {
   font-size: 15px !important;
 }
+
 .main-menu li .indicator {
   text-align: center;
   position: absolute;
   width: 100%;
   bottom: -20px;
   left: 0;
   display: none;
 }
+
 .main-menu li .arrow-up {
   position: absolute;
   bottom: 0;
   left: 45%;
   width: 0;
   height: 0;
   border-left: 7px solid transparent;
   border-right: 7px solid transparent;
   border-bottom: 7px solid #fff;
 }
+
 .main-menu li:hover .menu-panel {
   display: block;
   visibility: visible;
   opacity: 1;
   height: auto;
   -webkit-animation: fadeIn 0.5s;
   animation: fadeIn 0.5s;
@@ -766,368 +959,438 @@
   border-top: 1px solid #e4e7eb;
   width: 100%;
   box-shadow: 0 2px 5px 0 rgba(0, 0, 0, 0.25);
   padding: 30px 0;
   min-height: 244px;
   margin: 20px 0 0 0;
 }
+
 .main-menu li:hover .indicator {
   display: block;
 }
+
 @-webkit-keyframes fadeIn {
   from {
     opacity: 0;
   }
+
   to {
     opacity: 1;
   }
 }
+
 @keyframes fadeIn {
   from {
     opacity: 0;
   }
+
   to {
     opacity: 1;
   }
 }
-.main-menu .submenu > li > a,
-.main-menu .submenu > li a.header {
+
+.main-menu .submenu>li>a,
+.main-menu .submenu>li a.header {
   text-transform: uppercase;
   font-size: 16px;
   margin: 4px 0 10px 0;
   float: left;
 }
-.main-menu .submenu > li {
+
+.main-menu .submenu>li {
   width: 22%;
   float: left;
 }
-.main-menu .submenu > li.divider {
-  margin: 0 10px;;
+
+.main-menu .submenu>li.divider {
+  margin: 0 10px;
+  ;
   padding: 0;
   border-left: #FFF solid 1px;
   width: 1px;
   min-height: 160px;
 }
+
 .main-menu .submenu .menu-footer a {
   font-weight: bold;
 }
+
 .main-menu .submenu .img-responsive {
   max-height: 100px !important;
 }
+
 .main-menu .submenu a {
   display: block;
   border: none;
   /*color: #4d4f53;*/
   color: #004A90;
   text-decoration: none;
   text-transform: none;
   line-height: 16px;
   padding-bottom: 4px;
   padding-top: 4px;
 }
+
 .main-menu .submenu a .current {
   font-weight: bold;
 }
+
 .main-menu .submenu a:hover {
   color: #004892;
 }
+
 .main-menu .submenu ul,
 .main-menu .submenu li {
   margin: 0;
   list-style: none;
   line-height: 20px;
   padding: 0 0 4px 0;
 }
+
 .main-menu .submenu li ul li a {
   font-weight: normal;
 }
+
 .main-menu .submenu li li {
   display: block;
   width: 100%;
 }
+
 .main-menu .submenu li:hover .menu-panel li {
   font-size: 15px !important;
 }
-.main-menu .submenu > li.forth {
+
+.main-menu .submenu>li.forth {
   width: 22%;
 }
-.main-menu .submenu > li.third {
+
+.main-menu .submenu>li.third {
   width: 30%;
 }
-.main-menu .submenu > li.half {
+
+.main-menu .submenu>li.half {
   width: 48%;
 }
-.main-menu .submenu > li.half li {
+
+.main-menu .submenu>li.half li {
   display: inline-block;
   width: 49%;
 }
+
 @media screen and (min-width: 992px) {
-  .main-menu .submenu > li.half.three-col li {
+  .main-menu .submenu>li.half.three-col li {
     width: 28%;
   }
 }
+
 @media (max-width: 767px) {
 
   .corp-header {
     height: 40px;
     background-color: #ebebeb;
     border-bottom: 14px solid #0186be;
   }
 
-    .pageHeader {
-      height: 80px;
-    }
+  .pageHeader {
+    height: 80px;
+  }
 
 }
 
 @media (min-width: 768px) {
 
   .corp-header {
     height: 40px;
     background-color: #ebebeb;
   }
 
-   .pageHeader {
-      height: 80px;
-      border-bottom: 14px solid #0186be;
-   }
+  .pageHeader {
+    height: 80px;
+    border-bottom: 14px solid #0186be;
+  }
 
 }
+
 .section {
   width: 100%;
 }
+
 .section.crumbs {
   height: 40px;
   background-color: #ebebeb;
   margin-bottom: 24px;
 }
+
 img.logo {
   margin: 8px 0 0 0;
   float: left;
   width: 45px;
   height: 42px;
   border: 0;
 }
+
 img.logo.support {
   padding: 2px 0 0 10px;
   margin: 12px 0 0 12px;
   width: 110px;
   height: 44px;
 }
+
 /* ---------- corporate menu ----------  */
 .corp-header {
   height: 40px;
   background-color: #ebebeb;
 }
+
 .corp-header .corp-menu li:before {
   content: "|";
   padding-right: 8px;
   color: #888;
   /* float: left; */
   line-height: 18px;
 }
+
 .corp-header .corp-menu li:first-child:before {
   content: "";
   /* float: left; */
   line-height: 18px;
 }
+
 .corp-header ul li a.current {
   color: #000;
   opacity: 1;
 }
+
 .corp-header ul li a {
   padding: 0;
   color: #000;
   opacity: 0.7;
   font-size: 12px;
   font-weight: 700;
   text-transform: uppercase;
   transition: opacity 1s ease-in-out;
   -moz-transition: opacity 1s ease-in-out;
   -webkit-transition: opacity 1s ease-in-out;
 }
+
 .corp-header ul {
   float: right;
   width: auto;
 }
+
 .corp-header ul li {
   float: left;
   display: inline;
   margin: 6px 6px 0 3px;
 }
+
 .corp-header ul li a:hover {
   opacity: 1;
 }
+
 .corp-header .corp-menu ul li a.current {
   color: #000;
   opacity: 1;
 }
+
 .topLinks {
   float: right;
   text-align: left;
   margin: -42px -10px 0 0;
   height: 40px;
 }
+
 .topLinks .log {
   margin: 8px 0 0 0;
   font-size: 13px;
   font-weight: normal;
   float: left;
   width: 100%;
 }
+
 .topLinks a {
   margin: 0 6px 0 6px;
   font-weight: bold;
 }
+
 .support-header {
   height: 78px;
   background: #00a2e2;
 }
+
 .support-header .submit-search {
   width: 55%;
 }
+
 .support-header .searchwrapper {
   margin: -36px 22.4% 0 0 !important;
   position: static;
   right: 10%;
 }
+
 /* -------------------
 navigation on mobile
 --------------------- */
 .mobile-nav-container {
   padding: 10px 0;
   margin: 0;
 }
+
 .mobile-nav-container a {
   color: #fff;
   text-decoration: none;
   float: left;
   line-height: 20px;
   width: 100%;
   border-bottom: 1px solid #ABABAB;
   background: none;
 }
+
 .mobile-nav-container .mobile-nav-header {
   font-size: 17px;
   font-family: 'TabletGothic', 'Colaborate', Arial, sans-serif;
   font-weight: 300;
 }
+
 .mobile-nav-container .mobile-nav-header a {
   padding: 10px 0 10px 10px;
 }
+
 .mobile-nav-container ul {
   list-style: none;
   margin: 0;
   padding: 0;
 }
+
 .mobile-nav-container ul li {
   padding: 0;
   font-size: 15px;
   font-family: Arial, Helvetica, sans-serif;
   font-weight: normal;
 }
+
 .mobile-nav-container ul li a {
   padding: 8px 0 8px 30px;
   background: #9ba0a5;
 }
+
 .mobile-nav-container ul li a:hover {
   text-decoration: none;
   background: rgba(176, 178, 184, 0.97);
 }
+
 .lines-button {
   padding: 0.7rem 0.7rem 1.2rem 0.7rem;
   transition: .3s;
   cursor: pointer;
   user-select: none;
   border-radius: 0.57143rem;
 }
+
 .lines-button.closed {
   padding: 1.1rem 1.4rem 1.8rem 1.4rem;
 }
+
 .lines-button:hover {
   opacity: 1;
 }
+
 .lines-button:hover .lines:before {
   top: 1.14286rem;
 }
+
 .lines-button:hover .lines:after {
   top: -1.14286rem;
 }
+
 .lines-button:active {
   transition: 0s;
 }
+
 .lines-button.closed {
   -webkit-transform: scale3d(0.8, 0.8, 0.8);
   transform: scale3d(0.8, 0.8, 0.8);
 }
+
 .lines-button .lines {
   display: inline-block;
   width: 4rem;
   height: 0.57143rem;
   background: #fff;
   border-radius: 0.28571rem;
   transition: 0.3s;
   position: relative;
 }
+
 .lines-button .lines:before,
 .lines-button .lines:after {
   display: inline-block;
   width: 4rem;
   height: 0.57143rem;
   background: #fff;
   border-radius: 0.28571rem;
   transition: 0.3s;
   position: absolute;
   left: 0;
   content: '';
   -webkit-transform-origin: 0.28571rem center;
   transform-origin: 0.28571rem center;
 }
+
 .lines-button .lines:before {
   top: 1rem;
 }
+
 .lines-button .lines:after {
   top: -1rem;
 }
+
 .lines-button.x.closed .lines {
   background: transparent;
 }
+
 .lines-button.x.closed .lines:before,
 .lines-button.x.closed .lines:after {
   -webkit-transform-origin: 50% 50%;
   transform-origin: 50% 50%;
   top: 0;
   width: 4rem;
 }
+
 .lines-button.x.closed .lines:before {
   -webkit-transform: rotate3d(0, 0, 1, 45deg);
   transform: rotate3d(0, 0, 1, 45deg);
 }
+
 .lines-button.x.closed .lines:after {
   -webkit-transform: rotate3d(0, 0, 1, -45deg);
   transform: rotate3d(0, 0, 1, -45deg);
 }
+
 .sidebar-toggle .button.closed {
   margin: -5px 0 0 0;
 }
+
 /*--- sidebar on mobile -- */
 .sidebar-toggle {
   position: absolute;
   top: 3px;
   left: 0;
   width: 50px;
   height: 50px;
   background: transparent;
 }
+
 .sidebar-toggle .button {
   display: inline-block;
   margin: 0 0.5em;
   border: none;
   background: #8D8F96;
 }
+
 /* .sidebar {
   position: absolute;
   top: 46px;
   left: 0;
   background: rgba(141, 143, 150, 0.97);
   width: 175px;
   color: #fff;
@@ -1137,89 +1400,104 @@
   border-top: 16px solid #0194D2;
 } */
 /* navigation */
 .seemore {
   float: left;
   width: 100%;
 }
+
 .container.stat,
 .stat,
 .col-xs-12.stat {
   position: static !important;
 }
+
 @media screen and (min-width: 992px) {
-  .main-menu .submenu > li.half.three-col li {
+  .main-menu .submenu>li.half.three-col li {
     width: 28%;
   }
 }
+
 .submenu {
   margin: 0 auto;
   display: table;
   float: none;
 }
+
 a.mn-h,
 span.a-mm-h {
   text-transform: uppercase;
   font-size: 16px;
   color: #000;
   display: block;
   line-height: 16px;
   padding-bottom: 4px;
-  margin: 4px 0 10px 0;
+  margin: 10px 0 5px 0;
   float: left;
 }
+
 #upc-search {
   color: white;
   background-color: #6a6c73;
   padding: 8px;
   border-radius: 30px;
   font-size: 20px;
   -webkit-transition: all .4s ease;
   transition: all .4s ease;
 }
+
 .field #upc-search {
   color: #6a6c73;
   background-color: transparent;
 }
+
 .field #upc-search:hover {
   color: #000;
   background-color: transparent;
 }
+
 #blue-banner.searchwrapper.field {
   margin: -36px -2px 0 0;
 }
+
 #upc-search:hover {
   color: white;
   background-color: #aeb0b0;
   cursor: pointer;
 }
+
 .searchwrapper {
   float: right;
   margin: -30px -10px 0 10px;
 }
+
 .searchwrapper.icon-width {
   width: 53px;
 }
 
 .search {
   /*margin: 40px auto 28px auto;*/
   margin: 20px auto;
   display: table;
   width: 66%;
 }
+
 .search .form-control {
   display: inline;
 }
+
 .search .btn {
   display: inline;
 }
+
 .search .btn-primary {
   padding: 8px 22px !important;
   border-radius: 0 4px 4px 0;
 }
+
 form.search input.support-guided {
   width: 77%;
   height: 38px;
   padding: 8px 34px 8px 12px;
   font-size: 14px;
   line-height: 18px;
   color: #555;
@@ -1231,36 +1509,42 @@
   box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
   -webkit-transition: border-color ease-in-out 0.15s, -webkit-box-shadow ease-in-out 0.15s;
   -o-transition: border-color ease-in-out 0.15s, box-shadow ease-in-out 0.15s;
   transition: border-color ease-in-out 0.15s, box-shadow ease-in-out 0.15s;
   font-weight: bold;
   float: left;
 }
+
 .search-actions {
   position: relative;
 }
+
 .submit-search {
   background-color: #fff;
   border-color: #E2E2E2;
   box-shadow: inherit;
   border-top-right-radius: 3px;
   border-bottom-right-radius: 3px;
   width: 90%;
   margin: 20px auto 0 auto;
   display: table;
 }
+
 .modal-header {
   padding: 15px 15px 30px 15px !important;
 }
+
 .modal h4 {
   margin: 20px 0 20px 15px;
 }
+
 h3 .glyphicon {
   color: #565759;
 }
+
 .ajaxloader1,
 .ajaxloader2,
 .ajaxloader3,
 .ajaxloader4 {
   display: block;
   position: absolute;
   width: 40px;
@@ -1275,125 +1559,148 @@
   -webkit-animation: spin 1s linear infinite;
   -moz-animation: spin 1s linear infinite;
   -ms-animation: spin 1s linear infinite;
   -o-animation: spin 1s linear infinite;
   animation: spin 1s linear infinite;
   z-index: 99;
 }
+
 .ajaxloader2 {
   border-right: 0 none;
 }
+
 .ajaxloader3 {
   border-left-color: transparent;
 }
+
 .ajaxloader4 {
   border-bottom-color: transparent;
 }
+
 .ajaxloader3::after,
 .ajaxloader4::after {
   display: block;
   content: " ";
   width: 4px;
   height: 4px;
   border: 4px solid #fff;
   margin: 8px;
   border-radius: 50%;
 }
+
 .ajaxloader3::after {
   border-left-color: transparent;
   border-right-color: transparent;
 }
+
 .ajaxloader4::after {
   width: 13px;
   height: 13px;
   margin: 1px;
   border-width: 8px;
   border-top-color: transparent;
   border-left-color: transparent;
 }
+
 @-webkit-keyframes spin {
   from {
     -webkit-transform: rotate(0deg);
     opacity: 0.4;
   }
+
   50% {
     -webkit-transform: rotate(180deg);
     opacity: 1;
   }
+
   to {
     -webkit-transform: rotate(360deg);
     opacity: 0.4;
   }
 }
+
 @-moz-keyframes spin {
   from {
     -moz-transform: rotate(0deg);
     opacity: 0.4;
   }
+
   50% {
     -moz-transform: rotate(180deg);
     opacity: 1;
   }
+
   to {
     -moz-transform: rotate(360deg);
     opacity: 0.4;
   }
 }
+
 @-ms-keyframes spin {
   from {
     -ms-transform: rotate(0deg);
     opacity: 0.4;
   }
+
   50% {
     -ms-transform: rotate(180deg);
     opacity: 1;
   }
+
   to {
     -ms-transform: rotate(360deg);
     opacity: 0.4;
   }
 }
+
 @-o-keyframes spin {
   from {
     -o-transform: rotate(0deg);
     opacity: 0.4;
   }
+
   50% {
     -o-transform: rotate(180deg);
     opacity: 1;
   }
+
   to {
     -o-transform: rotate(360deg);
     opacity: 0.4;
   }
 }
+
 @keyframes spin {
   from {
     transform: rotate(0deg);
     opacity: 0.2;
   }
+
   50% {
     transform: rotate(180deg);
     opacity: 1;
   }
+
   to {
     transform: rotate(360deg);
     opacity: 0.2;
   }
 }
+
 .loading {
   position: absolute;
   background: rgba(255, 255, 255, 0.7);
   width: 100%;
   height: 100%;
   min-height: 100%;
   z-index: 999;
   transition: all .4s ease;
   top: -35px;
 }
+
 .loading:before {
   content: " ";
   display: block;
   position: absolute;
   width: 40px;
   height: 40px;
   left: 50%;
@@ -1406,339 +1713,404 @@
   -webkit-animation: spin 1s linear infinite;
   -moz-animation: spin 1s linear infinite;
   -ms-animation: spin 1s linear infinite;
   -o-animation: spin 1s linear infinite;
   animation: spin 1s linear infinite;
   z-index: 99;
 }
+
 .loading.fade {
   z-index: 0 !important;
   width: 98%;
   margin-top: 30px;
 }
+
 .loading.fade.in {
   z-index: 999 !important;
 }
+
 .content-fluid.pre-footer {
   background: #00b0ed;
   margin: 20px 0 -120px 0;
 }
+
 .blocks-container {
   position: relative;
   /*background: #00b0ed;*/
   width: 100%;
   max-width: 1200px;
   margin: 40px auto;
   display: table;
   /*border-radius: 4px;*/
   padding: 10px 0 14px 0;
 }
+
 @media (max-width: 1200px) {
   .blocks-container {
     width: 100%;
   }
+
   .container {
     width: 100%;
   }
+
   .container.newstyles {
     width: 100%;
   }
 }
+
 .block {
   width: 34%;
   padding: 10px 2% 30px 3%;
   float: left;
   position: relative;
   display: table-cell;
 }
+
 .block:after {
   content: "";
   background: #fff;
   width: 2px;
   height: 44%;
   position: absolute;
   top: 16%;
   right: 0;
 }
+
 .blocks-container .block:last-of-type {
   padding: 10px 0 30px 3%;
   width: 28%;
 }
+
 .blocks-container .block:last-of-type:after {
   content: "";
   background: none;
   width: 2px;
   height: 50%;
   position: absolute;
   top: 16%;
   right: 0;
 }
+
 .block h3 {
   color: white;
 }
+
 .block p {
   color: white;
   min-height: 70px;
   line-height: 22px;
   font-size: 14px;
 }
+
 .blocks-container .btn {
   background-color: #017cbc !important;
   border-radius: 4px;
   border: none;
   color: #fff;
   padding: 6px 14px !important;
   margin: 10px 10px 0 0;
   text-decoration: none;
   float: left;
   font-size: 13px;
   font-weight: normal;
   text-align: center;
   min-width: 150px;
 }
+
 .blocks-container a.btn:hover {
   background-color: #066CA1 !important;
   text-decoration: none;
 }
+
 .newstyles .list-group-item {
   margin-top: 10px;
 }
+
 .sidebar-links {
   background: #f0f0f2;
   padding: 0 0 10px 0;
   width: 215px;
   margin: 30px 0 10px 0;
   border-bottom: 20px solid #dfdfe0;
   float: left;
 }
+
 .sidebar-links:first-child {
   border-bottom: 0 solid #dfdfe0;
 }
+
 .sidebar-links.fix-search {
   position: fixed;
   top: 0;
 }
+
 .sidebar-links.slideup {
   background: transparent;
   border-bottom: 0 transparent;
   margin-left: -15px;
 }
+
 .sidebar-links.slideup h3 {
   background: transparent;
   color: #333;
   border-bottom: 3px solid #ddd;
   padding: 5px 0 14px 0;
   margin-left: 6px;
   max-width: 180px;
   transition: all .4s ease;
 }
+
 .sidebar-links.slideup a {
   font-size: 10.5pt;
   line-height: 19px;
 }
+
 .sidebar-links h3 {
   background: #8D8F96;
   border-top-right-radius: 6px;
   border-top-left-radius: 6px;
   padding: 10px 14px;
   color: white;
   margin: -10px 0 10px 0;
 }
+
 .sidebar-links ul {
   margin: 0;
   padding: 0 10px;
 }
+
 .sidebar-links li {
   list-style: none;
   padding: 4px 4px 6px 4px;
   margin: 0;
   font-size: 13px;
 }
+
 .sidebar-links li a {
   color: #333;
 }
+
 .sidebar-links p {
   margin: 0;
   padding: 6px 14px 0 14px;
 }
+
 .sidebar-links .RSS-link {
   font-size: 86%;
   background: transparent url(https://cdn.f5.com/websites/support/assets/images/icons/rss_icon_med.gif) no-repeat center left;
   padding: 1px 0 0 19px;
 }
+
 #help {
   float: left;
   margin: 20px 20px 0 14px;
   padding: 10px 23px;
 }
+
 .ihealth-popover {
   font-style: italic;
   padding: 2px 4px 6px 4px;
 }
-@media screen and (max-width: 991px), screen and (max-height: 700px) {
+
+@media screen and (max-width: 991px),
+screen and (max-height: 700px) {
   .sidebar-links.fix-search {
     position: relative !important;
   }
+
   .sidebar-links.slideup {
     margin-left: 0;
   }
 }
+
 @media (max-width: 991px) {
   .col-md-10.middlecontent {
     width: 100%;
     padding-right: 0;
     padding-left: 0;
   }
 }
+
 .take-tour {
   border: 1px solid #e5e5e5;
   border-radius: 3px;
   padding: 8px !important;
   background: #f0f0f2;
   font-weight: bold;
   margin: 10px 0 0 0 !important;
   width: 100%;
   max-width: 170px;
 }
+
 .glyphicon-dashboard:before {
   content: "\e141";
 }
+
 #tour {
   float: left;
   margin: 1px 6px 0px 0;
   padding: 0;
 }
+
 .tour-text {
   float: left;
   line-height: 18px;
 }
+
 .take-tour {
   float: left;
 }
+
 .take-tour:hover {
   color: black;
   background: #e8e8e8;
 }
+
 .st0 {
   fill: #333;
 }
+
 .st1 {
   fill: #333;
 }
+
 .st2 {
   fill: white;
 }
+
 .popover {
   font-size: .85em;
   border-radius: 4px;
   left: -55px;
 }
+
 .popover .arrow {
   display: none;
 }
+
 .popover .popover-inner .popover-content {
   padding: 9px 20px 20px 20px;
 }
+
 .popover .popover-inner .popover-content p {
   line-height: 15px;
   margin-bottom: 10px;
 }
+
 .popover #close {
   line-height: 0.5;
 }
+
 .popover .close {
   margin-right: -12px;
 }
+
 .pagination {
   padding: 20px;
   margin-bottom: 20px;
   float: left;
   width: 100%;
   border-top: 1px solid #ddd;
 }
+
 .pagination .results-per-page {
   float: right;
   margin: 0;
 }
+
 .pagination .results-per-page .results-per-page-label {
   font-size: 90%;
   font-weight: normal;
   margin: 2px 6px 0 0;
 }
+
 .pagination a:hover,
 .pagination a:active {
   text-decoration: none;
 }
+
 .pagination ul {
   list-style: none;
   float: left;
   margin: 0 0 6px 0;
   padding: 0;
 }
+
 .pagination ul li {
   float: left;
   display: inline;
   list-style: none;
   margin-right: 2px;
 }
+
 .pagination .spacing-dots {
   line-height: 34px;
   font-size: 110%;
   letter-spacing: 2px;
   margin: 0px 4px;
 }
+
 .pagination .glyphicon {
   margin: 1px -2px 0 -2px;
   padding: 0;
   font-size: 90%;
 }
+
 .pagination .glyphicon.glyphicon-chevron-right,
 .pagination .glyphicon.glyphicon-chevron-left {
   margin: 1px -1px 1px -2px;
 }
+
 .pagination .page {
   display: inline-block;
   padding: 1px 8px;
   margin-right: 3px;
   border-radius: 30px;
   border: solid 1px #EEEEEE;
   background: #ffffff;
   font-size: .875em;
   font-weight: bold;
   text-decoration: none;
   color: #717171;
   text-shadow: 0px 1px 0px #ffffff;
   line-height: 20px;
 }
+
 .pagination .page.gradient {
   background: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#f8f8f8), to(#e9e9e9));
   background: -moz-linear-gradient(0% 0% 270deg, #f8f8f8, #e9e9e9);
 }
+
 .pagination .page:hover,
 .pagination .page.gradient:hover {
   background: #fefefe;
   background: -webkit-gradient(linear, 0% 0%, 0% 100%, from(#FEFEFE), to(#f0f0f0));
   background: -moz-linear-gradient(0% 0% 270deg, #FEFEFE, #f0f0f0);
   border: solid 1px #EEEEEE;
 }
+
 .pagination .page.active {
   border: none;
   background: #2FB5B0;
   color: #fff;
   text-shadow: 0px 0px 3px rgba(0, 0, 0, 0.2);
   padding: 1px 8px 1px 8px;
   margin: 1px 4px 0 1px;
 }
+
 .pagination .page.label-default,
 .pagination .page .label-default {
   background-color: #e9e9e9;
 }
+
 .pagination .dftdropdown.label-default {
   background-color: #ffffff;
 }
+
 .scrollToTop {
   height: 40px;
   width: 40px;
   position: fixed;
   bottom: 20px;
   right: 20px;
   text-indent: -9999px;
@@ -1748,127 +2120,153 @@
   -webkit-transition-duration: 0.4s;
   -moz-transition-duration: 0.4s;
   transition-duration: 0.4s;
   opacity: 0.7;
   filter: alpha(opacity=70);
   z-index: 999;
 }
+
 .scrollToTop:hover {
   text-decoration: none;
   opacity: 1;
   filter: alpha(opacity=100);
   -webkit-transform: rotate(360deg);
   background: url('https://cdn.f5.com/websites/support/assets/images/up2.svg') no-repeat;
 }
+
 .alerts {
   background: #F0F0F2;
   height: 60px;
   overflow: hidden;
 }
+
 .alerts p {
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
   font-weight: normal !important;
   color: #333;
   text-align: left;
 }
+
 .alerts .date {
   font-family: Arial, Helvetica, sans-serif;
   font-weight: normal;
   font-size: 16px;
   padding-right: 10px;
 }
+
 .alerts .carousel-control.left,
 .alerts .carousel-control.right {
   display: none;
 }
+
 .alerts .carousel-control {
   z-index: 2;
 }
+
 .alerts .carousel-inner .item {
   opacity: 0;
   -webkit-transition-property: opacity;
   -moz-transition-property: opacity;
   -o-transition-property: opacity;
   transition-property: opacity;
 }
+
 .alerts .carousel-inner .active {
   opacity: 1;
 }
+
 .alerts .carousel-inner .active .left,
 .alerts .carousel-inner .active .right {
   left: 0;
 }
+
 .alerts .carousel-indicators {
   position: absolute;
   bottom: 0;
   left: auto;
   z-index: 15;
   padding-left: 0;
   margin-left: 0;
   width: 100%;
   top: 38px;
   text-align: right;
 }
+
 .alerts .carousel-indicators .active {
   background-color: #B0B0B0;
 }
+
 .alerts .carousel-indicators li {
   border: 1px solid #aeabab;
 }
+
 .alerts .item p {
   margin: 20px 0 10px;
 }
+
 .alerts .alert-item {
   max-height: 34px;
   float: left;
   overflow: hidden;
 }
+
 .alerts .alert-item img {
   max-height: 34px;
 }
+
 .alerts .alert-item img.icon {
   height: 21px;
   width: 23px;
   margin: -4px 6px 4px 0;
 }
+
 @media (max-width: 1000px) {
   .alerts {
     height: 100px;
   }
+
   .alerts .item p {
     min-height: 60px;
   }
+
   .alerts .carousel-indicators {
     top: 68px;
   }
 }
+
 .collapse-icon {
   width: 36px;
   float: left;
   margin: 0 0 0 -2px;
 }
+
 .activity-title {
   float: left;
   font-style: oblique;
   width: 90%;
 }
+
 .activity-text {
   float: left;
   margin-left: 34px;
   width: 100%;
 }
+
 .whatwhere.widericon {
   padding: 6px 6px;
 }
+
 .collapse-icon-fill {
   border: 1px solid transparent;
 }
+
 .attachment-activity {
   font-family: 'Glyphicons Halflings';
 }
+
 .close-cross {
   -webkit-appearance: none;
   cursor: pointer;
   background: 0 0;
   font-size: 11px;
   font-weight: 700;
   color: #000;
@@ -1876,600 +2274,712 @@
   filter: alpha(opacity=60);
   opacity: .6;
   border: 1px solid #ccc !important;
   padding: 0 4px 0 3px;
   line-height: 14px;
   border-radius: 3px;
 }
+
 .sr-steps {
   margin: 20px auto;
   display: table;
   padding: 20px 0 0 0;
 }
+
 .steps {
   font-size: 0.9em;
   line-height: 18px;
   margin: 8px 0 0 6px;
   font-weight: bold;
 }
+
 .row.form-group .text-danger {
   font-size: 13px;
   font-weight: normal;
   margin: 0 0 0 8px;
 }
+
 .row.form-group .text-danger a {
   color: #23527c;
   text-decoration: underline;
 }
+
 .char-count {
   margin: 4px 20px 0 0;
   font-size: 12px;
 }
+
 .statement-text {
   float: left;
   font-weight: normal;
   font-size: 13px;
   width: 100%;
 }
+
 h5.ttl-in-createSR {
   font-size: 90%;
   margin-top: 2px;
 }
+
 .slide-in-out.ng-hide-add,
 .slide-in-out.ng-hide-remove {
   /* ensure visibility during the transition */
   display: block !important;
   /* yes, important */
 }
+
 .slide-in-out,
 .fade-in-out.ng-show {
   transition: .25s linear all;
   max-height: 200px;
   overflow: hidden;
 }
+
 .slide-in-out.ng-hide {
   max-height: 0;
 }
+
 .confirmed .form-control {
   border-color: green;
 }
+
 .icon-check:before {
   content: "\f00c";
   color: green;
 }
+
 span.confirmed {
   font-family: Helvetica, sans-serif;
   font-size: 13px;
   color: green;
   margin: 0 0 0 8px;
 }
+
 .csp-article-type .article-actions {
   margin: 20px 16px;
   font-size: 18px;
   position: relative;
 }
+
 .csp-article-type .article-actions .glyphicon,
 .csp-article-type .article-actions [class^="icon-"],
 .csp-article-type .article-actions .article-actions [class*=" icon-"] {
   margin-right: 6px;
   background-color: #ccc;
   padding: 8px !important;
   border-radius: 30px;
   color: white;
   border: none !important;
   top: auto;
 }
+
 .csp-article-type .article-actions .glyphicon:hover,
 .csp-article-type .article-actions [class^="icon-"]:hover,
 .csp-article-type .article-actions [class*=" icon-"]:hover {
   background-color: #2D9E9A;
   cursor: pointer;
   border: none !important;
 }
+
 .csp-article-type .article-actions .glyphicon:active,
 .csp-article-type .article-actions [class^="icon-"]:active,
 .csp-article-type .article-actions [class*=" icon-"]:active,
 .csp-article-type .article-actions .glyphicon:focus,
 .csp-article-type .article-actions [class^="icon-"]:focus,
 .csp-article-type .article-actions [class*=" icon-"]:focus {
   cursor: pointer;
   border: none !important;
   outline: none;
 }
+
 .csp-article-type .article-actions .glyphicon.glyphicon-send {
   padding: 8px 10px 8px 6px !important;
 }
+
 .csp-article-type .article-actions .share.disabled [class^="icon-"],
 .csp-article-type .article-actions .share.disabled [class*=" icon-"] {
   background-color: #E6E6E6 !important;
   margin: 2px 4px 0 5px;
   cursor: default !important;
 }
+
 .csp-article-type a#downloadPdf {
   text-decoration: none;
 }
+
 .csp-article-type .faved {
   color: white !important;
 }
+
 .csp-article-type .form-control#shareViaEmail {
   font-size: 96%;
   margin: 6px 0;
   float: left;
 }
+
 .csp-article-type .share .dropdown-menu {
   padding: 14px 14px 20px 14px !important;
   left: -60px;
 }
+
 .csp-article-version .container-fluid.well.article-version {
   margin-left: 0;
 }
+
 .csp-article-version .dropdown-menu .dropdown-header ul {
   margin-top: 4px;
 }
+
 .csp-article-version a[data-toggle=dropdown] {
   font-weight: bold;
   font-size: 92%;
 }
+
 .feedback-outer-container {
   padding: 15px;
 }
+
 .feedback-outer-container .feedback-captcha {
   margin: 30px 0 15px 0;
 }
+
 .feedback-outer-container .feedback-submit {
   margin: 0;
 }
+
 .feedback-outer-container .feedback-message {
   margin: 15px 0 20px 0;
 }
+
 .feedback-outer-container .feedback-error-message {
   margin: 0 0 15px 0;
   color: #ff0000;
 }
+
 .guided-block {
   background-color: #00B0ED;
   float: none;
   color: white;
   border-radius: 5px;
   padding: 10px;
   margin: 0 auto;
   display: table;
 }
+
 .guided-block ::-webkit-input-placeholder {
   color: #fff;
 }
+
 .guided-block :-moz-placeholder {
   /* Firefox 18- */
   color: #fff;
 }
+
 .guided-block ::-moz-placeholder {
   /* Firefox 19+ */
   color: #fff;
 }
+
 .guided-block :-ms-input-placeholder {
   color: #fff;
 }
+
 .guided-block a {
   color: #fff;
 }
+
 .guided-block textarea:focus,
 .guided-block input:focus,
 .guided-block a:hover,
 .guided-block a:active,
 .guided-block a:focus,
 .guided-block a:hover h3 {
   color: #F3FDFF;
   text-decoration: none;
   outline: none;
 }
+
 .guided-block.full-width {
   width: 100%;
   background: #00A2E2 url('https://cdn.f5.com/websites/support/assets/images/bg-guided.jpg') repeat-x;
   background-position: bottom left;
   border-radius: 4px;
   margin-bottom: 10px;
 }
+
 .guided-block.full-width .glyphicon {
   padding: 6px;
   border: 1px solid #1885b1;
   border-radius: 30px;
   color: #0187bd;
   font-size: 18px;
   background: #ffffff;
   margin-right: 8px;
 }
+
 .guided-block.full-width .progress-container.prompt {
   width: 155px;
   margin: 10px;
   float: right;
   background: rgba(4, 84, 126, 0.43);
 }
+
 .guided-block.full-width .progress-container.prompt:hover {
   background: rgba(12, 54, 76, 0.43);
 }
+
 .guided-block.full-width .progress-container.prompt .highlight {
   color: black;
   font-weight: 700;
 }
+
 .guided-block.full-width .iu {
   padding-bottom: 8px;
 }
+
 .guided-block.full-width .iu h3 {
   color: #ffffff !important;
   margin: 10px 0 0 16px;
 }
+
 .guided-block .glyphicon {
   padding: 6px;
   border: 1px solid #E5E5E5;
   border-radius: 30px;
   color: #fff;
   font-size: 12px;
   margin-right: 4px;
 }
+
 .guided-block .text-danger.error {
   margin-left: 14px;
 }
+
 .progress-container {
   background: #017CBC;
   padding: 5px;
   width: 100%;
   color: #fff;
   margin-top: 10px;
   border-radius: 4px;
   font-size: 13px;
   line-height: 16px;
 }
+
 .progress-container.text {
   background: transparent;
 }
+
 .progress-container a {
   text-align: center;
   margin: 0 auto;
   padding: 5px;
   display: block;
 }
+
 .sidebar-links.guided-option {
   background: transparent;
   border-bottom: 0;
 }
+
 .sidebar-links.guided-option h3 {
   background: transparent;
   font-size: 17px;
   margin: 0;
   padding: 0;
 }
+
 .submit-search.lookup {
   background-color: transparent;
   border-color: rgba(0, 0, 0, 0);
   border-bottom-color: #717171;
   box-shadow: inherit;
   border-top-right-radius: 0;
   border-bottom-right-radius: 0;
   width: 90%;
   margin: 20px auto 0 auto;
   display: table;
   color: #9B9B9B;
   padding: 0 50px 2px 0;
 }
+
 .lookup-search-wrapper {
   width: 380px;
   float: left;
   margin: -18px 10px 4px -16px;
   transition: all .4s ease;
 }
+
 .lookup-search-wrapper.guided-full-width {
   width: 100%;
   float: left;
   margin: 0 0 0 18px;
   transition: all .4s ease;
   padding: 0 0 9px 0;
 }
+
 @media screen and (max-width: 992px) {
   .lookup-search-wrapper.guided-full-width {
     margin: 0;
   }
 }
+
 .lookup-search-wrapper.guided-full-width textarea {
   min-height: 26px;
   border-width: 2px;
   line-height: 1.5em;
   padding-bottom: 7px;
   box-sizing: border-box;
 }
+
 .lookup-search-wrapper.guided-full-width .submit-search.lookup {
   color: rgba(255, 255, 255, 0.94);
   border-bottom-color: rgba(255, 255, 255, 0.65);
   width: 100%;
   background: rgba(255, 255, 255, 0.15);
   padding: 4px 24px 4px 8px;
   border-radius: 3px;
   margin: 12px auto 0 auto;
 }
+
 .lookup-search-wrapper .searchwrapper.field {
   position: relative;
 }
+
 .lookup-search-wrapper .searchwrapper.field .reset {
   margin: 10px -4px 0 0px;
   position: relative;
   float: left;
   color: #9b9b9b;
 }
+
 .lookup-search-wrapper .searchwrapper.field .reset.wizard-option {
   margin: 12px 2px 0 0;
   position: relative;
   float: left;
   color: rgba(255, 255, 255, 0.9);
   background-color: transparent;
 }
+
 .lookup-search-wrapper .searchwrapper.field .reset:hover,
 .lookup-search-wrapper .searchwrapper.field .reset:focus {
   color: #4d4f53;
 }
+
 #submitWrapper #runSearchFromEnter {
   height: 1px;
   left: -9999px;
   position: absolute;
   width: 1px;
 }
+
 .search-filter .panel-group .panel {
   border-bottom: 1px solid #e5e5e5;
   border-radius: 0;
   box-shadow: 0 0 0 0 rgba(0, 0, 0, 0);
   margin-bottom: 10px;
 }
+
 .search-filter .panel-default {
   background-color: transparent;
   border-color: transparent;
   border-radius: 0;
   padding: 0;
 }
-.search-filter .panel-default > .panel-heading {
+
+.search-filter .panel-default>.panel-heading {
   border-color: transparent;
   background-color: transparent;
 }
+
 .search-filter .panel-heading {
   border-bottom: none;
   border-radius: 0;
   padding: 0;
 }
+
 .search-filter h4.panel-title {
   float: none;
   font-family: inherit;
 }
-.search-filter .panel-group .panel-heading + .panel-collapse > .panel-body,
-.search-filter .panel-group .panel-heading + .panel-collapse > .list-group {
+
+.search-filter .panel-group .panel-heading+.panel-collapse>.panel-body,
+.search-filter .panel-group .panel-heading+.panel-collapse>.list-group {
   border-top: none;
 }
+
 .search-filter .panel:last-child {
   border-bottom: 0 solid transparent !important;
 }
+
 .search-filter .panel-body {
   border: none;
   padding: 0 0 5px 0;
 }
+
 .search-filter .question-header {
   position: relative;
 }
+
 .search-filter .question-text {
   font-size: 13px;
   font-weight: bold;
   padding-bottom: 8px;
 }
+
 .search-filter .skipped-question-text {
   color: #dfdfdf;
 }
+
 .search-filter .selected-answers {
   color: #878787;
   font-size: 12px;
   font-weight: normal;
   padding-bottom: 8px;
 }
+
 .search-filter .caret.up {
   width: 0;
   height: 0;
   border-style: solid;
   border-width: 0 5px 8px 5px !important;
   border-color: transparent transparent #808080 transparent;
   position: absolute;
   right: 6px;
   top: 6px;
 }
+
 .search-filter .caret.down {
   width: 0;
   height: 0;
   border-style: solid;
   border-width: 8px 5px 0 5px !important;
   border-color: #c1c1c1 transparent transparent transparent;
   position: absolute;
   right: 6px;
   top: 6px;
 }
+
 .search-filter .accordion-toggle:link,
 .search-filter .accordion-toggle:visited,
 .search-filter .accordion-toggle:hover,
 .search-filter .accordion-toggle:active {
   outline: none;
   text-decoration: none;
 }
+
 .search-filter .completion-message {
   margin-right: 10px;
   margin-top: 0;
 }
+
 .filter-input-container {
   padding: 8px 2px 8px 2px;
 }
+
 .filter-input {
   background: #fff url('https://cdn.f5.com/websites/support/assets/images/multiple-select.png') no-repeat 100% -22px;
   border: 1px solid #d6d5d5;
   border-radius: 4px;
   font-family: sans-serif;
   font-size: 1em;
   min-height: 26px;
   outline: 0;
   padding: 0 20px 0 5px;
   width: 100%;
 }
+
 .question-tree {
   border: 1px solid #d6d5d5;
   border-radius: 4px;
   box-shadow: 0 4px 5px rgba(0, 0, 0, 0.08);
   padding: 0 5px 5px 5px;
 }
+
 .question-tree ul {
   list-style: none;
 }
+
 .question-tree ul li {
   font-size: 12px;
   line-height: 16px;
   padding: 0 4px 0 6px !important;
 }
+
 .question-tree ul li input[type=checkbox] {
   float: left;
   margin: 1px 4px 0 0;
 }
+
 .question-tree ul li label {
   color: #000000;
   font-size: 12px;
   font-weight: normal;
   margin-bottom: 2px;
   overflow: hidden;
   text-overflow: ellipsis;
   white-space: nowrap;
 }
+
 .answer-list {
   max-height: 300px;
   overflow: auto;
   padding-left: 0;
 }
+
 .answer-sub-list {
   padding-left: 20px;
 }
+
 .question-tree-container .apply-selected {
   width: 100%;
   margin-top: 10px;
 }
+
 .question-tree-container .apply-selected .duplicate-message {
   font-size: 12px;
   margin-left: 5px;
 }
+
 .question-tree-container .apply-selected .btn {
   margin-bottom: 5px;
 }
+
 .question-single-select label {
   color: #000000;
   font-size: 12px;
   font-weight: normal;
   margin-bottom: 2px;
   overflow: hidden;
   text-overflow: ellipsis;
   white-space: nowrap;
 }
+
 .question-single-select .question-container {
   line-height: 16px;
 }
+
 .question-container input {
   float: left;
   margin-right: 5px;
   margin-top: 0;
 }
+
 .question-tree ul.attribute-type {
   margin-top: 10px;
   margin-bottom: 10px;
 }
+
 .question-tree ul.attribute-type:last-child {
   margin-bottom: 0;
 }
+
 .guided-search-result .knownissue-title {
   float: left;
   position: absolute;
   z-index: 10;
   width: 35px;
   height: 35px;
   left: 15px;
 }
+
 .guided-search-result .truncate {
   overflow: hidden;
   white-space: normal;
 }
+
 .archived {
   margin: -4px 0 6px 0;
 }
+
 .archived label {
   font-weight: normal;
   margin: -3px 0 -3px -2px;
 }
+
 .guided-search .icon-1-5x.reset {
   font-size: 1.5em !important;
   position: relative !important;
   top: 0 !important;
   right: 0 !important;
   background: transparent none repeat scroll 0% 0%;
   border: medium none;
   display: inline;
   margin: 2px -20px 0px -36px !important;
   padding: 0;
   line-height: 34px;
   float: left;
   width: 30px;
 }
+
 .guided-search .icon-1-4x.reset {
   font-size: 1.2em !important;
   padding: 2px 0 2px 0;
   position: absolute;
 }
+
 .glyphicon.glyphicon-ok-sign {
   color: #1C9E99;
 }
+
 .guided-search .icon-1-5x.reset:hover,
 .guided-search .icon-1-5x.reset:active,
 .guided-search .icon-1-5x.reset:focus {
   border: none;
   outline: none;
 }
+
 .guided-search .icon-1-5x.reset:hover {
   cursor: pointer;
 }
+
 .guided-options .btn-xs,
-.guided-options .btn-group-xs > .btn {
+.guided-options .btn-group-xs>.btn {
   padding: 0;
   font-size: 16px;
   line-height: 0.2;
   border-radius: 4px;
   margin: -2px -22px 0px -26px;
   float: left;
   background-color: transparent;
   border-color: transparent;
   font-size: 22px;
   color: #606061;
 }
+
 .guided-options .btn-xs:focus,
-.guided-options .btn-group-xs > .btn:focus {
+.guided-options .btn-group-xs>.btn:focus {
   border: 1px solid transparent;
   outline: none;
 }
+
 .result-attribute span {
   color: #4D4F53;
   margin: 0 2px 0 0;
 }
+
 .sol-url {
   color: #AAAAAA;
 }
+
 .content-cont {
   float: left;
   margin: 10px 0;
 }
+
 .progress {
   height: 18px;
   margin-bottom: 10px;
   overflow: hidden;
   background-color: #f5f5f5;
   border-radius: 3px;
   -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
   box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
 }
+
 .progress-bar {
   float: left;
   width: 0;
   height: 100%;
   font-size: 11px;
   line-height: 18px;
   color: #fff;
@@ -2477,257 +2987,319 @@
   background-color: #479AE0;
   -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
   box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
   -webkit-transition: width .6s ease;
   -o-transition: width .6s ease;
   transition: width .6s ease;
 }
+
 .g-search-results p {
   margin-bottom: 20px;
 }
+
 .g-search-results .content-cont .glyphicon {
   display: none;
 }
+
 .g-search-results .content-cont.visited-link .glyphicon {
   display: inline !important;
 }
+
 .visited-link .glyphicon {
   margin-right: 4px;
   margin-left: 0;
   line-height: 20px;
 }
+
 .visited-link a,
 .visited-link a:visited {
   color: #727170;
 }
+
 .result-body {
   font-size: 88%;
 }
+
 .result-header {
   font-size: 98%;
 }
+
 .sol-num {
   font-weight: bold;
 }
+
 .sidebar-links.guided-option {
   background: transparent;
   border-bottom: 0;
 }
+
 .sidebar-links.guided-option h3 {
   font-size: 14px;
 }
+
 .admin-rma {
   margin: 0 0 10px 0;
 }
+
 .admin-rma input {
   margin: 3px 4px -2px 0;
   float: left;
   line-height: 0;
 }
+
 .admin-rma.radio label {
   padding-left: 0;
 }
+
 .create-rma-button {
   padding: 3px 10px;
 }
+
 .temp-SR {
   background: #f6f9fb;
   font-style: italic;
 }
+
 .temp-SR .sr-id.temp a {
   color: #ea8e04;
 }
+
 .ms .sorting .icon-1x {
   margin: 0 3px 2px 0;
 }
+
 .ms .sorting a,
 .ms .sorting a:hover {
   font-size: 90%;
   font-weight: bold;
   color: #4D4F53;
   text-decoration: none;
 }
+
 .ms .sorting a.no-hand:hover {
   cursor: default;
 }
+
 .ms .sorting .sorted {
   color: #949597;
 }
+
 .wrap-SR-search {
   margin: 6px 0;
 }
+
 .wrap-SR-search textarea:focus,
 .wrap-SR-search input:focus {
   outline: none;
 }
+
 .wrap-SR-search .lookup-search-wrapper {
   width: 380px;
   float: left;
   margin: -18px 10px 4px -16px;
   transition: all .4s ease;
 }
+
 .wrap-SR-search .lookup-search-wrapper .searchwrapper.field {
   margin: -32px 4px 0 0;
   position: relative;
 }
+
 .wrap-SR-search .submit-search.lookup {
   background-color: transparent;
   border-color: rgba(0, 0, 0, 0);
   border-bottom-color: #717171;
   box-shadow: inherit;
   border-top-right-radius: 0px;
   border-bottom-right-radius: 0px;
   width: 90%;
   margin: 20px auto 0 auto;
   display: table;
   color: #9B9B9B;
   padding: 0 50px 2px 0px;
 }
+
 .wrap-SR-search .SR-list-options {
   width: auto;
   float: left;
   margin: 6px 0 0 4px;
 }
+
 .wrap-SR-search .SR-list-options .clear-SR-queries {
   font-size: 96%;
   margin: 0 0 0 10px;
   float: right;
 }
+
 .wrap-SR-search .SR-list-options .filter-text {
   float: left;
 }
+
 .wrap-SR-search .SR-list-options .dropdown-menu {
   padding: 5px 16px 18px 2px !important;
   width: 280px;
 }
+
 .wrap-SR-search .SR-list-options .dropdown-menu.sr-filters .options li {
   padding: 0;
 }
+
 .wrap-SR-search .SR-list-options .dropdown-menu label {
   font-size: 90%;
   font-weight: 400;
   margin-bottom: 1px;
 }
+
 .wrap-SR-search .SR-list-options .dropdown-menu label input[type=radio],
 .wrap-SR-search .SR-list-options .dropdown-menu label input[type=checkbox] {
   margin: 1px 0 0;
 }
-.wrap-SR-search .SR-list-options .open > .dropdown-menu {
+
+.wrap-SR-search .SR-list-options .open>.dropdown-menu {
   display: block;
 }
+
 .wrap-SR-search .SR-list-options .btn-group.open .dropdown-toggle {
   -webkit-box-shadow: none;
   box-shadow: none;
 }
+
 .wrap-SR-search .icon-1x {
   margin: 2px 0 0 3px;
   float: left;
   font-size: 1.2em !important;
 }
+
 ul.sr-search-filters {
   float: left;
   font-size: 13px;
   margin: 8px 0 6px -40px !important;
 }
+
 ul.sr-search-filters li {
   float: left;
   list-style: none;
   margin: 0 4px;
 }
+
 ul.sr-search-filters .filter-text {
   float: left;
 }
+
 ul.sr-search-filters .icon-1x {
   margin: 0 0 0 3px;
   float: left;
   font-size: 1.2em !important;
 }
+
 .action-column {
   width: 30px;
 }
+
 .export-sr-excel {
   padding: 0 20px 0 0;
 }
+
 .export-sr-excel a:hover {
   text-decoration: none;
   color: #23527c;
 }
+
 .export-excel a:hover {
   text-decoration: none;
   color: #23527c;
 }
+
 .sr-search-filters {
   float: left;
   font-size: 13px;
   margin: 8px 0 6px -40px !important;
 }
+
 ul.sr-search-filters li {
   float: left;
   list-style: none;
   margin: 0 4px;
 }
+
 .create-sr-button {
   padding: 3px 10px;
 }
+
 .max-data-warning {
   font-size: 12px;
   font-style: italic;
 }
+
 .admin-sr {
   margin: 0 0 10px 0;
 }
+
 .admin-sr input {
   margin: 3px 4px -2px 0;
   float: left;
   line-height: 0;
 }
+
 .admin-sr.radio label {
   padding-left: 0;
 }
+
 .service-request-widget .load-container {
   overflow: inherit;
 }
+
 .confirmation-success h3 {
   color: green;
   margin-bottom: 8px;
 }
+
 .confirmation-success span {
   font-size: 14px;
 }
+
 .service-request .show-open {
   background-color: green;
 }
+
 .case-feedback {
   margin: 50px 0px 0 0px;
   padding: 4px;
   border-top: 1px solid #E0E0E0;
   font-size: 12px;
   text-align: right;
 }
+
 .service-request .icon-1x {
   font-size: 1.0em !important;
 }
+
 .service-request .icon-plus,
 .service-request .icon-minus {
   margin: -1px 0 2px -2px !important;
 }
+
 .service-request .rma-timer {
   font-size: 2em;
   font-style: normal;
 }
+
 .walkthrough {
   z-index: 999;
 }
+
 .walkthrough p {
   color: black;
 }
+
 .walkthrough .dropdown-menu.intro {
   padding: 5px !important;
   width: 350px;
 }
+
 .walkthrough .dropdown-menu.intro:before {
   content: "";
   display: block;
   position: absolute;
   width: 0;
   height: 0;
   border-color: transparent;
@@ -2735,23 +3307,27 @@
   border-style: solid;
   pointer-events: none;
   bottom: 100%;
   left: 50%;
   margin-left: -12px;
   border-bottom-color: #fff;
 }
+
 .walkthrough .dropdown-menu.right.intro:before {
   left: 80%;
 }
+
 .walkthrough .dropdown-menu.left.intro:before {
   left: 20%;
 }
+
 .walkthrough .dropdown-menu.top.intro:before {
   display: none;
 }
+
 .walkthrough .dropdown-menu.top.intro:after {
   content: '';
   display: block;
   position: absolute;
   width: 0;
   height: 0;
   border-color: transparent;
@@ -2759,102 +3335,120 @@
   border-style: solid;
   pointer-events: none;
   top: 100%;
   left: 50%;
   margin-left: -12px;
   border-top-color: #fff;
 }
+
 .walkthrough .dropdown-menu.welcome {
   padding: 30px !important;
   width: 550px;
 }
+
 .walkthrough .dropdown-menu.welcome h2 {
   margin-top: 5px;
 }
+
 .walkthrough .dropdown-menu.welcome:before {
   display: none;
 }
+
 .walkthrough .btn-primary {
   background-color: #2FB5B0;
   border-color: #2FB5B0;
 }
+
 .walkthrough .apply-selected {
   width: 100%;
   margin: 0 0 30px 0;
 }
+
 .walkthrough .admin {
   margin: 0 4px;
 }
+
 .inside-intro {
   padding: 14px;
   width: 100%;
   -moz-box-sizing: border-box;
   -webkit-box-sizing: border-box;
   box-sizing: border-box;
   font-size: 14px;
 }
+
 .intro-overlay {
   width: 100%;
   height: 100%;
   top: 0;
   left: 0;
   background: rgba(84, 97, 112, 0.39);
   position: fixed;
   z-index: 997;
 }
+
 .pop-out {
   position: relative;
   z-index: 998;
 }
+
 .csp-saved-knowledge-center-section-widget .wrap-article-section {
   padding: 14px 20px 14px 20px;
   background: #fff;
   margin: 10px 0 20px 0;
 }
+
 .csp-saved-knowledge-center-section-widget .wrap-article-section li {
   clear: left;
   list-style: none;
 }
+
 @media (max-width: 767px) {
   .csp-saved-knowledge-center-section-widget .wrap-article-section ul {
     margin: 0;
     padding: 0;
   }
 }
+
 .social-media-button {
   line-height: 1;
   vertical-align: baseline;
   display: inline-block;
   text-align: center;
 }
+
 .social-media-button .social-media-parent-container {
   padding: 0px;
   margin: 0px;
   text-indent: 0px;
   display: inline-block;
   vertical-align: baseline;
   font-size: 1px;
 }
+
 .social-media-button .social-media-container {
   position: relative;
   overflow: visible;
   display: block;
 }
+
 .social-media-button span {
   -webkit-box-sizing: content-box;
   -moz-box-sizing: content-box;
   box-sizing: content-box;
 }
+
 .social-media-button a:link,
 .social-media-button a:visited,
 .social-media-button a:hover,
 .social-media-button a:active {
   border: 0;
   text-decoration: none;
 }
+
 .social-media-button .title {
   color: #fff;
   cursor: pointer;
   display: block;
   white-space: nowrap;
   float: left;
   margin-left: 1px;
@@ -2868,19 +3462,21 @@
   border-radius: 2px;
   -webkit-border-radius: 2px;
   border-top-right-radius: 2px;
   border-bottom-right-radius: 2px;
   -webkit-border-top-right-radius: 2px;
   -webkit-border-bottom-right-radius: 2px;
 }
+
 .social-media-button .title .mark {
   display: inline-block;
   width: 0px;
   overflow: hidden;
 }
+
 .social-media-button .logo {
   cursor: pointer;
   border: 0;
   text-indent: -9999em;
   overflow: hidden;
   padding: 0;
   margin: 0;
@@ -2894,130 +3490,150 @@
   border-radius: 2px;
   -webkit-border-radius: 2px;
   border-top-right-radius: 2px;
   border-bottom-right-radius: 2px;
   -webkit-border-top-right-radius: 2px;
   -webkit-border-bottom-right-radius: 2px;
 }
+
 .social-media-button .title-text {
   color: #fff;
   font-size: 11px;
   font-family: Arial, sans-serif;
   font-weight: bold;
   font-style: normal;
   -webkit-font-smoothing: antialiased;
   display: inline-block;
   background: transparent none;
   vertical-align: top;
   height: 18px;
   line-height: 20px;
   float: none;
 }
+
 .linked-in-share .title {
   border-top-color: #0077b5;
   border-right-color: #0077b5;
   border-bottom-color: #0077b5;
   border-left-color: #0077b5;
   text-shadow: 0 -1px #005887;
   background-color: #0077b5;
   background-image: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #0077b5), color-stop(100%, #0077b5));
   background-image: -webkit-linear-gradient(top, #0077b5 0%, #0077b5 100%);
 }
+
 .linked-in-share .logo {
   background: #0077b5 url(assets/images/linkedIn-icon.png) no-repeat 0 0;
   border-right: 1px solid #066094;
 }
+
 .email-share .title {
   border-top-color: #B51B00;
   border-right-color: #B52200;
   border-bottom-color: #B50D00;
   border-left-color: #B50D00;
   text-shadow: 0 -1px #860F05;
   background-color: #B53C00;
   background-image: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #B52200), color-stop(100%, #B52200));
   background-image: -webkit-linear-gradient(top, #B52200 0%, #B54300 100%);
 }
+
 .email-share .logo {
   background: #b53600 url(assets/images/email-icon.png) no-repeat 0 0;
   border-right: 1px solid #872901;
 }
+
 .row.guided-search.federated {
   padding: 0;
 }
+
 .guided-search.federated .well .label-default,
 .guided-search.federated .well .tag {
   border: 1px solid #858E8E;
   background: #7C8685;
 }
+
 .whitesmoke.federated {
   padding: 0 0 20px 0;
   background-color: transparent !important;
   border: 0;
   border-right: 0 solid #E3E3E3;
   -webkit-box-shadow: inset 0 0 0 rgba(0, 0, 0, 0.01);
   box-shadow: inset 0 0 0 rgba(0, 0, 0, 0.01);
 }
+
 .whitesmoke h4.panel-title a {
   color: #337ab7;
   text-decoration: none;
 }
+
 .bigtab-selected {
   border-right: 1px solid #fff;
   margin-right: -5px;
 }
+
 .federated-search .search-entry-summary {
   border-bottom: 3px solid #ddd;
   margin: 15px 0 20px 0;
   padding-bottom: 25px;
 }
+
 .federated-search .search-entry-summary .reset-queries {
   float: right;
   margin: 0 0 8px 0;
 }
+
 .federated-search .search-entry-text {
   overflow: hidden;
   display: inline-block;
   margin-bottom: -10px;
 }
+
 .federated-search .g-search-wrapper.results {
   background-color: #FBFBFB;
   padding: 10px 10px 10px 10px;
   margin: 0;
   position: relative;
 }
+
 .federated-search .g-search-wrapper.results .name,
-.federated-search .g-search-wrapper.results .result-attribute > .value > span {
+.federated-search .g-search-wrapper.results .result-attribute>.value>span {
   color: #4D4F53;
 }
+
 .federated-search .g-search-wrapper .loading.fade {
   margin-top: 35px;
   margin-left: -20px;
   width: 100%;
 }
+
 .federated-search .g-search-wrapper .see-more {
   padding: 30px 0 0 58px;
   font-weight: 700;
 }
+
 .federated-search .small-title {
   margin: 22px 0 10px 4px;
   font-size: 13px;
   line-height: 20px;
 }
+
 .federated-search .federated-filter-box {
   background: #fbfbfb;
   color: #000;
   border: 1px solid #d6d5d5;
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
   padding: 14px 0 14px 10px;
   margin: 0 0 10px 0;
   float: left;
   width: 100%;
 }
+
 .federated-search .federated-filter-box .label-default.federated {
   font-size: 12px;
   line-height: 1;
   list-style: none;
   padding: 4px 6px 4px 6px;
   box-sizing: border-box;
   font-weight: normal;
@@ -3029,170 +3645,200 @@
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
   float: left;
   width: 95%;
   margin: 4px;
 }
+
 .federated-search .federated-filter-box ul.multiple-choice-list {
   margin: 1px 0 1px 6px;
   padding-left: 0;
 }
+
 .federated-search .federated-filter-box ul.multiple-choice-list li {
   line-height: 17px;
   padding: 0 4px 0 0 !important;
   font-size: 12px;
   list-style: none;
   margin: 0;
 }
+
 .federated-search .federated-filter-box ul.multiple-choice-list li label {
   font-weight: normal;
 }
+
 .federated-search .federated-filter-box ul.multiple-choice-list li input[type=radio],
 .federated-search .federated-filter-box ul.multiple-choice-list li input[type=checkbox] {
   margin: 1px 3px 0 0;
   line-height: normal;
   float: left;
 }
+
 .federated-search .federated-filter-box ul.multiple-choice-list li:last-child label {
   margin-bottom: 0;
 }
-.federated .panel-default > .panel-heading {
+
+.federated .panel-default>.panel-heading {
   color: #333;
   background-color: transparent;
   border-color: transparent;
 }
+
 .federated .panel {
   margin-bottom: 0;
   background-color: transparent;
   border: 0 solid transparent;
   border-radius: 0;
   -webkit-box-shadow: 0 0 0 rgba(0, 0, 0, 0.01);
   box-shadow: 0 0 0 rgba(0, 0, 0, 0.01);
 }
+
 .federated .panel-group {
   margin-bottom: 0;
 }
-.federated .panel-group .panel-heading + .panel-collapse > .panel-body,
-.federated .panel-group .panel-heading + .panel-collapse > .list-group {
+
+.federated .panel-group .panel-heading+.panel-collapse>.panel-body,
+.federated .panel-group .panel-heading+.panel-collapse>.list-group {
   border-top: 0 solid transparent;
 }
+
 ul.federated-tabs {
   padding-top: 0;
   padding-bottom: 0;
 }
+
 .federated-tabs h3 {
   font-size: 18px;
 }
+
 .federated-tabs li.active-tab,
 .federated-tabs li.non-active-tab,
-.federated-tabs .nav > li > a {
+.federated-tabs .nav>li>a {
   position: relative;
   float: left;
   list-style: none;
   border-radius: 4px 0 0 0;
   padding: 0 35px;
   background-color: transparent;
   -webkit-box-shadow: 1px 4px 3px rgba(0, 0, 0, 0.3);
   box-shadow: 1px 4px 3px rgba(0, 0, 0, 0.3);
 }
+
 .federated-tabs a {
   color: black;
   font-weight: 700;
   -webkit-user-select: none;
   /* Chrome/Safari */
   -moz-user-select: none;
   /* Firefox */
   -ms-user-select: none;
   /* IE10+ */
   /* Rules below not implemented in browsers yet */
   -o-user-select: none;
   user-select: none;
 }
+
 .federated-tabs li.active-tab {
   border-top: 4px solid #FBFBFB;
   background-color: #FBFBFB;
   padding-top: 10px;
 }
+
 .federated-tabs li.non-active-tab {
   border-top: 3px solid white;
   background-color: #F5F5F5;
   margin-top: 10px;
   margin-bottom: -2px;
   margin-left: 2px;
   border-bottom: none;
   border-bottom: 1px solid #ddd;
   z-index: 0;
 }
+
 .federated-tabs li.non-active-tab:hover {
   background-color: #f0f0f2;
   cursor: pointer;
 }
+
 .federated-tabs li.non-active-tab a {
   cursor: pointer;
   margin-bottom: -2px;
   background-color: transparent;
   line-height: 1.6;
 }
-.nav > li.active-tab > a:hover {
+
+.nav>li.active-tab>a:hover {
   background-color: transparent;
   border: 1px solid transparent;
   cursor: default;
 }
+
 .search-term {
   float: left;
   margin: 0 0 6px 0;
 }
+
 .f5-recommends {
   float: left;
   width: 100%;
   border-bottom: 1px solid #ddd;
   margin-bottom: 20px;
   padding-bottom: 10px;
 }
+
 .f5-recommends h4,
 .f5-recommends a {
   margin-left: 40px;
 }
+
 .g-search-results h4 {
   clear: both;
   margin-left: 40px;
 }
+
 .g-search-results p {
   margin-bottom: 10px;
 }
+
 .g-search-results input {
   float: left;
   margin: 3px 4px 0 0;
 }
+
 .g-search-results .archived label {
   vertical-align: super;
 }
+
 hr.thk-dvder {
   width: 100%;
   height: 4px;
   background-color: #d0d0d0;
   margin-top: 10px;
   margin-bottom: 10px;
   float: left;
 }
+
 .guided-search .g-search-wrapper {
   position: relative;
   min-height: 153px;
 }
+
 .guided-search .well [class^="icon-"],
 .guided-search .well [class*=" icon-"] {
   margin-left: 4px;
 }
+
 .guided-search .container-fluid.well .label-default:hover {
   color: #ffffff;
   border-color: #23A09B;
   background-color: #1DADA7 !important;
   cursor: pointer;
 }
+
 .guided-search .well .label-default,
 .guided-search .well .tag {
   font-size: 12px;
   line-height: 1;
   list-style: none;
   padding: 4px 2px 4px 8px;
   font-weight: normal;
@@ -3203,354 +3849,421 @@
   background: #16938E;
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
   margin: 0 2px 2px 2px;
   float: left;
 }
+
 .guided-search .btn-xs,
-.guided-search .btn-group-xs > .btn {
+.guided-search .btn-group-xs>.btn {
   padding: 0;
   font-size: 16px;
   line-height: 0.2;
   border-radius: 4px;
   margin: -2px -22px 0px -26px;
   float: left;
   background-color: transparent;
   border-color: transparent;
   font-size: 22px;
   color: #606061;
 }
+
 .guided-search .btn-xs:focus,
-.guided-search .btn-group-xs > .btn:focus {
+.guided-search .btn-group-xs>.btn:focus {
   border: 1px solid transparent;
   outline: none;
 }
+
 .guided-search .small-title {
   margin: 0 0 10px 4px;
   font-size: 13px;
   line-height: 20px;
 }
+
 .guided-search .loading.fade {
   margin-top: inherit;
   width: 100%;
 }
+
 .guided-search .loading {
   top: inherit;
 }
+
 .guided-search .reset-wizard {
   margin: 3px -5px 0 6px;
   float: right;
 }
+
 .guided-search .search-entry-summary {
   border-bottom: 3px solid #ddd;
   color: #000;
   margin: 4px 4px 15px 4px;
   overflow: hidden;
   padding: 0 0 5px 0;
 }
+
 .guided-search .additional-links {
   border-top: 3px solid #ddd;
   color: #000;
   margin: 0 4px 0 4px;
   overflow: hidden;
   padding: 0 0 5px 0;
   font-size: 13px;
   font-weight: bold;
   text-align: right;
 }
+
 .guided-search .additional-links .link-container {
   padding: 15px 0 0 0;
 }
+
 .guided-search .additional-links .create-service-request {
   margin-top: -4px;
 }
+
 .g-search-results-toggle {
   display: none;
 }
+
 .selected ul li {
   display: inline;
   list-style: none;
   float: left;
 }
+
 .selected ul {
   margin: 0;
   padding: 0;
 }
+
 .admin {
   padding: 3px 10px;
   margin: 0 4px;
 }
+
 .admin.clearall {
   padding: 3px 24px 3px 10px;
 }
+
 .text-search {
   font-weight: bold;
 }
+
 .filter-container {
   padding: 2px 0;
 }
+
 .filter-container.filter-container:nth-last-child(2) {
   padding-bottom: 3px !important;
   margin-bottom: 6px;
 }
+
 .no-indent {
   margin-left: -40px !important;
 }
+
 .no-indent label {
   display: inline;
 }
+
 .guided-options {
   margin-left: -14px;
 }
+
 .guided-options label {
   font-weight: normal;
   margin-bottom: 4px;
 }
+
 .guided-options li {
   list-style: none;
 }
+
 label.question {
   font-weight: bold;
   width: 94%;
 }
+
 .printonly {
   visibility: hidden;
 }
+
 .products-link-row {
   border-bottom: 3px solid #ddd;
 }
+
 .products-link {
   font-size: 13px;
   float: right;
   font-weight: bold;
   width: 100%;
   text-align: right;
 }
+
 @media (max-width: 767px) {
   .guided-options li ul {
     margin-left: -20px !important;
   }
+
   .col-xs-4.whitesmoke {
     width: 90%;
     margin: 0 5% 0 5%;
   }
+
   .g-search-results {
     opacity: 1;
     margin-top: 36px;
     width: 100%;
     background-color: #ffffff;
     z-index: 98;
     top: 0;
     left: 0;
     padding-bottom: 50px;
   }
+
   .g-search-results-toggle {
     position: absolute;
     right: 20px;
     display: inline-block;
     z-index: 99;
   }
+
   .footer .col-sm-3.col-md-2 {
     display: none;
   }
+
   .g-search-results h5 {
     margin-left: 20px;
   }
+
   .whitesmoke.federated {
     margin-top: 35px;
   }
 }
+
 @media (max-width: 640px) {
   form.search .btn-primary {
     padding: 8px 12px !important;
   }
 }
+
 .row.search-wrapper,
 .row.guided-search {
   padding: 20px 0 20px 0;
 }
+
 h1.welcome-text {
   height: 49px;
 }
+
 .knowledge-centers {
   position: relative;
   padding-bottom: 10px;
 }
+
 .knowledge-centers.home {
   display: table;
 }
+
 .knowledge-centers.home .kc-box-wrap {
   box-shadow: 0 1px 2px 0 rgba(200, 200, 200, 0.7);
   border-top: 4px #d3d3d3 solid;
   padding: 0 20px 20px 20px;
   float: left;
   position: relative;
   display: inline-block;
   margin: 0 20px 0 16px;
   background: #fefefe url('https://cdn.f5.com/websites/support/assets/images/bg-kc2.jpg') no-repeat;
   background-position: top right;
   border-radius: 4px;
 }
+
 .knowledge-centers.home ul li {
   line-height: 18px;
   padding: 2px 0 2px 0 !important;
   float: left;
   width: 100%;
 }
+
 h2.home-header {
   margin-bottom: 15px;
 }
+
 .middlecontent .pane {
   min-height: 20px;
   padding: 22px 10px 8px 10px;
   margin-bottom: 20px;
   background-color: #f2f2f4;
   border-radius: 4px;
   -webkit-box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.15);
   box-shadow: 1px 1px 2px rgba(0, 0, 0, 0.15);
   float: left;
   width: 100%;
   /* border-top: 4px solid #cecece; */
 }
+
 .middlecontent .pane-icon {
   width: 40px;
   float: left;
 }
+
 .middlecontent .pane-icon .icon-1-5x,
 .middlecontent .pane-icon .icon-2x {
   padding: 7px;
   border: 1px solid #C0BABA;
   border-radius: 30px;
   color: #787878;
   background: #fff;
 }
+
 .middlecontent .pane-text {
   float: right;
   width: 86%;
 }
+
 .middlecontent .pane-text h3 {
   padding: 0;
   margin: 0;
 }
+
 .middlecontent .pane-text a {
   color: #333;
   font-size: 96%;
 }
+
 .middlecontent .pane-text a,
 .middlecontent .pane-text h3,
 .middlecontent .pane-text p {
   text-decoration: none;
 }
+
 .row.home-tasks {
   margin-top: 35px;
 }
+
 @media (max-width: 600px) {
   .row.home-tasks {
     margin-top: 0;
   }
 }
+
 .article-container h2 {
   margin-top: 0;
 }
+
 .article-container .dropdown-menu {
   padding: 5px 16px 18px 2px !important;
   width: 280px;
 }
+
 .article-container .dropdown-menu .dropdown-header {
   display: block;
   padding: 3px 20px;
   font-size: 12px;
   line-height: 1.42857143;
   color: #343434;
   white-space: normal !important;
   width: 100%;
   margin: 2px 0;
   float: left;
 }
+
 .article-container .dropdown-menu .text-danger {
   color: #a94442;
   margin: 0 auto;
   display: table;
   font-size: 90%;
   font-weight: bold;
   padding: 0 0 4px 0;
 }
+
 .article-container .dropdown-menu ul {
   padding: 0;
   margin: 0;
 }
+
 .article-container .dropdown-menu ul li {
   float: left;
   list-style-type: none;
   margin: 0 5px 0 0;
 }
+
 .article-container .article-content ul {
   list-style-position: outside;
   list-style-type: disc;
   font-size: 14px;
   padding-left: 15px;
   margin: 10px 0 15px 25px;
   clear: both;
 }
+
 .article-container .article-content ul ul {
   list-style-type: circle;
   display: block;
   margin-bottom: 15px;
 }
+
 .article-container .article-content ol {
   clear: both;
 }
+
 .article-container .btn.dropdown-toggle {
   border: 1px solid rgba(163, 160, 160, 0.3);
   background-color: white;
 }
+
 .article-container .caret.larger {
   display: inline-block;
   width: 0;
   height: 0;
   margin-right: 8px;
   margin-left: 6px;
   float: right;
   margin-top: 8px;
   vertical-align: middle;
   border-top: 7px solid;
   border-right: 6px solid transparent;
   border-left: 6px solid transparent;
 }
+
 .article-container h4,
 .article-container .sectiontitle {
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
   font-weight: normal !important;
   color: #000;
   font-size: 16px;
   margin: 18px 0 10px 0;
   float: left;
   width: 100%;
 }
+
 .article-container h5,
 .article-container .subsectiontitle {
   font-weight: bold;
   font-size: 14px;
   margin: 20px 0 0 0;
 }
+
 .article-container .note {
   padding: 6px 0;
   font-weight: normal;
   font-style: italic;
   color: #078A85;
 }
+
 .article-container .code {
   padding: 2px 4px;
   font-size: 100%;
   color: #000;
   background-color: #ebebeb;
   border-radius: 4px;
   font-family: Menlo, Monaco, Consolas, "Courier New", monospace;
 }
+
 .article-container .important,
 .article-container .warning {
   display: block;
   padding: 9.5px;
   margin: 10px 0 10px;
   font-size: 14px;
   line-height: 1.42857143;
@@ -3559,121 +4272,138 @@
   border: 1px solid #e3e3e3;
   border-radius: 4px;
   font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
   font-weight: normal;
   float: left;
   width: 100%;
 }
+
 .article-container .exsample {
   float: left;
   width: 100%;
   margin: 16px 0 6px 0;
 }
+
 .article-container .example,
 .article-container .example2,
 .article-container pre {
   padding: 2px 4px;
   font-size: 100%;
   color: #000;
   background-color: transparent;
   border-radius: 4px;
   border: 0;
   font-family: Menlo, Monaco, Consolas, "Courier New", monospace;
 }
+
 .article-container .impact {
   font-style: italic;
   color: #545454;
   font-weight: normal;
 }
+
 .article-container .kbd,
 .article-container kbd {
   padding: 2px 4px;
   font-size: 100%;
   color: #000;
   background-color: #ebebeb;
   border-radius: 3px;
   -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0);
   box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0);
   font-family: Menlo, Monaco, Consolas, "Courier New", monospace;
 }
+
 .article-container table.askf5table tr:first-child {
   padding: 4px;
   font-weight: bold;
   font-size: 10pt;
   vertical-align: bottom;
   background-color: #f5f5f5;
 }
+
 .article-container .article-status {
   color: #a70000;
 }
+
 .article-container .table-responsive {
   overflow-x: inherit !important;
 }
+
 tr td:nth-last-child(n+5),
-tr td:nth-last-child(n+5) ~ td {
+tr td:nth-last-child(n+5)~td {
   font-size: 90%;
 }
+
 tr td:nth-last-child(n+9),
-tr td:nth-last-child(n+9) ~ td {
+tr td:nth-last-child(n+9)~td {
   font-size: 84%;
 }
+
 .new-articles-container .icon-mail:before,
 .new-articles-container .icon-envelope:before {
   margin-right: 1px;
 }
+
 .new-articles-container .check-filter,
 .new-articles-container .check-filter input[type="checkbox"],
 .new-articles-container .check-filter input[type="radio"] {
   font-weight: 400;
   float: left;
   margin: 6px 3px 0 0;
 }
+
 .new-articles-container .check-filter-text {
   float: left;
   margin: 5px 12px 0 0;
   font-size: 12px;
 }
+
 .new-articles-container h4 {
   color: #000;
   float: left;
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
   font-size: 16px;
   font-weight: normal !important;
   margin: 13px 0 10px 0;
   width: 100%;
 }
+
 .new-articles-container h7 {
   font-size: 14px;
   font-weight: bold;
   margin: 10px 0;
   float: left;
   color: #000;
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
 }
+
 .new-articles-container .caret.larger {
   display: inline-block;
   width: 0;
   height: 0;
   margin-right: 8px;
   margin-left: 6px;
   float: right;
   margin-top: 8px;
   vertical-align: middle;
   border-top: 7px solid;
   border-right: 6px solid transparent;
   border-left: 6px solid transparent;
 }
+
 .new-articles-container .subscribe-updates {
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
   font-weight: normal !important;
   color: #333;
   font-size: 14px;
   margin: 4px 6px 4px 0;
   float: right;
 }
+
 .new-articles-container .flexcontainer {
   list-style: none;
   display: -webkit-box;
   display: -moz-box;
   display: -ms-flexbox;
   display: -webkit-flex;
   display: flex;
@@ -3682,19 +4412,21 @@
   align-items: flex-start;
   flex-flow: wrap;
   -webkit-flex-wrap: wrap;
   flex-wrap: wrap;
   -ms-writing-mode: lr-tb;
   -ms-flex-wrap: wrap;
 }
+
 .new-articles-container .container-fluid.well {
   margin-left: 0;
   margin-right: 0;
   margin-bottom: 10px;
 }
+
 .new-articles-container .container-fluid.well .label-default {
   font-size: 14px;
   line-height: 1;
   list-style: none;
   padding: 8px 6px 8px 6px;
   margin-right: 10px;
   font-weight: normal;
@@ -3703,164 +4435,197 @@
   color: #777777;
   border: 1px solid #ccc;
   background: #fff;
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
 }
+
 .new-articles-container .container-fluid.well .label-default[disabled].disabled:hover {
   pointer-events: none;
   cursor: not-allowed;
   color: #777777;
   border: 1px solid #ccc;
   background-color: #E6E6E6 !important;
 }
+
 .new-articles-container .RSS-link {
   font-size: 86%;
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/rss_icon_med.gif') no-repeat center left;
   padding: 1px 0 0 22px;
   margin: 0 0 0 14px;
 }
+
 .new-articles-container .no-results {
   margin-top: 10px;
 }
+
 .new-articles-container .loading.fade {
   margin-top: 35px;
 }
+
 .new-articles-container select[disabled].disabled {
   pointer-events: none;
 }
+
 .new-articles-container .tooltip-trigger.flex2 {
   margin-right: 10px;
 }
+
 .new-articles-container .tooltip-trigger .flex2 {
   width: 100%;
 }
+
 @media (max-width: 900px) {
   .new-articles-container .container-fluid.well .label-default {
     font-size: 11px;
     padding: 5px;
     margin-bottom: 10px;
   }
+
   .new-articles-container .flexcontainer .btn-primary {
     padding: 2px 8px;
   }
+
   .new-articles-container .flex1,
   .new-articles-container .flex2,
   .new-articles-container .flex3,
   .new-articles-container .flex4 {
     width: 40%;
   }
+
   .new-articles-container .newstyles {
     padding: 0 10px !important;
   }
+
   .new-articles-container .RSS-link {
     width: 100%;
     float: left;
     margin: 10px 0 0 0;
   }
 }
+
 @media (max-width: 700px) {
   .new-articles-container .RSS-link {
     width: 100%;
     float: left;
     margin: 10px 0 0 0;
   }
 }
+
 @media (max-width: 600px) {
   .new-articles-container .flexcontainer {
     -webkit-flex-flow: column wrap;
     flex-flow: column wrap;
     padding: 0;
   }
+
   .new-articles-container .container-fluid.well .label-default {
     width: 90%;
     max-width: 300px;
   }
+
   .new-articles-container .tooltip-trigger.flex2 {
     width: 90%;
     max-width: 300px;
   }
+
   .new-articles-container .tooltip-trigger .flex2 {
     width: 100% !important;
   }
+
   .new-articles-container .subscribe-updates {
     width: 100%;
     float: left;
   }
 }
+
 @media (max-width: 430px) {
   .new-articles-container .well {
     padding: 10px;
   }
 }
+
 .new-articles-container .result-attribute span {
   color: #4D4F53;
 }
+
 .new-articles-container .result-attribute span.sol-url {
   color: #AAAAAA;
 }
+
 .new-articles-container .btn-group.open .dropdown-toggle {
   -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0);
   box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0);
 }
+
 .new-articles-container .dropdown-menu {
   padding: 5px 16px 18px 2px !important;
   width: 280px;
 }
+
 .new-articles-container .dropdown-menu .dropdown-header {
   display: block;
   padding: 3px 20px;
   font-size: 12px;
   line-height: 1.42857143;
   color: #343434;
   white-space: normal !important;
   width: 100%;
   margin: 2px 0;
   float: left;
 }
+
 .new-articles-container .dropdown-menu.sr-filters input[type=radio] {
   margin: 0 5px 0 -10px;
   width: 20px;
   height: 16px;
   line-height: 16px;
   float: left;
 }
+
 .new-articles-container ul.date-filter ul li {
   list-style: none;
   padding: 0;
 }
+
 .new-articles-container ul.date-filter ul li label {
   margin: 2px 5px;
   font-weight: 400;
 }
+
 .new-articles-container .btn-primary[disabled],
 .new-articles-container .btn-primary.disabled {
   color: #777;
   background-color: #E6E6E6;
   border-color: #ccc;
   opacity: 1;
 }
+
 .request-case-access .align-label {
   line-height: 30px;
 }
+
 .tech-documents label {
   margin: 8px 10px 0 0;
   font-weight: 400;
 }
+
 .tech-documents input {
   vertical-align: middle;
   position: relative;
   top: -3px;
 }
+
 .tech-documents .container-fluid.well {
   margin-left: 0;
   margin-right: 0;
   margin-bottom: 10px;
 }
+
 .tech-documents .container-fluid.well .label-default {
   font-size: 14px;
   line-height: 1;
   list-style: none;
   padding: 8px 6px 8px 6px;
   margin-right: 10px;
   font-weight: normal;
@@ -3869,38 +4634,42 @@
   color: #777777;
   border: 1px solid #ccc;
   background: #fff;
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
 }
+
 .tech-documents .container-fluid.well .label-default[disabled].disabled:hover {
   pointer-events: none;
   cursor: not-allowed;
   color: #777777;
   border: 1px solid #ccc;
   background-color: #E6E6E6 !important;
 }
+
 .tech-documents h4 {
   color: #000;
   float: left;
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
   font-size: 16px;
   font-weight: normal !important;
   margin: 13px 0 10px 0;
   width: 100%;
 }
+
 .tech-documents h7 {
   font-size: 14px;
   font-weight: bold;
   margin: 5px 0 10px 0;
   float: left;
   color: #000;
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
 }
+
 .tech-documents .flexcontainer {
   list-style: none;
   display: -webkit-box;
   display: -moz-box;
   display: -ms-flexbox;
   display: -webkit-flex;
   display: flex;
@@ -3909,684 +4678,829 @@
   align-items: flex-start;
   flex-flow: wrap;
   -webkit-flex-wrap: wrap;
   flex-wrap: wrap;
   -ms-writing-mode: lr-tb;
   -ms-flex-wrap: wrap;
 }
+
 .tech-documents .btn-primary[disabled],
 .tech-documents .btn-primary.disabled {
   color: #777;
   background-color: #E6E6E6;
   border-color: #ccc;
   opacity: 1;
 }
+
 .tech-documents .document-types {
   margin-top: 10px;
 }
+
 .tech-documents .document-types ul {
   list-style: none;
   margin: 0;
   padding: 0;
 }
+
 .tech-documents .document-types li {
   display: inline;
 }
+
 .tech-documents .no-results {
   margin-top: 10px;
 }
+
 .tech-documents .loading.fade {
   margin-top: 35px;
 }
+
 .tech-documents .selected-document-filters {
   margin: 10px 0;
 }
+
 .tech-documents select[disabled].disabled {
   pointer-events: none;
 }
+
 .tech-documents .tooltip-trigger.flex2 {
   margin-right: 10px;
 }
+
 .tech-documents .tooltip-trigger .flex2 {
   width: 100%;
 }
+
 @media (max-width: 900px) {
   .tech-documents .container-fluid.well .label-default {
     font-size: 11px;
     padding: 5px;
     margin-bottom: 10px;
   }
+
   .tech-documents .flexcontainer .btn-primary {
     padding: 2px 8px;
   }
+
   .tech-documents .flex1 {
     width: 40%;
   }
+
   .tech-documents .tooltip-trigger.flex2 {
     width: 25%;
   }
+
   .tech-documents .newstyles {
     padding: 0 10px !important;
   }
+
   .tech-documents .RSS-link {
     width: 100%;
     float: left;
     margin: 10px 0 0 0;
   }
 }
+
 @media (max-width: 600px) {
   .tech-documents .flexcontainer {
     -webkit-flex-flow: column wrap;
     flex-flow: column wrap;
     padding: 0;
   }
+
   .tech-documents .container-fluid.well .label-default {
     width: 90%;
     max-width: 300px;
   }
+
   .tech-documents .tooltip-trigger.flex2 {
     width: 100%;
   }
 }
+
 @media (max-width: 430px) {
   .tech-documents .well {
     padding: 10px;
   }
 }
+
 .site-feedback .connect-message {
   margin: 15px 0;
 }
+
 .site-feedback .select-feedback-topic {
   width: 300px;
 }
+
 .site-feedback .feedback-text {
   margin-top: 20px;
 }
+
 .site-feedback .feedback-captcha {
   margin: 10px -15px 20px -15px;
 }
+
 .site-feedback .feedback-submit {
   margin: 0;
 }
+
 .site-feedback .feedback-message {
   margin: 15px -15px 20px -15px;
 }
+
 .site-feedback .feedback-error-message {
   margin: 15px -15px 20px -15px;
   color: #ff0000;
 }
+
 .searchwrapper.field {
   margin: -36px -2px 0 0;
 }
+
 .submit-search.srs {
   background-color: #fff;
   border-color: #E2E2E2;
   box-shadow: inherit;
   border-top-right-radius: 3px;
   border-bottom-right-radius: 3px;
   width: 100%;
   margin: 0px;
   padding-right: 40px;
   display: table;
 }
+
 .table-bordered {
   background-color: #fff;
 }
+
 .customize {
   margin: 20px 10px 10px 0;
 }
+
 .customized-warning {
   float: right;
   width: 100%;
   text-align: right;
   font-size: 96%;
   color: #2D908C;
   margin: 0 10px 0 0;
 }
-.customized-warning > .glyphicon {
+
+.customized-warning>.glyphicon {
   margin-right: 2px;
 }
+
 #sortable input {
   width: 24px;
   height: 24px;
   position: absolute;
   left: 10px;
   top: 5px;
 }
+
 ul#sortable {
   float: left;
   width: 100%;
   margin: 0 0 20px -20px;
 }
+
 ul#sortable li {
   margin: 4px 0;
   clear: left;
   list-style: none;
   position: relative;
   line-height: 24px;
   padding: 8px 0 10px 43px;
   background: #f5f5f5;
   border: solid #E6E6E6;
   border-width: 2px;
   font-size: 11pt;
 }
+
 ul#sortable.draggable li {
   cursor: crosshair;
   border: 2px dashed #E6E6E6;
 }
+
 ul#sortable.draggable li:hover {
   cursor: move;
   background: #ECECEC !important;
   border: 2px dashed #D9D9D9;
 }
+
 .modal h6 {
   margin: 0 0 10px 15px;
   line-height: 20px;
   font-weight: normal;
 }
+
 .srs-wrapper {
   width: 42%;
   float: left;
   margin: 0 4px 0 0;
 }
+
 .results-per-page.requests {
   margin-bottom: 5px;
 }
+
 .results-per-page.requests .label-default {
   padding: 3px 6px 3px 6px !important;
 }
+
 ul.sr-filters ul li {
   list-style: none;
   padding: 2px 0;
 }
+
 ul.sr-filters ul li input[type=checkbox] {
   width: 16px;
   height: 16px;
   float: left;
   margin: 1px 5px 0 0;
 }
+
 .glyphicon.pr-view {
   margin: -1px 7px 0 0;
   font-size: 20px;
   float: left;
 }
+
 .dropdown a {
   font-size: 96%;
 }
+
 .dropdown a:hover,
 .dropdown a:active,
 .dropdown a:focus {
   text-decoration: none;
 }
+
 table.askf5table.ms tr:first-child {
   background-color: #E2E2E2;
 }
+
 .narrow-col {
   width: 110px;
 }
+
 .narrow-col-sm {
   width: 36px;
 }
+
 .term {
   font-weight: bold;
   font-style: oblique;
   padding: 0 0 4px 0;
   display: block;
 }
+
 .sr-search-txt {
   font-size: 96%;
   margin: 0 0 4px 6px;
 }
+
 .ms .icon-1x {
   font-size: 1.1em !important;
   margin: 0 2px 0 0;
   float: left;
   padding: 0;
   line-height: 18px;
 }
+
 .ms .article-actions {
   margin: 0 auto !important;
   display: table;
 }
+
 .disabled {
   background-color: #E6E6E6 !important;
   border-radius: 30px;
 }
+
 .faved,
 .subscribed {
   background-color: #4F8D97 !important;
 }
+
 .faved:hover,
 .subscribed:hover {
   background-color: #2D9E9A !important;
 }
+
 .not-subscribed {
   background-color: #ccc !important;
 }
+
 .not-subscribed:hover {
   background-color: #2D9E9A !important;
 }
+
 .this-wraps {
   width: 100%;
   min-width: 380px;
   float: left;
   white-space: normal !important;
   margin: 0;
 }
+
 .bordered {
   padding: 1px 4px;
   border: 1px solid #DDDDDD;
   border-radius: 4px;
   margin: 2px;
   line-height: 24px;
 }
+
 .customized-icon {
   color: #2FB5B0;
   cursor: pointer;
 }
+
 .being-edited {
   background-color: rgba(245, 241, 226, 0.44);
   border: 2px dashed #E6ECEF !important;
 }
+
 .article-actions .glyphicon,
 .article-actions [class^="icon-"],
 .article-actions [class*=" icon-"] {
   margin-right: 6px;
   background-color: #ccc;
   padding: 8px !important;
   border-radius: 30px;
   color: white;
   border: none !important;
   -webkit-transition: all .4s ease;
   transition: all .4s ease;
 }
+
 .table-sort {
   cursor: pointer;
 }
+
 .load-container {
   position: relative;
   overflow: hidden;
 }
+
 .load-container .loading.fade {
   width: 100%;
 }
+
 .admin-impersonate {
   float: right;
   margin: 14px 2px 0 0;
   font-size: 13px;
   font-weight: normal;
   padding: 4px 14px;
   background-color: #f5f5f5;
   border: 1px solid #e3e3e3;
   border-radius: 4px;
   -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
   box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
 }
+
 .admin-impersonate-name,
 .admin-impersonate-text.impersonated-view {
   color: #e51837;
 }
+
 .my-support-home h2 {
   margin-top: 10px;
   margin-bottom: 0;
 }
+
 .support-feedback {
   margin: 10px 0 0;
   padding: 4px;
   border-top: 1px solid transparent;
   font-size: 12px;
   text-align: right;
 }
+
 .service-request .label-text {
   font-size: 0.9em;
   line-height: 14px;
 }
+
 .whatwhere {
   color: white;
   background-color: #6a6c73;
   padding: 6px 9px;
   margin: 4px 8px 4px 0;
   border-radius: 20px;
   font-size: 14px !important;
   line-height: 12px;
   -webkit-transition: all .4s ease;
   transition: all .4s ease;
 }
+
 .icon-new-window.whatwhere {
   padding: 6px 6px;
 }
+
 .service-request .form-field-addons {
   font-size: 0.9em;
   line-height: 14px;
   text-decoration: none;
 }
+
 .service-request .form-field-addons .serial-number-tip {
   line-height: 34px;
 }
+
 .form-field-addons .radio.preferred {
   margin-bottom: 0;
 }
+
 .form-field-addons .radio.preferred input[type=radio] {
   margin-top: 0 !important;
 }
+
 .service-request hr {
   margin-top: 30px;
   margin-bottom: 20px;
   border: 0;
   border-top: 1px solid #E0E0E0;
 }
+
 .service-request h5 {
   margin-top: 26px;
   margin-bottom: 20px;
 }
+
 .form-group.hasradio {
   margin-bottom: 6px;
 }
+
 .service-request .label-text.tall {
   line-height: 34px;
 }
+
 .hasradio .control-label {
-  margin-top: 10px ;
+  margin-top: 10px;
 }
+
 .hasradio label {
   margin-right: 14px;
 }
+
 .service-request textarea {
   min-height: 80px;
 }
+
 .desc,
 .desc6 {
   display: none;
 }
+
 .service-request p {
   font-size: 1em;
   line-height: 18px;
 }
+
 .service-request .panel {
   background: transparent;
   border: none;
   box-shadow: 0 0 0 0;
 }
+
 .service-request .whitesmoke {
   padding: 0 0 20px 0;
   background-color: transparent;
   border-right: 1px solid #e3e3e3;
   border-left: none;
   border-top: none;
   border-bottom: none;
   border-radius: 0;
   -webkit-box-shadow: 0 0 0 0;
   box-shadow: 0 0 0 0;
   font-size: 0.9em;
 }
+
 .service-request .icon-1x {
   font-size: 1.0em !important;
 }
+
 .service-request .icon-plus {
   margin: -1px 0 2px -2px !important;
 }
+
 .no-style {
   background: transparent;
   border: 0;
 }
+
 .icon-calendar:before {
   content: "\e602";
 }
+
 .icon-right:before {
   content: "\f105";
 }
+
 .icon-left:before {
   content: "\f104";
 }
+
 .details {
   margin: -4px auto -14px auto;
   display: table;
   width: 65%;
   font-weight: bold;
   font-family: 'TabletGothic', 'Colaborate', Arial, sans-serif;
   font-size: 16px;
   letter-spacing: 0.02em;
 }
+
 .btn-default:hover,
 .btn-default:focus,
 .btn-default.focus,
 .btn-default:active,
 .btn-default.active,
-.open > .dropdown-toggle.btn-default {
+.open>.dropdown-toggle.btn-default {
   color: #333;
   background-color: #e6e6e6;
   border-color: #D4D3D3;
   outline: none;
 }
+
 .btn:focus,
 .btn:active:focus,
 .btn.active:focus,
 .btn.focus,
 .btn:active.focus,
 .btn.active.focus {
   outline: none;
 }
+
 .service-request input.error {
   border: 2px solid rgba(220, 78, 27, 0.71);
 }
+
 .service-request input.error:focus {
   border: 1px solid #66afe9;
 }
+
 .last-saved {
   margin: -6px 6px 4px 0;
   font-size: 0.9em;
   font-style: oblique;
   width: 100%;
   text-align: right;
 }
+
 .last-saved.attachments {
   text-align: left;
   border-bottom: 1px solid #E0E0E0;
   padding: 0 0 10px 0;
   margin: 0 0 10px 0;
   font-style: normal;
 }
+
 .numtitle {
   background-color: whitesmoke;
   padding: 7px 12px;
   border-radius: 30px;
   font-size: 15px;
   font-weight: bold;
   line-height: 20px;
 }
+
 .numtitle.current {
   background-color: #2FB5B0;
   color: #fff;
 }
+
 .guided-search .well .label-default.gray {
   font-size: 12px;
   line-height: 1;
   list-style: none;
   padding: 4px 6px 4px 6px;
   font-weight: normal;
   text-decoration: none;
   white-space: nowrap;
   color: #777777;
   border: 1px solid #DCDCDC;
   background: rgba(0, 0, 0, 0.08) !important;
 }
+
 .guided-search .well .label-default.gray:hover {
   background: rgba(0, 0, 0, 0.14) !important;
 }
+
 ul#qkview li {
   list-style: none;
   margin: 0;
   padding: 0;
 }
+
 ul#qkview li label {
   font-weight: 400 !important;
   font-size: 0.9em;
   margin: 0 0 4px 6px;
 }
+
 .ttl-in-createSR {
   font-size: 90%;
   margin-top: 16px !important;
 }
+
 .service-request .form-group p {
   margin: 3px 0 0 0;
 }
+
 .service-request .open {
   background-color: green;
 }
+
 .request-change {
   margin: 0 16px;
   font-size: 0.96em;
 }
+
 .service-request.view .whatwhere {
   margin-top: -3px !important;
 }
+
 .guided-search .search-summary {
   display: inline-block;
   font-weight: bold;
   padding-left: 15px;
   padding-right: 15px;
 }
+
 @media (min-width: 1000px) {
   .rma-steps {
     width: 62%;
   }
 }
+
 .drop-container .drop-instructions {
   margin-top: 15px;
   margin-bottom: 20px;
 }
+
 .drop-container .drop-frame {
   border: 1px solid #fff;
   box-sizing: border-box;
   min-height: 600px;
   width: 100%;
 }
+
 .rma-pool-report {
   margin-top: 20px;
 }
+
 .rma-pool-report .rma-pool-header {
   margin-bottom: 15px;
 }
+
 ul.temporaryServiceRequests {
   margin: 0;
   list-style-position: outside;
   list-style: none;
   padding: 0;
   font-size: 13px;
 }
+
 .account-maintenance .user-card {
   border: solid thin #424242;
   border-radius: 2px;
   margin: 2px;
   display: block;
 }
+
 .account-maintenance .user-card h3,
 .account-maintenance .user-card address {
   padding: 8px;
 }
+
 .account-maintenance .user-card address,
 .account-maintenance .user-card dl {
   margin: 0;
 }
+
 .account-maintenance .user-card .button-container {
   text-align: right;
 }
+
 .account-maintenance .edit-user-profile-button {
   display: inline-block;
   width: 25%;
   margin: 0;
   border: none;
   background-color: #ffffff;
   font-size: large;
   border-top: thin #E0E0E0 solid;
   border-left: thin #E0E0E0 solid;
   padding-top: 8px;
   padding-bottom: 8px;
 }
+
 .account-maintenance .expand-user-card-button {
   border-right: solid thin #E0E0E0;
 }
+
 .account-maintenance h2 {
   float: none;
 }
+
 .account-maintenance .search-form {
   padding-top: .5em;
 }
+
 .account-maintenance .page-selector {
   padding-top: .5em;
 }
+
 .account-maintenance .card-list {
   list-style: none;
   margin: 0;
   padding: 0;
 }
+
 .account-maintenance .card-list .open-card {
   height: auto;
 }
+
 .account-maintenance .card-list .open-card .card-button {
   border-bottom: solid thin black;
 }
+
 .account-maintenance .card-list li {
   border: solid thin black;
   padding-left: 1em;
   display: block;
   height: 3em;
   line-height: 3em;
   margin-top: .5em;
 }
+
 .account-maintenance .card-list li .card-button {
   margin: 0;
   background-color: #ffffff;
   border: none;
   height: 100%;
   border-left: solid thin #000000;
   width: 4em;
 }
+
 .account-maintenance .card-list li .card-button .glyphicon {
   margin: 0;
 }
+
 .account-maintenance .card-list li .card-link {
   margin-right: 1em;
 }
+
 .user-profile .search-form {
   padding-top: 8px;
 }
+
 .user-profile .card-list {
   list-style: none;
   margin: 0;
   padding: 0;
 }
+
 .user-profile .card-list .open-card {
   height: auto;
 }
+
 .user-profile .card-list .open-card .card-button {
   border-bottom: solid thin black;
 }
+
 .user-profile .card-list li {
   border: solid thin black;
   padding-left: 1em;
   display: block;
   height: 3em;
   line-height: 3em;
   margin-top: .5em;
 }
+
 .user-profile .card-list li .card-button {
   margin: 0;
   background-color: #ffffff;
   border: none;
   height: 100%;
   border-left: solid thin #000000;
   width: 4em;
 }
+
 .user-profile .card-list li .card-button .glyphicon {
   margin: 0;
 }
+
 .user-profile .card-list li .card-link {
   margin-right: 1em;
 }
+
 .btn-group.customize .btn {
   padding: 4px 6px;
   margin: 0 6px 4px 0;
   font-weight: normal;
   text-decoration: none;
   white-space: nowrap;
   color: #777;
@@ -4594,22 +5508,25 @@
   background: rgba(0, 0, 0, 0.08);
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
   font-size: 12px;
   line-height: 1;
 }
+
 .btn-group.customize .btn:hover {
   color: #555;
   border-color: #bbb;
   background-color: rgba(0, 0, 0, 0.1);
 }
+
 .btn-default {
   border-color: #E2E2E2;
 }
+
 .label-default {
   font-size: 12px;
   line-height: 1;
   list-style: none;
   padding: 4px 6px 4px 6px;
   font-weight: normal;
   text-decoration: none;
@@ -4617,33 +5534,38 @@
   color: #777;
   border: 1px solid #ccc;
   background: rgba(0, 0, 0, 0.08);
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
 }
+
 .no-style {
   background: transparent;
   border: 0;
 }
+
 .label-default:hover {
   color: #555;
   border-color: #bbb;
   background-color: rgba(0, 0, 0, 0.1);
   cursor: pointer;
 }
+
 a.label-default:hover {
   text-decoration: none;
   color: #555;
   border-color: #bbb;
   background-color: rgba(0, 0, 0, 0.1) !important;
 }
+
 h4 .label-default {
   font-family: Arial, Helvetica, sans-serif;
 }
+
 .container-fluid.well .label-default {
   font-size: 14px;
   line-height: 1;
   list-style: none;
   padding: 8px 6px 8px 6px;
   margin-right: 10px;
   font-weight: normal;
@@ -4652,270 +5574,329 @@
   color: #777;
   border: 1px solid #ccc;
   background: white;
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
 }
+
 .container-fluid.well .label-default:hover {
   text-decoration: none;
   color: black;
   border-color: #bbb;
   background-color: white !important;
 }
+
 .btn.dropdown-toggle {
   border: 1px solid rgba(163, 160, 160, 0.3);
   background-color: white;
 }
+
 .content-fluid {
   width: 100%;
+  text-align: center;
+  margin-top: 30px;
 }
+
 .container-fluid.well {
   margin-left: 15px;
   margin-right: 15px;
 }
+
 .search-wrapper .container-fluid.well {
   margin-left: 26px;
 }
+
 .guided-search .container-fluid.well {
   margin-left: 0;
 }
+
 /* ----------------------------
 media styles
 --------------------------- */
 @media (max-width: 1000px) {
   #MainMenu {
     display: none;
   }
+
   a.mysupport {
     margin: 12px 16px 0 0;
   }
+
   .topLinks {
     margin: -32px 14px 0 0;
   }
+
   .searchwrapper {
     float: right;
     margin: -30px -10px 0 10px;
   }
+
   .search {
     width: 90%;
   }
+
   form.search input.support-guided {
     width: 68%;
   }
 }
+
 @media (min-width: 1001px) {
+
   .sidebar-toggle,
   .sidebar {
     display: none;
   }
+
   .archived input {
     margin: 0 4px 0 -14px;
     line-height: 20px;
   }
 }
+
 @media (min-width: 992px) {
   .col-md-10.middlecontent {
     width: 80%;
     margin: 35px 15px 0 0;
   }
 }
+
 @media (max-width: 768px) {
   .block {
     width: 94%;
     padding: 10px 2% 30px 4%;
     float: left;
     position: relative;
     display: table-cell;
     border-bottom: 1px solid white;
     margin-left: 3%;
   }
+
   .blocks-container .block:last-of-type {
     padding: 10px 2% 30px 4%;
     width: 94%;
     margin-left: 3%;
   }
+
   .block:after {
     content: "";
     background: none;
   }
+
   .blocks-container {
     padding: 0;
   }
+
   .ihealth-popover .popover.left {
     margin-left: 270px;
     margin-top: -70px;
   }
-  .ihealth-popover .popover.left > .arrow {
+
+  .ihealth-popover .popover.left>.arrow {
     bottom: -11px;
     left: 20%;
     margin-left: -11px;
     border-top-color: #999;
     border-top-color: rgba(0, 0, 0, 0.25);
     border-bottom-width: 0;
   }
-  .ihealth-popover .popover.left > .arrow:after {
+
+  .ihealth-popover .popover.left>.arrow:after {
     bottom: 1px;
     margin-left: -10px;
     content: " ";
     border-top-color: white;
     border-bottom-width: 0;
   }
 }
+
 @media (max-width: 520px) {
   img.logo.support {
     margin: 20px 0 0 10px;
     max-width: 108px;
   }
+
   #upc-search {
     color: white;
     background-color: #A3A5B0;
     padding: 6px;
   }
+
   .searchwrapper {
     float: right;
     margin: -30px -10px 0 10px;
   }
+
   .topLinks {
     margin: 0;
   }
+
   .nobanner .topLinks,
   .nobanner .topLinks a {
     color: #337ab7;
   }
+
   form.search input.support-guided {
     width: 62%;
   }
+
   .search {
     width: 100%;
     padding: 0 2px;
   }
+
   .corp-menu ul li a {
     font-size: 8px !important;
   }
+
   .pageHeader {
     height: 110px;
   }
+
   /* Shows summary text of entries in the service request activity log properly in smaller viewports */
   .activity-title {
     max-width: 80%;
   }
 }
+
 @media (max-width: 430px) {
   .corp-menu ul li {
     margin: 10px 0 0 4px;
     font-size: 90%;
   }
+
   .row.corp-header .corp-menu li:before {
     padding-right: 3px;
   }
+
   .btn-primary {
     padding: 8px 22px;
   }
+
   .well {
     padding: 10px 0;
   }
 }
+
 /* My Support page */
 .table-bordered {
   background-color: white;
 }
+
 /* Create SR*/
 .no-style:active,
 .no-style:focus {
   outline: none;
   border: 0;
 }
+
 /* The only new style for the FAQ page: */
 .faq h3 {
   font-size: 17px;
 }
+
 .rsssettings {
   margin-top: 10px;
 }
+
 .rss-link {
   font-size: 70%;
   background: transparent url('https://cdn.f5.com/websites/support/assets/images/icons/rss_icon_med.gif') no-repeat center left;
   padding: 1px 0 0 22px;
   margin: 0 0 0 14px;
 }
+
 /*feedback*/
 .feedback_content,
 .feedback_trigger {
   font-size: 16px;
   font-family: 'Helvetica Neue', Helvetica, Tahoma, Arial, sans-serif;
   -webkit-transition: all 500ms ease-in-out;
   -moz-transition: all 500ms ease-in-out;
   -o-transition: all 500ms ease-in-out;
   transition: all 500ms ease-in-out;
 }
+
 .feedback_content ul {
   list-style: none;
   padding-left: 11px;
 }
+
 .feedback_trigger {
   cursor: pointer;
   -webkit-border-top-left-radius: 0;
   -moz-border-radius-topleft: 0;
   border-top-left-radius: 0;
   -webkit-border-bottom-left-radius: 0;
   -moz-border-radius-bottomleft: 0;
   border-bottom-left-radius: 0;
   z-index: 2001;
 }
+
 .feedback_trigger.left-top,
 .feedback_trigger.left-bottom,
 .feedback_trigger.right-top,
 .feedback_trigger.right-bottom {
   width: 40px;
   height: 100px;
 }
+
 .feedback_trigger.bottom-left {
   width: 100px;
   height: 40px;
 }
+
 .feedback_content {
   width: 380px;
   height: 300px;
   z-index: 2001;
 }
+
 .feedback_content.email_present {
   height: 360px;
 }
+
 .feedback_content ul li {
   margin-right: 20px;
   margin-bottom: 10px;
 }
+
 .feedback_content label {
   display: inline-block;
   font-size: 12px;
 }
+
 .feedback_name {
   display: block;
   width: 340px;
 }
+
 .feedback_email {
   display: block;
   width: 340px;
 }
+
 .feedback_message {
   display: block;
   width: 340px;
   resize: none;
 }
+
 .feedback_submit {
   float: right;
 }
+
 .feedback_trigger_text {
   white-space: nowrap;
   position: absolute;
   top: 40px;
   letter-spacing: 2px;
   font-size: 17px;
 }
+
 .left-top .feedback_trigger_text,
 .left-bottom .feedback_trigger_text,
 .right-top .feedback_trigger_text,
 .right-bottom .feedback_trigger_text {
   white-space: nowrap;
   position: absolute;
   top: 40px;
@@ -4923,20 +5904,23 @@
   font-size: 17px;
   -webkit-transform: rotate(-90deg);
   -moz-transform: rotate(-90deg);
   -ms-transform: rotate(-90deg);
   -o-transform: rotate(-90deg);
   filter: none;
 }
+
 .fm_clean {
   background-color: #DDDDDD;
 }
+
 .fm_clean.feedback_trigger:hover {
   background-color: #CCCCCC;
 }
+
 .fm_clean button {
   padding: 4px 14px;
   display: inline;
   background: #2FB5B0;
   border: none;
   color: white;
   cursor: pointer;
@@ -4944,75 +5928,87 @@
   -webkit-border-radius: 4px;
   -moz-border-radius: 4px;
   border-radius: 4px;
   /*text-shadow: 1px 1px #666;*/
   font-size: 13px;
   margin-right: 10px;
 }
+
 .fm_clean button:hover {
   background-color: #9C9A9A;
 }
+
 .fm_clean .feedback_trigger_text {
   right: -25px;
   letter-spacing: 1px;
 }
+
 .fm_clean .feedback_title {
   padding-top: 5px;
 }
+
 .fm_clean .feedback_title span {
   /*margin: 10px;
     font-size: 14px;*/
   font-weight: bold;
   font-size: 13px;
   margin: 10px 0 10px 14px;
   float: left;
   width: 100%;
 }
+
 .feedback_content.fm_clean.feedback_content_closed.left-top,
 .feedback_content.fm_clean.feedback_content_closed.left-bottom {
   margin-left: -380px;
 }
+
 .feedback_content.fm_clean.left-top,
 .feedback_content.fm_clean.left-bottom {
   margin-left: 0;
   -webkit-border-top-right-radius: 6px;
   -moz-border-radius-topright: 6px;
   border-top-right-radius: 6px;
   -webkit-border-bottom-right-radius: 6px;
   -moz-border-radius-bottomright: 6px;
   border-bottom-right-radius: 6px;
   color: #333;
 }
+
 .feedback_trigger.fm_clean.feedback_trigger_closed.left-top,
 .feedback_trigger.fm_clean.feedback_trigger_closed.left-bottom {
   margin-left: 0;
 }
+
 .feedback_trigger.fm_clean.left-top,
 .feedback_trigger.fm_clean.left-bottom {
   margin-left: 380px;
   -webkit-border-top-right-radius: 6px;
   -moz-border-radius-topright: 6px;
   border-top-right-radius: 6px;
   -webkit-border-bottom-right-radius: 6px;
   -moz-border-radius-bottomright: 6px;
   border-bottom-right-radius: 6px;
   color: #333;
 }
+
 .feedback_content.fm_jquery.feedback_content_closed.left-top,
 .feedback_content.fm_jquery.feedback_content_closed.left-bottom {
   margin-left: -382px;
 }
+
 .feedback_content.fm_jquery.left-top,
 .feedback_content.fm_jquery.left-bottom {
   margin-left: 0;
 }
+
 .feedback_trigger.fm_jquery.feedback_trigger_closed.left-top,
 .feedback_trigger.fm_jquery.feedback_trigger_closed.left-bottom {
   margin-left: 0;
 }
+
 .feedback_trigger.fm_jquery.left-top,
 .feedback_trigger.fm_jquery.left-bottom {
   margin-left: 382px;
   -webkit-border-top-left-radius: 6px;
   -moz-border-radius-topleft: 6px;
   border-top-left-radius: 6px;
   -webkit-border-bottom-left-radius: 6px;
@@ -5021,187 +6017,232 @@
   -webkit-border-top-right-radius: 6px;
   -moz-border-radius-topright: 6px;
   border-top-right-radius: 6px;
   -webkit-border-bottom-right-radius: 6px;
   -moz-border-radius-bottomright: 6px;
   border-bottom-right-radius: 6px;
 }
+
 .fm_jquery .feedback_trigger_text {
   right: -20px;
 }
+
 .fm_jquery.feedback_content {
   padding: 0;
   width: 380px;
   height: 340px;
 }
+
 .fm_jquery.feedback_content.email_present {
   height: 390px;
 }
+
 .fm_jquery.feedback_trigger {
   padding: 0;
   border: 0;
 }
+
 .feedback_content.fm_bootstrap.feedback_content_closed.left-top,
 .feedback_content.fm_bootstrap.feedback_content_closed.left-bottom {
   margin-left: -380px;
 }
+
 .feedback_content.fm_bootstrap.left-top,
 .feedback_content.fm_bootstrap.left-bottom {
   margin-left: 0;
 }
+
 .feedback_trigger.fm_bootstrap.feedback_trigger_closed.left-top,
 .feedback_trigger.fm_bootstrap.feedback_trigger_closed.left-bottom {
   margin-left: 0;
 }
+
 .feedback_trigger.fm_bootstrap.left-top,
 .feedback_trigger.fm_bootstrap.left-bottom {
   margin-left: 380px;
 }
+
 .fm_bootstrap .feedback_trigger_text {
   right: -25px;
 }
+
 .fm_bootstrap.hero-unit {
   padding: 0px;
 }
+
 .fm_bootstrap.hero-unit ul {
   margin-left: 15px;
 }
+
 .fm_bootstrap .feedback_title {
   margin-bottom: 10px;
 }
+
 .fm_bootstrap .feedback_title span {
   margin-left: 15px;
 }
+
 .fm_bootstrap .feedback_trigger_text {
   top: 35px;
 }
+
 .fm_bootstrap.feedback_content ul {
   padding: 0;
 }
+
 .fm_bootstrap.feedback_content {
   height: 340px;
 }
+
 .fm_bootstrap.feedback_content.email_present {
   height: 430px;
 }
+
 .fm_bootstrap.feedback_trigger:hover {
   background-color: #AAAAAA;
 }
+
 .required_asterisk {
   color: red;
 }
+
 .feedback_content.radio_button_list_present {
   height: 380px;
 }
+
 .feedback_content.email_present.radio_button_list_present {
   height: 440px;
 }
+
 .radio_button_wrapper {
   display: inline-block;
   text-align: center;
   margin-right: 35px;
 }
+
 .feedback_content .radio_button_wrapper label {
   display: block;
 }
+
 .radio_button_list_title_wrapper {
   margin-bottom: 10px;
 }
+
 .fm_jquery.feedback_content.radio_button_list_present {
   height: 430px;
 }
+
 .fm_bootstrap.feedback_content.radio_button_list_present {
   height: 470px;
 }
+
 .fm_jquery.feedback_content.email_present.radio_button_list_present {
   height: 500px;
 }
+
 .fm_bootstrap.feedback_content.email_present.radio_button_list_present {
   height: 550px;
 }
+
 @media screen {
+
   .fm_clean .feedback_trigger_text,
   .fm_jquery .feedback_trigger_text,
   .fm_bootstrap .feedback_trigger_text {
     right: -70px;
     width: 100px;
     margin-top: -45px;
     filter: progid:DXImageTransform.Microsoft.Matrix(M11=0, M12=1, M21=-1, M22=0, sizingMethod='auto expand');
   }
+
   .fm_bootstrap .feedback_trigger_text {
     right: -65px;
     margin-top: -40px;
   }
 }
+
 .feedback_trigger.left-top {
   position: fixed;
   top: 100px;
   left: 0;
 }
+
 .feedback_content.left-top {
   position: fixed;
   top: 50px;
   left: 0;
 }
+
 .feedback_trigger.left-bottom {
   position: fixed;
   bottom: 100px;
   left: 0;
 }
+
 .feedback_content.left-bottom {
   position: fixed;
   bottom: 50px;
   left: 0;
 }
+
 .feedback_trigger.right-top {
   position: fixed;
   top: 100px;
   right: 0;
 }
+
 .feedback_content.right-top {
   position: fixed;
   top: 50px;
   right: 0;
 }
+
 .feedback_trigger.right-bottom {
   position: fixed;
   bottom: 100px;
   right: 0;
 }
+
 .feedback_content.right-bottom {
   position: fixed;
   bottom: 50px;
   right: 0;
 }
+
 .feedback_content.fm_clean.feedback_content_closed.right-top,
 .feedback_content.fm_clean.feedback_content_closed.right-bottom {
   margin-right: -380px;
 }
+
 .feedback_content.fm_clean.right-top,
 .feedback_content.fm_clean.right-bottom {
   margin-right: 0;
   -webkit-border-top-left-radius: 6px;
   -moz-border-radius-topleft: 6px;
   border-top-left-radius: 6px;
   -webkit-border-bottom-left-radius: 6px;
   -moz-border-radius-bottomleft: 6px;
   border-bottom-left-radius: 6px;
 }
+
 .feedback_content.fm_jquery.feedback_content_closed.right-top,
 .feedback_content.fm_jquery.feedback_content_closed.right-bottom {
   margin-right: -382px;
 }
+
 .feedback_content.fm_jquery.right-top,
 .feedback_content.fm_jquery.right-bottom {
   margin-right: 0;
 }
+
 .feedback_content.fm_bootstrap.feedback_content_closed.right-top,
 .feedback_content.fm_bootstrap.feedback_content_closed.right-bottom {
   margin-right: -380px;
 }
+
 .feedback_content.fm_bootstrap.right-top,
 .feedback_content.fm_bootstrap.right-bottom {
   margin-right: 0;
   -webkit-border-top-left-radius: 6px;
   -moz-border-radius-topleft: 6px;
   border-top-left-radius: 6px;
   -webkit-border-bottom-left-radius: 6px;
@@ -5210,32 +6251,36 @@
   -webkit-border-top-right-radius: 0;
   -moz-border-radius-topright: 0;
   border-top-right-radius: 0;
   -webkit-border-bottom-right-radius: 0;
   -moz-border-radius-bottomright: 0;
   border-bottom-right-radius: 0;
 }
+
 .feedback_trigger.fm_clean.feedback_trigger_closed.right-top,
 .feedback_trigger.fm_clean.feedback_trigger_closed.right-bottom {
   margin-right: 0;
 }
+
 .feedback_trigger.fm_clean.right-top,
 .feedback_trigger.fm_clean.right-bottom {
   margin-right: 380px;
   -webkit-border-top-left-radius: 6px;
   -moz-border-radius-topleft: 6px;
   border-top-left-radius: 6px;
   -webkit-border-bottom-left-radius: 6px;
   -moz-border-radius-bottomleft: 6px;
   border-bottom-left-radius: 6px;
 }
+
 .feedback_trigger.fm_jquery.feedback_trigger_closed.right-top,
 .feedback_trigger.fm_jquery.feedback_trigger_closed.right-bottom {
   margin-right: 0;
 }
+
 .feedback_trigger.fm_jquery.right-top,
 .feedback_trigger.fm_jquery.right-bottom {
   margin-right: 382px;
   -webkit-border-top-right-radius: 0;
   -moz-border-radius-topright: 0;
   border-top-right-radius: 0;
   -webkit-border-bottom-right-radius: 0;
@@ -5244,18 +6289,20 @@
   -webkit-border-top-left-radius: 6px;
   -moz-border-radius-topleft: 6px;
   border-top-left-radius: 6px;
   -webkit-border-bottom-left-radius: 6px;
   -moz-border-radius-bottomleft: 6px;
   border-bottom-left-radius: 6px;
 }
+
 .feedback_trigger.fm_bootstrap.feedback_trigger_closed.right-top,
 .feedback_trigger.fm_bootstrap.feedback_trigger_closed.right-bottom {
   margin-right: 0;
 }
+
 .feedback_trigger.fm_bootstrap.right-top,
 .feedback_trigger.fm_bootstrap.right-bottom {
   margin-right: 380px;
   -webkit-border-top-left-radius: 6px;
   -moz-border-radius-topleft: 6px;
   border-top-left-radius: 6px;
   -webkit-border-bottom-left-radius: 6px;
@@ -5264,47 +6311,53 @@
   -webkit-border-top-right-radius: 0;
   -moz-border-radius-topright: 0;
   border-top-right-radius: 0;
   -webkit-border-bottom-right-radius: 0;
   -moz-border-radius-bottomright: 0;
   border-bottom-right-radius: 0;
 }
+
 .feedback_me_frame {
   border: none;
   overflow: auto;
   height: 90%;
   width: 98%;
 }
+
 .feedback-delayed-dlg {
   position: fixed;
   width: 250px;
   height: 100px;
   top: 50%;
   left: 50%;
   vertical-align: middle;
   text-align: center;
   margin-left: -125px;
   margin-top: -50px;
   -webkit-border-radius: 6px;
   -moz-border-radius: 6px;
   border-radius: 6px;
 }
+
 .feedback-delayed-dlg.success {
   background-color: #2ECC40;
 }
+
 .feedback-delayed-dlg.fail {
   background-color: #FF4136;
 }
+
 .feedback-dlg-close {
   position: absolute;
   right: 0;
   padding: 1px;
   background: white;
   cursor: pointer;
 }
+
 .feedback-sucess-fail-message-inner {
   position: fixed;
   width: 200px;
   height: 50px;
   background-color: white;
   top: 50%;
   left: 50%;
@@ -5313,258 +6366,306 @@
   margin-left: -100px;
   margin-top: -25px;
   -webkit-border-radius: 6px;
   -moz-border-radius: 6px;
   border-radius: 6px;
   line-height: 50px;
 }
-.feedback-sucess-fail-message-inner > span {
+
+.feedback-sucess-fail-message-inner>span {
   display: inline-block;
   vertical-align: middle;
   line-height: 1em;
 }
+
 .feedback-sucess-message,
 .feedback-fail-message {
   display: inline-block;
   width: 200px;
   height: 50px;
 }
+
 .fdbk-title {
   font-weight: bold;
   font-size: 13px;
   margin: 10px 0 10px 14px;
   float: left;
   width: 100%;
 }
+
 p.feedback-msg {
   padding: 2px 0 10px 0;
   font-size: 14px;
 }
+
 .knowledge-centers {
   position: relative;
 }
+
 .knowledge-centers ul.platform-name {
   margin-left: 20px;
 }
+
 .knowledge-centers.productInfo ul {
   font-size: 14px;
 }
+
 .knowledge-centers ul {
   margin: 0;
   list-style: none outside;
   padding: 0;
   font-size: 13px;
 }
+
 .knowledge-centers ul li {
   line-height: 20px !important;
 }
+
 .knowledge-centers ul li .icon-1x {
   margin: 0 2px 0 -2px !important;
 }
+
 .knowledge-centers div.slideable {
   margin: 0 0 0 18px;
   padding: 0;
 }
+
 .knowledge-centers div.slideable .slideable_content {
   line-height: 22px;
   padding: 1px 0 2px 0 !important;
 }
+
 .knowledge-centers.home ul {
   font-size: 15px;
   font-family: 'TabletGothic', 'Colaborate', Arial, sans-serif;
   font-weight: 500;
 }
+
 .knowledge-centers h3 {
   border-bottom: 3px solid #ddd;
   padding: 2px 0 14px 0;
   margin: 30px 5px 16px 0;
 }
+
 .knowledge-centers h4 {
   font-family: 'TabletGothicSemiBold', 'Colaborate', Arial, sans-serif;
   font-size: 16px;
   float: none;
 }
+
 .knowledge-centers h5 {
   font-size: 14px;
   min-height: 30px;
 }
+
 .knowledge-centers h5.no-bold {
   font-weight: normal;
 }
+
 .knowledge-centers h5.more-info {
   margin-top: 18px;
   margin-left: 8px;
   font-size: 1.1em;
 }
+
 .knowledge-centers .result-attribute {
   font-size: 94%;
   color: #999;
 }
+
 .knowledge-centers product-items,
 .knowledge-centers platform-items {
   display: table;
 }
+
 img.responsive {
   width: 100%;
   max-width: 380px;
 }
+
 img.responsive.cloud-img-logo {
   width: 100%;
   max-width: 240px;
   padding: 24px 10px;
   margin: 0 auto;
   display: table;
 }
+
 .relatedPlatforms {
   margin-bottom: 15px;
 }
+
 #allDownloadsLink {
   display: inline-block;
   margin-top: 10px;
 }
+
 .artid-bold {
   font-weight: bold;
 }
+
 .italic {
   font-style: italic;
 }
+
 .clear-left {
   clear: left;
 }
+
 .icon-1x.btn {
   font-size: 21px;
   margin: -2px 0 2px 0;
   padding: 0;
 }
+
 .animate-show {
   line-height: 20px;
   border: 1px solid white;
   opacity: 1;
   background: white;
 }
+
 .animate-show.ng-hide,
 .animate-show.ng-hide-add,
 .animate-show.ng-hide-remove {
   -webkit-transition: all linear 0.5s;
   -moz-transition: all linear 0.5s;
   -o-transition: all linear 0.5s;
   transition: all linear 0.5s;
 }
+
 .animate-show.ng-hide {
   line-height: 0;
   opacity: 1;
 }
+
 a.series-platforms {
   line-height: 20px;
 }
+
 ul.platform-name {
   margin-bottom: 5px;
 }
+
 .connect-message {
   margin: 10px 0;
   float: left;
   line-height: 20px !important;
 }
+
 #spinnerContainer .loading.fade {
   margin-top: inherit;
   width: 100%;
 }
+
 #spinnerContainer .loading {
   top: inherit;
 }
+
 #spinnerContainer div {
   -webkit-border-radius: 6px;
   -moz-border-radius: 6px;
   border-radius: 6px;
 }
+
 @media (max-width: 960px) {
   .steps {
     font-size: 0.8em;
   }
 }
+
 @media (max-width: 768px) {
   .steps {
     font-size: 0.8em;
     line-height: 14px !important;
     font-weight: bold;
     float: left;
     margin: 0 auto;
     display: table;
     padding: 14px 0;
   }
 }
+
 @media (max-width: 420px) {
   .steps {
     display: none;
   }
 }
+
 .icon-title {
   cursor: default;
 }
+
 .asteriskField {
   color: red;
   font-size: 1.2em;
 }
+
 label.normal-weight {
   font-weight: normal;
 }
+
 .disabled-link {
   cursor: default !important;
   text-decoration: none !important;
 }
+
 a.no-decoration:link,
 a.no-decoration:visited,
 a.no-decoration:focus,
 a.no-decoration:hover,
 a.no-decoration:active {
   text-decoration: none;
 }
+
 .hide-me {
   display: none;
 }
+
 .tooltip-inner {
   padding: 9px 18px;
   color: white;
   background-color: #4C4E52;
 }
+
 .tooltip.bottom .tooltip-arrow,
 .tooltip.top .tooltip-arrow {
   border-top-color: #4C4E52;
   border-bottom-color: #4C4E52;
 }
 
 @font-face {
-    font-family: Proxima;
-    font-weight: 400;
-    font-style: normal;
-    src: url(/assets/fonts/ProximaMedium.woff2) format('woff2'), url(/assets/fonts/ProximaMedium.woff) format('woff')
+  font-family: Proxima;
+  font-weight: 400;
+  font-style: normal;
+  src: url(/assets/fonts/ProximaMedium.woff2) format('woff2'), url(/assets/fonts/ProximaMedium.woff) format('woff')
 }
 
 @font-face {
-    font-family: Proxima;
-    font-weight: 700;
-    font-style: normal;
-    src: url(/assets/fonts/ProximaBold.woff2) format('woff2'), url(/assets/fonts/ProximaBold.woff) format('woff')
+  font-family: Proxima;
+  font-weight: 700;
+  font-style: normal;
+  src: url(/assets/fonts/ProximaBold.woff2) format('woff2'), url(/assets/fonts/ProximaBold.woff) format('woff')
 }
 
 @font-face {
-    font-family: Proxima;
-    font-weight: 100;
-    font-style: normal;
-    src: url(/assets/fonts/ProximaThin.woff2) format('woff2'), url(/assets/fonts/ProximaThin.woff) format('woff')
+  font-family: Proxima;
+  font-weight: 100;
+  font-style: normal;
+  src: url(/assets/fonts/ProximaThin.woff2) format('woff2'), url(/assets/fonts/ProximaThin.woff) format('woff')
 }
 
 body {
-    font-family: Proxima,-apple-system,BlinkMacSystemFont,"Segoe UI",Roboto,sans-serif,"Apple Color Emoji","Segoe UI Emoji","Segoe UI Symbol";
-    font-size: 16px;
-    font-weight: 400;
-    line-height: 1.375;
-    color: #4D4F53;
-    background-color: #FFF;
-    position: relative
+  font-family: Proxima, -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
+  font-size: 16px;
+  font-weight: 400;
+  line-height: 1.375;
+  color: #4D4F53;
+  background-color: #FFF;
+  position: relative
 }
 
 /* Start of Coveo search bar in header */
 
 #search-toggle {
   color: #fff;
   background-color: #6a6c73;
@@ -5604,21 +6705,21 @@
   padding-left: 15px;
   margin-right: auto;
   margin-left: auto;
 }
 
 @media (max-width: 1200px) {
   #search-container .container {
-      width: 100%;
+    width: 100%;
   }
 }
 
 @media (min-width: 1200px) {
   #search-container .container {
-      width: 1280px !important;
+    width: 1280px !important;
   }
 }
 
 #search-container #blue-banner {
   position: relative;
 }
 
@@ -5657,38 +6758,43 @@
 }
 
 #search-container .CoveoSearchbox .magic-box .magic-box-input>input {
   font-size: 14px;
 }
 
 #search-container .CoveoSearchbox .magic-box {
-    border: thin solid #bcc3ca;
-    border-radius: 2px;
+  border: thin solid #bcc3ca;
+  border-radius: 2px;
+}
+
+.magic-box .magic-box-clear {
+  height: 38px !important;
+  line-height: 38px !important;
 }
 
 #search-container .search-tips {
   display: block;
   position: absolute;
   top: 24px;
   left: 1020px;
   width: 90px;
 }
 
 #search-container .search-tips a {
-  color: #fff!important;
-  font-size: .9em!important;
+  color: #fff !important;
+  font-size: .9em !important;
   line-height: 18px;
-  text-decoration: none!important;
+  text-decoration: none !important;
 
 }
 
 @media screen and (max-width: 1160px) {
   #search-container .search-tips {
-      position: inherit;
-      top: inherit;
-      left: inherit;
-      margin: auto;
-      padding-bottom: 10px;
+    position: inherit;
+    top: inherit;
+    left: inherit;
+    margin: auto;
+    padding-bottom: 10px;
   }
 }
 
 /* End of Coveo search bar in header */
```

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaBold.woff` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaBold.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaBold.woff2` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaBold.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaMedium.woff2` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaMedium.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaThin.woff` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaThin.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/ProximaThin.woff2` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/ProximaThin.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/CoveoJsSearch.Lazy.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/bootstrap.js` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/bootstrap.min.js` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/clouddocs.js` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/clouddocs.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/feedback.js` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/feedback.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/jquery.appear.js` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/jquery.appear.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme/static/js/printThis.js` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme/static/js/printThis.js`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/PKG-INFO` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f5-sphinx-theme
-Version: 2.5.0
+Version: 2.5.2
 Summary: Sphinx theme for F5 Networks
 Home-page: https://github.com/F5DevCentral/f5-sphinx-theme
 Author: F5 Networks
 Author-email: f5-sphinx-theme@f5.com
 License: Apache2
 Classifier: Framework :: Sphinx
 Classifier: Framework :: Sphinx :: Theme
```

### Comparing `f5_sphinx_theme-2.5.0/f5_sphinx_theme.egg-info/SOURCES.txt` & `f5_sphinx_theme-2.5.2/f5_sphinx_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `f5_sphinx_theme-2.5.0/setup.py` & `f5_sphinx_theme-2.5.2/setup.py`

 * *Files identical despite different names*
