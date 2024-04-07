# Comparing `tmp/syncMyMoodle-0.1.0.tar.gz` & `tmp/syncMyMoodle-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncMyMoodle-0.1.0.tar", last modified: Tue Mar 21 15:47:18 2023, max compression
+gzip compressed data, was "syncMyMoodle-0.1.1.tar", last modified: Sun Apr  7 11:19:24 2024, max compression
```

## Comparing `syncMyMoodle-0.1.0.tar` & `syncMyMoodle-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 septatrix  (1000) septatrix  (1000)        0 2023-03-21 15:47:18.452927 syncMyMoodle-0.1.0/
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)    35149 2021-07-18 20:20:06.000000 syncMyMoodle-0.1.0/LICENSE
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)     8442 2023-03-21 15:47:18.452927 syncMyMoodle-0.1.0/PKG-INFO
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)     7793 2022-10-20 13:28:14.000000 syncMyMoodle-0.1.0/README.md
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)      445 2022-10-20 13:27:59.000000 syncMyMoodle-0.1.0/pyproject.toml
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)      982 2023-03-21 15:47:18.452927 syncMyMoodle-0.1.0/setup.cfg
-drwxr-xr-x   0 septatrix  (1000) septatrix  (1000)        0 2023-03-21 15:47:18.451928 syncMyMoodle-0.1.0/syncMyMoodle.egg-info/
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)     8442 2023-03-21 15:47:18.000000 syncMyMoodle-0.1.0/syncMyMoodle.egg-info/PKG-INFO
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)      293 2023-03-21 15:47:18.000000 syncMyMoodle-0.1.0/syncMyMoodle.egg-info/SOURCES.txt
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)        1 2023-03-21 15:47:18.000000 syncMyMoodle-0.1.0/syncMyMoodle.egg-info/dependency_links.txt
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)      177 2023-03-21 15:47:18.000000 syncMyMoodle-0.1.0/syncMyMoodle.egg-info/requires.txt
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)       13 2023-03-21 15:47:18.000000 syncMyMoodle-0.1.0/syncMyMoodle.egg-info/top_level.txt
-drwxr-xr-x   0 septatrix  (1000) septatrix  (1000)        0 2023-03-21 15:47:18.452927 syncMyMoodle-0.1.0/syncmymoodle/
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)        0 2021-07-23 19:20:05.000000 syncMyMoodle-0.1.0/syncmymoodle/__init__.py
--rwxr-xr-x   0 septatrix  (1000) septatrix  (1000)    50300 2023-03-21 15:42:55.000000 syncMyMoodle-0.1.0/syncmymoodle/__main__.py
--rw-r--r--   0 septatrix  (1000) septatrix  (1000)      212 2021-11-11 17:37:01.000000 syncMyMoodle-0.1.0/syncmymoodle/debug.py
+drwxr-xr-x   0 roman     (1000) users      (985)        0 2024-04-07 11:19:24.440528 syncMyMoodle-0.1.1/
+-rw-r--r--   0 roman     (1000) users      (985)    35149 2021-10-07 12:12:02.000000 syncMyMoodle-0.1.1/LICENSE
+-rw-r--r--   0 roman     (1000) users      (985)     9025 2024-04-07 11:19:24.440528 syncMyMoodle-0.1.1/PKG-INFO
+-rw-r--r--   0 roman     (1000) users      (985)     7916 2024-04-07 11:10:20.000000 syncMyMoodle-0.1.1/README.md
+-rw-r--r--   0 roman     (1000) users      (985)      445 2022-02-07 14:25:13.000000 syncMyMoodle-0.1.1/pyproject.toml
+-rw-r--r--   0 roman     (1000) users      (985)      982 2024-04-07 11:19:24.440528 syncMyMoodle-0.1.1/setup.cfg
+drwxr-xr-x   0 roman     (1000) users      (985)        0 2024-04-07 11:19:24.437194 syncMyMoodle-0.1.1/syncMyMoodle.egg-info/
+-rw-r--r--   0 roman     (1000) users      (985)     9025 2024-04-07 11:19:24.000000 syncMyMoodle-0.1.1/syncMyMoodle.egg-info/PKG-INFO
+-rw-r--r--   0 roman     (1000) users      (985)      271 2024-04-07 11:19:24.000000 syncMyMoodle-0.1.1/syncMyMoodle.egg-info/SOURCES.txt
+-rw-r--r--   0 roman     (1000) users      (985)        1 2024-04-07 11:19:24.000000 syncMyMoodle-0.1.1/syncMyMoodle.egg-info/dependency_links.txt
+-rw-r--r--   0 roman     (1000) users      (985)      177 2024-04-07 11:19:24.000000 syncMyMoodle-0.1.1/syncMyMoodle.egg-info/requires.txt
+-rw-r--r--   0 roman     (1000) users      (985)       13 2024-04-07 11:19:24.000000 syncMyMoodle-0.1.1/syncMyMoodle.egg-info/top_level.txt
+drwxr-xr-x   0 roman     (1000) users      (985)        0 2024-04-07 11:19:24.437194 syncMyMoodle-0.1.1/syncmymoodle/
+-rw-r--r--   0 roman     (1000) users      (985)        0 2021-10-07 12:12:02.000000 syncMyMoodle-0.1.1/syncmymoodle/__init__.py
+-rwxr-xr-x   0 roman     (1000) users      (985)    50425 2024-04-07 11:14:12.000000 syncMyMoodle-0.1.1/syncmymoodle/__main__.py
```

### Comparing `syncMyMoodle-0.1.0/LICENSE` & `syncMyMoodle-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `syncMyMoodle-0.1.0/PKG-INFO` & `syncMyMoodle-0.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: syncMyMoodle
-Version: 0.1.0
-Summary: Synchronization client for RWTH Moodle
-Home-page: https://github.com/Romern/syncMyMoodle
-Author: Nils Kattenbeck
-Author-email: nilskemail+pypi@gmail.com
-Project-URL: Bug Tracker, https://github.com/Romern/syncMyMoodle/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: keyring
-Provides-Extra: test
-License-File: LICENSE
-
 # syncMyMoodle
 
 Synchronization client for RWTH Moodle
 
 Downloads the following materials:
 
 * Assignment files, submissions and feedback
@@ -144,36 +126,36 @@
 or to `~/.config/syncmymoodle/config.json` if you wish to configure `syncmymoodle` user-wide.
 
 Here's an overview of the file with some additional remarks as to what each
 configuration does:
 
 ```js
 {
-    "selected_courses": [], //Only these courses will be synced, of the form "https://moodle.rwth-aachen.de/course/view.php?id=XXXXX" (if empty, all courses will be synced)
-    "skip_courses": [], //Skip these courses
-    "only_sync_semester": [], //Only these semesters will be synced, of the form 20ws (only used if selected_courses is empty, if empty all semesters will be synced)
-    "user": "", //Your RWTH SSO username
-    "password": "", //Your RWTH SSO password (not needed if you use secret service)
-    "basedir": "./", //The base directory where all files will be synced to
-    "cookie_file": "./session", //The location of the cookie file,
-    "use_secret_service": false, //Use the secret service integration (requires the secretstorage pip module)
-    "no_links": false, //Skip links embedded in pages. This would disable OpenCast links for example
-    "used_modules": { //Disable downloading certain modules
-        "assign": true, //Assignments
-        "resource": true, //Resources
+    "selected_courses": [], // Only the specified courses (e.g. ["https://moodle.rwth-aachen.de/course/view.php?id=XXXXX"], separated using commas) will be synced
+    "skip_courses": [], // Exclude the specified courses. `selected_courses` overrides this option.
+    "only_sync_semester": [], // Only the specified semesters (e.g. ["23ss", "22ws"]) will be synced. `selected_courses` overrides this option.
+    "user": "", // RWTH SSO username
+    "password": "", // RWTH SSO password
+    "basedir": "./", // The base directory where all your files will be synced to
+    "cookie_file": "./session", // The location of the session/cookie file, which can be used instead of a password.
+    "use_secret_service": false, // Use the Secret Service integration (see README), instead of a password or a cookie file.
+    "no_links": false, // Skip links embedded in pages. Warning: This *will* prevent Onlycast videos from being downloaded.
+    "used_modules": { // Disable downloading certain modules.
+        "assign": true, // Assignments
+        "resource": true, // Resources
         "url": {
-            "youtube": true, //Youtube Links/Embeds
-            "opencast": true, //Opencast Links/Embeds
-            "sciebo": true, //Sciebo Links/Embeds
-            "quiz": false //Quiz Links
+            "youtube": true, // Include YouTube Links/Embeds
+            "opencast": true, // Include Opencast Links/Embeds
+            "sciebo": true, // Include Sciebo Links/Embeds
+            "quiz": false // Include Quiz Links
         },
-        "folder": true, //Folders
+        "folder": true, // Include folders
     },
-    "exclude_filetypes": [] //Exclude specific filetypes, e.g. ["mp4","mkv"] do disable downloading most videos
-    "exlcude_files": [] // Exclude specific files using UNIX filename pattern matching (e.g. "Lecture{video,zoom}*.{mp4,mkv}")
+    "exclude_filetypes": [], // Exclude specific filetypes (e.g. ["mp4", "mkv"]) to disable downloading most videos
+    "exclude_files": [] // Exclude specific files using UNIX filename pattern matching (e.g. "Lecture{video,zoom}*.{mp4,mkv}")
 }
 ```
 
 Command line arguments have a higher priority than configuration files.
 You can override any of the options that you have configured in the file
 using command line arguments.
```

### Comparing `syncMyMoodle-0.1.0/README.md` & `syncMyMoodle-0.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,37 @@
+Metadata-Version: 2.1
+Name: syncMyMoodle
+Version: 0.1.1
+Summary: Synchronization client for RWTH Moodle
+Home-page: https://github.com/Romern/syncMyMoodle
+Author: Nils Kattenbeck
+Author-email: nilskemail+pypi@gmail.com
+Project-URL: Bug Tracker, https://github.com/Romern/syncMyMoodle/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.0.0
+Requires-Dist: beautifulsoup4>=4.0.0
+Requires-Dist: yt-dlp>=2021.12.27
+Requires-Dist: pdfkit>=0.6.0
+Requires-Dist: tqdm>=4.0.0
+Provides-Extra: keyring
+Requires-Dist: secretstorage>=3.1.0; extra == "keyring"
+Provides-Extra: test
+Requires-Dist: black; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: flake8-bugbear; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: types-requests; extra == "test"
+
 # syncMyMoodle
 
 Synchronization client for RWTH Moodle
 
 Downloads the following materials:
 
 * Assignment files, submissions and feedback
@@ -126,36 +156,36 @@
 or to `~/.config/syncmymoodle/config.json` if you wish to configure `syncmymoodle` user-wide.
 
 Here's an overview of the file with some additional remarks as to what each
 configuration does:
 
 ```js
 {
-    "selected_courses": [], //Only these courses will be synced, of the form "https://moodle.rwth-aachen.de/course/view.php?id=XXXXX" (if empty, all courses will be synced)
-    "skip_courses": [], //Skip these courses
-    "only_sync_semester": [], //Only these semesters will be synced, of the form 20ws (only used if selected_courses is empty, if empty all semesters will be synced)
-    "user": "", //Your RWTH SSO username
-    "password": "", //Your RWTH SSO password (not needed if you use secret service)
-    "basedir": "./", //The base directory where all files will be synced to
-    "cookie_file": "./session", //The location of the cookie file,
-    "use_secret_service": false, //Use the secret service integration (requires the secretstorage pip module)
-    "no_links": false, //Skip links embedded in pages. This would disable OpenCast links for example
-    "used_modules": { //Disable downloading certain modules
-        "assign": true, //Assignments
-        "resource": true, //Resources
+    "selected_courses": [], // Only the specified courses (e.g. ["https://moodle.rwth-aachen.de/course/view.php?id=XXXXX"], separated using commas) will be synced
+    "skip_courses": [], // Exclude the specified courses. `selected_courses` overrides this option.
+    "only_sync_semester": [], // Only the specified semesters (e.g. ["23ss", "22ws"]) will be synced. `selected_courses` overrides this option.
+    "user": "", // RWTH SSO username
+    "password": "", // RWTH SSO password
+    "basedir": "./", // The base directory where all your files will be synced to
+    "cookie_file": "./session", // The location of the session/cookie file, which can be used instead of a password.
+    "use_secret_service": false, // Use the Secret Service integration (see README), instead of a password or a cookie file.
+    "no_links": false, // Skip links embedded in pages. Warning: This *will* prevent Onlycast videos from being downloaded.
+    "used_modules": { // Disable downloading certain modules.
+        "assign": true, // Assignments
+        "resource": true, // Resources
         "url": {
-            "youtube": true, //Youtube Links/Embeds
-            "opencast": true, //Opencast Links/Embeds
-            "sciebo": true, //Sciebo Links/Embeds
-            "quiz": false //Quiz Links
+            "youtube": true, // Include YouTube Links/Embeds
+            "opencast": true, // Include Opencast Links/Embeds
+            "sciebo": true, // Include Sciebo Links/Embeds
+            "quiz": false // Include Quiz Links
         },
-        "folder": true, //Folders
+        "folder": true, // Include folders
     },
-    "exclude_filetypes": [] //Exclude specific filetypes, e.g. ["mp4","mkv"] do disable downloading most videos
-    "exlcude_files": [] // Exclude specific files using UNIX filename pattern matching (e.g. "Lecture{video,zoom}*.{mp4,mkv}")
+    "exclude_filetypes": [], // Exclude specific filetypes (e.g. ["mp4", "mkv"]) to disable downloading most videos
+    "exclude_files": [] // Exclude specific files using UNIX filename pattern matching (e.g. "Lecture{video,zoom}*.{mp4,mkv}")
 }
 ```
 
 Command line arguments have a higher priority than configuration files.
 You can override any of the options that you have configured in the file
 using command line arguments.
```

### Comparing `syncMyMoodle-0.1.0/setup.cfg` & `syncMyMoodle-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syncMyMoodle
-version = 0.1.0
+version = 0.1.1
 author = Nils Kattenbeck
 author_email = nilskemail+pypi@gmail.com
 description = Synchronization client for RWTH Moodle
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Romern/syncMyMoodle
 project_urls =
```

### Comparing `syncMyMoodle-0.1.0/syncMyMoodle.egg-info/PKG-INFO` & `syncMyMoodle-0.1.1/syncMyMoodle.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 Metadata-Version: 2.1
 Name: syncMyMoodle
-Version: 0.1.0
+Version: 0.1.1
 Summary: Synchronization client for RWTH Moodle
 Home-page: https://github.com/Romern/syncMyMoodle
 Author: Nils Kattenbeck
 Author-email: nilskemail+pypi@gmail.com
 Project-URL: Bug Tracker, https://github.com/Romern/syncMyMoodle/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.0.0
+Requires-Dist: beautifulsoup4>=4.0.0
+Requires-Dist: yt-dlp>=2021.12.27
+Requires-Dist: pdfkit>=0.6.0
+Requires-Dist: tqdm>=4.0.0
 Provides-Extra: keyring
+Requires-Dist: secretstorage>=3.1.0; extra == "keyring"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: black; extra == "test"
+Requires-Dist: isort; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: flake8-bugbear; extra == "test"
+Requires-Dist: mypy; extra == "test"
+Requires-Dist: types-requests; extra == "test"
 
 # syncMyMoodle
 
 Synchronization client for RWTH Moodle
 
 Downloads the following materials:
 
@@ -144,36 +156,36 @@
 or to `~/.config/syncmymoodle/config.json` if you wish to configure `syncmymoodle` user-wide.
 
 Here's an overview of the file with some additional remarks as to what each
 configuration does:
 
 ```js
 {
-    "selected_courses": [], //Only these courses will be synced, of the form "https://moodle.rwth-aachen.de/course/view.php?id=XXXXX" (if empty, all courses will be synced)
-    "skip_courses": [], //Skip these courses
-    "only_sync_semester": [], //Only these semesters will be synced, of the form 20ws (only used if selected_courses is empty, if empty all semesters will be synced)
-    "user": "", //Your RWTH SSO username
-    "password": "", //Your RWTH SSO password (not needed if you use secret service)
-    "basedir": "./", //The base directory where all files will be synced to
-    "cookie_file": "./session", //The location of the cookie file,
-    "use_secret_service": false, //Use the secret service integration (requires the secretstorage pip module)
-    "no_links": false, //Skip links embedded in pages. This would disable OpenCast links for example
-    "used_modules": { //Disable downloading certain modules
-        "assign": true, //Assignments
-        "resource": true, //Resources
+    "selected_courses": [], // Only the specified courses (e.g. ["https://moodle.rwth-aachen.de/course/view.php?id=XXXXX"], separated using commas) will be synced
+    "skip_courses": [], // Exclude the specified courses. `selected_courses` overrides this option.
+    "only_sync_semester": [], // Only the specified semesters (e.g. ["23ss", "22ws"]) will be synced. `selected_courses` overrides this option.
+    "user": "", // RWTH SSO username
+    "password": "", // RWTH SSO password
+    "basedir": "./", // The base directory where all your files will be synced to
+    "cookie_file": "./session", // The location of the session/cookie file, which can be used instead of a password.
+    "use_secret_service": false, // Use the Secret Service integration (see README), instead of a password or a cookie file.
+    "no_links": false, // Skip links embedded in pages. Warning: This *will* prevent Onlycast videos from being downloaded.
+    "used_modules": { // Disable downloading certain modules.
+        "assign": true, // Assignments
+        "resource": true, // Resources
         "url": {
-            "youtube": true, //Youtube Links/Embeds
-            "opencast": true, //Opencast Links/Embeds
-            "sciebo": true, //Sciebo Links/Embeds
-            "quiz": false //Quiz Links
+            "youtube": true, // Include YouTube Links/Embeds
+            "opencast": true, // Include Opencast Links/Embeds
+            "sciebo": true, // Include Sciebo Links/Embeds
+            "quiz": false // Include Quiz Links
         },
-        "folder": true, //Folders
+        "folder": true, // Include folders
     },
-    "exclude_filetypes": [] //Exclude specific filetypes, e.g. ["mp4","mkv"] do disable downloading most videos
-    "exlcude_files": [] // Exclude specific files using UNIX filename pattern matching (e.g. "Lecture{video,zoom}*.{mp4,mkv}")
+    "exclude_filetypes": [], // Exclude specific filetypes (e.g. ["mp4", "mkv"]) to disable downloading most videos
+    "exclude_files": [] // Exclude specific files using UNIX filename pattern matching (e.g. "Lecture{video,zoom}*.{mp4,mkv}")
 }
 ```
 
 Command line arguments have a higher priority than configuration files.
 You can override any of the options that you have configured in the file
 using command line arguments.
```

### Comparing `syncMyMoodle-0.1.0/syncmymoodle/__main__.py` & `syncMyMoodle-0.1.1/syncmymoodle/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import http.client
 import json
 import logging
 import os
 import pickle
 import re
 import shutil
+import sys
 import urllib.parse
 from argparse import ArgumentParser
 from contextlib import closing
 from fnmatch import fnmatchcase
 from pathlib import Path
 from typing import TYPE_CHECKING, List
 
@@ -174,21 +175,22 @@
         self.user_id = None
         self.root_node = None
 
     # RWTH SSO Login
 
     def login(self):
         def get_session_key(soup):
-            try:
-                session_key = soup.find("input", {"name": "sesskey"})["value"]
-            except TypeError:
-                logger.critical("Can't retrieve session key")
-                logger.info(soup)
+            script = soup.find("script", string=lambda text: text and "sesskey" in text)
+            js_text = script.text
+            match = re.search(r'"sesskey":"(.*?)"', js_text)
+            if match:
+                return match.group(1)
+            else:
+                logger.critical("Can't retrieve session key from JavaScript config")
                 exit(1)
-            return session_key
 
         self.session = requests.Session()
         cookie_file = Path(self.config.get("cookie_file", "./session"))
         if cookie_file.exists():
             with cookie_file.open("rb") as f:
                 self.session.cookies.update(pickle.load(f))
         resp = self.session.get("https://moodle.rwth-aachen.de/")
@@ -214,15 +216,15 @@
             soup = bs(resp2.text, features="html.parser")
         if soup.find("input", {"name": "RelayState"}) is None:
             logger.critical(
                 "Failed to login! Maybe your login-info was wrong or the RWTH-Servers have difficulties, see https://maintenance.rz.rwth-aachen.de/ticket/status/messages . For more info use the --verbose argument."
             )
             logger.info("-------Login-Error-Soup--------")
             logger.info(soup)
-            exit(1)
+            sys.exit(1)
         data = {
             "RelayState": soup.find("input", {"name": "RelayState"})["value"],
             "SAMLResponse": soup.find("input", {"name": "SAMLResponse"})["value"],
         }
         resp = self.session.post(
             "https://moodle.rwth-aachen.de/Shibboleth.sso/SAML2/POST", data=data
         )
@@ -321,15 +323,15 @@
             params=params,
             data=data,
         )
         if not resp.json().get("userid") or not resp.json()["userprivateaccesskey"]:
             logger.critical(
                 f"Error while getting userid and access key: {json.dumps(resp.json(), indent=4)}"
             )
