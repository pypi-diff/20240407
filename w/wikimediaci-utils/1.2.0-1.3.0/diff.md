# Comparing `tmp/wikimediaci_utils-1.2.0.tar.gz` & `tmp/wikimediaci_utils-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikimediaci_utils-1.2.0.tar", last modified: Tue Jan 24 11:46:23 2023, max compression
+gzip compressed data, was "wikimediaci_utils-1.3.0.tar", last modified: Sun Apr  7 13:39:55 2024, max compression
```

## Comparing `wikimediaci_utils-1.2.0.tar` & `wikimediaci_utils-1.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-24 11:46:23.017000 wikimediaci_utils-1.2.0/
--rw-r--r--   0 user      (1000) user      (1000)    35149 2019-12-14 10:39:21.000000 wikimediaci_utils-1.2.0/COPYING
--rw-r--r--   0 user      (1000) user      (1000)      594 2023-01-24 11:46:23.017000 wikimediaci_utils-1.2.0/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      243 2020-07-17 23:40:34.000000 wikimediaci_utils-1.2.0/README.rst
--rw-r--r--   0 user      (1000) user      (1000)       38 2023-01-24 11:46:23.017000 wikimediaci_utils-1.2.0/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      609 2023-01-24 11:40:17.000000 wikimediaci_utils-1.2.0/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-24 11:46:23.016000 wikimediaci_utils-1.2.0/wikimediaci_utils/
--rw-r--r--   0 user      (1000) user      (1000)     2862 2023-01-24 11:40:51.000000 wikimediaci_utils-1.2.0/wikimediaci_utils/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)        0 2020-01-16 04:29:39.000000 wikimediaci_utils-1.2.0/wikimediaci_utils/py.typed
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-01-24 11:46:23.017000 wikimediaci_utils-1.2.0/wikimediaci_utils.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      594 2023-01-24 11:46:22.000000 wikimediaci_utils-1.2.0/wikimediaci_utils.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      288 2023-01-24 11:46:22.000000 wikimediaci_utils-1.2.0/wikimediaci_utils.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-01-24 11:46:22.000000 wikimediaci_utils-1.2.0/wikimediaci_utils.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)       16 2023-01-24 11:46:22.000000 wikimediaci_utils-1.2.0/wikimediaci_utils.egg-info/requires.txt
--rw-r--r--   0 user      (1000) user      (1000)       18 2023-01-24 11:46:22.000000 wikimediaci_utils-1.2.0/wikimediaci_utils.egg-info/top_level.txt
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2024-04-07 13:39:55.511021 wikimediaci_utils-1.3.0/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)    35149 2024-04-01 18:55:05.000000 wikimediaci_utils-1.3.0/COPYING
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      640 2024-04-07 13:39:55.511021 wikimediaci_utils-1.3.0/PKG-INFO
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      243 2024-04-01 18:55:05.000000 wikimediaci_utils-1.3.0/README.rst
+-rw-r--r--   0 taavi     (1000) taavi     (1000)       38 2024-04-07 13:39:55.511021 wikimediaci_utils-1.3.0/setup.cfg
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      609 2024-04-07 13:35:32.000000 wikimediaci_utils-1.3.0/setup.py
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2024-04-07 13:39:55.507021 wikimediaci_utils-1.3.0/tests/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)     1770 2024-04-01 18:55:05.000000 wikimediaci_utils-1.3.0/tests/test_init.py
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2024-04-07 13:39:55.511021 wikimediaci_utils-1.3.0/wikimediaci_utils/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)     2860 2024-04-01 19:39:51.000000 wikimediaci_utils-1.3.0/wikimediaci_utils/__init__.py
+-rw-r--r--   0 taavi     (1000) taavi     (1000)        0 2024-04-01 18:55:05.000000 wikimediaci_utils-1.3.0/wikimediaci_utils/py.typed
+drwxr-xr-x   0 taavi     (1000) taavi     (1000)        0 2024-04-07 13:39:55.511021 wikimediaci_utils-1.3.0/wikimediaci_utils.egg-info/
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      640 2024-04-07 13:39:55.000000 wikimediaci_utils-1.3.0/wikimediaci_utils.egg-info/PKG-INFO
+-rw-r--r--   0 taavi     (1000) taavi     (1000)      307 2024-04-07 13:39:55.000000 wikimediaci_utils-1.3.0/wikimediaci_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 taavi     (1000) taavi     (1000)        1 2024-04-07 13:39:55.000000 wikimediaci_utils-1.3.0/wikimediaci_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 taavi     (1000) taavi     (1000)       16 2024-04-07 13:39:55.000000 wikimediaci_utils-1.3.0/wikimediaci_utils.egg-info/requires.txt
+-rw-r--r--   0 taavi     (1000) taavi     (1000)       18 2024-04-07 13:39:55.000000 wikimediaci_utils-1.3.0/wikimediaci_utils.egg-info/top_level.txt
```

### Comparing `wikimediaci_utils-1.2.0/COPYING` & `wikimediaci_utils-1.3.0/COPYING`

 * *Files identical despite different names*

### Comparing `wikimediaci_utils-1.2.0/PKG-INFO` & `wikimediaci_utils-1.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: wikimediaci_utils
-Version: 1.2.0
+Version: 1.3.0
 Summary: Common utility functions for tools related to Wikimedia CI
 Home-page: https://gerrit.wikimedia.org/g/integration/utils
 Author: Kunal Mehta
 Author-email: legoktm@debian.org
 License: GPL-3.0-or-later
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: COPYING
+Requires-Dist: pyyaml
+Requires-Dist: requests
 
 wikimediaci_utils
 =================
 
 A collection of utility functions that are commonly used in tools that
 assist with Wikimedia Continuous Integration.
