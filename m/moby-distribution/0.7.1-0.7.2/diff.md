# Comparing `tmp/moby_distribution-0.7.1.tar.gz` & `tmp/moby_distribution-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moby_distribution-0.7.1.tar", max compression
+gzip compressed data, was "moby_distribution-0.7.2.tar", max compression
```

## Comparing `moby_distribution-0.7.1.tar` & `moby_distribution-0.7.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/LICENSE
--rw-r--r--   0        0        0     7006 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/README.md
--rw-r--r--   0        0        0      954 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/__init__.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/__init__.py
--rw-r--r--   0        0        0     5910 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/auth.py
--rw-r--r--   0        0        0     7598 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/client.py
--rw-r--r--   0        0        0      917 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/exceptions.py
--rw-r--r--   0        0        0      752 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/__init__.py
--rw-r--r--   0        0        0    11137 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/blobs.py
--rw-r--r--   0        0        0    15826 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/image.py
--rw-r--r--   0        0        0     4875 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/manifests.py
--rw-r--r--   0        0        0     1033 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/resources/tags.py
--rw-r--r--   0        0        0     3972 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/registry/utils.py
--rw-r--r--   0        0        0        0 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/__init__.py
--rw-r--r--   0        0        0     1140 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/auth.py
--rw-r--r--   0        0        0     1077 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/base.py
--rw-r--r--   0        0        0     4204 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/endpoint.py
--rw-r--r--   0        0        0     3985 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/image_json.py
--rw-r--r--   0        0        0     4615 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/moby_distribution/spec/manifest.py
--rw-r--r--   0        0        0      910 2024-04-07 08:06:17.854354 moby_distribution-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 moby_distribution-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 08:30:35.078737 moby_distribution-0.7.2/LICENSE
+-rw-r--r--   0        0        0     7006 2024-04-07 08:30:35.078737 moby_distribution-0.7.2/README.md
+-rw-r--r--   0        0        0      954 2024-04-07 08:30:35.078737 moby_distribution-0.7.2/moby_distribution/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:30:35.078737 moby_distribution-0.7.2/moby_distribution/registry/__init__.py
+-rw-r--r--   0        0        0     5910 2024-04-07 08:30:35.078737 moby_distribution-0.7.2/moby_distribution/registry/auth.py
+-rw-r--r--   0        0        0     7598 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/client.py
+-rw-r--r--   0        0        0      917 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/exceptions.py
+-rw-r--r--   0        0        0      752 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/resources/__init__.py
+-rw-r--r--   0        0        0    11137 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/resources/blobs.py
+-rw-r--r--   0        0        0    15826 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/resources/image.py
+-rw-r--r--   0        0        0     4875 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/resources/manifests.py
+-rw-r--r--   0        0        0     1033 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/resources/tags.py
+-rw-r--r--   0        0        0     3972 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/registry/utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/spec/__init__.py
+-rw-r--r--   0        0        0     1140 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/spec/auth.py
+-rw-r--r--   0        0        0     1077 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/spec/base.py
+-rw-r--r--   0        0        0     4204 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/spec/endpoint.py
+-rw-r--r--   0        0        0     3985 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/spec/image_json.py
+-rw-r--r--   0        0        0     4615 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/moby_distribution/spec/manifest.py
+-rw-r--r--   0        0        0      910 2024-04-07 08:30:35.082737 moby_distribution-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 moby_distribution-0.7.2/PKG-INFO
```

### Comparing `moby_distribution-0.7.1/LICENSE` & `moby_distribution-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/README.md` & `moby_distribution-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/__init__.py` & `moby_distribution-0.7.2/moby_distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from moby_distribution.spec.image_json import ImageJSON
 from moby_distribution.spec.manifest import (
     ManifestSchema1,
     ManifestSchema2,
     OCIManifestSchema1,
 )
 
-__version__ = "0.7.1"
+__version__ = "0.7.2"
 __all__ = [
     "DockerRegistryV2Client",
     "Blob",
     "ManifestRef",
     "Tags",
     "APIEndpoint",
     "OFFICIAL_ENDPOINT",
```

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/auth.py` & `moby_distribution-0.7.2/moby_distribution/registry/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/client.py` & `moby_distribution-0.7.2/moby_distribution/registry/client.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/exceptions.py` & `moby_distribution-0.7.2/moby_distribution/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/resources/__init__.py` & `moby_distribution-0.7.2/moby_distribution/registry/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/resources/blobs.py` & `moby_distribution-0.7.2/moby_distribution/registry/resources/blobs.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/resources/image.py` & `moby_distribution-0.7.2/moby_distribution/registry/resources/image.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/resources/manifests.py` & `moby_distribution-0.7.2/moby_distribution/registry/resources/manifests.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/resources/tags.py` & `moby_distribution-0.7.2/moby_distribution/registry/resources/tags.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/registry/utils.py` & `moby_distribution-0.7.2/moby_distribution/registry/utils.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/spec/auth.py` & `moby_distribution-0.7.2/moby_distribution/spec/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/spec/base.py` & `moby_distribution-0.7.2/moby_distribution/spec/base.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/spec/endpoint.py` & `moby_distribution-0.7.2/moby_distribution/spec/endpoint.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/spec/image_json.py` & `moby_distribution-0.7.2/moby_distribution/spec/image_json.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/moby_distribution/spec/manifest.py` & `moby_distribution-0.7.2/moby_distribution/spec/manifest.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.7.1/pyproject.toml` & `moby_distribution-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moby-distribution"
-version = "0.7.1"
+version = "0.7.2"
 description = "Yet another moby(docker) distribution implement by python."
 authors = ["shabbywu <shabbywu@qq.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/distribution"
 homepage = "https://github.com/shabbywu/distribution"
```

### Comparing `moby_distribution-0.7.1/PKG-INFO` & `moby_distribution-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moby-distribution
-Version: 0.7.1
+Version: 0.7.2
 Summary: Yet another moby(docker) distribution implement by python.
 Home-page: https://github.com/shabbywu/distribution
 License: Apache-2.0
 Author: shabbywu
 Author-email: shabbywu@qq.com
 Requires-Python: >=3.6.2,<4
 Classifier: License :: OSI Approved :: Apache Software License
```

