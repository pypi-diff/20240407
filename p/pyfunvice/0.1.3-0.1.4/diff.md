# Comparing `tmp/pyfunvice-0.1.3.tar.gz` & `tmp/pyfunvice-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfunvice-0.1.3.tar", max compression
+gzip compressed data, was "pyfunvice-0.1.4.tar", max compression
```

## Comparing `pyfunvice-0.1.3.tar` & `pyfunvice-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.3/README.md
--rw-r--r--   0        0        0     5569 2024-03-29 15:59:09.569908 pyfunvice-0.1.3/pyfunvice/__init__.py
--rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.3/pyfunvice/cli.py
--rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.3/pyfunvice/common_func.py
--rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.3/pyfunvice/docker_cli.py
--rw-r--r--   0        0        0      577 2024-03-26 09:15:00.081774 pyfunvice-0.1.3/pyfunvice/struct.py
--rw-r--r--   0        0        0      454 2024-03-29 16:07:12.133675 pyfunvice-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.4/README.md
+-rw-r--r--   0        0        0     5570 2024-04-02 01:41:13.443528 pyfunvice-0.1.4/pyfunvice/__init__.py
+-rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.4/pyfunvice/cli.py
+-rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.4/pyfunvice/common_func.py
+-rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.4/pyfunvice/docker_cli.py
+-rw-r--r--   0        0        0      577 2024-03-26 09:15:00.081774 pyfunvice-0.1.4/pyfunvice/struct.py
+-rw-r--r--   0        0        0      454 2024-04-07 07:09:38.597243 pyfunvice-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.4/PKG-INFO
```

### Comparing `pyfunvice-0.1.3/README.md` & `pyfunvice-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.3/pyfunvice/__init__.py` & `pyfunvice-0.1.4/pyfunvice/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
                 result = await func(file_name)
                 delete_file(file_name)
                 return result
 
             @faas_router.post(path)
             async def process_function(
                 file: UploadFile = File(...),
-                requestId: str = Form(...),
+                requestId: str = Form(None),
             ):
                 try:
                     if not file:
                         raise Exception("file is empty")
                     if requestId is None or len(requestId) == 0:
                         requestId = get_uuid()
                     file_name: str = requestId
```

### Comparing `pyfunvice-0.1.3/pyfunvice/cli.py` & `pyfunvice-0.1.4/pyfunvice/cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.3/pyfunvice/docker_cli.py` & `pyfunvice-0.1.4/pyfunvice/docker_cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.3/pyfunvice/struct.py` & `pyfunvice-0.1.4/pyfunvice/struct.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.3/PKG-INFO` & `pyfunvice-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfunvice
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: 遥奕
 Author-email: jibing.yjb@alibaba-inc.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

