# Comparing `tmp/hatch-ci-0.1.4b72.tar.gz` & `tmp/hatch-ci-0.1.4b75.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatch-ci-0.1.4b72.tar", last modified: Fri Apr  5 22:10:05 2024, max compression
+gzip compressed data, was "hatch-ci-0.1.4b75.tar", last modified: Sun Apr  7 18:41:01 2024, max compression
```

## Comparing `hatch-ci-0.1.4b72.tar` & `hatch-ci-0.1.4b75.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:10:05.772301 hatch-ci-0.1.4b72/
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-05 22:10:05.772301 hatch-ci-0.1.4b72/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-05 22:10:03.000000 hatch-ci-0.1.4b72/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 22:10:03.000000 hatch-ci-0.1.4b72/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 22:10:05.772301 hatch-ci-0.1.4b72/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:10:05.768300 hatch-ci-0.1.4b72/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:10:05.772301 hatch-ci-0.1.4b72/src/hatch_ci/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/code.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/hook_build.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/hook_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/hook_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/script.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/text.py
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/src/hatch_ci/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:10:05.772301 hatch-ci-0.1.4b72/src/hatch_ci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-05 22:10:05.000000 hatch-ci-0.1.4b72/src/hatch_ci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-05 22:10:05.000000 hatch-ci-0.1.4b72/src/hatch_ci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 22:10:05.000000 hatch-ci-0.1.4b72/src/hatch_ci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-05 22:10:05.000000 hatch-ci-0.1.4b72/src/hatch_ci.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-05 22:10:05.000000 hatch-ci-0.1.4b72/src/hatch_ci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 22:10:05.000000 hatch-ci-0.1.4b72/src/hatch_ci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 22:10:05.772301 hatch-ci-0.1.4b72/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_fileos.py
--rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_script.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-05 22:09:27.000000 hatch-ci-0.1.4b72/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:41:01.005335 hatch-ci-0.1.4b75/
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-07 18:41:01.005335 hatch-ci-0.1.4b75/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-07 18:40:58.000000 hatch-ci-0.1.4b75/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-07 18:40:58.000000 hatch-ci-0.1.4b75/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 18:41:01.005335 hatch-ci-0.1.4b75/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:41:01.001335 hatch-ci-0.1.4b75/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:41:01.005335 hatch-ci-0.1.4b75/src/hatch_ci/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3889 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2338 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/hook_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/hook_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/hook_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8277 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/src/hatch_ci/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:41:01.005335 hatch-ci-0.1.4b75/src/hatch_ci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-04-07 18:41:00.000000 hatch-ci-0.1.4b75/src/hatch_ci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-07 18:41:00.000000 hatch-ci-0.1.4b75/src/hatch_ci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 18:41:00.000000 hatch-ci-0.1.4b75/src/hatch_ci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-07 18:41:00.000000 hatch-ci-0.1.4b75/src/hatch_ci.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 18:41:00.000000 hatch-ci-0.1.4b75/src/hatch_ci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 18:41:00.000000 hatch-ci-0.1.4b75/src/hatch_ci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 18:41:01.005335 hatch-ci-0.1.4b75/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8318 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_fileos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5871 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9536 2024-04-07 18:40:21.000000 hatch-ci-0.1.4b75/tests/test_tools.py
```

### Comparing `hatch-ci-0.1.4b72/LICENSE.txt` & `hatch-ci-0.1.4b75/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/PKG-INFO` & `hatch-ci-0.1.4b75/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.1.4b72
+Version: 0.1.4b75
 Summary: Hatch plugin for ci system versioning
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Keywords: git,hatch,plugin,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hatch-ci-0.1.4b72/README.md` & `hatch-ci-0.1.4b75/README.md`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/pyproject.toml` & `hatch-ci-0.1.4b75/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-__version__ = "0.1.4b72"
-__hash__ = "1fc37bfa7d6d1b1dcf552564c5a9abd1c74797aa"
+__version__ = "0.1.4b75"
+__hash__ = "a4ff965e8349e70ec79d6abc9a426ca10e8b86b3"
 build-backend = "hatchling.build"
 
 [project]
 name = "hatch-ci"
-version = "0.1.4b72"
+version = "0.1.4b75"
 description = "Hatch plugin for ci system versioning"
 readme = "README.md"
 license = { text = "MIT" }
 requires-python = ">= 3.8"
 keywords = [
   "git",
   "hatch",
```

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/_support.py` & `hatch-ci-0.1.4b75/src/hatch_ci/_support.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/cli.py` & `hatch-ci-0.1.4b75/src/hatch_ci/cli.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/code.py` & `hatch-ci-0.1.4b75/src/hatch_ci/code.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/exceptions.py` & `hatch-ci-0.1.4b75/src/hatch_ci/exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/fileos.py` & `hatch-ci-0.1.4b75/src/hatch_ci/fileos.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/hook_build.py` & `hatch-ci-0.1.4b75/src/hatch_ci/hook_build.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/hook_version.py` & `hatch-ci-0.1.4b75/src/hatch_ci/hook_version.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/scm.py` & `hatch-ci-0.1.4b75/src/hatch_ci/scm.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/script.py` & `hatch-ci-0.1.4b75/src/hatch_ci/script.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/text.py` & `hatch-ci-0.1.4b75/src/hatch_ci/text.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci/tools.py` & `hatch-ci-0.1.4b75/src/hatch_ci/tools.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci.egg-info/PKG-INFO` & `hatch-ci-0.1.4b75/src/hatch_ci.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatch-ci
-Version: 0.1.4b72
+Version: 0.1.4b75
 Summary: Hatch plugin for ci system versioning
 Author-email: Antonio Cavallo <a.cavallo@cavallinux.eu>
 License: MIT
 Project-URL: Issues, https://github.com/cav71/hatch-ci/issues
 Project-URL: Source, https://github.com/cav71/hatch-ci
 Keywords: git,hatch,plugin,scm,version
 Classifier: Development Status :: 4 - Beta
```

### Comparing `hatch-ci-0.1.4b72/src/hatch_ci.egg-info/SOURCES.txt` & `hatch-ci-0.1.4b75/src/hatch_ci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_cli.py` & `hatch-ci-0.1.4b75/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_code.py` & `hatch-ci-0.1.4b75/tests/test_code.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_conftest.py` & `hatch-ci-0.1.4b75/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_e2e.py` & `hatch-ci-0.1.4b75/tests/test_e2e.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_exceptions.py` & `hatch-ci-0.1.4b75/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_fileos.py` & `hatch-ci-0.1.4b75/tests/test_fileos.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_scm.py` & `hatch-ci-0.1.4b75/tests/test_scm.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_script.py` & `hatch-ci-0.1.4b75/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_text.py` & `hatch-ci-0.1.4b75/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `hatch-ci-0.1.4b72/tests/test_tools.py` & `hatch-ci-0.1.4b75/tests/test_tools.py`

 * *Files identical despite different names*