-            exit(1)
+            sys.exit(1)
         self.user_id = resp.json()["userid"]
         self.user_private_access_key = resp.json()["userprivateaccesskey"]
         return self.user_id, self.user_private_access_key
 
     def get_assignment(self, course_id):
         data = {
             "courseids[0]": int(course_id),
@@ -1189,28 +1191,28 @@
         logger.warning(
             "You do not have wkhtmltopdf in your path. Quiz-PDFs are NOT generated"
         )
 
     if secretstorage and config.get("use_secret_service"):
         if config.get("password"):
             logger.critical("You need to remove your password from your config file!")
-            exit(1)
+            sys.exit(1)
 
         connection = secretstorage.dbus_init()
         collection = secretstorage.get_default_collection(connection)
         if collection.is_locked():
             collection.unlock()
         attributes = {"application": "syncMyMoodle"}
         results = list(collection.search_items(attributes))
         if len(results) == 0:
             if not args.user and not config.get("user"):
                 print(
                     "You need to provide your username in the config file or through --user!"
                 )
-                exit(1)
+                sys.exit(1)
             if args.password:
                 password = args.password
             else:
                 password = getpass.getpass("Password:")
             attributes["username"] = config["user"]
             item = collection.create_item(
                 f'{config["user"]}@rwth-aachen.de', attributes, password
@@ -1229,15 +1231,15 @@
             config["user"] = item.get_attributes().get("username")
         config["password"] = item.get_secret().decode("utf-8")
 
     if not config.get("user") or not config.get("password"):
         logger.critical(
             "You need to specify your username and password in the config file or as an argument!"
         )
-        exit(1)
+        sys.exit(1)
 
     smm = SyncMyMoodle(config)
 
     print("Logging in...")
     smm.login()
     smm.get_moodle_wstoken()
     smm.get_userid()
```