```

### Comparing `wikimediaci_utils-1.2.0/setup.py` & `wikimediaci_utils-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 
 setup(
     name='wikimediaci_utils',
-    version='1.2.0',
+    version='1.3.0',
     packages=['wikimediaci_utils'],
     package_data={'wikimediaci_utils': ['py.typed']},
-    python_requires='>=3.5',
+    python_requires='>=3.7',
     url='https://gerrit.wikimedia.org/g/integration/utils',
     license='GPL-3.0-or-later',
     author='Kunal Mehta',
     author_email='legoktm@debian.org',
     description='Common utility functions for tools related to Wikimedia CI',
     long_description=open('README.rst').read(),
     long_description_content_type='text/x-rst',
```

### Comparing `wikimediaci_utils-1.2.0/wikimediaci_utils/__init__.py` & `wikimediaci_utils-1.3.0/wikimediaci_utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     """Whether a repository is bundled in the MediaWiki tarball"""
     return repo in get_bundled_list()
 
 
 @functools.lru_cache()
 def _settings_yaml() -> dict:
     r = session.get("https://gitlab.wikimedia.org/repos/releng/release/"
-                    "-/raw/master/make-release/settings.yaml")
+                    "-/raw/main/make-release/settings.yaml")
     r.raise_for_status()
     return yaml.safe_load(r.text)
 
 
 def get_bundled_list() -> list:
     """List of repositories that are bundled in the MediaWiki tarball"""
     return [name for name in _settings_yaml()['bundles']['base']]
```

### Comparing `wikimediaci_utils-1.2.0/wikimediaci_utils.egg-info/PKG-INFO` & `wikimediaci_utils-1.3.0/wikimediaci_utils.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
-Name: wikimediaci-utils
-Version: 1.2.0
+Name: wikimediaci_utils
+Version: 1.3.0
 Summary: Common utility functions for tools related to Wikimedia CI
 Home-page: https://gerrit.wikimedia.org/g/integration/utils
 Author: Kunal Mehta
 Author-email: legoktm@debian.org
 License: GPL-3.0-or-later
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: COPYING
+Requires-Dist: pyyaml
+Requires-Dist: requests
 
 wikimediaci_utils
 =================
 
 A collection of utility functions that are commonly used in tools that
 assist with Wikimedia Continuous Integration.
```

