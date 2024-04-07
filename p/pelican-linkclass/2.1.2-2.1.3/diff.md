# Comparing `tmp/pelican_linkclass-2.1.2.tar.gz` & `tmp/pelican_linkclass-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Oct 31 15:33:56 2023, max compression
+gzip compressed data, was "pelican_linkclass-2.1.3.tar", last modified: Sun Apr  7 09:25:56 2024, max compression
```

## Comparing `pelican_linkclass-2.1.2.tar` & `pelican_linkclass-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,5 @@
--rw-r--r--   0        0        0      201 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/.editorconfig
--rw-r--r--   0        0        0      736 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1104 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/CHANGELOG.md
--rw-r--r--   0        0        0      562 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       38 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/RELEASE.md
--rw-r--r--   0        0        0      184 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/external-link.png
--rw-r--r--   0        0        0     2585 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/linkclass-example.png
--rw-r--r--   0        0        0     3167 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/tasks.py
--rw-r--r--   0        0        0       82 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/.github/FUNDING.yml
--rw-r--r--   0        0        0     2318 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       39 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/pelican/plugins/linkclass/__init__.py
--rw-r--r--   0        0        0     1790 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/pelican/plugins/linkclass/linkclass.py
--rw-r--r--   0        0        0     3978 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/pelican/plugins/linkclass/mdx_linkclass.py
--rw-r--r--   0        0        0     6981 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/pelican/plugins/linkclass/test_linkclass.py
--rw-r--r--   0        0        0       55 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/.gitignore
--rw-r--r--   0        0        0    34523 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/LICENSE
--rw-r--r--   0        0        0     3902 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/README.md
--rw-r--r--   0        0        0     2671 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     5339 2023-10-31 15:33:56.000000 pelican_linkclass-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/LICENSE
+-rw-r--r--   0        0        0     3902 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/README.md
+-rw-r--r--   0        0        0     2322 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3167 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/tasks.py
+-rw-r--r--   0        0        0     5368 2024-04-07 09:25:50.000000 pelican_linkclass-2.1.3/PKG-INFO
```

### Comparing `pelican_linkclass-2.1.2/tasks.py` & `pelican_linkclass-2.1.3/tasks.py`

 * *Files identical despite different names*

### Comparing `pelican_linkclass-2.1.2/LICENSE` & `pelican_linkclass-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pelican_linkclass-2.1.2/README.md` & `pelican_linkclass-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pelican_linkclass-2.1.2/PKG-INFO` & `pelican_linkclass-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: pelican-linkclass
-Version: 2.1.2
+Version: 2.1.3
 Summary: Pelican plugin to set anchor tag's class attribute to differentiate between internal and external links
-Project-URL: Homepage, https://github.com/pelican-plugins/linkclass
-Project-URL: Issue Tracker, https://github.com/pelican-plugins/linkclass/issues
-Project-URL: Funding, https://donate.getpelican.com/
-Author-email: Rafael Laboissière <rafael@laboissiere.net>
+Keywords: pelican plugin link class
+Author-Email: Rafael Laboissière <rafael@laboissiere.net>
 License: AGPL-3.0
-License-File: LICENSE
-Keywords: link class,pelican,plugin
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: Pelican
 Classifier: Framework :: Pelican :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Homepage, https://github.com/pelican-plugins/linkclass
+Project-URL: Issue tracker, https://github.com/pelican-plugins/linkclass/issues
+Project-URL: Funding, https://donate.getpelican.com/
 Requires-Python: <4.0,>=3.8.1
 Requires-Dist: pelican>=4.5
 Requires-Dist: py3dns>=3.2
+Requires-Dist: markdown>=3.4; extra == "markdown"
 Provides-Extra: markdown
-Requires-Dist: markdown>=3.4; extra == 'markdown'
 Description-Content-Type: text/markdown
 
 Link Class: A Plugin for Pelican
 ================================
 
 [![Build Status](https://img.shields.io/github/actions/workflow/status/pelican-plugins/linkclass/main.yml?branch=main)](https://github.com/pelican-plugins/linkclass/actions)
 [![PyPI Version](https://img.shields.io/pypi/v/pelican-linkclass)](https://pypi.org/project/pelican-linkclass/)
```

