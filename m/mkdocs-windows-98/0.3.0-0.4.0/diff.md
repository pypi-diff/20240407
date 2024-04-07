# Comparing `tmp/mkdocs-windows-98-0.3.0.tar.gz` & `tmp/mkdocs-windows-98-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-windows-98-0.3.0.tar", last modified: Fri Apr  5 19:06:12 2024, max compression
+gzip compressed data, was "mkdocs-windows-98-0.4.0.tar", last modified: Sun Apr  7 10:34:07 2024, max compression
```

## Comparing `mkdocs-windows-98-0.3.0.tar` & `mkdocs-windows-98-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:06:12.692742 mkdocs-windows-98-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-05 19:05:58.000000 mkdocs-windows-98-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-05 19:06:12.692742 mkdocs-windows-98-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-05 19:05:58.000000 mkdocs-windows-98-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 19:05:58.000000 mkdocs-windows-98-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 19:06:12.692742 mkdocs-windows-98-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:06:12.692742 mkdocs-windows-98-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:06:12.692742 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 19:05:58.000000 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 19:06:12.692742 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-05 19:06:12.000000 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-05 19:06:12.000000 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 19:06:12.000000 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-05 19:06:12.000000 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 19:06:12.000000 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 19:06:12.000000 mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:33:41.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:34:07.777280 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-07 10:34:07.000000 mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/top_level.txt
```

### Comparing `mkdocs-windows-98-0.3.0/LICENSE` & `mkdocs-windows-98-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.3.0/PKG-INFO` & `mkdocs-windows-98-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.3.0
+Version: 0.4.0
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `mkdocs-windows-98-0.3.0/README.md` & `mkdocs-windows-98-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-windows-98-0.3.0/pyproject.toml` & `mkdocs-windows-98-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-windows-98"
-version = "0.3.0"
+version = "0.4.0"
 description = "Windows 98 MkDocs Theme"
 readme = "README.md"
 authors = [
   {name = "Useless DevLab", email = "useless.devlab@gmail.com"}
 ]
 requires-python = ">=3.9"
```

### Comparing `mkdocs-windows-98-0.3.0/src/mkdocs_windows_98.egg-info/PKG-INFO` & `mkdocs-windows-98-0.4.0/src/mkdocs_windows_98.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-windows-98
-Version: 0.3.0
+Version: 0.4.0
 Summary: Windows 98 MkDocs Theme
 Author-email: Useless DevLab <useless.devlab@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

