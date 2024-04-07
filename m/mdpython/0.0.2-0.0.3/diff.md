# Comparing `tmp/mdpython-0.0.2.tar.gz` & `tmp/mdpython-0.0.3.tar.gz`

## Comparing `mdpython-0.0.2.tar` & `mdpython-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 mdpython-0.0.2/hello_world.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/__init__.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/__init__.py
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/compare.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/compare_dir.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.2/src/mdpython/fileutils/html_template.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 mdpython-0.0.2/README.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 mdpython-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 mdpython-0.0.3/hello_world.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/__init__.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/example.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/fileutils/__init__.py
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/fileutils/compare.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/fileutils/compare_dir.py
+-rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/fileutils/html_template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/uiutils/__init__.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 mdpython-0.0.3/src/mdpython/uiutils/menu_based_app.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 mdpython-0.0.3/README.md
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 mdpython-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 mdpython-0.0.3/PKG-INFO
```

### Comparing `mdpython-0.0.2/src/mdpython/fileutils/compare.py` & `mdpython-0.0.3/src/mdpython/fileutils/compare.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.2/src/mdpython/fileutils/compare_dir.py` & `mdpython-0.0.3/src/mdpython/fileutils/compare_dir.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.2/src/mdpython/fileutils/html_template.py` & `mdpython-0.0.3/src/mdpython/fileutils/html_template.py`

 * *Files identical despite different names*

### Comparing `mdpython-0.0.2/pyproject.toml` & `mdpython-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mdpython"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Dhaval", email="seedhaval@gmail.com" },
 ]
 description = "MD Python Library"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

