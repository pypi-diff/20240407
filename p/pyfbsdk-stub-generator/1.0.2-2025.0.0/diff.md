# Comparing `tmp/pyfbsdk-stub-generator-1.0.2.tar.gz` & `tmp/pyfbsdk-stub-generator-2025.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfbsdk-stub-generator-1.0.2.tar", last modified: Sun Aug 13 14:04:18 2023, max compression
+gzip compressed data, was "pyfbsdk-stub-generator-2025.0.0.tar", last modified: Sun Apr  7 15:21:28 2024, max compression
```

## Comparing `pyfbsdk-stub-generator-1.0.2.tar` & `pyfbsdk-stub-generator-2025.0.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/base_content/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/module_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/native_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/dunder_methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/dunder_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/dunder_methods/dunder_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/fb_property/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/fb_property/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_urls.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py
--rw-r--r--   0 runner    (1001) docker     (123)    16699 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/stub_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-08-13 14:04:18.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-13 14:04:18.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-13 14:04:18.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-13 14:04:18.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-13 14:04:18.000000 pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-13 14:04:02.000000 pyfbsdk-stub-generator-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-13 14:04:18.722009 pyfbsdk-stub-generator-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.656886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.656886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/base_content/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/base_content/pyfbsdk.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/module_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9792 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/native_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.656886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.656886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/dunder_methods/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/dunder_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/dunder_methods/dunder_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/fb_property/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/fb_property/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12649 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16699 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6745 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/stub_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-07 15:21:28.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-04-07 15:21:28.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:21:28.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 15:21:28.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-07 15:21:28.000000 pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-07 15:21:24.000000 pyfbsdk-stub-generator-2025.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-07 15:21:28.660886 pyfbsdk-stub-generator-2025.0.0/setup.cfg
```

### Comparing `pyfbsdk-stub-generator-1.0.2/LICENSE` & `pyfbsdk-stub-generator-2025.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/PKG-INFO` & `pyfbsdk-stub-generator-2025.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
 Name: pyfbsdk-stub-generator
-Version: 1.0.2
+Version: 2025.0.0
 Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
 Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
 Author: Nils Soderman
 License: MIT-0
 Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: requests
+Requires-Dist: Js2Py
 
 # MotionBuilder pyfbsdk stub-file generator
 Script for generating python stub files for Autodesk MotionBuilder's pyfbsdk module.
 
 These stub files include all classes & functions that can be accessed through the pyfbsdk module.
 They also include type hints and docstrings for most entities.
 
 
 <br>
 
 
 # Pre-generated files
 The GitHub repository already contains some pre-generated stub files that are ready to be used, simply get them from the [generated-stub-files](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files) folder:
-* [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
-* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2025](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2025)
 * [MotionBuilder 2024](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2024)
+* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
 
 <br>
 
 # Usage
 
 ## Generate stub files
 If you want to generate your own stub files for your MotionBuilder version:
```

### Comparing `pyfbsdk-stub-generator-1.0.2/README.md` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,40 @@
+Metadata-Version: 2.1
+Name: pyfbsdk-stub-generator
+Version: 2025.0.0
+Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
+Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
+Author: Nils Soderman
+License: MIT-0
+Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: requests
+Requires-Dist: Js2Py
+
 # MotionBuilder pyfbsdk stub-file generator
 Script for generating python stub files for Autodesk MotionBuilder's pyfbsdk module.
 
 These stub files include all classes & functions that can be accessed through the pyfbsdk module.
 They also include type hints and docstrings for most entities.
 
 
 <br>
 
 
 # Pre-generated files
 The GitHub repository already contains some pre-generated stub files that are ready to be used, simply get them from the [generated-stub-files](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files) folder:
-* [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
-* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2025](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2025)
 * [MotionBuilder 2024](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2024)
+* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
 
 <br>
 
 # Usage
 
 ## Generate stub files
 If you want to generate your own stub files for your MotionBuilder version:
@@ -35,8 +53,8 @@
 
 <br>
 
 # Application Spesific Setup
 
 ## Visual Studio Code
 
-These stub files comes bundeled with the [MotionBuilder Utils](https://marketplace.visualstudio.com/items?itemName=NilsSoderman.mobu-utils) VSCode extention.
+These stub files comes bundeled with the [MotionBuilder Utils](https://marketplace.visualstudio.com/items?itemName=NilsSoderman.mobu-utils) VSCode extention.
```

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/__init__.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/module_types.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/module_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,14 +82,19 @@
     def GetParamsAsString(self):
         ParametersAsStrings = []
         for i, Param in enumerate(self._Params):
             if self.bIsMethod and i == 0:
                 Param.Name = "self"
                 Param.Type = None
             ParametersAsStrings.append(Param.GetAsString())
