# Comparing `tmp/gmalglib-0.2.0.tar.gz` & `tmp/gmalglib-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.2.0.tar", last modified: Wed Apr  3 13:30:36 2024, max compression
+gzip compressed data, was "gmalglib-0.3.1.tar", last modified: Sun Apr  7 12:11:40 2024, max compression
```

## Comparing `gmalglib-0.2.0.tar` & `gmalglib-0.3.1.tar`

### file list

```diff
@@ -1,26 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 13:30:30.000000 gmalglib-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-03 13:30:36.495877 gmalglib-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 13:30:30.000000 gmalglib-0.2.0/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 13:30:30.000000 gmalglib-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.491877 gmalglib-0.2.0/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/include/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 13:30:30.000000 gmalglib-0.2.0/include/gmalglib/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 13:30:30.000000 gmalglib-0.2.0/include/gmalglib/sm4.h
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-03 13:30:30.000000 gmalglib-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:30:36.495877 gmalglib-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 13:30:30.000000 gmalglib-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm3module.c
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm4.c
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm4.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm4module.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.880397 gmalglib-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-07 12:11:30.000000 gmalglib-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 12:11:40.880397 gmalglib-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 12:11:30.000000 gmalglib-0.3.1/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-07 12:11:30.000000 gmalglib-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.872397 gmalglib-0.3.1/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.876397 gmalglib-0.3.1/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 12:11:30.000000 gmalglib-0.3.1/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-07 12:11:30.000000 gmalglib-0.3.1/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-07 12:11:30.000000 gmalglib-0.3.1/include/gmalglib/zuc.h
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-07 12:11:30.000000 gmalglib-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 12:11:40.880397 gmalglib-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-07 12:11:30.000000 gmalglib-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.876397 gmalglib-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.876397 gmalglib-0.3.1/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.880397 gmalglib-0.3.1/src/gmalglib/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/core/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5132 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/core/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6401 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/core/zuc.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11064 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/coremodule.c
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/zuc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-07 12:11:30.000000 gmalglib-0.3.1/src/gmalglib/zuc.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 12:11:40.880397 gmalglib-0.3.1/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 12:11:40.000000 gmalglib-0.3.1/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.2.0/LICENSE` & `gmalglib-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.2.0/PKG-INFO` & `gmalglib-0.3.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.2.0
-Summary: GM algorithms C extension for python.
+Version: 0.3.1
+Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gmalglib-0.2.0/include/gmalglib/sm3.h` & `gmalglib-0.3.1/include/gmalglib/sm3.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 #ifndef GMALGLIB_SM3_H
 #define GMALGLIB_SM3_H
-#ifdef __cplusplus
-extern "C" {
-#endif
 
 #include <stdint.h>
 
 #define SM3_MAX_MSG_BITLEN      0xffffffffffffffffULL  // (1 << 64 - 1)
 #define SM3_DIGEST_LENGTH       32
 
 #define SM3_ERR_OVERFLOW        -1
@@ -14,17 +11,22 @@
 typedef struct _SM3 {
     uint32_t value[8];
     uint8_t msg_buffer[64];
     uint64_t msg_buffer_length;
     uint64_t msg_bitlen;
 } SM3;
 
+#ifdef __cplusplus
+extern "C" {
+#endif
+
 void SM3_Init(SM3* self);
 
 int SM3_Update(SM3* self, const uint8_t* data, uint64_t data_len);
 
 void SM3_Digest(SM3* self, uint8_t* digest);
 
 #ifdef __cplusplus
 }
 #endif
+
 #endif // !GMALGLIB_SM3_H
```

### Comparing `gmalglib-0.2.0/pyproject.toml` & `gmalglib-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gmalglib"
 authors = [
     {name = "ww-rm", email = "ww-rm@qq.com"},
 ]
-description = "GM algorithms C extension for python."
+description = "Python package implementing GM algorithms in C."
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: C",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Security :: Cryptography",
@@ -20,17 +20,17 @@
 dynamic = ["version", "readme"]
 
 [project.urls]
 "Homepage" = "https://github.com/ww-rm/gmalglib"
 "Issues" = "https://github.com/ww-rm/gmalglib/issues"
 "Documentation" = "https://gmalglib.readthedocs.io"
 
+[tool.setuptools]
+include-package-data = false
+
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["gmalglib"]
 
-[tool.setuptools.exclude-package-data]
-gmalglib = ["*.c"]
-
 [tool.setuptools.dynamic]
 version = {attr = "gmalglib.__version__"}
 readme = {file = ["README.en.md"], content-type = "text/markdown"}
```

### Comparing `gmalglib-0.2.0/src/gmalglib/sm3.c` & `gmalglib-0.3.1/src/gmalglib/core/sm3.c`

 * *Files identical despite different names*

### Comparing `gmalglib-0.2.0/src/gmalglib/sm3.pyi` & `gmalglib-0.3.1/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.2.0/src/gmalglib/sm4.c` & `gmalglib-0.3.1/src/gmalglib/core/sm4.c`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 
     for (i = 0; i < 32; i += 4)
     {
         round_key[i    ] = K0 = K0 ^ T1(K1 ^ K2 ^ K3 ^ CK[i    ]);
         round_key[i + 1] = K1 = K1 ^ T1(K2 ^ K3 ^ K0 ^ CK[i + 1]);
         round_key[i + 2] = K2 = K2 ^ T1(K3 ^ K0 ^ K1 ^ CK[i + 2]);
         round_key[i + 3] = K3 = K3 ^ T1(K0 ^ K1 ^ K2 ^ CK[i + 3]);
-
     }
 }
 
 void SM4_Init(SM4* self, const uint8_t* key)
 {
     ExpandKey(key, self->round_key);
 }
```

### Comparing `gmalglib-0.2.0/src/gmalglib/sm4.pyi` & `gmalglib-0.3.1/src/gmalglib/sm4.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.2.0/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.3.1/src/gmalglib.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.2.0
-Summary: GM algorithms C extension for python.
+Version: 0.3.1
+Summary: Python package implementing GM algorithms in C.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

