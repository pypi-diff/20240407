# Comparing `tmp/django-tidb-4.2.3.tar.gz` & `tmp/django-tidb-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tidb-4.2.3.tar", last modified: Tue Oct 24 13:39:39 2023, max compression
+gzip compressed data, was "django-tidb-4.2.4.tar", last modified: Sun Apr  7 06:32:21 2024, max compression
```

## Comparing `django-tidb-4.2.3.tar` & `django-tidb-4.2.4.tar`

### file list

```diff
@@ -1,27 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:39:39.300258 django-tidb-4.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11294 2023-10-24 13:39:29.000000 django-tidb-4.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7510 2023-10-24 13:39:39.296257 django-tidb-4.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2023-10-24 13:39:29.000000 django-tidb-4.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:39:39.292257 django-tidb-4.2.3/django_tidb/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    15470 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/features.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:39:39.296257 django-tidb-4.2.3/django_tidb/fields/
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9238 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2023-10-24 13:39:29.000000 django-tidb-4.2.3/django_tidb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:39:39.296257 django-tidb-4.2.3/django_tidb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7510 2023-10-24 13:39:39.000000 django-tidb-4.2.3/django_tidb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-10-24 13:39:39.000000 django-tidb-4.2.3/django_tidb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 13:39:39.000000 django-tidb-4.2.3/django_tidb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-24 13:39:39.000000 django-tidb-4.2.3/django_tidb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2023-10-24 13:39:29.000000 django-tidb-4.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 13:39:39.300258 django-tidb-4.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 13:39:39.296257 django-tidb-4.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2023-10-24 13:39:29.000000 django-tidb-4.2.3/tests/test_tidb_auto_id_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    14561 2023-10-24 13:39:29.000000 django-tidb-4.2.3/tests/test_tidb_auto_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2023-10-24 13:39:29.000000 django-tidb-4.2.3/tests/test_tidb_ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2023-10-24 13:39:29.000000 django-tidb-4.2.3/tests/test_tidb_explain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.771673 django-tidb-4.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11294 2024-04-07 06:32:17.000000 django-tidb-4.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-04-07 06:32:21.771673 django-tidb-4.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-04-07 06:32:17.000000 django-tidb-4.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.767673 django-tidb-4.2.4/django_tidb/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15470 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/features.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.771673 django-tidb-4.2.4/django_tidb/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/fields/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9238 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-07 06:32:17.000000 django-tidb-4.2.4/django_tidb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 06:32:21.771673 django-tidb-4.2.4/django_tidb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 06:32:21.000000 django-tidb-4.2.4/django_tidb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-07 06:32:17.000000 django-tidb-4.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 06:32:21.771673 django-tidb-4.2.4/setup.cfg
```

### Comparing `django-tidb-4.2.3/LICENSE` & `django-tidb-4.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/PKG-INFO` & `django-tidb-4.2.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tidb
-Version: 4.2.3
+Version: 4.2.4
 Summary: Django backend for TiDB
 Author-email: Xiang Zhang <zhangxiang02@pingcap.com>, Di Wang <wangdi@pingcap.com>
 Project-URL: Homepage, https://github.com/pingcap/tidb
 Project-URL: Bug Reports, https://github.com/pingcap/django-tidb/issues
 Project-URL: Source, https://github.com/pingcap/django-tidb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: vector
