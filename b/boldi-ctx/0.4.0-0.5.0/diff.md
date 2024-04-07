# Comparing `tmp/boldi_ctx-0.4.0.tar.gz` & `tmp/boldi_ctx-0.5.0.tar.gz`

## Comparing `boldi_ctx-0.4.0.tar` & `boldi_ctx-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_ctx-0.4.0/boldi/_ctx_version.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 boldi_ctx-0.4.0/boldi/ctx.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_ctx-0.4.0/.gitignore
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 boldi_ctx-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_ctx-0.4.0/../../README.md
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 boldi_ctx-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 boldi_ctx-0.5.0/boldi/_ctx_version.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 boldi_ctx-0.5.0/boldi/ctx.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 boldi_ctx-0.5.0/.gitignore
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 boldi_ctx-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 boldi_ctx-0.5.0/../../README.md
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 boldi_ctx-0.5.0/PKG-INFO
```

### Comparing `boldi_ctx-0.4.0/boldi/ctx.py` & `boldi_ctx-0.5.0/boldi/ctx.py`

 * *Files identical despite different names*

### Comparing `boldi_ctx-0.4.0/pyproject.toml` & `boldi_ctx-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `boldi_ctx-0.4.0/../../README.md` & `boldi_ctx-0.5.0/../../README.md`

 * *Files identical despite different names*

### Comparing `boldi_ctx-0.4.0/PKG-INFO` & `boldi_ctx-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: boldi-ctx
-Version: 0.4.0
+Version: 0.5.0
 Summary: boldi.ctx part of Boldi's Python libraries
 Author-email: Boldizsár Palotás <boldizsar.palotas@gmail.com>
 License: MIT
 Requires-Python: >=3.9
-Requires-Dist: boldi-proc==0.4.0
+Requires-Dist: boldi-proc==0.5.0
 Provides-Extra: dev
 Requires-Dist: typing-extensions; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Boldi's Python Libraries
 
 These are Boldi's personal Python libraries.
```

