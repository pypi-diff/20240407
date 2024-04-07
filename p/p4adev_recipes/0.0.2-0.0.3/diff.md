# Comparing `tmp/p4adev_recipes-0.0.2.tar.gz` & `tmp/p4adev_recipes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p4adev_recipes-0.0.2.tar", max compression
+gzip compressed data, was "p4adev_recipes-0.0.3.tar", max compression
```

## Comparing `p4adev_recipes-0.0.2.tar` & `p4adev_recipes-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1804 2024-04-05 17:52:03.839984 p4adev_recipes-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 16:10:57.050848 p4adev_recipes-0.0.2/src/p4adev_recipes/__init__.py
--rw-r--r--   0        0        0     2654 2024-03-29 20:54:49.914404 p4adev_recipes-0.0.2/src/p4adev_recipes/bundle_installer.py
--rw-r--r--   0        0        0      231 2024-03-24 15:26:55.856462 p4adev_recipes-0.0.2/src/p4adev_recipes/recipe/__init__.py
--rw-r--r--   0        0        0     1722 2024-03-24 15:44:26.145401 p4adev_recipes-0.0.2/src/p4adev_recipes/recipe/adv_cc_recipe.py
--rw-r--r--   0        0        0     3092 2024-04-05 16:14:35.253853 p4adev_recipes-0.0.2/src/p4adev_recipes/recipe/build_tool_recipe.py
--rw-r--r--   0        0        0     1802 2024-04-05 16:14:29.457853 p4adev_recipes-0.0.2/src/p4adev_recipes/recipe/no_setup_pypi_recipe.py
--rw-r--r--   0        0        0      496 1970-01-01 00:00:00.000000 p4adev_recipes-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11324 2024-04-07 18:46:04.204843 p4adev_recipes-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2116 2024-04-07 18:51:21.139825 p4adev_recipes-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 16:10:57.050848 p4adev_recipes-0.0.3/src/p4adev_recipes/__init__.py
+-rw-r--r--   0        0        0     2654 2024-03-29 20:54:49.914404 p4adev_recipes-0.0.3/src/p4adev_recipes/bundle_installer.py
+-rw-r--r--   0        0        0      231 2024-03-24 15:26:55.856462 p4adev_recipes-0.0.3/src/p4adev_recipes/recipe/__init__.py
+-rw-r--r--   0        0        0     1722 2024-03-24 15:44:26.145401 p4adev_recipes-0.0.3/src/p4adev_recipes/recipe/adv_cc_recipe.py
+-rw-r--r--   0        0        0     3092 2024-04-05 16:14:35.253853 p4adev_recipes-0.0.3/src/p4adev_recipes/recipe/build_tool_recipe.py
+-rw-r--r--   0        0        0     1802 2024-04-05 16:14:29.457853 p4adev_recipes-0.0.3/src/p4adev_recipes/recipe/no_setup_pypi_recipe.py
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 p4adev_recipes-0.0.3/PKG-INFO
```

### Comparing `p4adev_recipes-0.0.2/pyproject.toml` & `p4adev_recipes-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 [tool.poetry]
 name = "p4adev_recipes"
-version = "0.0.2"
-description = "Some advanced recipes bases for python-for-android."
+version = "0.0.3"
+description = "Some advanced recipes bases for python-for-android projects."
 authors = ["BlackCatDevel0per <bcdev@mail.ru>"]
+license = "Apache 2.0"
+
+packages = [
+    { include = "p4adev_recipes", from = "src" }
+]
+
+[tool.poetry.urls]
+Homepage = "https://github.com/BlackCatDevel0per/p4adev_recipes"
+Depository = "https://github.com/BlackCatDevel0per/p4adev_recipes"
+Repository = "https://github.com/BlackCatDevel0per/p4adev_recipes"
 
 [tool.ruff]
 line-length = 100
 select = [
 	"RUF",
 	"FBT",
 	"FURB",
@@ -105,16 +115,16 @@
 [tool.poetry.group.recommends]
 optional = true
 
 [tool.poetry.group.recommends.dependencies]
 python-for-android = {url = "https://github.com/BlackCatDevel0per/python-for-android/archive/refs/heads/master.zip"}
 sh = ">=1.10,<2.0"
 
-# [tool.poetry.group.dev]
-# optional = true
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.2"
 pytest-dependency = "^0.5.1"
 ruff = "^0.0.292"
 ipykernel = "^6.29.4"
 ipython = "8.12.3"
```

### Comparing `p4adev_recipes-0.0.2/src/p4adev_recipes/bundle_installer.py` & `p4adev_recipes-0.0.3/src/p4adev_recipes/bundle_installer.py`

 * *Files identical despite different names*

### Comparing `p4adev_recipes-0.0.2/src/p4adev_recipes/recipe/adv_cc_recipe.py` & `p4adev_recipes-0.0.3/src/p4adev_recipes/recipe/adv_cc_recipe.py`

 * *Files identical despite different names*

### Comparing `p4adev_recipes-0.0.2/src/p4adev_recipes/recipe/build_tool_recipe.py` & `p4adev_recipes-0.0.3/src/p4adev_recipes/recipe/build_tool_recipe.py`

 * *Files identical despite different names*

### Comparing `p4adev_recipes-0.0.2/src/p4adev_recipes/recipe/no_setup_pypi_recipe.py` & `p4adev_recipes-0.0.3/src/p4adev_recipes/recipe/no_setup_pypi_recipe.py`

 * *Files identical despite different names*

