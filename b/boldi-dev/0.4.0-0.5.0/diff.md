# Comparing `tmp/boldi_dev-0.4.0.tar.gz` & `tmp/boldi_dev-0.5.0.tar.gz`

## Comparing `boldi_dev-0.4.0.tar` & `boldi_dev-0.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/boldi/_dev_version.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/boldi/dev/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/boldi/dev/cli.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/boldi/dev/docs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/boldi/dev/lint.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/boldi/dev/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/boldi/dev/test.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/.gitignore
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/../../README.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 boldi_dev-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/boldi/_dev_version.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/boldi/dev/__init__.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/boldi/dev/cli.py
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/boldi/dev/docs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/boldi/dev/lint.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/boldi/dev/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/boldi/dev/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/.gitignore
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/../../README.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 boldi_dev-0.5.0/PKG-INFO
```

### Comparing `boldi_dev-0.4.0/boldi/dev/cli.py` & `boldi_dev-0.5.0/boldi/dev/cli.py`

 * *Files identical despite different names*

### Comparing `boldi_dev-0.4.0/boldi/dev/package.py` & `boldi_dev-0.5.0/boldi/dev/package.py`

 * *Files identical despite different names*

### Comparing `boldi_dev-0.4.0/pyproject.toml` & `boldi_dev-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boldi_dev-0.4.0/../../README.md` & `boldi_dev-0.5.0/../../README.md`

 * *Files identical despite different names*

### Comparing `boldi_dev-0.4.0/PKG-INFO` & `boldi_dev-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: boldi-dev
-Version: 0.4.0
+Version: 0.5.0
 Summary: boldi.dev part of Boldi's Python libraries
 Author-email: Boldizsár Palotás <boldizsar.palotas@gmail.com>
 License: MIT
 Requires-Python: >=3.9
-Requires-Dist: boldi-cli==0.4.0
-Requires-Dist: boldi-ctx==0.4.0
+Requires-Dist: boldi-cli==0.5.0
+Requires-Dist: boldi-ctx==0.5.0
 Requires-Dist: mdx-truly-sane-lists
 Requires-Dist: mkdocs-autorefs
 Requires-Dist: mkdocs-material
 Requires-Dist: mkdocstrings[python]
 Requires-Dist: mypy
 Requires-Dist: ruff
 Description-Content-Type: text/markdown
```

