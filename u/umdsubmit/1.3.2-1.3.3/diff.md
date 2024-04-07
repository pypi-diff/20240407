# Comparing `tmp/umdsubmit-1.3.2.tar.gz` & `tmp/umdsubmit-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umdsubmit-1.3.2.tar", max compression
+gzip compressed data, was "umdsubmit-1.3.3.tar", max compression
```

## Comparing `umdsubmit-1.3.2.tar` & `umdsubmit-1.3.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-12-05 22:24:37.275405 umdsubmit-1.3.2/LICENSE
--rw-r--r--   0        0        0     1800 2023-12-20 21:11:51.853169 umdsubmit-1.3.2/README.md
--rw-r--r--   0        0        0      448 2024-01-29 14:06:02.249882 umdsubmit-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     3819 2024-01-29 14:05:54.035953 umdsubmit-1.3.2/src/umdsubmit/submit.py
--rw-r--r--   0        0        0     2229 1970-01-01 00:00:00.000000 umdsubmit-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-12-05 22:24:37.275405 umdsubmit-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1800 2023-12-20 21:11:51.853169 umdsubmit-1.3.3/README.md
+-rw-r--r--   0        0        0      448 2024-04-07 18:49:47.316111 umdsubmit-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3885 2024-04-07 18:48:47.172251 umdsubmit-1.3.3/src/umdsubmit/submit.py
+-rw-r--r--   0        0        0     2280 1970-01-01 00:00:00.000000 umdsubmit-1.3.3/PKG-INFO
```

### Comparing `umdsubmit-1.3.2/LICENSE` & `umdsubmit-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `umdsubmit-1.3.2/README.md` & `umdsubmit-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `umdsubmit-1.3.2/src/umdsubmit/submit.py` & `umdsubmit-1.3.3/src/umdsubmit/submit.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,8 +103,11 @@
     if not os.path.isfile('.submitUser'):
         auth()
     shutil.make_archive('submit', 'zip', os.getcwd())
     submit_zip_object =  open('submit.zip', 'rb')
     files = {"submittedFiles": ("submit.zip", submit_zip_object)}
     data = {"courseName" : get_info("courseName"), "projectNumber" : get_info("projectNumber"), "semester" : get_info("semester"), "courseKey" : get_info("courseKey"), "authentication.type" : get_info("authentication.type"), "baseURL" : get_info("baseURL"), "submitURL" : get_info("submitURL"), "cvsAccount" : get_cvs_account(), "oneTimePassword" : get_one_time_password(), "submitClientTool" : "umdsubmit", "submitClientVersion" : "1.0"}
     response = requests.post(get_info("submitURL"), files = files, data = data)
+    if response.status_code == 401:
+        auth()
+        main()
     print(response.text)
```

### Comparing `umdsubmit-1.3.2/PKG-INFO` & `umdsubmit-1.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: umdsubmit
-Version: 1.3.2
+Version: 1.3.3
 Summary: Allows submitting to the UMD Submit Server from the command line, without the Eclipse Plugin
 Author: Nico Carbone
 Author-email: carbone.nicolas0@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # umdsubmit
 
 This package allows submitting to the UMD Submit Server from the command line, without the Eclipse Plugin.
```

