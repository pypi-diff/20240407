# Comparing `tmp/mahdi_env-1.0.1.tar.gz` & `tmp/mahdi_env-2.0.0.tar.gz`

## Comparing `mahdi_env-1.0.1.tar` & `mahdi_env-2.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/.gitattributes
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/src/mahdi_env/__init__.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/src/mahdi_env/env.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/.gitignore
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/README.md
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mahdi_env-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/.gitattributes
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/src/mahdi_env/__init__.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/src/mahdi_env/env.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/.gitignore
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/README.md
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mahdi_env-2.0.0/PKG-INFO
```

### Comparing `mahdi_env-1.0.1/.github/workflows/python-publish.yml` & `mahdi_env-2.0.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `mahdi_env-1.0.1/src/mahdi_env/env.py` & `mahdi_env-2.0.0/src/mahdi_env/env.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 """
+
     Loads the environment variables from the .export file if
         - The DB environment variable is not set that means either:
             - I am running in the console
             - or other user than me is running the script.
+
     """
 
 import subprocess
 from os import environ
 from pathlib import Path
 
 class ENVDict(dict) :
-    """ This calss is a subclass of dict that returns a default value of
-    empty string when the key is not present, this is useful when the ENV
-    is not defined so the programm doesn't crash.
+    """
+
+    This calss is a subclass of dict that returns a default value of
+    empty string when the key is not present.
+    This is useful when the ENV is not defined so the programm doesn't crash.
+    like when there is no access to the .export file. (like another user is running the script)
+    or when some environment variables are not set in the current machine but are set in another machine. (like Genomics server) but not on the local machine.
+
     """
 
     def __getitem__(self , key , default = '') :
         return super().__getitem__(key) if key in self else default
 
 def get_env() -> ENVDict :
-    """ Reads the environment variables from the .export file and returns them """
-    if 'DB' in environ :
-        return ENVDict(environ)
+    """
+
+    Reads the environment variables from the .export file and returns them
+
+    """
 
     fn = Path(f"{environ['HOME']}/.export")
     if not fn.exists() :
         fn = Path('/homes/nber/mahdimir/.export')
 
+    if not fn.exists() :
+        return ENVDict(environ)
+
     with open(fn) as f :
         script = f.read()
+
     script = script.encode() + b'\nenv'
 
-    with subprocess.Popen(['sh'] ,
-                          stdin = subprocess.PIPE ,
-                          stdout = subprocess.PIPE) as p :
+    _sp = subprocess.PIPE
+    with subprocess.Popen(['sh'] , stdin = _sp , stdout = _sp) as p :
         result = p.communicate(script)
 
     for line in result[0].decode().splitlines() :
         var , _ , value = line.partition('=')
         environ[var] = value
 
-    if not 'DB' in environ :
-        raise Exception('DB is not set in environment variables.')
-
     return ENVDict(environ)
```

### Comparing `mahdi_env-1.0.1/.gitignore` & `mahdi_env-2.0.0/.gitignore`

 * *Files identical despite different names*

