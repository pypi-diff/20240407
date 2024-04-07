# Comparing `tmp/disnake-ext-invitetracker-0.0.2.tar.gz` & `tmp/disnake-ext-invitetracker-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disnake-ext-invitetracker-0.0.2.tar", last modified: Thu Sep  1 05:49:44 2022, max compression
+gzip compressed data, was "disnake-ext-invitetracker-1.0.tar", last modified: Sun Apr  7 02:34:55 2024, max compression
```

## Comparing `disnake-ext-invitetracker-0.0.2.tar` & `disnake-ext-invitetracker-1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-09-01 05:49:44.824333 disnake-ext-invitetracker-0.0.2/
--rw-rw-rw-   0        0        0    11538 2022-07-20 19:09:56.000000 disnake-ext-invitetracker-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2323 2022-09-01 05:49:44.823333 disnake-ext-invitetracker-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      797 2022-07-20 19:38:18.000000 disnake-ext-invitetracker-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2022-09-01 05:49:44.795327 disnake-ext-invitetracker-0.0.2/disnake/
-drwxrwxrwx   0        0        0        0 2022-09-01 05:49:44.796327 disnake-ext-invitetracker-0.0.2/disnake/ext/
-drwxrwxrwx   0        0        0        0 2022-09-01 05:49:44.803329 disnake-ext-invitetracker-0.0.2/disnake/ext/invitetracker/
--rw-rw-rw-   0        0        0      214 2022-09-01 05:47:57.000000 disnake-ext-invitetracker-0.0.2/disnake/ext/invitetracker/__init__.py
--rw-rw-rw-   0        0        0     2091 2022-09-01 05:46:29.000000 disnake-ext-invitetracker-0.0.2/disnake/ext/invitetracker/invite_logger.py
-drwxrwxrwx   0        0        0        0 2022-09-01 05:49:44.819332 disnake-ext-invitetracker-0.0.2/disnake_ext_invitetracker.egg-info/
--rw-rw-rw-   0        0        0     2323 2022-09-01 05:49:44.000000 disnake-ext-invitetracker-0.0.2/disnake_ext_invitetracker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2022-09-01 05:49:44.000000 disnake-ext-invitetracker-0.0.2/disnake_ext_invitetracker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-01 05:49:44.000000 disnake-ext-invitetracker-0.0.2/disnake_ext_invitetracker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-09-01 05:49:44.000000 disnake-ext-invitetracker-0.0.2/disnake_ext_invitetracker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-09-01 05:49:44.000000 disnake-ext-invitetracker-0.0.2/disnake_ext_invitetracker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-09-01 05:49:44.825333 disnake-ext-invitetracker-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2706 2022-07-20 19:39:07.000000 disnake-ext-invitetracker-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.549580 disnake-ext-invitetracker-1.0/
+-rw-rw-rw-   0        0        0    11539 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/LICENSE
+-rw-rw-rw-   0        0        0     2478 2024-04-07 02:34:55.548114 disnake-ext-invitetracker-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.525999 disnake-ext-invitetracker-1.0/disnake/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.525999 disnake-ext-invitetracker-1.0/disnake/ext/
+drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.529401 disnake-ext-invitetracker-1.0/disnake/ext/invitetracker/
+-rw-rw-rw-   0        0        0      199 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/disnake/ext/invitetracker/__init__.py
+-rw-rw-rw-   0        0        0     4883 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/disnake/ext/invitetracker/invite_tracker.py
+drwxrwxrwx   0        0        0        0 2024-04-07 02:34:55.548114 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/
+-rw-rw-rw-   0        0        0     2478 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 02:34:55.000000 disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 02:34:55.549580 disnake-ext-invitetracker-1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2608 2024-04-07 02:30:49.000000 disnake-ext-invitetracker-1.0/setup.py
```

### Comparing `disnake-ext-invitetracker-0.0.2/LICENSE` & `disnake-ext-invitetracker-1.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright (c) 2022 Lukef
+   Copyright (c) 2024 earluv
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `disnake-ext-invitetracker-0.0.2/PKG-INFO` & `disnake-ext-invitetracker-1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: disnake-ext-invitetracker
-Version: 0.0.2
+Version: 1.0
 Summary: A module that allows you to track invitations
-Home-page: https://github.com/LukeFokin/disnake-ext-invitetracker
+Home-page: https://github.com/earluv/disnake-ext-invitetracker
 Author: Lukef
 License: Apache Software License
-Project-URL: Source, https://github.com/LukeFokin/disnake-ext-invitetracker
+Project-URL: Source, https://github.com/earluv/disnake-ext-invitetracker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinxcontrib_trio; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # disnake-ext-invitetracker
 
 [![PyPI version info](https://img.shields.io/pypi/v/disnake-ext-invitetracker.svg)](https://pypi.python.org/pypi/disnake-ext-invitetracker)
 
 ## About
 
@@ -55,13 +56,15 @@
 
 # Windows
 py -3 -m pip install -U disnake-ext-invitetracker
 ```
 
 ## Links
 
