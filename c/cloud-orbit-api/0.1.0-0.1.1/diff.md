# Comparing `tmp/cloud_orbit_api-0.1.0.tar.gz` & `tmp/cloud_orbit_api-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud_orbit_api-0.1.0.tar", max compression
+gzip compressed data, was "cloud_orbit_api-0.1.1.tar", max compression
```

## Comparing `cloud_orbit_api-0.1.0.tar` & `cloud_orbit_api-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2024-04-07 05:53:54.196222 cloud_orbit_api-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-07 05:53:54.196222 cloud_orbit_api-0.1.0/cloud_orbit_api/__init__.py
--rw-r--r--   0        0        0     1123 2024-04-07 05:53:54.196222 cloud_orbit_api-0.1.0/cloud_orbit_api/db_factory.py
--rw-r--r--   0        0        0     1454 2024-04-07 05:53:54.196222 cloud_orbit_api-0.1.0/cloud_orbit_api/main.py
--rw-r--r--   0        0        0       90 2024-04-07 05:53:54.196222 cloud_orbit_api-0.1.0/cloud_orbit_api/models.py
--rw-r--r--   0        0        0      636 2024-04-07 05:53:54.196222 cloud_orbit_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 cloud_orbit_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-04-07 06:47:43.759718 cloud_orbit_api-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 06:47:43.759718 cloud_orbit_api-0.1.1/cloud_orbit_api/__init__.py
+-rw-r--r--   0        0        0     1123 2024-04-07 06:47:43.759718 cloud_orbit_api-0.1.1/cloud_orbit_api/db_factory.py
+-rw-r--r--   0        0        0     1454 2024-04-07 06:47:43.759718 cloud_orbit_api-0.1.1/cloud_orbit_api/main.py
+-rw-r--r--   0        0        0       90 2024-04-07 06:47:43.759718 cloud_orbit_api-0.1.1/cloud_orbit_api/models.py
+-rw-r--r--   0        0        0      493 2024-04-07 06:47:43.759718 cloud_orbit_api-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 cloud_orbit_api-0.1.1/PKG-INFO
```

### Comparing `cloud_orbit_api-0.1.0/cloud_orbit_api/db_factory.py` & `cloud_orbit_api-0.1.1/cloud_orbit_api/db_factory.py`

 * *Files identical despite different names*

### Comparing `cloud_orbit_api-0.1.0/cloud_orbit_api/main.py` & `cloud_orbit_api-0.1.1/cloud_orbit_api/main.py`

 * *Files identical despite different names*

### Comparing `cloud_orbit_api-0.1.0/PKG-INFO` & `cloud_orbit_api-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: cloud-orbit-api
-Version: 0.1.0
+Version: 0.1.1
 Summary: This a demo project
 Author: sukruth grandhi
 Author-email: sukruthgrandhi@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: fastapi (>=0.110.1,<0.111.0)
-Requires-Dist: passlib[bcrypt] (>=1.7.4,<2.0.0)
-Requires-Dist: python-jose[cryptography] (>=3.3.0,<4.0.0)
-Requires-Dist: python-multipart (>=0.0.9,<0.0.10)
 Requires-Dist: uvicorn[standard] (>=0.29.0,<0.30.0)
 Description-Content-Type: text/markdown
 
 This is demo project.
```

