# Comparing `tmp/mkdocs-nbconvert-0.2.2.tar.gz` & `tmp/mkdocs-nbconvert-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-nbconvert-0.2.2.tar", last modified: Mon Mar 11 10:34:05 2024, max compression
+gzip compressed data, was "mkdocs-nbconvert-0.3.tar", last modified: Sun Apr  7 08:55:04 2024, max compression
```

## Comparing `mkdocs-nbconvert-0.2.2.tar` & `mkdocs-nbconvert-0.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 10:34:05.478945 mkdocs-nbconvert-0.2.2/
--rw-rw-rw-   0        0        0      183 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.2.2/AUTHORS.md
--rw-rw-rw-   0        0        0     1049 2024-03-11 10:26:49.000000 mkdocs-nbconvert-0.2.2/CHANGELOG.md
--rw-rw-rw-   0        0        0       15 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.2.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0     1295 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.2.2/LICENSE
--rw-rw-rw-   0        0        0      127 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1808 2024-03-11 10:34:05.475942 mkdocs-nbconvert-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      844 2024-03-11 10:26:32.000000 mkdocs-nbconvert-0.2.2/README.md
--rw-rw-rw-   0        0        0     1349 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0      343 2024-03-11 10:26:32.000000 mkdocs-nbconvert-0.2.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-03-11 10:34:05.479943 mkdocs-nbconvert-0.2.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-11 10:34:05.367087 mkdocs-nbconvert-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-11 10:34:05.407564 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert/
--rw-rw-rw-   0        0        0       88 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert/__init__.py
--rw-rw-rw-   0        0        0     6924 2024-03-11 10:26:32.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert/plugin.py
--rw-rw-rw-   0        0        0      427 2024-03-11 10:34:03.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert/version.py
-drwxrwxrwx   0        0        0        0 2024-03-11 10:34:05.472941 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/
--rw-rw-rw-   0        0        0     1808 2024-03-11 10:34:04.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2024-03-11 10:34:05.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 10:34:04.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-03-11 10:34:04.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       27 2024-03-11 10:34:04.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-03-11 10:34:04.000000 mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 08:55:04.435161 mkdocs-nbconvert-0.3/
+-rw-rw-rw-   0        0        0      183 2024-04-07 04:31:07.000000 mkdocs-nbconvert-0.3/AUTHORS.md
+-rw-rw-rw-   0        0        0     1148 2024-04-07 04:46:51.000000 mkdocs-nbconvert-0.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0       15 2024-04-07 04:31:10.000000 mkdocs-nbconvert-0.3/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0     1295 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.3/LICENSE
+-rw-rw-rw-   0        0        0      127 2024-03-11 09:13:40.000000 mkdocs-nbconvert-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2154 2024-04-07 08:55:04.432161 mkdocs-nbconvert-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      844 2024-03-11 10:26:32.000000 mkdocs-nbconvert-0.3/README.md
+-rw-rw-rw-   0        0        0     1876 2024-04-07 04:46:04.000000 mkdocs-nbconvert-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      343 2024-03-11 10:26:32.000000 mkdocs-nbconvert-0.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 08:55:04.436162 mkdocs-nbconvert-0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 08:55:04.318610 mkdocs-nbconvert-0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 08:55:04.381458 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert/
+-rw-rw-rw-   0        0        0       12 2024-04-07 04:46:04.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert/.gitignore
+-rw-rw-rw-   0        0        0       75 2024-04-07 04:46:04.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert/__init__.py
+-rw-rw-rw-   0        0        0      422 2024-04-07 08:55:02.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert/_version.py
+-rw-rw-rw-   0        0        0     6924 2024-04-07 04:30:36.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert/plugin.py
+drwxrwxrwx   0        0        0        0 2024-04-07 08:55:04.430161 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/
+-rw-rw-rw-   0        0        0     2154 2024-04-07 08:55:03.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2024-04-07 08:55:04.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 08:55:03.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-07 08:55:03.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       27 2024-04-07 08:55:03.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-07 08:55:03.000000 mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/top_level.txt
```

### Comparing `mkdocs-nbconvert-0.2.2/CHANGELOG.md` & `mkdocs-nbconvert-0.3/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # CHANGELOG
 
+## v0.3
+
+> 📅 **Date** 2024-4-7
+
+Mark the package's Development Status to 5 - Production/Stable
+
 ## v0.2.2
 
 > 📅 **Date** 2024-3-11
 
 Update dependencies and tools to latest version.
 
 ## v0.2.1
```

### Comparing `mkdocs-nbconvert-0.2.2/LICENSE` & `mkdocs-nbconvert-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-nbconvert-0.2.2/PKG-INFO` & `mkdocs-nbconvert-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: mkdocs-nbconvert
-Version: 0.2.2
+Version: 0.3
 Summary: A MkDocs plug-in provides a source parser for *.ipynb Jupyter notebook files, base on nbconvert.
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://tanbro.github.io/mkdocs-nbconvert
 Project-URL: Repository, https://github.com/tanbro/mkdocs-nbconvert
 Project-URL: Documentation, https://tanbro.github.io/mkdocs-nbconvert
 Keywords: mkdocs,mkdocs-plugin,jupyter,notebook,jupyter-notebook,markdown,md,nbconvert
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Documentation
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: mkdocs>=1.4
 Requires-Dist: nbconvert>=4.2
 
 # mkdocs-nbconvert
```

### Comparing `mkdocs-nbconvert-0.2.2/README.md` & `mkdocs-nbconvert-0.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert/plugin.py` & `mkdocs-nbconvert-0.3/src/mkdocs_nbconvert/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-nbconvert-0.2.2/src/mkdocs_nbconvert.egg-info/PKG-INFO` & `mkdocs-nbconvert-0.3/src/mkdocs_nbconvert.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: mkdocs-nbconvert
-Version: 0.2.2
+Version: 0.3
 Summary: A MkDocs plug-in provides a source parser for *.ipynb Jupyter notebook files, base on nbconvert.
 Author-email: liu xue yan <liu_xue_yan@foxmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://tanbro.github.io/mkdocs-nbconvert
 Project-URL: Repository, https://github.com/tanbro/mkdocs-nbconvert
 Project-URL: Documentation, https://tanbro.github.io/mkdocs-nbconvert
 Keywords: mkdocs,mkdocs-plugin,jupyter,notebook,jupyter-notebook,markdown,md,nbconvert
 Classifier: License :: OSI Approved :: BSD License
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Documentation
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: mkdocs>=1.4
 Requires-Dist: nbconvert>=4.2
 
 # mkdocs-nbconvert
```