-- [Usage Examples](https://github.com/LukeFokin/disnake-ext-invitetracker/tree/main/examples)
+- [Usage Examples](https://github.com/earluv/disnake-ext-invitetracker/tree/main/examples)
 - [Disnake Server](https://discord.gg/disnake)
+- [Disnake [RU] Server](https://discord.gg/RrpKVNuRCc)
+- [Earluv | Discord](https://discordapp.com/users/211148434273468426)
 
 ## License
 
-Copyright (c) 2022 Lukef  
+Copyright (c) 2024 earluv
```

### Comparing `disnake-ext-invitetracker-0.0.2/README.md` & `disnake-ext-invitetracker-1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -20,13 +20,15 @@
 
 # Windows
 py -3 -m pip install -U disnake-ext-invitetracker
 ```
 
 ## Links
 
-- [Usage Examples](https://github.com/LukeFokin/disnake-ext-invitetracker/tree/main/examples)
+- [Usage Examples](https://github.com/earluv/disnake-ext-invitetracker/tree/main/examples)
 - [Disnake Server](https://discord.gg/disnake)
+- [Disnake [RU] Server](https://discord.gg/RrpKVNuRCc)
+- [Earluv | Discord](https://discordapp.com/users/211148434273468426)
 
 ## License
 
-Copyright (c) 2022 Lukef  
+Copyright (c) 2024 earluv
```

### Comparing `disnake-ext-invitetracker-0.0.2/disnake_ext_invitetracker.egg-info/PKG-INFO` & `disnake-ext-invitetracker-1.0/disnake_ext_invitetracker.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: disnake-ext-invitetracker
-Version: 0.0.2
+Version: 1.0
 Summary: A module that allows you to track invitations
-Home-page: https://github.com/LukeFokin/disnake-ext-invitetracker
+Home-page: https://github.com/earluv/disnake-ext-invitetracker
 Author: Lukef
 License: Apache Software License
-Project-URL: Source, https://github.com/LukeFokin/disnake-ext-invitetracker
+Project-URL: Source, https://github.com/earluv/disnake-ext-invitetracker
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Communications
 Classifier: Topic :: Documentation
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.6.0
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Provides-Extra: docs
 License-File: LICENSE
+Provides-Extra: docs
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: sphinxcontrib_trio; extra == "docs"
+Requires-Dist: sphinx-rtd-theme; extra == "docs"
 
 # disnake-ext-invitetracker
 
 [![PyPI version info](https://img.shields.io/pypi/v/disnake-ext-invitetracker.svg)](https://pypi.python.org/pypi/disnake-ext-invitetracker)
 
 ## About
 
@@ -55,13 +56,15 @@
 
 # Windows
 py -3 -m pip install -U disnake-ext-invitetracker
 ```
 
 ## Links
 
-- [Usage Examples](https://github.com/LukeFokin/disnake-ext-invitetracker/tree/main/examples)
+- [Usage Examples](https://github.com/earluv/disnake-ext-invitetracker/tree/main/examples)
 - [Disnake Server](https://discord.gg/disnake)
+- [Disnake [RU] Server](https://discord.gg/RrpKVNuRCc)
+- [Earluv | Discord](https://discordapp.com/users/211148434273468426)
 
 ## License
 
-Copyright (c) 2022 Lukef  
+Copyright (c) 2024 earluv
```

### Comparing `disnake-ext-invitetracker-0.0.2/setup.py` & `disnake-ext-invitetracker-1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Communications",
     "Topic :: Documentation",
     "Topic :: Documentation :: Sphinx",
@@ -38,15 +36,15 @@
 }
 
 packages = [
     "disnake.ext.invitetracker",
 ]
 
 project_urls = {
-    "Source": "https://github.com/LukeFokin/disnake-ext-invitetracker",
+    "Source": "https://github.com/earluv/disnake-ext-invitetracker",
 }
 
 _version_regex = r"^version = ('|\")((?:[0-9]+\.)*[0-9]+(?:\.?([a-z]+)(?:\.?[0-9])?)?)\1$"
 
 with open("disnake/ext/invitetracker/__init__.py") as stream:
     match = re.search(_version_regex, stream.read(), re.MULTILINE)
 
@@ -76,11 +74,11 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     extras_require=extras_require,
     license="Apache Software License",
     name="disnake-ext-invitetracker",
     packages=packages,
     project_urls=project_urls,
-    python_requires=">=3.6.0",
-    url="https://github.com/LukeFokin/disnake-ext-invitetracker",
+    python_requires=">=3.8.0",
+    url="https://github.com/earluv/disnake-ext-invitetracker",
     version=version,
 )
```

