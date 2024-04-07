# Comparing `tmp/snakenest-0.2.0-py3-none-any.whl.zip` & `tmp/snakenest-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6034 bytes, number of entries: 10
--rw-r--r--  2.0 unx     1443 b- defN 20-Feb-02 00:00 snakenest/__init__.py
--rw-r--r--  2.0 unx      351 b- defN 20-Feb-02 00:00 snakenest/configuration.py
--rw-r--r--  2.0 unx     4641 b- defN 20-Feb-02 00:00 snakenest/context.py
--rw-r--r--  2.0 unx      565 b- defN 20-Feb-02 00:00 snakenest/event.py
--rw-r--r--  2.0 unx     1911 b- defN 20-Feb-02 00:00 snakenest/rulez.py
--rw-r--r--  2.0 unx      366 b- defN 20-Feb-02 00:00 snakenest/singleton.py
-?rw-r--r--  2.0 unx     3236 b- defN 20-Feb-02 00:00 snakenest-0.2.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 snakenest-0.2.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 snakenest-0.2.0.dist-info/licenses/LICENSE.txt
-?rw-r--r--  2.0 unx      776 b- defN 20-Feb-02 00:00 snakenest-0.2.0.dist-info/RECORD
-10 files, 13376 bytes uncompressed, 4716 bytes compressed:  64.7%
+Zip file size: 6067 bytes, number of entries: 10
+-rw-r--r--  2.0 fat     1443 b- defN 20-Feb-02 00:00 snakenest/__init__.py
+-rw-r--r--  2.0 fat      351 b- defN 20-Feb-02 00:00 snakenest/configuration.py
+-rw-r--r--  2.0 fat     4705 b- defN 20-Feb-02 00:00 snakenest/context.py
+-rw-r--r--  2.0 fat      565 b- defN 20-Feb-02 00:00 snakenest/event.py
+-rw-r--r--  2.0 fat     1958 b- defN 20-Feb-02 00:00 snakenest/rulez.py
+-rw-r--r--  2.0 fat      366 b- defN 20-Feb-02 00:00 snakenest/singleton.py
+?rw-r--r--  2.0 fat     3236 b- defN 20-Feb-02 00:00 snakenest-0.2.1.dist-info/METADATA
+?rw-r--r--  2.0 fat       87 b- defN 20-Feb-02 00:00 snakenest-0.2.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat        0 b- defN 20-Feb-02 00:00 snakenest-0.2.1.dist-info/licenses/LICENSE.txt
+?rw-r--r--  2.0 fat      776 b- defN 20-Feb-02 00:00 snakenest-0.2.1.dist-info/RECORD
+10 files, 13487 bytes uncompressed, 4749 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: snakenest/rulez.py
 Comment: 
 
 Filename: snakenest/singleton.py
 Comment: 
 
-Filename: snakenest-0.2.0.dist-info/METADATA
+Filename: snakenest-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: snakenest-0.2.0.dist-info/WHEEL
+Filename: snakenest-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: snakenest-0.2.0.dist-info/licenses/LICENSE.txt
+Filename: snakenest-0.2.1.dist-info/licenses/LICENSE.txt
 Comment: 
 
-Filename: snakenest-0.2.0.dist-info/RECORD
+Filename: snakenest-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## snakenest/context.py

```diff
@@ -79,15 +79,16 @@
             del cls.__nest
             cls.__nest = None
             cls.__init()
 
     @classmethod
     def __initialize_snakes(cls):
         for snake_name, snake_value in cls.__nest['definitions'].items():
-            cls.__create_from_name(snake_name, snake_value)
+            if snake_name not in cls.__nest['byQualifier']:
+                cls.__create_from_name(snake_name, snake_value)
 
     @classmethod
     def __create_from_name(cls, snake_name, snake_definition):
         snake_class = snake_definition[0]
         snake_args: SnakeParameters = snake_definition[1]
 
         # update value from config
```

## snakenest/rulez.py

```diff
@@ -38,26 +38,28 @@
                 else:
                     obj = obj[val[i]]
             else:
                 break
         return ''
 
     @staticmethod
-    def __get_from_env(name):
+    def __get_from_env(name: str):
 
-        if name in environ:
-            return environ[name]
+        to_find = str(name)
+
+        if to_find in environ:
+            return environ[to_find]
 
         return ''
 
     def get(self, item: str, default=None):
         search = item
         default_item = default
 
-        matches = findall('\\${(.*?)}', item)
+        matches = findall('\\${(.*?)}', str(item))
         has_match = len(matches) > 0
 
         if has_match > 0:
             split = matches[0].split(':')
             default_item = split[1] if len(split) > 1 else None
             search = split[0]
```

## Comparing `snakenest-0.2.0.dist-info/METADATA` & `snakenest-0.2.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: SnakeNest
-Version: 0.2.0
+Version: 0.2.1
 Summary: Snake Nest
 Author-email: Roberto Di Rienzo <roberto.dirienzo@codelithic.com>
 Maintainer-email: Roberto Di Rienzo <roberto.dirienzo@codelithic.com>
 License-File: LICENSE.txt
 Keywords: codelithic,injection,spring
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

## Comparing `snakenest-0.2.0.dist-info/RECORD` & `snakenest-0.2.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 snakenest/__init__.py,sha256=7NINvJpj79Bpq8Sony8Azy-mAT5onLeLxH5r5syZ_lQ,1443
 snakenest/configuration.py,sha256=OK6TjkkIREgCnRkxoB1nXoGXial1PYX7GqLh0EfaKPc,351
-snakenest/context.py,sha256=k775JQEkhFxLtRKChQs3l_hUofznU6A4gEWp98WM8Ks,4641
+snakenest/context.py,sha256=2tMG0sJJ2-E1BhZxC-ENzYEaZYbNXT6li3Fd2_98ZiM,4705
 snakenest/event.py,sha256=t0eZ14VcZJFVr4JpUhrf3vncvXT1c3qQ0lZgwb5qHjY,565
-snakenest/rulez.py,sha256=6ffiPuFekC4frfLgjh6y5HVZJN35zzGu9ayjzpW6LrM,1911
+snakenest/rulez.py,sha256=K4bJesybRfDy7fh19tX43wLevPdqEotaG8LuBo3yPmc,1958
 snakenest/singleton.py,sha256=awP_ONrN1XREpRO_wrU_fpPRlqLvBWzOPFv4DovN4iA,366
-snakenest-0.2.0.dist-info/METADATA,sha256=jmTLtooOcfUnhHVCyJyjH4XDqoINGzbQJN6oK0h67iE,3236
-snakenest-0.2.0.dist-info/WHEEL,sha256=uNdcs2TADwSd5pVaP0Z_kcjcvvTUklh2S7bxZMF8Uj0,87
-snakenest-0.2.0.dist-info/licenses/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-snakenest-0.2.0.dist-info/RECORD,,
+snakenest-0.2.1.dist-info/METADATA,sha256=RbvQO3RofdjrqFvGEqhDnHqO5U7PWe2fgty5RB7ctL8,3236
+snakenest-0.2.1.dist-info/WHEEL,sha256=as-1oFTWSeWBgyzh0O_qF439xqBe6AbBgt4MfYe5zwY,87
+snakenest-0.2.1.dist-info/licenses/LICENSE.txt,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+snakenest-0.2.1.dist-info/RECORD,,
```