+            
+        # Insert a / to indicate that the function only accepts positional parameters
+        # Only the function takes more than 1 parameter (excluding self)
+        if (not self.bIsMethod and len(self._Params) > 0) or len(self._Params) > 1:
+            ParametersAsStrings.append("/")
 
         return ",".join(ParametersAsStrings)
 
     def GetAsString(self):
         FunctionAsString = ""
         if self.bIsOverload:
             FunctionAsString += "@overload\n"
```

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/native_generator.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/native_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import inspect
+import typing
 import types
 
 from types import ModuleType
 from importlib import reload
 
 from . import module_types
 from .module_types import StubClass, StubFunction, StubParameter, StubProperty
@@ -108,15 +109,15 @@
             ParentClassName = ENUMERATION_NAME
 
         ParentClassNames.append(ParentClassName)
 
     return ParentClassNames
 
 
-def GetFunctionInfoFromDocString(Function) -> list[tuple[list[StubParameter], str]]:
+def GetFunctionInfoFromDocString(Function: typing.Callable) -> list[tuple[list[StubParameter], str]]:
     """
     Get Parameters & Return type from the docstring, can return multiple results if overload functions exists.
 
     Returns: a list of tuple([Parameters], ReturnType)
     """
     def _GenerateParams(ParamsString, DefaultValue = None) -> list[StubParameter]:
         """ 
@@ -135,18 +136,24 @@
     if not Function.__doc__:  # No docstring
         return []
 
     FunctionParamters = []
     # Read the docstring and split it up if there are multiple function overrides
     FunctionsDocs = [x for x in Function.__doc__.split("\n") if x]
     for Doc in FunctionsDocs:
+        # Make sure `Doc` now follows this format: "FunctionName( (str)arg1 [, (object)arg2]) -> object"
+        if not Doc.strip().startswith(Function.__name__) or not all(x in Doc for x in ["->", "(", ")"]):
+            continue
+
         # 'Doc' will now look something like this:
         # ShowToolByName( (str)arg1 [, (object)arg2]) -> object
         Doc = Doc.partition("(")[2]  # Remove function name
         Params, _, ReturnType = Doc.rpartition("->")
+        
+        ReturnType = ReturnType.strip(" :")
 
         # Split params into required & optional
         Params = Params.rpartition(")")[0]
         RequiredParams, _, OptionalParams = Params.partition("[")
         OptionalParams = OptionalParams.replace("[", "").replace("]", "").lstrip(',')
 
         Params = []
```

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/__init__.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/dunder_methods/dunder_methods.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/dunder_methods/dunder_methods.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/fb_property/fb_property_plugin.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/doc_bases.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/modules/pyfbsdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,19 @@
         Parameters = (None, None, None, None, None, Parameter(Type = (pyfbsdk.FBProperty, "None")))
         ReturnType = Any
         
 class FBModel(ClassBase):
     class Parent(PropertyBase):
         Types = (pyfbsdk.FBModel, "None")
 
