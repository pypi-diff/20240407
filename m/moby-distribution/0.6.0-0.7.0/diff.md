# Comparing `tmp/moby_distribution-0.6.0.tar.gz` & `tmp/moby_distribution-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moby_distribution-0.6.0.tar", max compression
+gzip compressed data, was "moby_distribution-0.7.0.tar", max compression
```

## Comparing `moby_distribution-0.6.0.tar` & `moby_distribution-0.7.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/LICENSE
--rw-r--r--   0        0        0     7006 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/README.md
--rw-r--r--   0        0        0      895 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/__init__.py
--rw-r--r--   0        0        0        0 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/__init__.py
--rw-r--r--   0        0        0     5910 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/auth.py
--rw-r--r--   0        0        0     7598 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/client.py
--rw-r--r--   0        0        0      917 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/exceptions.py
--rw-r--r--   0        0        0      752 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/__init__.py
--rw-r--r--   0        0        0    11137 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/blobs.py
--rw-r--r--   0        0        0    14792 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/image.py
--rw-r--r--   0        0        0     4875 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/manifests.py
--rw-r--r--   0        0        0     1033 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/resources/tags.py
--rw-r--r--   0        0        0     3972 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/registry/utils.py
--rw-r--r--   0        0        0        0 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/__init__.py
--rw-r--r--   0        0        0     1140 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/auth.py
--rw-r--r--   0        0        0     1070 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/base.py
--rw-r--r--   0        0        0     4204 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/endpoint.py
--rw-r--r--   0        0        0     3757 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/image_json.py
--rw-r--r--   0        0        0     4594 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/moby_distribution/spec/manifest.py
--rw-r--r--   0        0        0      914 2024-04-02 03:45:12.909599 moby_distribution-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8027 1970-01-01 00:00:00.000000 moby_distribution-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7006 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/README.md
+-rw-r--r--   0        0        0      895 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/registry/__init__.py
+-rw-r--r--   0        0        0     5910 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/registry/auth.py
+-rw-r--r--   0        0        0     7598 2024-04-07 07:30:24.034268 moby_distribution-0.7.0/moby_distribution/registry/client.py
+-rw-r--r--   0        0        0      917 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/exceptions.py
+-rw-r--r--   0        0        0      752 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/__init__.py
+-rw-r--r--   0        0        0    11137 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/blobs.py
+-rw-r--r--   0        0        0    14792 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/image.py
+-rw-r--r--   0        0        0     4875 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/manifests.py
+-rw-r--r--   0        0        0     1033 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/resources/tags.py
+-rw-r--r--   0        0        0     3972 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/registry/utils.py
+-rw-r--r--   0        0        0        0 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/__init__.py
+-rw-r--r--   0        0        0     1140 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/auth.py
+-rw-r--r--   0        0        0     1070 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/base.py
+-rw-r--r--   0        0        0     4204 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/endpoint.py
+-rw-r--r--   0        0        0     3757 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/image_json.py
+-rw-r--r--   0        0        0     4594 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/moby_distribution/spec/manifest.py
+-rw-r--r--   0        0        0      910 2024-04-07 07:30:24.038267 moby_distribution-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8019 1970-01-01 00:00:00.000000 moby_distribution-0.7.0/PKG-INFO
```

### Comparing `moby_distribution-0.6.0/LICENSE` & `moby_distribution-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/README.md` & `moby_distribution-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/__init__.py` & `moby_distribution-0.7.0/moby_distribution/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from moby_distribution.registry.resources.image import ImageRef, LayerRef
 from moby_distribution.registry.resources.manifests import ManifestRef
 from moby_distribution.registry.resources.tags import Tags
 from moby_distribution.spec.endpoint import OFFICIAL_ENDPOINT, APIEndpoint
 from moby_distribution.spec.image_json import ImageJSON
 from moby_distribution.spec.manifest import ManifestSchema1, ManifestSchema2, OCIManifestSchema1
 
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 __ALL__ = [
     "DockerRegistryV2Client",
     "Blob",
     "ManifestRef",
     "Tags",
     "APIEndpoint",
     "ManifestSchema1",
```

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/auth.py` & `moby_distribution-0.7.0/moby_distribution/registry/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/client.py` & `moby_distribution-0.7.0/moby_distribution/registry/client.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/exceptions.py` & `moby_distribution-0.7.0/moby_distribution/registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/resources/__init__.py` & `moby_distribution-0.7.0/moby_distribution/registry/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/resources/blobs.py` & `moby_distribution-0.7.0/moby_distribution/registry/resources/blobs.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/resources/image.py` & `moby_distribution-0.7.0/moby_distribution/registry/resources/image.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/resources/manifests.py` & `moby_distribution-0.7.0/moby_distribution/registry/resources/manifests.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/resources/tags.py` & `moby_distribution-0.7.0/moby_distribution/registry/resources/tags.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/registry/utils.py` & `moby_distribution-0.7.0/moby_distribution/registry/utils.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/spec/auth.py` & `moby_distribution-0.7.0/moby_distribution/spec/auth.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/spec/base.py` & `moby_distribution-0.7.0/moby_distribution/spec/base.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/spec/endpoint.py` & `moby_distribution-0.7.0/moby_distribution/spec/endpoint.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/spec/image_json.py` & `moby_distribution-0.7.0/moby_distribution/spec/image_json.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/moby_distribution/spec/manifest.py` & `moby_distribution-0.7.0/moby_distribution/spec/manifest.py`

 * *Files identical despite different names*

### Comparing `moby_distribution-0.6.0/pyproject.toml` & `moby_distribution-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "moby-distribution"
-version = "0.6.0"
+version = "0.7.0"
 description = "Yet another moby(docker) distribution implement by python."
 authors = ["shabbywu <shabbywu@qq.com>"]
 license = "Apache-2.0"
 
 readme = "README.md"
 repository = "https://github.com/shabbywu/distribution"
 homepage = "https://github.com/shabbywu/distribution"
 
 [tool.poetry.dependencies]
 python = ">= 3.6.2,<4"
 www-authenticate = "^0.9.2"
 requests = ">= 2.20.0"
 pydantic = ">= 1.5"
-py-libtrust = ">= 1.0.4"
+py-libtrust = ">= 2.0.0"
 curlify = "2.2.1"
-cryptography = "<37.0"
+cryptography = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 requests-mock = "^1.9.3"
 docker = "*"
```

### Comparing `moby_distribution-0.6.0/PKG-INFO` & `moby_distribution-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: moby-distribution
-Version: 0.6.0
+Version: 0.7.0
 Summary: Yet another moby(docker) distribution implement by python.
 Home-page: https://github.com/shabbywu/distribution
 License: Apache-2.0
 Author: shabbywu
 Author-email: shabbywu@qq.com
 Requires-Python: >=3.6.2,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: cryptography (<37.0)
+Requires-Dist: cryptography
 Requires-Dist: curlify (==2.2.1)
-Requires-Dist: py-libtrust (>=1.0.4)
+Requires-Dist: py-libtrust (>=2.0.0)
 Requires-Dist: pydantic (>=1.5)
 Requires-Dist: requests (>=2.20.0)
 Requires-Dist: www-authenticate (>=0.9.2,<0.10.0)
 Project-URL: Repository, https://github.com/shabbywu/distribution
 Description-Content-Type: text/markdown
 
 # moby-distribution - Yet another moby(docker) distribution implement by python.
```

