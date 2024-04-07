# Comparing `tmp/ks3sdk-1.6.1.tar.gz` & `tmp/ks3sdk-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ks3sdk-1.6.1.tar", last modified: Fri Mar 22 09:49:55 2024, max compression
+gzip compressed data, was "ks3sdk-1.6.2.tar", last modified: Sun Apr  7 06:16:12 2024, max compression
```

## Comparing `ks3sdk-1.6.1.tar` & `ks3sdk-1.6.2.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 09:49:55.967621 ks3sdk-1.6.1/
--rw-r--r--   0 root         (0) root         (0)     1065 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       74 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2314 2024-03-22 09:49:55.967621 ks3sdk-1.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1631 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 09:49:55.963621 ks3sdk-1.6.1/examples/
--rw-r--r--   0 root         (0) root         (0)    22705 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/basic.py
--rw-r--r--   0 root         (0) root         (0)      974 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/billing.py
--rw-r--r--   0 root         (0) root         (0)     9667 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/bucket.py
--rw-r--r--   0 root         (0) root         (0)     5968 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/crc64.py
--rw-r--r--   0 root         (0) root         (0)    10988 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/encryption.py
--rw-r--r--   0 root         (0) root         (0)     3827 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/multi_thread.py
--rw-r--r--   0 root         (0) root         (0)     2620 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/multipart.py
--rw-r--r--   0 root         (0) root         (0)    12419 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/object.py
--rw-r--r--   0 root         (0) root         (0)      558 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/postProcessTask.py
--rw-r--r--   0 root         (0) root         (0)      868 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/examples/sts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 09:49:55.966621 ks3sdk-1.6.1/ks3/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5764 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/acl.py
--rw-r--r--   0 root         (0) root         (0)     5046 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/auth.py
--rw-r--r--   0 root         (0) root         (0)     4326 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/authV4.py
--rw-r--r--   0 root         (0) root         (0)      885 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/billing.py
--rw-r--r--   0 root         (0) root         (0)    48537 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/bucket.py
--rw-r--r--   0 root         (0) root         (0)     5930 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/bucketlistresultset.py
--rw-r--r--   0 root         (0) root         (0)      771 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/compat.py
--rw-r--r--   0 root         (0) root         (0)    14200 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/connection.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/conv.py
--rw-r--r--   0 root         (0) root         (0)     4913 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/crc64_combine.py
--rw-r--r--   0 root         (0) root         (0)      979 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/deletemarker.py
--rw-r--r--   0 root         (0) root         (0)     8597 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/encryptFp.py
--rw-r--r--   0 root         (0) root         (0)     2796 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/encryption.py
--rw-r--r--   0 root         (0) root         (0)     7259 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/exception.py
--rw-r--r--   0 root         (0) root         (0)     2378 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/handler.py
--rw-r--r--   0 root         (0) root         (0)     5898 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/http.py
--rw-r--r--   0 root         (0) root         (0)    53623 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/key.py
--rw-r--r--   0 root         (0) root         (0)     4430 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/keyfile.py
--rw-r--r--   0 root         (0) root         (0)    14015 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/multipart.py
--rw-r--r--   0 root         (0) root         (0)     1648 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/objectTagging.py
--rw-r--r--   0 root         (0) root         (0)      579 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/prefix.py
--rw-r--r--   0 root         (0) root         (0)    22544 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/provider.py
--rw-r--r--   0 root         (0) root         (0)     4698 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/resultset.py
--rw-r--r--   0 root         (0) root         (0)     1202 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/sts.py
--rw-r--r--   0 root         (0) root         (0)      894 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/user.py
--rw-r--r--   0 root         (0) root         (0)     7079 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 09:49:55.966621 ks3sdk-1.6.1/ks3/xmlParsers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2778 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/bucketCors.py
--rw-r--r--   0 root         (0) root         (0)     1705 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/bucketCrossReplicate.py
--rw-r--r--   0 root         (0) root         (0)     6888 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/bucketLifecycle.py
--rw-r--r--   0 root         (0) root         (0)     3256 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/bucketLogging.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/bucketMirror.py
--rw-r--r--   0 root         (0) root         (0)      635 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/bucketQuota.py
--rw-r--r--   0 root         (0) root         (0)      721 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/ks3/xmlParsers/bucketVersioning.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-22 09:49:55.967621 ks3sdk-1.6.1/ks3sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2314 2024-03-22 09:49:55.000000 ks3sdk-1.6.1/ks3sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1089 2024-03-22 09:49:55.000000 ks3sdk-1.6.1/ks3sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-22 09:49:55.000000 ks3sdk-1.6.1/ks3sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-03-22 09:49:55.000000 ks3sdk-1.6.1/ks3sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2024-03-22 09:49:55.000000 ks3sdk-1.6.1/ks3sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       35 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-22 09:49:55.967621 ks3sdk-1.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1355 2024-03-22 09:49:07.000000 ks3sdk-1.6.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/
+-rw-r--r--   0 root         (0) root         (0)     1065 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       74 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.836873 ks3sdk-1.6.2/examples/
+-rw-r--r--   0 root         (0) root         (0)    24554 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/basic.py
+-rw-r--r--   0 root         (0) root         (0)      974 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/billing.py
+-rw-r--r--   0 root         (0) root         (0)     9667 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     5968 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/crc64.py
+-rw-r--r--   0 root         (0) root         (0)    10988 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     3827 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/multi_thread.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/multipart.py
+-rw-r--r--   0 root         (0) root         (0)    12419 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/object.py
+-rw-r--r--   0 root         (0) root         (0)      558 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/postProcessTask.py
+-rw-r--r--   0 root         (0) root         (0)      868 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/examples/sts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.839873 ks3sdk-1.6.2/ks3/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5764 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/acl.py
+-rw-r--r--   0 root         (0) root         (0)     5109 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/auth.py
+-rw-r--r--   0 root         (0) root         (0)     4326 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/authV4.py
+-rw-r--r--   0 root         (0) root         (0)      885 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/billing.py
+-rw-r--r--   0 root         (0) root         (0)    50561 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/bucket.py
+-rw-r--r--   0 root         (0) root         (0)     6887 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/bucketlistresultset.py
+-rw-r--r--   0 root         (0) root         (0)      771 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/compat.py
+-rw-r--r--   0 root         (0) root         (0)    14200 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/connection.py
+-rw-r--r--   0 root         (0) root         (0)      493 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/conv.py
+-rw-r--r--   0 root         (0) root         (0)     4913 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/crc64_combine.py
+-rw-r--r--   0 root         (0) root         (0)      979 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/deletemarker.py
+-rw-r--r--   0 root         (0) root         (0)     8597 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/encryptFp.py
+-rw-r--r--   0 root         (0) root         (0)     2796 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/encryption.py
+-rw-r--r--   0 root         (0) root         (0)     7259 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/exception.py
+-rw-r--r--   0 root         (0) root         (0)     2378 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/handler.py
+-rw-r--r--   0 root         (0) root         (0)     5898 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/http.py
+-rw-r--r--   0 root         (0) root         (0)    55353 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/key.py
+-rw-r--r--   0 root         (0) root         (0)     4430 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/keyfile.py
+-rw-r--r--   0 root         (0) root         (0)    14015 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/multipart.py
+-rw-r--r--   0 root         (0) root         (0)     1648 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/objectTagging.py
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/prefix.py
+-rw-r--r--   0 root         (0) root         (0)    22966 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/provider.py
+-rw-r--r--   0 root         (0) root         (0)     4698 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/resultset.py
+-rw-r--r--   0 root         (0) root         (0)     1202 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/sts.py
+-rw-r--r--   0 root         (0) root         (0)      894 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/user.py
+-rw-r--r--   0 root         (0) root         (0)     7079 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/ks3/xmlParsers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2778 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketCors.py
+-rw-r--r--   0 root         (0) root         (0)     2480 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketCrossReplicate.py
+-rw-r--r--   0 root         (0) root         (0)     8168 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketLifecycle.py
+-rw-r--r--   0 root         (0) root         (0)     3256 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketLogging.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketMirror.py
+-rw-r--r--   0 root         (0) root         (0)      635 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketQuota.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketRetention.py
+-rw-r--r--   0 root         (0) root         (0)      721 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/ks3/xmlParsers/bucketVersioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/ks3sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2314 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1123 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2024-04-07 06:16:12.000000 ks3sdk-1.6.2/ks3sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-07 06:16:12.840873 ks3sdk-1.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1355 2024-04-07 06:15:11.000000 ks3sdk-1.6.2/setup.py
```

### Comparing `ks3sdk-1.6.1/LICENSE` & `ks3sdk-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/PKG-INFO` & `ks3sdk-1.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ks3sdk
-Version: 1.6.1
+Version: 1.6.2
 Summary: Ksyun KS3 SDK
 Home-page: https://gitee.com/ks3sdk/ks3-python-sdk
 Author: ksc_ks3
 Author-email: ksc_ks3@kingsoft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ks3sdk-1.6.1/README.md` & `ks3sdk-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/basic.py` & `ks3sdk-1.6.2/examples/basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,1407 +14,1522 @@
 000000d0: 204b 6579 0a66 726f 6d20 6b73 332e 6f62   Key.from ks3.ob
 000000e0: 6a65 6374 5461 6767 696e 6720 696d 706f  jectTagging impo
 000000f0: 7274 2054 6167 0a66 726f 6d20 6b73 332e  rt Tag.from ks3.
 00000100: 786d 6c50 6172 7365 7273 2e62 7563 6b65  xmlParsers.bucke
 00000110: 7443 6f72 7320 696d 706f 7274 2042 7563  tCors import Buc
 00000120: 6b65 7443 6f72 732c 2043 4f52 5352 756c  ketCors, CORSRul
 00000130: 650a 6672 6f6d 206b 7333 2e78 6d6c 5061  e.from ks3.xmlPa
