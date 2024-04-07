# Comparing `tmp/multigit_lib-0.0.1-py3-none-any.whl.zip` & `tmp/multigit_lib-0.0.1.post1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 14066 bytes, number of entries: 6
+Zip file size: 14174 bytes, number of entries: 6
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 multigitlib/__init__.py
--rw-r--r--  2.0 unx      169 b- defN 20-Feb-02 00:00 multigitlib/__main__.py
-?rw-r--r--  2.0 unx      982 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      480 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.dist-info/RECORD
-6 files, 36891 bytes uncompressed, 13194 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx      251 b- defN 20-Feb-02 00:00 multigitlib/__main__.py
+?rw-r--r--  2.0 unx      988 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.post1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.post1.dist-info/WHEEL
+?rw-r--r--  2.0 unx    35149 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.post1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      504 b- defN 20-Feb-02 00:00 multigit_lib-0.0.1.post1.dist-info/RECORD
+6 files, 37003 bytes uncompressed, 13254 bytes compressed:  64.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: multigitlib/__init__.py
 Comment: 
 
 Filename: multigitlib/__main__.py
 Comment: 
 
-Filename: multigit_lib-0.0.1.dist-info/METADATA
+Filename: multigit_lib-0.0.1.post1.dist-info/METADATA
 Comment: 
 
-Filename: multigit_lib-0.0.1.dist-info/WHEEL
+Filename: multigit_lib-0.0.1.post1.dist-info/WHEEL
 Comment: 
 
-Filename: multigit_lib-0.0.1.dist-info/licenses/LICENSE
+Filename: multigit_lib-0.0.1.post1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: multigit_lib-0.0.1.dist-info/RECORD
+Filename: multigit_lib-0.0.1.post1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## multigitlib/__main__.py

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*-
 
-__version__ = '0.0.1'
+# See https://packaging.python.org/en/latest/specifications/version-specifiers
+__version__ = '0.0.1-1'
 
 # Import stuff
 import sys
 
 def main():
-	print('RUNNING MULTIGITLIB')
+	print('RUNNING MULTIGIT LIB')
 
 
 if __name__ == '__main__':
 	sys.exit(
 		main()
 	)
```

## Comparing `multigit_lib-0.0.1.dist-info/METADATA` & `multigit_lib-0.0.1.post1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: multigit.lib
-Version: 0.0.1
+Version: 0.0.1.post1
 Summary: Library to manage git repos within git repos.
 Author-email: "Jesús M. Navarro" <jesusmnavarrolopez@gmail.com>
 License: GPL-3.0
 License-File: LICENSE
 Keywords: Python,git-utilities
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

## Comparing `multigit_lib-0.0.1.dist-info/licenses/LICENSE` & `multigit_lib-0.0.1.post1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

