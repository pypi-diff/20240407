# Comparing `tmp/pyfineflow-1.0.7.tar.gz` & `tmp/pyfineflow-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfineflow-1.0.7.tar", last modified: Sat Apr  6 14:33:31 2024, max compression
+gzip compressed data, was "pyfineflow-1.0.8.tar", last modified: Sun Apr  7 14:09:03 2024, max compression
```

## Comparing `pyfineflow-1.0.7.tar` & `pyfineflow-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 14:33:31.206926 pyfineflow-1.0.7/
--rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1142 2024-04-06 14:33:31.205926 pyfineflow-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-06 14:33:31.193572 pyfineflow-1.0.7/pyfineflow/
--rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.0.7/pyfineflow/__init__.py
--rw-rw-rw-   0        0        0    16364 2024-04-06 14:33:16.000000 pyfineflow-1.0.7/pyfineflow/core.py
--rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.0.7/pyfineflow/log_conf.py
--rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.0.7/pyfineflow/schemas.py
--rw-rw-rw-   0        0        0     4111 2024-02-16 03:26:57.000000 pyfineflow-1.0.7/pyfineflow/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-06 14:33:31.203924 pyfineflow-1.0.7/pyfineflow.egg-info/
--rw-rw-rw-   0        0        0     1142 2024-04-06 14:33:31.000000 pyfineflow-1.0.7/pyfineflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2024-04-06 14:33:31.000000 pyfineflow-1.0.7/pyfineflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 14:33:31.000000 pyfineflow-1.0.7/pyfineflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-06 14:33:31.000000 pyfineflow-1.0.7/pyfineflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-06 14:33:31.000000 pyfineflow-1.0.7/pyfineflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-06 14:33:31.206926 pyfineflow-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0      540 2024-04-06 14:33:29.000000 pyfineflow-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/
+-rw-rw-rw-   0        0        0     1086 2024-02-03 16:31:19.000000 pyfineflow-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1142 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 14:09:03.932138 pyfineflow-1.0.8/pyfineflow/
+-rw-rw-rw-   0        0        0        0 2024-01-18 17:00:18.000000 pyfineflow-1.0.8/pyfineflow/__init__.py
+-rw-rw-rw-   0        0        0    16364 2024-04-06 14:33:16.000000 pyfineflow-1.0.8/pyfineflow/core.py
+-rw-rw-rw-   0        0        0     1222 2024-01-18 17:00:18.000000 pyfineflow-1.0.8/pyfineflow/log_conf.py
+-rw-rw-rw-   0        0        0     3449 2024-01-18 17:00:18.000000 pyfineflow-1.0.8/pyfineflow/schemas.py
+-rw-rw-rw-   0        0        0     4171 2024-04-07 14:08:33.000000 pyfineflow-1.0.8/pyfineflow/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/pyfineflow.egg-info/
+-rw-rw-rw-   0        0        0     1142 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-07 14:09:03.000000 pyfineflow-1.0.8/pyfineflow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 14:09:03.947763 pyfineflow-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      540 2024-04-07 14:09:01.000000 pyfineflow-1.0.8/setup.py
```

### Comparing `pyfineflow-1.0.7/LICENSE` & `pyfineflow-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.7/PKG-INFO` & `pyfineflow-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.0.7
+Version: 1.0.8
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
```

### Comparing `pyfineflow-1.0.7/pyfineflow/core.py` & `pyfineflow-1.0.8/pyfineflow/core.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.7/pyfineflow/log_conf.py` & `pyfineflow-1.0.8/pyfineflow/log_conf.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.7/pyfineflow/schemas.py` & `pyfineflow-1.0.8/pyfineflow/schemas.py`

 * *Files identical despite different names*

### Comparing `pyfineflow-1.0.7/pyfineflow/utils.py` & `pyfineflow-1.0.8/pyfineflow/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 def get_md5_hash(input_string):
     md5 = hashlib.md5()
     md5.update(input_string.encode('utf-8'))
     return md5.hexdigest()
 
 
 type_map = {
+    '_empty': 'any',
+    'Any': 'any',
+    'any': 'any',
     'int': 'integer',
     'float': 'float',
     'bool': 'boolean',
     'list': 'list',
     'str': 'string',
     'Enum': 'enum'
```

### Comparing `pyfineflow-1.0.7/pyfineflow.egg-info/PKG-INFO` & `pyfineflow-1.0.8/pyfineflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfineflow
-Version: 1.0.7
+Version: 1.0.8
 Summary: python nodes server for fineflow
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyfineflow
 
 > fineflow的python节点后端
```

### Comparing `pyfineflow-1.0.7/setup.py` & `pyfineflow-1.0.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # --skip-existing 覆盖
 # python setup.py sdist bdist_wheel
 # twine upload dist/* --skip-existing
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='pyfineflow',
-    version='1.0.7',
+    version='1.0.8',
     packages=find_packages(exclude=['__pycache__']),
     description='python nodes server for fineflow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'fastapi',
     ]
```

