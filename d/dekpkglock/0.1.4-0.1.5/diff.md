# Comparing `tmp/dekpkglock-0.1.4.tar.gz` & `tmp/dekpkglock-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dekpkglock-0.1.4.tar", last modified: Sat Apr  6 19:51:19 2024, max compression
+gzip compressed data, was "dekpkglock-0.1.5.tar", last modified: Sat Apr  6 20:04:10 2024, max compression
```

## Comparing `dekpkglock-0.1.4.tar` & `dekpkglock-0.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      123 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/README.md
--rw-r--r--   0        0        0        0 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/__init__.py
--rw-r--r--   0        0        0       42 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/click/__entry__.py
--rw-r--r--   0        0        0      361 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/click/__init__.py
--rw-r--r--   0        0        0      223 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/core/__init__.py
--rw-r--r--   0        0        0     2047 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/core/base/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-06 19:51:18.151023 dekpkglock-0.1.4/dekpkglock/core/pdm.py
--rw-r--r--   0        0        0   140317 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
--rw-r--r--   0        0        0   140317 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock
--rw-r--r--   0        0        0   101191 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock
--rw-r--r--   0        0        0   101213 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock
--rw-r--r--   0        0        0    31259 2024-04-06 19:51:18.155023 dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
--rw-r--r--   0        0        0   123953 2024-04-06 19:51:18.159023 dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
--rw-r--r--   0        0        0      476 2024-04-06 19:51:19.583017 dekpkglock-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      123 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/__init__.py
+-rw-r--r--   0        0        0       42 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/click/__entry__.py
+-rw-r--r--   0        0        0      479 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/click/__init__.py
+-rw-r--r--   0        0        0      244 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/core/__init__.py
+-rw-r--r--   0        0        0     2244 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/core/base/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/core/pdm.py
+-rw-r--r--   0        0        0   140317 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock
+-rw-r--r--   0        0        0   140317 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock
+-rw-r--r--   0        0        0   101191 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock
+-rw-r--r--   0        0        0   101213 2024-04-06 20:04:09.289536 dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock
+-rw-r--r--   0        0        0    31259 2024-04-06 20:04:09.293537 dekpkglock-0.1.5/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock
+-rw-r--r--   0        0        0   123953 2024-04-06 20:04:09.293537 dekpkglock-0.1.5/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock
+-rw-r--r--   0        0        0      476 2024-04-06 20:04:10.753548 dekpkglock-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      359 1970-01-01 00:00:00.000000 dekpkglock-0.1.5/PKG-INFO
```

### Comparing `dekpkglock-0.1.4/dekpkglock/core/base/__init__.py` & `dekpkglock-0.1.5/dekpkglock/core/base/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import os
 from pathlib import Path
-from dektools.file import list_dir, write_file
+from dektools.file import list_dir, write_file, remove_path
 
 
 class PackageLockerBase:
     name = None
     module_name = __name__.partition(".")[0]
     package_file = None
     lock_file = None
     path_resources = [Path(__file__).resolve().parent.parent.parent / 'resources']
 
-    def lock(self, path):
+    def lock(self, path, remove=True):
         result = self.resolve_package_lock(path)
         for k, v in result.items():
-            self.lock_package(k, v)
+            if remove:
+                remove_path(self.get_package_lockfile(k))
+            if os.path.isfile(v):
+                self.lock_package(k, v)
         return bool(result)
 
     def patch(self, path, index=0):
         unique = set()
         for fp, lock_file in self.find_package_lock(path):
             if lock_file not in unique and lock_file.startswith(str(self.path_resources[index])):
                 self.patch_lock(fp, lock_file)
@@ -33,24 +36,26 @@
                         yield fp, os.path.join(
                             path_res, self.name, path_package_rp, meta['version'], self.lock_file
                         )
 
     def resolve_package_lock(self, path):
         result = {}
         for fp, lock_file in self.find_package_lock(path):
-            if os.path.isfile(lock_file):
-                result[fp] = lock_file
+            result[fp] = lock_file
         return result
 
     def lock_package(self, file_package, file_lock):
-        write_file(os.path.join(os.path.dirname(file_package), self.lock_file), c=file_lock)
+        write_file(self.get_package_lockfile(file_package), c=file_lock)
 
     def is_hit(self, filepath):
         return os.path.basename(filepath) == self.package_file
 
+    def get_package_lockfile(self, filepath):
+        return os.path.join(os.path.dirname(filepath), self.lock_file)
+
     def get_package_meta(self, filepath):
         raise NotImplementedError
 
     def patch_lock(self, file_package, file_lock):
         raise NotImplementedError
```

### Comparing `dekpkglock-0.1.4/dekpkglock/core/pdm.py` & `dekpkglock-0.1.5/dekpkglock/core/pdm.py`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock` & `dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.44/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock` & `dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.45/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock` & `dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.46/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.4/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock` & `dekpkglock-0.1.5/dekpkglock/resources/pdm/dekspider/project/0.1.47/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock` & `dekpkglock-0.1.5/dekpkglock/resources/pdm/djcreator/project/0.1.47/pdm.lock`

 * *Files identical despite different names*

### Comparing `dekpkglock-0.1.4/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock` & `dekpkglock-0.1.5/dekpkglock/resources/pdm/djcreator/wrapper/0.1.47/pdm.lock`

 * *Files identical despite different names*