+
+class FBModelPath3D(ClassBase):
+    class PathEndCapStyle(PropertyBase):
+        Types = pyfbsdk.FBModelPath3D.EPathEndCapStyle
+
 # ---------------------------------------------------------------------
 #                          Functions
 # ---------------------------------------------------------------------
 
 class GetToolPosition(FunctionBase):
     """This function will get the position of a specific tool.
     ### Parameters:
```

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/manual_documentation/plugin_manual_docs.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/documentation_cache.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/page_parser.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/documentation_scraper/table_of_contents.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/online_documentation/plugin_online_documentation.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/plugins/plugin.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/plugins/plugin.py`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator/stub_generator.py` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator/stub_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     for ImportedModule in list(sys.modules.values()):
         if isinstance(ImportedModule, ModuleType) and "pyfbsdk_stub_generator" in ImportedModule.__name__:
             reload(ImportedModule)
 
     for Path in (
         os.path.dirname(os.path.dirname(__file__)),
         f"C:/Python{sys.version_info.major}{sys.version_info.minor}/lib/site-packages",
-        f"{os.getenv('APPDATA')}/Python/Python310/site-packages"
+        f"{os.getenv('APPDATA')}/Python/Python{sys.version_info.major}{sys.version_info.minor}/site-packages"
     ):
         if Path not in sys.path:
             sys.path.append(Path)
     __name__ = "pyfbsdk_stub_generator.stub_generator"  # pylint: disable=redefined-builtin
     os.environ["PYFBSDK_DEVMODE"] = "True"
 
 from . import plugins
```

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/PKG-INFO` & `pyfbsdk-stub-generator-2025.0.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-Metadata-Version: 2.1
-Name: pyfbsdk-stub-generator
-Version: 1.0.2
-Summary: Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
-Home-page: https://github.com/nils-soderman/pyfbsdk-stub-generator
-Author: Nils Soderman
-License: MIT-0
-Keywords: pyfbsdk,motionbuilder,mobu,autodesk,stub,stubfile,generator,gen
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MotionBuilder pyfbsdk stub-file generator
 Script for generating python stub files for Autodesk MotionBuilder's pyfbsdk module.
 
 These stub files include all classes & functions that can be accessed through the pyfbsdk module.
 They also include type hints and docstrings for most entities.
 
 
 <br>
 
 
 # Pre-generated files
 The GitHub repository already contains some pre-generated stub files that are ready to be used, simply get them from the [generated-stub-files](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files) folder:
-* [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
-* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2025](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2025)
 * [MotionBuilder 2024](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2024)
+* [MotionBuilder 2023](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2023)
+* [MotionBuilder 2022](https://github.com/nils-soderman/pyfbsdk-stub-generator/tree/main/generated-stub-files/motionbuilder-2022)
 
 <br>
 
 # Usage
 
 ## Generate stub files
 If you want to generate your own stub files for your MotionBuilder version:
@@ -48,8 +36,8 @@
 
 <br>
 
 # Application Spesific Setup
 
 ## Visual Studio Code
 
-These stub files comes bundeled with the [MotionBuilder Utils](https://marketplace.visualstudio.com/items?itemName=NilsSoderman.mobu-utils) VSCode extention.
+These stub files comes bundeled with the [MotionBuilder Utils](https://marketplace.visualstudio.com/items?itemName=NilsSoderman.mobu-utils) VSCode extention.
```

### Comparing `pyfbsdk-stub-generator-1.0.2/pyfbsdk_stub_generator.egg-info/SOURCES.txt` & `pyfbsdk-stub-generator-2025.0.0/pyfbsdk_stub_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfbsdk-stub-generator-1.0.2/setup.cfg` & `pyfbsdk-stub-generator-2025.0.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyfbsdk-stub-generator
-version = 1.0.2
+version = 2025.0.0
 author = Nils Soderman
 description = Generate pyfbsdk stub files for better intellisense when working with MotionBuilder
 license = MIT-0
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nils-soderman/pyfbsdk-stub-generator
 keywords = pyfbsdk, motionbuilder, mobu, autodesk, stub, stubfile, generator, gen
```