+Requires-Dist: numpy~=1.0; extra == "vector"
 
 # TiDB dialect for Django
 
 ![PyPI](https://img.shields.io/pypi/v/django-tidb)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-tidb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/django-tidb)
 [![.github/workflows/ci.yml](https://github.com/pingcap/django-tidb/actions/workflows/ci.yml/badge.svg)](https://github.com/pingcap/django-tidb/actions/workflows/ci.yml)
@@ -84,14 +86,18 @@
     },
 }
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 USE_TZ = False
 SECRET_KEY = 'django_tests_secret_key'
 ```
 
+- [AUTO_RANDOM](#using-auto_random)
+- [AUTO_ID_CACHE](#using-auto_id_cache)
+- [Vector (Beta)](#vector-beta)
+
 ### Using `AUTO_RANDOM`
 
 [`AUTO_RANDOM`](https://docs.pingcap.com/tidb/stable/auto-random) is a feature in TiDB that generates unique IDs for a table automatically. It is similar to `AUTO_INCREMENT`, but it can avoid write hotspot in a single storage node caused by TiDB assigning consecutive IDs. It also have some restrictions, please refer to the [documentation](https://docs.pingcap.com/tidb/stable/auto-random#restrictions).
 
 To use `AUTO_RANDOM` in Django, you can do it by following two ways:
 
 1. Declare globally in `settings.py` as shown below, it will affect all models:
@@ -152,14 +158,63 @@
 ```
 
 But there are some limitations:
 
 - `tidb_auto_id_cache` can only affect the table creation, after that it will be ignored even if you change it.
 - `tidb_auto_id_cache` only affects the `AUTO_INCREMENT` column.
 
+### Vector (Beta)
+
+Now only TiDB Cloud Serverless cluster supports vector data type, see [Integrating Vector Search into TiDB Serverless for AI Applications](https://www.pingcap.com/blog/integrating-vector-search-into-tidb-for-ai-applications/).
+
+`VectorField` is still in beta, and the API may change in the future.
+
+To use `VectorField` in Django, you need to install `django-tidb` with `vector` extra:
+
+```bash
+pip install 'django-tidb[vector]'
+```
+
+Then you can use `VectorField` in your model:
+
+```python
+from django.db import models
+from django_tidb.fields.vector import VectorField
+
+class Test(models.Model):
+    embedding = VectorField(dimensions=3)
+```
+
+#### Create a record
+
+```python
+Test.objects.create(embedding=[1, 2, 3])
+```
+
+#### Get instances with vector field
+
+TiDB Vector support below distance functions:
+
+- `L1Distance`
+- `L2Distance`
+- `CosineDistance`
+- `NegativeInnerProduct`
+
+Get instances with vector field and calculate distance to a given vector:
+
+```python
+Test.objects.annotate(distance=CosineDistance('embedding', [3, 1, 2]))
+```
+
+Get instances with vector field and calculate distance to a given vector, and filter by distance:
+
+```python
+Test.objects.alias(distance=CosineDistance('embedding', [3, 1, 2])).filter(distance__lt=5)
+```
+
 ## Supported versions
 
 - TiDB 4.0 and newer
 - Django 3.2, 4.1 and 4.2
 - Python 3.6 and newer(must match Django's Python version requirement)
 
 ## Test
```

### Comparing `django-tidb-4.2.3/README.md` & `django-tidb-4.2.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -61,14 +61,18 @@
     },
 }
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 USE_TZ = False
 SECRET_KEY = 'django_tests_secret_key'
 ```
 
+- [AUTO_RANDOM](#using-auto_random)
+- [AUTO_ID_CACHE](#using-auto_id_cache)
+- [Vector (Beta)](#vector-beta)
+
 ### Using `AUTO_RANDOM`
 
 [`AUTO_RANDOM`](https://docs.pingcap.com/tidb/stable/auto-random) is a feature in TiDB that generates unique IDs for a table automatically. It is similar to `AUTO_INCREMENT`, but it can avoid write hotspot in a single storage node caused by TiDB assigning consecutive IDs. It also have some restrictions, please refer to the [documentation](https://docs.pingcap.com/tidb/stable/auto-random#restrictions).
 
 To use `AUTO_RANDOM` in Django, you can do it by following two ways:
 
 1. Declare globally in `settings.py` as shown below, it will affect all models:
@@ -129,14 +133,63 @@
 ```
 
 But there are some limitations:
 
 - `tidb_auto_id_cache` can only affect the table creation, after that it will be ignored even if you change it.
 - `tidb_auto_id_cache` only affects the `AUTO_INCREMENT` column.
 
+### Vector (Beta)
+
+Now only TiDB Cloud Serverless cluster supports vector data type, see [Integrating Vector Search into TiDB Serverless for AI Applications](https://www.pingcap.com/blog/integrating-vector-search-into-tidb-for-ai-applications/).
+
+`VectorField` is still in beta, and the API may change in the future.
+
+To use `VectorField` in Django, you need to install `django-tidb` with `vector` extra:
+
+```bash
+pip install 'django-tidb[vector]'
+```
+
+Then you can use `VectorField` in your model:
+
+```python
+from django.db import models
+from django_tidb.fields.vector import VectorField
+
+class Test(models.Model):
+    embedding = VectorField(dimensions=3)
+```
+
+#### Create a record
+
+```python
+Test.objects.create(embedding=[1, 2, 3])
+```
+
+#### Get instances with vector field
+
+TiDB Vector support below distance functions:
+
+- `L1Distance`
+- `L2Distance`
+- `CosineDistance`
+- `NegativeInnerProduct`
+
+Get instances with vector field and calculate distance to a given vector:
+
+```python
+Test.objects.annotate(distance=CosineDistance('embedding', [3, 1, 2]))
+```
+
+Get instances with vector field and calculate distance to a given vector, and filter by distance:
+
+```python
+Test.objects.alias(distance=CosineDistance('embedding', [3, 1, 2])).filter(distance__lt=5)
+```
+
 ## Supported versions
 
 - TiDB 4.0 and newer
 - Django 3.2, 4.1 and 4.2
 - Python 3.6 and newer(must match Django's Python version requirement)
 
 ## Test
```

### Comparing `django-tidb-4.2.3/django_tidb/__init__.py` & `django-tidb-4.2.4/django_tidb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,11 +12,11 @@
 # limitations under the License.
 
 # Check Django compatibility before other imports which may fail if the
 # wrong version of Django is installed.
 
 from .patch import monkey_patch
 
-__version__ = "4.2.3"
+__version__ = "4.2.4"
 
 
 monkey_patch()
```

### Comparing `django-tidb-4.2.3/django_tidb/base.py` & `django-tidb-4.2.4/django_tidb/base.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb/features.py` & `django-tidb-4.2.4/django_tidb/features.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb/fields/__init__.py` & `django-tidb-4.2.4/django_tidb/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb/introspection.py` & `django-tidb-4.2.4/django_tidb/introspection.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb/operations.py` & `django-tidb-4.2.4/django_tidb/operations.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb/patch.py` & `django-tidb-4.2.4/django_tidb/patch.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb/schema.py` & `django-tidb-4.2.4/django_tidb/schema.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb/version.py` & `django-tidb-4.2.4/django_tidb/version.py`

 * *Files identical despite different names*

### Comparing `django-tidb-4.2.3/django_tidb.egg-info/PKG-INFO` & `django-tidb-4.2.4/django_tidb.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tidb
-Version: 4.2.3
+Version: 4.2.4
 Summary: Django backend for TiDB
 Author-email: Xiang Zhang <zhangxiang02@pingcap.com>, Di Wang <wangdi@pingcap.com>
 Project-URL: Homepage, https://github.com/pingcap/tidb
 Project-URL: Bug Reports, https://github.com/pingcap/django-tidb/issues
 Project-URL: Source, https://github.com/pingcap/django-tidb
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
@@ -16,14 +16,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: vector
+Requires-Dist: numpy~=1.0; extra == "vector"
 
 # TiDB dialect for Django
 
 ![PyPI](https://img.shields.io/pypi/v/django-tidb)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-tidb)
 ![PyPI - Downloads](https://img.shields.io/pypi/dw/django-tidb)
 [![.github/workflows/ci.yml](https://github.com/pingcap/django-tidb/actions/workflows/ci.yml/badge.svg)](https://github.com/pingcap/django-tidb/actions/workflows/ci.yml)
@@ -84,14 +86,18 @@
     },
 }
 DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
 USE_TZ = False
 SECRET_KEY = 'django_tests_secret_key'
 ```
 
+- [AUTO_RANDOM](#using-auto_random)
+- [AUTO_ID_CACHE](#using-auto_id_cache)
+- [Vector (Beta)](#vector-beta)
+
 ### Using `AUTO_RANDOM`
 
 [`AUTO_RANDOM`](https://docs.pingcap.com/tidb/stable/auto-random) is a feature in TiDB that generates unique IDs for a table automatically. It is similar to `AUTO_INCREMENT`, but it can avoid write hotspot in a single storage node caused by TiDB assigning consecutive IDs. It also have some restrictions, please refer to the [documentation](https://docs.pingcap.com/tidb/stable/auto-random#restrictions).
 
 To use `AUTO_RANDOM` in Django, you can do it by following two ways:
 
 1. Declare globally in `settings.py` as shown below, it will affect all models:
@@ -152,14 +158,63 @@
 ```
 
 But there are some limitations:
 
 - `tidb_auto_id_cache` can only affect the table creation, after that it will be ignored even if you change it.
 - `tidb_auto_id_cache` only affects the `AUTO_INCREMENT` column.
 
+### Vector (Beta)
+
+Now only TiDB Cloud Serverless cluster supports vector data type, see [Integrating Vector Search into TiDB Serverless for AI Applications](https://www.pingcap.com/blog/integrating-vector-search-into-tidb-for-ai-applications/).
+
+`VectorField` is still in beta, and the API may change in the future.
+
+To use `VectorField` in Django, you need to install `django-tidb` with `vector` extra:
+
+```bash
+pip install 'django-tidb[vector]'
+```
+
+Then you can use `VectorField` in your model:
+
+```python
+from django.db import models
+from django_tidb.fields.vector import VectorField
+
+class Test(models.Model):
+    embedding = VectorField(dimensions=3)
+```
+
+#### Create a record
+
+```python
+Test.objects.create(embedding=[1, 2, 3])
+```
+
+#### Get instances with vector field
+
+TiDB Vector support below distance functions:
+
+- `L1Distance`
+- `L2Distance`
+- `CosineDistance`
+- `NegativeInnerProduct`
+
+Get instances with vector field and calculate distance to a given vector:
+
+```python
+Test.objects.annotate(distance=CosineDistance('embedding', [3, 1, 2]))
+```
+
+Get instances with vector field and calculate distance to a given vector, and filter by distance:
+
+```python
+Test.objects.alias(distance=CosineDistance('embedding', [3, 1, 2])).filter(distance__lt=5)
+```
+
 ## Supported versions
 
 - TiDB 4.0 and newer
 - Django 3.2, 4.1 and 4.2
 - Python 3.6 and newer(must match Django's Python version requirement)
 
 ## Test
```

### Comparing `django-tidb-4.2.3/pyproject.toml` & `django-tidb-4.2.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -27,12 +27,15 @@
 dynamic = ["version"]
 
 [project.urls]
 "Homepage" = "https://github.com/pingcap/tidb"
 "Bug Reports" = "https://github.com/pingcap/django-tidb/issues"
 "Source" = "https://github.com/pingcap/django-tidb"
 
+[project.optional-dependencies]
+vector = ["numpy~=1.0"]
+
 [tool.setuptools]
 packages = ["django_tidb", "django_tidb.fields"]
 
 [tool.setuptools.dynamic]
 version = {attr = "django_tidb.__version__"}
```

