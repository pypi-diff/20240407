# Comparing `tmp/whylogs_container_types-0.4.15.tar.gz` & `tmp/whylogs_container_types-0.4.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whylogs_container_types-0.4.15.tar", max compression
+gzip compressed data, was "whylogs_container_types-0.4.16.tar", max compression
```

## Comparing `whylogs_container_types-0.4.15.tar` & `whylogs_container_types-0.4.16.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      104 2023-11-29 03:51:56.422148 whylogs_container_types-0.4.15/README.md
--rw-r--r--   0        0        0     1146 2024-04-04 17:26:17.304098 whylogs_container_types-0.4.15/pyproject.toml
--rw-r--r--   0        0        0     1287 2024-04-04 17:16:23.730230 whylogs_container_types-0.4.15/whylogs_container_types/__init__.py
--rw-r--r--   0        0        0      735 1970-01-01 00:00:00.000000 whylogs_container_types-0.4.15/PKG-INFO
+-rw-r--r--   0        0        0      104 2023-11-29 03:51:56.422148 whylogs_container_types-0.4.16/README.md
+-rw-r--r--   0        0        0     1156 2024-04-07 05:51:57.652133 whylogs_container_types-0.4.16/pyproject.toml
+-rw-r--r--   0        0        0     1287 2024-04-04 17:16:23.730230 whylogs_container_types-0.4.16/whylogs_container_types/__init__.py
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 whylogs_container_types-0.4.16/PKG-INFO
```

### Comparing `whylogs_container_types-0.4.15/pyproject.toml` & `whylogs_container_types-0.4.16/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "whylogs-container-types"
-version = "0.4.15"
+version = "0.4.16"
 description = ""
 authors = ["Anthony Naddeo <anthony@whylabs.ai>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "whylogs_container_types/**/*.py" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 whylogs = "*"
-langkit = "0.0.28.dev0"
+langkit = ">=0.0.28.dev0,<0.0.29"
 
 
 [tool.poetry.group.dev.dependencies]
 pyright = "^1.1.337"
 ruff = "^0.1.13"
 
 [build-system]
```

### Comparing `whylogs_container_types-0.4.15/whylogs_container_types/__init__.py` & `whylogs_container_types-0.4.16/whylogs_container_types/__init__.py`

 * *Files identical despite different names*

### Comparing `whylogs_container_types-0.4.15/PKG-INFO` & `whylogs_container_types-0.4.16/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: whylogs-container-types
-Version: 0.4.15
+Version: 0.4.16
 Summary: 
 License: MIT
 Author: Anthony Naddeo
 Author-email: anthony@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langkit (==0.0.28.dev0)
+Requires-Dist: langkit (==0.0.28.*)
 Requires-Dist: whylogs
 Description-Content-Type: text/markdown
 
 
 This packages contains various types that are used for customizing the whylogs python container. 
 
 TBD
```

