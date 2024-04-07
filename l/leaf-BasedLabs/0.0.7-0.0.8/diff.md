# Comparing `tmp/leaf_BasedLabs-0.0.7.tar.gz` & `tmp/leaf_BasedLabs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leaf_BasedLabs-0.0.7.tar", last modified: Wed Apr  3 22:16:16 2024, max compression
+gzip compressed data, was "leaf_BasedLabs-0.0.8.tar", last modified: Sun Apr  7 11:29:20 2024, max compression
```

## Comparing `leaf_BasedLabs-0.0.7.tar` & `leaf_BasedLabs-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-03 22:16:16.124746 leaf_BasedLabs-0.0.7/
--rw-rw-r--   0 jt        (1000) jt        (1000)    11357 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.7/LICENSE
--rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-03 22:16:16.124746 leaf_BasedLabs-0.0.7/PKG-INFO
--rw-rw-r--   0 jt        (1000) jt        (1000)     1442 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.7/README.md
--rw-rw-r--   0 jt        (1000) jt        (1000)      526 2024-04-03 22:11:05.000000 leaf_BasedLabs-0.0.7/pyproject.toml
--rw-rw-r--   0 jt        (1000) jt        (1000)       38 2024-04-03 22:16:16.124746 leaf_BasedLabs-0.0.7/setup.cfg
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-03 22:16:16.124746 leaf_BasedLabs-0.0.7/src/
--rw-rw-r--   0 jt        (1000) jt        (1000)        0 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.7/src/__init__.py
--rw-rw-r--   0 jt        (1000) jt        (1000)     1331 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.7/src/example.py
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-03 22:16:16.124746 leaf_BasedLabs-0.0.7/src/leaf/
--rw-rw-r--   0 jt        (1000) jt        (1000)       63 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.7/src/leaf/__init__.py
--rw-rw-r--   0 jt        (1000) jt        (1000)      471 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.7/src/leaf/exception.py
--rw-rw-r--   0 jt        (1000) jt        (1000)     9266 2024-04-03 22:08:38.000000 leaf_BasedLabs-0.0.7/src/leaf/filesystem.py
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-03 22:16:16.124746 leaf_BasedLabs-0.0.7/src/leaf_BasedLabs.egg-info/
--rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-03 22:16:16.000000 leaf_BasedLabs-0.0.7/src/leaf_BasedLabs.egg-info/PKG-INFO
--rw-rw-r--   0 jt        (1000) jt        (1000)      316 2024-04-03 22:16:16.000000 leaf_BasedLabs-0.0.7/src/leaf_BasedLabs.egg-info/SOURCES.txt
--rw-rw-r--   0 jt        (1000) jt        (1000)        1 2024-04-03 22:16:16.000000 leaf_BasedLabs-0.0.7/src/leaf_BasedLabs.egg-info/dependency_links.txt
--rw-rw-r--   0 jt        (1000) jt        (1000)       28 2024-04-03 22:16:16.000000 leaf_BasedLabs-0.0.7/src/leaf_BasedLabs.egg-info/top_level.txt
-drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-03 22:16:16.124746 leaf_BasedLabs-0.0.7/src/tests/
--rw-rw-r--   0 jt        (1000) jt        (1000)     3602 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.7/src/tests/tests.py
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/
+-rw-rw-r--   0 jt        (1000) jt        (1000)    11357 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/LICENSE
+-rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/PKG-INFO
+-rw-rw-r--   0 jt        (1000) jt        (1000)     1442 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/README.md
+-rw-rw-r--   0 jt        (1000) jt        (1000)      526 2024-04-07 11:29:15.000000 leaf_BasedLabs-0.0.8/pyproject.toml
+-rw-rw-r--   0 jt        (1000) jt        (1000)       38 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/setup.cfg
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.194776 leaf_BasedLabs-0.0.8/src/
+-rw-rw-r--   0 jt        (1000) jt        (1000)        0 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/__init__.py
+-rw-rw-r--   0 jt        (1000) jt        (1000)     1331 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/example.py
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/src/leaf/
+-rw-rw-r--   0 jt        (1000) jt        (1000)       63 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/leaf/__init__.py
+-rw-rw-r--   0 jt        (1000) jt        (1000)      471 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/leaf/exception.py
+-rw-rw-r--   0 jt        (1000) jt        (1000)     9355 2024-04-07 11:28:44.000000 leaf_BasedLabs-0.0.8/src/leaf/filesystem.py
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/
+-rw-r--r--   0 jt        (1000) jt        (1000)     1987 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/PKG-INFO
+-rw-rw-r--   0 jt        (1000) jt        (1000)      316 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/SOURCES.txt
+-rw-rw-r--   0 jt        (1000) jt        (1000)        1 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/dependency_links.txt
+-rw-rw-r--   0 jt        (1000) jt        (1000)       28 2024-04-07 11:29:20.000000 leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/top_level.txt
+drwxrwxr-x   0 jt        (1000) jt        (1000)        0 2024-04-07 11:29:20.198776 leaf_BasedLabs-0.0.8/src/tests/
+-rw-rw-r--   0 jt        (1000) jt        (1000)     3602 2024-04-03 22:08:11.000000 leaf_BasedLabs-0.0.8/src/tests/tests.py
```

### Comparing `leaf_BasedLabs-0.0.7/LICENSE` & `leaf_BasedLabs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `leaf_BasedLabs-0.0.7/PKG-INFO` & `leaf_BasedLabs-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaf_BasedLabs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Leaf is a small (just two .py files) on-demand hierachical filesystem database.
 Author-email: Igor Bruev <jaktenstid1@gmail.com>
 Project-URL: Homepage, https://github.com/BasedLabs/leaf
 Project-URL: Issues, https://github.com/BasedLabs/leaf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leaf_BasedLabs-0.0.7/README.md` & `leaf_BasedLabs-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `leaf_BasedLabs-0.0.7/pyproject.toml` & `leaf_BasedLabs-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "leaf_BasedLabs"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Igor Bruev", email="jaktenstid1@gmail.com" },
 ]
 description = "Leaf is a small (just two .py files) on-demand hierachical filesystem database."
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `leaf_BasedLabs-0.0.7/src/example.py` & `leaf_BasedLabs-0.0.8/src/example.py`

 * *Files identical despite different names*

### Comparing `leaf_BasedLabs-0.0.7/src/leaf/filesystem.py` & `leaf_BasedLabs-0.0.8/src/leaf/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,18 @@
 
     def read_string(self) -> str:
         self._ensure_exists()
 
         with open(self.full_path, "r") as f:
             return f.read()
 
+    @property
+    def size(self) -> int:
+        return os.stat(self.full_path).st_size
+
     def read_lines(self) -> List[str]:
         self._ensure_exists()
 
         with open(self.full_path, "r") as f:
             return f.readlines()
 
     def read_bytes(self) -> bytes:
```

### Comparing `leaf_BasedLabs-0.0.7/src/leaf_BasedLabs.egg-info/PKG-INFO` & `leaf_BasedLabs-0.0.8/src/leaf_BasedLabs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leaf_BasedLabs
-Version: 0.0.7
+Version: 0.0.8
 Summary: Leaf is a small (just two .py files) on-demand hierachical filesystem database.
 Author-email: Igor Bruev <jaktenstid1@gmail.com>
 Project-URL: Homepage, https://github.com/BasedLabs/leaf
 Project-URL: Issues, https://github.com/BasedLabs/leaf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `leaf_BasedLabs-0.0.7/src/tests/tests.py` & `leaf_BasedLabs-0.0.8/src/tests/tests.py`

 * *Files identical despite different names*

