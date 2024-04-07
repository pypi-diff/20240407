# Comparing `tmp/pylogrotate-1.0.0.tar.gz` & `tmp/pylogrotate-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylogrotate-1.0.0.tar", last modified: Thu Nov  2 09:18:42 2023, max compression
+gzip compressed data, was "pylogrotate-1.1.0.tar", last modified: Sun Apr  7 06:19:54 2024, max compression
```

## Comparing `pylogrotate-1.0.0.tar` & `pylogrotate-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 cadl       (501) staff       (20)        0 2023-11-02 09:18:42.007905 pylogrotate-1.0.0/
--rw-r--r--   0 cadl       (501) staff       (20)     1067 2017-02-04 02:23:37.000000 pylogrotate-1.0.0/LICENSE
--rw-r--r--   0 cadl       (501) staff       (20)     1011 2023-11-02 09:18:42.007618 pylogrotate-1.0.0/PKG-INFO
--rw-r--r--   0 cadl       (501) staff       (20)      956 2023-11-02 08:19:55.000000 pylogrotate-1.0.0/README.md
-drwxr-xr-x   0 cadl       (501) staff       (20)        0 2023-11-02 09:18:42.005549 pylogrotate-1.0.0/pylogrotate/
--rw-r--r--   0 cadl       (501) staff       (20)        0 2017-02-04 02:23:37.000000 pylogrotate-1.0.0/pylogrotate/__init__.py
--rw-r--r--   0 cadl       (501) staff       (20)     7432 2023-11-02 08:44:07.000000 pylogrotate-1.0.0/pylogrotate/main.py
-drwxr-xr-x   0 cadl       (501) staff       (20)        0 2023-11-02 09:18:42.006769 pylogrotate-1.0.0/pylogrotate.egg-info/
--rw-r--r--   0 cadl       (501) staff       (20)     1011 2023-11-02 09:18:41.000000 pylogrotate-1.0.0/pylogrotate.egg-info/PKG-INFO
--rw-r--r--   0 cadl       (501) staff       (20)      308 2023-11-02 09:18:42.000000 pylogrotate-1.0.0/pylogrotate.egg-info/SOURCES.txt
--rw-r--r--   0 cadl       (501) staff       (20)        1 2023-11-02 09:18:41.000000 pylogrotate-1.0.0/pylogrotate.egg-info/dependency_links.txt
--rw-r--r--   0 cadl       (501) staff       (20)       54 2023-11-02 09:18:41.000000 pylogrotate-1.0.0/pylogrotate.egg-info/entry_points.txt
--rw-r--r--   0 cadl       (501) staff       (20)       44 2023-11-02 09:18:41.000000 pylogrotate-1.0.0/pylogrotate.egg-info/requires.txt
--rw-r--r--   0 cadl       (501) staff       (20)       12 2023-11-02 09:18:41.000000 pylogrotate-1.0.0/pylogrotate.egg-info/top_level.txt
--rw-r--r--   0 cadl       (501) staff       (20)       38 2023-11-02 09:18:42.007971 pylogrotate-1.0.0/setup.cfg
--rw-r--r--   0 cadl       (501) staff       (20)     1241 2023-11-02 09:17:11.000000 pylogrotate-1.0.0/setup.py
-drwxr-xr-x   0 cadl       (501) staff       (20)        0 2023-11-02 09:18:42.006929 pylogrotate-1.0.0/tests/
--rw-r--r--   0 cadl       (501) staff       (20)     2720 2023-11-02 09:12:19.000000 pylogrotate-1.0.0/tests/test_pylogrotate.py
+drwxr-xr-x   0 cadl       (501) staff       (20)        0 2024-04-07 06:19:54.550233 pylogrotate-1.1.0/
+-rw-r--r--   0 cadl       (501) staff       (20)     1067 2017-02-04 02:23:37.000000 pylogrotate-1.1.0/LICENSE
+-rw-r--r--   0 cadl       (501) staff       (20)     1053 2024-04-07 06:19:54.550011 pylogrotate-1.1.0/PKG-INFO
+-rw-r--r--   0 cadl       (501) staff       (20)      956 2023-11-02 08:19:55.000000 pylogrotate-1.1.0/README.md
+drwxr-xr-x   0 cadl       (501) staff       (20)        0 2024-04-07 06:19:54.548094 pylogrotate-1.1.0/pylogrotate/
+-rw-r--r--   0 cadl       (501) staff       (20)        0 2017-02-04 02:23:37.000000 pylogrotate-1.1.0/pylogrotate/__init__.py
+-rw-r--r--   0 cadl       (501) staff       (20)     7905 2024-04-07 06:18:15.000000 pylogrotate-1.1.0/pylogrotate/main.py
+drwxr-xr-x   0 cadl       (501) staff       (20)        0 2024-04-07 06:19:54.549498 pylogrotate-1.1.0/pylogrotate.egg-info/
+-rw-r--r--   0 cadl       (501) staff       (20)     1053 2024-04-07 06:19:54.000000 pylogrotate-1.1.0/pylogrotate.egg-info/PKG-INFO
+-rw-r--r--   0 cadl       (501) staff       (20)      308 2024-04-07 06:19:54.000000 pylogrotate-1.1.0/pylogrotate.egg-info/SOURCES.txt
+-rw-r--r--   0 cadl       (501) staff       (20)        1 2024-04-07 06:19:54.000000 pylogrotate-1.1.0/pylogrotate.egg-info/dependency_links.txt
+-rw-r--r--   0 cadl       (501) staff       (20)       54 2024-04-07 06:19:54.000000 pylogrotate-1.1.0/pylogrotate.egg-info/entry_points.txt
+-rw-r--r--   0 cadl       (501) staff       (20)       54 2024-04-07 06:19:54.000000 pylogrotate-1.1.0/pylogrotate.egg-info/requires.txt
+-rw-r--r--   0 cadl       (501) staff       (20)       12 2024-04-07 06:19:54.000000 pylogrotate-1.1.0/pylogrotate.egg-info/top_level.txt
+-rw-r--r--   0 cadl       (501) staff       (20)       38 2024-04-07 06:19:54.550285 pylogrotate-1.1.0/setup.cfg
+-rw-r--r--   0 cadl       (501) staff       (20)     1254 2024-04-07 06:18:26.000000 pylogrotate-1.1.0/setup.py
+drwxr-xr-x   0 cadl       (501) staff       (20)        0 2024-04-07 06:19:54.549195 pylogrotate-1.1.0/tests/
+-rw-r--r--   0 cadl       (501) staff       (20)     4013 2024-04-07 06:18:15.000000 pylogrotate-1.1.0/tests/test_pylogrotate.py
```

### Comparing `pylogrotate-1.0.0/LICENSE` & `pylogrotate-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylogrotate-1.0.0/PKG-INFO` & `pylogrotate-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogrotate
-Version: 1.0.0
+Version: 1.1.0
 Summary: Logrotate in Python
 Home-page: https://github.com/xiachufang/pylogrotate
 Author: gfreezy
 Author-email: gfreezy@gmail.com
 License: MIT
 Keywords: logrotate
 Classifier: Development Status :: 3 - Alpha
