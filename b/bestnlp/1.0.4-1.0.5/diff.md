# Comparing `tmp/bestnlp-1.0.4-py3-none-any.whl.zip` & `tmp/bestnlp-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,12 @@
-Zip file size: 6758 bytes, number of entries: 9
+Zip file size: 1912397 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      239 b- defN 24-Apr-03 06:50 bestnlp/__init__.py
+-rw-r--r--  2.0 unx  5071852 b- defN 24-Mar-29 09:38 bestnlp/dict.txt
 -rw-r--r--  2.0 unx     7301 b- defN 24-Apr-07 06:43 bestnlp/new_word_discovery.py
 -rw-r--r--  2.0 unx     4182 b- defN 24-Apr-07 06:43 bestnlp/similar_word_discovery.py
 -rw-r--r--  2.0 unx     4004 b- defN 24-Mar-29 09:39 bestnlp/similar_word_discovery_embedding.py
 -rw-r--r--  2.0 unx      842 b- defN 24-Apr-03 02:41 bestnlp/utils.py
--rw-r--r--  2.0 unx      245 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      719 b- defN 24-Apr-07 06:49 bestnlp-1.0.4.dist-info/RECORD
-9 files, 17632 bytes uncompressed, 5516 bytes compressed:  68.7%
+-rw-r--r--  2.0 unx      245 b- defN 24-Apr-07 06:54 bestnlp-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-07 06:54 bestnlp-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-Apr-07 06:54 bestnlp-1.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      795 b- defN 24-Apr-07 06:54 bestnlp-1.0.5.dist-info/RECORD
+10 files, 5089560 bytes uncompressed, 1911047 bytes compressed:  62.5%
```

## zipnote {}

```diff
@@ -1,28 +1,31 @@
 Filename: bestnlp/__init__.py
 Comment: 
 
+Filename: bestnlp/dict.txt
+Comment: 
+
 Filename: bestnlp/new_word_discovery.py
 Comment: 
 
 Filename: bestnlp/similar_word_discovery.py
 Comment: 
 
 Filename: bestnlp/similar_word_discovery_embedding.py
 Comment: 
 
 Filename: bestnlp/utils.py
 Comment: 
 
-Filename: bestnlp-1.0.4.dist-info/METADATA
+Filename: bestnlp-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: bestnlp-1.0.4.dist-info/WHEEL
+Filename: bestnlp-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: bestnlp-1.0.4.dist-info/top_level.txt
+Filename: bestnlp-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: bestnlp-1.0.4.dist-info/RECORD
+Filename: bestnlp-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `bestnlp-1.0.4.dist-info/RECORD` & `bestnlp-1.0.5.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 bestnlp/__init__.py,sha256=yWr8dJQkCu83EoT_iYfJ_XAO1EFHFvZz47Wud_dClzM,239
+bestnlp/dict.txt,sha256=cZfDIR3dmJYrA2zfQDJNHqK_qhK9Ao5o-qcBEaiOEqg,5071852
 bestnlp/new_word_discovery.py,sha256=Ddnb0kvu_ksppp7qyhzZsoJ2T8mf87xPNY2J5MjT0GQ,7301
 bestnlp/similar_word_discovery.py,sha256=kgKmD0mbJMXyb1iTRnw_CrtZRvlP5T1wCTg_myjXv_A,4182
 bestnlp/similar_word_discovery_embedding.py,sha256=HsoxJomebHNlB9JyNfGghGSPJ6FJ4X0eAvRnbTUUmf8,4004
 bestnlp/utils.py,sha256=g8F8OjAFl2Fkwn6WyppxHdreeBnN9bVwBFqNUa1Wfww,842
-bestnlp-1.0.4.dist-info/METADATA,sha256=hr4y8afKZ72xSu5VEOKYZNb-4x3y9J79MyC6cnhc1hc,245
-bestnlp-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-bestnlp-1.0.4.dist-info/top_level.txt,sha256=gEejasanGTcCsrx7FMvnDNjB5jb-Xf07bqn5DqRKxg8,8
-bestnlp-1.0.4.dist-info/RECORD,,
+bestnlp-1.0.5.dist-info/METADATA,sha256=md5B9wwlTfyc4Sh2n2xFcKU72T1vmbcGwkACSvJhU3A,245
+bestnlp-1.0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+bestnlp-1.0.5.dist-info/top_level.txt,sha256=gEejasanGTcCsrx7FMvnDNjB5jb-Xf07bqn5DqRKxg8,8
+bestnlp-1.0.5.dist-info/RECORD,,
```

