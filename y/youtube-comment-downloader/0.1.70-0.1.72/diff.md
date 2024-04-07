# Comparing `tmp/youtube-comment-downloader-0.1.70.tar.gz` & `tmp/youtube-comment-downloader-0.1.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-comment-downloader-0.1.70.tar", last modified: Sat Sep  2 07:26:04 2023, max compression
+gzip compressed data, was "youtube-comment-downloader-0.1.72.tar", last modified: Sun Apr  7 18:58:51 2024, max compression
```

## Comparing `youtube-comment-downloader-0.1.70.tar` & `youtube-comment-downloader-0.1.72.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:26:04.485712 youtube-comment-downloader-0.1.70/
--rw-r--r--   0 runner    (1001) docker     (999)     1081 2023-09-02 07:25:54.000000 youtube-comment-downloader-0.1.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     2863 2023-09-02 07:26:04.485712 youtube-comment-downloader-0.1.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2324 2023-09-02 07:25:54.000000 youtube-comment-downloader-0.1.70/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       90 2023-09-02 07:25:54.000000 youtube-comment-downloader-0.1.70/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)      802 2023-09-02 07:26:04.485712 youtube-comment-downloader-0.1.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-09-02 07:25:54.000000 youtube-comment-downloader-0.1.70/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:26:04.485712 youtube-comment-downloader-0.1.70/youtube_comment_downloader/
--rw-r--r--   0 runner    (1001) docker     (999)     3615 2023-09-02 07:25:54.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      291 2023-09-02 07:25:54.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (999)     7163 2023-09-02 07:25:54.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader/downloader.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-09-02 07:26:04.485712 youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2863 2023-09-02 07:26:04.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      472 2023-09-02 07:26:04.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-09-02 07:26:04.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       79 2023-09-02 07:26:04.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       20 2023-09-02 07:26:04.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       27 2023-09-02 07:26:04.000000 youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/tests/test_search_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/youtube_comment_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7475 2024-04-07 18:58:44.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader/downloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:58:51.895699 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 18:58:51.000000 youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/top_level.txt
```

### Comparing `youtube-comment-downloader-0.1.70/LICENSE` & `youtube-comment-downloader-0.1.72/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube-comment-downloader-0.1.70/PKG-INFO` & `youtube-comment-downloader-0.1.72/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: youtube-comment-downloader
-Version: 0.1.70
+Version: 0.1.72
 Summary: Simple script for downloading Youtube comments without using the Youtube API
 Home-page: https://github.com/egbertbouman/youtube-comment-downloader
 Author: Egbert Bouman
 Author-email: ebouman@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dateparser
+Requires-Dist: requests
 
 # youtube-comment-downloader
 Simple script for downloading Youtube comments without using the Youtube API. The output is in line delimited JSON.
 
 ### Installation
 
 Preferably inside a [python virtual environment](https://virtualenv.pypa.io/en/latest/) install this package via:
```

### Comparing `youtube-comment-downloader-0.1.70/README.md` & `youtube-comment-downloader-0.1.72/README.md`

 * *Files identical despite different names*

### Comparing `youtube-comment-downloader-0.1.70/setup.cfg` & `youtube-comment-downloader-0.1.72/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = youtube-comment-downloader
-version = 0.1.70
+version = 0.1.72
 description = Simple script for downloading Youtube comments without using the Youtube API
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license-file = LICENSE
 url = https://github.com/egbertbouman/youtube-comment-downloader
 author = Egbert Bouman
```

### Comparing `youtube-comment-downloader-0.1.70/youtube_comment_downloader/__init__.py` & `youtube-comment-downloader-0.1.72/youtube_comment_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `youtube-comment-downloader-0.1.70/youtube_comment_downloader.egg-info/PKG-INFO` & `youtube-comment-downloader-0.1.72/youtube_comment_downloader.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: youtube-comment-downloader
-Version: 0.1.70
+Version: 0.1.72
 Summary: Simple script for downloading Youtube comments without using the Youtube API
 Home-page: https://github.com/egbertbouman/youtube-comment-downloader
 Author: Egbert Bouman
 Author-email: ebouman@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dateparser
+Requires-Dist: requests
 
 # youtube-comment-downloader
 Simple script for downloading Youtube comments without using the Youtube API. The output is in line delimited JSON.
 
 ### Installation
 
 Preferably inside a [python virtual environment](https://virtualenv.pypa.io/en/latest/) install this package via:
```