@@ -22,7 +22,8 @@
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: hdfs
 Requires-Dist: pqueue
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: freezegun; extra == "test"
+Requires-Dist: zstandard; extra == "test"
```

### Comparing `pylogrotate-1.0.0/README.md` & `pylogrotate-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pylogrotate-1.0.0/pylogrotate/main.py` & `pylogrotate-1.1.0/pylogrotate/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 DEFAULT_CONFIG = {
     'paths': [],
     'mode': '0o644',
     'user': 'root',
     'group': 'root',
     # 'rotate': 7,
     'compress': True,
+    'compressalgorithm': 'gzip',
     'copy': [],
     'copytohdfs': [],
     'hdfs': {},
     'dateformat': '%Y%m%d',
     'destext': 'rotates/%Y%m/%d',
     'fnformat': '{logname}-{timestamp}',
     'sharedscripts': True,
@@ -101,26 +102,33 @@
 
 def gzip(path):
     if not path:
         return
     run('gzip -kf {}'.format(path))
 
 
+def zstd(path):
+    if not path:
+        return
+    run('zstd -kf {}'.format(path))
+
+
 class Rotator(object):
 
     def __init__(self, config):
         self.paths = config['paths']
 
         self.mode = int(config['mode'], 8)
         self.user = config['user']
         self.group = config['group']
 
         # FIXME: Handle rotated files keeping correctly
         # self.keep_files = int(config['rotate'])
         self.compress = config['compress']
+        self.compress_algorithm = config['compressalgorithm']
 
         self.copy = config['copy']
         self.copytohdfs = config['copytohdfs']
         self.hdfs_config = config['hdfs']
         self.hdfs_client = None
         if self.hdfs_config:
             self.hdfs_client = hdfs.InsecureClient(**self.hdfs_config)
@@ -168,16 +176,22 @@
         self.queue.put((path, dest_path), timeout=self.queue_block_timeout)
 
         os.chmod(dest_path, self.mode)
         chown(dest_path, self.user, self.group)
         return dest_path
 
     def compress_file(self, dest_path):
-        gzip(dest_path)
-        return '{}.gz'.format(dest_path)
+        if self.compress_algorithm == 'gzip':
+            gzip(dest_path)
+            return '{}.gz'.format(dest_path)
+        elif self.compress_algorithm == 'zstd':
+            zstd(dest_path)
+            return '{}.zst'.format(dest_path)
+        else:
+            raise ValueError('Unsupported compression algorithm: {}'.format(self.compress_algorithm))
 
     def _copy_file(self, path, from_, to):
         if not to:
             return
         dest = os.path.normpath(path.replace(from_, to))
         dest_dir = os.path.dirname(dest)
         if not os.path.exists(dest_dir):
```

### Comparing `pylogrotate-1.0.0/pylogrotate.egg-info/PKG-INFO` & `pylogrotate-1.1.0/pylogrotate.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylogrotate
-Version: 1.0.0
+Version: 1.1.0
 Summary: Logrotate in Python
 Home-page: https://github.com/xiachufang/pylogrotate
 Author: gfreezy
 Author-email: gfreezy@gmail.com
 License: MIT
 Keywords: logrotate
 Classifier: Development Status :: 3 - Alpha
@@ -22,7 +22,8 @@
 License-File: LICENSE
 Requires-Dist: pyyaml
 Requires-Dist: hdfs
 Requires-Dist: pqueue
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: freezegun; extra == "test"
+Requires-Dist: zstandard; extra == "test"
```

### Comparing `pylogrotate-1.0.0/setup.py` & `pylogrotate-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 
 install_requires = ['pyyaml', 'hdfs', 'pqueue']
 
 
 setup(
     name='pylogrotate',
-    version='1.0.0',
+    version='1.1.0',
     description='Logrotate in Python',
     author='gfreezy',
     author_email='gfreezy@gmail.com',
     url='https://github.com/xiachufang/pylogrotate',
     packages=find_packages(exclude=['contrib', 'docs', 'tests*']),
     install_requires=install_requires,
-    extras_require=dict(test=['pytest', 'freezegun']),
+    extras_require=dict(test=['pytest', 'freezegun', 'zstandard']),
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: Chinese (Simplified)',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `pylogrotate-1.0.0/tests/test_pylogrotate.py` & `pylogrotate-1.1.0/tests/test_pylogrotate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # coding: utf-8
 
 import grp
 import gzip
+import zstandard
 import io
 import os
 import pwd
 import socket
 
 import pytest
 import freezegun
@@ -79,14 +80,55 @@
     assert len(tmpdir.join('nginx').listdir()) == 1
 
     rf = _traverse(tmpdir.join('nginx'))
     with gzip.open(str(rf)) as rf:
         assert rf.read() == content
 
 
+def test_compress_gzip(tmpdir):
+    content = b'This log file should be compressed.'
+
+    f = tmpdir.mkdir('nginx').join('access.rotate-this.log')
+    f.write(content)
+
+    assert f.exists()
+    assert len(tmpdir.join('nginx').listdir()) == 1
+    rotator = Rotator(get_config(paths=[str(f)], compress=True, compressalgorithm='gzip'))
+    rotator.rotate()
+
+    # `f` compressed and moved into `*-rotate/` directory
+    assert not f.exists()
+    assert len(tmpdir.join('nginx').listdir()) == 1
+
+    rf = _traverse(tmpdir.join('nginx'))
+    with gzip.open(str(rf)) as rf:
+        assert rf.read() == content
+
+
+def test_compress_zstd(tmpdir):
+    content = b'This log file should be compressed.'
+
+    f = tmpdir.mkdir('nginx').join('access.rotate-this.log')
+    f.write(content)
+
+    assert f.exists()
+    assert len(tmpdir.join('nginx').listdir()) == 1
+    rotator = Rotator(get_config(paths=[str(f)], compress=True, compressalgorithm='zstd'))
+    rotator.rotate()
+
+    # `f` compressed and moved into `*-rotate/` directory
+    assert not f.exists()
+    assert len(tmpdir.join('nginx').listdir()) == 1
+
+    rf = _traverse(tmpdir.join('nginx'))
+    with open(str(rf), 'rb') as rf:
+        dctx = zstandard.ZstdDecompressor()
+        assert dctx.decompress(rf.read()) == content
+
+
 def test_skip_empty_files(tmpdir):
     f = tmpdir.mkdir('nginx').join('access.skip-empty.log')
     f.write('')
 
     # `f` exists and is the only file in `nginx/` directory
     assert f.exists()
     assert len(tmpdir.join('nginx').listdir()) == 1
```

