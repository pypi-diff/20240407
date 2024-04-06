# Comparing `tmp/sprocketship-0.1.2.tar.gz` & `tmp/sprocketship-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sprocketship-0.1.2.tar", last modified: Sat Apr  6 18:04:53 2024, max compression
+gzip compressed data, was "sprocketship-0.1.3.tar", last modified: Sat Apr  6 20:07:15 2024, max compression
```

## Comparing `sprocketship-0.1.2.tar` & `sprocketship-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:53.331671 sprocketship-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 18:04:41.000000 sprocketship-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 18:04:41.000000 sprocketship-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 18:04:53.331671 sprocketship-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-06 18:04:41.000000 sprocketship-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 18:04:41.000000 sprocketship-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:04:53.331671 sprocketship-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:53.327671 sprocketship-0.1.2/sprocketship/
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 18:04:41.000000 sprocketship-0.1.2/sprocketship/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:53.331671 sprocketship-0.1.2/sprocketship/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-06 18:04:41.000000 sprocketship-0.1.2/sprocketship/templates/javascript.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:53.331671 sprocketship-0.1.2/sprocketship.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 18:04:53.000000 sprocketship-0.1.2/sprocketship.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 18:04:53.000000 sprocketship-0.1.2/sprocketship.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:04:53.000000 sprocketship-0.1.2/sprocketship.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 18:04:53.000000 sprocketship-0.1.2/sprocketship.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 18:04:53.000000 sprocketship-0.1.2/sprocketship.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 18:04:53.000000 sprocketship-0.1.2/sprocketship.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-06 20:07:10.000000 sprocketship-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 20:07:10.000000 sprocketship-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 20:07:15.364867 sprocketship-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-06 20:07:10.000000 sprocketship-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-06 20:07:10.000000 sprocketship-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:07:15.364867 sprocketship-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/sprocketship/
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-04-06 20:07:10.000000 sprocketship-0.1.3/sprocketship/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/sprocketship/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-06 20:07:10.000000 sprocketship-0.1.3/sprocketship/templates/javascript.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:07:15.364867 sprocketship-0.1.3/sprocketship.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6838 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 20:07:15.000000 sprocketship-0.1.3/sprocketship.egg-info/top_level.txt
```

### Comparing `sprocketship-0.1.2/LICENSE` & `sprocketship-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.2/PKG-INFO` & `sprocketship-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.2
+Version: 0.1.3
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.2 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.3 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

### Comparing `sprocketship-0.1.2/README.md` & `sprocketship-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.2/pyproject.toml` & `sprocketship-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sprocketship"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Nicklaus Roacb", email="nicklausroach@gmail.com" },
 ]
 readme = "README.md"
 description = "Better stored procedure management"
 dependencies = [
     "click",
```

### Comparing `sprocketship-0.1.2/sprocketship/cli.py` & `sprocketship-0.1.3/sprocketship/cli.py`

 * *Files identical despite different names*

### Comparing `sprocketship-0.1.2/sprocketship.egg-info/PKG-INFO` & `sprocketship-0.1.3/sprocketship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sprocketship
-Version: 0.1.2
+Version: 0.1.3
 Summary: Better stored procedure management
 Author-email: Nicklaus Roacb <nicklausroach@gmail.com>
 Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: sprocketship Version: 0.1.2 Summary: Better stored
+Metadata-Version: 2.1 Name: sprocketship Version: 0.1.3 Summary: Better stored
 procedure management Author-email: Nicklaus Roacb
 gmail.com> Project-URL: Homepage, https://github.com/nicklausroach/sprocketship
 Project-URL: Issues, https://github.com/pypa/nicklausroach/sprocketship
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 click Requires-Dist: snowflake Requires-Dist: ABSQL Requires-Dist: ruamel.yaml
```