-00000140: 7273 6572 732e 6275 636b 6574 4c69 6665  rsers.bucketLife
-00000150: 6379 636c 6520 696d 706f 7274 2042 7563  cycle import Buc
-00000160: 6b65 744c 6966 6563 7963 6c65 2c20 5275  ketLifecycle, Ru
-00000170: 6c65 2061 7320 4c69 6665 6379 636c 6552  le as LifecycleR
-00000180: 756c 652c 2046 696c 7465 7220 6173 204c  ule, Filter as L
-00000190: 6966 6563 7963 6c65 4669 6c74 6572 2c20  ifecycleFilter, 
-000001a0: 5c0a 2020 4578 7069 7261 7469 6f6e 2061  \.  Expiration a
-000001b0: 7320 4c69 6665 6379 636c 6545 7870 6972  s LifecycleExpir
-000001c0: 6174 696f 6e2c 2054 7261 6e73 6974 696f  ation, Transitio
-000001d0: 6e20 6173 204c 6966 6563 7963 6c65 5472  n as LifecycleTr
-000001e0: 616e 7369 7469 6f6e 0a66 726f 6d20 6b73  ansition.from ks
-000001f0: 332e 786d 6c50 6172 7365 7273 2e62 7563  3.xmlParsers.buc
-00000200: 6b65 744c 6f67 6769 6e67 2069 6d70 6f72  ketLogging impor
-00000210: 7420 4275 636b 6574 4c6f 6767 696e 670a  t BucketLogging.
-00000220: 2320 e9a6 96e5 8588 e588 9de5 a78b e58c  # ..............
-00000230: 9641 6363 6573 734b 6579 4964 e380 8141  .AccessKeyId...A
-00000240: 6363 6573 734b 6579 5365 6372 6574 e380  ccessKeySecret..
-00000250: 8145 6e64 706f 696e 74e7 ad89 e4bf a1e6  .Endpoint.......
-00000260: 81af e380 820a 2320 e980 9ae8 bf87 e78e  ......# ........
-00000270: afe5 a283 e58f 98e9 878f e88e b7e5 8f96  ................
-00000280: efbc 8ce6 8896 e880 85e6 8a8a e8af b8e5  ................
-00000290: a682 e280 9c3c e4bd a0e7 9a84 4163 6365  .....<......Acce
-000002a0: 7373 4b65 7949 643e e280 9de6 9bbf e68d  ssKeyId>........
-000002b0: a2e6 8890 e79c 9fe5 ae9e e79a 8441 6363  .............Acc
-000002c0: 6573 734b 6579 4964 e7ad 89e3 8082 0a66  essKeyId.......f
-000002d0: 726f 6d20 6b73 332e 786d 6c50 6172 7365  rom ks3.xmlParse
-000002e0: 7273 2e62 7563 6b65 744d 6972 726f 7220  rs.bucketMirror 
-000002f0: 696d 706f 7274 2042 7563 6b65 744d 6972  import BucketMir
-00000300: 726f 722c 2041 7379 6e63 4d69 7272 6f72  ror, AsyncMirror
-00000310: 5275 6c65 2c20 5379 6e63 4d69 7272 6f72  Rule, SyncMirror
-00000320: 5275 6c65 732c 204d 6972 726f 7252 6571  Rules, MirrorReq
-00000330: 7565 7374 5365 7474 696e 672c 205c 0a20  uestSetting, \. 
-00000340: 2048 6561 6465 7253 6574 7469 6e67 0a66   HeaderSetting.f
-00000350: 726f 6d20 6261 7365 3634 2069 6d70 6f72  rom base64 impor
-00000360: 7420 7572 6c73 6166 655f 6236 3465 6e63  t urlsafe_b64enc
-00000370: 6f64 650a 696d 706f 7274 2061 7379 6e63  ode.import async
-00000380: 696f 0a0a 616b 203d 206f 732e 6765 7465  io..ak = os.gete
-00000390: 6e76 2827 4b53 335f 4941 4d5f 4143 4345  nv('KS3_IAM_ACCE
-000003a0: 5353 5f4b 4559 5f49 4427 2c20 273c 594f  SS_KEY_ID', '<YO
-000003b0: 5552 5f41 4343 4553 535f 4b45 593e 2729  UR_ACCESS_KEY>')
-000003c0: 0a73 6b20 3d20 6f73 2e67 6574 656e 7628  .sk = os.getenv(
-000003d0: 274b 5333 5f49 414d 5f41 4343 4553 535f  'KS3_IAM_ACCESS_
-000003e0: 4b45 595f 5345 4352 4554 272c 2027 3c59  KEY_SECRET', '<Y
-000003f0: 4f55 525f 5345 4352 4554 5f4b 4559 3e27  OUR_SECRET_KEY>'
-00000400: 290a 6275 636b 6574 5f6e 616d 6520 3d20  ).bucket_name = 
-00000410: 6f73 2e67 6574 656e 7628 274b 5333 5f42  os.getenv('KS3_B
-00000420: 5543 4b45 5427 2c20 273c 4b53 335f 5445  UCKET', '<KS3_TE
-00000430: 5354 5f42 5543 4b45 543e 2729 0a65 6e64  ST_BUCKET>').end
-00000440: 706f 696e 7420 3d20 276b 7333 2d63 6e2d  point = 'ks3-cn-
-00000450: 6265 696a 696e 672e 6b73 7975 6e63 732e  beijing.ksyuncs.
-00000460: 636f 6d27 2023 6f73 2e67 6574 656e 7628  com' #os.getenv(
-00000470: 274b 5333 5f54 4553 545f 454e 4450 4f49  'KS3_TEST_ENDPOI
-00000480: 4e54 272c 2027 6b73 332d 636e 2d73 6861  NT', 'ks3-cn-sha
-00000490: 6e67 6861 692d 696e 7465 726e 616c 2e6b  nghai-internal.k
-000004a0: 7379 756e 6373 2e63 6f6d 2729 0a0a 636f  syuncs.com')..co
-000004b0: 6e6e 203d 2043 6f6e 6e65 6374 696f 6e28  nn = Connection(
-000004c0: 616b 2c20 736b 2c20 686f 7374 3d65 6e64  ak, sk, host=end
-000004d0: 706f 696e 742c 2070 6f72 743d 3830 2c20  point, port=80, 
-000004e0: 7561 5f61 6464 6f6e 3d27 7465 7374 2d75  ua_addon='test-u
-000004f0: 612f 3127 2920 2370 6f72 743d 3830 3931  a/1') #port=8091
-00000500: 2c0a 6b65 795f 6e61 6d65 203d 2027 7465  ,.key_name = 'te
-00000510: 7374 5f6b 6579 270a 0a0a 6465 6620 6765  st_key'...def ge
-00000520: 7441 6c6c 4275 636b 6574 7328 7072 6f6a  tAllBuckets(proj
-00000530: 6563 745f 6964 733d 4e6f 6e65 293a 0a20  ect_ids=None):. 
-00000540: 2062 7563 6b65 7473 203d 2063 6f6e 6e2e   buckets = conn.
-00000550: 6765 745f 616c 6c5f 6275 636b 6574 7328  get_all_buckets(
-00000560: 7072 6f6a 6563 745f 6964 733d 7072 6f6a  project_ids=proj
-00000570: 6563 745f 6964 7329 2023 0a20 2066 6f72  ect_ids) #.  for
-00000580: 2062 2069 6e20 6275 636b 6574 733a 0a20   b in buckets:. 
-00000590: 2020 2070 7269 6e74 2862 2e6e 616d 652c     print(b.name,
-000005a0: 2062 2e72 6567 696f 6e2c 2062 2e52 6567   b.region, b.Reg
-000005b0: 696f 6e2c 2062 2e63 7265 6174 696f 6e5f  ion, b.creation_
-000005c0: 6461 7465 290a 0a64 6566 2068 6561 6442  date)..def headB
-000005d0: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-000005e0: 6529 3a0a 2020 2320 e5a6 82e6 9e9c e6ad  e):.  # ........
-000005f0: a3e5 b8b8 e8bf 94e5 9b9e efbc 8ce5 8899  ................
-00000600: 4275 636b 6574 e5ad 98e5 9ca8 efbc 9be5  Bucket..........
-00000610: a682 e69e 9ce6 8a9b e587 ba53 3352 6573  ...........S3Res
-00000620: 706f 6e73 6545 7272 6f72 0a20 2063 6f6e  ponseError.  con
-00000630: 6e2e 6865 6164 5f62 7563 6b65 7428 6275  n.head_bucket(bu
-00000640: 636b 6574 5f6e 616d 6529 0a0a 6465 6620  cket_name)..def 
-00000650: 6765 7442 7563 6b65 744c 6f63 6174 696f  getBucketLocatio
-00000660: 6e28 6275 636b 6574 5f6e 616d 6529 3a0a  n(bucket_name):.
-00000670: 2020 7072 696e 7428 636f 6e6e 2e67 6574    print(conn.get
-00000680: 5f62 7563 6b65 745f 6c6f 6361 7469 6f6e  _bucket_location
-00000690: 2862 7563 6b65 745f 6e61 6d65 2929 0a0a  (bucket_name))..
-000006a0: 6465 6620 6372 6561 7465 4275 636b 6574  def createBucket
-000006b0: 2862 7563 6b65 745f 6e61 6d65 2c20 6c6f  (bucket_name, lo
-000006c0: 6361 7469 6f6e 3d27 2729 3a0a 2020 636f  cation=''):.  co
-000006d0: 6e6e 2e63 7265 6174 655f 6275 636b 6574  nn.create_bucket
-000006e0: 2862 7563 6b65 745f 6e61 6d65 2c20 6c6f  (bucket_name, lo
-000006f0: 6361 7469 6f6e 3d6c 6f63 6174 696f 6e2c  cation=location,
-00000700: 2068 6561 6465 7273 3d7b 0a20 2020 2027   headers={.    '
-00000710: 782d 6b73 732d 6275 636b 6574 2d74 7970  x-kss-bucket-typ
-00000720: 6527 3a20 2741 5243 4849 5645 270a 2020  e': 'ARCHIVE'.  
-00000730: 7d29 0a0a 6465 6620 6465 6c65 7465 4275  })..def deleteBu
-00000740: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00000750: 293a 0a20 2074 7279 3a0a 2020 2020 636f  ):.  try:.    co
-00000760: 6e6e 2e64 656c 6574 655f 6275 636b 6574  nn.delete_bucket
-00000770: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-00000780: 6578 6365 7074 2053 3352 6573 706f 6e73  except S3Respons
-00000790: 6545 7272 6f72 2061 7320 6572 726f 723a  eError as error:
-000007a0: 0a20 2020 2070 7269 6e74 2827 6572 726f  .    print('erro
-000007b0: 7227 290a 2020 2020 7072 696e 7428 6572  r').    print(er
-000007c0: 726f 7229 0a0a 6465 6620 6765 7442 7563  ror)..def getBuc
-000007d0: 6b65 7441 636c 2862 7563 6b65 745f 6e61  ketAcl(bucket_na
-000007e0: 6d65 293a 0a20 2062 203d 2063 6f6e 6e2e  me):.  b = conn.
-000007f0: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00000800: 745f 6e61 6d65 290a 2020 706f 6c69 6379  t_name).  policy
-00000810: 203d 2062 2e67 6574 5f61 636c 2829 0a20   = b.get_acl(). 
-00000820: 2023 2070 7269 6e74 2870 6f6c 6963 7929   # print(policy)
-00000830: 0a20 2066 6f72 2067 7261 6e74 2069 6e20  .  for grant in 
-00000840: 706f 6c69 6379 2e61 636c 2e67 7261 6e74  policy.acl.grant
-00000850: 733a 0a20 2020 2070 7269 6e74 2867 7261  s:.    print(gra
-00000860: 6e74 2e70 6572 6d69 7373 696f 6e2c 2067  nt.permission, g
-00000870: 7261 6e74 2e64 6973 706c 6179 5f6e 616d  rant.display_nam
-00000880: 652c 2067 7261 6e74 2e65 6d61 696c 5f61  e, grant.email_a
-00000890: 6464 7265 7373 2c20 6772 616e 742e 6964  ddress, grant.id
-000008a0: 290a 0a64 6566 2073 6574 4275 636b 6574  )..def setBucket
-000008b0: 4163 6c28 6275 636b 6574 5f6e 616d 6529  Acl(bucket_name)
-000008c0: 3a0a 2020 6220 3d20 636f 6e6e 2e67 6574  :.  b = conn.get
-000008d0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
-000008e0: 616d 6529 0a20 2062 2e73 6574 5f61 636c  ame).  b.set_acl
-000008f0: 2822 7072 6976 6174 6522 290a 0a64 6566  ("private")..def
-00000900: 206d 616e 6167 6542 7563 6b65 7450 6f6c   manageBucketPol
-00000910: 6963 7928 6275 636b 6574 5f6e 616d 6529  icy(bucket_name)
-00000920: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
-00000930: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
-00000940: 6b65 745f 6e61 6d65 290a 2020 6275 636b  ket_name).  buck
-00000950: 6574 2e73 6574 5f62 7563 6b65 745f 706f  et.set_bucket_po
-00000960: 6c69 6379 280a 2020 2020 706f 6c69 6379  licy(.    policy
-00000970: 3d27 7b22 5374 6174 656d 656e 7422 3a5b  ='{"Statement":[
-00000980: 7b22 5265 736f 7572 6365 223a 5b22 6b72  {"Resource":["kr
-00000990: 6e3a 6b73 633a 6b73 333a 3a3a 6a69 616e  n:ksc:ks3:::jian
-000009a0: 6772 616e 3132 3322 2c22 6b72 6e3a 6b73  gran123","krn:ks
-000009b0: 633a 6b73 333a 3a3a 6a69 616e 6772 616e  c:ks3:::jiangran
-000009c0: 3132 332f 2a22 5d2c 2250 7269 6e63 6970  123/*"],"Princip
-000009d0: 616c 223a 7b22 4b53 4322 3a5b 226b 726e  al":{"KSC":["krn
-000009e0: 3a6b 7363 3a69 616d 3a3a 3332 3433 3234  :ksc:iam::324324
-000009f0: 3233 3a72 6f6f 7422 5d7d 2c22 4163 7469  23:root"]},"Acti
-00000a00: 6f6e 223a 5b22 6b73 333a 2a22 5d2c 2245  on":["ks3:*"],"E
-00000a10: 6666 6563 7422 3a22 416c 6c6f 7722 7d5d  ffect":"Allow"}]
-00000a20: 7d27 290a 2020 2320 706f 6c69 6379 203d  }').  # policy =
-00000a30: 2062 7563 6b65 742e 6765 745f 6275 636b   bucket.get_buck
-00000a40: 6574 5f70 6f6c 6963 7928 290a 2020 2320  et_policy().  # 
-00000a50: 6275 636b 6574 2e64 656c 6574 655f 6275  bucket.delete_bu
-00000a60: 636b 6574 5f70 6f6c 6963 7928 290a 0a64  cket_policy()..d
-00000a70: 6566 206d 616e 6167 6542 7563 6b65 7452  ef manageBucketR
-00000a80: 6570 6c69 6361 7469 6f6e 2862 7563 6b65  eplication(bucke
-00000a90: 745f 6e61 6d65 293a 0a20 2062 7563 6b65  t_name):.  bucke
-00000aa0: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
-00000ab0: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
-00000ac0: 0a20 2074 7279 3a0a 2020 2020 7072 696e  .  try:.    prin
-00000ad0: 7428 6275 636b 6574 2e67 6574 5f62 7563  t(bucket.get_buc
-00000ae0: 6b65 745f 6372 7228 292e 746f 5f78 6d6c  ket_crr().to_xml
-00000af0: 2829 290a 2020 6578 6365 7074 3a0a 2020  ()).  except:.  
-00000b00: 2020 6275 636b 6574 2e73 6574 5f62 7563    bucket.set_buc
-00000b10: 6b65 745f 6372 7228 2774 6573 742d 6275  ket_crr('test-bu
-00000b20: 636b 6574 2d70 726f 6a65 6374 272c 2064  cket-project', d
-00000b30: 656c 6574 654d 6172 6b65 7253 7461 7475  eleteMarkerStatu
-00000b40: 733d 2744 6973 6162 6c65 6427 2c20 7072  s='Disabled', pr
-00000b50: 6566 6978 5f6c 6973 743d 5b27 6865 6c6c  efix_list=['hell
-00000b60: 6f27 5d29 0a0a 6465 6620 6765 7442 7563  o'])..def getBuc
-00000b70: 6b65 744c 6966 6543 7963 6c65 2862 7563  ketLifeCycle(buc
-00000b80: 6b65 745f 6e61 6d65 293a 0a20 2062 7563  ket_name):.  buc
-00000b90: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
-00000ba0: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-00000bb0: 6529 0a20 206c 6966 6563 7963 6c65 203d  e).  lifecycle =
-00000bc0: 2062 7563 6b65 742e 6765 745f 6275 636b   bucket.get_buck
-00000bd0: 6574 5f6c 6966 6563 7963 6c65 2829 0a20  et_lifecycle(). 
-00000be0: 2070 7269 6e74 286c 6966 6563 7963 6c65   print(lifecycle
-00000bf0: 2e74 6f5f 786d 6c28 2929 0a0a 6465 6620  .to_xml())..def 
-00000c00: 7365 7442 7563 6b65 744c 6966 6543 7963  setBucketLifeCyc
-00000c10: 6c65 2862 7563 6b65 745f 6e61 6d65 293a  le(bucket_name):
-00000c20: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
-00000c30: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
-00000c40: 6574 5f6e 616d 6529 0a20 206c 6966 6563  et_name).  lifec
-00000c50: 7963 6c65 203d 2042 7563 6b65 744c 6966  ycle = BucketLif
-00000c60: 6563 7963 6c65 2829 0a20 2023 2069 6420  ecycle().  # id 
-00000c70: e592 8c20 7374 6174 7573 20e5 bf85 e9a1  ... status .....
-00000c80: bb0a 2020 7275 6c65 203d 204c 6966 6563  ..  rule = Lifec
-00000c90: 7963 6c65 5275 6c65 2869 643d 2772 756c  ycleRule(id='rul
-00000ca0: 6531 272c 2073 7461 7475 733d 2745 6e61  e1', status='Ena
-00000cb0: 626c 6564 2729 0a20 2064 6174 6520 3d20  bled').  date = 
-00000cc0: 6461 7465 7469 6d65 2832 3032 312c 2039  datetime(2021, 9
-00000cd0: 2c20 3132 292e 7374 7266 7469 6d65 2827  , 12).strftime('
-00000ce0: 2559 2d25 6d2d 2564 5425 483a 254d 3a25  %Y-%m-%dT%H:%M:%
-00000cf0: 5327 2920 2b20 272b 3038 3a30 3027 0a20  S') + '+08:00'. 
-00000d00: 2072 756c 652e 6578 7069 7261 7469 6f6e   rule.expiration
-00000d10: 203d 204c 6966 6563 7963 6c65 4578 7069   = LifecycleExpi
-00000d20: 7261 7469 6f6e 2864 6174 653d 6461 7465  ration(date=date
-00000d30: 290a 2020 6c69 6665 6379 636c 652e 7275  ).  lifecycle.ru
-00000d40: 6c65 203d 205b 7275 6c65 5d0a 2020 6275  le = [rule].  bu
-00000d50: 636b 6574 2e73 6574 5f62 7563 6b65 745f  cket.set_bucket_
-00000d60: 6c69 6665 6379 636c 6528 6c69 6665 6379  lifecycle(lifecy
-00000d70: 636c 6529 0a0a 0a64 6566 2073 6574 4275  cle)...def setBu
-00000d80: 636b 6574 4c69 6665 4379 636c 6532 2862  cketLifeCycle2(b
-00000d90: 7563 6b65 745f 6e61 6d65 293a 0a20 2062  ucket_name):.  b
-00000da0: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
-00000db0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
-00000dc0: 616d 6529 0a20 2074 6167 203d 2054 6167  ame).  tag = Tag
-00000dd0: 286b 6579 3d22 7461 6731 222c 2076 616c  (key="tag1", val
-00000de0: 7565 3d22 7465 7374 3122 290a 2020 2320  ue="test1").  # 
-00000df0: e7ad 9be9 8089 e589 8de7 bc80 e4b8 ba20  ............... 
-00000e00: 7072 6566 6978 31e3 8081 e6a0 87e7 adbe  prefix1.........
-00000e10: e4b8 ba20 7461 6731 3a74 6573 7431 20e7  ... tag1:test1 .
-00000e20: 9a84 206f 626a 6563 7473 efbc 8ce8 aebe  .. objects......
-00000e30: e7bd aee8 bf87 e69c 9fe8 a784 e588 99ef  ................
-00000e40: bc8c e59c a8e5 85b6 e69c 80e5 908e e4bf  ................
-00000e50: aee6 94b9 e697 b6e9 97b4 33e5 a4a9 e590  ..........3.....
-00000e60: 8ee8 bf87 e69c 9fe3 8082 0a20 2072 756c  ...........  rul
-00000e70: 6531 203d 204c 6966 6563 7963 6c65 5275  e1 = LifecycleRu
-00000e80: 6c65 2827 7275 6c65 3127 2c20 4c69 6665  le('rule1', Life
-00000e90: 6379 636c 6546 696c 7465 7228 2770 7265  cycleFilter('pre
-00000ea0: 6669 7831 272c 2074 6167 733d 5b74 6167  fix1', tags=[tag
-00000eb0: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
-00000ec0: 2020 2020 2020 2020 2020 2020 7374 6174              stat
-00000ed0: 7573 3d27 456e 6162 6c65 6427 2c0a 2020  us='Enabled',.  
-00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ef0: 2020 2020 2020 6578 7069 7261 7469 6f6e        expiration
-00000f00: 3d4c 6966 6563 7963 6c65 4578 7069 7261  =LifecycleExpira
-00000f10: 7469 6f6e 2864 6179 733d 3329 290a 0a20  tion(days=3)).. 
-00000f20: 2023 20e8 aebe e7bd aee8 bf87 e69c 9fe8   # .............
-00000f30: a784 e588 99ef bc8c e7ad 9be9 8089 e6a0  ................
-00000f40: 87e7 adbe e4b8 ba20 7461 6731 3a74 6573  ....... tag1:tes
-00000f50: 7431 20e7 9a84 206f 626a 6563 7473 efbc  t1 ... objects..
-00000f60: 8ce6 9c80 e590 8ee4 bfae e694 b9e6 97b6  ................
-00000f70: e997 b4e5 9ca8 e68c 87e5 ae9a e697 a5e6  ................
-00000f80: 9c9f e4b9 8be5 898d e79a 84ef bc8c e8bf  ................
-00000f90: 87e6 9c9f 0a20 2072 756c 6532 203d 204c  .....  rule2 = L
-00000fa0: 6966 6563 7963 6c65 5275 6c65 2827 7275  ifecycleRule('ru
-00000fb0: 6c65 3227 2c20 4c69 6665 6379 636c 6546  le2', LifecycleF
-00000fc0: 696c 7465 7228 7461 6773 3d5b 7461 675d  ilter(tags=[tag]
-00000fd0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00000fe0: 2020 2020 2020 2020 2020 2073 7461 7475             statu
-00000ff0: 733d 2745 6e61 626c 6564 272c 0a20 2020  s='Enabled',.   
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2065 7870 6972 6174 696f 6e3d       expiration=
-00001020: 4c69 6665 6379 636c 6545 7870 6972 6174  LifecycleExpirat
-00001030: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-00001040: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001050: 6174 653d 6461 7465 7469 6d65 2832 3032  ate=datetime(202
-00001060: 312c 2031 322c 2031 3229 2e69 736f 666f  1, 12, 12).isofo
-00001070: 726d 6174 2874 696d 6573 7065 633d 2773  rmat(timespec='s
-00001080: 6563 6f6e 6473 2729 202b 2027 2b30 383a  econds') + '+08:
-00001090: 3030 2729 290a 0a20 2023 20e8 aebe e7bd  00'))..  # .....
-000010a0: aee5 ad98 e582 a8e7 b1bb e59e 8be8 bdac  ................
-000010b0: e68d a2e8 a784 e588 99ef bc8c e7ad 9be9  ................
-000010c0: 8089 e589 8de7 bc80 e4b8 ba20 7072 6566  ........... pref
-000010d0: 6978 3320 e79a 8420 6f62 6a65 6374 73ef  ix3 ... objects.
-000010e0: bc8c e59c a8e5 85b6 e69c 80e5 908e e4bf  ................
-000010f0: aee6 94b9 e697 b6e9 97b4 3230 e5a4 a9e4  ..........20....
-00001100: b98b e590 8ee8 bdac e4b8 bae4 bd8e e9a2  ................
-00001110: 91e8 aebf e997 aee7 b1bb e59e 8bef bc8c  ................
-00001120: e59c a8e5 85b6 e69c 80e5 908e e4bf aee6  ................
-00001130: 94b9 e697 b6e9 97b4 3330 e5a4 a9e4 b98b  ........30......
-00001140: e590 8ee8 bdac e4b8 bae5 bd92 e6a1 a3e7  ................
-00001150: b1bb e59e 8be3 8082 0a20 2072 756c 6533  .........  rule3
-00001160: 203d 204c 6966 6563 7963 6c65 5275 6c65   = LifecycleRule
-00001170: 2827 7275 6c65 3327 2c20 4c69 6665 6379  ('rule3', Lifecy
-00001180: 636c 6546 696c 7465 7228 2770 7265 6669  cleFilter('prefi
-00001190: 7833 2729 2c0a 2020 2020 2020 2020 2020  x3'),.          
-000011a0: 2020 2020 2020 2020 2020 2020 2020 7374                st
-000011b0: 6174 7573 3d27 456e 6162 6c65 6427 2c0a  atus='Enabled',.
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 2020 2020 2020 2020 7472 616e 7369 7469          transiti
-000011e0: 6f6e 733d 5b4c 6966 6563 7963 6c65 5472  ons=[LifecycleTr
-000011f0: 616e 7369 7469 6f6e 2864 6179 733d 3230  ansition(days=20
-00001200: 2c20 7374 6f72 6167 655f 636c 6173 733d  , storage_class=
-00001210: 2753 5441 4e44 4152 445f 4941 2729 2c0a  'STANDARD_IA'),.
-00001220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001240: 2020 2020 204c 6966 6563 7963 6c65 5472       LifecycleTr
-00001250: 616e 7369 7469 6f6e 2864 6179 733d 3630  ansition(days=60
-00001260: 2c20 7374 6f72 6167 655f 636c 6173 733d  , storage_class=
-00001270: 2741 5243 4849 5645 2729 5d29 0a0a 2020  'ARCHIVE')])..  
-00001280: 2320 e8ae bee7 bdae e5ad 98e5 82a8 e7b1  # ..............
-00001290: bbe5 9e8b e8bd ace6 8da2 e8a7 84e5 8899  ................
-000012a0: efbc 8ce7 ad9b e980 89e5 898d e7bc 80e4  ................
-000012b0: b8ba 2070 7265 6669 7833 20e7 9a84 206f  .. prefix3 ... o
-000012c0: 626a 6563 7473 efbc 8ce6 9c80 e590 8ee4  bjects..........
-000012d0: bfae e694 b9e6 97b6 e997 b4e5 9ca8 e68c  ................
-000012e0: 87e5 ae9a e697 a5e6 9c9f e4b9 8be5 898d  ................
-000012f0: e79a 84ef bc8c e8bd ace4 b8ba e4bd 8ee9  ................
-00001300: a291 e8ae bfe9 97ae e7b1 bbe5 9e8b 0a20  ............... 
-00001310: 2072 756c 6534 203d 204c 6966 6563 7963   rule4 = Lifecyc
-00001320: 6c65 5275 6c65 2827 7275 6c65 3427 2c20  leRule('rule4', 
-00001330: 4c69 6665 6379 636c 6546 696c 7465 7228  LifecycleFilter(
-00001340: 2770 7265 6669 7834 2729 2c0a 2020 2020  'prefix4'),.    
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 2020 7374 6174 7573 3d27 456e 6162      status='Enab
-00001370: 6c65 6427 2c0a 2020 2020 2020 2020 2020  led',.          
-00001380: 2020 2020 2020 2020 2020 2020 2020 7472                tr
-00001390: 616e 7369 7469 6f6e 733d 5b0a 2020 2020  ansitions=[.    
-000013a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013b0: 2020 2020 2020 4c69 6665 6379 636c 6554        LifecycleT
-000013c0: 7261 6e73 6974 696f 6e28 6461 7465 3d64  ransition(date=d
-000013d0: 6174 6574 696d 6528 3230 3231 2c20 3132  atetime(2021, 12
-000013e0: 2c20 3132 292e 6973 6f66 6f72 6d61 7428  , 12).isoformat(
-000013f0: 7469 6d65 7370 6563 3d27 7365 636f 6e64  timespec='second
-00001400: 7327 2920 2b20 272b 3038 3a30 3027 2c0a  s') + '+08:00',.
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001430: 2020 2020 2020 2020 2020 2020 2020 7374                st
-00001440: 6f72 6167 655f 636c 6173 733d 2753 5441  orage_class='STA
-00001450: 4e44 4152 445f 4941 2729 5d29 0a0a 2020  NDARD_IA')])..  
-00001460: 2320 7072 696e 7428 7275 6c65 312e 746f  # print(rule1.to
-00001470: 5f78 6d6c 2829 290a 2020 2320 7072 696e  _xml()).  # prin
-00001480: 7428 7275 6c65 322e 746f 5f78 6d6c 2829  t(rule2.to_xml()
-00001490: 290a 2020 2320 7072 696e 7428 7275 6c65  ).  # print(rule
-000014a0: 332e 746f 5f78 6d6c 2829 290a 2020 2320  3.to_xml()).  # 
-000014b0: 7072 696e 7428 7275 6c65 342e 746f 5f78  print(rule4.to_x
-000014c0: 6d6c 2829 290a 2020 6c69 6665 6379 636c  ml()).  lifecycl
-000014d0: 6520 3d20 4275 636b 6574 4c69 6665 6379  e = BucketLifecy
-000014e0: 636c 6528 5b72 756c 6531 2c20 7275 6c65  cle([rule1, rule
-000014f0: 322c 2072 756c 6533 2c20 7275 6c65 345d  2, rule3, rule4]
-00001500: 293b 0a20 2062 7563 6b65 742e 7365 745f  );.  bucket.set_
-00001510: 6275 636b 6574 5f6c 6966 6563 7963 6c65  bucket_lifecycle
-00001520: 286c 6966 6563 7963 6c65 290a 0a64 6566  (lifecycle)..def
-00001530: 2064 656c 6574 6542 7563 6b65 744c 6966   deleteBucketLif
-00001540: 6543 7963 6c65 2862 7563 6b65 745f 6e61  eCycle(bucket_na
-00001550: 6d65 293a 0a20 2062 7563 6b65 7420 3d20  me):.  bucket = 
-00001560: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
-00001570: 6275 636b 6574 5f6e 616d 6529 0a20 2062  bucket_name).  b
-00001580: 7563 6b65 742e 6465 6c65 7465 5f62 7563  ucket.delete_buc
-00001590: 6b65 745f 6c69 6665 6379 636c 6528 290a  ket_lifecycle().
-000015a0: 0a64 6566 2067 6574 4275 636b 6574 4c6f  .def getBucketLo
-000015b0: 6767 696e 6728 6275 636b 6574 5f6e 616d  gging(bucket_nam
-000015c0: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
-000015d0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
-000015e0: 7563 6b65 745f 6e61 6d65 290a 2020 7072  ucket_name).  pr
-000015f0: 696e 7428 6275 636b 6574 2e67 6574 5f62  int(bucket.get_b
-00001600: 7563 6b65 745f 6c6f 6767 696e 6728 292e  ucket_logging().
-00001610: 746f 5f78 6d6c 2829 290a 0a64 6566 2073  to_xml())..def s
-00001620: 6574 4275 636b 6574 4c6f 6767 696e 6728  etBucketLogging(
-00001630: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
-00001640: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00001650: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00001660: 6e61 6d65 290a 2020 626c 6f67 6769 6e67  name).  blogging
-00001670: 203d 2042 7563 6b65 744c 6f67 6769 6e67   = BucketLogging
-00001680: 2874 6172 6765 743d 6275 636b 6574 5f6e  (target=bucket_n
-00001690: 616d 652c 2074 6172 6765 745f 7072 6566  ame, target_pref
-000016a0: 6978 3d27 7465 7374 5f6c 6f67 2729 0a20  ix='test_log'). 
-000016b0: 2070 7269 6e74 2862 7563 6b65 742e 7365   print(bucket.se
-000016c0: 745f 6275 636b 6574 5f6c 6f67 6769 6e67  t_bucket_logging
-000016d0: 2862 6c6f 6767 696e 672e 746f 5f78 6d6c  (blogging.to_xml
-000016e0: 2829 2929 0a0a 6465 6620 656e 6162 6c65  ()))..def enable
-000016f0: 4275 636b 6574 4c6f 6767 696e 6728 6275  BucketLogging(bu
-00001700: 636b 6574 5f6e 616d 6529 3a0a 2020 6275  cket_name):.  bu
-00001710: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
-00001720: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
-00001730: 6d65 290a 2020 7072 696e 7428 6275 636b  me).  print(buck
-00001740: 6574 2e65 6e61 626c 655f 6c6f 6767 696e  et.enable_loggin
-00001750: 6728 6275 636b 6574 2c20 7461 7267 6574  g(bucket, target
-00001760: 5f70 7265 6669 783d 2768 6568 6568 6568  _prefix='heheheh
-00001770: 6527 2929 0a0a 6465 6620 6469 7361 626c  e'))..def disabl
-00001780: 6542 7563 6b65 744c 6f67 6769 6e67 2862  eBucketLogging(b
-00001790: 7563 6b65 745f 6e61 6d65 293a 0a20 2062  ucket_name):.  b
-000017a0: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
-000017b0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
-000017c0: 616d 6529 0a20 2070 7269 6e74 2862 7563  ame).  print(buc
-000017d0: 6b65 742e 6469 7361 626c 655f 6c6f 6767  ket.disable_logg
-000017e0: 696e 6728 2929 0a0a 6465 6620 6765 7442  ing())..def getB
-000017f0: 7563 6b65 7443 6f72 7328 6275 636b 6574  ucketCors(bucket
-00001800: 5f6e 616d 6529 3a0a 2020 6275 636b 6574  _name):.  bucket
-00001810: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-00001820: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-00001830: 2020 7072 696e 7428 6275 636b 6574 2e67    print(bucket.g
-00001840: 6574 5f62 7563 6b65 745f 636f 7273 2829  et_bucket_cors()
-00001850: 2e74 6f5f 786d 6c28 2929 0a0a 6465 6620  .to_xml())..def 
-00001860: 7075 7442 7563 6b65 7443 6f72 7328 6275  putBucketCors(bu
-00001870: 636b 6574 5f6e 616d 6529 3a0a 2020 6275  cket_name):.  bu
-00001880: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
-00001890: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
-000018a0: 6d65 290a 2020 636f 7273 203d 2042 7563  me).  cors = Buc
-000018b0: 6b65 7443 6f72 7328 5b43 4f52 5352 756c  ketCors([CORSRul
-000018c0: 6528 6f72 6967 696e 733d 5b22 6874 7470  e(origins=["http
-000018d0: 3a2f 2f64 6576 2e6b 7379 756e 2e63 6f6d  ://dev.ksyun.com
-000018e0: 225d 2c20 6d65 7468 6f64 733d 5b22 4745  "], methods=["GE
-000018f0: 5422 2c20 2248 4541 4422 5d2c 206d 6178  T", "HEAD"], max
-00001900: 5f61 6765 3d22 3230 3022 2c20 6865 6164  _age="200", head
-00001910: 6572 733d 5b22 636f 6e74 656e 742d 7479  ers=["content-ty
-00001920: 7065 225d 2c20 6578 706f 7365 645f 6865  pe"], exposed_he
-00001930: 6164 6572 733d 5b22 636f 6e74 656e 742d  aders=["content-
-00001940: 7479 7065 222c 2022 782d 6b73 732d 6163  type", "x-kss-ac
-00001950: 6c22 5d29 5d29 0a20 2070 7269 6e74 2827  l"])]).  print('
-00001960: 636f 7273 3a20 272c 2063 6f72 732e 746f  cors: ', cors.to
-00001970: 5f78 6d6c 2829 290a 2020 7072 696e 7428  _xml()).  print(
-00001980: 6275 636b 6574 2e73 6574 5f62 7563 6b65  bucket.set_bucke
-00001990: 745f 636f 7273 2863 6f72 7329 290a 0a64  t_cors(cors))..d
-000019a0: 6566 2064 656c 6574 6542 7563 6b65 7443  ef deleteBucketC
-000019b0: 6f72 7328 6275 636b 6574 5f6e 616d 6529  ors(bucket_name)
-000019c0: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
-000019d0: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
-000019e0: 6b65 745f 6e61 6d65 290a 2020 7072 696e  ket_name).  prin
-000019f0: 7428 6275 636b 6574 2e64 656c 6574 655f  t(bucket.delete_
-00001a00: 6275 636b 6574 5f63 6f72 7328 2929 0a0a  bucket_cors())..
-00001a10: 6465 6620 6765 7442 7563 6b65 7443 7272  def getBucketCrr
-00001a20: 2862 7563 6b65 745f 6e61 6d65 293a 0a20  (bucket_name):. 
-00001a30: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
-00001a40: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-00001a50: 5f6e 616d 6529 0a20 2070 7269 6e74 2862  _name).  print(b
-00001a60: 7563 6b65 742e 6765 745f 6275 636b 6574  ucket.get_bucket
-00001a70: 5f63 7272 2829 2e74 6f5f 786d 6c28 2929  _crr().to_xml())
-00001a80: 0a0a 6465 6620 7365 7442 7563 6b65 7443  ..def setBucketC
-00001a90: 7272 2862 7563 6b65 745f 6e61 6d65 293a  rr(bucket_name):
-00001aa0: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
-00001ab0: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
-00001ac0: 6574 5f6e 616d 6529 0a20 2023 2064 656c  et_name).  # del
-00001ad0: 6574 654d 6172 6b65 7253 7461 7475 7320  eteMarkerStatus 
-00001ae0: e79a 84e5 80bc e4b8 ba20 456e 6162 6c65  ......... Enable
-00001af0: 6420 e592 8c20 4469 7361 626c 6564 0a20  d ... Disabled. 
-00001b00: 2070 7269 6e74 2862 7563 6b65 742e 7365   print(bucket.se
-00001b10: 745f 6275 636b 6574 5f63 7272 2827 7465  t_bucket_crr('te
-00001b20: 7374 2d62 7563 6b65 742d 7265 706c 6927  st-bucket-repli'
-00001b30: 2c20 6465 6c65 7465 4d61 726b 6572 5374  , deleteMarkerSt
-00001b40: 6174 7573 3d22 456e 6162 6c65 6422 2c20  atus="Enabled", 
-00001b50: 7072 6566 6978 3d5b 2768 656c 6c6f 275d  prefix=['hello']
-00001b60: 2929 0a0a 6465 6620 6465 6c65 7465 4275  ))..def deleteBu
-00001b70: 636b 6574 4372 7228 6275 636b 6574 5f6e  cketCrr(bucket_n
-00001b80: 616d 6529 3a0a 2020 6275 636b 6574 203d  ame):.  bucket =
-00001b90: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
-00001ba0: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-00001bb0: 7072 696e 7428 6275 636b 6574 2e64 656c  print(bucket.del
-00001bc0: 6574 655f 6275 636b 6574 5f63 7272 2829  ete_bucket_crr()
-00001bd0: 290a 0a64 6566 2067 6574 4275 636b 6574  )..def getBucket
-00001be0: 4c6f 6767 696e 6728 6275 636b 6574 5f6e  Logging(bucket_n
-00001bf0: 616d 6529 3a0a 2020 6275 636b 6574 203d  ame):.  bucket =
-00001c00: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
-00001c10: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-00001c20: 7072 696e 7428 6275 636b 6574 2e67 6574  print(bucket.get
-00001c30: 5f62 7563 6b65 745f 6c6f 6767 696e 6728  _bucket_logging(
-00001c40: 292e 746f 5f78 6d6c 2829 290a 0a64 6566  ).to_xml())..def
-00001c50: 2073 6574 4275 636b 6574 4c6f 6767 696e   setBucketLoggin
-00001c60: 6728 6275 636b 6574 5f6e 616d 6529 3a0a  g(bucket_name):.
-00001c70: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00001c80: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00001c90: 745f 6e61 6d65 290a 2020 626c 6f67 6769  t_name).  bloggi
-00001ca0: 6e67 203d 2042 7563 6b65 744c 6f67 6769  ng = BucketLoggi
-00001cb0: 6e67 2874 6172 6765 743d 6275 636b 6574  ng(target=bucket
-00001cc0: 5f6e 616d 6529 0a20 2070 7269 6e74 2862  _name).  print(b
-00001cd0: 7563 6b65 742e 7365 745f 6275 636b 6574  ucket.set_bucket
-00001ce0: 5f6c 6f67 6769 6e67 2862 6c6f 6767 696e  _logging(bloggin
-00001cf0: 672e 746f 5f78 6d6c 2829 2929 0a0a 6465  g.to_xml()))..de
-00001d00: 6620 6765 7442 7563 6b65 744d 6972 726f  f getBucketMirro
-00001d10: 7228 6275 636b 6574 5f6e 616d 6529 3a0a  r(bucket_name):.
-00001d20: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
-00001d30: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
-00001d40: 745f 6e61 6d65 290a 2020 7072 696e 7428  t_name).  print(
-00001d50: 6275 636b 6574 2e67 6574 5f62 7563 6b65  bucket.get_bucke
-00001d60: 745f 6d69 7272 6f72 2829 290a 0a64 6566  t_mirror())..def
-00001d70: 2073 6574 4275 636b 6574 4d69 7272 6f72   setBucketMirror
-00001d80: 2862 7563 6b65 745f 6e61 6d65 293a 0a20  (bucket_name):. 
-00001d90: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
-00001da0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-00001db0: 5f6e 616d 6529 0a20 2073 6574 5f68 6561  _name).  set_hea
-00001dc0: 6465 7273 203d 205b 7b0a 2020 2020 2020  ders = [{.      
-00001dd0: 226b 6579 223a 2022 6422 2c0a 2020 2020  "key": "d",.    
-00001de0: 2020 2276 616c 7565 223a 2022 6222 0a20    "value": "b". 
-00001df0: 207d 5d0a 2020 7265 6d6f 7665 5f68 6561   }].  remove_hea
-00001e00: 6465 7273 203d 205b 7b0a 2020 2020 2020  ders = [{.      
-00001e10: 226b 6579 223a 2022 6422 0a20 207d 5d0a  "key": "d".  }].
-00001e20: 2020 7061 7373 5f68 6561 6465 7273 203d    pass_headers =
-00001e30: 205b 7b0a 2020 2020 2020 226b 6579 223a   [{.      "key":
-00001e40: 2022 6162 6322 0a20 207d 5d0a 2020 6865   "abc".  }].  he
-00001e50: 6164 6572 5f73 6574 7469 6e67 203d 2048  ader_setting = H
-00001e60: 6561 6465 7253 6574 7469 6e67 2873 6574  eaderSetting(set
-00001e70: 5f68 6561 6465 7273 3d73 6574 5f68 6561  _headers=set_hea
-00001e80: 6465 7273 2c20 7265 6d6f 7665 5f68 6561  ders, remove_hea
-00001e90: 6465 7273 3d72 656d 6f76 655f 6865 6164  ders=remove_head
-00001ea0: 6572 732c 2070 6173 735f 616c 6c3d 4661  ers, pass_all=Fa
-00001eb0: 6c73 652c 2070 6173 735f 6865 6164 6572  lse, pass_header
-00001ec0: 733d 7061 7373 5f68 6561 6465 7273 290a  s=pass_headers).
-00001ed0: 2020 6d69 7272 6f72 5f72 6571 7565 7374    mirror_request
-00001ee0: 5f73 6574 7469 6e67 203d 204d 6972 726f  _setting = Mirro
-00001ef0: 7252 6571 7565 7374 5365 7474 696e 6728  rRequestSetting(
-00001f00: 7061 7373 5f71 7565 7279 5f73 7472 696e  pass_query_strin
-00001f10: 673d 4661 6c73 652c 2066 6f6c 6c6f 7733  g=False, follow3
-00001f20: 7878 3d46 616c 7365 2c20 6865 6164 6572  xx=False, header
-00001f30: 5f73 6574 7469 6e67 3d68 6561 6465 725f  _setting=header_
-00001f40: 7365 7474 696e 6729 0a20 2061 7379 6e63  setting).  async
-00001f50: 5f6d 6972 726f 725f 7275 6c65 203d 2041  _mirror_rule = A
-00001f60: 7379 6e63 4d69 7272 6f72 5275 6c65 2e72  syncMirrorRule.r
-00001f70: 756c 655f 7769 7468 5f61 636c 286d 6972  ule_with_acl(mir
-00001f80: 726f 725f 7572 6c73 3d5b 2268 7474 703a  ror_urls=["http:
-00001f90: 2f2f 6162 632e 6f6d 222c 2022 6874 7470  //abc.om", "http
-00001fa0: 3a2f 2f77 7777 2e77 7073 2e63 6e22 5d2c  ://www.wps.cn"],
-00001fb0: 2073 6176 696e 675f 7365 7474 696e 675f   saving_setting_
-00001fc0: 6163 6c3d 2270 7269 7661 7465 2229 0a20  acl="private"). 
-00001fd0: 2073 796e 635f 6d69 7272 6f72 5f72 756c   sync_mirror_rul
-00001fe0: 6573 203d 2053 796e 634d 6972 726f 7252  es = SyncMirrorR
-00001ff0: 756c 6573 2e72 756c 6573 5f77 6974 685f  ules.rules_with_
-00002000: 7072 6566 6978 5f61 636c 286b 6579 5f70  prefix_acl(key_p
-00002010: 7265 6669 7865 733d 5b22 6162 6322 5d2c  refixes=["abc"],
-00002020: 206d 6972 726f 725f 7572 6c3d 2268 7474   mirror_url="htt
-00002030: 703a 2f2f 762d 6b73 2d61 2d69 2e6f 7269  p://v-ks-a-i.ori
-00002040: 6769 6e61 6c76 6f64 2e63 6f6d 222c 206d  ginalvod.com", m
-00002050: 6972 726f 725f 7265 7175 6573 745f 7365  irror_request_se
-00002060: 7474 696e 673d 6d69 7272 6f72 5f72 6571  tting=mirror_req
-00002070: 7565 7374 5f73 6574 7469 6e67 2c20 7361  uest_setting, sa
-00002080: 7669 6e67 5f73 6574 7469 6e67 5f61 636c  ving_setting_acl
-00002090: 3d22 7072 6976 6174 6522 290a 2020 6d69  ="private").  mi
-000020a0: 7272 6f72 203d 2042 7563 6b65 744d 6972  rror = BucketMir
-000020b0: 726f 7228 7573 655f 6465 6661 756c 745f  ror(use_default_
-000020c0: 726f 626f 7473 3d46 616c 7365 2c20 6173  robots=False, as
-000020d0: 796e 635f 6d69 7272 6f72 5f72 756c 653d  ync_mirror_rule=
-000020e0: 6173 796e 635f 6d69 7272 6f72 5f72 756c  async_mirror_rul
-000020f0: 652c 2073 796e 635f 6d69 7272 6f72 5f72  e, sync_mirror_r
-00002100: 756c 6573 3d5b 7379 6e63 5f6d 6972 726f  ules=[sync_mirro
-00002110: 725f 7275 6c65 735d 290a 2020 7072 696e  r_rules]).  prin
-00002120: 7428 6275 636b 6574 2e73 6574 5f62 7563  t(bucket.set_buc
-00002130: 6b65 745f 6d69 7272 6f72 286d 6972 726f  ket_mirror(mirro
-00002140: 7229 290a 0a64 6566 2064 656c 6574 6542  r))..def deleteB
-00002150: 7563 6b65 744d 6972 726f 7228 6275 636b  ucketMirror(buck
-00002160: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
-00002170: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00002180: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00002190: 290a 2020 7072 696e 7428 6275 636b 6574  ).  print(bucket
-000021a0: 2e64 656c 6574 655f 6275 636b 6574 5f6d  .delete_bucket_m
-000021b0: 6972 726f 7228 2929 0a0a 2323 2323 2323  irror())..######
-000021c0: 2323 2323 2323 2323 2323 2323 2323 2320  ############### 
-000021d0: 206b 7333 2e62 696c 6c69 6e67 2020 2323   ks3.billing  ##
-000021e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000021f0: 2323 2323 2323 2323 230a 6672 6f6d 206b  #########.from k
-00002200: 7333 2e62 696c 6c69 6e67 2069 6d70 6f72  s3.billing impor
-00002210: 7420 6765 745f 6275 636b 6574 735f 6461  t get_buckets_da
-00002220: 7461 0a0a 6465 6620 6765 7442 7563 6b65  ta..def getBucke
-00002230: 7473 4461 7461 2862 7563 6b65 745f 6e61  tsData(bucket_na
-00002240: 6d65 733d 4e6f 6e65 293a 0a20 2064 6174  mes=None):.  dat
-00002250: 6120 3d20 6765 745f 6275 636b 6574 735f  a = get_buckets_
-00002260: 6461 7461 2861 6b2c 2073 6b2c 2073 7461  data(ak, sk, sta
-00002270: 7274 5f74 696d 653d 2232 3032 3131 3131  rt_time="2021111
-00002280: 3932 3330 3022 2c20 656e 645f 7469 6d65  92300", end_time
-00002290: 3d22 3230 3231 3131 3139 3233 3539 222c  ="202111192359",
-000022a0: 2062 7563 6b65 745f 6e61 6d65 733d 6275   bucket_names=bu
-000022b0: 636b 6574 5f6e 616d 6573 2c20 7072 6f64  cket_names, prod
-000022c0: 7563 7473 3d22 4461 7461 5369 7a65 2c52  ucts="DataSize,R
-000022d0: 6571 7565 7374 7347 6574 2229 0a20 2070  equestsGet").  p
-000022e0: 7269 6e74 2864 6174 6129 0a0a 2323 2323  rint(data)..####
-000022f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002300: 2320 206b 7333 2e6f 626a 6563 7420 2023  #  ks3.object  #
-00002310: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002320: 2323 2323 2323 2323 2323 0a64 6566 2067  ##########.def g
-00002330: 6574 4f62 6a65 6374 4d65 7461 2862 7563  etObjectMeta(buc
-00002340: 6b65 745f 6e61 6d65 2c20 6f62 6a65 6374  ket_name, object
-00002350: 5f6b 6579 5f6e 616d 652c 2068 6561 6465  _key_name, heade
-00002360: 7273 3d4e 6f6e 6529 3a0a 2020 6275 636b  rs=None):.  buck
-00002370: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00002380: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00002390: 290a 2020 7265 7370 203d 2062 7563 6b65  ).  resp = bucke
-000023a0: 742e 6765 745f 6b65 795f 6d65 7461 286f  t.get_key_meta(o
-000023b0: 626a 6563 745f 6b65 795f 6e61 6d65 2c20  bject_key_name, 
-000023c0: 6865 6164 6572 733d 6865 6164 6572 7329  headers=headers)
-000023d0: 0a20 2069 6620 7265 7370 3a0a 2020 2020  .  if resp:.    
-000023e0: 7072 696e 7428 22e8 8eb7 e58f 96e6 9687  print(".........
-000023f0: e4bb b668 6561 6465 72e6 8890 e58a 9f3a  ...header......:
-00002400: 2022 2c20 7265 7370 2e68 6561 6465 7273   ", resp.headers
-00002410: 290a 0a64 6566 2075 706c 6f61 644f 626a  )..def uploadObj
-00002420: 6563 7446 726f 6d46 696c 6528 6669 6c65  ectFromFile(file
-00002430: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
-00002440: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
-00002450: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
-00002460: 206b 203d 2062 7563 6b65 742e 6e65 775f   k = bucket.new_
-00002470: 6b65 7928 6669 6c65 6e61 6d65 290a 2020  key(filename).  
-00002480: 7265 7420 3d20 6b2e 7365 745f 636f 6e74  ret = k.set_cont
-00002490: 656e 7473 5f66 726f 6d5f 6669 6c65 6e61  ents_from_filena
-000024a0: 6d65 286f 732e 7061 7468 2e65 7870 616e  me(os.path.expan
-000024b0: 6475 7365 7228 227e 2229 202b 2027 2f44  duser("~") + '/D
-000024c0: 6f77 6e6c 6f61 6473 2f27 202b 2066 696c  ownloads/' + fil
-000024d0: 656e 616d 6529 0a20 2069 6620 7265 7420  ename).  if ret 
-000024e0: 616e 6420 7265 742e 7374 6174 7573 203d  and ret.status =
-000024f0: 3d20 3230 303a 0a20 2020 2070 7269 6e74  = 200:.    print
-00002500: 2822 e4b8 8ae4 bca0 e688 90e5 8a9f 2229  ("............")
-00002510: 0a0a 6465 6620 7570 6c6f 6164 5f61 7379  ..def upload_asy
-00002520: 6e63 2866 696c 656e 616d 6529 3a0a 2020  nc(filename):.  
-00002530: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00002540: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00002550: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
-00002560: 6574 2e6e 6577 5f6b 6579 2866 696c 656e  et.new_key(filen
-00002570: 616d 6529 0a20 2072 6574 203d 2061 7379  ame).  ret = asy
-00002580: 6e63 696f 2e72 756e 286b 2e75 706c 6f61  ncio.run(k.uploa
-00002590: 645f 6669 6c65 5f61 7379 6e63 286f 732e  d_file_async(os.
-000025a0: 7061 7468 2e65 7870 616e 6475 7365 7228  path.expanduser(
-000025b0: 227e 2229 202b 2027 2f44 6f77 6e6c 6f61  "~") + '/Downloa
-000025c0: 6473 2f27 202b 2066 696c 656e 616d 6529  ds/' + filename)
-000025d0: 290a 2020 6966 2072 6574 2061 6e64 2072  ).  if ret and r
-000025e0: 6574 2e73 7461 7475 7320 3d3d 2032 3030  et.status == 200
-000025f0: 3a0a 2020 2020 7072 696e 7428 22e4 b88a  :.    print("...
-00002600: e4bc a0e6 8890 e58a 9f22 290a 0a64 6566  .........")..def
-00002610: 2075 706c 6f61 644f 626a 6563 7446 726f   uploadObjectFro
-00002620: 6d53 7472 696e 6728 293a 0a20 2062 7563  mString():.  buc
-00002630: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
-00002640: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-00002650: 6529 0a20 206b 203d 2062 7563 6b65 742e  e).  k = bucket.
-00002660: 6e65 775f 6b65 7928 27e5 a4a7 e5ae b6e5  new_key('.......
-00002670: a5bd 2729 0a20 2023 2023 206b 6579 20e5  ..').  # # key .
-00002680: 928c 2076 616c 7565 20e9 9c80 e8a6 8120  .. value ...... 
-00002690: 7572 6c20 e7bc 96e7 a081 0a20 2023 2074  url .......  # t
-000026a0: 6167 6769 6e67 5374 7220 3d20 276e 616d  aggingStr = 'nam
-000026b0: 653d 6a68 270a 2020 2320 6865 6164 6572  e=jh'.  # header
-000026c0: 7320 3d20 7b27 782d 6b73 732d 7461 6767  s = {'x-kss-tagg
-000026d0: 696e 6727 3a20 7461 6767 696e 6753 7472  ing': taggingStr
-000026e0: 7d0a 2020 7265 7420 3d20 6b2e 7365 745f  }.  ret = k.set_
-000026f0: 636f 6e74 656e 7473 5f66 726f 6d5f 7374  contents_from_st
-00002700: 7269 6e67 2827 2077 6f72 6c64 2729 0a20  ring(' world'). 
-00002710: 2023 2023 20e8 afb7 e6b1 8249 44e3 8082   # # ......ID...
-00002720: e8af b7e6 b182 4944 e698 afe6 9cac e6ac  ......ID........
-00002730: a1e8 afb7 e6b1 82e7 9a84 e594 afe4 b880  ................
-00002740: e6a0 87e8 af86 efbc 8ce5 bcba e783 88e5  ................
-00002750: bbba e8ae aee5 9ca8 e7a8 8be5 ba8f e697  ................
-00002760: a5e5 bf97 e4b8 ade6 b7bb e58a a0e6 ada4  ................
-00002770: e58f 82e6 95b0 e380 820a 2020 2320 7072  ..........  # pr
-00002780: 696e 7428 7265 742e 6865 6164 6572 735b  int(ret.headers[
-00002790: 2778 2d6b 7373 2d72 6571 7565 7374 2d69  'x-kss-request-i
-000027a0: 6427 5d29 0a20 2023 2023 2045 5461 67e6  d']).  # # ETag.
-000027b0: 98af 7075 745f 6f62 6a65 6374 e696 b9e6  ..put_object....
-000027c0: b395 e8bf 94e5 9b9e e580 bce7 89b9 e69c  ................
-000027d0: 89e7 9a84 e5b1 9ee6 80a7 efbc 8ce7 94a8  ................
-000027e0: e4ba 8ee6 a087 e8af 86e4 b880 e4b8 aa4f  ...............O
-000027f0: 626a 6563 74e7 9a84 e586 85e5 aeb9 e380  bject...........
-00002800: 820a 2020 2320 7072 696e 7428 7265 742e  ..  # print(ret.
-00002810: 6865 6164 6572 7329 0a20 2023 2048 5454  headers).  # HTT
-00002820: 50e8 bf94 e59b 9ee7 a081 e380 820a 2020  P.............  
-00002830: 6966 2072 6574 2061 6e64 2072 6574 2e73  if ret and ret.s
-00002840: 7461 7475 7320 3d3d 2032 3030 3a0a 2020  tatus == 200:.  
-00002850: 2020 7072 696e 7428 22e4 b88a e4bc a0e6    print(".......
-00002860: 8890 e58a 9f22 290a 0a64 6566 2068 6561  .....")..def hea
-00002870: 644f 626a 6563 7428 293a 0a20 2062 7563  dObject():.  buc
-00002880: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
-00002890: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-000028a0: 6529 0a20 206b 203d 2062 7563 6b65 742e  e).  k = bucket.
-000028b0: 6765 745f 6b65 7928 2774 6573 745f 656e  get_key('test_en
-000028c0: 6372 7970 7469 6f6e 2729 0a20 2069 6620  cryption').  if 
-000028d0: 6b3a 0a20 2020 2070 7269 6e74 286b 2e6e  k:.    print(k.n
-000028e0: 616d 652c 206b 2e73 697a 652c 206b 2e6c  ame, k.size, k.l
-000028f0: 6173 745f 6d6f 6469 6669 6564 2c20 6b2e  ast_modified, k.
-00002900: 6f62 6a65 6374 5f74 7970 652c 206b 2e74  object_type, k.t
-00002910: 6167 6769 6e67 5f63 6f75 6e74 290a 0a64  agging_count)..d
-00002920: 6566 2064 6f77 6e6c 6f61 644f 626a 6563  ef downloadObjec
-00002930: 7441 6e64 5072 696e 7428 6b65 796e 616d  tAndPrint(keynam
-00002940: 652c 2062 7974 655f 7261 6e67 653d 2830  e, byte_range=(0
-00002950: 2c20 3129 2c20 6865 6164 6572 733d 4e6f  , 1), headers=No
-00002960: 6e65 293a 0a20 2062 7563 6b65 7420 3d20  ne):.  bucket = 
-00002970: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
-00002980: 6275 636b 6574 5f6e 616d 6529 0a20 206b  bucket_name).  k
-00002990: 203d 2062 7563 6b65 742e 6765 745f 6b65   = bucket.get_ke
-000029a0: 7928 6b65 796e 616d 6529 0a20 2073 203d  y(keyname).  s =
-000029b0: 206b 2e67 6574 5f63 6f6e 7465 6e74 735f   k.get_contents_
-000029c0: 6173 5f73 7472 696e 6728 6279 7465 5f72  as_string(byte_r
-000029d0: 616e 6765 3d62 7974 655f 7261 6e67 652c  ange=byte_range,
-000029e0: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
-000029f0: 292e 6465 636f 6465 2829 0a20 2070 7269  ).decode().  pri
-00002a00: 6e74 2873 290a 0a64 6566 2064 6f77 6e6c  nt(s)..def downl
-00002a10: 6f61 645f 6173 796e 6328 6b65 796e 616d  oad_async(keynam
-00002a20: 652c 2068 6561 6465 7273 3d4e 6f6e 6529  e, headers=None)
-00002a30: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
-00002a40: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
-00002a50: 6b65 745f 6e61 6d65 290a 2020 6b20 3d20  ket_name).  k = 
-00002a60: 6275 636b 6574 2e67 6574 5f6b 6579 286b  bucket.get_key(k
-00002a70: 6579 6e61 6d65 290a 2020 7472 793a 0a20  eyname).  try:. 
-00002a80: 2020 2061 7379 6e63 696f 2e72 756e 286b     asyncio.run(k
-00002a90: 2e64 6f77 6e6c 6f61 645f 6669 6c65 5f61  .download_file_a
-00002aa0: 7379 6e63 286f 732e 7061 7468 2e65 7870  sync(os.path.exp
-00002ab0: 616e 6475 7365 7228 227e 2229 202b 2027  anduser("~") + '
-00002ac0: 2f44 6f77 6e6c 6f61 6473 2f27 202b 206b  /Downloads/' + k
-00002ad0: 6579 6e61 6d65 2929 0a20 2020 2070 7269  eyname)).    pri
-00002ae0: 6e74 2827 e4b8 8be8 bdbd e688 90e5 8a9f  nt('............
-00002af0: 2729 0a20 2065 7863 6570 743a 0a20 2020  ').  except:.   
-00002b00: 2070 7269 6e74 2827 e4b8 8be8 bdbd e5a4   print('........
-00002b10: b1e8 b4a5 2729 0a0a 6465 6620 646f 776e  ....')..def down
-00002b20: 6c6f 6164 4f62 6a65 6374 4173 5374 7265  loadObjectAsStre
-00002b30: 616d 416e 6450 7269 6e74 2829 3a0a 2020  amAndPrint():.  
-00002b40: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
-00002b50: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
-00002b60: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
-00002b70: 6574 2e67 6574 5f6b 6579 2827 7368 616b  et.get_key('shak
-00002b80: 652e 7478 7427 290a 2020 6279 7465 7320  e.txt').  bytes 
-00002b90: 3d20 6b2e 7265 6164 2833 3030 290a 2020  = k.read(300).  
-00002ba0: 7072 696e 7428 2773 7461 7274 3a20 272c  print('start: ',
-00002bb0: 2064 6174 6574 696d 652e 6e6f 7728 292e   datetime.now().
-00002bc0: 7374 7266 7469 6d65 2822 2559 2d25 6d2d  strftime("%Y-%m-
-00002bd0: 2564 2025 483a 254d 3a25 532e 2566 2229  %d %H:%M:%S.%f")
-00002be0: 290a 2020 7768 696c 6520 6279 7465 733a  ).  while bytes:
-00002bf0: 0a20 2020 2073 203d 2062 7974 6573 2e64  .    s = bytes.d
-00002c00: 6563 6f64 6528 290a 2020 2020 7072 696e  ecode().    prin
-00002c10: 7428 2762 7974 6573 2064 6563 6f64 6564  t('bytes decoded
-00002c20: 3a27 2c20 7329 0a20 2020 2074 696d 652e  :', s).    time.
-00002c30: 736c 6565 7028 3529 0a20 2020 2062 7974  sleep(5).    byt
-00002c40: 6573 203d 206b 2e72 6561 6428 3330 3029  es = k.read(300)
-00002c50: 0a20 2070 7269 6e74 2827 656e 643a 2027  .  print('end: '
-00002c60: 2c20 6461 7465 7469 6d65 2e6e 6f77 2829  , datetime.now()
-00002c70: 2e73 7472 6674 696d 6528 2225 592d 256d  .strftime("%Y-%m
-00002c80: 2d25 6420 2548 3a25 4d3a 2553 2e25 6622  -%d %H:%M:%S.%f"
-00002c90: 2929 0a0a 6465 6620 646f 776e 6c6f 6164  ))..def download
-00002ca0: 4f62 6a65 6374 416e 6453 6176 6528 6b65  ObjectAndSave(ke
-00002cb0: 795f 6e61 6d65 2c20 6279 7465 5f72 616e  y_name, byte_ran
-00002cc0: 6765 3d28 302c 2031 292c 2068 6561 6465  ge=(0, 1), heade
-00002cd0: 7273 3d4e 6f6e 6529 3a0a 2020 6275 636b  rs=None):.  buck
-00002ce0: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
-00002cf0: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
-00002d00: 290a 2020 6b20 3d20 6275 636b 6574 2e67  ).  k = bucket.g
-00002d10: 6574 5f6b 6579 286b 6579 5f6e 616d 6529  et_key(key_name)
-00002d20: 0a20 206b 2e67 6574 5f63 6f6e 7465 6e74  .  k.get_content
-00002d30: 735f 746f 5f66 696c 656e 616d 6528 272f  s_to_filename('/
-00002d40: 5573 6572 732f 6a61 6262 6172 2f44 6f77  Users/jabbar/Dow
-00002d50: 6e6c 6f61 6473 2f44 5343 3033 3338 302e  nloads/DSC03380.
-00002d60: 656e 6372 7970 742e e99d 9ee5 8886 e59d  encrypt.........
-00002d70: 972e 6a70 672e 646f 776e 6c6f 6164 272c  ..jpg.download',
-00002d80: 2068 6561 6465 7273 3d68 6561 6465 7273   headers=headers
-00002d90: 290a 0a64 6566 2064 656c 6574 654f 626a  )..def deleteObj
-00002da0: 6563 7428 6b65 795f 6e61 6d65 293a 0a20  ect(key_name):. 
-00002db0: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
-00002dc0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-00002dd0: 5f6e 616d 6529 0a20 2074 7279 3a0a 2020  _name).  try:.  
-00002de0: 2020 6275 636b 6574 2e64 656c 6574 655f    bucket.delete_
-00002df0: 6b65 7928 6b65 795f 6e61 6d65 290a 2020  key(key_name).  
-00002e00: 2020 7072 696e 7428 22e5 88a0 e999 a4e6    print(".......
-00002e10: 8890 e58a 9f22 290a 2020 6578 6365 7074  .....").  except
-00002e20: 2045 7863 6570 7469 6f6e 2061 7320 653a   Exception as e:
-00002e30: 0a20 2020 2070 7269 6e74 2822 e588 a0e9  .    print("....
-00002e40: 99a4 e5a4 b1e8 b4a5 2229 0a20 2020 2070  ........").    p
-00002e50: 7269 6e74 2865 290a 2020 2020 7061 7373  rint(e).    pass
-00002e60: 0a0a 6465 6620 6765 744f 626a 6563 7441  ..def getObjectA
-00002e70: 636c 2829 3a0a 2020 6275 636b 6574 203d  cl():.  bucket =
-00002e80: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
-00002e90: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
-00002ea0: 706f 6c69 6379 203d 2062 7563 6b65 742e  policy = bucket.
-00002eb0: 6765 745f 6163 6c28 2761 7274 6963 6c65  get_acl('article
-00002ec0: 2e74 7874 2729 0a20 2070 7269 6e74 2870  .txt').  print(p
-00002ed0: 6f6c 6963 792e 746f 5f78 6d6c 2829 290a  olicy.to_xml()).
-00002ee0: 0a64 6566 2073 6574 4f62 6a65 6374 4163  .def setObjectAc
-00002ef0: 6c28 293a 0a20 2062 7563 6b65 7420 3d20  l():.  bucket = 
-00002f00: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
-00002f10: 6275 636b 6574 5f6e 616d 6529 0a20 2023  bucket_name).  #
-00002f20: 206f 626a 6563 7420 706f 6c69 6379 203a   object policy :
-00002f30: 2070 7269 7661 7465 207c 2070 7562 6c69   private | publi
-00002f40: 632d 7265 6164 207c 2070 7562 6c69 632d  c-read | public-
-00002f50: 7265 6164 2d77 7269 7465 0a20 2062 7563  read-write.  buc
-00002f60: 6b65 742e 7365 745f 6163 6c28 2270 7562  ket.set_acl("pub
-00002f70: 6c69 632d 7265 6164 222c 2027 3c59 4f55  lic-read", '<YOU
-00002f80: 525f 4b45 595f 4e41 4d45 3e27 290a 0a64  R_KEY_NAME>')..d
-00002f90: 6566 2073 6574 4f62 6a65 6374 4d65 7461  ef setObjectMeta
-00002fa0: 2829 3a0a 2020 6220 3d20 636f 6e6e 2e67  ():.  b = conn.g
-00002fb0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-00002fc0: 5f6e 616d 6529 0a20 2062 2e63 6f70 795f  _name).  b.copy_
-00002fd0: 6b65 7928 273c 796f 7572 4b65 794e 616d  key('<yourKeyNam
-00002fe0: 653e 272c 2027 3c79 6f75 7242 7563 6b65  e>', '<yourBucke
-00002ff0: 744e 616d 653e 272c 2027 3c79 6f75 724b  tName>', '<yourK
-00003000: 6579 4e61 6d65 3e27 2c0a 2020 2020 2020  eyName>',.      
-00003010: 2020 2020 2020 2068 6561 6465 7273 3d7b         headers={
-00003020: 2763 6f6e 7465 6e74 2d74 7970 6527 3a20  'content-type': 
-00003030: 2774 6578 742f 706c 6169 6e27 2c20 2778  'text/plain', 'x
-00003040: 2d6b 7373 2d6d 6574 6164 6174 612d 6469  -kss-metadata-di
-00003050: 7265 6374 6976 6527 3a20 2752 4550 4c41  rective': 'REPLA
-00003060: 4345 277d 290a 0a64 6566 2073 6574 4f62  CE'})..def setOb
-00003070: 6a65 6374 5374 6f72 6167 6543 6c61 7373  jectStorageClass
-00003080: 2829 3a0a 2020 6220 3d20 636f 6e6e 2e67  ():.  b = conn.g
-00003090: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-000030a0: 5f6e 616d 6529 0a20 2062 2e63 6f70 795f  _name).  b.copy_
-000030b0: 6b65 7928 273c 796f 7572 4b65 794e 616d  key('<yourKeyNam
-000030c0: 653e 272c 2027 3c79 6f75 7242 7563 6b65  e>', '<yourBucke
-000030d0: 744e 616d 653e 272c 2027 3c79 6f75 724b  tName>', '<yourK
-000030e0: 6579 4e61 6d65 3e27 2c20 6865 6164 6572  eyName>', header
-000030f0: 733d 7b27 782d 6b73 732d 7374 6f72 6167  s={'x-kss-storag
-00003100: 652d 636c 6173 7327 3a20 2753 5441 4e44  e-class': 'STAND
-00003110: 4152 445f 4941 277d 290a 0a64 6566 2063  ARD_IA'})..def c
-00003120: 6f70 7928 6473 744b 6579 2c20 7372 634b  opy(dstKey, srcK
-00003130: 6579 2c20 6473 745f 6275 636b 6574 5f6e  ey, dst_bucket_n
-00003140: 616d 653d 4e6f 6e65 2c20 6865 6164 6572  ame=None, header
-00003150: 733d 4e6f 6e65 293a 0a20 2023 2062 7563  s=None):.  # buc
-00003160: 6b65 745f 6e61 6d65 203d 2027 6861 7070  ket_name = 'happ
-00003170: 7968 6f75 7227 0a20 2062 203d 2063 6f6e  yhour'.  b = con
-00003180: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
-00003190: 6b65 745f 6e61 6d65 290a 2020 7265 7475  ket_name).  retu
-000031a0: 726e 2062 2e63 6f70 795f 6b65 7928 6473  rn b.copy_key(ds
-000031b0: 744b 6579 2c20 6473 745f 6275 636b 6574  tKey, dst_bucket
-000031c0: 5f6e 616d 652c 2073 7263 4b65 792c 2068  _name, srcKey, h
-000031d0: 6561 6465 7273 3d68 6561 6465 7273 290a  eaders=headers).
-000031e0: 0a64 6566 2063 6f70 795f 656e 6372 7970  .def copy_encryp
-000031f0: 7469 6f6e 2864 7374 4b65 792c 2073 7263  tion(dstKey, src
-00003200: 4b65 792c 2065 6e63 7279 7074 5f6b 6579  Key, encrypt_key
-00003210: 3d4e 6f6e 6529 3a0a 2020 6220 3d20 636f  =None):.  b = co
-00003220: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
-00003230: 636b 6574 5f6e 616d 6529 0a20 2062 2e63  cket_name).  b.c
-00003240: 6f70 795f 6b65 7928 6473 744b 6579 2c20  opy_key(dstKey, 
-00003250: 6275 636b 6574 5f6e 616d 652c 2073 7263  bucket_name, src
-00003260: 4b65 792c 2065 6e63 7279 7074 5f6b 6579  Key, encrypt_key
-00003270: 3d65 6e63 7279 7074 5f6b 6579 290a 0a64  =encrypt_key)..d
-00003280: 6566 206c 6973 745f 6f62 6a65 6374 7328  ef list_objects(
-00003290: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
-000032a0: 6e6e 2e67 6574 5f62 7563 6b65 7428 2774  nn.get_bucket('t
-000032b0: 6573 742d 6275 636b 6574 2729 0a20 206b  est-bucket').  k
-000032c0: 6579 7320 3d20 6275 636b 6574 2e6c 6973  eys = bucket.lis
-000032d0: 7428 7072 6566 6978 3d27 3136 2729 0a20  t(prefix='16'). 
-000032e0: 2072 6573 3120 3d20 5b6b 2e6e 616d 6520   res1 = [k.name 
-000032f0: 666f 7220 6b20 696e 206b 6579 735d 0a20  for k in keys]. 
-00003300: 2070 7269 6e74 2827 7265 7331 203a 2027   print('res1 : '
-00003310: 2c20 7265 7331 290a 0a20 206b 6579 7332  , res1)..  keys2
-00003320: 203d 2062 7563 6b65 742e 6c69 7374 4f62   = bucket.listOb
-00003330: 6a65 6374 7328 7072 6566 6978 3d27 3136  jects(prefix='16
-00003340: 2729 0a20 2023 2072 6573 3220 3d20 5b6b  ').  # res2 = [k
-00003350: 2e6e 616d 6520 666f 7220 6b20 696e 206b  .name for k in k
-00003360: 6579 7332 5d0a 2020 7072 696e 7428 276b  eys2].  print('k
-00003370: 6579 7332 203a 2027 2c20 6b65 7973 3229  eys2 : ', keys2)
-00003380: 0a20 2023 2066 6f72 206b 2069 6e20 6b65  .  # for k in ke
-00003390: 7973 3a0a 2020 2320 2020 7072 696e 7428  ys:.  #   print(
-000033a0: 276f 626a 6563 743a 272c 206b 2e6e 616d  'object:', k.nam
-000033b0: 6529 0a0a 6465 6620 6c69 7374 5f6f 626a  e)..def list_obj
-000033c0: 6563 7473 5f76 3228 6465 6c69 6d69 7465  ects_v2(delimite
-000033d0: 723d 2723 272c 2070 7265 6669 783d 4e6f  r='#', prefix=No
-000033e0: 6e65 2c20 6d61 785f 6b65 7973 3d4e 6f6e  ne, max_keys=Non
-000033f0: 652c 206d 6172 6b65 723d 4e6f 6e65 2c20  e, marker=None, 
-00003400: 656e 636f 6469 6e67 5f74 7970 653d 2727  encoding_type=''
-00003410: 2c20 6665 7463 685f 6f77 6e65 723d 5472  , fetch_owner=Tr
-00003420: 7565 293a 0a20 2062 7563 6b65 7420 3d20  ue):.  bucket = 
-00003430: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
-00003440: 6275 636b 6574 5f6e 616d 6529 0a20 206b  bucket_name).  k
-00003450: 6579 7320 3d20 6275 636b 6574 2e6c 6973  eys = bucket.lis
-00003460: 745f 7632 2864 656c 696d 6974 6572 3d64  t_v2(delimiter=d
-00003470: 656c 696d 6974 6572 2c20 7072 6566 6978  elimiter, prefix
-00003480: 3d70 7265 6669 782c 206d 6178 5f6b 6579  =prefix, max_key
-00003490: 733d 6d61 785f 6b65 7973 2c20 6d61 726b  s=max_keys, mark
-000034a0: 6572 3d6d 6172 6b65 722c 2065 6e63 6f64  er=marker, encod
-000034b0: 696e 675f 7479 7065 3d65 6e63 6f64 696e  ing_type=encodin
-000034c0: 675f 7479 7065 2c20 6665 7463 685f 6f77  g_type, fetch_ow
-000034d0: 6e65 723d 6665 7463 685f 6f77 6e65 7229  ner=fetch_owner)
-000034e0: 0a20 2066 6f72 206b 2069 6e20 6b65 7973  .  for k in keys
-000034f0: 3a0a 2020 2020 7072 696e 7428 276f 626a  :.    print('obj
-00003500: 6563 743a 272c 206b 2e6e 616d 6529 0a0a  ect:', k.name)..
-00003510: 6465 6620 6c69 7374 4f62 6a65 6374 734d  def listObjectsM
-00003520: 6f72 6528 6275 636b 6574 5f6e 616d 652c  ore(bucket_name,
-00003530: 2064 656c 696d 6974 6572 3d4e 6f6e 652c   delimiter=None,
-00003540: 2070 7265 6669 783d 4e6f 6e65 2c20 6d61   prefix=None, ma
-00003550: 785f 6b65 7973 3d4e 6f6e 652c 206d 6172  x_keys=None, mar
-00003560: 6b65 723d 4e6f 6e65 293a 0a20 2062 7563  ker=None):.  buc
-00003570: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
-00003580: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
-00003590: 6529 0a20 206b 6579 7320 3d20 6275 636b  e).  keys = buck
-000035a0: 6574 2e6c 6973 7428 6465 6c69 6d69 7465  et.list(delimite
-000035b0: 723d 6465 6c69 6d69 7465 722c 2070 7265  r=delimiter, pre
-000035c0: 6669 783d 7072 6566 6978 2c20 6d61 785f  fix=prefix, max_
-000035d0: 6b65 7973 3d6d 6178 5f6b 6579 732c 206d  keys=max_keys, m
-000035e0: 6172 6b65 723d 6d61 726b 6572 290a 2020  arker=marker).  
-000035f0: 2320 7072 696e 7428 6c65 6e28 6b65 7973  # print(len(keys
-00003600: 2929 0a20 2072 6573 203d 205b 6b2e 6e61  )).  res = [k.na
-00003610: 6d65 2066 6f72 206b 2069 6e20 6b65 7973  me for k in keys
-00003620: 5d0a 2020 7072 696e 7428 2772 6573 3a20  ].  print('res: 
-00003630: 272c 2072 6573 290a 2020 2320 7072 696e  ', res).  # prin
-00003640: 7428 2769 7465 6d3a 272c 206b 2e6e 616d  t('item:', k.nam
-00003650: 652c 2074 7970 6528 6b29 290a 0a64 6566  e, type(k))..def
-00003660: 206c 6973 7441 6e64 4465 6c65 7465 2829   listAndDelete()
-00003670: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
-00003680: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
-00003690: 6b65 745f 6e61 6d65 290a 2020 6b65 7973  ket_name).  keys
-000036a0: 203d 2062 7563 6b65 742e 6c69 7374 2864   = bucket.list(d
-000036b0: 656c 696d 6974 6572 3d27 2f27 2c20 6d61  elimiter='/', ma
-000036c0: 785f 6b65 7973 3d31 302c 2070 7265 6669  x_keys=10, prefi
-000036d0: 783d 2731 3527 290a 2020 7072 696e 7428  x='15').  print(
-000036e0: 6b65 7973 2e6d 6172 6b65 7229 0a20 2066  keys.marker).  f
-000036f0: 6f72 206b 2069 6e20 6b65 7973 3a0a 2020  or k in keys:.  
-00003700: 2020 7072 696e 7428 276f 626a 6563 743a    print('object:
-00003710: 272c 206b 2e6e 616d 6529 0a20 2020 2064  ', k.name).    d
-00003720: 656c 6574 654f 626a 6563 7428 6b2e 6e61  eleteObject(k.na
-00003730: 6d65 290a 0a64 6566 206c 6973 744f 626a  me)..def listObj
-00003740: 6563 7473 416e 6446 696c 7465 7228 656e  ectsAndFilter(en
-00003750: 6454 696d 653d 4e6f 6e65 293a 0a20 2062  dTime=None):.  b
-00003760: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
-00003770: 5f62 7563 6b65 7428 2761 7574 6f2d 7465  _bucket('auto-te
-00003780: 7374 2d62 7563 6b65 7427 290a 2020 6b65  st-bucket').  ke
-00003790: 7973 203d 2062 7563 6b65 742e 6c69 7374  ys = bucket.list
-000037a0: 4f62 6a65 6374 7328 6465 6c69 6d69 7465  Objects(delimite
-000037b0: 723d 272f 272c 206d 6178 5f6b 6579 733d  r='/', max_keys=
-000037c0: 3229 2023 2073 7461 7274 5f74 696d 653d  2) # start_time=
-000037d0: 3136 3430 3333 3134 3436 2c20 656e 645f  1640331446, end_
-000037e0: 7469 6d65 3d31 3634 3138 3935 3039 360a  time=1641895096.
-000037f0: 2020 666f 7220 6b20 696e 206b 6579 733a    for k in keys:
-00003800: 0a20 2020 2070 7269 6e74 286b 290a 0a64  .    print(k)..d
-00003810: 6566 2067 6574 4f62 6a65 6374 5461 6767  ef getObjectTagg
-00003820: 696e 6728 293a 0a20 2062 7563 6b65 7420  ing():.  bucket 
-00003830: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
-00003840: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
-00003850: 206b 6579 203d 2062 7563 6b65 742e 6765   key = bucket.ge
-00003860: 745f 6b65 7928 2774 6573 7454 6167 6769  t_key('testTaggi
-00003870: 6e67 2729 0a20 2074 6167 6769 6e67 203d  ng').  tagging =
-00003880: 206b 6579 2e67 6574 5f6f 626a 6563 745f   key.get_object_
-00003890: 7461 6767 696e 6728 290a 2020 7072 696e  tagging().  prin
-000038a0: 7428 7461 6767 696e 672e 746f 5f78 6d6c  t(tagging.to_xml
-000038b0: 2829 290a 0a64 6566 2073 6574 4f62 6a65  ())..def setObje
-000038c0: 6374 5461 6767 696e 6728 293a 0a20 2062  ctTagging():.  b
-000038d0: 7563 6b65 7420 3d20 636f 6e6e 2e67 6574  ucket = conn.get
-000038e0: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
-000038f0: 616d 6529 0a20 206b 6579 203d 2062 7563  ame).  key = buc
-00003900: 6b65 742e 6765 745f 6b65 7928 2774 6573  ket.get_key('tes
-00003910: 7454 6167 6769 6e67 2729 0a20 2074 6167  tTagging').  tag
-00003920: 6769 6e67 203d 205b 5461 6728 2730 2729  ging = [Tag('0')
-00003930: 2c20 5461 6728 2731 272c 2027 3127 295d  , Tag('1', '1')]
-00003940: 0a20 206b 6579 2e73 6574 5f6f 626a 6563  .  key.set_objec
-00003950: 745f 7461 6767 696e 6728 7461 6767 696e  t_tagging(taggin
-00003960: 6729 0a0a 6465 6620 6465 6c65 7465 4f62  g)..def deleteOb
-00003970: 6a65 6374 5461 6767 696e 6728 293a 0a20  jectTagging():. 
-00003980: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
-00003990: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-000039a0: 5f6e 616d 6529 0a20 206b 6579 203d 2062  _name).  key = b
-000039b0: 7563 6b65 742e 6765 745f 6b65 7928 2768  ucket.get_key('h
-000039c0: 6568 6527 290a 2020 6b65 792e 6465 6c65  ehe').  key.dele
-000039d0: 7465 5f6f 626a 6563 745f 7461 6767 696e  te_object_taggin
-000039e0: 6728 290a 0a64 6566 2063 616c 6346 6f6c  g()..def calcFol
-000039f0: 6465 7253 697a 6528 6275 636b 6574 2c20  derSize(bucket, 
-00003a00: 666f 6c64 6572 293a 0a20 206c 656e 6774  folder):.  lengt
-00003a10: 6820 3d20 300a 2020 6b65 7973 203d 2062  h = 0.  keys = b
-00003a20: 7563 6b65 742e 6c69 7374 2870 7265 6669  ucket.list(prefi
-00003a30: 783d 666f 6c64 6572 290a 2020 666f 7220  x=folder).  for 
-00003a40: 6b20 696e 206b 6579 733a 0a20 2020 2069  k in keys:.    i
-00003a50: 6620 6973 696e 7374 616e 6365 286b 2c20  f isinstance(k, 
-00003a60: 4b65 7929 3a0a 2020 2020 2020 6c65 6e67  Key):.      leng
-00003a70: 7468 202b 3d20 6b2e 7369 7a65 0a20 2072  th += k.size.  r
-00003a80: 6574 7572 6e20 6c65 6e67 7468 0a0a 6672  eturn length..fr
-00003a90: 6f6d 206b 7333 2e70 7265 6669 7820 696d  om ks3.prefix im
-00003aa0: 706f 7274 2050 7265 6669 780a 0a23 20e5  port Prefix..# .
-00003ab0: 8897 e4b8 bee6 8c87 e5ae 9ae7 9bae e5bd  ................
-00003ac0: 95e4 b88b e79a 84e6 9687 e4bb b6e5 a4a7  ................
-00003ad0: e5b0 8f0a 6465 6620 6765 7446 6f6c 6465  ....def getFolde
-00003ae0: 7253 697a 6549 6e42 7563 6b65 7428 293a  rSizeInBucket():
-00003af0: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
-00003b00: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
-00003b10: 6574 5f6e 616d 6529 0a20 206b 6579 7320  et_name).  keys 
-00003b20: 3d20 6275 636b 6574 2e6c 6973 7428 6465  = bucket.list(de
-00003b30: 6c69 6d69 7465 723d 272f 2729 0a20 2066  limiter='/').  f
-00003b40: 6f72 206b 2069 6e20 6b65 7973 3a0a 2020  or k in keys:.  
-00003b50: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00003b60: 6b2c 2050 7265 6669 7829 3a0a 2020 2020  k, Prefix):.    
-00003b70: 2020 7072 696e 7428 2764 6972 3a20 2720    print('dir: ' 
-00003b80: 2b20 6b2e 6e61 6d65 202b 2027 2020 7369  + k.name + '  si
-00003b90: 7a65 3a27 202b 2073 7472 2863 616c 6346  ze:' + str(calcF
-00003ba0: 6f6c 6465 7253 697a 6528 6275 636b 6574  olderSize(bucket
-00003bb0: 2c20 6b2e 6e61 6d65 2929 202b 2022 4279  , k.name)) + "By
-00003bc0: 7465 2229 0a0a 0a64 6566 2074 6573 745f  te")...def test_
-00003bd0: 6d75 6c74 6970 6172 745f 7570 6c6f 6164  multipart_upload
-00003be0: 2865 6e63 7279 7074 5f6b 6579 3d4e 6f6e  (encrypt_key=Non
-00003bf0: 6529 3a0a 2020 696d 706f 7274 206d 6174  e):.  import mat
-00003c00: 682c 206f 730a 2020 6672 6f6d 2066 696c  h, os.  from fil
-00003c10: 6563 6875 6e6b 696f 2069 6d70 6f72 7420  echunkio import 
-00003c20: 4669 6c65 4368 756e 6b49 4f0a 2020 6275  FileChunkIO.  bu
-00003c30: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
-00003c40: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
-00003c50: 6d65 290a 0a20 2073 6f75 7263 655f 7061  me)..  source_pa
-00003c60: 7468 203d 2027 2f55 7365 7273 2f6a 6162  th = '/Users/jab
-00003c70: 6261 722f 446f 776e 6c6f 6164 732f 4453  bar/Downloads/DS
-00003c80: 4330 3333 3830 2e4a 5047 270a 2020 2320  C03380.JPG'.  # 
-00003c90: e6ba 90e6 9687 e4bb b6e5 a4a7 e5b0 8f0a  ................
-00003ca0: 2020 736f 7572 6365 5f73 697a 6520 3d20    source_size = 
-00003cb0: 6f73 2e73 7461 7428 736f 7572 6365 5f70  os.stat(source_p
-00003cc0: 6174 6829 2e73 745f 7369 7a65 0a0a 2020  ath).st_size..  
-00003cd0: 6d70 203d 2062 7563 6b65 742e 696e 6974  mp = bucket.init
-00003ce0: 6961 7465 5f6d 756c 7469 7061 7274 5f75  iate_multipart_u
-00003cf0: 706c 6f61 6428 2244 5343 3033 3338 302e  pload("DSC03380.
-00003d00: 6d70 2e6a 7067 222c 2065 6e63 7279 7074  mp.jpg", encrypt
-00003d10: 5f6b 6579 3d65 6e63 7279 7074 5f6b 6579  _key=encrypt_key
-00003d20: 290a 2020 7072 696e 7428 6d70 290a 0a20  ).  print(mp).. 
-00003d30: 2063 6875 6e6b 5f73 697a 6520 3d20 3532   chunk_size = 52
-00003d40: 3432 3838 300a 2020 6368 756e 6b5f 636f  42880.  chunk_co
-00003d50: 756e 7420 3d20 696e 7428 6d61 7468 2e63  unt = int(math.c
-00003d60: 6569 6c28 736f 7572 6365 5f73 697a 6520  eil(source_size 
-00003d70: 2a20 312e 3020 2f20 6368 756e 6b5f 7369  * 1.0 / chunk_si
-00003d80: 7a65 202a 2031 2e30 2929 0a0a 2020 2320  ze * 1.0))..  # 
-00003d90: e980 9ae8 bf87 2046 696c 6543 6875 6e6b  ...... FileChunk
-00003da0: 494f 20e5 b086 e696 87e4 bbb6 e588 86e7  IO .............
-00003db0: 8987 0a20 2066 6f72 2069 2069 6e20 7261  ...  for i in ra
-00003dc0: 6e67 6528 6368 756e 6b5f 636f 756e 7429  nge(chunk_count)
-00003dd0: 3a0a 2020 2020 6f66 6673 6574 203d 2063  :.    offset = c
-00003de0: 6875 6e6b 5f73 697a 6520 2a20 690a 2020  hunk_size * i.  
-00003df0: 2020 6279 7465 7320 3d20 6d69 6e28 6368    bytes = min(ch
-00003e00: 756e 6b5f 7369 7a65 2c20 736f 7572 6365  unk_size, source
-00003e10: 5f73 697a 6520 2d20 6f66 6673 6574 290a  _size - offset).
-00003e20: 2020 2020 7769 7468 2046 696c 6543 6875      with FileChu
-00003e30: 6e6b 494f 2873 6f75 7263 655f 7061 7468  nkIO(source_path
-00003e40: 2c20 2772 272c 206f 6666 7365 743d 6f66  , 'r', offset=of
-00003e50: 6673 6574 2c20 6279 7465 733d 6279 7465  fset, bytes=byte
-00003e60: 7329 2061 7320 6670 3a0a 2020 2020 2020  s) as fp:.      
-00003e70: 2320 e980 90e4 b8aa e4b8 8ae4 bca0 e588  # ..............
-00003e80: 86e7 8987 0a20 2020 2020 206d 702e 7570  .....      mp.up
-00003e90: 6c6f 6164 5f70 6172 745f 6672 6f6d 5f66  load_part_from_f
-00003ea0: 696c 6528 6670 2c20 7061 7274 5f6e 756d  ile(fp, part_num
-00003eb0: 3d69 202b 2031 290a 2020 7072 696e 7428  =i + 1).  print(
-00003ec0: 6d70 2e74 6f5f 786d 6c28 2929 0a20 2023  mp.to_xml()).  #
-00003ed0: 20e5 8f91 e980 81e8 afb7 e6b1 82ef bc8c   ...............
-00003ee0: e590 88e5 b9b6 e588 86e7 8987 efbc 8ce5  ................
-00003ef0: ae8c e688 90e5 8886 e789 87e4 b88a e4bc  ................
-00003f00: a00a 2020 7265 7420 3d20 6d70 2e63 6f6d  ..  ret = mp.com
-00003f10: 706c 6574 655f 7570 6c6f 6164 2829 0a20  plete_upload(). 
-00003f20: 2069 6620 7265 7420 616e 6420 7265 742e   if ret and ret.
-00003f30: 7374 6174 7573 203d 3d20 3230 303a 0a20  status == 200:. 
-00003f40: 2020 2070 7269 6e74 2822 e4b8 8ae4 bca0     print("......
-00003f50: e688 90e5 8a9f 2229 0a0a 6465 6620 7465  ......")..def te
-00003f60: 7374 5f66 6574 6368 5f6f 626a 6563 7428  st_fetch_object(
-00003f70: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
-00003f80: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
-00003f90: 636b 6574 5f6e 616d 6529 0a20 206b 6579  cket_name).  key
-00003fa0: 203d 2062 7563 6b65 742e 6e65 775f 6b65   = bucket.new_ke
-00003fb0: 7928 2777 7777 2d6c 6f67 6f27 290a 2020  y('www-logo').  
-00003fc0: 6b65 792e 6665 7463 685f 6f62 6a65 6374  key.fetch_object
-00003fd0: 2873 6f75 7263 655f 7572 6c3d 2768 7474  (source_url='htt
-00003fe0: 703a 2f2f 6665 2e6b 7379 756e 2e63 6f6d  p://fe.ksyun.com
-00003ff0: 2f70 726f 6a65 6374 2f72 6573 6f75 7263  /project/resourc
-00004000: 652f 696d 672f 7777 772d 6c6f 676f 2e70  e/img/www-logo.p
-00004010: 6e67 272c 0a20 2020 2020 2020 2020 2020  ng',.           
-00004020: 2020 2020 2020 2020 2020 2068 6561 6465             heade
-00004030: 7273 3d7b 2778 2d6b 7373 2d61 636c 273a  rs={'x-kss-acl':
-00004040: 2027 7075 626c 6963 2d72 6561 6427 7d29   'public-read'})
-00004050: 0a20 2070 7269 6e74 2827 6665 7463 68e6  .  print('fetch.
-00004060: 8890 e58a 9f27 290a 0a64 6566 2074 6573  .....')..def tes
-00004070: 745f 6765 6e65 7261 7465 5f75 726c 286b  t_generate_url(k
-00004080: 6579 5f6e 616d 652c 2069 6d61 6765 5f61  ey_name, image_a
-00004090: 7474 7273 3d4e 6f6e 6529 3a0a 2020 6220  ttrs=None):.  b 
-000040a0: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
-000040b0: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
-000040c0: 206b 203d 2062 2e67 6574 5f6b 6579 286b   k = b.get_key(k
-000040d0: 6579 5f6e 616d 6529 0a20 2069 6620 6b3a  ey_name).  if k:
-000040e0: 0a20 2020 2075 726c 203d 206b 2e67 656e  .    url = k.gen
-000040f0: 6572 6174 655f 7572 6c28 3630 302c 2069  erate_url(600, i
-00004100: 6d61 6765 5f61 7474 7273 3d69 6d61 6765  mage_attrs=image
-00004110: 5f61 7474 7273 2920 2023 2036 3073 20e5  _attrs)  # 60s .
-00004120: 908e e8af a5e9 93be e68e a5e8 bf87 e69c  ................
-00004130: 9f0a 2020 2020 7072 696e 7428 7572 6c29  ..    print(url)
-00004140: 0a20 2065 6c73 653a 0a20 2020 2070 7269  .  else:.    pri
-00004150: 6e74 2827 6f62 6a65 6374 206e 6f74 2066  nt('object not f
-00004160: 6f75 6e64 2729 0a0a 6465 6620 7465 7374  ound')..def test
-00004170: 5f67 6574 5f70 7265 7369 676e 6564 5f75  _get_presigned_u
-00004180: 726c 286b 6579 5f6e 616d 6529 3a0a 2020  rl(key_name):.  
-00004190: 6220 3d20 636f 6e6e 2e67 6574 5f62 7563  b = conn.get_buc
-000041a0: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
-000041b0: 0a20 2023 20e6 96b0 e5bb bae5 afb9 e8b1  .  # ...........
-000041c0: a16b 6579 0a20 206b 203d 2062 2e6e 6577  .key.  k = b.new
-000041d0: 5f6b 6579 286b 6579 5f6e 616d 6529 0a20  _key(key_name). 
-000041e0: 2069 6620 6b3a 0a20 2020 2075 726c 203d   if k:.    url =
-000041f0: 206b 2e67 6574 5f70 7265 7369 676e 6564   k.get_presigned
-00004200: 5f75 726c 2836 3030 3030 2920 2023 2036  _url(60000)  # 6
-00004210: 3073 20e5 908e e8af a5e9 93be e68e a5e8  0s .............
-00004220: bf87 e69c 9f0a 2020 2020 7072 696e 7428  ......    print(
-00004230: 7572 6c29 0a20 2020 2072 6574 7572 6e20  url).    return 
-00004240: 7572 6c0a 0a64 6566 2072 6573 746f 7265  url..def restore
-00004250: 4f62 6a65 6374 286b 6579 5f6e 616d 6529  Object(key_name)
-00004260: 3a0a 2020 6220 3d20 636f 6e6e 2e67 6574  :.  b = conn.get
-00004270: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
-00004280: 616d 6529 0a20 206b 203d 2062 2e67 6574  ame).  k = b.get
-00004290: 5f6b 6579 286b 6579 5f6e 616d 6529 0a20  _key(key_name). 
-000042a0: 206b 2e72 6573 746f 7265 5f6f 626a 6563   k.restore_objec
-000042b0: 7428 290a 0a64 6566 2074 6573 745f 7075  t()..def test_pu
-000042c0: 745f 7669 615f 7072 6573 6967 6e65 645f  t_via_presigned_
-000042d0: 7572 6c28 6b65 7929 3a0a 2020 7572 6c20  url(key):.  url 
-000042e0: 3d20 7465 7374 5f67 6574 5f70 7265 7369  = test_get_presi
-000042f0: 676e 6564 5f75 726c 286b 6579 290a 2020  gned_url(key).  
-00004300: 7769 7468 206f 7065 6e28 272e 2f61 7274  with open('./art
-00004310: 6963 6c65 2e74 7874 272c 2027 7262 2729  icle.txt', 'rb')
-00004320: 2061 7320 6670 3a0a 2020 2020 7265 7375   as fp:.    resu
-00004330: 6c74 203d 2072 6571 7565 7374 732e 7075  lt = requests.pu
-00004340: 7428 7572 6c2c 2064 6174 613d 6670 290a  t(url, data=fp).
-00004350: 2020 2020 7072 696e 7428 7265 7375 6c74      print(result
-00004360: 290a 0a66 726f 6d20 6b73 332e 7374 7320  )..from ks3.sts 
-00004370: 696d 706f 7274 2061 7373 756d 6552 6f6c  import assumeRol
-00004380: 650a 6465 6620 7465 7374 5f61 7373 756d  e.def test_assum
-00004390: 6552 6f6c 6528 293a 0a20 2070 7269 6e74  eRole():.  print
-000043a0: 2861 7373 756d 6552 6f6c 6528 616b 2c20  (assumeRole(ak, 
-000043b0: 736b 2c20 226b 726e 3a6b 7363 3a69 616d  sk, "krn:ksc:iam
-000043c0: 3a3a 7878 783a 726f 6c65 2f78 782d 7465  ::xxx:role/xx-te
-000043d0: 7374 2d62 7563 6b65 7422 2c20 226b 7333  st-bucket", "ks3
-000043e0: 222c 2033 3630 3029 290a 0a0a 6465 6620  ", 3600))...def 
-000043f0: 7075 745f 6f62 6a65 6374 5f63 616c 6c62  put_object_callb
-00004400: 6163 6b28 6b65 795f 6e61 6d65 293a 0a20  ack(key_name):. 
-00004410: 2062 203d 2063 6f6e 6e2e 6765 745f 6275   b = conn.get_bu
-00004420: 636b 6574 2827 6861 6e6a 696e 672d 7465  cket('hanjing-te
-00004430: 7374 3030 3027 290a 2020 2320 e696 b0e5  st000').  # ....
-00004440: bbba e5af b9e8 b1a1 6b65 790a 2020 6b20  ........key.  k 
-00004450: 3d20 622e 6e65 775f 6b65 7928 6b65 795f  = b.new_key(key_
-00004460: 6e61 6d65 290a 2020 2320 e4b8 8ae4 bca0  name).  # ......
-00004470: e688 90e5 8a9f e590 8eef bc8c e590 91e5  ................
-00004480: 9b9e e8b0 83e5 9cb0 e59d 8050 4f53 54e6  ...........POST.
-00004490: 95b0 e68d ae0a 2020 2320 e99c 80e8 a681  ......  # ......
-000044a0: e8ae bee7 bdae 6078 2d6b 7373 2d63 616c  ......`x-kss-cal
-000044b0: 6c62 6163 6b75 726c 60e5 928c 6078 2d6b  lbackurl`...`x-k
-000044c0: 7373 2d63 616c 6c62 6163 6b62 6f64 7960  ss-callbackbody`
-000044d0: e8af b7e6 b182 e5a4 b4ef bc8c e8af a6e8  ................
-000044e0: a781 e696 87e6 a1a3 5be4 b88a e4bc a0e5  ........[.......
-000044f0: 9b9e e8b0 83e5 a484 e790 865d 2868 7474  ...........](htt
-00004500: 7073 3a2f 2f64 6f63 732e 6b73 7975 6e2e  ps://docs.ksyun.
-00004510: 636f 6d2f 646f 6375 6d65 6e74 732f 3935  com/documents/95
-00004520: 3629 e380 820a 2020 2320 782d 6b73 732d  6)....  # x-kss-
-00004530: 6361 6c6c 6261 636b 7572 6c20 e4b8 bae5  callbackurl ....
-00004540: 8f91 e8b5 b7e5 9b9e e8b0 83e6 97b6 e8af  ................
-00004550: b7e6 b182 e79a 84e6 9c8d e58a a1e5 99a8  ................
-00004560: e59c b0e5 9d80 0a20 2023 2078 2d6b 7373  .......  # x-kss
-00004570: 2d63 616c 6c62 6163 6b62 6f64 7920 e4b8  -callbackbody ..
-00004580: bae5 8f91 e8b5 b7e5 9b9e e8b0 83e6 97b6  ................
-00004590: e8af b7e6 b182 e79a 8462 6f64 79e7 9a84  .........body...
-000045a0: e580 bc0a 2020 6865 6164 6572 7320 3d20  ....  headers = 
-000045b0: 7b22 782d 6b73 732d 6361 6c6c 6261 636b  {"x-kss-callback
-000045c0: 7572 6c22 3a20 2268 7474 7073 3a2f 2f79  url": "https://y
-000045d0: 682d 7368 2e6b 7333 2d63 6e2d 7368 616e  h-sh.ks3-cn-shan
-000045e0: 6768 6169 2e6b 7379 756e 6373 2e63 6f6d  ghai.ksyuncs.com
-000045f0: 222c 2022 782d 6b73 732d 6361 6c6c 6261  ", "x-kss-callba
-00004600: 636b 626f 6479 223a 2022 6f62 6a65 6374  ckbody": "object
-00004610: 4b65 793d 247b 6b65 797d 2665 7461 673d  Key=${key}&etag=
-00004620: 247b 6574 6167 7d26 6275 636b 6574 3d24  ${etag}&bucket=$
-00004630: 7b62 7563 6b65 747d 266f 626a 6563 7453  {bucket}&objectS
-00004640: 697a 653d 247b 6f62 6a65 6374 5369 7a65  ize=${objectSize
-00004650: 7d26 6d69 6d65 5479 7065 3d24 7b6d 696d  }&mimeType=${mim
-00004660: 6554 7970 657d 2663 7265 6174 6554 696d  eType}&createTim
-00004670: 653d 247b 6372 6561 7465 5469 6d65 7d22  e=${createTime}"
-00004680: 2c20 2278 2d6b 7373 2d63 616c 6c62 6163  , "x-kss-callbac
-00004690: 6b61 7574 6822 3a31 7d0a 2020 7265 7420  kauth":1}.  ret 
-000046a0: 3d20 6b2e 7365 745f 636f 6e74 656e 7473  = k.set_contents
-000046b0: 5f66 726f 6d5f 7374 7269 6e67 2822 7465  _from_string("te
-000046c0: 7374 2d63 616c 6c62 6163 6b22 2c20 6865  st-callback", he
-000046d0: 6164 6572 733d 6865 6164 6572 7329 0a20  aders=headers). 
-000046e0: 2069 6620 7265 7420 616e 6420 7265 742e   if ret and ret.
-000046f0: 7374 6174 7573 203d 3d20 3230 303a 0a20  status == 200:. 
-00004700: 2020 2070 7269 6e74 2822 e4b8 8ae4 bca0     print("......
-00004710: e688 90e5 8a9f 2229 0a0a 2320 6765 7441  ......")..# getA
-00004720: 6c6c 4275 636b 6574 7328 290a 2320 6865  llBuckets().# he
-00004730: 6164 4275 636b 6574 2827 626a 2729 0a23  adBucket('bj').#
-00004740: 2067 6574 4275 636b 6574 4c6f 6361 7469   getBucketLocati
-00004750: 6f6e 2827 7465 7374 2d68 6f73 742d 7374  on('test-host-st
-00004760: 796c 6527 290a 2320 6372 6561 7465 4275  yle').# createBu
-00004770: 636b 6574 2827 7465 7374 2d62 7563 6b65  cket('test-bucke
-00004780: 742d 6172 6368 6976 652d 7465 7374 2d73  t-archive-test-s
-00004790: 6861 6e67 6861 6932 272c 206c 6f63 6174  hanghai2', locat
-000047a0: 696f 6e3d 2753 4841 4e47 4841 4927 290a  ion='SHANGHAI').
-000047b0: 2320 6465 6c65 7465 4275 636b 6574 2827  # deleteBucket('
-000047c0: 7465 7374 2d62 7563 6b65 7427 290a 2320  test-bucket').# 
-000047d0: 6765 7442 7563 6b65 7441 636c 2827 7465  getBucketAcl('te
-000047e0: 7374 2d62 7563 6b65 7427 290a 2320 7365  st-bucket').# se
-000047f0: 7442 7563 6b65 7441 636c 2827 7465 7374  tBucketAcl('test
-00004800: 2d62 7563 6b65 7427 290a 2320 6d61 6e61  -bucket').# mana
-00004810: 6765 4275 636b 6574 5265 706c 6963 6174  geBucketReplicat
-00004820: 696f 6e28 2774 6573 742d 6275 636b 6574  ion('test-bucket
-00004830: 2729 0a23 2067 6574 4275 636b 6574 4c69  ').# getBucketLi
-00004840: 6665 4379 636c 6528 6275 636b 6574 5f6e  feCycle(bucket_n
-00004850: 616d 6529 0a23 2073 6574 4275 636b 6574  ame).# setBucket
-00004860: 4c69 6665 4379 636c 6528 6275 636b 6574  LifeCycle(bucket
-00004870: 5f6e 616d 6529 0a23 2073 6574 4275 636b  _name).# setBuck
-00004880: 6574 4c69 6665 4379 636c 6532 2862 7563  etLifeCycle2(buc
-00004890: 6b65 745f 6e61 6d65 290a 2320 6465 6c65  ket_name).# dele
-000048a0: 7465 4275 636b 6574 4c69 6665 4379 636c  teBucketLifeCycl
-000048b0: 6528 6275 636b 6574 5f6e 616d 6529 0a23  e(bucket_name).#
-000048c0: 2067 6574 4275 636b 6574 4c6f 6767 696e   getBucketLoggin
-000048d0: 6728 6275 636b 6574 5f6e 616d 6529 0a23  g(bucket_name).#
-000048e0: 2073 6574 4275 636b 6574 4c6f 6767 696e   setBucketLoggin
-000048f0: 6728 6275 636b 6574 5f6e 616d 6529 0a23  g(bucket_name).#
-00004900: 2064 6973 6162 6c65 4275 636b 6574 4c6f   disableBucketLo
-00004910: 6767 696e 6728 6275 636b 6574 5f6e 616d  gging(bucket_nam
-00004920: 6529 0a23 2065 6e61 626c 6542 7563 6b65  e).# enableBucke
-00004930: 744c 6f67 6769 6e67 2862 7563 6b65 745f  tLogging(bucket_
-00004940: 6e61 6d65 290a 2320 7075 7442 7563 6b65  name).# putBucke
-00004950: 7443 6f72 7328 6275 636b 6574 5f6e 616d  tCors(bucket_nam
-00004960: 6529 0a23 2067 6574 4275 636b 6574 436f  e).# getBucketCo
-00004970: 7273 2862 7563 6b65 745f 6e61 6d65 290a  rs(bucket_name).
-00004980: 2320 6465 6c65 7465 4275 636b 6574 436f  # deleteBucketCo
-00004990: 7273 2862 7563 6b65 745f 6e61 6d65 290a  rs(bucket_name).
-000049a0: 2320 6465 6c65 7465 4275 636b 6574 4372  # deleteBucketCr
-000049b0: 7228 6275 636b 6574 5f6e 616d 6529 0a23  r(bucket_name).#
-000049c0: 2067 6574 4275 636b 6574 4372 7228 6275   getBucketCrr(bu
-000049d0: 636b 6574 5f6e 616d 6529 0a23 2073 6574  cket_name).# set
-000049e0: 4275 636b 6574 4372 7228 6275 636b 6574  BucketCrr(bucket
-000049f0: 5f6e 616d 6529 0a23 2073 6574 4275 636b  _name).# setBuck
-00004a00: 6574 4d69 7272 6f72 2862 7563 6b65 745f  etMirror(bucket_
-00004a10: 6e61 6d65 290a 2320 6465 6c65 7465 4275  name).# deleteBu
-00004a20: 636b 6574 4d69 7272 6f72 2862 7563 6b65  cketMirror(bucke
-00004a30: 745f 6e61 6d65 290a 2320 6765 7442 7563  t_name).# getBuc
-00004a40: 6b65 744d 6972 726f 7228 6275 636b 6574  ketMirror(bucket
-00004a50: 5f6e 616d 6529 0a23 2323 2323 206f 626a  _name).##### obj
-00004a60: 6563 7420 2323 2323 230a 2320 6765 744f  ect #####.# getO
-00004a70: 626a 6563 744d 6574 6128 6275 636b 6574  bjectMeta(bucket
-00004a80: 5f6e 616d 652c 2027 6172 7469 636c 652e  _name, 'article.
-00004a90: 7478 7427 290a 2320 6c69 7374 5f6f 626a  txt').# list_obj
-00004aa0: 6563 7473 2829 0a23 206c 6973 744f 626a  ects().# listObj
-00004ab0: 6563 7473 4d6f 7265 2822 6175 746f 2d74  ectsMore("auto-t
-00004ac0: 6573 742d 6275 636b 6574 222c 2064 656c  est-bucket", del
-00004ad0: 696d 6974 6572 3d27 2f27 2c20 6d61 785f  imiter='/', max_
-00004ae0: 6b65 7973 3d32 2c20 6d61 726b 6572 3d27  keys=2, marker='
-00004af0: 3130 3530 2729 0a23 206c 6973 744f 626a  1050').# listObj
-00004b00: 6563 7473 4d6f 7265 2822 6175 746f 2d74  ectsMore("auto-t
-00004b10: 6573 742d 6275 636b 6574 222c 2064 656c  est-bucket", del
-00004b20: 696d 6974 6572 3d27 2f27 2c20 6d61 785f  imiter='/', max_
-00004b30: 6b65 7973 3d32 2c20 6d61 726b 6572 3d27  keys=2, marker='
-00004b40: 3130 352f 2729 0a23 206c 6973 744f 626a  105/').# listObj
-00004b50: 6563 7473 4d6f 7265 2822 6175 746f 2d74  ectsMore("auto-t
-00004b60: 6573 742d 6275 636b 6574 222c 2064 656c  est-bucket", del
-00004b70: 696d 6974 6572 3d27 2f27 2c20 6d61 785f  imiter='/', max_
-00004b80: 6b65 7973 3d32 2c20 6d61 726b 6572 3d27  keys=2, marker='
-00004b90: 3130 3525 3246 2729 0a23 206c 6973 744f  105%2F').# listO
-00004ba0: 626a 6563 7473 416e 6446 696c 7465 7228  bjectsAndFilter(
-00004bb0: 290a 2320 7365 744f 626a 6563 7454 6167  ).# setObjectTag
-00004bc0: 6769 6e67 2829 0a23 2067 6574 4f62 6a65  ging().# getObje
-00004bd0: 6374 5461 6767 696e 6728 290a 2320 6465  ctTagging().# de
-00004be0: 6c65 7465 4f62 6a65 6374 5461 6767 696e  leteObjectTaggin
-00004bf0: 6728 290a 2320 6765 7446 6f6c 6465 7253  g().# getFolderS
-00004c00: 697a 6549 6e42 7563 6b65 7428 293b 0a23  izeInBucket();.#
-00004c10: 2064 6f77 6e6c 6f61 644f 626a 6563 7441   downloadObjectA
-00004c20: 6e64 5072 696e 7428 290a 2320 646f 776e  ndPrint().# down
-00004c30: 6c6f 6164 4f62 6a65 6374 4173 5374 7265  loadObjectAsStre
-00004c40: 616d 416e 6450 7269 6e74 2829 0a23 2064  amAndPrint().# d
-00004c50: 6f77 6e6c 6f61 644f 626a 6563 7441 6e64  ownloadObjectAnd
-00004c60: 5361 7665 2862 7563 6b65 745f 6e61 6d65  Save(bucket_name
-00004c70: 2c20 2744 5343 3033 3338 302e 656e 6372  , 'DSC03380.encr
-00004c80: 7970 742e e99d 9ee5 8886 e59d 972e 6a70  ypt...........jp
-00004c90: 6727 2c20 6865 6164 6572 733d 7b0a 2320  g', headers={.# 
-00004ca0: 2020 2772 616e 6765 273a 2027 6279 7465    'range': 'byte
-00004cb0: 733d 302d 3532 3432 3838 3027 0a23 207d  s=0-5242880'.# }
-00004cc0: 290a 2320 636f 756e 7420 3d20 3230 0a23  ).# count = 20.#
-00004cd0: 2077 6869 6c65 2054 7275 653a 0a23 2075   while True:.# u
-00004ce0: 706c 6f61 644f 626a 6563 7446 726f 6d46  ploadObjectFromF
-00004cf0: 696c 6528 27e6 b395 e6b2 bb2e 6a70 6567  ile('.......jpeg
-00004d00: 2729 0a75 706c 6f61 645f 6173 796e 6328  ').upload_async(
-00004d10: 27e6 b395 e6b2 bb2e 6a70 6567 2729 0a64  '.......jpeg').d
-00004d20: 6f77 6e6c 6f61 645f 6173 796e 6328 2731  ownload_async('1
-00004d30: 3635 3936 3834 3837 322e 746f 7272 656e  659684872.torren
-00004d40: 7427 290a 2320 7570 6c6f 6164 4f62 6a65  t').# uploadObje
-00004d50: 6374 4672 6f6d 4669 6c65 2827 7861 6227  ctFromFile('xab'
-00004d60: 290a 2320 7570 6c6f 6164 4f62 6a65 6374  ).# uploadObject
-00004d70: 4672 6f6d 4669 6c65 2827 7861 6327 290a  FromFile('xac').
-00004d80: 2320 2020 7469 6d65 2e73 6c65 6570 2835  #   time.sleep(5
-00004d90: 290a 2320 2020 636f 756e 7420 3d20 636f  ).#   count = co
-00004da0: 756e 7420 2d20 310a 2320 7570 6c6f 6164  unt - 1.# upload
-00004db0: 4f62 6a65 6374 4672 6f6d 5374 7269 6e67  ObjectFromString
-00004dc0: 2829 0a23 2068 6561 644f 626a 6563 7428  ().# headObject(
-00004dd0: 290a 2320 646f 776e 6c6f 6164 4f62 6a65  ).# downloadObje
-00004de0: 6374 416e 6450 7269 6e74 2827 7465 7374  ctAndPrint('test
-00004df0: 5f64 6972 6563 746f 7279 2f27 290a 2320  _directory/').# 
-00004e00: 6465 6c65 7465 4f62 6a65 6374 2822 7465  deleteObject("te
-00004e10: 6c6c 6d65 7768 7922 290a 2320 6765 744f  llmewhy").# getO
-00004e20: 626a 6563 7441 636c 2829 0a0a 2320 7465  bjectAcl()..# te
-00004e30: 7374 5f6d 756c 7469 7061 7274 5f75 706c  st_multipart_upl
-00004e40: 6f61 6428 656e 6372 7970 745f 6b65 793d  oad(encrypt_key=
-00004e50: 5472 7565 290a 0a23 2074 6573 745f 6665  True)..# test_fe
-00004e60: 7463 685f 6f62 6a65 6374 2829 0a23 2064  tch_object().# d
-00004e70: 6566 2074 6573 745f 6765 6e65 7261 7465  ef test_generate
-00004e80: 5f75 726c 286b 6579 5f6e 616d 652c 2069  _url(key_name, i
-00004e90: 6d61 6765 5f61 7474 7273 3d4e 6f6e 6529  mage_attrs=None)
-00004ea0: 3a0a 2320 2020 6220 3d20 636f 6e6e 2e67  :.#   b = conn.g
-00004eb0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
-00004ec0: 5f6e 616d 6529 0a23 2020 206b 203d 2062  _name).#   k = b
-00004ed0: 2e67 6574 5f6b 6579 286b 6579 5f6e 616d  .get_key(key_nam
-00004ee0: 6529 0a23 2020 2069 6620 6b3a 0a23 2020  e).#   if k:.#  
-00004ef0: 2020 2075 726c 203d 206b 2e67 656e 6572     url = k.gener
-00004f00: 6174 655f 7572 6c28 3630 302c 2069 6d61  ate_url(600, ima
-00004f10: 6765 5f61 7474 7273 3d69 6d61 6765 5f61  ge_attrs=image_a
-00004f20: 7474 7273 2920 2023 2036 3073 20e5 908e  ttrs)  # 60s ...
-00004f30: e8af a5e9 93be e68e a5e8 bf87 e69c 9f0a  ................
-00004f40: 2320 2020 2020 7072 696e 7428 7572 6c29  #     print(url)
-00004f50: 0a23 2020 2065 6c73 653a 0a23 2020 2020  .#   else:.#    
-00004f60: 2070 7269 6e74 2827 6f62 6a65 6374 206e   print('object n
-00004f70: 6f74 2066 6f75 6e64 2729 0a0a 2320 6275  ot found')..# bu
-00004f80: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
-00004f90: 6275 636b 6574 2827 7465 7374 2d62 7563  bucket('test-buc
-00004fa0: 6b65 7427 290a 2320 6b65 7973 203d 2062  ket').# keys = b
-00004fb0: 7563 6b65 742e 6c69 7374 2829 0a23 2066  ucket.list().# f
-00004fc0: 6f72 206b 2069 6e20 6b65 7973 3a0a 2320  or k in keys:.# 
-00004fd0: 2020 7072 696e 7428 6b29 0a23 2020 2069    print(k).#   i
-00004fe0: 6620 6973 696e 7374 616e 6365 286b 2c20  f isinstance(k, 
-00004ff0: 4b65 7929 3a0a 2320 2020 2020 7572 6c20  Key):.#     url 
-00005000: 3d20 6b2e 6765 6e65 7261 7465 5f75 726c  = k.generate_url
-00005010: 2836 3030 290a 2320 2020 2020 7265 7320  (600).#     res 
-00005020: 3d20 7265 7175 6573 7473 2e67 6574 2875  = requests.get(u
-00005030: 726c 290a 2320 2020 2020 6966 2072 6573  rl).#     if res
-00005040: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-00005050: 3230 303a 0a23 2020 2020 2020 2070 7269  200:.#       pri
-00005060: 6e74 2875 726c 290a 0a0a 2320 7265 7320  nt(url)...# res 
-00005070: 3d20 7265 7175 6573 7473 2e67 6574 2875  = requests.get(u
-00005080: 726c 290a 2320 6173 7365 7274 2072 6573  rl).# assert res
-00005090: 2e73 7461 7475 735f 636f 6465 2021 3d20  .status_code != 
-000050a0: 3430 330a 2320 7465 7374 5f67 656e 6572  403.# test_gener
-000050b0: 6174 655f 7572 6c28 275c 5c61 5c5c 5c5c  ate_url('\\a\\\\
-000050c0: 3a3c 3e2a 3f7c 3a71 2e6a 7065 6727 290a  :<>*?|:q.jpeg').
-000050d0: 2320 7465 7374 5f67 656e 6572 6174 655f  # test_generate_
-000050e0: 7572 6c28 2723 7832 3b2e 6a70 2e63 7376  url('#x2;.jp.csv
-000050f0: 2729 0a23 2074 6573 745f 6765 6e65 7261  ').# test_genera
-00005100: 7465 5f75 726c 2827 3130 3038 362f 3139  te_url('10086/19
-00005110: 382e 3138 2d72 6573 6574 2de5 85b1 e8ae  8.18-reset-.....
-00005120: a139 e69d a12e 7478 7427 290a 2320 7465  .9....txt').# te
-00005130: 7374 5f67 656e 6572 6174 655f 7572 6c28  st_generate_url(
-00005140: 2731 3030 3836 2f67 6574 6275 636b 6574  '10086/getbucket
-00005150: 2e63 7376 2729 0a23 2074 6573 745f 6765  .csv').# test_ge
-00005160: 745f 7072 6573 6967 6e65 645f 7572 6c28  t_presigned_url(
-00005170: 277e 2a63 2f68 6563 6b44 6174 612b 7364  '~*c/heckData+sd
-00005180: 663d 2532 462e 6a73 6f6e 2729 0a23 2074  f=%2F.json').# t
-00005190: 6573 745f 7075 745f 7669 615f 7072 6573  est_put_via_pres
-000051a0: 6967 6e65 645f 7572 6c28 2769 6e64 6578  igned_url('index
-000051b0: 2e68 746d 6c27 290a 2320 6c69 7374 5f6f  .html').# list_o
-000051c0: 626a 6563 7473 5f76 3228 6465 6c69 6d69  bjects_v2(delimi
-000051d0: 7465 723d 272f 272c 2065 6e63 6f64 696e  ter='/', encodin
-000051e0: 675f 7479 7065 3d27 7572 6c27 2c20 6665  g_type='url', fe
-000051f0: 7463 685f 6f77 6e65 723d 4661 6c73 6529  tch_owner=False)
-00005200: 0a23 206c 6973 745f 6f62 6a65 6374 7328  .# list_objects(
-00005210: 290a 2320 6c69 7374 4f62 6a65 6374 734d  ).# listObjectsM
-00005220: 6f72 6528 290a 2320 6465 6c65 7465 4f62  ore().# deleteOb
-00005230: 6a65 6374 2829 0a23 206c 6973 744f 626a  ject().# listObj
-00005240: 6563 7473 416e 6446 696c 7465 7228 290a  ectsAndFilter().
-00005250: 2320 6c69 7374 416e 6444 656c 6574 6528  # listAndDelete(
-00005260: 290a 2320 7265 7374 6f72 654f 626a 6563  ).# restoreObjec
-00005270: 7428 2277 7777 2d6c 6f67 6f22 290a 2320  t("www-logo").# 
-00005280: 6765 7442 7563 6b65 7473 4461 7461 2822  getBucketsData("
-00005290: 7465 7374 2d62 7563 6b65 7422 290a 2320  test-bucket").# 
-000052a0: 7465 7374 5f61 7373 756d 6552 6f6c 6528  test_assumeRole(
-000052b0: 290a 0a23 2063 6f70 795f 656e 6372 7970  )..# copy_encryp
-000052c0: 7469 6f6e 2827 6172 7469 636c 652e 656e  tion('article.en
-000052d0: 6372 7970 7469 6f6e 2e74 7874 272c 2027  cryption.txt', '
-000052e0: 6172 7469 636c 652e 7478 7427 2c20 656e  article.txt', en
-000052f0: 6372 7970 745f 6b65 793d 5472 7565 290a  crypt_key=True).
-00005300: 0a23 2066 696c 654e 616d 6520 3d20 225c  .# fileName = "\
-00005310: 7530 3036 625c 7530 3037 335c 7530 3035  u006b\u0073\u005
-00005320: 665c 7530 3037 335c 7530 3036 335c 7530  f\u0073\u0063\u0
-00005330: 3036 315c 7530 3036 655c 7530 3035 665c  061\u006e\u005f\
-00005340: 7530 3036 665c 7530 3036 335c 7530 3037  u006f\u0063\u007
-00005350: 325c 7530 3032 665c 7530 3033 325c 7530  2\u002f\u0032\u0
-00005360: 3033 305c 7530 3033 315c 7530 3033 385c  030\u0031\u0038\
-00005370: 7530 3032 645c 7530 3033 305c 7530 3033  u002d\u0030\u003
-00005380: 335c 7530 3032 645c 7530 3033 315c 7530  3\u002d\u0031\u0
-00005390: 3033 325c 7530 3032 665c 7530 3031 305c  032\u002f\u0010\
-000053a0: 7566 6666 645c 7530 3037 305c 7566 6666  ufffd\u0070\ufff
-000053b0: 645c 7566 6666 645c 7566 6666 645c 7530  d\ufffd\ufffd\u0
-000053c0: 3030 325c 7530 3032 655c 7530 3035 375c  002\u002e\u0057\
-000053d0: 7530 3037 665c 7530 3035 625c 7566 6666  u007f\u005b\ufff
-000053e0: 645c 7530 3030 385c 7566 6666 645c 7530  d\u0008\ufffd\u0
-000053f0: 3032 615c 7566 6666 645c 7530 3032 655c  02a\ufffd\u002e\
-00005400: 7530 3036 615c 7530 3037 305c 7530 3036  u006a\u0070\u006
-00005410: 3722 3b0a 2320 6865 6865 203d 2022 10ef  7";.# hehe = "..
-00005420: bfbd 70ef bfbd efbf bdef bfbd 022e 577f  ..p...........W.
-00005430: 5bef bfbd 2aef bfbd 2e6a 7067 220a 2320  [...*....jpg".# 
-00005440: 666f 7220 6320 696e 2068 6568 653a 0a23  for c in hehe:.#
-00005450: 2020 2020 2070 7269 6e74 2872 6570 7228       print(repr(
-00005460: 6329 2c20 6329 0a23 2075 726c 636f 6465  c), c).# urlcode
-00005470: 6420 3d20 7572 6c6c 6962 2e70 6172 7365  d = urllib.parse
-00005480: 2e71 756f 7465 2866 696c 654e 616d 6529  .quote(fileName)
-00005490: 0a23 2075 6e71 756f 7465 6420 3d20 7572  .# unquoted = ur
-000054a0: 6c6c 6962 2e70 6172 7365 2e75 6e71 756f  llib.parse.unquo
-000054b0: 7465 2827 2546 4627 290a 2320 7175 6f74  te('%FF').# quot
-000054c0: 6564 203d 2075 726c 6c69 622e 7061 7273  ed = urllib.pars
-000054d0: 652e 7175 6f74 6528 756e 7175 6f74 6564  e.quote(unquoted
-000054e0: 290a 2320 7072 696e 7428 756e 7175 6f74  ).# print(unquot
-000054f0: 6564 290a 2320 7072 696e 7428 7175 6f74  ed).# print(quot
-00005500: 6564 290a 0a23 2067 6574 4f62 6a65 6374  ed)..# getObject
-00005510: 4d65 7461 2827 7465 7374 2d62 7563 6b65  Meta('test-bucke
-00005520: 7427 2c20 2761 7274 6963 6c65 2e74 7874  t', 'article.txt
-00005530: 2729 0a23 206b 6579 203d 2063 6f70 7928  ').# key = copy(
-00005540: 2761 7274 6963 6c65 2e74 7874 272c 2027  'article.txt', '
-00005550: 6172 7469 636c 652e 7478 7427 2c20 6473  article.txt', ds
-00005560: 745f 6275 636b 6574 5f6e 616d 653d 2774  t_bucket_name='t
-00005570: 6573 742d 6275 636b 6574 2729 0a23 2070  est-bucket').# p
-00005580: 7269 6e74 2827 6166 7465 7220 636f 7079  rint('after copy
-00005590: 5c6e 5c6e 2729 0a23 2067 6574 4f62 6a65  \n\n').# getObje
-000055a0: 6374 4d65 7461 2827 7465 7374 2d62 7563  ctMeta('test-buc
-000055b0: 6b65 7427 2c20 2761 7274 6963 6c65 2e74  ket', 'article.t
-000055c0: 7874 2729 0a23 2067 6574 4f62 6a65 6374  xt').# getObject
-000055d0: 4d65 7461 2827 7465 7374 2d62 7563 6b65  Meta('test-bucke
-000055e0: 7427 2c20 2744 5343 3033 3338 302e 7373  t', 'DSC03380.ss
-000055f0: 6563 2e6a 7067 2729 0a23 2075 706c 6f61  ec.jpg').# uploa
-00005600: 644f 626a 6563 7446 726f 6d46 696c 6528  dObjectFromFile(
-00005610: 2744 5343 3033 3338 302e 656e 6372 7970  'DSC03380.encryp
-00005620: 742e 6a70 6727 290a 0a23 2069 6d70 6f72  t.jpg')..# impor
-00005630: 7420 6261 7365 3634 0a23 2069 6d70 6f72  t base64.# impor
-00005640: 7420 686d 6163 0a23 2069 6d70 6f72 7420  t hmac.# import 
-00005650: 6861 7368 6c69 620a 2320 696d 706f 7274  hashlib.# import
-00005660: 2075 726c 6c69 620a 2320 6820 3d20 686d   urllib.# h = hm
-00005670: 6163 2e6e 6577 2822 6163 6365 7373 6b65  ac.new("accesske
-00005680: 7922 2c0a 2320 2020 2020 2020 2020 2020  y",.#           
-00005690: 2020 2022 4745 545c 6e5c 6e5c 6e31 3134     "GET\n\n\n114
-000056a0: 3138 3839 3132 305c 6e2f 6578 616d 706c  1889120\n/exampl
-000056b0: 6562 7563 6b65 742f 6f73 732d 6170 692e  ebucket/oss-api.
-000056c0: 7064 6622 2c0a 2320 2020 2020 2020 2020  pdf",.#         
-000056d0: 2020 2020 2068 6173 686c 6962 2e73 6861       hashlib.sha
-000056e0: 3129 0a23 2075 726c 6c69 622e 7175 6f74  1).# urllib.quot
-000056f0: 6520 2862 6173 6536 342e 656e 636f 6465  e (base64.encode
-00005700: 7374 7269 6e67 2868 2e64 6967 6573 7428  string(h.digest(
-00005710: 2929 2e73 7472 6970 2829 290a 0a23 2062  )).strip())..# b
-00005720: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
-00005730: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
-00005740: 2320 2320 666f 7220 7020 696e 2062 2e67  # # for p in b.g
-00005750: 6574 5f61 6c6c 5f6d 756c 7469 7061 7274  et_all_multipart
-00005760: 5f75 706c 6f61 6473 286b 6579 5f6d 6172  _uploads(key_mar
-00005770: 6b65 723d 2774 6573 742d 6d75 6c74 6927  ker='test-multi'
-00005780: 2c20 7570 6c6f 6164 5f69 645f 6d61 726b  , upload_id_mark
-00005790: 6572 3d27 6262 6663 6630 6261 6235 6538  er='bbfcf0bab5e8
-000057a0: 3435 6438 3935 6430 6366 6364 3236 3332  45d895d0cfcd2632
-000057b0: 6266 3138 2729 3a20 2020 2027 3765 3662  bf18'):    '7e6b
-000057c0: 3762 3739 3132 6431 3465 6230 3934 3234  7b7912d14eb09424
-000057d0: 3133 6632 3632 6334 3838 6563 270a 2320  13f262c488ec'.# 
-000057e0: 616c 6c5f 7570 6c6f 6164 7320 3d20 622e  all_uploads = b.
-000057f0: 6765 745f 616c 6c5f 6d75 6c74 6970 6172  get_all_multipar
-00005800: 745f 7570 6c6f 6164 7328 6b65 795f 6d61  t_uploads(key_ma
-00005810: 726b 6572 3d27 4453 4330 3333 3830 2e65  rker='DSC03380.e
-00005820: 6e63 7279 7074 2e6a 7067 2d64 6464 6464  ncrypt.jpg-ddddd
-00005830: 6464 6427 2923 6d61 785f 7570 6c6f 6164  ddd')#max_upload
-00005840: 733d 3237 290a 2320 7072 696e 7428 6c65  s=27).# print(le
-00005850: 6e28 616c 6c5f 7570 6c6f 6164 7329 290a  n(all_uploads)).
-00005860: 2320 666f 7220 7020 696e 2061 6c6c 5f75  # for p in all_u
-00005870: 706c 6f61 6473 3a0a 2320 2020 7072 696e  ploads:.#   prin
-00005880: 7428 702c 2070 2e69 6429 0a23 2070 7574  t(p, p.id).# put
-00005890: 5f6f 626a 6563 745f 6361 6c6c 6261 636b  _object_callback
-000058a0: 2827 7465 7374 2d63 616c 6c62 6163 6b27  ('test-callback'
-000058b0: 29                                       )
+00000140: 7273 6572 732e 6275 636b 6574 4372 6f73  rsers.bucketCros
+00000150: 7352 6570 6c69 6361 7465 2069 6d70 6f72  sReplicate impor
+00000160: 7420 4275 636b 6574 4372 6f73 7352 6570  t BucketCrossRep
+00000170: 6c69 6361 7465 0a66 726f 6d20 6b73 332e  licate.from ks3.
+00000180: 786d 6c50 6172 7365 7273 2e62 7563 6b65  xmlParsers.bucke
+00000190: 744c 6966 6563 7963 6c65 2069 6d70 6f72  tLifecycle impor
+000001a0: 7420 4275 636b 6574 4c69 6665 6379 636c  t BucketLifecycl
+000001b0: 652c 2052 756c 6520 6173 204c 6966 6563  e, Rule as Lifec
+000001c0: 7963 6c65 5275 6c65 2c20 4669 6c74 6572  ycleRule, Filter
+000001d0: 2061 7320 4c69 6665 6379 636c 6546 696c   as LifecycleFil
+000001e0: 7465 722c 205c 0a20 2045 7870 6972 6174  ter, \.  Expirat
+000001f0: 696f 6e20 6173 204c 6966 6563 7963 6c65  ion as Lifecycle
+00000200: 4578 7069 7261 7469 6f6e 2c20 5472 616e  Expiration, Tran
+00000210: 7369 7469 6f6e 2061 7320 4c69 6665 6379  sition as Lifecy
+00000220: 636c 6554 7261 6e73 6974 696f 6e2c 2041  cleTransition, A
+00000230: 626f 7274 496e 636f 6d70 6c65 7465 4d75  bortIncompleteMu
+00000240: 6c74 6970 6172 7455 706c 6f61 640a 6672  ltipartUpload.fr
+00000250: 6f6d 206b 7333 2e78 6d6c 5061 7273 6572  om ks3.xmlParser
+00000260: 732e 6275 636b 6574 4c6f 6767 696e 6720  s.bucketLogging 
+00000270: 696d 706f 7274 2042 7563 6b65 744c 6f67  import BucketLog
+00000280: 6769 6e67 0a23 20e9 a696 e585 88e5 889d  ging.# .........
+00000290: e5a7 8be5 8c96 4163 6365 7373 4b65 7949  ......AccessKeyI
+000002a0: 64e3 8081 4163 6365 7373 4b65 7953 6563  d...AccessKeySec
+000002b0: 7265 74e3 8081 456e 6470 6f69 6e74 e7ad  ret...Endpoint..
+000002c0: 89e4 bfa1 e681 afe3 8082 0a23 20e9 809a  ...........# ...
+000002d0: e8bf 87e7 8eaf e5a2 83e5 8f98 e987 8fe8  ................
+000002e0: 8eb7 e58f 96ef bc8c e688 96e8 8085 e68a  ................
+000002f0: 8ae8 afb8 e5a6 82e2 809c 3ce4 bda0 e79a  ..........<.....
+00000300: 8441 6363 6573 734b 6579 4964 3ee2 809d  .AccessKeyId>...
+00000310: e69b bfe6 8da2 e688 90e7 9c9f e5ae 9ee7  ................
+00000320: 9a84 4163 6365 7373 4b65 7949 64e7 ad89  ..AccessKeyId...
+00000330: e380 820a 6672 6f6d 206b 7333 2e78 6d6c  ....from ks3.xml
+00000340: 5061 7273 6572 732e 6275 636b 6574 4d69  Parsers.bucketMi
+00000350: 7272 6f72 2069 6d70 6f72 7420 4275 636b  rror import Buck
+00000360: 6574 4d69 7272 6f72 2c20 4173 796e 634d  etMirror, AsyncM
+00000370: 6972 726f 7252 756c 652c 2053 796e 634d  irrorRule, SyncM
+00000380: 6972 726f 7252 756c 6573 2c20 4d69 7272  irrorRules, Mirr
+00000390: 6f72 5265 7175 6573 7453 6574 7469 6e67  orRequestSetting
+000003a0: 2c20 5c0a 2020 4865 6164 6572 5365 7474  , \.  HeaderSett
+000003b0: 696e 670a 6672 6f6d 206b 7333 2e78 6d6c  ing.from ks3.xml
+000003c0: 5061 7273 6572 732e 6275 636b 6574 5265  Parsers.bucketRe
+000003d0: 7465 6e74 696f 6e20 696d 706f 7274 2042  tention import B
+000003e0: 7563 6b65 7452 6574 656e 7469 6f6e 2c20  ucketRetention, 
+000003f0: 5275 6c65 2061 7320 5265 7465 6e74 696f  Rule as Retentio
+00000400: 6e52 756c 650a 6672 6f6d 2062 6173 6536  nRule.from base6
+00000410: 3420 696d 706f 7274 2075 726c 7361 6665  4 import urlsafe
+00000420: 5f62 3634 656e 636f 6465 0a69 6d70 6f72  _b64encode.impor
+00000430: 7420 6173 796e 6369 6f0a 0a61 6b20 3d20  t asyncio..ak = 
+00000440: 6f73 2e67 6574 656e 7628 274b 5333 5f49  os.getenv('KS3_I
+00000450: 414d 5f41 4343 4553 535f 4b45 595f 4944  AM_ACCESS_KEY_ID
+00000460: 272c 2027 3c59 4f55 525f 4143 4345 5353  ', '<YOUR_ACCESS
+00000470: 5f4b 4559 3e27 290a 736b 203d 206f 732e  _KEY>').sk = os.
+00000480: 6765 7465 6e76 2827 4b53 335f 4941 4d5f  getenv('KS3_IAM_
+00000490: 4143 4345 5353 5f4b 4559 5f53 4543 5245  ACCESS_KEY_SECRE
+000004a0: 5427 2c20 273c 594f 5552 5f53 4543 5245  T', '<YOUR_SECRE
+000004b0: 545f 4b45 593e 2729 0a62 7563 6b65 745f  T_KEY>').bucket_
+000004c0: 6e61 6d65 203d 206f 732e 6765 7465 6e76  name = os.getenv
+000004d0: 2827 4b53 335f 4255 434b 4554 272c 2027  ('KS3_BUCKET', '
+000004e0: 3c4b 5333 5f54 4553 545f 4255 434b 4554  <KS3_TEST_BUCKET
+000004f0: 3e27 290a 656e 6470 6f69 6e74 203d 2027  >').endpoint = '
+00000500: 6b73 332d 636e 2d62 6569 6a69 6e67 2e6b  ks3-cn-beijing.k
+00000510: 7379 756e 6373 2e63 6f6d 2720 236f 732e  syuncs.com' #os.
+00000520: 6765 7465 6e76 2827 4b53 335f 5445 5354  getenv('KS3_TEST
+00000530: 5f45 4e44 504f 494e 5427 2c20 276b 7333  _ENDPOINT', 'ks3
+00000540: 2d63 6e2d 7368 616e 6768 6169 2d69 6e74  -cn-shanghai-int
+00000550: 6572 6e61 6c2e 6b73 7975 6e63 732e 636f  ernal.ksyuncs.co
+00000560: 6d27 290a 0a63 6f6e 6e20 3d20 436f 6e6e  m')..conn = Conn
+00000570: 6563 7469 6f6e 2861 6b2c 2073 6b2c 2068  ection(ak, sk, h
+00000580: 6f73 743d 656e 6470 6f69 6e74 2c20 706f  ost=endpoint, po
+00000590: 7274 3d38 302c 2075 615f 6164 646f 6e3d  rt=80, ua_addon=
+000005a0: 2774 6573 742d 7561 2f31 2729 2023 706f  'test-ua/1') #po
+000005b0: 7274 3d38 3039 312c 0a6b 6579 5f6e 616d  rt=8091,.key_nam
+000005c0: 6520 3d20 2774 6573 745f 6b65 7927 0a0a  e = 'test_key'..
+000005d0: 0a64 6566 2067 6574 416c 6c42 7563 6b65  .def getAllBucke
+000005e0: 7473 2870 726f 6a65 6374 5f69 6473 3d4e  ts(project_ids=N
+000005f0: 6f6e 6529 3a0a 2020 6275 636b 6574 7320  one):.  buckets 
+00000600: 3d20 636f 6e6e 2e67 6574 5f61 6c6c 5f62  = conn.get_all_b
+00000610: 7563 6b65 7473 2870 726f 6a65 6374 5f69  uckets(project_i
+00000620: 6473 3d70 726f 6a65 6374 5f69 6473 2920  ds=project_ids) 
+00000630: 230a 2020 666f 7220 6220 696e 2062 7563  #.  for b in buc
+00000640: 6b65 7473 3a0a 2020 2020 7072 696e 7428  kets:.    print(
+00000650: 622e 6e61 6d65 2c20 622e 7265 6769 6f6e  b.name, b.region
+00000660: 2c20 622e 5265 6769 6f6e 2c20 622e 6372  , b.Region, b.cr
+00000670: 6561 7469 6f6e 5f64 6174 6529 0a0a 6465  eation_date)..de
+00000680: 6620 6865 6164 4275 636b 6574 2862 7563  f headBucket(buc
+00000690: 6b65 745f 6e61 6d65 293a 0a20 2023 20e5  ket_name):.  # .
+000006a0: a682 e69e 9ce6 ada3 e5b8 b8e8 bf94 e59b  ................
+000006b0: 9eef bc8c e588 9942 7563 6b65 74e5 ad98  .......Bucket...
+000006c0: e59c a8ef bc9b e5a6 82e6 9e9c e68a 9be5  ................
+000006d0: 87ba 5333 5265 7370 6f6e 7365 4572 726f  ..S3ResponseErro
+000006e0: 720a 2020 636f 6e6e 2e68 6561 645f 6275  r.  conn.head_bu
+000006f0: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00000700: 290a 0a64 6566 2067 6574 4275 636b 6574  )..def getBucket
+00000710: 4c6f 6361 7469 6f6e 2862 7563 6b65 745f  Location(bucket_
+00000720: 6e61 6d65 293a 0a20 2070 7269 6e74 2863  name):.  print(c
+00000730: 6f6e 6e2e 6765 745f 6275 636b 6574 5f6c  onn.get_bucket_l
+00000740: 6f63 6174 696f 6e28 6275 636b 6574 5f6e  ocation(bucket_n
+00000750: 616d 6529 290a 0a64 6566 2063 7265 6174  ame))..def creat
+00000760: 6542 7563 6b65 7428 6275 636b 6574 5f6e  eBucket(bucket_n
+00000770: 616d 652c 206c 6f63 6174 696f 6e3d 2727  ame, location=''
+00000780: 293a 0a20 2063 6f6e 6e2e 6372 6561 7465  ):.  conn.create
+00000790: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+000007a0: 616d 652c 206c 6f63 6174 696f 6e3d 6c6f  ame, location=lo
+000007b0: 6361 7469 6f6e 2c20 6865 6164 6572 733d  cation, headers=
+000007c0: 7b0a 2020 2020 2778 2d6b 7373 2d62 7563  {.    'x-kss-buc
+000007d0: 6b65 742d 7479 7065 273a 2027 4152 4348  ket-type': 'ARCH
+000007e0: 4956 4527 0a20 207d 290a 0a64 6566 2064  IVE'.  })..def d
+000007f0: 656c 6574 6542 7563 6b65 7428 6275 636b  eleteBucket(buck
+00000800: 6574 5f6e 616d 6529 3a0a 2020 7472 793a  et_name):.  try:
+00000810: 0a20 2020 2063 6f6e 6e2e 6465 6c65 7465  .    conn.delete
+00000820: 5f62 7563 6b65 7428 6275 636b 6574 5f6e  _bucket(bucket_n
+00000830: 616d 6529 0a20 2065 7863 6570 7420 5333  ame).  except S3
+00000840: 5265 7370 6f6e 7365 4572 726f 7220 6173  ResponseError as
+00000850: 2065 7272 6f72 3a0a 2020 2020 7072 696e   error:.    prin
+00000860: 7428 2765 7272 6f72 2729 0a20 2020 2070  t('error').    p
+00000870: 7269 6e74 2865 7272 6f72 290a 0a64 6566  rint(error)..def
+00000880: 2067 6574 4275 636b 6574 4163 6c28 6275   getBucketAcl(bu
+00000890: 636b 6574 5f6e 616d 6529 3a0a 2020 6220  cket_name):.  b 
+000008a0: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+000008b0: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+000008c0: 2070 6f6c 6963 7920 3d20 622e 6765 745f   policy = b.get_
+000008d0: 6163 6c28 290a 2020 2320 7072 696e 7428  acl().  # print(
+000008e0: 706f 6c69 6379 290a 2020 666f 7220 6772  policy).  for gr
+000008f0: 616e 7420 696e 2070 6f6c 6963 792e 6163  ant in policy.ac
+00000900: 6c2e 6772 616e 7473 3a0a 2020 2020 7072  l.grants:.    pr
+00000910: 696e 7428 6772 616e 742e 7065 726d 6973  int(grant.permis
+00000920: 7369 6f6e 2c20 6772 616e 742e 6469 7370  sion, grant.disp
+00000930: 6c61 795f 6e61 6d65 2c20 6772 616e 742e  lay_name, grant.
+00000940: 656d 6169 6c5f 6164 6472 6573 732c 2067  email_address, g
+00000950: 7261 6e74 2e69 6429 0a0a 6465 6620 7365  rant.id)..def se
+00000960: 7442 7563 6b65 7441 636c 2862 7563 6b65  tBucketAcl(bucke
+00000970: 745f 6e61 6d65 293a 0a20 2062 203d 2063  t_name):.  b = c
+00000980: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00000990: 7563 6b65 745f 6e61 6d65 290a 2020 622e  ucket_name).  b.
+000009a0: 7365 745f 6163 6c28 2270 7269 7661 7465  set_acl("private
+000009b0: 2229 0a0a 6465 6620 6d61 6e61 6765 4275  ")..def manageBu
+000009c0: 636b 6574 506f 6c69 6379 2862 7563 6b65  cketPolicy(bucke
+000009d0: 745f 6e61 6d65 293a 0a20 2062 7563 6b65  t_name):.  bucke
+000009e0: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
+000009f0: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
+00000a00: 0a20 2062 7563 6b65 742e 7365 745f 6275  .  bucket.set_bu
+00000a10: 636b 6574 5f70 6f6c 6963 7928 0a20 2020  cket_policy(.   
+00000a20: 2070 6f6c 6963 793d 277b 2253 7461 7465   policy='{"State
+00000a30: 6d65 6e74 223a 5b7b 2252 6573 6f75 7263  ment":[{"Resourc
+00000a40: 6522 3a5b 226b 726e 3a6b 7363 3a6b 7333  e":["krn:ksc:ks3
+00000a50: 3a3a 3a6a 6961 6e67 7261 6e31 3233 222c  :::jiangran123",
+00000a60: 226b 726e 3a6b 7363 3a6b 7333 3a3a 3a6a  "krn:ksc:ks3:::j
+00000a70: 6961 6e67 7261 6e31 3233 2f2a 225d 2c22  iangran123/*"],"
+00000a80: 5072 696e 6369 7061 6c22 3a7b 224b 5343  Principal":{"KSC
+00000a90: 223a 5b22 6b72 6e3a 6b73 633a 6961 6d3a  ":["krn:ksc:iam:
+00000aa0: 3a33 3234 3332 3432 333a 726f 6f74 225d  :32432423:root"]
+00000ab0: 7d2c 2241 6374 696f 6e22 3a5b 226b 7333  },"Action":["ks3
+00000ac0: 3a2a 225d 2c22 4566 6665 6374 223a 2241  :*"],"Effect":"A
+00000ad0: 6c6c 6f77 227d 5d7d 2729 0a20 2023 2070  llow"}]}').  # p
+00000ae0: 6f6c 6963 7920 3d20 6275 636b 6574 2e67  olicy = bucket.g
+00000af0: 6574 5f62 7563 6b65 745f 706f 6c69 6379  et_bucket_policy
+00000b00: 2829 0a20 2023 2062 7563 6b65 742e 6465  ().  # bucket.de
+00000b10: 6c65 7465 5f62 7563 6b65 745f 706f 6c69  lete_bucket_poli
+00000b20: 6379 2829 0a0a 6465 6620 6d61 6e61 6765  cy()..def manage
+00000b30: 4275 636b 6574 5265 706c 6963 6174 696f  BucketReplicatio
+00000b40: 6e28 6275 636b 6574 5f6e 616d 6529 3a0a  n(bucket_name):.
+00000b50: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00000b60: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00000b70: 745f 6e61 6d65 290a 2020 7472 793a 0a20  t_name).  try:. 
+00000b80: 2020 2070 7269 6e74 2862 7563 6b65 742e     print(bucket.
+00000b90: 6765 745f 6275 636b 6574 5f63 7272 2829  get_bucket_crr()
+00000ba0: 2e74 6f5f 786d 6c28 2929 0a20 2065 7863  .to_xml()).  exc
+00000bb0: 6570 743a 0a20 2020 2062 7563 6b65 742e  ept:.    bucket.
+00000bc0: 7365 745f 6275 636b 6574 5f63 7272 2827  set_bucket_crr('
+00000bd0: 7465 7374 2d62 7563 6b65 742d 7072 6f6a  test-bucket-proj
+00000be0: 6563 7427 2c20 6465 6c65 7465 4d61 726b  ect', deleteMark
+00000bf0: 6572 5374 6174 7573 3d27 4469 7361 626c  erStatus='Disabl
+00000c00: 6564 272c 2070 7265 6669 785f 6c69 7374  ed', prefix_list
+00000c10: 3d5b 2768 656c 6c6f 275d 290a 0a64 6566  =['hello'])..def
+00000c20: 2067 6574 4275 636b 6574 4c69 6665 4379   getBucketLifeCy
+00000c30: 636c 6528 6275 636b 6574 5f6e 616d 6529  cle(bucket_name)
+00000c40: 3a0a 2020 6275 636b 6574 203d 2063 6f6e  :.  bucket = con
+00000c50: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
+00000c60: 6b65 745f 6e61 6d65 290a 2020 6c69 6665  ket_name).  life
+00000c70: 6379 636c 6520 3d20 6275 636b 6574 2e67  cycle = bucket.g
+00000c80: 6574 5f62 7563 6b65 745f 6c69 6665 6379  et_bucket_lifecy
+00000c90: 636c 6528 290a 2020 7072 696e 7428 6c69  cle().  print(li
+00000ca0: 6665 6379 636c 652e 746f 5f78 6d6c 2829  fecycle.to_xml()
+00000cb0: 290a 0a64 6566 2073 6574 4275 636b 6574  )..def setBucket
+00000cc0: 4c69 6665 4379 636c 6528 6275 636b 6574  LifeCycle(bucket
+00000cd0: 5f6e 616d 6529 3a0a 2020 6275 636b 6574  _name):.  bucket
+00000ce0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+00000cf0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+00000d00: 2020 6c69 6665 6379 636c 6520 3d20 4275    lifecycle = Bu
+00000d10: 636b 6574 4c69 6665 6379 636c 6528 290a  cketLifecycle().
+00000d20: 2020 2320 6964 20e5 928c 2073 7461 7475    # id ... statu
+00000d30: 7320 e5bf 85e9 a1bb 0a20 2072 756c 6520  s .......  rule 
+00000d40: 3d20 4c69 6665 6379 636c 6552 756c 6528  = LifecycleRule(
+00000d50: 6964 3d27 7275 6c65 3127 2c20 7374 6174  id='rule1', stat
+00000d60: 7573 3d27 456e 6162 6c65 6427 290a 2020  us='Enabled').  
+00000d70: 6461 7465 203d 2064 6174 6574 696d 6528  date = datetime(
+00000d80: 3230 3231 2c20 392c 2031 3229 2e73 7472  2021, 9, 12).str
+00000d90: 6674 696d 6528 2725 592d 256d 2d25 6454  ftime('%Y-%m-%dT
+00000da0: 2548 3a25 4d3a 2553 2729 202b 2027 2b30  %H:%M:%S') + '+0
+00000db0: 383a 3030 270a 2020 7275 6c65 2e65 7870  8:00'.  rule.exp
+00000dc0: 6972 6174 696f 6e20 3d20 4c69 6665 6379  iration = Lifecy
+00000dd0: 636c 6545 7870 6972 6174 696f 6e28 6461  cleExpiration(da
+00000de0: 7465 3d64 6174 6529 0a20 206c 6966 6563  te=date).  lifec
+00000df0: 7963 6c65 2e72 756c 6520 3d20 5b72 756c  ycle.rule = [rul
+00000e00: 655d 0a20 2062 7563 6b65 742e 7365 745f  e].  bucket.set_
+00000e10: 6275 636b 6574 5f6c 6966 6563 7963 6c65  bucket_lifecycle
+00000e20: 286c 6966 6563 7963 6c65 290a 0a0a 6465  (lifecycle)...de
+00000e30: 6620 7365 7442 7563 6b65 744c 6966 6543  f setBucketLifeC
+00000e40: 7963 6c65 3228 6275 636b 6574 5f6e 616d  ycle2(bucket_nam
+00000e50: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
+00000e60: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00000e70: 7563 6b65 745f 6e61 6d65 290a 2020 7461  ucket_name).  ta
+00000e80: 6720 3d20 5461 6728 6b65 793d 2274 6167  g = Tag(key="tag
+00000e90: 3122 2c20 7661 6c75 653d 2274 6573 7431  1", value="test1
+00000ea0: 2229 0a20 2023 20e7 ad9b e980 89e5 898d  ").  # .........
+00000eb0: e7bc 80e4 b8ba 2070 7265 6669 7831 e380  ...... prefix1..
+00000ec0: 81e6 a087 e7ad bee4 b8ba 2074 6167 313a  .......... tag1:
+00000ed0: 7465 7374 3120 e79a 8420 6f62 6a65 6374  test1 ... object
+00000ee0: 73ef bc8c e8ae bee7 bdae e8bf 87e6 9c9f  s...............
+00000ef0: e8a7 84e5 8899 efbc 8ce5 9ca8 e585 b6e6  ................
+00000f00: 9c80 e590 8ee4 bfae e694 b9e6 97b6 e997  ................
+00000f10: b433 e5a4 a9e5 908e e8bf 87e6 9c9f e380  .3..............
+00000f20: 820a 2020 7275 6c65 3120 3d20 4c69 6665  ..  rule1 = Life
+00000f30: 6379 636c 6552 756c 6528 2772 756c 6531  cycleRule('rule1
+00000f40: 272c 204c 6966 6563 7963 6c65 4669 6c74  ', LifecycleFilt
+00000f50: 6572 2827 7072 6566 6978 3127 2c20 7461  er('prefix1', ta
+00000f60: 6773 3d5b 7461 675d 292c 0a20 2020 2020  gs=[tag]),.     
+00000f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000f80: 2020 2073 7461 7475 733d 2745 6e61 626c     status='Enabl
+00000f90: 6564 272c 0a20 2020 2020 2020 2020 2020  ed',.           
+00000fa0: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+00000fb0: 6972 6174 696f 6e3d 4c69 6665 6379 636c  iration=Lifecycl
+00000fc0: 6545 7870 6972 6174 696f 6e28 6461 7973  eExpiration(days
+00000fd0: 3d33 2929 0a0a 2020 2320 e8ae bee7 bdae  =3))..  # ......
+00000fe0: e8bf 87e6 9c9f e8a7 84e5 8899 efbc 8ce7  ................
+00000ff0: ad9b e980 89e6 a087 e7ad bee4 b8ba 2074  .............. t
+00001000: 6167 313a 7465 7374 3120 e79a 8420 6f62  ag1:test1 ... ob
+00001010: 6a65 6374 73ef bc8c e69c 80e5 908e e4bf  jects...........
+00001020: aee6 94b9 e697 b6e9 97b4 e59c a8e6 8c87  ................
+00001030: e5ae 9ae6 97a5 e69c 9fe4 b98b e589 8de7  ................
+00001040: 9a84 efbc 8ce8 bf87 e69c 9f0a 2020 7275  ............  ru
+00001050: 6c65 3220 3d20 4c69 6665 6379 636c 6552  le2 = LifecycleR
+00001060: 756c 6528 2772 756c 6532 272c 204c 6966  ule('rule2', Lif
+00001070: 6563 7963 6c65 4669 6c74 6572 2874 6167  ecycleFilter(tag
+00001080: 733d 5b74 6167 5d29 2c0a 2020 2020 2020  s=[tag]),.      
+00001090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010a0: 2020 7374 6174 7573 3d27 456e 6162 6c65    status='Enable
+000010b0: 6427 2c0a 2020 2020 2020 2020 2020 2020  d',.            
+000010c0: 2020 2020 2020 2020 2020 2020 6578 7069              expi
+000010d0: 7261 7469 6f6e 3d4c 6966 6563 7963 6c65  ration=Lifecycle
+000010e0: 4578 7069 7261 7469 6f6e 280a 2020 2020  Expiration(.    
+000010f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001100: 2020 2020 2020 6461 7465 3d64 6174 6574        date=datet
+00001110: 696d 6528 3230 3231 2c20 3132 2c20 3132  ime(2021, 12, 12
+00001120: 292e 6973 6f66 6f72 6d61 7428 7469 6d65  ).isoformat(time
+00001130: 7370 6563 3d27 7365 636f 6e64 7327 2920  spec='seconds') 
+00001140: 2b20 272b 3038 3a30 3027 2929 0a0a 2020  + '+08:00'))..  
+00001150: 2320 e8ae bee7 bdae e5ad 98e5 82a8 e7b1  # ..............
+00001160: bbe5 9e8b e8bd ace6 8da2 e8a7 84e5 8899  ................
+00001170: efbc 8ce7 ad9b e980 89e5 898d e7bc 80e4  ................
+00001180: b8ba 2070 7265 6669 7833 20e7 9a84 206f  .. prefix3 ... o
+00001190: 626a 6563 7473 efbc 8ce5 9ca8 e585 b6e6  bjects..........
+000011a0: 9c80 e590 8ee4 bfae e694 b9e6 97b6 e997  ................
+000011b0: b432 30e5 a4a9 e4b9 8be5 908e e8bd ace4  .20.............
+000011c0: b8ba e4bd 8ee9 a291 e8ae bfe9 97ae e7b1  ................
+000011d0: bbe5 9e8b efbc 8ce5 9ca8 e585 b6e6 9c80  ................
+000011e0: e590 8ee4 bfae e694 b9e6 97b6 e997 b433  ...............3
+000011f0: 30e5 a4a9 e4b9 8be5 908e e8bd ace4 b8ba  0...............
+00001200: e5bd 92e6 a1a3 e7b1 bbe5 9e8b e380 820a  ................
+00001210: 2020 7275 6c65 3320 3d20 4c69 6665 6379    rule3 = Lifecy
+00001220: 636c 6552 756c 6528 2772 756c 6533 272c  cleRule('rule3',
+00001230: 204c 6966 6563 7963 6c65 4669 6c74 6572   LifecycleFilter
+00001240: 2827 7072 6566 6978 3327 292c 0a20 2020  ('prefix3'),.   
+00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001260: 2020 2020 2073 7461 7475 733d 2745 6e61       status='Ena
+00001270: 626c 6564 272c 0a20 2020 2020 2020 2020  bled',.         
+00001280: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001290: 7261 6e73 6974 696f 6e73 3d5b 4c69 6665  ransitions=[Life
+000012a0: 6379 636c 6554 7261 6e73 6974 696f 6e28  cycleTransition(
+000012b0: 6461 7973 3d32 302c 2073 746f 7261 6765  days=20, storage
+000012c0: 5f63 6c61 7373 3d27 5354 414e 4441 5244  _class='STANDARD
+000012d0: 5f49 4127 292c 0a20 2020 2020 2020 2020  _IA'),.         
+000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 2020 2020 2020 2020 4c69 6665              Life
+00001300: 6379 636c 6554 7261 6e73 6974 696f 6e28  cycleTransition(
+00001310: 6461 7973 3d36 302c 2073 746f 7261 6765  days=60, storage
+00001320: 5f63 6c61 7373 3d27 4152 4348 4956 4527  _class='ARCHIVE'
+00001330: 295d 290a 0a20 2023 20e8 aebe e7bd aee5  )])..  # .......
+00001340: ad98 e582 a8e7 b1bb e59e 8be8 bdac e68d  ................
+00001350: a2e8 a784 e588 99ef bc8c e7ad 9be9 8089  ................
+00001360: e589 8de7 bc80 e4b8 ba20 7072 6566 6978  ......... prefix
+00001370: 3320 e79a 8420 6f62 6a65 6374 73ef bc8c  3 ... objects...
+00001380: e69c 80e5 908e e4bf aee6 94b9 e697 b6e9  ................
+00001390: 97b4 e59c a8e6 8c87 e5ae 9ae6 97a5 e69c  ................
+000013a0: 9fe4 b98b e589 8de7 9a84 efbc 8ce8 bdac  ................
+000013b0: e4b8 bae4 bd8e e9a2 91e8 aebf e997 aee7  ................
+000013c0: b1bb e59e 8b0a 2020 7275 6c65 3420 3d20  ......  rule4 = 
+000013d0: 4c69 6665 6379 636c 6552 756c 6528 2772  LifecycleRule('r
+000013e0: 756c 6534 272c 204c 6966 6563 7963 6c65  ule4', Lifecycle
+000013f0: 4669 6c74 6572 2827 7072 6566 6978 3427  Filter('prefix4'
+00001400: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00001410: 2020 2020 2020 2020 2020 2073 7461 7475             statu
+00001420: 733d 2745 6e61 626c 6564 272c 0a20 2020  s='Enabled',.   
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 2020 2074 7261 6e73 6974 696f 6e73       transitions
+00001450: 3d5b 0a20 2020 2020 2020 2020 2020 2020  =[.             
+00001460: 2020 2020 2020 2020 2020 2020 204c 6966               Lif
+00001470: 6563 7963 6c65 5472 616e 7369 7469 6f6e  ecycleTransition
+00001480: 2864 6174 653d 6461 7465 7469 6d65 2832  (date=datetime(2
+00001490: 3032 312c 2031 322c 2031 3229 2e69 736f  021, 12, 12).iso
+000014a0: 666f 726d 6174 2874 696d 6573 7065 633d  format(timespec=
+000014b0: 2773 6563 6f6e 6473 2729 202b 2027 2b30  'seconds') + '+0
+000014c0: 383a 3030 272c 0a20 2020 2020 2020 2020  8:00',.         
+000014d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014f0: 2020 2020 2073 746f 7261 6765 5f63 6c61       storage_cla
+00001500: 7373 3d27 5354 414e 4441 5244 5f49 4127  ss='STANDARD_IA'
+00001510: 295d 290a 2020 2320 e8ae bee7 bdae e588  )]).  # ........
+00001520: 86e7 8987 e4b8 8ae4 bca0 e7a2 8ee7 8987  ................
+00001530: e6b8 85e7 9086 e8a7 84e5 8899 efbc 8ce7  ................
+00001540: ad9b e980 89e5 898d e7bc 80e4 b8ba 2070  .............. p
+00001550: 7265 6669 7835 20e7 9a84 2070 6172 74ef  refix5 ... part.
+00001560: bc8c e59c a8e6 9c80 e590 8ee4 bfae e694  ................
+00001570: b9e6 97b6 e997 b437 e5a4 a9e5 908e e588  .......7........
+00001580: a0e9 99a4 0a20 2072 756c 6535 203d 204c  .....  rule5 = L
+00001590: 6966 6563 7963 6c65 5275 6c65 2827 7275  ifecycleRule('ru
+000015a0: 6c65 3527 2c20 4c69 6665 6379 636c 6546  le5', LifecycleF
+000015b0: 696c 7465 7228 2770 7265 6669 7835 2729  ilter('prefix5')
+000015c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000015d0: 2020 2020 2020 2020 2020 7374 6174 7573            status
+000015e0: 3d27 456e 6162 6c65 6427 2c0a 2020 2020  ='Enabled',.    
+000015f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001600: 2020 2020 6162 6f72 745f 696e 636f 6d70      abort_incomp
+00001610: 6c65 7465 5f6d 756c 7469 7061 7274 5f75  lete_multipart_u
+00001620: 706c 6f61 643d 4162 6f72 7449 6e63 6f6d  pload=AbortIncom
+00001630: 706c 6574 654d 756c 7469 7061 7274 5570  pleteMultipartUp
+00001640: 6c6f 6164 2864 6179 735f 6166 7465 725f  load(days_after_
+00001650: 696e 6974 6961 7469 6f6e 3d37 2929 0a0a  initiation=7))..
+00001660: 2020 2320 7072 696e 7428 7275 6c65 312e    # print(rule1.
+00001670: 746f 5f78 6d6c 2829 290a 2020 2320 7072  to_xml()).  # pr
+00001680: 696e 7428 7275 6c65 322e 746f 5f78 6d6c  int(rule2.to_xml
+00001690: 2829 290a 2020 2320 7072 696e 7428 7275  ()).  # print(ru
+000016a0: 6c65 332e 746f 5f78 6d6c 2829 290a 2020  le3.to_xml()).  
+000016b0: 2320 7072 696e 7428 7275 6c65 342e 746f  # print(rule4.to
+000016c0: 5f78 6d6c 2829 290a 2020 2320 7072 696e  _xml()).  # prin
+000016d0: 7428 7275 6c65 352e 746f 5f78 6d6c 2829  t(rule5.to_xml()
+000016e0: 290a 2020 6c69 6665 6379 636c 6520 3d20  ).  lifecycle = 
+000016f0: 4275 636b 6574 4c69 6665 6379 636c 6528  BucketLifecycle(
+00001700: 5b72 756c 6531 2c20 7275 6c65 322c 2072  [rule1, rule2, r
+00001710: 756c 6533 2c20 7275 6c65 342c 2072 756c  ule3, rule4, rul
+00001720: 6535 5d29 0a20 2062 7563 6b65 742e 7365  e5]).  bucket.se
+00001730: 745f 6275 636b 6574 5f6c 6966 6563 7963  t_bucket_lifecyc
+00001740: 6c65 286c 6966 6563 7963 6c65 290a 0a64  le(lifecycle)..d
+00001750: 6566 2064 656c 6574 6542 7563 6b65 744c  ef deleteBucketL
+00001760: 6966 6543 7963 6c65 2862 7563 6b65 745f  ifeCycle(bucket_
+00001770: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+00001780: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00001790: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+000017a0: 2062 7563 6b65 742e 6465 6c65 7465 5f62   bucket.delete_b
+000017b0: 7563 6b65 745f 6c69 6665 6379 636c 6528  ucket_lifecycle(
+000017c0: 290a 0a64 6566 2067 6574 4275 636b 6574  )..def getBucket
+000017d0: 4c6f 6767 696e 6728 6275 636b 6574 5f6e  Logging(bucket_n
+000017e0: 616d 6529 3a0a 2020 6275 636b 6574 203d  ame):.  bucket =
+000017f0: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+00001800: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+00001810: 7072 696e 7428 6275 636b 6574 2e67 6574  print(bucket.get
+00001820: 5f62 7563 6b65 745f 6c6f 6767 696e 6728  _bucket_logging(
+00001830: 292e 746f 5f78 6d6c 2829 290a 0a64 6566  ).to_xml())..def
+00001840: 2073 6574 4275 636b 6574 4c6f 6767 696e   setBucketLoggin
+00001850: 6728 6275 636b 6574 5f6e 616d 6529 3a0a  g(bucket_name):.
+00001860: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00001870: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00001880: 745f 6e61 6d65 290a 2020 626c 6f67 6769  t_name).  bloggi
+00001890: 6e67 203d 2042 7563 6b65 744c 6f67 6769  ng = BucketLoggi
+000018a0: 6e67 2874 6172 6765 743d 6275 636b 6574  ng(target=bucket
+000018b0: 5f6e 616d 652c 2074 6172 6765 745f 7072  _name, target_pr
+000018c0: 6566 6978 3d27 7465 7374 5f6c 6f67 2729  efix='test_log')
+000018d0: 0a20 2070 7269 6e74 2862 7563 6b65 742e  .  print(bucket.
+000018e0: 7365 745f 6275 636b 6574 5f6c 6f67 6769  set_bucket_loggi
+000018f0: 6e67 2862 6c6f 6767 696e 672e 746f 5f78  ng(blogging.to_x
+00001900: 6d6c 2829 2929 0a0a 6465 6620 656e 6162  ml()))..def enab
+00001910: 6c65 4275 636b 6574 4c6f 6767 696e 6728  leBucketLogging(
+00001920: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
+00001930: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00001940: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00001950: 6e61 6d65 290a 2020 7072 696e 7428 6275  name).  print(bu
+00001960: 636b 6574 2e65 6e61 626c 655f 6c6f 6767  cket.enable_logg
+00001970: 696e 6728 6275 636b 6574 2c20 7461 7267  ing(bucket, targ
+00001980: 6574 5f70 7265 6669 783d 2768 6568 6568  et_prefix='heheh
+00001990: 6568 6527 2929 0a0a 6465 6620 6469 7361  ehe'))..def disa
+000019a0: 626c 6542 7563 6b65 744c 6f67 6769 6e67  bleBucketLogging
+000019b0: 2862 7563 6b65 745f 6e61 6d65 293a 0a20  (bucket_name):. 
+000019c0: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
+000019d0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
+000019e0: 5f6e 616d 6529 0a20 2070 7269 6e74 2862  _name).  print(b
+000019f0: 7563 6b65 742e 6469 7361 626c 655f 6c6f  ucket.disable_lo
+00001a00: 6767 696e 6728 2929 0a0a 6465 6620 6765  gging())..def ge
+00001a10: 7442 7563 6b65 7443 6f72 7328 6275 636b  tBucketCors(buck
+00001a20: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
+00001a30: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+00001a40: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00001a50: 290a 2020 7072 696e 7428 6275 636b 6574  ).  print(bucket
+00001a60: 2e67 6574 5f62 7563 6b65 745f 636f 7273  .get_bucket_cors
+00001a70: 2829 2e74 6f5f 786d 6c28 2929 0a0a 6465  ().to_xml())..de
+00001a80: 6620 7075 7442 7563 6b65 7443 6f72 7328  f putBucketCors(
+00001a90: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
+00001aa0: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00001ab0: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00001ac0: 6e61 6d65 290a 2020 636f 7273 203d 2042  name).  cors = B
+00001ad0: 7563 6b65 7443 6f72 7328 5b43 4f52 5352  ucketCors([CORSR
+00001ae0: 756c 6528 6f72 6967 696e 733d 5b22 6874  ule(origins=["ht
+00001af0: 7470 3a2f 2f64 6576 2e6b 7379 756e 2e63  tp://dev.ksyun.c
+00001b00: 6f6d 225d 2c20 6d65 7468 6f64 733d 5b22  om"], methods=["
+00001b10: 4745 5422 2c20 2248 4541 4422 5d2c 206d  GET", "HEAD"], m
+00001b20: 6178 5f61 6765 3d22 3230 3022 2c20 6865  ax_age="200", he
+00001b30: 6164 6572 733d 5b22 636f 6e74 656e 742d  aders=["content-
+00001b40: 7479 7065 225d 2c20 6578 706f 7365 645f  type"], exposed_
+00001b50: 6865 6164 6572 733d 5b22 636f 6e74 656e  headers=["conten
+00001b60: 742d 7479 7065 222c 2022 782d 6b73 732d  t-type", "x-kss-
+00001b70: 6163 6c22 5d29 5d29 0a20 2070 7269 6e74  acl"])]).  print
+00001b80: 2827 636f 7273 3a20 272c 2063 6f72 732e  ('cors: ', cors.
+00001b90: 746f 5f78 6d6c 2829 290a 2020 7072 696e  to_xml()).  prin
+00001ba0: 7428 6275 636b 6574 2e73 6574 5f62 7563  t(bucket.set_buc
+00001bb0: 6b65 745f 636f 7273 2863 6f72 7329 290a  ket_cors(cors)).
+00001bc0: 0a64 6566 2064 656c 6574 6542 7563 6b65  .def deleteBucke
+00001bd0: 7443 6f72 7328 6275 636b 6574 5f6e 616d  tCors(bucket_nam
+00001be0: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
+00001bf0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00001c00: 7563 6b65 745f 6e61 6d65 290a 2020 7072  ucket_name).  pr
+00001c10: 696e 7428 6275 636b 6574 2e64 656c 6574  int(bucket.delet
+00001c20: 655f 6275 636b 6574 5f63 6f72 7328 2929  e_bucket_cors())
+00001c30: 0a0a 6465 6620 6765 7442 7563 6b65 7443  ..def getBucketC
+00001c40: 7272 2862 7563 6b65 745f 6e61 6d65 293a  rr(bucket_name):
+00001c50: 0a20 2062 7563 6b65 7420 3d20 636f 6e6e  .  bucket = conn
+00001c60: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
+00001c70: 6574 5f6e 616d 6529 0a20 2070 7269 6e74  et_name).  print
+00001c80: 2862 7563 6b65 742e 6765 745f 6275 636b  (bucket.get_buck
+00001c90: 6574 5f63 7272 2829 2e74 6f5f 786d 6c28  et_crr().to_xml(
+00001ca0: 2929 0a0a 6465 6620 7365 7442 7563 6b65  ))..def setBucke
+00001cb0: 7443 7272 2862 7563 6b65 745f 6e61 6d65  tCrr(bucket_name
+00001cc0: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
+00001cd0: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
+00001ce0: 636b 6574 5f6e 616d 6529 0a20 2023 2064  cket_name).  # d
+00001cf0: 656c 6574 654d 6172 6b65 7253 7461 7475  eleteMarkerStatu
+00001d00: 7320 e79a 84e5 80bc e4b8 ba20 456e 6162  s ......... Enab
+00001d10: 6c65 6420 e592 8c20 4469 7361 626c 6564  led ... Disabled
+00001d20: 0a20 2023 2068 6973 746f 7269 6361 6c4f  .  # historicalO
+00001d30: 626a 6563 7452 6570 6c69 6361 7469 6f6e  bjectReplication
+00001d40: 20e8 a1a8 e7a4 bae6 98af e590 a6e5 bc80   ...............
+00001d50: e590 afe5 ad98 e987 8fe5 a48d e588 b6ef  ................
+00001d60: bc8c e580 bce4 b8ba 2045 6e61 626c 6564  ........ Enabled
+00001d70: 20e5 928c 2044 6973 6162 6c65 640a 2020   ... Disabled.  
+00001d80: 7072 696e 7428 6275 636b 6574 2e73 6574  print(bucket.set
+00001d90: 5f62 7563 6b65 745f 6372 7228 2774 6573  _bucket_crr('tes
+00001da0: 742d 6275 636b 6574 2d72 6570 6c69 272c  t-bucket-repli',
+00001db0: 2064 656c 6574 654d 6172 6b65 7253 7461   deleteMarkerSta
+00001dc0: 7475 733d 4275 636b 6574 4372 6f73 7352  tus=BucketCrossR
+00001dd0: 6570 6c69 6361 7465 2e45 4e41 424c 4544  eplicate.ENABLED
+00001de0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00001df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e00: 6869 7374 6f72 6963 616c 4f62 6a65 6374  historicalObject
+00001e10: 5265 706c 6963 6174 696f 6e3d 4275 636b  Replication=Buck
+00001e20: 6574 4372 6f73 7352 6570 6c69 6361 7465  etCrossReplicate
+00001e30: 2e45 4e41 424c 4544 2c20 7072 6566 6978  .ENABLED, prefix
+00001e40: 3d5b 2768 656c 6c6f 275d 2929 0a0a 6465  =['hello']))..de
+00001e50: 6620 6465 6c65 7465 4275 636b 6574 4372  f deleteBucketCr
+00001e60: 7228 6275 636b 6574 5f6e 616d 6529 3a0a  r(bucket_name):.
+00001e70: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00001e80: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00001e90: 745f 6e61 6d65 290a 2020 7072 696e 7428  t_name).  print(
+00001ea0: 6275 636b 6574 2e64 656c 6574 655f 6275  bucket.delete_bu
+00001eb0: 636b 6574 5f63 7272 2829 290a 0a64 6566  cket_crr())..def
+00001ec0: 2067 6574 4275 636b 6574 4c6f 6767 696e   getBucketLoggin
+00001ed0: 6728 6275 636b 6574 5f6e 616d 6529 3a0a  g(bucket_name):.
+00001ee0: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00001ef0: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00001f00: 745f 6e61 6d65 290a 2020 7072 696e 7428  t_name).  print(
+00001f10: 6275 636b 6574 2e67 6574 5f62 7563 6b65  bucket.get_bucke
+00001f20: 745f 6c6f 6767 696e 6728 292e 746f 5f78  t_logging().to_x
+00001f30: 6d6c 2829 290a 0a64 6566 2073 6574 4275  ml())..def setBu
+00001f40: 636b 6574 4c6f 6767 696e 6728 6275 636b  cketLogging(buck
+00001f50: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
+00001f60: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+00001f70: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00001f80: 290a 2020 626c 6f67 6769 6e67 203d 2042  ).  blogging = B
+00001f90: 7563 6b65 744c 6f67 6769 6e67 2874 6172  ucketLogging(tar
+00001fa0: 6765 743d 6275 636b 6574 5f6e 616d 6529  get=bucket_name)
+00001fb0: 0a20 2070 7269 6e74 2862 7563 6b65 742e  .  print(bucket.
+00001fc0: 7365 745f 6275 636b 6574 5f6c 6f67 6769  set_bucket_loggi
+00001fd0: 6e67 2862 6c6f 6767 696e 672e 746f 5f78  ng(blogging.to_x
+00001fe0: 6d6c 2829 2929 0a0a 6465 6620 6765 7442  ml()))..def getB
+00001ff0: 7563 6b65 744d 6972 726f 7228 6275 636b  ucketMirror(buck
+00002000: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
+00002010: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+00002020: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00002030: 290a 2020 7072 696e 7428 6275 636b 6574  ).  print(bucket
+00002040: 2e67 6574 5f62 7563 6b65 745f 6d69 7272  .get_bucket_mirr
+00002050: 6f72 2829 290a 0a64 6566 2073 6574 4275  or())..def setBu
+00002060: 636b 6574 4d69 7272 6f72 2862 7563 6b65  cketMirror(bucke
+00002070: 745f 6e61 6d65 293a 0a20 2062 7563 6b65  t_name):.  bucke
+00002080: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
+00002090: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
+000020a0: 0a20 2073 6574 5f68 6561 6465 7273 203d  .  set_headers =
+000020b0: 205b 7b0a 2020 2020 2020 226b 6579 223a   [{.      "key":
+000020c0: 2022 6422 2c0a 2020 2020 2020 2276 616c   "d",.      "val
+000020d0: 7565 223a 2022 6222 0a20 207d 5d0a 2020  ue": "b".  }].  
+000020e0: 7265 6d6f 7665 5f68 6561 6465 7273 203d  remove_headers =
+000020f0: 205b 7b0a 2020 2020 2020 226b 6579 223a   [{.      "key":
+00002100: 2022 6422 0a20 207d 5d0a 2020 7061 7373   "d".  }].  pass
+00002110: 5f68 6561 6465 7273 203d 205b 7b0a 2020  _headers = [{.  
+00002120: 2020 2020 226b 6579 223a 2022 6162 6322      "key": "abc"
+00002130: 0a20 207d 5d0a 2020 6865 6164 6572 5f73  .  }].  header_s
+00002140: 6574 7469 6e67 203d 2048 6561 6465 7253  etting = HeaderS
+00002150: 6574 7469 6e67 2873 6574 5f68 6561 6465  etting(set_heade
+00002160: 7273 3d73 6574 5f68 6561 6465 7273 2c20  rs=set_headers, 
+00002170: 7265 6d6f 7665 5f68 6561 6465 7273 3d72  remove_headers=r
+00002180: 656d 6f76 655f 6865 6164 6572 732c 2070  emove_headers, p
+00002190: 6173 735f 616c 6c3d 4661 6c73 652c 2070  ass_all=False, p
+000021a0: 6173 735f 6865 6164 6572 733d 7061 7373  ass_headers=pass
+000021b0: 5f68 6561 6465 7273 290a 2020 6d69 7272  _headers).  mirr
+000021c0: 6f72 5f72 6571 7565 7374 5f73 6574 7469  or_request_setti
+000021d0: 6e67 203d 204d 6972 726f 7252 6571 7565  ng = MirrorReque
+000021e0: 7374 5365 7474 696e 6728 7061 7373 5f71  stSetting(pass_q
+000021f0: 7565 7279 5f73 7472 696e 673d 4661 6c73  uery_string=Fals
+00002200: 652c 2066 6f6c 6c6f 7733 7878 3d46 616c  e, follow3xx=Fal
+00002210: 7365 2c20 6865 6164 6572 5f73 6574 7469  se, header_setti
+00002220: 6e67 3d68 6561 6465 725f 7365 7474 696e  ng=header_settin
+00002230: 6729 0a20 2061 7379 6e63 5f6d 6972 726f  g).  async_mirro
+00002240: 725f 7275 6c65 203d 2041 7379 6e63 4d69  r_rule = AsyncMi
+00002250: 7272 6f72 5275 6c65 2e72 756c 655f 7769  rrorRule.rule_wi
+00002260: 7468 5f61 636c 286d 6972 726f 725f 7572  th_acl(mirror_ur
+00002270: 6c73 3d5b 2268 7474 703a 2f2f 6162 632e  ls=["http://abc.
+00002280: 6f6d 222c 2022 6874 7470 3a2f 2f77 7777  om", "http://www
+00002290: 2e77 7073 2e63 6e22 5d2c 2073 6176 696e  .wps.cn"], savin
+000022a0: 675f 7365 7474 696e 675f 6163 6c3d 2270  g_setting_acl="p
+000022b0: 7269 7661 7465 2229 0a20 2073 796e 635f  rivate").  sync_
+000022c0: 6d69 7272 6f72 5f72 756c 6573 203d 2053  mirror_rules = S
+000022d0: 796e 634d 6972 726f 7252 756c 6573 2e72  yncMirrorRules.r
+000022e0: 756c 6573 5f77 6974 685f 7072 6566 6978  ules_with_prefix
+000022f0: 5f61 636c 286b 6579 5f70 7265 6669 7865  _acl(key_prefixe
+00002300: 733d 5b22 6162 6322 5d2c 206d 6972 726f  s=["abc"], mirro
+00002310: 725f 7572 6c3d 2268 7474 703a 2f2f 762d  r_url="http://v-
+00002320: 6b73 2d61 2d69 2e6f 7269 6769 6e61 6c76  ks-a-i.originalv
+00002330: 6f64 2e63 6f6d 222c 206d 6972 726f 725f  od.com", mirror_
+00002340: 7265 7175 6573 745f 7365 7474 696e 673d  request_setting=
+00002350: 6d69 7272 6f72 5f72 6571 7565 7374 5f73  mirror_request_s
+00002360: 6574 7469 6e67 2c20 7361 7669 6e67 5f73  etting, saving_s
+00002370: 6574 7469 6e67 5f61 636c 3d22 7072 6976  etting_acl="priv
+00002380: 6174 6522 290a 2020 6d69 7272 6f72 203d  ate").  mirror =
+00002390: 2042 7563 6b65 744d 6972 726f 7228 7573   BucketMirror(us
+000023a0: 655f 6465 6661 756c 745f 726f 626f 7473  e_default_robots
+000023b0: 3d46 616c 7365 2c20 6173 796e 635f 6d69  =False, async_mi
+000023c0: 7272 6f72 5f72 756c 653d 6173 796e 635f  rror_rule=async_
+000023d0: 6d69 7272 6f72 5f72 756c 652c 2073 796e  mirror_rule, syn
+000023e0: 635f 6d69 7272 6f72 5f72 756c 6573 3d5b  c_mirror_rules=[
+000023f0: 7379 6e63 5f6d 6972 726f 725f 7275 6c65  sync_mirror_rule
+00002400: 735d 290a 2020 7072 696e 7428 6275 636b  s]).  print(buck
+00002410: 6574 2e73 6574 5f62 7563 6b65 745f 6d69  et.set_bucket_mi
+00002420: 7272 6f72 286d 6972 726f 7229 290a 0a64  rror(mirror))..d
+00002430: 6566 2064 656c 6574 6542 7563 6b65 744d  ef deleteBucketM
+00002440: 6972 726f 7228 6275 636b 6574 5f6e 616d  irror(bucket_nam
+00002450: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
+00002460: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00002470: 7563 6b65 745f 6e61 6d65 290a 2020 7072  ucket_name).  pr
+00002480: 696e 7428 6275 636b 6574 2e64 656c 6574  int(bucket.delet
+00002490: 655f 6275 636b 6574 5f6d 6972 726f 7228  e_bucket_mirror(
+000024a0: 2929 0a0a 0a64 6566 2073 6574 4275 636b  ))...def setBuck
+000024b0: 6574 5265 7465 6e74 696f 6e28 6275 636b  etRetention(buck
+000024c0: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
+000024d0: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+000024e0: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+000024f0: 290a 2020 6275 636b 6574 5f72 6574 656e  ).  bucket_reten
+00002500: 7469 6f6e 203d 2042 7563 6b65 7452 6574  tion = BucketRet
+00002510: 656e 7469 6f6e 2829 0a20 2023 20e8 aebe  ention().  # ...
+00002520: e7bd aee5 9b9e e694 b6e7 ab99 e8a7 84e5  ................
+00002530: 8899 efbc 9ae5 90af e794 a82f e7a6 81e7  .........../....
+00002540: 94a8 e380 81e6 9687 e4bb b6e4 bf9d e795  ................
+00002550: 99e5 a4a9 e695 b00a 2020 7275 6c65 203d  ........  rule =
+00002560: 2052 6574 656e 7469 6f6e 5275 6c65 2852   RetentionRule(R
+00002570: 6574 656e 7469 6f6e 5275 6c65 2e45 4e41  etentionRule.ENA
+00002580: 424c 4544 2c20 3229 0a20 2023 2072 756c  BLED, 2).  # rul
+00002590: 6520 3d20 5265 7465 6e74 696f 6e52 756c  e = RetentionRul
+000025a0: 6528 5265 7465 6e74 696f 6e52 756c 652e  e(RetentionRule.
+000025b0: 4449 5341 424c 4544 2c20 3229 0a20 2062  DISABLED, 2).  b
+000025c0: 7563 6b65 745f 7265 7465 6e74 696f 6e2e  ucket_retention.
+000025d0: 7275 6c65 203d 2072 756c 650a 2020 6275  rule = rule.  bu
+000025e0: 636b 6574 2e73 6574 5f62 7563 6b65 745f  cket.set_bucket_
+000025f0: 7265 7465 6e74 696f 6e28 6275 636b 6574  retention(bucket
+00002600: 5f72 6574 656e 7469 6f6e 290a 0a0a 6465  _retention)...de
+00002610: 6620 6765 7442 7563 6b65 7452 6574 656e  f getBucketReten
+00002620: 7469 6f6e 2862 7563 6b65 745f 6e61 6d65  tion(bucket_name
+00002630: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
+00002640: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
+00002650: 636b 6574 5f6e 616d 6529 0a20 2072 6574  cket_name).  ret
+00002660: 203d 2062 7563 6b65 742e 6765 745f 6275   = bucket.get_bu
+00002670: 636b 6574 5f72 6574 656e 7469 6f6e 2829  cket_retention()
+00002680: 0a20 2070 7269 6e74 2872 6574 2e74 6f5f  .  print(ret.to_
+00002690: 786d 6c28 2929 0a0a 0a64 6566 206c 6973  xml())...def lis
+000026a0: 7452 6574 656e 7469 6f6e 2862 7563 6b65  tRetention(bucke
+000026b0: 745f 6e61 6d65 293a 0a20 2062 7563 6b65  t_name):.  bucke
+000026c0: 7420 3d20 636f 6e6e 2e67 6574 5f62 7563  t = conn.get_buc
+000026d0: 6b65 7428 6275 636b 6574 5f6e 616d 6529  ket(bucket_name)
+000026e0: 0a20 206b 6579 7320 3d20 6275 636b 6574  .  keys = bucket
+000026f0: 2e6c 6973 745f 7265 7465 6e74 696f 6e28  .list_retention(
+00002700: 290a 2020 666f 7220 6b20 696e 206b 6579  ).  for k in key
+00002710: 733a 0a20 2020 2070 7269 6e74 286b 2e6e  s:.    print(k.n
+00002720: 616d 6529 0a20 2020 2070 7269 6e74 286b  ame).    print(k
+00002730: 2e72 6574 656e 7469 6f6e 5f69 6429 0a20  .retention_id). 
+00002740: 2020 2070 7269 6e74 286b 2e73 746f 7261     print(k.stora
+00002750: 6765 5f63 6c61 7373 290a 0a0a 6465 6620  ge_class)...def 
+00002760: 636c 6561 724f 626a 6563 7428 6275 636b  clearObject(buck
+00002770: 6574 5f6e 616d 6529 3a0a 2020 6275 636b  et_name):.  buck
+00002780: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+00002790: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+000027a0: 290a 2020 6b20 3d20 6275 636b 6574 2e6e  ).  k = bucket.n
+000027b0: 6577 5f6b 6579 2827 636c 6561 725f 6b65  ew_key('clear_ke
+000027c0: 795f 6e61 6d65 2729 0a20 206b 2e63 6c65  y_name').  k.cle
+000027d0: 6172 5f6f 626a 6563 7428 273c 7265 7465  ar_object('<rete
+000027e0: 6e74 696f 6e5f 6964 3e27 290a 0a0a 6465  ntion_id>')...de
+000027f0: 6620 7265 636f 7665 724f 626a 6563 7428  f recoverObject(
+00002800: 6275 636b 6574 5f6e 616d 6529 3a0a 2020  bucket_name):.  
+00002810: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00002820: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00002830: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
+00002840: 6574 2e6e 6577 5f6b 6579 2827 7265 636f  et.new_key('reco
+00002850: 7665 725f 6b65 795f 6e61 6d65 2729 0a20  ver_key_name'). 
+00002860: 2023 20e5 a682 e69e 9c72 6574 656e 7469   # ......retenti
+00002870: 6f6e 5f69 64e4 b8ba e7a9 baef bc8c e9bb  on_id...........
+00002880: 98e8 aea4 e681 a2e5 a48d e59b 9ee6 94b6  ................
+00002890: e7ab 99e4 b8ad e68c 87e5 ae9a 6b65 79e7  ............key.
+000028a0: 9a84 e69c 80e6 96b0 e789 88e6 9cac 0a20  ............... 
+000028b0: 206b 2e72 6563 6f76 6572 5f6f 626a 6563   k.recover_objec
+000028c0: 7428 6f76 6572 7772 6974 653d 5472 7565  t(overwrite=True
+000028d0: 2c20 7265 7465 6e74 696f 6e5f 6964 3d27  , retention_id='
+000028e0: 3c72 6574 656e 7469 6f6e 5f69 643e 2729  <retention_id>')
+000028f0: 0a0a 0a23 2323 2323 2323 2323 2323 2323  ...#############
+00002900: 2323 2323 2323 2323 2020 6b73 332e 6269  ########  ks3.bi
+00002910: 6c6c 696e 6720 2023 2323 2323 2323 2323  lling  #########
+00002920: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002930: 2323 0a66 726f 6d20 6b73 332e 6269 6c6c  ##.from ks3.bill
+00002940: 696e 6720 696d 706f 7274 2067 6574 5f62  ing import get_b
+00002950: 7563 6b65 7473 5f64 6174 610a 0a64 6566  uckets_data..def
+00002960: 2067 6574 4275 636b 6574 7344 6174 6128   getBucketsData(
+00002970: 6275 636b 6574 5f6e 616d 6573 3d4e 6f6e  bucket_names=Non
+00002980: 6529 3a0a 2020 6461 7461 203d 2067 6574  e):.  data = get
+00002990: 5f62 7563 6b65 7473 5f64 6174 6128 616b  _buckets_data(ak
+000029a0: 2c20 736b 2c20 7374 6172 745f 7469 6d65  , sk, start_time
+000029b0: 3d22 3230 3231 3131 3139 3233 3030 222c  ="202111192300",
+000029c0: 2065 6e64 5f74 696d 653d 2232 3032 3131   end_time="20211
+000029d0: 3131 3932 3335 3922 2c20 6275 636b 6574  1192359", bucket
+000029e0: 5f6e 616d 6573 3d62 7563 6b65 745f 6e61  _names=bucket_na
+000029f0: 6d65 732c 2070 726f 6475 6374 733d 2244  mes, products="D
+00002a00: 6174 6153 697a 652c 5265 7175 6573 7473  ataSize,Requests
+00002a10: 4765 7422 290a 2020 7072 696e 7428 6461  Get").  print(da
+00002a20: 7461 290a 0a23 2323 2323 2323 2323 2323  ta)..###########
+00002a30: 2323 2323 2323 2323 2323 2020 6b73 332e  ##########  ks3.
+00002a40: 6f62 6a65 6374 2020 2323 2323 2323 2323  object  ########
+00002a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002a60: 2323 230a 6465 6620 6765 744f 626a 6563  ###.def getObjec
+00002a70: 744d 6574 6128 6275 636b 6574 5f6e 616d  tMeta(bucket_nam
+00002a80: 652c 206f 626a 6563 745f 6b65 795f 6e61  e, object_key_na
+00002a90: 6d65 2c20 6865 6164 6572 733d 4e6f 6e65  me, headers=None
+00002aa0: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
+00002ab0: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
+00002ac0: 636b 6574 5f6e 616d 6529 0a20 2072 6573  cket_name).  res
+00002ad0: 7020 3d20 6275 636b 6574 2e67 6574 5f6b  p = bucket.get_k
+00002ae0: 6579 5f6d 6574 6128 6f62 6a65 6374 5f6b  ey_meta(object_k
+00002af0: 6579 5f6e 616d 652c 2068 6561 6465 7273  ey_name, headers
+00002b00: 3d68 6561 6465 7273 290a 2020 6966 2072  =headers).  if r
+00002b10: 6573 703a 0a20 2020 2070 7269 6e74 2822  esp:.    print("
+00002b20: e88e b7e5 8f96 e696 87e4 bbb6 6865 6164  ............head
+00002b30: 6572 e688 90e5 8a9f 3a20 222c 2072 6573  er......: ", res
+00002b40: 702e 6865 6164 6572 7329 0a0a 6465 6620  p.headers)..def 
+00002b50: 7570 6c6f 6164 4f62 6a65 6374 4672 6f6d  uploadObjectFrom
+00002b60: 4669 6c65 2866 696c 656e 616d 6529 3a0a  File(filename):.
+00002b70: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00002b80: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00002b90: 745f 6e61 6d65 290a 2020 6b20 3d20 6275  t_name).  k = bu
+00002ba0: 636b 6574 2e6e 6577 5f6b 6579 2866 696c  cket.new_key(fil
+00002bb0: 656e 616d 6529 0a20 2072 6574 203d 206b  ename).  ret = k
+00002bc0: 2e73 6574 5f63 6f6e 7465 6e74 735f 6672  .set_contents_fr
+00002bd0: 6f6d 5f66 696c 656e 616d 6528 6f73 2e70  om_filename(os.p
+00002be0: 6174 682e 6578 7061 6e64 7573 6572 2822  ath.expanduser("
+00002bf0: 7e22 2920 2b20 272f 446f 776e 6c6f 6164  ~") + '/Download
+00002c00: 732f 2720 2b20 6669 6c65 6e61 6d65 290a  s/' + filename).
+00002c10: 2020 6966 2072 6574 2061 6e64 2072 6574    if ret and ret
+00002c20: 2e73 7461 7475 7320 3d3d 2032 3030 3a0a  .status == 200:.
+00002c30: 2020 2020 7072 696e 7428 22e4 b88a e4bc      print(".....
+00002c40: a0e6 8890 e58a 9f22 290a 0a64 6566 2075  .......")..def u
+00002c50: 706c 6f61 645f 6173 796e 6328 6669 6c65  pload_async(file
+00002c60: 6e61 6d65 293a 0a20 2062 7563 6b65 7420  name):.  bucket 
+00002c70: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00002c80: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+00002c90: 206b 203d 2062 7563 6b65 742e 6e65 775f   k = bucket.new_
+00002ca0: 6b65 7928 6669 6c65 6e61 6d65 290a 2020  key(filename).  
+00002cb0: 7265 7420 3d20 6173 796e 6369 6f2e 7275  ret = asyncio.ru
+00002cc0: 6e28 6b2e 7570 6c6f 6164 5f66 696c 655f  n(k.upload_file_
+00002cd0: 6173 796e 6328 6f73 2e70 6174 682e 6578  async(os.path.ex
+00002ce0: 7061 6e64 7573 6572 2822 7e22 2920 2b20  panduser("~") + 
+00002cf0: 272f 446f 776e 6c6f 6164 732f 2720 2b20  '/Downloads/' + 
+00002d00: 6669 6c65 6e61 6d65 2929 0a20 2069 6620  filename)).  if 
+00002d10: 7265 7420 616e 6420 7265 742e 7374 6174  ret and ret.stat
+00002d20: 7573 203d 3d20 3230 303a 0a20 2020 2070  us == 200:.    p
+00002d30: 7269 6e74 2822 e4b8 8ae4 bca0 e688 90e5  rint("..........
+00002d40: 8a9f 2229 0a0a 6465 6620 7570 6c6f 6164  ..")..def upload
+00002d50: 4f62 6a65 6374 4672 6f6d 5374 7269 6e67  ObjectFromString
+00002d60: 2829 3a0a 2020 6275 636b 6574 203d 2063  ():.  bucket = c
+00002d70: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00002d80: 7563 6b65 745f 6e61 6d65 290a 2020 6b20  ucket_name).  k 
+00002d90: 3d20 6275 636b 6574 2e6e 6577 5f6b 6579  = bucket.new_key
+00002da0: 2827 e5a4 a7e5 aeb6 e5a5 bd27 290a 2020  ('.........').  
+00002db0: 2320 2320 6b65 7920 e592 8c20 7661 6c75  # # key ... valu
+00002dc0: 6520 e99c 80e8 a681 2075 726c 20e7 bc96  e ...... url ...
+00002dd0: e7a0 810a 2020 2320 7461 6767 696e 6753  ....  # taggingS
+00002de0: 7472 203d 2027 6e61 6d65 3d6a 6827 0a20  tr = 'name=jh'. 
+00002df0: 2023 2068 6561 6465 7273 203d 207b 2778   # headers = {'x
+00002e00: 2d6b 7373 2d74 6167 6769 6e67 273a 2074  -kss-tagging': t
+00002e10: 6167 6769 6e67 5374 727d 0a20 2072 6574  aggingStr}.  ret
+00002e20: 203d 206b 2e73 6574 5f63 6f6e 7465 6e74   = k.set_content
+00002e30: 735f 6672 6f6d 5f73 7472 696e 6728 2720  s_from_string(' 
+00002e40: 776f 726c 6427 290a 2020 2320 2320 e8af  world').  # # ..
+00002e50: b7e6 b182 4944 e380 82e8 afb7 e6b1 8249  ....ID.........I
+00002e60: 44e6 98af e69c ace6 aca1 e8af b7e6 b182  D...............
+00002e70: e79a 84e5 94af e4b8 80e6 a087 e8af 86ef  ................
+00002e80: bc8c e5bc bae7 8388 e5bb bae8 aeae e59c  ................
+00002e90: a8e7 a88b e5ba 8fe6 97a5 e5bf 97e4 b8ad  ................
+00002ea0: e6b7 bbe5 8aa0 e6ad a4e5 8f82 e695 b0e3  ................
+00002eb0: 8082 0a20 2023 2070 7269 6e74 2872 6574  ...  # print(ret
+00002ec0: 2e68 6561 6465 7273 5b27 782d 6b73 732d  .headers['x-kss-
+00002ed0: 7265 7175 6573 742d 6964 275d 290a 2020  request-id']).  
+00002ee0: 2320 2320 4554 6167 e698 af70 7574 5f6f  # # ETag...put_o
+00002ef0: 626a 6563 74e6 96b9 e6b3 95e8 bf94 e59b  bject...........
+00002f00: 9ee5 80bc e789 b9e6 9c89 e79a 84e5 b19e  ................
+00002f10: e680 a7ef bc8c e794 a8e4 ba8e e6a0 87e8  ................
+00002f20: af86 e4b8 80e4 b8aa 4f62 6a65 6374 e79a  ........Object..
+00002f30: 84e5 8685 e5ae b9e3 8082 0a20 2023 2070  ...........  # p
+00002f40: 7269 6e74 2872 6574 2e68 6561 6465 7273  rint(ret.headers
+00002f50: 290a 2020 2320 4854 5450 e8bf 94e5 9b9e  ).  # HTTP......
+00002f60: e7a0 81e3 8082 0a20 2069 6620 7265 7420  .......  if ret 
+00002f70: 616e 6420 7265 742e 7374 6174 7573 203d  and ret.status =
+00002f80: 3d20 3230 303a 0a20 2020 2070 7269 6e74  = 200:.    print
+00002f90: 2822 e4b8 8ae4 bca0 e688 90e5 8a9f 2229  ("............")
+00002fa0: 0a0a 6465 6620 6865 6164 4f62 6a65 6374  ..def headObject
+00002fb0: 2829 3a0a 2020 6275 636b 6574 203d 2063  ():.  bucket = c
+00002fc0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00002fd0: 7563 6b65 745f 6e61 6d65 290a 2020 6b20  ucket_name).  k 
+00002fe0: 3d20 6275 636b 6574 2e67 6574 5f6b 6579  = bucket.get_key
+00002ff0: 2827 7465 7374 5f65 6e63 7279 7074 696f  ('test_encryptio
+00003000: 6e27 290a 2020 6966 206b 3a0a 2020 2020  n').  if k:.    
+00003010: 7072 696e 7428 6b2e 6e61 6d65 2c20 6b2e  print(k.name, k.
+00003020: 7369 7a65 2c20 6b2e 6c61 7374 5f6d 6f64  size, k.last_mod
+00003030: 6966 6965 642c 206b 2e6f 626a 6563 745f  ified, k.object_
+00003040: 7479 7065 2c20 6b2e 7461 6767 696e 675f  type, k.tagging_
+00003050: 636f 756e 7429 0a0a 6465 6620 646f 776e  count)..def down
+00003060: 6c6f 6164 4f62 6a65 6374 416e 6450 7269  loadObjectAndPri
+00003070: 6e74 286b 6579 6e61 6d65 2c20 6279 7465  nt(keyname, byte
+00003080: 5f72 616e 6765 3d28 302c 2031 292c 2068  _range=(0, 1), h
+00003090: 6561 6465 7273 3d4e 6f6e 6529 3a0a 2020  eaders=None):.  
+000030a0: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+000030b0: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+000030c0: 6e61 6d65 290a 2020 6b20 3d20 6275 636b  name).  k = buck
+000030d0: 6574 2e67 6574 5f6b 6579 286b 6579 6e61  et.get_key(keyna
+000030e0: 6d65 290a 2020 7320 3d20 6b2e 6765 745f  me).  s = k.get_
+000030f0: 636f 6e74 656e 7473 5f61 735f 7374 7269  contents_as_stri
+00003100: 6e67 2862 7974 655f 7261 6e67 653d 6279  ng(byte_range=by
+00003110: 7465 5f72 616e 6765 2c20 6865 6164 6572  te_range, header
+00003120: 733d 6865 6164 6572 7329 2e64 6563 6f64  s=headers).decod
+00003130: 6528 290a 2020 7072 696e 7428 7329 0a0a  e().  print(s)..
+00003140: 6465 6620 646f 776e 6c6f 6164 5f61 7379  def download_asy
+00003150: 6e63 286b 6579 6e61 6d65 2c20 6865 6164  nc(keyname, head
+00003160: 6572 733d 4e6f 6e65 293a 0a20 2062 7563  ers=None):.  buc
+00003170: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
+00003180: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
+00003190: 6529 0a20 206b 203d 2062 7563 6b65 742e  e).  k = bucket.
+000031a0: 6765 745f 6b65 7928 6b65 796e 616d 6529  get_key(keyname)
+000031b0: 0a20 2074 7279 3a0a 2020 2020 6173 796e  .  try:.    asyn
+000031c0: 6369 6f2e 7275 6e28 6b2e 646f 776e 6c6f  cio.run(k.downlo
+000031d0: 6164 5f66 696c 655f 6173 796e 6328 6f73  ad_file_async(os
+000031e0: 2e70 6174 682e 6578 7061 6e64 7573 6572  .path.expanduser
+000031f0: 2822 7e22 2920 2b20 272f 446f 776e 6c6f  ("~") + '/Downlo
+00003200: 6164 732f 2720 2b20 6b65 796e 616d 6529  ads/' + keyname)
+00003210: 290a 2020 2020 7072 696e 7428 27e4 b88b  ).    print('...
+00003220: e8bd bde6 8890 e58a 9f27 290a 2020 6578  .........').  ex
+00003230: 6365 7074 3a0a 2020 2020 7072 696e 7428  cept:.    print(
+00003240: 27e4 b88b e8bd bde5 a4b1 e8b4 a527 290a  '............').
+00003250: 0a64 6566 2064 6f77 6e6c 6f61 644f 626a  .def downloadObj
+00003260: 6563 7441 7353 7472 6561 6d41 6e64 5072  ectAsStreamAndPr
+00003270: 696e 7428 293a 0a20 2062 7563 6b65 7420  int():.  bucket 
+00003280: 3d20 636f 6e6e 2e67 6574 5f62 7563 6b65  = conn.get_bucke
+00003290: 7428 6275 636b 6574 5f6e 616d 6529 0a20  t(bucket_name). 
+000032a0: 206b 203d 2062 7563 6b65 742e 6765 745f   k = bucket.get_
+000032b0: 6b65 7928 2773 6861 6b65 2e74 7874 2729  key('shake.txt')
+000032c0: 0a20 2062 7974 6573 203d 206b 2e72 6561  .  bytes = k.rea
+000032d0: 6428 3330 3029 0a20 2070 7269 6e74 2827  d(300).  print('
+000032e0: 7374 6172 743a 2027 2c20 6461 7465 7469  start: ', dateti
+000032f0: 6d65 2e6e 6f77 2829 2e73 7472 6674 696d  me.now().strftim
+00003300: 6528 2225 592d 256d 2d25 6420 2548 3a25  e("%Y-%m-%d %H:%
+00003310: 4d3a 2553 2e25 6622 2929 0a20 2077 6869  M:%S.%f")).  whi
+00003320: 6c65 2062 7974 6573 3a0a 2020 2020 7320  le bytes:.    s 
+00003330: 3d20 6279 7465 732e 6465 636f 6465 2829  = bytes.decode()
+00003340: 0a20 2020 2070 7269 6e74 2827 6279 7465  .    print('byte
+00003350: 7320 6465 636f 6465 643a 272c 2073 290a  s decoded:', s).
+00003360: 2020 2020 7469 6d65 2e73 6c65 6570 2835      time.sleep(5
+00003370: 290a 2020 2020 6279 7465 7320 3d20 6b2e  ).    bytes = k.
+00003380: 7265 6164 2833 3030 290a 2020 7072 696e  read(300).  prin
+00003390: 7428 2765 6e64 3a20 272c 2064 6174 6574  t('end: ', datet
+000033a0: 696d 652e 6e6f 7728 292e 7374 7266 7469  ime.now().strfti
+000033b0: 6d65 2822 2559 2d25 6d2d 2564 2025 483a  me("%Y-%m-%d %H:
+000033c0: 254d 3a25 532e 2566 2229 290a 0a64 6566  %M:%S.%f"))..def
+000033d0: 2064 6f77 6e6c 6f61 644f 626a 6563 7441   downloadObjectA
+000033e0: 6e64 5361 7665 286b 6579 5f6e 616d 652c  ndSave(key_name,
+000033f0: 2062 7974 655f 7261 6e67 653d 2830 2c20   byte_range=(0, 
+00003400: 3129 2c20 6865 6164 6572 733d 4e6f 6e65  1), headers=None
+00003410: 293a 0a20 2062 7563 6b65 7420 3d20 636f  ):.  bucket = co
+00003420: 6e6e 2e67 6574 5f62 7563 6b65 7428 6275  nn.get_bucket(bu
+00003430: 636b 6574 5f6e 616d 6529 0a20 206b 203d  cket_name).  k =
+00003440: 2062 7563 6b65 742e 6765 745f 6b65 7928   bucket.get_key(
+00003450: 6b65 795f 6e61 6d65 290a 2020 6b2e 6765  key_name).  k.ge
+00003460: 745f 636f 6e74 656e 7473 5f74 6f5f 6669  t_contents_to_fi
+00003470: 6c65 6e61 6d65 2827 2f55 7365 7273 2f6a  lename('/Users/j
+00003480: 6162 6261 722f 446f 776e 6c6f 6164 732f  abbar/Downloads/
+00003490: 4453 4330 3333 3830 2e65 6e63 7279 7074  DSC03380.encrypt
+000034a0: 2ee9 9d9e e588 86e5 9d97 2e6a 7067 2e64  ...........jpg.d
+000034b0: 6f77 6e6c 6f61 6427 2c20 6865 6164 6572  ownload', header
+000034c0: 733d 6865 6164 6572 7329 0a0a 6465 6620  s=headers)..def 
+000034d0: 6465 6c65 7465 4f62 6a65 6374 286b 6579  deleteObject(key
+000034e0: 5f6e 616d 6529 3a0a 2020 6275 636b 6574  _name):.  bucket
+000034f0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+00003500: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+00003510: 2020 7472 793a 0a20 2020 2062 7563 6b65    try:.    bucke
+00003520: 742e 6465 6c65 7465 5f6b 6579 286b 6579  t.delete_key(key
+00003530: 5f6e 616d 6529 0a20 2020 2070 7269 6e74  _name).    print
+00003540: 2822 e588 a0e9 99a4 e688 90e5 8a9f 2229  ("............")
+00003550: 0a20 2065 7863 6570 7420 4578 6365 7074  .  except Except
+00003560: 696f 6e20 6173 2065 3a0a 2020 2020 7072  ion as e:.    pr
+00003570: 696e 7428 22e5 88a0 e999 a4e5 a4b1 e8b4  int("...........
+00003580: a522 290a 2020 2020 7072 696e 7428 6529  .").    print(e)
+00003590: 0a20 2020 2070 6173 730a 0a64 6566 2067  .    pass..def g
+000035a0: 6574 4f62 6a65 6374 4163 6c28 293a 0a20  etObjectAcl():. 
+000035b0: 2062 7563 6b65 7420 3d20 636f 6e6e 2e67   bucket = conn.g
+000035c0: 6574 5f62 7563 6b65 7428 6275 636b 6574  et_bucket(bucket
+000035d0: 5f6e 616d 6529 0a20 2070 6f6c 6963 7920  _name).  policy 
+000035e0: 3d20 6275 636b 6574 2e67 6574 5f61 636c  = bucket.get_acl
+000035f0: 2827 6172 7469 636c 652e 7478 7427 290a  ('article.txt').
+00003600: 2020 7072 696e 7428 706f 6c69 6379 2e74    print(policy.t
+00003610: 6f5f 786d 6c28 2929 0a0a 6465 6620 7365  o_xml())..def se
+00003620: 744f 626a 6563 7441 636c 2829 3a0a 2020  tObjectAcl():.  
+00003630: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00003640: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00003650: 6e61 6d65 290a 2020 2320 6f62 6a65 6374  name).  # object
+00003660: 2070 6f6c 6963 7920 3a20 7072 6976 6174   policy : privat
+00003670: 6520 7c20 7075 626c 6963 2d72 6561 6420  e | public-read 
+00003680: 7c20 7075 626c 6963 2d72 6561 642d 7772  | public-read-wr
+00003690: 6974 650a 2020 6275 636b 6574 2e73 6574  ite.  bucket.set
+000036a0: 5f61 636c 2822 7075 626c 6963 2d72 6561  _acl("public-rea
+000036b0: 6422 2c20 273c 594f 5552 5f4b 4559 5f4e  d", '<YOUR_KEY_N
+000036c0: 414d 453e 2729 0a0a 6465 6620 7365 744f  AME>')..def setO
+000036d0: 626a 6563 744d 6574 6128 293a 0a20 2062  bjectMeta():.  b
+000036e0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+000036f0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+00003700: 2020 622e 636f 7079 5f6b 6579 2827 3c79    b.copy_key('<y
+00003710: 6f75 724b 6579 4e61 6d65 3e27 2c20 273c  ourKeyName>', '<
+00003720: 796f 7572 4275 636b 6574 4e61 6d65 3e27  yourBucketName>'
+00003730: 2c20 273c 796f 7572 4b65 794e 616d 653e  , '<yourKeyName>
+00003740: 272c 0a20 2020 2020 2020 2020 2020 2020  ',.             
+00003750: 6865 6164 6572 733d 7b27 636f 6e74 656e  headers={'conten
+00003760: 742d 7479 7065 273a 2027 7465 7874 2f70  t-type': 'text/p
+00003770: 6c61 696e 272c 2027 782d 6b73 732d 6d65  lain', 'x-kss-me
+00003780: 7461 6461 7461 2d64 6972 6563 7469 7665  tadata-directive
+00003790: 273a 2027 5245 504c 4143 4527 7d29 0a0a  ': 'REPLACE'})..
+000037a0: 6465 6620 7365 744f 626a 6563 7453 746f  def setObjectSto
+000037b0: 7261 6765 436c 6173 7328 293a 0a20 2062  rageClass():.  b
+000037c0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+000037d0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+000037e0: 2020 622e 636f 7079 5f6b 6579 2827 3c79    b.copy_key('<y
+000037f0: 6f75 724b 6579 4e61 6d65 3e27 2c20 273c  ourKeyName>', '<
+00003800: 796f 7572 4275 636b 6574 4e61 6d65 3e27  yourBucketName>'
+00003810: 2c20 273c 796f 7572 4b65 794e 616d 653e  , '<yourKeyName>
+00003820: 272c 2068 6561 6465 7273 3d7b 2778 2d6b  ', headers={'x-k
+00003830: 7373 2d73 746f 7261 6765 2d63 6c61 7373  ss-storage-class
+00003840: 273a 2027 5354 414e 4441 5244 5f49 4127  ': 'STANDARD_IA'
+00003850: 7d29 0a0a 6465 6620 636f 7079 2864 7374  })..def copy(dst
+00003860: 4b65 792c 2073 7263 4b65 792c 2064 7374  Key, srcKey, dst
+00003870: 5f62 7563 6b65 745f 6e61 6d65 3d4e 6f6e  _bucket_name=Non
+00003880: 652c 2068 6561 6465 7273 3d4e 6f6e 6529  e, headers=None)
+00003890: 3a0a 2020 2320 6275 636b 6574 5f6e 616d  :.  # bucket_nam
+000038a0: 6520 3d20 2768 6170 7079 686f 7572 270a  e = 'happyhour'.
+000038b0: 2020 6220 3d20 636f 6e6e 2e67 6574 5f62    b = conn.get_b
+000038c0: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
+000038d0: 6529 0a20 2072 6574 7572 6e20 622e 636f  e).  return b.co
+000038e0: 7079 5f6b 6579 2864 7374 4b65 792c 2064  py_key(dstKey, d
+000038f0: 7374 5f62 7563 6b65 745f 6e61 6d65 2c20  st_bucket_name, 
+00003900: 7372 634b 6579 2c20 6865 6164 6572 733d  srcKey, headers=
+00003910: 6865 6164 6572 7329 0a0a 6465 6620 636f  headers)..def co
+00003920: 7079 5f65 6e63 7279 7074 696f 6e28 6473  py_encryption(ds
+00003930: 744b 6579 2c20 7372 634b 6579 2c20 656e  tKey, srcKey, en
+00003940: 6372 7970 745f 6b65 793d 4e6f 6e65 293a  crypt_key=None):
+00003950: 0a20 2062 203d 2063 6f6e 6e2e 6765 745f  .  b = conn.get_
+00003960: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
+00003970: 6d65 290a 2020 622e 636f 7079 5f6b 6579  me).  b.copy_key
+00003980: 2864 7374 4b65 792c 2062 7563 6b65 745f  (dstKey, bucket_
+00003990: 6e61 6d65 2c20 7372 634b 6579 2c20 656e  name, srcKey, en
+000039a0: 6372 7970 745f 6b65 793d 656e 6372 7970  crypt_key=encryp
+000039b0: 745f 6b65 7929 0a0a 6465 6620 6c69 7374  t_key)..def list
+000039c0: 5f6f 626a 6563 7473 2829 3a0a 2020 6275  _objects():.  bu
+000039d0: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
+000039e0: 6275 636b 6574 2827 7465 7374 2d62 7563  bucket('test-buc
+000039f0: 6b65 7427 290a 2020 6b65 7973 203d 2062  ket').  keys = b
+00003a00: 7563 6b65 742e 6c69 7374 2870 7265 6669  ucket.list(prefi
+00003a10: 783d 2731 3627 290a 2020 7265 7331 203d  x='16').  res1 =
+00003a20: 205b 6b2e 6e61 6d65 2066 6f72 206b 2069   [k.name for k i
+00003a30: 6e20 6b65 7973 5d0a 2020 7072 696e 7428  n keys].  print(
+00003a40: 2772 6573 3120 3a20 272c 2072 6573 3129  'res1 : ', res1)
+00003a50: 0a0a 2020 6b65 7973 3220 3d20 6275 636b  ..  keys2 = buck
+00003a60: 6574 2e6c 6973 744f 626a 6563 7473 2870  et.listObjects(p
+00003a70: 7265 6669 783d 2731 3627 290a 2020 2320  refix='16').  # 
+00003a80: 7265 7332 203d 205b 6b2e 6e61 6d65 2066  res2 = [k.name f
+00003a90: 6f72 206b 2069 6e20 6b65 7973 325d 0a20  or k in keys2]. 
+00003aa0: 2070 7269 6e74 2827 6b65 7973 3220 3a20   print('keys2 : 
+00003ab0: 272c 206b 6579 7332 290a 2020 2320 666f  ', keys2).  # fo
+00003ac0: 7220 6b20 696e 206b 6579 733a 0a20 2023  r k in keys:.  #
+00003ad0: 2020 2070 7269 6e74 2827 6f62 6a65 6374     print('object
+00003ae0: 3a27 2c20 6b2e 6e61 6d65 290a 0a64 6566  :', k.name)..def
+00003af0: 206c 6973 745f 6f62 6a65 6374 735f 7632   list_objects_v2
+00003b00: 2864 656c 696d 6974 6572 3d27 2327 2c20  (delimiter='#', 
+00003b10: 7072 6566 6978 3d4e 6f6e 652c 206d 6178  prefix=None, max
+00003b20: 5f6b 6579 733d 4e6f 6e65 2c20 6d61 726b  _keys=None, mark
+00003b30: 6572 3d4e 6f6e 652c 2065 6e63 6f64 696e  er=None, encodin
+00003b40: 675f 7479 7065 3d27 272c 2066 6574 6368  g_type='', fetch
+00003b50: 5f6f 776e 6572 3d54 7275 6529 3a0a 2020  _owner=True):.  
+00003b60: 6275 636b 6574 203d 2063 6f6e 6e2e 6765  bucket = conn.ge
+00003b70: 745f 6275 636b 6574 2862 7563 6b65 745f  t_bucket(bucket_
+00003b80: 6e61 6d65 290a 2020 6b65 7973 203d 2062  name).  keys = b
+00003b90: 7563 6b65 742e 6c69 7374 5f76 3228 6465  ucket.list_v2(de
+00003ba0: 6c69 6d69 7465 723d 6465 6c69 6d69 7465  limiter=delimite
+00003bb0: 722c 2070 7265 6669 783d 7072 6566 6978  r, prefix=prefix
+00003bc0: 2c20 6d61 785f 6b65 7973 3d6d 6178 5f6b  , max_keys=max_k
+00003bd0: 6579 732c 206d 6172 6b65 723d 6d61 726b  eys, marker=mark
+00003be0: 6572 2c20 656e 636f 6469 6e67 5f74 7970  er, encoding_typ
+00003bf0: 653d 656e 636f 6469 6e67 5f74 7970 652c  e=encoding_type,
+00003c00: 2066 6574 6368 5f6f 776e 6572 3d66 6574   fetch_owner=fet
+00003c10: 6368 5f6f 776e 6572 290a 2020 666f 7220  ch_owner).  for 
+00003c20: 6b20 696e 206b 6579 733a 0a20 2020 2070  k in keys:.    p
+00003c30: 7269 6e74 2827 6f62 6a65 6374 3a27 2c20  rint('object:', 
+00003c40: 6b2e 6e61 6d65 290a 0a64 6566 206c 6973  k.name)..def lis
+00003c50: 744f 626a 6563 7473 4d6f 7265 2862 7563  tObjectsMore(buc
+00003c60: 6b65 745f 6e61 6d65 2c20 6465 6c69 6d69  ket_name, delimi
+00003c70: 7465 723d 4e6f 6e65 2c20 7072 6566 6978  ter=None, prefix
+00003c80: 3d4e 6f6e 652c 206d 6178 5f6b 6579 733d  =None, max_keys=
+00003c90: 4e6f 6e65 2c20 6d61 726b 6572 3d4e 6f6e  None, marker=Non
+00003ca0: 6529 3a0a 2020 6275 636b 6574 203d 2063  e):.  bucket = c
+00003cb0: 6f6e 6e2e 6765 745f 6275 636b 6574 2862  onn.get_bucket(b
+00003cc0: 7563 6b65 745f 6e61 6d65 290a 2020 6b65  ucket_name).  ke
+00003cd0: 7973 203d 2062 7563 6b65 742e 6c69 7374  ys = bucket.list
+00003ce0: 2864 656c 696d 6974 6572 3d64 656c 696d  (delimiter=delim
+00003cf0: 6974 6572 2c20 7072 6566 6978 3d70 7265  iter, prefix=pre
+00003d00: 6669 782c 206d 6178 5f6b 6579 733d 6d61  fix, max_keys=ma
+00003d10: 785f 6b65 7973 2c20 6d61 726b 6572 3d6d  x_keys, marker=m
+00003d20: 6172 6b65 7229 0a20 2023 2070 7269 6e74  arker).  # print
+00003d30: 286c 656e 286b 6579 7329 290a 2020 7265  (len(keys)).  re
+00003d40: 7320 3d20 5b6b 2e6e 616d 6520 666f 7220  s = [k.name for 
+00003d50: 6b20 696e 206b 6579 735d 0a20 2070 7269  k in keys].  pri
+00003d60: 6e74 2827 7265 733a 2027 2c20 7265 7329  nt('res: ', res)
+00003d70: 0a20 2023 2070 7269 6e74 2827 6974 656d  .  # print('item
+00003d80: 3a27 2c20 6b2e 6e61 6d65 2c20 7479 7065  :', k.name, type
+00003d90: 286b 2929 0a0a 6465 6620 6c69 7374 416e  (k))..def listAn
+00003da0: 6444 656c 6574 6528 293a 0a20 2062 7563  dDelete():.  buc
+00003db0: 6b65 7420 3d20 636f 6e6e 2e67 6574 5f62  ket = conn.get_b
+00003dc0: 7563 6b65 7428 6275 636b 6574 5f6e 616d  ucket(bucket_nam
+00003dd0: 6529 0a20 206b 6579 7320 3d20 6275 636b  e).  keys = buck
+00003de0: 6574 2e6c 6973 7428 6465 6c69 6d69 7465  et.list(delimite
+00003df0: 723d 272f 272c 206d 6178 5f6b 6579 733d  r='/', max_keys=
+00003e00: 3130 2c20 7072 6566 6978 3d27 3135 2729  10, prefix='15')
+00003e10: 0a20 2070 7269 6e74 286b 6579 732e 6d61  .  print(keys.ma
+00003e20: 726b 6572 290a 2020 666f 7220 6b20 696e  rker).  for k in
+00003e30: 206b 6579 733a 0a20 2020 2070 7269 6e74   keys:.    print
+00003e40: 2827 6f62 6a65 6374 3a27 2c20 6b2e 6e61  ('object:', k.na
+00003e50: 6d65 290a 2020 2020 6465 6c65 7465 4f62  me).    deleteOb
+00003e60: 6a65 6374 286b 2e6e 616d 6529 0a0a 6465  ject(k.name)..de
+00003e70: 6620 6c69 7374 4f62 6a65 6374 7341 6e64  f listObjectsAnd
+00003e80: 4669 6c74 6572 2865 6e64 5469 6d65 3d4e  Filter(endTime=N
+00003e90: 6f6e 6529 3a0a 2020 6275 636b 6574 203d  one):.  bucket =
+00003ea0: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+00003eb0: 2827 6175 746f 2d74 6573 742d 6275 636b  ('auto-test-buck
+00003ec0: 6574 2729 0a20 206b 6579 7320 3d20 6275  et').  keys = bu
+00003ed0: 636b 6574 2e6c 6973 744f 626a 6563 7473  cket.listObjects
+00003ee0: 2864 656c 696d 6974 6572 3d27 2f27 2c20  (delimiter='/', 
+00003ef0: 6d61 785f 6b65 7973 3d32 2920 2320 7374  max_keys=2) # st
+00003f00: 6172 745f 7469 6d65 3d31 3634 3033 3331  art_time=1640331
+00003f10: 3434 362c 2065 6e64 5f74 696d 653d 3136  446, end_time=16
+00003f20: 3431 3839 3530 3936 0a20 2066 6f72 206b  41895096.  for k
+00003f30: 2069 6e20 6b65 7973 3a0a 2020 2020 7072   in keys:.    pr
+00003f40: 696e 7428 6b29 0a0a 6465 6620 6765 744f  int(k)..def getO
+00003f50: 626a 6563 7454 6167 6769 6e67 2829 3a0a  bjectTagging():.
+00003f60: 2020 6275 636b 6574 203d 2063 6f6e 6e2e    bucket = conn.
+00003f70: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+00003f80: 745f 6e61 6d65 290a 2020 6b65 7920 3d20  t_name).  key = 
+00003f90: 6275 636b 6574 2e67 6574 5f6b 6579 2827  bucket.get_key('
+00003fa0: 7465 7374 5461 6767 696e 6727 290a 2020  testTagging').  
+00003fb0: 7461 6767 696e 6720 3d20 6b65 792e 6765  tagging = key.ge
+00003fc0: 745f 6f62 6a65 6374 5f74 6167 6769 6e67  t_object_tagging
+00003fd0: 2829 0a20 2070 7269 6e74 2874 6167 6769  ().  print(taggi
+00003fe0: 6e67 2e74 6f5f 786d 6c28 2929 0a0a 6465  ng.to_xml())..de
+00003ff0: 6620 7365 744f 626a 6563 7454 6167 6769  f setObjectTaggi
+00004000: 6e67 2829 3a0a 2020 6275 636b 6574 203d  ng():.  bucket =
+00004010: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+00004020: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+00004030: 6b65 7920 3d20 6275 636b 6574 2e67 6574  key = bucket.get
+00004040: 5f6b 6579 2827 7465 7374 5461 6767 696e  _key('testTaggin
+00004050: 6727 290a 2020 7461 6767 696e 6720 3d20  g').  tagging = 
+00004060: 5b54 6167 2827 3027 292c 2054 6167 2827  [Tag('0'), Tag('
+00004070: 3127 2c20 2731 2729 5d0a 2020 6b65 792e  1', '1')].  key.
+00004080: 7365 745f 6f62 6a65 6374 5f74 6167 6769  set_object_taggi
+00004090: 6e67 2874 6167 6769 6e67 290a 0a64 6566  ng(tagging)..def
+000040a0: 2064 656c 6574 654f 626a 6563 7454 6167   deleteObjectTag
+000040b0: 6769 6e67 2829 3a0a 2020 6275 636b 6574  ging():.  bucket
+000040c0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+000040d0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+000040e0: 2020 6b65 7920 3d20 6275 636b 6574 2e67    key = bucket.g
+000040f0: 6574 5f6b 6579 2827 6865 6865 2729 0a20  et_key('hehe'). 
+00004100: 206b 6579 2e64 656c 6574 655f 6f62 6a65   key.delete_obje
+00004110: 6374 5f74 6167 6769 6e67 2829 0a0a 6465  ct_tagging()..de
+00004120: 6620 6361 6c63 466f 6c64 6572 5369 7a65  f calcFolderSize
+00004130: 2862 7563 6b65 742c 2066 6f6c 6465 7229  (bucket, folder)
+00004140: 3a0a 2020 6c65 6e67 7468 203d 2030 0a20  :.  length = 0. 
+00004150: 206b 6579 7320 3d20 6275 636b 6574 2e6c   keys = bucket.l
+00004160: 6973 7428 7072 6566 6978 3d66 6f6c 6465  ist(prefix=folde
+00004170: 7229 0a20 2066 6f72 206b 2069 6e20 6b65  r).  for k in ke
+00004180: 7973 3a0a 2020 2020 6966 2069 7369 6e73  ys:.    if isins
+00004190: 7461 6e63 6528 6b2c 204b 6579 293a 0a20  tance(k, Key):. 
+000041a0: 2020 2020 206c 656e 6774 6820 2b3d 206b       length += k
+000041b0: 2e73 697a 650a 2020 7265 7475 726e 206c  .size.  return l
+000041c0: 656e 6774 680a 0a66 726f 6d20 6b73 332e  ength..from ks3.
+000041d0: 7072 6566 6978 2069 6d70 6f72 7420 5072  prefix import Pr
+000041e0: 6566 6978 0a0a 2320 e588 97e4 b8be e68c  efix..# ........
+000041f0: 87e5 ae9a e79b aee5 bd95 e4b8 8be7 9a84  ................
+00004200: e696 87e4 bbb6 e5a4 a7e5 b08f 0a64 6566  .............def
+00004210: 2067 6574 466f 6c64 6572 5369 7a65 496e   getFolderSizeIn
+00004220: 4275 636b 6574 2829 3a0a 2020 6275 636b  Bucket():.  buck
+00004230: 6574 203d 2063 6f6e 6e2e 6765 745f 6275  et = conn.get_bu
+00004240: 636b 6574 2862 7563 6b65 745f 6e61 6d65  cket(bucket_name
+00004250: 290a 2020 6b65 7973 203d 2062 7563 6b65  ).  keys = bucke
+00004260: 742e 6c69 7374 2864 656c 696d 6974 6572  t.list(delimiter
+00004270: 3d27 2f27 290a 2020 666f 7220 6b20 696e  ='/').  for k in
+00004280: 206b 6579 733a 0a20 2020 2069 6620 6973   keys:.    if is
+00004290: 696e 7374 616e 6365 286b 2c20 5072 6566  instance(k, Pref
+000042a0: 6978 293a 0a20 2020 2020 2070 7269 6e74  ix):.      print
+000042b0: 2827 6469 723a 2027 202b 206b 2e6e 616d  ('dir: ' + k.nam
+000042c0: 6520 2b20 2720 2073 697a 653a 2720 2b20  e + '  size:' + 
+000042d0: 7374 7228 6361 6c63 466f 6c64 6572 5369  str(calcFolderSi
+000042e0: 7a65 2862 7563 6b65 742c 206b 2e6e 616d  ze(bucket, k.nam
+000042f0: 6529 2920 2b20 2242 7974 6522 290a 0a0a  e)) + "Byte")...
+00004300: 6465 6620 7465 7374 5f6d 756c 7469 7061  def test_multipa
+00004310: 7274 5f75 706c 6f61 6428 656e 6372 7970  rt_upload(encryp
+00004320: 745f 6b65 793d 4e6f 6e65 293a 0a20 2069  t_key=None):.  i
+00004330: 6d70 6f72 7420 6d61 7468 2c20 6f73 0a20  mport math, os. 
+00004340: 2066 726f 6d20 6669 6c65 6368 756e 6b69   from filechunki
+00004350: 6f20 696d 706f 7274 2046 696c 6543 6875  o import FileChu
+00004360: 6e6b 494f 0a20 2062 7563 6b65 7420 3d20  nkIO.  bucket = 
+00004370: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
+00004380: 6275 636b 6574 5f6e 616d 6529 0a0a 2020  bucket_name)..  
+00004390: 736f 7572 6365 5f70 6174 6820 3d20 272f  source_path = '/
+000043a0: 5573 6572 732f 6a61 6262 6172 2f44 6f77  Users/jabbar/Dow
+000043b0: 6e6c 6f61 6473 2f44 5343 3033 3338 302e  nloads/DSC03380.
+000043c0: 4a50 4727 0a20 2023 20e6 ba90 e696 87e4  JPG'.  # .......
+000043d0: bbb6 e5a4 a7e5 b08f 0a20 2073 6f75 7263  .........  sourc
+000043e0: 655f 7369 7a65 203d 206f 732e 7374 6174  e_size = os.stat
+000043f0: 2873 6f75 7263 655f 7061 7468 292e 7374  (source_path).st
+00004400: 5f73 697a 650a 0a20 206d 7020 3d20 6275  _size..  mp = bu
+00004410: 636b 6574 2e69 6e69 7469 6174 655f 6d75  cket.initiate_mu
+00004420: 6c74 6970 6172 745f 7570 6c6f 6164 2822  ltipart_upload("
+00004430: 4453 4330 3333 3830 2e6d 702e 6a70 6722  DSC03380.mp.jpg"
+00004440: 2c20 656e 6372 7970 745f 6b65 793d 656e  , encrypt_key=en
+00004450: 6372 7970 745f 6b65 7929 0a20 2070 7269  crypt_key).  pri
+00004460: 6e74 286d 7029 0a0a 2020 6368 756e 6b5f  nt(mp)..  chunk_
+00004470: 7369 7a65 203d 2035 3234 3238 3830 0a20  size = 5242880. 
+00004480: 2063 6875 6e6b 5f63 6f75 6e74 203d 2069   chunk_count = i
+00004490: 6e74 286d 6174 682e 6365 696c 2873 6f75  nt(math.ceil(sou
+000044a0: 7263 655f 7369 7a65 202a 2031 2e30 202f  rce_size * 1.0 /
+000044b0: 2063 6875 6e6b 5f73 697a 6520 2a20 312e   chunk_size * 1.
+000044c0: 3029 290a 0a20 2023 20e9 809a e8bf 8720  0))..  # ...... 
+000044d0: 4669 6c65 4368 756e 6b49 4f20 e5b0 86e6  FileChunkIO ....
+000044e0: 9687 e4bb b6e5 8886 e789 870a 2020 666f  ............  fo
+000044f0: 7220 6920 696e 2072 616e 6765 2863 6875  r i in range(chu
+00004500: 6e6b 5f63 6f75 6e74 293a 0a20 2020 206f  nk_count):.    o
+00004510: 6666 7365 7420 3d20 6368 756e 6b5f 7369  ffset = chunk_si
+00004520: 7a65 202a 2069 0a20 2020 2062 7974 6573  ze * i.    bytes
+00004530: 203d 206d 696e 2863 6875 6e6b 5f73 697a   = min(chunk_siz
+00004540: 652c 2073 6f75 7263 655f 7369 7a65 202d  e, source_size -
+00004550: 206f 6666 7365 7429 0a20 2020 2077 6974   offset).    wit
+00004560: 6820 4669 6c65 4368 756e 6b49 4f28 736f  h FileChunkIO(so
+00004570: 7572 6365 5f70 6174 682c 2027 7227 2c20  urce_path, 'r', 
+00004580: 6f66 6673 6574 3d6f 6666 7365 742c 2062  offset=offset, b
+00004590: 7974 6573 3d62 7974 6573 2920 6173 2066  ytes=bytes) as f
+000045a0: 703a 0a20 2020 2020 2023 20e9 8090 e4b8  p:.      # .....
+000045b0: aae4 b88a e4bc a0e5 8886 e789 870a 2020  ..............  
+000045c0: 2020 2020 6d70 2e75 706c 6f61 645f 7061      mp.upload_pa
+000045d0: 7274 5f66 726f 6d5f 6669 6c65 2866 702c  rt_from_file(fp,
+000045e0: 2070 6172 745f 6e75 6d3d 6920 2b20 3129   part_num=i + 1)
+000045f0: 0a20 2070 7269 6e74 286d 702e 746f 5f78  .  print(mp.to_x
+00004600: 6d6c 2829 290a 2020 2320 e58f 91e9 8081  ml()).  # ......
+00004610: e8af b7e6 b182 efbc 8ce5 9088 e5b9 b6e5  ................
+00004620: 8886 e789 87ef bc8c e5ae 8ce6 8890 e588  ................
+00004630: 86e7 8987 e4b8 8ae4 bca0 0a20 2072 6574  ...........  ret
+00004640: 203d 206d 702e 636f 6d70 6c65 7465 5f75   = mp.complete_u
+00004650: 706c 6f61 6428 290a 2020 6966 2072 6574  pload().  if ret
+00004660: 2061 6e64 2072 6574 2e73 7461 7475 7320   and ret.status 
+00004670: 3d3d 2032 3030 3a0a 2020 2020 7072 696e  == 200:.    prin
+00004680: 7428 22e4 b88a e4bc a0e6 8890 e58a 9f22  t("............"
+00004690: 290a 0a64 6566 2074 6573 745f 6665 7463  )..def test_fetc
+000046a0: 685f 6f62 6a65 6374 2829 3a0a 2020 6275  h_object():.  bu
+000046b0: 636b 6574 203d 2063 6f6e 6e2e 6765 745f  cket = conn.get_
+000046c0: 6275 636b 6574 2862 7563 6b65 745f 6e61  bucket(bucket_na
+000046d0: 6d65 290a 2020 6b65 7920 3d20 6275 636b  me).  key = buck
+000046e0: 6574 2e6e 6577 5f6b 6579 2827 7777 772d  et.new_key('www-
+000046f0: 6c6f 676f 2729 0a20 206b 6579 2e66 6574  logo').  key.fet
+00004700: 6368 5f6f 626a 6563 7428 736f 7572 6365  ch_object(source
+00004710: 5f75 726c 3d27 6874 7470 3a2f 2f66 652e  _url='http://fe.
+00004720: 6b73 7975 6e2e 636f 6d2f 7072 6f6a 6563  ksyun.com/projec
+00004730: 742f 7265 736f 7572 6365 2f69 6d67 2f77  t/resource/img/w
+00004740: 7777 2d6c 6f67 6f2e 706e 6727 2c0a 2020  ww-logo.png',.  
+00004750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004760: 2020 2020 6865 6164 6572 733d 7b27 782d      headers={'x-
+00004770: 6b73 732d 6163 6c27 3a20 2770 7562 6c69  kss-acl': 'publi
+00004780: 632d 7265 6164 277d 290a 2020 7072 696e  c-read'}).  prin
+00004790: 7428 2766 6574 6368 e688 90e5 8a9f 2729  t('fetch......')
+000047a0: 0a0a 6465 6620 7465 7374 5f67 656e 6572  ..def test_gener
+000047b0: 6174 655f 7572 6c28 6b65 795f 6e61 6d65  ate_url(key_name
+000047c0: 2c20 696d 6167 655f 6174 7472 733d 4e6f  , image_attrs=No
+000047d0: 6e65 293a 0a20 2062 203d 2063 6f6e 6e2e  ne):.  b = conn.
+000047e0: 6765 745f 6275 636b 6574 2862 7563 6b65  get_bucket(bucke
+000047f0: 745f 6e61 6d65 290a 2020 6b20 3d20 622e  t_name).  k = b.
+00004800: 6765 745f 6b65 7928 6b65 795f 6e61 6d65  get_key(key_name
+00004810: 290a 2020 6966 206b 3a0a 2020 2020 7572  ).  if k:.    ur
+00004820: 6c20 3d20 6b2e 6765 6e65 7261 7465 5f75  l = k.generate_u
+00004830: 726c 2836 3030 2c20 696d 6167 655f 6174  rl(600, image_at
+00004840: 7472 733d 696d 6167 655f 6174 7472 7329  trs=image_attrs)
+00004850: 2020 2320 3630 7320 e590 8ee8 afa5 e993    # 60s ........
+00004860: bee6 8ea5 e8bf 87e6 9c9f 0a20 2020 2070  ...........    p
+00004870: 7269 6e74 2875 726c 290a 2020 656c 7365  rint(url).  else
+00004880: 3a0a 2020 2020 7072 696e 7428 276f 626a  :.    print('obj
+00004890: 6563 7420 6e6f 7420 666f 756e 6427 290a  ect not found').
+000048a0: 0a64 6566 2074 6573 745f 6765 745f 7072  .def test_get_pr
+000048b0: 6573 6967 6e65 645f 7572 6c28 6b65 795f  esigned_url(key_
+000048c0: 6e61 6d65 293a 0a20 2062 203d 2063 6f6e  name):.  b = con
+000048d0: 6e2e 6765 745f 6275 636b 6574 2862 7563  n.get_bucket(buc
+000048e0: 6b65 745f 6e61 6d65 290a 2020 2320 e696  ket_name).  # ..
+000048f0: b0e5 bbba e5af b9e8 b1a1 6b65 790a 2020  ..........key.  
+00004900: 6b20 3d20 622e 6e65 775f 6b65 7928 6b65  k = b.new_key(ke
+00004910: 795f 6e61 6d65 290a 2020 6966 206b 3a0a  y_name).  if k:.
+00004920: 2020 2020 7572 6c20 3d20 6b2e 6765 745f      url = k.get_
+00004930: 7072 6573 6967 6e65 645f 7572 6c28 3630  presigned_url(60
+00004940: 3030 3029 2020 2320 3630 7320 e590 8ee8  000)  # 60s ....
+00004950: afa5 e993 bee6 8ea5 e8bf 87e6 9c9f 0a20  ............... 
+00004960: 2020 2070 7269 6e74 2875 726c 290a 2020     print(url).  
+00004970: 2020 7265 7475 726e 2075 726c 0a0a 6465    return url..de
+00004980: 6620 7265 7374 6f72 654f 626a 6563 7428  f restoreObject(
+00004990: 6b65 795f 6e61 6d65 293a 0a20 2062 203d  key_name):.  b =
+000049a0: 2063 6f6e 6e2e 6765 745f 6275 636b 6574   conn.get_bucket
+000049b0: 2862 7563 6b65 745f 6e61 6d65 290a 2020  (bucket_name).  
+000049c0: 6b20 3d20 622e 6765 745f 6b65 7928 6b65  k = b.get_key(ke
+000049d0: 795f 6e61 6d65 290a 2020 6b2e 7265 7374  y_name).  k.rest
+000049e0: 6f72 655f 6f62 6a65 6374 2829 0a0a 6465  ore_object()..de
+000049f0: 6620 7465 7374 5f70 7574 5f76 6961 5f70  f test_put_via_p
+00004a00: 7265 7369 676e 6564 5f75 726c 286b 6579  resigned_url(key
+00004a10: 293a 0a20 2075 726c 203d 2074 6573 745f  ):.  url = test_
+00004a20: 6765 745f 7072 6573 6967 6e65 645f 7572  get_presigned_ur
+00004a30: 6c28 6b65 7929 0a20 2077 6974 6820 6f70  l(key).  with op
+00004a40: 656e 2827 2e2f 6172 7469 636c 652e 7478  en('./article.tx
+00004a50: 7427 2c20 2772 6227 2920 6173 2066 703a  t', 'rb') as fp:
+00004a60: 0a20 2020 2072 6573 756c 7420 3d20 7265  .    result = re
+00004a70: 7175 6573 7473 2e70 7574 2875 726c 2c20  quests.put(url, 
+00004a80: 6461 7461 3d66 7029 0a20 2020 2070 7269  data=fp).    pri
+00004a90: 6e74 2872 6573 756c 7429 0a0a 6672 6f6d  nt(result)..from
+00004aa0: 206b 7333 2e73 7473 2069 6d70 6f72 7420   ks3.sts import 
+00004ab0: 6173 7375 6d65 526f 6c65 0a64 6566 2074  assumeRole.def t
+00004ac0: 6573 745f 6173 7375 6d65 526f 6c65 2829  est_assumeRole()
+00004ad0: 3a0a 2020 7072 696e 7428 6173 7375 6d65  :.  print(assume
+00004ae0: 526f 6c65 2861 6b2c 2073 6b2c 2022 6b72  Role(ak, sk, "kr
+00004af0: 6e3a 6b73 633a 6961 6d3a 3a78 7878 3a72  n:ksc:iam::xxx:r
+00004b00: 6f6c 652f 7878 2d74 6573 742d 6275 636b  ole/xx-test-buck
+00004b10: 6574 222c 2022 6b73 3322 2c20 3336 3030  et", "ks3", 3600
+00004b20: 2929 0a0a 0a64 6566 2070 7574 5f6f 626a  ))...def put_obj
+00004b30: 6563 745f 6361 6c6c 6261 636b 286b 6579  ect_callback(key
+00004b40: 5f6e 616d 6529 3a0a 2020 6220 3d20 636f  _name):.  b = co
+00004b50: 6e6e 2e67 6574 5f62 7563 6b65 7428 2768  nn.get_bucket('h
+00004b60: 616e 6a69 6e67 2d74 6573 7430 3030 2729  anjing-test000')
+00004b70: 0a20 2023 20e6 96b0 e5bb bae5 afb9 e8b1  .  # ...........
+00004b80: a16b 6579 0a20 206b 203d 2062 2e6e 6577  .key.  k = b.new
+00004b90: 5f6b 6579 286b 6579 5f6e 616d 6529 0a20  _key(key_name). 
+00004ba0: 2023 20e4 b88a e4bc a0e6 8890 e58a 9fe5   # .............
+00004bb0: 908e efbc 8ce5 9091 e59b 9ee8 b083 e59c  ................
+00004bc0: b0e5 9d80 504f 5354 e695 b0e6 8dae 0a20  ....POST....... 
+00004bd0: 2023 20e9 9c80 e8a6 81e8 aebe e7bd ae60   # ............`
+00004be0: 782d 6b73 732d 6361 6c6c 6261 636b 7572  x-kss-callbackur
+00004bf0: 6c60 e592 8c60 782d 6b73 732d 6361 6c6c  l`...`x-kss-call
+00004c00: 6261 636b 626f 6479 60e8 afb7 e6b1 82e5  backbody`.......
+00004c10: a4b4 efbc 8ce8 afa6 e8a7 81e6 9687 e6a1  ................
+00004c20: a35b e4b8 8ae4 bca0 e59b 9ee8 b083 e5a4  .[..............
+00004c30: 84e7 9086 5d28 6874 7470 733a 2f2f 646f  ....](https://do
+00004c40: 6373 2e6b 7379 756e 2e63 6f6d 2f64 6f63  cs.ksyun.com/doc
+00004c50: 756d 656e 7473 2f39 3536 29e3 8082 0a20  uments/956).... 
+00004c60: 2023 2078 2d6b 7373 2d63 616c 6c62 6163   # x-kss-callbac
+00004c70: 6b75 726c 20e4 b8ba e58f 91e8 b5b7 e59b  kurl ...........
+00004c80: 9ee8 b083 e697 b6e8 afb7 e6b1 82e7 9a84  ................
+00004c90: e69c 8de5 8aa1 e599 a8e5 9cb0 e59d 800a  ................
+00004ca0: 2020 2320 782d 6b73 732d 6361 6c6c 6261    # x-kss-callba
+00004cb0: 636b 626f 6479 20e4 b8ba e58f 91e8 b5b7  ckbody .........
+00004cc0: e59b 9ee8 b083 e697 b6e8 afb7 e6b1 82e7  ................
+00004cd0: 9a84 626f 6479 e79a 84e5 80bc 0a20 2068  ..body.......  h
+00004ce0: 6561 6465 7273 203d 207b 2278 2d6b 7373  eaders = {"x-kss
+00004cf0: 2d63 616c 6c62 6163 6b75 726c 223a 2022  -callbackurl": "
+00004d00: 6874 7470 733a 2f2f 7968 2d73 682e 6b73  https://yh-sh.ks
+00004d10: 332d 636e 2d73 6861 6e67 6861 692e 6b73  3-cn-shanghai.ks
+00004d20: 7975 6e63 732e 636f 6d22 2c20 2278 2d6b  yuncs.com", "x-k
+00004d30: 7373 2d63 616c 6c62 6163 6b62 6f64 7922  ss-callbackbody"
+00004d40: 3a20 226f 626a 6563 744b 6579 3d24 7b6b  : "objectKey=${k
+00004d50: 6579 7d26 6574 6167 3d24 7b65 7461 677d  ey}&etag=${etag}
+00004d60: 2662 7563 6b65 743d 247b 6275 636b 6574  &bucket=${bucket
+00004d70: 7d26 6f62 6a65 6374 5369 7a65 3d24 7b6f  }&objectSize=${o
+00004d80: 626a 6563 7453 697a 657d 266d 696d 6554  bjectSize}&mimeT
+00004d90: 7970 653d 247b 6d69 6d65 5479 7065 7d26  ype=${mimeType}&
+00004da0: 6372 6561 7465 5469 6d65 3d24 7b63 7265  createTime=${cre
+00004db0: 6174 6554 696d 657d 222c 2022 782d 6b73  ateTime}", "x-ks
+00004dc0: 732d 6361 6c6c 6261 636b 6175 7468 223a  s-callbackauth":
+00004dd0: 317d 0a20 2072 6574 203d 206b 2e73 6574  1}.  ret = k.set
+00004de0: 5f63 6f6e 7465 6e74 735f 6672 6f6d 5f73  _contents_from_s
+00004df0: 7472 696e 6728 2274 6573 742d 6361 6c6c  tring("test-call
+00004e00: 6261 636b 222c 2068 6561 6465 7273 3d68  back", headers=h
+00004e10: 6561 6465 7273 290a 2020 6966 2072 6574  eaders).  if ret
+00004e20: 2061 6e64 2072 6574 2e73 7461 7475 7320   and ret.status 
+00004e30: 3d3d 2032 3030 3a0a 2020 2020 7072 696e  == 200:.    prin
+00004e40: 7428 22e4 b88a e4bc a0e6 8890 e58a 9f22  t("............"
+00004e50: 290a 0a23 2067 6574 416c 6c42 7563 6b65  )..# getAllBucke
+00004e60: 7473 2829 0a23 2068 6561 6442 7563 6b65  ts().# headBucke
+00004e70: 7428 2762 6a27 290a 2320 6765 7442 7563  t('bj').# getBuc
+00004e80: 6b65 744c 6f63 6174 696f 6e28 2774 6573  ketLocation('tes
+00004e90: 742d 686f 7374 2d73 7479 6c65 2729 0a23  t-host-style').#
+00004ea0: 2063 7265 6174 6542 7563 6b65 7428 2774   createBucket('t
+00004eb0: 6573 742d 6275 636b 6574 2d61 7263 6869  est-bucket-archi
+00004ec0: 7665 2d74 6573 742d 7368 616e 6768 6169  ve-test-shanghai
+00004ed0: 3227 2c20 6c6f 6361 7469 6f6e 3d27 5348  2', location='SH
+00004ee0: 414e 4748 4149 2729 0a23 2064 656c 6574  ANGHAI').# delet
+00004ef0: 6542 7563 6b65 7428 2774 6573 742d 6275  eBucket('test-bu
+00004f00: 636b 6574 2729 0a23 2067 6574 4275 636b  cket').# getBuck
+00004f10: 6574 4163 6c28 2774 6573 742d 6275 636b  etAcl('test-buck
+00004f20: 6574 2729 0a23 2073 6574 4275 636b 6574  et').# setBucket
+00004f30: 4163 6c28 2774 6573 742d 6275 636b 6574  Acl('test-bucket
+00004f40: 2729 0a23 206d 616e 6167 6542 7563 6b65  ').# manageBucke
+00004f50: 7452 6570 6c69 6361 7469 6f6e 2827 7465  tReplication('te
+00004f60: 7374 2d62 7563 6b65 7427 290a 2320 6765  st-bucket').# ge
+00004f70: 7442 7563 6b65 744c 6966 6543 7963 6c65  tBucketLifeCycle
+00004f80: 2862 7563 6b65 745f 6e61 6d65 290a 2320  (bucket_name).# 
+00004f90: 7365 7442 7563 6b65 744c 6966 6543 7963  setBucketLifeCyc
+00004fa0: 6c65 2862 7563 6b65 745f 6e61 6d65 290a  le(bucket_name).
+00004fb0: 2320 7365 7442 7563 6b65 744c 6966 6543  # setBucketLifeC
+00004fc0: 7963 6c65 3228 6275 636b 6574 5f6e 616d  ycle2(bucket_nam
+00004fd0: 6529 0a23 2064 656c 6574 6542 7563 6b65  e).# deleteBucke
+00004fe0: 744c 6966 6543 7963 6c65 2862 7563 6b65  tLifeCycle(bucke
+00004ff0: 745f 6e61 6d65 290a 2320 6765 7442 7563  t_name).# getBuc
+00005000: 6b65 744c 6f67 6769 6e67 2862 7563 6b65  ketLogging(bucke
+00005010: 745f 6e61 6d65 290a 2320 7365 7442 7563  t_name).# setBuc
+00005020: 6b65 744c 6f67 6769 6e67 2862 7563 6b65  ketLogging(bucke
+00005030: 745f 6e61 6d65 290a 2320 6469 7361 626c  t_name).# disabl
+00005040: 6542 7563 6b65 744c 6f67 6769 6e67 2862  eBucketLogging(b
+00005050: 7563 6b65 745f 6e61 6d65 290a 2320 656e  ucket_name).# en
+00005060: 6162 6c65 4275 636b 6574 4c6f 6767 696e  ableBucketLoggin
+00005070: 6728 6275 636b 6574 5f6e 616d 6529 0a23  g(bucket_name).#
+00005080: 2070 7574 4275 636b 6574 436f 7273 2862   putBucketCors(b
+00005090: 7563 6b65 745f 6e61 6d65 290a 2320 6765  ucket_name).# ge
+000050a0: 7442 7563 6b65 7443 6f72 7328 6275 636b  tBucketCors(buck
+000050b0: 6574 5f6e 616d 6529 0a23 2064 656c 6574  et_name).# delet
+000050c0: 6542 7563 6b65 7443 6f72 7328 6275 636b  eBucketCors(buck
+000050d0: 6574 5f6e 616d 6529 0a23 2064 656c 6574  et_name).# delet
+000050e0: 6542 7563 6b65 7443 7272 2862 7563 6b65  eBucketCrr(bucke
+000050f0: 745f 6e61 6d65 290a 2320 6765 7442 7563  t_name).# getBuc
+00005100: 6b65 7443 7272 2862 7563 6b65 745f 6e61  ketCrr(bucket_na
+00005110: 6d65 290a 2320 7365 7442 7563 6b65 7443  me).# setBucketC
+00005120: 7272 2862 7563 6b65 745f 6e61 6d65 290a  rr(bucket_name).
+00005130: 2320 7365 7442 7563 6b65 744d 6972 726f  # setBucketMirro
+00005140: 7228 6275 636b 6574 5f6e 616d 6529 0a23  r(bucket_name).#
+00005150: 2064 656c 6574 6542 7563 6b65 744d 6972   deleteBucketMir
+00005160: 726f 7228 6275 636b 6574 5f6e 616d 6529  ror(bucket_name)
+00005170: 0a23 2067 6574 4275 636b 6574 4d69 7272  .# getBucketMirr
+00005180: 6f72 2862 7563 6b65 745f 6e61 6d65 290a  or(bucket_name).
+00005190: 2323 2323 2320 6f62 6a65 6374 2023 2323  ##### object ###
+000051a0: 2323 0a23 2067 6574 4f62 6a65 6374 4d65  ##.# getObjectMe
+000051b0: 7461 2862 7563 6b65 745f 6e61 6d65 2c20  ta(bucket_name, 
+000051c0: 2761 7274 6963 6c65 2e74 7874 2729 0a23  'article.txt').#
+000051d0: 206c 6973 745f 6f62 6a65 6374 7328 290a   list_objects().
+000051e0: 2320 6c69 7374 4f62 6a65 6374 734d 6f72  # listObjectsMor
+000051f0: 6528 2261 7574 6f2d 7465 7374 2d62 7563  e("auto-test-buc
+00005200: 6b65 7422 2c20 6465 6c69 6d69 7465 723d  ket", delimiter=
+00005210: 272f 272c 206d 6178 5f6b 6579 733d 322c  '/', max_keys=2,
+00005220: 206d 6172 6b65 723d 2731 3035 3027 290a   marker='1050').
+00005230: 2320 6c69 7374 4f62 6a65 6374 734d 6f72  # listObjectsMor
+00005240: 6528 2261 7574 6f2d 7465 7374 2d62 7563  e("auto-test-buc
+00005250: 6b65 7422 2c20 6465 6c69 6d69 7465 723d  ket", delimiter=
+00005260: 272f 272c 206d 6178 5f6b 6579 733d 322c  '/', max_keys=2,
+00005270: 206d 6172 6b65 723d 2731 3035 2f27 290a   marker='105/').
+00005280: 2320 6c69 7374 4f62 6a65 6374 734d 6f72  # listObjectsMor
+00005290: 6528 2261 7574 6f2d 7465 7374 2d62 7563  e("auto-test-buc
+000052a0: 6b65 7422 2c20 6465 6c69 6d69 7465 723d  ket", delimiter=
+000052b0: 272f 272c 206d 6178 5f6b 6579 733d 322c  '/', max_keys=2,
+000052c0: 206d 6172 6b65 723d 2731 3035 2532 4627   marker='105%2F'
+000052d0: 290a 2320 6c69 7374 4f62 6a65 6374 7341  ).# listObjectsA
+000052e0: 6e64 4669 6c74 6572 2829 0a23 2073 6574  ndFilter().# set
+000052f0: 4f62 6a65 6374 5461 6767 696e 6728 290a  ObjectTagging().
+00005300: 2320 6765 744f 626a 6563 7454 6167 6769  # getObjectTaggi
+00005310: 6e67 2829 0a23 2064 656c 6574 654f 626a  ng().# deleteObj
+00005320: 6563 7454 6167 6769 6e67 2829 0a23 2067  ectTagging().# g
+00005330: 6574 466f 6c64 6572 5369 7a65 496e 4275  etFolderSizeInBu
+00005340: 636b 6574 2829 3b0a 2320 646f 776e 6c6f  cket();.# downlo
+00005350: 6164 4f62 6a65 6374 416e 6450 7269 6e74  adObjectAndPrint
+00005360: 2829 0a23 2064 6f77 6e6c 6f61 644f 626a  ().# downloadObj
+00005370: 6563 7441 7353 7472 6561 6d41 6e64 5072  ectAsStreamAndPr
+00005380: 696e 7428 290a 2320 646f 776e 6c6f 6164  int().# download
+00005390: 4f62 6a65 6374 416e 6453 6176 6528 6275  ObjectAndSave(bu
+000053a0: 636b 6574 5f6e 616d 652c 2027 4453 4330  cket_name, 'DSC0
+000053b0: 3333 3830 2e65 6e63 7279 7074 2ee9 9d9e  3380.encrypt....
+000053c0: e588 86e5 9d97 2e6a 7067 272c 2068 6561  .......jpg', hea
+000053d0: 6465 7273 3d7b 0a23 2020 2027 7261 6e67  ders={.#   'rang
+000053e0: 6527 3a20 2762 7974 6573 3d30 2d35 3234  e': 'bytes=0-524
+000053f0: 3238 3830 270a 2320 7d29 0a23 2063 6f75  2880'.# }).# cou
+00005400: 6e74 203d 2032 300a 2320 7768 696c 6520  nt = 20.# while 
+00005410: 5472 7565 3a0a 2320 7570 6c6f 6164 4f62  True:.# uploadOb
+00005420: 6a65 6374 4672 6f6d 4669 6c65 2827 e6b3  jectFromFile('..
+00005430: 95e6 b2bb 2e6a 7065 6727 290a 7570 6c6f  .....jpeg').uplo
+00005440: 6164 5f61 7379 6e63 2827 e6b3 95e6 b2bb  ad_async('......
+00005450: 2e6a 7065 6727 290a 646f 776e 6c6f 6164  .jpeg').download
+00005460: 5f61 7379 6e63 2827 3136 3539 3638 3438  _async('16596848
+00005470: 3732 2e74 6f72 7265 6e74 2729 0a23 2075  72.torrent').# u
+00005480: 706c 6f61 644f 626a 6563 7446 726f 6d46  ploadObjectFromF
+00005490: 696c 6528 2778 6162 2729 0a23 2075 706c  ile('xab').# upl
+000054a0: 6f61 644f 626a 6563 7446 726f 6d46 696c  oadObjectFromFil
+000054b0: 6528 2778 6163 2729 0a23 2020 2074 696d  e('xac').#   tim
+000054c0: 652e 736c 6565 7028 3529 0a23 2020 2063  e.sleep(5).#   c
+000054d0: 6f75 6e74 203d 2063 6f75 6e74 202d 2031  ount = count - 1
+000054e0: 0a23 2075 706c 6f61 644f 626a 6563 7446  .# uploadObjectF
+000054f0: 726f 6d53 7472 696e 6728 290a 2320 6865  romString().# he
+00005500: 6164 4f62 6a65 6374 2829 0a23 2064 6f77  adObject().# dow
+00005510: 6e6c 6f61 644f 626a 6563 7441 6e64 5072  nloadObjectAndPr
+00005520: 696e 7428 2774 6573 745f 6469 7265 6374  int('test_direct
+00005530: 6f72 792f 2729 0a23 2064 656c 6574 654f  ory/').# deleteO
+00005540: 626a 6563 7428 2274 656c 6c6d 6577 6879  bject("tellmewhy
+00005550: 2229 0a23 2067 6574 4f62 6a65 6374 4163  ").# getObjectAc
+00005560: 6c28 290a 0a23 2074 6573 745f 6d75 6c74  l()..# test_mult
+00005570: 6970 6172 745f 7570 6c6f 6164 2865 6e63  ipart_upload(enc
+00005580: 7279 7074 5f6b 6579 3d54 7275 6529 0a0a  rypt_key=True)..
+00005590: 2320 7465 7374 5f66 6574 6368 5f6f 626a  # test_fetch_obj
+000055a0: 6563 7428 290a 2320 6465 6620 7465 7374  ect().# def test
+000055b0: 5f67 656e 6572 6174 655f 7572 6c28 6b65  _generate_url(ke
+000055c0: 795f 6e61 6d65 2c20 696d 6167 655f 6174  y_name, image_at
+000055d0: 7472 733d 4e6f 6e65 293a 0a23 2020 2062  trs=None):.#   b
+000055e0: 203d 2063 6f6e 6e2e 6765 745f 6275 636b   = conn.get_buck
+000055f0: 6574 2862 7563 6b65 745f 6e61 6d65 290a  et(bucket_name).
+00005600: 2320 2020 6b20 3d20 622e 6765 745f 6b65  #   k = b.get_ke
+00005610: 7928 6b65 795f 6e61 6d65 290a 2320 2020  y(key_name).#   
+00005620: 6966 206b 3a0a 2320 2020 2020 7572 6c20  if k:.#     url 
+00005630: 3d20 6b2e 6765 6e65 7261 7465 5f75 726c  = k.generate_url
+00005640: 2836 3030 2c20 696d 6167 655f 6174 7472  (600, image_attr
+00005650: 733d 696d 6167 655f 6174 7472 7329 2020  s=image_attrs)  
+00005660: 2320 3630 7320 e590 8ee8 afa5 e993 bee6  # 60s ..........
+00005670: 8ea5 e8bf 87e6 9c9f 0a23 2020 2020 2070  .........#     p
+00005680: 7269 6e74 2875 726c 290a 2320 2020 656c  rint(url).#   el
+00005690: 7365 3a0a 2320 2020 2020 7072 696e 7428  se:.#     print(
+000056a0: 276f 626a 6563 7420 6e6f 7420 666f 756e  'object not foun
+000056b0: 6427 290a 0a23 2062 7563 6b65 7420 3d20  d')..# bucket = 
+000056c0: 636f 6e6e 2e67 6574 5f62 7563 6b65 7428  conn.get_bucket(
+000056d0: 2774 6573 742d 6275 636b 6574 2729 0a23  'test-bucket').#
+000056e0: 206b 6579 7320 3d20 6275 636b 6574 2e6c   keys = bucket.l
+000056f0: 6973 7428 290a 2320 666f 7220 6b20 696e  ist().# for k in
+00005700: 206b 6579 733a 0a23 2020 2070 7269 6e74   keys:.#   print
+00005710: 286b 290a 2320 2020 6966 2069 7369 6e73  (k).#   if isins
+00005720: 7461 6e63 6528 6b2c 204b 6579 293a 0a23  tance(k, Key):.#
+00005730: 2020 2020 2075 726c 203d 206b 2e67 656e       url = k.gen
+00005740: 6572 6174 655f 7572 6c28 3630 3029 0a23  erate_url(600).#
+00005750: 2020 2020 2072 6573 203d 2072 6571 7565       res = reque
+00005760: 7374 732e 6765 7428 7572 6c29 0a23 2020  sts.get(url).#  
+00005770: 2020 2069 6620 7265 732e 7374 6174 7573     if res.status
+00005780: 5f63 6f64 6520 213d 2032 3030 3a0a 2320  _code != 200:.# 
+00005790: 2020 2020 2020 7072 696e 7428 7572 6c29        print(url)
+000057a0: 0a0a 0a23 2072 6573 203d 2072 6571 7565  ...# res = reque
+000057b0: 7374 732e 6765 7428 7572 6c29 0a23 2061  sts.get(url).# a
+000057c0: 7373 6572 7420 7265 732e 7374 6174 7573  ssert res.status
+000057d0: 5f63 6f64 6520 213d 2034 3033 0a23 2074  _code != 403.# t
+000057e0: 6573 745f 6765 6e65 7261 7465 5f75 726c  est_generate_url
+000057f0: 2827 5c5c 615c 5c5c 5c3a 3c3e 2a3f 7c3a  ('\\a\\\\:<>*?|:
+00005800: 712e 6a70 6567 2729 0a23 2074 6573 745f  q.jpeg').# test_
+00005810: 6765 6e65 7261 7465 5f75 726c 2827 2378  generate_url('#x
+00005820: 323b 2e6a 702e 6373 7627 290a 2320 7465  2;.jp.csv').# te
+00005830: 7374 5f67 656e 6572 6174 655f 7572 6c28  st_generate_url(
+00005840: 2731 3030 3836 2f31 3938 2e31 382d 7265  '10086/198.18-re
+00005850: 7365 742d e585 b1e8 aea1 39e6 9da1 2e74  set-......9....t
+00005860: 7874 2729 0a23 2074 6573 745f 6765 6e65  xt').# test_gene
+00005870: 7261 7465 5f75 726c 2827 3130 3038 362f  rate_url('10086/
+00005880: 6765 7462 7563 6b65 742e 6373 7627 290a  getbucket.csv').
+00005890: 2320 7465 7374 5f67 6574 5f70 7265 7369  # test_get_presi
+000058a0: 676e 6564 5f75 726c 2827 7e2a 632f 6865  gned_url('~*c/he
+000058b0: 636b 4461 7461 2b73 6466 3d25 3246 2e6a  ckData+sdf=%2F.j
+000058c0: 736f 6e27 290a 2320 7465 7374 5f70 7574  son').# test_put
+000058d0: 5f76 6961 5f70 7265 7369 676e 6564 5f75  _via_presigned_u
+000058e0: 726c 2827 696e 6465 782e 6874 6d6c 2729  rl('index.html')
+000058f0: 0a23 206c 6973 745f 6f62 6a65 6374 735f  .# list_objects_
+00005900: 7632 2864 656c 696d 6974 6572 3d27 2f27  v2(delimiter='/'
+00005910: 2c20 656e 636f 6469 6e67 5f74 7970 653d  , encoding_type=
+00005920: 2775 726c 272c 2066 6574 6368 5f6f 776e  'url', fetch_own
+00005930: 6572 3d46 616c 7365 290a 2320 6c69 7374  er=False).# list
+00005940: 5f6f 626a 6563 7473 2829 0a23 206c 6973  _objects().# lis
+00005950: 744f 626a 6563 7473 4d6f 7265 2829 0a23  tObjectsMore().#
+00005960: 2064 656c 6574 654f 626a 6563 7428 290a   deleteObject().
+00005970: 2320 6c69 7374 4f62 6a65 6374 7341 6e64  # listObjectsAnd
+00005980: 4669 6c74 6572 2829 0a23 206c 6973 7441  Filter().# listA
+00005990: 6e64 4465 6c65 7465 2829 0a23 2072 6573  ndDelete().# res
+000059a0: 746f 7265 4f62 6a65 6374 2822 7777 772d  toreObject("www-
+000059b0: 6c6f 676f 2229 0a23 2067 6574 4275 636b  logo").# getBuck
+000059c0: 6574 7344 6174 6128 2274 6573 742d 6275  etsData("test-bu
+000059d0: 636b 6574 2229 0a23 2074 6573 745f 6173  cket").# test_as
+000059e0: 7375 6d65 526f 6c65 2829 0a0a 2320 636f  sumeRole()..# co
+000059f0: 7079 5f65 6e63 7279 7074 696f 6e28 2761  py_encryption('a
+00005a00: 7274 6963 6c65 2e65 6e63 7279 7074 696f  rticle.encryptio
+00005a10: 6e2e 7478 7427 2c20 2761 7274 6963 6c65  n.txt', 'article
+00005a20: 2e74 7874 272c 2065 6e63 7279 7074 5f6b  .txt', encrypt_k
+00005a30: 6579 3d54 7275 6529 0a0a 2320 6669 6c65  ey=True)..# file
+00005a40: 4e61 6d65 203d 2022 5c75 3030 3662 5c75  Name = "\u006b\u
+00005a50: 3030 3733 5c75 3030 3566 5c75 3030 3733  0073\u005f\u0073
+00005a60: 5c75 3030 3633 5c75 3030 3631 5c75 3030  \u0063\u0061\u00
+00005a70: 3665 5c75 3030 3566 5c75 3030 3666 5c75  6e\u005f\u006f\u
+00005a80: 3030 3633 5c75 3030 3732 5c75 3030 3266  0063\u0072\u002f
+00005a90: 5c75 3030 3332 5c75 3030 3330 5c75 3030  \u0032\u0030\u00
+00005aa0: 3331 5c75 3030 3338 5c75 3030 3264 5c75  31\u0038\u002d\u
+00005ab0: 3030 3330 5c75 3030 3333 5c75 3030 3264  0030\u0033\u002d
+00005ac0: 5c75 3030 3331 5c75 3030 3332 5c75 3030  \u0031\u0032\u00
+00005ad0: 3266 5c75 3030 3130 5c75 6666 6664 5c75  2f\u0010\ufffd\u
+00005ae0: 3030 3730 5c75 6666 6664 5c75 6666 6664  0070\ufffd\ufffd
+00005af0: 5c75 6666 6664 5c75 3030 3032 5c75 3030  \ufffd\u0002\u00
+00005b00: 3265 5c75 3030 3537 5c75 3030 3766 5c75  2e\u0057\u007f\u
+00005b10: 3030 3562 5c75 6666 6664 5c75 3030 3038  005b\ufffd\u0008
+00005b20: 5c75 6666 6664 5c75 3030 3261 5c75 6666  \ufffd\u002a\uff
+00005b30: 6664 5c75 3030 3265 5c75 3030 3661 5c75  fd\u002e\u006a\u
+00005b40: 3030 3730 5c75 3030 3637 223b 0a23 2068  0070\u0067";.# h
+00005b50: 6568 6520 3d20 2210 efbf bd70 efbf bdef  ehe = "....p....
+00005b60: bfbd efbf bd02 2e57 7f5b efbf bd2a efbf  .......W.[...*..
+00005b70: bd2e 6a70 6722 0a23 2066 6f72 2063 2069  ..jpg".# for c i
+00005b80: 6e20 6865 6865 3a0a 2320 2020 2020 7072  n hehe:.#     pr
+00005b90: 696e 7428 7265 7072 2863 292c 2063 290a  int(repr(c), c).
+00005ba0: 2320 7572 6c63 6f64 6564 203d 2075 726c  # urlcoded = url
+00005bb0: 6c69 622e 7061 7273 652e 7175 6f74 6528  lib.parse.quote(
+00005bc0: 6669 6c65 4e61 6d65 290a 2320 756e 7175  fileName).# unqu
+00005bd0: 6f74 6564 203d 2075 726c 6c69 622e 7061  oted = urllib.pa
+00005be0: 7273 652e 756e 7175 6f74 6528 2725 4646  rse.unquote('%FF
+00005bf0: 2729 0a23 2071 756f 7465 6420 3d20 7572  ').# quoted = ur
+00005c00: 6c6c 6962 2e70 6172 7365 2e71 756f 7465  llib.parse.quote
+00005c10: 2875 6e71 756f 7465 6429 0a23 2070 7269  (unquoted).# pri
+00005c20: 6e74 2875 6e71 756f 7465 6429 0a23 2070  nt(unquoted).# p
+00005c30: 7269 6e74 2871 756f 7465 6429 0a0a 2320  rint(quoted)..# 
+00005c40: 6765 744f 626a 6563 744d 6574 6128 2774  getObjectMeta('t
+00005c50: 6573 742d 6275 636b 6574 272c 2027 6172  est-bucket', 'ar
+00005c60: 7469 636c 652e 7478 7427 290a 2320 6b65  ticle.txt').# ke
+00005c70: 7920 3d20 636f 7079 2827 6172 7469 636c  y = copy('articl
+00005c80: 652e 7478 7427 2c20 2761 7274 6963 6c65  e.txt', 'article
+00005c90: 2e74 7874 272c 2064 7374 5f62 7563 6b65  .txt', dst_bucke
+00005ca0: 745f 6e61 6d65 3d27 7465 7374 2d62 7563  t_name='test-buc
+00005cb0: 6b65 7427 290a 2320 7072 696e 7428 2761  ket').# print('a
+00005cc0: 6674 6572 2063 6f70 795c 6e5c 6e27 290a  fter copy\n\n').
+00005cd0: 2320 6765 744f 626a 6563 744d 6574 6128  # getObjectMeta(
+00005ce0: 2774 6573 742d 6275 636b 6574 272c 2027  'test-bucket', '
+00005cf0: 6172 7469 636c 652e 7478 7427 290a 2320  article.txt').# 
+00005d00: 6765 744f 626a 6563 744d 6574 6128 2774  getObjectMeta('t
+00005d10: 6573 742d 6275 636b 6574 272c 2027 4453  est-bucket', 'DS
+00005d20: 4330 3333 3830 2e73 7365 632e 6a70 6727  C03380.ssec.jpg'
+00005d30: 290a 2320 7570 6c6f 6164 4f62 6a65 6374  ).# uploadObject
+00005d40: 4672 6f6d 4669 6c65 2827 4453 4330 3333  FromFile('DSC033
+00005d50: 3830 2e65 6e63 7279 7074 2e6a 7067 2729  80.encrypt.jpg')
+00005d60: 0a0a 2320 696d 706f 7274 2062 6173 6536  ..# import base6
+00005d70: 340a 2320 696d 706f 7274 2068 6d61 630a  4.# import hmac.
+00005d80: 2320 696d 706f 7274 2068 6173 686c 6962  # import hashlib
+00005d90: 0a23 2069 6d70 6f72 7420 7572 6c6c 6962  .# import urllib
+00005da0: 0a23 2068 203d 2068 6d61 632e 6e65 7728  .# h = hmac.new(
+00005db0: 2261 6363 6573 736b 6579 222c 0a23 2020  "accesskey",.#  
+00005dc0: 2020 2020 2020 2020 2020 2020 2247 4554              "GET
+00005dd0: 5c6e 5c6e 5c6e 3131 3431 3838 3931 3230  \n\n\n1141889120
+00005de0: 5c6e 2f65 7861 6d70 6c65 6275 636b 6574  \n/examplebucket
+00005df0: 2f6f 7373 2d61 7069 2e70 6466 222c 0a23  /oss-api.pdf",.#
+00005e00: 2020 2020 2020 2020 2020 2020 2020 6861                ha
+00005e10: 7368 6c69 622e 7368 6131 290a 2320 7572  shlib.sha1).# ur
+00005e20: 6c6c 6962 2e71 756f 7465 2028 6261 7365  llib.quote (base
+00005e30: 3634 2e65 6e63 6f64 6573 7472 696e 6728  64.encodestring(
+00005e40: 682e 6469 6765 7374 2829 292e 7374 7269  h.digest()).stri
+00005e50: 7028 2929 0a0a 2320 6220 3d20 636f 6e6e  p())..# b = conn
+00005e60: 2e67 6574 5f62 7563 6b65 7428 6275 636b  .get_bucket(buck
+00005e70: 6574 5f6e 616d 6529 0a23 2023 2066 6f72  et_name).# # for
+00005e80: 2070 2069 6e20 622e 6765 745f 616c 6c5f   p in b.get_all_
+00005e90: 6d75 6c74 6970 6172 745f 7570 6c6f 6164  multipart_upload
+00005ea0: 7328 6b65 795f 6d61 726b 6572 3d27 7465  s(key_marker='te
+00005eb0: 7374 2d6d 756c 7469 272c 2075 706c 6f61  st-multi', uploa
+00005ec0: 645f 6964 5f6d 6172 6b65 723d 2762 6266  d_id_marker='bbf
+00005ed0: 6366 3062 6162 3565 3834 3564 3839 3564  cf0bab5e845d895d
+00005ee0: 3063 6663 6432 3633 3262 6631 3827 293a  0cfcd2632bf18'):
+00005ef0: 2020 2020 2737 6536 6237 6237 3931 3264      '7e6b7b7912d
+00005f00: 3134 6562 3039 3432 3431 3366 3236 3263  14eb0942413f262c
+00005f10: 3438 3865 6327 0a23 2061 6c6c 5f75 706c  488ec'.# all_upl
+00005f20: 6f61 6473 203d 2062 2e67 6574 5f61 6c6c  oads = b.get_all
+00005f30: 5f6d 756c 7469 7061 7274 5f75 706c 6f61  _multipart_uploa
+00005f40: 6473 286b 6579 5f6d 6172 6b65 723d 2744  ds(key_marker='D
+00005f50: 5343 3033 3338 302e 656e 6372 7970 742e  SC03380.encrypt.
+00005f60: 6a70 672d 6464 6464 6464 6464 2729 236d  jpg-dddddddd')#m
+00005f70: 6178 5f75 706c 6f61 6473 3d32 3729 0a23  ax_uploads=27).#
+00005f80: 2070 7269 6e74 286c 656e 2861 6c6c 5f75   print(len(all_u
+00005f90: 706c 6f61 6473 2929 0a23 2066 6f72 2070  ploads)).# for p
+00005fa0: 2069 6e20 616c 6c5f 7570 6c6f 6164 733a   in all_uploads:
+00005fb0: 0a23 2020 2070 7269 6e74 2870 2c20 702e  .#   print(p, p.
+00005fc0: 6964 290a 2320 7075 745f 6f62 6a65 6374  id).# put_object
+00005fd0: 5f63 616c 6c62 6163 6b28 2774 6573 742d  _callback('test-
+00005fe0: 6361 6c6c 6261 636b 2729                 callback')
```

### Comparing `ks3sdk-1.6.1/examples/billing.py` & `ks3sdk-1.6.2/examples/billing.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/bucket.py` & `ks3sdk-1.6.2/examples/bucket.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/crc64.py` & `ks3sdk-1.6.2/examples/crc64.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/encryption.py` & `ks3sdk-1.6.2/examples/encryption.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/multi_thread.py` & `ks3sdk-1.6.2/examples/multi_thread.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/multipart.py` & `ks3sdk-1.6.2/examples/multipart.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/object.py` & `ks3sdk-1.6.2/examples/object.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/postProcessTask.py` & `ks3sdk-1.6.2/examples/postProcessTask.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/examples/sts.py` & `ks3sdk-1.6.2/examples/sts.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/acl.py` & `ks3sdk-1.6.2/ks3/acl.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/auth.py` & `ks3sdk-1.6.2/ks3/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
                    'response-content-language', 'response-expires',
                    'response-cache-control', 'response-content-disposition',
                    'response-content-encoding', 'delete', 'lifecycle',
                    'tagging', 'restore', 'notification', 'thumbnail', 'queryadp',
                    'adp', 'asyntask', 'querytask', 'domain',
                    'storageClass',
                    'websiteConfig',
-                   'compose', 'quota', 'policy', 'crr', 'fetch', 'append', 'position', 'mirror']
+                   'compose', 'quota', 'policy', 'crr', 'fetch', 'append', 'position',
+                   'mirror', 'retention', 'recycle', 'recover', 'clear']
 
 
 def url_encode(key):
     if not key:
         return ""
     encode_key = parse.quote(utils.get_utf8_value(key))
     # if '%20' in encode_key:
```

### Comparing `ks3sdk-1.6.1/ks3/authV4.py` & `ks3sdk-1.6.2/ks3/authV4.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/billing.py` & `ks3sdk-1.6.2/ks3/billing.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/bucket.py` & `ks3sdk-1.6.2/ks3/bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 from dateutil import parser
 import ks3.utils
 from ks3 import handler
 from ks3.acl import Policy, CannedACLStrings
 from ks3.bucketlistresultset import BucketListResultSet
 from ks3.bucketlistresultset import MultiPartUploadListResultSet
 from ks3.bucketlistresultset import VersionedBucketListResultSet
+from ks3.bucketlistresultset import BucketRetentionListResultSet
 from ks3.xmlParsers.bucketLogging import BucketLogging
 from ks3.exception import S3ResponseError
 from ks3.key import Key
 from ks3.multipart import MultiPartUpload, CompleteMultiPartUpload
 from ks3.prefix import Prefix
 from ks3.resultset import ResultSet
 from ks3.xmlParsers.bucketQuota import BucketQuota
 from ks3.xmlParsers.bucketVersioning import BucketVersioningConfig
 from ks3.deletemarker import DeleteMarker
+from ks3.xmlParsers.bucketRetention import BucketRetention
 
 try:
     from ks3.encryption import Crypts
 except:
     pass
 
 
@@ -134,14 +136,18 @@
                      expires_in_absolute=False):
         return self.connection.generate_url(expires_in, method, self.name,
                                             headers=headers,
                                             force_http=force_http,
                                             response_headers=response_headers,
                                             expires_in_absolute=expires_in_absolute)
 
+    def lookup(self, key_name):
+        k, resp = self._get_key_internal(key_name, None, None)
+        return k is not None
+
     # def delete_keys(self, keys, quiet=False, mfa_token=None, headers=None):
     #     """
     #     Deletes a set of keys using S3's Multi-object delete API. If a
     #     VersionID is specified for that key then that version is removed.
     #     Returns a MultiDeleteResult Object, which contains Deleted
     #     and Error elements for each key you ask to delete.
     #     """
@@ -311,14 +317,17 @@
 
     def list(self, prefix=None, delimiter='/', marker=None, max_keys=None):
         """
         List object keys within specified bucket.
         """
         return BucketListResultSet(self, prefix, delimiter, marker, max_keys)
 
+    def list_retention(self, prefix=None, delimiter='/', marker=None, max_keys=None):
+        return BucketRetentionListResultSet(self, prefix, delimiter, marker, max_keys)
+
     def listObjects(self, prefix=None, delimiter=None, marker=None, max_keys=None, startTime=None, endTime=None,
                     filename=None, start_time=None, end_time=None):
         if start_time is not None:
             startTime = start_time
         if end_time is not None:
             endTime = end_time
         keys = self.list(prefix, delimiter, marker, max_keys)
@@ -386,14 +395,17 @@
         A lower-level method for listing contents of a bucket.
         """
         return self._get_all([('Version', Key),
                               ('CommonPrefixes', Prefix),
                               ('DeleteMarker', DeleteMarker)],
                              'versions', headers, **params)
 
+    def get_all_retention_keys(self, **params):
+        return self._get_all([('Contents', Key), ('CommonPrefixes', Prefix)], initial_query_string='recycle', **params)
+
     def _get_all(self, element_map, initial_query_string='',
                  headers=None, **params):
         query_args = self._get_all_query_args(
             params,
             initial_query_string=initial_query_string
         )
         response = self.connection.make_request('GET', self.name,
@@ -848,16 +860,17 @@
                                                 query_args='policy', headers=headers)
         body = response.read()
         if response.status == 204:
             return None
         else:
             raise S3ResponseError(response.status, response.reason, body)
 
-    def set_bucket_crr(self, targetBucket, deleteMarkerStatus='Disabled', prefix_list=None, headers=None):
-        replicate = BucketCrossReplicate(targetBucket, deleteMarkerStatus, prefix_list)
+    def set_bucket_crr(self, targetBucket, deleteMarkerStatus=BucketCrossReplicate.DISABLED, prefix_list=None,
+                       historicalObjectReplication=BucketCrossReplicate.DISABLED, headers=None):
+        replicate = BucketCrossReplicate(targetBucket, deleteMarkerStatus, prefix_list, historicalObjectReplication)
         if headers is None:
             headers = {}
         headers['Content-Type'] = 'text/xml'
         replicate_xml = replicate.to_xml()
         if not isinstance(replicate_xml, bytes):
             replicate_xml = replicate_xml.encode('utf-8')
         md5 = ks3.utils.compute_base64_md5_digest(replicate_xml)
@@ -1113,14 +1126,43 @@
         response = self.connection.make_request('DELETE', self.name, query_args='mirror')
         body = response.read()
         if response.status == 204:
             return None
         else:
             raise S3ResponseError(response.status, response.reason, body)
 
+    def set_bucket_retention(self, bucket_retention):
+        headers = {'content-type': 'application/xml'}
+        retention_xml = bucket_retention.to_xml()
+        if not isinstance(retention_xml, bytes):
+            retention_xml = retention_xml.encode('utf-8')
+        md5 = ks3.utils.compute_base64_md5_digest(retention_xml)
+        headers['Content-MD5'] = md5
+        response = self.connection.make_request('PUT', self.name, data=retention_xml,
+                                                query_args='retention',
+                                                headers=headers)
+        body = response.read()
+        if response.status == 200:
+            return None
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
+    def get_bucket_retention(self):
+        response = self.connection.make_request('GET', self.name, query_args='retention')
+        body = response.read()
+        if response.status == 200:
+            retention = BucketRetention()
+            h = handler.XmlHandler(retention, self)
+            if not isinstance(body, bytes):
+                body = body.encode('utf-8')
+            xml.sax.parseString(body, h)
+            return retention
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
 
 class BucketLocation(object):
     def __init__(self):
         self.location = ''
 
     def startElement(self, name, attrs, connection):
         pass
```

### Comparing `ks3sdk-1.6.1/ks3/bucketlistresultset.py` & `ks3sdk-1.6.2/ks3/bucketlistresultset.py`

 * *Files 20% similar despite different names*

```diff
@@ -98,14 +98,41 @@
                                        delimiter=self.delimiter,
                                        key_marker=self.key_marker,
                                        version_id_marker=self.version_id_marker,
                                        headers=self.headers,
                                        encoding_type=self.encoding_type)
 
 
+def bucket_retention_lister(bucket, prefix='', delimiter='', marker='', max_keys=''):
+    more_results = True
+    k = None
+    while more_results:
+        rs = bucket.get_all_retention_keys(prefix=prefix, delimiter=delimiter, marker=marker, max_keys=max_keys)
+        for k in rs:
+            yield k
+        if k:
+            marker = rs.next_marker or k.name
+        if marker:
+            marker = parse.unquote(marker)
+        more_results = rs.is_truncated
+
+
+class BucketRetentionListResultSet(object):
+    def __init__(self, bucket=None, prefix='', delimiter='', marker='', max_keys=''):
+        self.bucket = bucket
+        self.prefix = prefix
+        self.delimiter = delimiter
+        self.marker = marker
+        self.max_keys = max_keys
+
+    def __iter__(self):
+        return bucket_retention_lister(self.bucket, prefix=self.prefix,
+                                       delimiter=self.delimiter, marker=self.marker, max_keys=self.max_keys)
+
+
 def multipart_upload_lister(bucket, key_marker='',
                             upload_id_marker='',
                             headers=None, encoding_type=None):
     """
     A generator function for listing multipart uploads in a bucket.
     """
     more_results = True
```

### Comparing `ks3sdk-1.6.1/ks3/compat.py` & `ks3sdk-1.6.2/ks3/compat.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/connection.py` & `ks3sdk-1.6.2/ks3/connection.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/crc64_combine.py` & `ks3sdk-1.6.2/ks3/crc64_combine.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/deletemarker.py` & `ks3sdk-1.6.2/ks3/deletemarker.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/encryptFp.py` & `ks3sdk-1.6.2/ks3/encryptFp.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/encryption.py` & `ks3sdk-1.6.2/ks3/encryption.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/exception.py` & `ks3sdk-1.6.2/ks3/exception.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/handler.py` & `ks3sdk-1.6.2/ks3/handler.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/http.py` & `ks3sdk-1.6.2/ks3/http.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/key.py` & `ks3sdk-1.6.2/ks3/key.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,17 @@
         self.resp = None
         self.mode = None
         self.size = None
         self.version_id = None
         self.source_version_id = None
         self.delete_marker = False
         self.encrypted = None
+        self.retention_id = None
+        self.recycle_time = None
+        self.estimated_clear_time = None
         #
         self.local_hashes = {}
         self.user_meta = {}
         self.tagging_count = None
         self.object_type = None
         self.append_next_position = None
         self.server_crc = None
@@ -181,14 +184,20 @@
             self.size = int(value)
         elif name == 'StorageClass':
             self.storage_class = value
         elif name == 'Owner':
             pass
         elif name == 'VersionId':
             self.version_id = value
+        elif name == 'RetentionId':
+            self.retention_id = value
+        elif name == 'RecycleTime':
+            self.recycle_time = value
+        elif name == 'EstimatedClearTime':
+            self.estimated_clear_time = value
         else:
             setattr(self, name, value)
 
     def delete(self, headers=None):
         """
         Delete this key from S3
         """
@@ -1105,14 +1114,45 @@
             return None
         else:
             raise S3ResponseError(response.status, response.reason, body)
 
     def fetch_object(self, source_url=None, callback_url=None, headers=None):
         self.bucket.fetch_object(self.name, source_url=source_url, callback_url=callback_url, headers=headers)
 
+    def recover_object(self, overwrite=None, retention_id=None, headers=None):
+        if headers is None:
+            headers = {}
+        if overwrite is not None:
+            headers[self.provider.retention_overwrite_header] = 'true' if overwrite else 'false'
+        if retention_id is not None:
+            headers[self.provider.retention_id_header] = retention_id
+        query_args = 'recover'
+
+        response = self.bucket.connection.make_request('POST', self.bucket.name, self.name,
+                                                       query_args=query_args, headers=headers)
+        body = response.read()
+        if response.status == 200:
+            return None
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
+    def clear_object(self, retention_id=None, headers=None):
+        if headers is None:
+            headers = {}
+        if retention_id is not None:
+            headers[self.provider.retention_id_header] = retention_id
+        query_args = 'clear'
+        response = self.bucket.connection.make_request('DELETE', self.bucket.name, self.name,
+                                                       query_args=query_args, headers=headers)
+        body = response.read()
+        if response.status == 200:
+            return None
+        else:
+            raise S3ResponseError(response.status, response.reason, body)
+
     def handle_version_headers(self, resp, force=False):
         provider = self.bucket.connection.provider
         # If the Key object already has a version_id attribute value, it
         # means that it represents an explicit version and the user is
         # doing a get_contents_*(version_id=<foo>) to retrieve another
         # version of the Key.  In that case, we don't really want to
         # overwrite the version_id in this Key object.  Comprende?
```

### Comparing `ks3sdk-1.6.1/ks3/keyfile.py` & `ks3sdk-1.6.2/ks3/keyfile.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/multipart.py` & `ks3sdk-1.6.2/ks3/multipart.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/objectTagging.py` & `ks3sdk-1.6.2/ks3/objectTagging.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/prefix.py` & `ks3sdk-1.6.2/ks3/prefix.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/provider.py` & `ks3sdk-1.6.2/ks3/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 SERVER_SIDE_ENCRYPTION_KEY = 'server-side-encryption-header'
 VERSION_ID_HEADER_KEY = 'version-id-header'
 RESTORE_HEADER_KEY = 'restore-header'
 TAGGING_COUNT_HEADER_KEY = 'tagging-count-header'
 OBJECT_TYPE_HEADER_KEY = 'object-type-header'
 APPEND_NEXT_POSITION_HEADER_KEY = 'append-next-position-header'
 CHECKSUM_CRC64ECMA_HEADER_KEY = 'checksum-crc64ecma-header'
+RETENTION_OVERWRITE_HEADER_KEY = 'retention-overwrite'
+RETENTION_ID_HEADER_KEY = 'retention-id'
 
 STORAGE_COPY_ERROR = 'StorageCopyError'
 STORAGE_CREATE_ERROR = 'StorageCreateError'
 STORAGE_DATA_ERROR = 'StorageDataError'
 STORAGE_PERMISSIONS_ERROR = 'StoragePermissionsError'
 STORAGE_RESPONSE_ERROR = 'StorageResponseError'
 NO_CREDENTIALS_PROVIDED = object()
@@ -116,15 +118,17 @@
             VERSION_ID_HEADER_KEY: KSS_HEADER_PREFIX + 'version-id',
             STORAGE_CLASS_HEADER_KEY: KSS_HEADER_PREFIX + 'storage-class',
             MFA_HEADER_KEY: KSS_HEADER_PREFIX + 'mfa',
             RESTORE_HEADER_KEY: KSS_HEADER_PREFIX + 'restore',
             TAGGING_COUNT_HEADER_KEY: KSS_HEADER_PREFIX + 'tagging-count',
             OBJECT_TYPE_HEADER_KEY: KSS_HEADER_PREFIX + 'object-type',
             APPEND_NEXT_POSITION_HEADER_KEY: KSS_HEADER_PREFIX + 'append-next-position',
-            CHECKSUM_CRC64ECMA_HEADER_KEY: KSS_HEADER_PREFIX + 'checksum-crc64ecma'
+            CHECKSUM_CRC64ECMA_HEADER_KEY: KSS_HEADER_PREFIX + 'checksum-crc64ecma',
+            RETENTION_OVERWRITE_HEADER_KEY: KSS_HEADER_PREFIX + 'retention-overwrite',
+            RETENTION_ID_HEADER_KEY: KSS_HEADER_PREFIX + 'retention-id'
         },
         'aws': {
             HEADER_PREFIX_KEY: AWS_HEADER_PREFIX,
             METADATA_PREFIX_KEY: AWS_HEADER_PREFIX + 'meta-',
             ACL_HEADER_KEY: AWS_HEADER_PREFIX + 'acl',
             AUTH_HEADER_KEY: 'AWS',
             COPY_SOURCE_HEADER_KEY: AWS_HEADER_PREFIX + 'copy-source',
@@ -449,14 +453,16 @@
         self.version_id = header_info_map[VERSION_ID_HEADER_KEY]
         self.mfa_header = header_info_map[MFA_HEADER_KEY]
         self.restore_header = header_info_map[RESTORE_HEADER_KEY]
         self.tagging_count_header = header_info_map[TAGGING_COUNT_HEADER_KEY]
         self.object_type_header = header_info_map[OBJECT_TYPE_HEADER_KEY]
         self.append_next_position_header = header_info_map[APPEND_NEXT_POSITION_HEADER_KEY]
         self.checksum_crc64ecma_header = header_info_map[CHECKSUM_CRC64ECMA_HEADER_KEY]
+        self.retention_overwrite_header = header_info_map[RETENTION_OVERWRITE_HEADER_KEY]
+        self.retention_id_header = header_info_map[RETENTION_ID_HEADER_KEY]
 
 
     def configure_errors(self):
         error_map = self.ErrorMap[self.name]
         self.storage_copy_error = error_map[STORAGE_COPY_ERROR]
         self.storage_create_error = error_map[STORAGE_CREATE_ERROR]
         self.storage_data_error = error_map[STORAGE_DATA_ERROR]
```

### Comparing `ks3sdk-1.6.1/ks3/resultset.py` & `ks3sdk-1.6.2/ks3/resultset.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/sts.py` & `ks3sdk-1.6.2/ks3/sts.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/user.py` & `ks3sdk-1.6.2/ks3/user.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/utils.py` & `ks3sdk-1.6.2/ks3/utils.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/xmlParsers/bucketCors.py` & `ks3sdk-1.6.2/ks3/xmlParsers/bucketCors.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/xmlParsers/bucketLifecycle.py` & `ks3sdk-1.6.2/ks3/xmlParsers/bucketLifecycle.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ks3.objectTagging import Tag
 
+
 class BucketLifecycle(object):
     def __init__(self, rule=None):
         if rule is None:
             self.rule = []
         else:
             self.rule = rule
 
@@ -27,21 +28,22 @@
         s += '</LifecycleConfiguration>'
         return s
 
 
 class Rule(object):
     def __init__(self, id=None, filter=None, status=None, expiration=None, transitions=None,
                  noncurrent_version_expiration=None,
-                 noncurrent_version_transition=None):
+                 noncurrent_version_transition=None, abort_incomplete_multipart_upload=None):
         self.id = id
         self.filter = filter
         self.status = status
         self.expiration = expiration
-        self.noncurrent_version_expiration=noncurrent_version_expiration
-        self.noncurrent_version_transition=noncurrent_version_transition
+        self.noncurrent_version_expiration = noncurrent_version_expiration
+        self.noncurrent_version_transition = noncurrent_version_transition
+        self.abort_incomplete_multipart_upload = abort_incomplete_multipart_upload
         if transitions is None:
             self.transitions = []
         else:
             self.transitions = transitions
 
     def startElement(self, name, attrs, connection):
         if name == 'Expiration':
@@ -49,14 +51,16 @@
             return self.expiration
         if name == 'Filter':
             self.filter = Filter()
             return self.filter
         if name == 'Transition':
             self.transitions.append(Transition())
             return self.transitions[-1]
+        if name == 'AbortIncompleteMultipartUpload':
+            self.abort_incomplete_multipart_upload = AbortIncompleteMultipartUpload()
         if name == 'NoncurrentVersionTransition':
             self.noncurrent_version_transition = NoncurrentVersionTransition()
             return self.noncurrent_version_transition
         if name == 'NoncurrentVersionExpiration':
             self.noncurrent_version_expiration = NoncurrentVersionExpiration()
             return self.noncurrent_version_expiration
         return None
@@ -78,14 +82,16 @@
         if self.filter is not None:
             s += self.filter.to_xml()
         if self.expiration is not None:
             s += self.expiration.to_xml()
         if self.transitions is not None:
             for t in self.transitions:
                 s += t.to_xml()
+        if self.abort_incomplete_multipart_upload is not None:
+            s += self.abort_incomplete_multipart_upload.to_xml()
         if self.noncurrent_version_expiration is not None:
             s += self.noncurrent_version_expiration.to_xml()
         if self.noncurrent_version_transition is not None:
             s += self.noncurrent_version_transition.to_xml()
         s += '</Rule>'
         return s
 
@@ -204,17 +210,44 @@
         if self.storage_class is not None:
             s += '<StorageClass>%s</StorageClass>' % self.storage_class
         if self.noncurrent_days is not None:
             s += '<NoncurrentDays>%s</NoncurrentDays>' % self.noncurrent_days
         s += '</NoncurrentVersionTransition>'
         return s
 
+
 class NoncurrentVersionExpiration(object):
     def __init__(self, noncurrent_days=None):
         self.noncurrent_days = noncurrent_days
 
     def to_xml(self):
         s = '<NoncurrentVersionExpiration>'
         if self.noncurrent_days is not None:
             s += '<NoncurrentDays>%s</NoncurrentDays>' % self.noncurrent_days
         s += '</NoncurrentVersionExpiration>'
         return s
+
+
+class AbortIncompleteMultipartUpload(object):
+    def __init__(self, days_after_initiation=None, date=None):
+        self.days_after_initiation = days_after_initiation
+        self.date = date
+
+    def startElement(self, name, attrs, connection):
+        return None
+
+    def endElement(self, name, value, connection):
+        if name == 'DaysAfterInitiation':
+            self.days_after_initiation = value
+        elif name == 'Date':
+            self.date = value
+        else:
+            setattr(self, name, value)
+
+    def to_xml(self):
+        s = '<AbortIncompleteMultipartUpload>'
+        if self.days_after_initiation is not None:
+            s += '<DaysAfterInitiation>%s</DaysAfterInitiation>' % self.days_after_initiation
+        if self.date is not None:
+            s += '<Date>%s</Date>' % self.date
+        s += '</AbortIncompleteMultipartUpload>'
+        return s
```

### Comparing `ks3sdk-1.6.1/ks3/xmlParsers/bucketLogging.py` & `ks3sdk-1.6.2/ks3/xmlParsers/bucketLogging.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/xmlParsers/bucketMirror.py` & `ks3sdk-1.6.2/ks3/xmlParsers/bucketMirror.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/xmlParsers/bucketQuota.py` & `ks3sdk-1.6.2/ks3/xmlParsers/bucketQuota.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3/xmlParsers/bucketVersioning.py` & `ks3sdk-1.6.2/ks3/xmlParsers/bucketVersioning.py`

 * *Files identical despite different names*

### Comparing `ks3sdk-1.6.1/ks3sdk.egg-info/PKG-INFO` & `ks3sdk-1.6.2/ks3sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ks3sdk
-Version: 1.6.1
+Version: 1.6.2
 Summary: Ksyun KS3 SDK
 Home-page: https://gitee.com/ks3sdk/ks3-python-sdk
 Author: ksc_ks3
 Author-email: ksc_ks3@kingsoft.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ks3sdk-1.6.1/ks3sdk.egg-info/SOURCES.txt` & `ks3sdk-1.6.2/ks3sdk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,13 +43,14 @@
 ks3/xmlParsers/__init__.py
 ks3/xmlParsers/bucketCors.py
 ks3/xmlParsers/bucketCrossReplicate.py
 ks3/xmlParsers/bucketLifecycle.py
 ks3/xmlParsers/bucketLogging.py
 ks3/xmlParsers/bucketMirror.py
 ks3/xmlParsers/bucketQuota.py
+ks3/xmlParsers/bucketRetention.py
 ks3/xmlParsers/bucketVersioning.py
 ks3sdk.egg-info/PKG-INFO
 ks3sdk.egg-info/SOURCES.txt
 ks3sdk.egg-info/dependency_links.txt
 ks3sdk.egg-info/requires.txt
 ks3sdk.egg-info/top_level.txt
```

### Comparing `ks3sdk-1.6.1/setup.py` & `ks3sdk-1.6.2/setup.py`

 * *Files identical despite different names*

