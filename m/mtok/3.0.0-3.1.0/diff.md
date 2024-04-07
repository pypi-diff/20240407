# Comparing `tmp/mtok-3.0.0.tar.gz` & `tmp/mtok-3.1.0.tar.gz`

## Comparing `mtok-3.0.0.tar` & `mtok-3.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-3.0.0/.github/workflows/publish-on-pip.yml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-3.0.0/src/mtok/__init__.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 mtok-3.0.0/src/mtok/helpers.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-3.0.0/src/mtok/mtok.py
--rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mtok-3.0.0/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-3.0.0/README.md
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 mtok-3.1.0/.github/workflows/publish-on-pip.yml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 mtok-3.1.0/src/mtok/__init__.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 mtok-3.1.0/src/mtok/helpers.py
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 mtok-3.1.0/src/mtok/mtok.py
+-rw-r--r--   0        0        0     3538 2020-02-02 00:00:00.000000 mtok-3.1.0/.gitignore
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 mtok-3.1.0/README.md
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 mtok-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 mtok-3.1.0/PKG-INFO
```

### Comparing `mtok-3.0.0/.github/workflows/publish-on-pip.yml` & `mtok-3.1.0/.github/workflows/publish-on-pip.yml`

 * *Files identical despite different names*

### Comparing `mtok-3.0.0/src/mtok/helpers.py` & `mtok-3.1.0/src/mtok/helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import requests
+from os import environ
 
 class Const :
-    # local GitHub token absolute filepath ~/.gt.json
-    lg = '.gt'
-    lg = Path(lg)
+    # local GitHub token absolute filepath $HOME/.gt.json, I assume it is in the home directory
+    lg = Path(environ['HOME']) / '.gt'
     # GitHub username
     gu = 'imahdimir'
 
 c = Const()
 
 def get_gt() :
     with open(c.lg , 'r') as f :
```

### Comparing `mtok-3.0.0/src/mtok/mtok.py` & `mtok-3.1.0/src/mtok/mtok.py`

 * *Files identical despite different names*

### Comparing `mtok-3.0.0/.gitignore` & `mtok-3.1.0/.gitignore`

 * *Files identical despite different names*

