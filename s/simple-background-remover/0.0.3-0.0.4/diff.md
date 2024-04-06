# Comparing `tmp/simple_background_remover-0.0.3.tar.gz` & `tmp/simple_background_remover-0.0.4.tar.gz`

## Comparing `simple_background_remover-0.0.3.tar` & `simple_background_remover-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/src/simple_background_remover/__init__.py
--rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/src/simple_background_remover/color_helper.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/src/simple_background_remover/simple_background_remover.py
--rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/LICENSE
--rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/README.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 simple_background_remover-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/src/simple_background_remover/__init__.py
+-rw-r--r--   0        0        0     4099 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/src/simple_background_remover/color_helper.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/src/simple_background_remover/simple_background_remover.py
+-rw-r--r--   0        0        0     3115 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2604 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/README.md
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 simple_background_remover-0.0.4/PKG-INFO
```

### Comparing `simple_background_remover-0.0.3/.github/workflows/python-publish.yml` & `simple_background_remover-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.3/src/simple_background_remover/color_helper.py` & `simple_background_remover-0.0.4/src/simple_background_remover/color_helper.py`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.3/src/simple_background_remover/simple_background_remover.py` & `simple_background_remover-0.0.4/src/simple_background_remover/simple_background_remover.py`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.3/.gitignore` & `simple_background_remover-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.3/LICENSE` & `simple_background_remover-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.3/README.md` & `simple_background_remover-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `simple_background_remover-0.0.3/pyproject.toml` & `simple_background_remover-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simple_background_remover"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="oversizedcanoe" },
 ]
 description = "A quick and dirty background remover for simple images with solid(ish) background colors."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `simple_background_remover-0.0.3/PKG-INFO` & `simple_background_remover-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simple_background_remover
-Version: 0.0.3
+Version: 0.0.4
 Summary: A quick and dirty background remover for simple images with solid(ish) background colors.
 Project-URL: Homepage, https://github.com/oversizedcanoe/simple_background_remover 
 Author: oversizedcanoe
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

