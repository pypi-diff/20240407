# Comparing `tmp/boldi_cli-0.4.0.tar.gz` & `tmp/boldi_cli-0.5.0.tar.gz`

## Comparing `boldi_cli-0.4.0.tar` & `boldi_cli-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_cli-0.4.0/boldi/_cli_version.py
--rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 boldi_cli-0.4.0/boldi/cli.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_cli-0.4.0/.gitignore
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 boldi_cli-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_cli-0.4.0/../../README.md
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 boldi_cli-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_cli-0.5.0/boldi/_cli_version.py
+-rw-r--r--   0        0        0     2867 2020-02-02 00:00:00.000000 boldi_cli-0.5.0/boldi/cli.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_cli-0.5.0/.gitignore
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 boldi_cli-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_cli-0.5.0/../../README.md
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 boldi_cli-0.5.0/PKG-INFO
```

### Comparing `boldi_cli-0.4.0/boldi/cli.py` & `boldi_cli-0.5.0/boldi/cli.py`

 * *Files identical despite different names*

### Comparing `boldi_cli-0.4.0/pyproject.toml` & `boldi_cli-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boldi_cli-0.4.0/../../README.md` & `boldi_cli-0.5.0/../../README.md`

 * *Files identical despite different names*

### Comparing `boldi_cli-0.4.0/PKG-INFO` & `boldi_cli-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: boldi-cli
-Version: 0.4.0
+Version: 0.5.0
 Summary: boldi.cli part of Boldi's Python libraries
 Author-email: Boldizsár Palotás <boldizsar.palotas@gmail.com>
 License: MIT
 Requires-Python: >=3.9
-Requires-Dist: boldi-ctx==0.4.0
+Requires-Dist: boldi-ctx==0.5.0
 Requires-Dist: rich
 Description-Content-Type: text/markdown
 
 # Boldi's Python Libraries
 
 These are Boldi's personal Python libraries.
```

