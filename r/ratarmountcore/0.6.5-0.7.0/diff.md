# Comparing `tmp/ratarmountcore-0.6.5.tar.gz` & `tmp/ratarmountcore-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratarmountcore-0.6.5.tar", last modified: Sat Apr  6 16:58:02 2024, max compression
+gzip compressed data, was "ratarmountcore-0.7.0.tar", last modified: Sun Apr  7 13:35:31 2024, max compression
```

## Comparing `ratarmountcore-0.6.5.tar` & `ratarmountcore-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.998101 ratarmountcore-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-06 16:58:01.998101 ratarmountcore-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.990101 ratarmountcore-0.6.5/ratarmountcore/
--rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/AutoMountLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12753 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/BlockParallelReaders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/FileVersionLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/FolderMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/MountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/ProgressBar.py
--rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/RarMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SQLiteBlobFile.py
--rw-r--r--   0 runner    (1001) docker     (127)    51490 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SQLiteIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)    78477 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SQLiteIndexedTar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SingleFileMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/StenciledFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/SubvolumesMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/UnionMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12292 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/ZipMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3045 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11682 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/compressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     9381 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/ratarmountcore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.994101 ratarmountcore-0.6.5/ratarmountcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 16:58:01.000000 ratarmountcore-0.6.5/ratarmountcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-06 16:58:01.998101 ratarmountcore-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 16:58:01.994101 ratarmountcore-0.6.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_AutoMountLayer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_BlockParallelReaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_RarMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SQLiteBlobFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SQLiteIndex.py
--rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SQLiteIndexedTar.py
--rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_StenciledFile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_SubvolumesMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_UnionMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_ZipMountSource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_compressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-06 16:57:51.000000 ratarmountcore-0.6.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.718862 ratarmountcore-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-07 13:35:31.718862 ratarmountcore-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.710862 ratarmountcore-0.7.0/ratarmountcore/
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/AutoMountLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12839 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/BlockParallelReaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/FileVersionLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5508 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/FolderMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29124 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/LibarchiveMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/MountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/ProgressBar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9312 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/RarMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SQLiteBlobFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57126 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SQLiteIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78386 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SQLiteIndexedTar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SingleFileMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/StenciledFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/SubvolumesMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9425 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/UnionMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13363 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/ZipMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20325 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/compressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/ratarmountcore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.714861 ratarmountcore-0.7.0/ratarmountcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-07 13:35:31.000000 ratarmountcore-0.7.0/ratarmountcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-07 13:35:31.718862 ratarmountcore-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 13:35:31.714861 ratarmountcore-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7049 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_AutoMountLayer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11698 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_BlockParallelReaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_LibarchiveMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_RarMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SQLiteBlobFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SQLiteIndex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22938 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SQLiteIndexedTar.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10296 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_StenciledFile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8765 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_SubvolumesMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_UnionMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_ZipMountSource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3625 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_compressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6547 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6834 2024-04-07 13:35:21.000000 ratarmountcore-0.7.0/tests/test_utils.py
```

### Comparing `ratarmountcore-0.6.5/LICENSE` & `ratarmountcore-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/PKG-INFO` & `ratarmountcore-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratarmountcore
-Version: 0.6.5
+Version: 0.7.0
 Summary: Random Access Read-Only Tar Mount Library
 Home-page: https://github.com/mxmlnkn/ratarmount/ratarmountcore
 Author: Maximilian Knespel
 Author-email: mxmlnkn@github.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
@@ -24,33 +24,35 @@
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses; python_version < "3.7.0"
 Requires-Dist: importlib-metadata; python_version < "3.8.0"
 Provides-Extra: full
-Requires-Dist: indexed_bzip2<2.0,>=1.3.1; extra == "full"
 Requires-Dist: indexed_gzip<2.0,>=1.6.3; extra == "full"
 Requires-Dist: indexed_zstd<2.0,>=1.3.1; sys_platform == "darwin" and extra == "full"
 Requires-Dist: indexed_zstd<2.0,>=1.2.2; platform_system != "Windows" and extra == "full"
+Requires-Dist: libarchive-c<6.0,~=5.1; extra == "full"
 Requires-Dist: python-xz~=0.4.0; extra == "full"
-Requires-Dist: rapidgzip>=0.10.0; extra == "full"
+Requires-Dist: rapidgzip>=0.13.1; extra == "full"
 Requires-Dist: rarfile~=4.0; extra == "full"
 Provides-Extra: bzip2
-Requires-Dist: indexed_bzip2<2.0,>=1.3.1; extra == "bzip2"
+Requires-Dist: rapidgzip>=0.13.1; extra == "bzip2"
 Provides-Extra: gzip
 Requires-Dist: indexed_gzip<2.0,>=1.6.3; extra == "gzip"
 Provides-Extra: rar
 Requires-Dist: rarfile~=4.0; extra == "rar"
 Provides-Extra: xz
 Requires-Dist: python-xz~=0.4.0; extra == "xz"
 Provides-Extra: zip
 Provides-Extra: zstd
 Requires-Dist: indexed_zstd<2.0,>=1.3.1; sys_platform == "darwin" and extra == "zstd"
 Requires-Dist: indexed_zstd<2.0,>=1.2.2; platform_system != "Windows" and extra == "zstd"
+Provides-Extra: 7z
+Requires-Dist: libarchive-c<6.0,~=5.1; extra == "7z"
 
 # Random Access Read-Only Tar Mount (Ratarmount) Library
 
 [![PyPI version](https://badge.fury.io/py/ratarmountcore.svg)](https://badge.fury.io/py/ratarmountcore)
 [![Python Version](https://img.shields.io/pypi/pyversions/ratarmountcore)](https://pypi.org/project/ratarmountcore/)
 [![Downloads](https://static.pepy.tech/badge/ratarmountcore/month)](https://pepy.tech/project/ratarmountcore)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
```

### Comparing `ratarmountcore-0.6.5/README.md` & `ratarmountcore-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/AutoMountLayer.py` & `ratarmountcore-0.7.0/ratarmountcore/AutoMountLayer.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/BlockParallelReaders.py` & `ratarmountcore-0.7.0/ratarmountcore/BlockParallelReaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,14 +282,15 @@
         ParallelXZReader._tryOpenGlobalFile(filename)
 
     @staticmethod
     def _tryOpenGlobalFile(filename):
         # This is not thread-safe! But it will be executed in a process pool, in which each worker has its own
         # global variable set. Using a global variable for this is safe because we know that there is one process pool
         # per BlockParallelReader, meaning the filename is a constant for each worker.
+        # pylint: disable=global-statement
         global _parallelXzReaderFile
         if _parallelXzReaderFile is None:
             _parallelXzReaderFile = xz.open(filename, 'rb')
 
     @staticmethod
     def _decodeBlock(filename, offset, size):
         ParallelXZReader._tryOpenGlobalFile(filename)
@@ -312,14 +313,15 @@
         super().__init__(filename, fileObject, blockBoundaries, parallelization)
 
     @staticmethod
     def _decodeBlock(filename, offset, size):
         # This is not thread-safe! But it will be executed in a process pool, in which each worker has its own
         # global variable set. Using a global variable for this is safe because we know that there is one process pool
         # per BlockParallelReader, meaning the filename is a constant for each worker.
+        # pylint: disable=global-statement
         global _parallelZstdReaderFile
         if _parallelZstdReaderFile is None:
             _parallelZstdReaderFile = indexed_zstd.IndexedZstdFile(filename)
 
         _parallelZstdReaderFile.seek(offset)
         return _parallelZstdReaderFile.read(size)
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore/FileVersionLayer.py` & `ratarmountcore-0.7.0/ratarmountcore/FileVersionLayer.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/FolderMountSource.py` & `ratarmountcore-0.7.0/ratarmountcore/FolderMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/MountSource.py` & `ratarmountcore-0.7.0/ratarmountcore/MountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/ProgressBar.py` & `ratarmountcore-0.7.0/ratarmountcore/ProgressBar.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/RarMountSource.py` & `ratarmountcore-0.7.0/ratarmountcore/RarMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/SQLiteBlobFile.py` & `ratarmountcore-0.7.0/ratarmountcore/SQLiteBlobFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/SQLiteIndex.py` & `ratarmountcore-0.7.0/ratarmountcore/SQLiteIndex.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import stat
 import sys
 import tarfile
 import time
 import traceback
 import urllib.parse
 
-from typing import Any, AnyStr, Callable, Dict, IO, List, Optional, Tuple
+from typing import Any, AnyStr, Callable, Dict, IO, List, Optional, Tuple, Union
 from dataclasses import dataclass
 
 try:
     import indexed_gzip
 except ImportError:
     pass
 
@@ -25,15 +25,15 @@
 except ImportError:
     pass
 
 from .version import __version__
 from .MountSource import FileInfo, createRootFileInfo
 from .compressions import TAR_COMPRESSION_FORMATS
 from .SQLiteBlobFile import SQLiteBlobsFile, WriteSQLiteBlobs
-from .utils import RatarmountError, IndexNotOpenError, InvalidIndexError, findModuleVersion
+from .utils import RatarmountError, IndexNotOpenError, InvalidIndexError, findModuleVersion, MismatchingIndexError
 
 
 def getSqliteTables(connection: sqlite3.Connection):
     return [x[0] for x in connection.execute('SELECT name FROM sqlite_master WHERE type="table"')]
 
 
 def _toVersionTuple(version: str) -> Optional[Tuple[int, int, int]]:
@@ -63,27 +63,36 @@
     #   - Initial version
     # Version 0.2.0:
     #   - Add sparse support and 'offsetheader' and 'issparse' columns to the SQLite database
     #   - Add TAR file size metadata in order to quickly check whether the TAR changed
     #   - Add 'offsetheader' to the primary key of the 'files' table so that files which were
     #     updated in the TAR can still be accessed if necessary.
     # Version 0.3.0:
-    #   - Add arguments influencing the created index to metadata (ignore-zeros, recursive, ...)
+    #   - Add arguments influencing the created index to 'metadata' table (ignore-zeros, recursive, ...)
     # Version 0.4.0:
-    #   - Added 'gzipindexes' table, which may contain multiple blobs in contrast to 'gzipindex' table.
-    __version__ = '0.4.0'
+    #   - Add 'gzipindexes' table, which may contain multiple blobs in contrast to 'gzipindex' table.
+    # Version 0.5.0:
+    #   - Add 'backend' name to 'metadata' table. Indexes created by different backends should by default
+    #     be assumed to be incompatible, especially for chimera files, but also when one was created with
+    #     libarchive, then it will not be readable with the SQLiteIndexedTar backend because it does not
+    #     collect data offsets.
+    #   - Add 'isGnuIncremental' to 'metadata' table.
+    __version__ = '0.5.0'
 
     NUMBER_OF_METADATA_TO_VERIFY = 1000  # shouldn't take more than 1 second according to benchmarks
 
     # The maximum blob size configured by SQLite is exactly 1 GB, see https://www.sqlite.org/limits.html
     # Therefore, this should be smaller. Another argument for making it smaller is that this blob size
     # will be held fully in memory temporarily.
     # But, making it too small would result in too many non-backwards compatible indexes being created.
     _MAX_BLOB_SIZE = 256 * 1024 * 1024  # 256 MiB
 
+    # TODO Would be nice for index verification to have columns for recursionlevel (INTEGER) and isgenerated (BOOL)
+    #      that is true for automatically inserted parent folders that do not actually exist in the archive.
+    #      How version compatible would that table change be? Test with old ratarmount versions.
     _CREATE_FILES_TABLE = """
         CREATE TABLE "files" (
             "path"          VARCHAR(65535) NOT NULL,  /* path with leading and without trailing slash */
             "name"          VARCHAR(65535) NOT NULL,
             "offsetheader"  INTEGER,  /* seek offset from TAR file where the TAR metadata for this file resides */
             "offset"        INTEGER,  /* seek offset from TAR file where these file's contents resides */
             "size"          INTEGER,
@@ -116,15 +125,16 @@
             "offsetheader"  INTEGER,
             "offset"        INTEGER,
             PRIMARY KEY (path,name)
             UNIQUE (path,name)
         );"""
 
     _CREATE_METADATA_TABLE = """
-        /* Empty table whose sole existence specifies that the archive has been fully processed. */
+        /* Empty table whose sole existence specifies that the archive has been fully processed.
+         * Common keys: tarstats, arguments, isGnuIncremental, backendName */
         CREATE TABLE IF NOT EXISTS "metadata" (
             "key"      VARCHAR(65535) NOT NULL, /* e.g. "tarsize" */
             "value"    VARCHAR(65535) NOT NULL  /* e.g. size in bytes as integer */
         );
     """
 
     _CREATE_VERSIONS_TABLE = """
@@ -140,26 +150,43 @@
             "minor"    INTEGER,
             "patch"    INTEGER
         );
     """
 
     # Check some of the first and last files in the archive and some random selection in between.
     # Do not verify folders because parent folders and root get automatically added!
-    FROM_REGULAR_FILES = f"""FROM "files" WHERE (mode & {stat.S_IFREG}) != 0"""
+    # Ignore rows with isTar=True because recomputing this would require trying an expensive recursive mount.
+    # We cannot simply ignore rows with NOT isTar because there will be multiple entries with the same
+    # offset header for those recursive entries.
+    # We also need to ignore all rows for recursive entries because they will have the parent TAR path prepended,
+    # which the error check code is not expecting.
+    # This check is done by creating a subquery/table that gathers all recursive archives (isTar==True) that
+    # enclose the current rows offset. If there is no such archive, then the current row is non-recursive
+    # and safe to check. Unfortunately, it seems that this is quadratic in complexity and basically hangs for
+    # larger files.
+    # FROM "files" AS t1 WHERE (mode & {stat.S_IFREG}) != 0 AND NOT EXISTS (
+    #     SELECT 1 FROM "files" AS t2 WHERE isTar AND t1.offsetheader BETWEEN t2.offset AND t2.offset + t2.size - 1
+    # )
+    # As an alternative, exempt the path from the consistency check.
+    # Note also that for pure compressed files such as simple.bz2, the offsetheader can be None.
+    # These rows should also be filtered.
+    FROM_REGULAR_FILES = f"""FROM "files" WHERE (mode & {stat.S_IFREG}) != 0 AND offsetheader IS NOT NULL"""
 
     def __init__(
         self,
         indexFilePath: Optional[str],
         indexFolders: Optional[List[str]] = None,
         archiveFilePath: Optional[str] = None,
+        *,  # force all parameters after to be keyword-only
         encoding: str = tarfile.ENCODING,
         checkMetadata: Optional[Callable[[Dict[str, Any]], None]] = None,
         printDebug: int = 0,
         preferMemory: bool = False,
         indexMinimumFileCount: int = 0,
+        backendName: str = '',
     ):
         """
         indexFilePath
             Path to the index file. This takes precedence over defaultIndexFilePath.
             If it is ':memory:', then the SQLite database will be kept in memory
             and not stored to the file system at any point.
         indexFolders
@@ -173,31 +200,39 @@
         preferMemory
             If True, then load existing indexes and write to explicitly given index file paths but
             if no such things are given, then create the new index in memory as if indexFilePath
             = ':memory:' was specified.
         indexMinimumFileCount
             If > 0, then open new databases in memory and write them out if this threshold has been
             exceeded. It may also be written to a file if a gzip index is stored.
+        backendName
+            The backend name to be stored as metadata and to determine compatibility of found indexes.
         """
 
+        if not backendName:
+            raise ValueError("A non-empty backend name must be specified!")
+
         self.printDebug = printDebug
         self.sqlConnection: Optional[sqlite3.Connection] = None
         # Will hold the actually opened valid path to an index file
         self.indexFilePath: Optional[str] = None
         self.encoding = encoding
         self.possibleIndexFilePaths = SQLiteIndex.getPossibleIndexFilePaths(
             indexFilePath, indexFolders, archiveFilePath
         )
         # stores which parent folders were last tried to add to database and therefore do exist
         self.parentFolderCache: List[Tuple[str, str]] = []
         self.checkMetadata = checkMetadata
         self.preferMemory = preferMemory
         self.indexMinimumFileCount = indexMinimumFileCount
+        self.backendName = backendName
         self._insertedRowCount = 0
 
+        assert self.backendName
+
         # Ignore minimum file count option if an index file path or index folder is configured.
         # For latter, ignore the special empty folder [''], which means that the indexes are stored
         # besides the archives.
         # Why all this exceptions? Because the index-minimum-file-count, which is set by default,
         # is only intended to avoid littering folders with index files in the common use case of mounting
         # a folder of archives or single small archives recursively. If the user goes through the trouble
         # of specifying an index file or folder, then littering should not be a problem as index creations
@@ -243,28 +278,28 @@
         """Tries to find an already existing index."""
         for indexPath in self.possibleIndexFilePaths:
             if self._tryLoadIndex(indexPath):
                 self.indexFilePath = indexPath
                 break
 
     def openInMemory(self):
-        self._openPath(':memory:')
+        self.indexFilePath, self.sqlConnection = SQLiteIndex._openPath(':memory:')
 
     def openWritable(self):
         if self.possibleIndexFilePaths and not self.preferMemory:
             for indexPath in self.possibleIndexFilePaths:
                 if SQLiteIndex._pathIsWritable(
                     indexPath, printDebug=self.printDebug
                 ) and SQLiteIndex._pathCanBeUsedForSqlite(indexPath, printDebug=self.printDebug):
-                    self._openPath(indexPath)
+                    self.indexFilePath, self.sqlConnection = SQLiteIndex._openPath(indexPath)
                     break
         else:
             if self.printDebug >= 3 and self.preferMemory:
                 print("[Info] Create new index in memory because memory is to be preferred, e.g., for small archives.")
-            self._openPath(':memory:')
+            self.indexFilePath, self.sqlConnection = SQLiteIndex._openPath(':memory:')
 
         if not self.indexIsLoaded():
             raise InvalidIndexError(
                 "Could not find any existing index or writable location for an index in "
                 + str(self.possibleIndexFilePaths)
             )
 
@@ -332,59 +367,85 @@
             if self.printDebug >= 2:
                 print(exception)
             if self.printDebug >= 3:
                 traceback.print_exc()
 
     def _storeFileMetadata(self, filePath: AnyStr) -> None:
         """Adds some consistency meta information to recognize the need to update the cached TAR index"""
-
-        connection = self.getConnection()
-
         try:
             tarStats = os.stat(filePath)
             serializedTarStats = json.dumps(
                 {attr: getattr(tarStats, attr) for attr in dir(tarStats) if attr.startswith('st_')}
             )
-            connection.execute('INSERT INTO "metadata" VALUES (?,?)', ("tarstats", serializedTarStats))
+            self.storeMetadataKeyValue("tarstats", serializedTarStats)
         except Exception as exception:
             print("[Warning] There was an error when adding file metadata.")
             print("[Warning] Automatic detection of changed TAR files during index loading might not work.")
             if self.printDebug >= 2:
                 print(exception)
             if self.printDebug >= 3:
                 traceback.print_exc()
 
-    def storeMetadata(self, metadata: AnyStr, filePath: Optional[AnyStr] = None) -> None:
+    def storeMetadataKeyValue(self, key: AnyStr, value: Union[str, bytes]) -> None:
         connection = self.getConnection()
-
-        self._storeVersionsMetadata()
-
         connection.executescript(SQLiteIndex._CREATE_METADATA_TABLE)
 
-        if filePath:
-            self._storeFileMetadata(filePath)
-
         try:
-            connection.execute('INSERT INTO "metadata" VALUES (?,?)', ("arguments", metadata))
+            connection.execute('INSERT OR REPLACE INTO "metadata" VALUES (?,?)', (key, value))
         except Exception as exception:
             if self.printDebug >= 2:
                 print(exception)
             print("[Warning] There was an error when adding argument metadata.")
             print("[Warning] Automatic detection of changed arguments files during index loading might not work.")
 
         connection.commit()
 
+    def storeMetadata(self, metadata: AnyStr, filePath: Optional[AnyStr] = None) -> None:
+        self._storeVersionsMetadata()
+        self.storeMetadataKeyValue('backendName', self.backendName)
+        if filePath:
+            self._storeFileMetadata(filePath)
+        self.storeMetadataKeyValue('arguments', metadata)
+        self.storeMetadataKeyValue('backendName', self.backendName)
+
     def dropMetadata(self):
         self.getConnection().executescript(
             """
             DROP TABLE IF EXISTS metadata;
             DROP TABLE IF EXISTS versions;
             """
         )
 
+    @staticmethod
+    def checkMetadataArguments(metadata: Dict, arguments, argumentsToCheck: List[str]):
+        # Check arguments used to create the found index.
+        # These are only warnings and not forcing a rebuild by default.
+        # TODO: Add option to force index rebuild on metadata mismatch?
+        differingArgs = []
+        for arg in argumentsToCheck:
+            if arg in metadata and hasattr(arguments, arg) and metadata[arg] != getattr(arguments, arg):
+                differingArgs.append((arg, metadata[arg], getattr(arguments, arg)))
+        if differingArgs:
+            print("[Warning] The arguments used for creating the found index differ from the arguments ")
+            print("[Warning] given for mounting the archive now. In order to apply these changes, ")
+            print("[Warning] recreate the index using the --recreate-index option!")
+            for arg, oldState, newState in differingArgs:
+                print(f"[Warning] {arg}: index: {oldState}, current: {newState}")
+
+    def checkMetadataBackend(self, metadata: Dict):
+        # Because of a lack of sufficient foresight, the backend name was not added to the index in older verions.
+        backendName = metadata.get('backendName')
+        if isinstance(backendName, str):
+            if backendName != self.backendName:
+                raise MismatchingIndexError(
+                    f"Cannot open an index created with backend '{backendName}'!\n"
+                    f"Will stop trying to open the archive with backend '{self.backendName}'.\n"
+                    f"Use --recreate-index if '{backendName}' is not installed."
+                )
+
     def getIndexVersion(self):
         return self.getConnection().execute("""SELECT version FROM versions WHERE name == 'index';""").fetchone()[0]
 
     @staticmethod
     def _pathIsWritable(path: str, printDebug: int = 0) -> bool:
         try:
             folder = os.path.dirname(path)
@@ -464,27 +525,30 @@
             PRAGMA TEMP_STORE = MEMORY;
             PRAGMA JOURNAL_MODE = OFF;
             PRAGMA SYNCHRONOUS = OFF;
             """
         )
         return sqlConnection
 
-    def _openPath(self, indexFilePath: Optional[str]):
-        self.indexFilePath = indexFilePath if indexFilePath else ':memory:'
+    @staticmethod
+    def _openPath(indexFilePath: Optional[str], printDebug: int = 0) -> Tuple[str, sqlite3.Connection]:
+        indexFilePath = indexFilePath if indexFilePath else ':memory:'
 
-        if self.printDebug >= 1:
-            print("Creating new SQLite index database at", self.indexFilePath)
+        if printDebug >= 1:
+            print("Creating new SQLite index database at", indexFilePath)
 
-        self.sqlConnection = SQLiteIndex._openSqlDb(self.indexFilePath)
-        tables = getSqliteTables(self.sqlConnection)
+        sqlConnection = SQLiteIndex._openSqlDb(indexFilePath)
+        tables = getSqliteTables(sqlConnection)
         if {"files", "filestmp", "parentfolders"}.intersection(tables):
             raise InvalidIndexError(
                 f"The index file {indexFilePath} already seems to contain a table. Please specify --recreate-index."
             )
-        self.sqlConnection.executescript(SQLiteIndex._CREATE_FILES_TABLE)
+        sqlConnection.executescript(SQLiteIndex._CREATE_FILES_TABLE)
+
+        return indexFilePath, sqlConnection
 
     def reloadIndexReadOnly(self):
         if not self.indexFilePath or self.indexFilePath == ':memory:' or not self.sqlConnection:
             return
 
         self.sqlConnection.commit()
         self.sqlConnection.close()
@@ -608,16 +672,28 @@
 
         # For listing directory entries the file version can't be applied meaningfully at this abstraction layer.
         # E.g., should it affect the file version of the directory to list, or should it work on the listed files
         # instead and if so how exactly if there aren't the same versions for all files available, ...?
         # Or, are folders assumed to be overwritten by a new folder entry in a TAR or should they be union mounted?
         # If they should be union mounted, like is the case now, then the folder version only makes sense for
         # its attributes.
+        #
+        # Order by offsetheader in order to preserve the order they appear in the archive to potentially enable
+        # faster access to the whoole archive when iterating over all files in order.
+        # Note that Python's dictionary preserves the insertion order since Python 3.6.
+        # https://docs.python.org/3.6/whatsnew/3.6.html#new-dict-implementation
+        # While it was not a guarantee to stay that way, it is guaranteed for Python 3.7+:
+        # > the insertion-order preservation nature of dict objects has been declared to be an official part of the
+        # > Python language spec.
+        # https://docs.python.org/3.11/library/stdtypes.html#dict.values
+        # > Dictionaries preserve insertion order. Note that updating a key does not affect the order.
+        # > Keys added after deletion are inserted at the end.
         rows = self.getConnection().execute(
-            'SELECT * FROM "files" WHERE "path" == (?)', (self._queryNormpath(path).rstrip('/'),)
+            'SELECT * FROM "files" WHERE "path" == (?) ORDER BY "offsetheader"',
+            (self._queryNormpath(path).rstrip('/'),),
         )
         directory: Dict[str, FileInfo] = {}
         gotResults = False
         for row in rows:
             gotResults = True
             if row['name']:
                 directory[row['name']] = self._rowToFileInfo(row)
@@ -847,14 +923,15 @@
                 print("[Warning] The found outdated index does not contain any sparse file information.")
                 print("[Warning] The index will also miss data about multiple versions of a file.")
                 print("[Warning] Please recreate the index if you have problems with those.")
 
             if 'metadata' in tables:
                 metadata = dict(self.sqlConnection.execute('SELECT * FROM metadata;'))
                 if self.checkMetadata:
+                    self.checkMetadataBackend(metadata)
                     self.checkMetadata(metadata)
 
         except Exception as e:
             # indexIsLoaded checks self.sqlConnection, so close it before returning because it was found to be faulty
             try:
                 self.sqlConnection.close()
             except sqlite3.Error:
@@ -889,14 +966,16 @@
             return True
 
         if not os.path.isfile(indexFilePath):
             return False
 
         try:
             self.loadIndex(indexFilePath)
+        except MismatchingIndexError as e:
+            raise e
         except Exception as exception:
             if self.printDebug >= 3:
                 traceback.print_exc()
 
             print("[Warning] Could not load file:", indexFilePath)
             print("[Info] Exception:", exception)
             print("[Info] Some likely reasons for not being able to load the index file:")
@@ -927,15 +1006,15 @@
 
     def synchronizeCompressionOffsets(self, fileObject: IO[bytes], compression: str):
         """
         Will load block offsets from SQLite database to backend if a fitting table exists.
         Else it will force creation and store the block offsets of the compression backend into a new table.
         """
         if compression and (not self.indexFilePath or self.indexFilePath == ':memory:'):
-            if self.printDebug >= 2:
+            if self.indexMinimumFileCount != 0 and self.printDebug >= 2:
                 print(
                     f"[Info] Will try to reopen the database on disk even though the file count threshold "
                     f"({self.indexMinimumFileCount}) might not be exceeded ({self._insertedRowCount}) because "
                     f"the archive is compressed."
                 )
             self._reloadIndexOnDisk()
 
@@ -982,15 +1061,19 @@
             if table_name in tables:
                 db.execute(f"DROP TABLE {table_name}")
             db.execute(f"CREATE TABLE {table_name} ( blockoffset INTEGER PRIMARY KEY, dataoffset INTEGER )")
             db.executemany(f"INSERT INTO {table_name} VALUES (?,?)", getBlockOffsets().items())
             db.commit()
             return
 
-        if hasattr(fileObject, 'import_index') and hasattr(fileObject, 'export_index') and compression == 'gz':
+        if (
+            hasattr(fileObject, 'import_index')
+            and hasattr(fileObject, 'export_index')
+            and compression in ['gz', 'zlib']
+        ):
             tables = getSqliteTables(db)
 
             if 'gzipindex' in tables or 'gzipindexes' in tables:
                 if self._loadGzipIndex(fileObject, 'gzipindexes' if 'gzipindexes' in tables else 'gzipindex'):
                     return
 
                 if self.printDebug >= 2:
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore/SQLiteIndexedTar.py` & `ratarmountcore-0.7.0/ratarmountcore/SQLiteIndexedTar.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,19 +16,14 @@
 import time
 import traceback
 
 from timeit import default_timer as timer
 from typing import Any, Callable, cast, Dict, Generator, IO, Iterable, List, Optional, Tuple, Union
 
 try:
-    import indexed_bzip2
-except ImportError:
-    pass
-
-try:
     import indexed_gzip
 except ImportError:
     pass
 
 try:
     import rapidgzip
 except ImportError:
@@ -39,15 +34,15 @@
 except ImportError:
     xz = None  # type: ignore
 
 from .MountSource import FileInfo, MountSource
 from .ProgressBar import ProgressBar
 from .SQLiteIndex import SQLiteIndex, SQLiteIndexedTarUserData
 from .StenciledFile import StenciledFile
-from .compressions import findAvailableOpen, getGzipInfo, TAR_COMPRESSION_FORMATS
+from .compressions import detectCompression, findAvailableOpen, getGzipInfo, TAR_COMPRESSION_FORMATS
 from .utils import (
     RatarmountError,
     InvalidIndexError,
     CompressionError,
     ceilDiv,
     isOnSlowDrive,
     overrides,
@@ -179,14 +174,15 @@
         # fmt: off
         tarInfo          : tarfile.TarInfo,
         fileObject       : IO[bytes],
         pathPrefix       : str,
         streamOffset     : int,
         isGnuIncremental : Optional[bool],
         mountRecursively : bool,
+        transform        : Callable[[str], str],
         printDebug       : int,
         # fmt: on
     ) -> Tuple[List[Tuple], bool, Optional[bool]]:
         """Postprocesses a TarInfo object into one or multiple FileInfo tuples."""
 
         if tarInfo.type == b'D' and not isGnuIncremental:
             isGnuIncremental = True
@@ -195,15 +191,18 @@
                 print("[Warning] was encountered but this archive was not automatically recognized as such!")
                 print("[Warning] Please call ratarmount with the --gnu-incremental flag if there are problems.")
                 print()
 
         if isGnuIncremental:
             _TarFileMetadataReader._fixIncrementalBackupNamePrefixes(fileObject, tarInfo, printDebug)
 
-        path, name = SQLiteIndex.normpath(pathPrefix + "/" + tarInfo.name).rsplit("/", 1)
+        fullPath = pathPrefix + "/" + tarInfo.name
+        if tarInfo.isdir():
+            fullPath += "/"
+        path, name = SQLiteIndex.normpath(transform(fullPath)).rsplit("/", 1)
 
         # TODO: As for the tarfile type SQLite expects int but it is generally bytes.
         #       Most of them would be convertible to int like tarfile.SYMTYPE which is b'2',
         #       but others should throw errors, like GNUTYPE_SPARSE which is b'S'.
         #       When looking at the generated index, those values get silently converted to 0?
         # fmt: off
         fileInfo : Tuple = (
@@ -249,14 +248,15 @@
         size             : int,
         pathPrefix       : str,
         streamOffset     : int,
         isGnuIncremental : Optional[bool],
         mountRecursively : bool,
         ignoreZeros      : bool,
         encoding         : str,
+        transform        : Callable[[str], str],
         printDebug       : int,
     ):
         """
         Opens a view of the data range [startOffset, startOffset+size) of the given pathToTar and extracts
         all TAR file metadata and returns it as FileInfo tuples.
         """
 
@@ -278,14 +278,15 @@
                     newFileInfos, mightBeTar, isGnuIncremental = _TarFileMetadataReader._processTarInfo(
                         tarInfo,
                         pathPrefix=pathPrefix,
                         streamOffset=streamOffset + startOffset,
                         fileObject=fileObject,
                         isGnuIncremental=isGnuIncremental,
                         mountRecursively=mountRecursively,
+                        transform=transform,
                         printDebug=printDebug,
                     )
 
                     if mightBeTar:
                         filesToMountRecursively.extend(newFileInfos)
                     else:
                         fileInfos.extend(newFileInfos)
@@ -421,14 +422,15 @@
                             subSize,
                             pathPrefix,
                             streamOffset,
                             self._parent._isGnuIncremental,
                             self._parent.mountRecursively,
                             self._parent.ignoreZeros,
                             self._parent.encoding,
+                            self._parent.transform,
                             self._parent.printDebug,
                         ),
                     )
                 )
 
             if result is None:
                 break
@@ -503,14 +505,15 @@
                 newFileInfos, mightBeTar, self._parent._isGnuIncremental = _TarFileMetadataReader._processTarInfo(
                     tarInfo,
                     fileObject=fileObject,
                     pathPrefix=pathPrefix,
                     streamOffset=streamOffset,
                     isGnuIncremental=self._parent._isGnuIncremental,
                     mountRecursively=self._parent.mountRecursively,
+                    transform=self._parent.transform,
                     printDebug=self._parent.printDebug,
                 )
 
                 if mightBeTar:
                     filesToMountRecursively.extend(newFileInfos)
 
                 fileInfos.extend(newFileInfos)
@@ -585,28 +588,30 @@
     DEFAULT_GZIP_SEEK_POINT_SPACING = 16 * 1024 * 1024
 
     def __init__(
         # fmt: off
         self,
         tarFileName                  : Optional[str]             = None,
         fileObject                   : Optional[IO[bytes]]       = None,
+        *,  # force all parameters after to be keyword-only
         writeIndex                   : bool                      = False,
         clearIndexCache              : bool                      = False,
         indexFilePath                : Optional[str]             = None,
         indexFolders                 : Optional[List[str]]       = None,
         recursive                    : bool                      = False,
         gzipSeekPointSpacing         : int                       = DEFAULT_GZIP_SEEK_POINT_SPACING,
         encoding                     : str                       = tarfile.ENCODING,
         stripRecursiveTarExtension   : bool                      = False,
         ignoreZeros                  : bool                      = False,
         verifyModificationTime       : bool                      = False,
         parallelization              : int                       = 1,
         isGnuIncremental             : Optional[bool]            = None,
         printDebug                   : int                       = 0,
         transformRecursiveMountPoint : Optional[Tuple[str, str]] = None,
+        transform                    : Optional[Tuple[str, str]] = None,
         prioritizedBackends          : Optional[List[str]]       = None,
         indexMinimumFileCount        : int                       = 0,
         # pylint: disable=unused-argument
         **kwargs
         # fmt: on
     ) -> None:
         """
@@ -664,26 +669,34 @@
         """
 
         # fmt: off
         self.mountRecursively             = recursive
         self.encoding                     = encoding
         self.stripRecursiveTarExtension   = stripRecursiveTarExtension
         self.transformRecursiveMountPoint = transformRecursiveMountPoint
+        self.transformPattern             = transform
         self.ignoreZeros                  = ignoreZeros
         self.verifyModificationTime       = verifyModificationTime
         self.gzipSeekPointSpacing         = gzipSeekPointSpacing
         self.parallelization              = parallelization
         self.printDebug                   = printDebug
         self.isFileObject                 = fileObject is not None
         self._isGnuIncremental            = isGnuIncremental
         self.hasBeenAppendedTo            = False
         # fmt: on
         self.prioritizedBackends: List[str] = [] if prioritizedBackends is None else prioritizedBackends
 
-        # Determine an archive file name to show for debug output
+        self.transform = (
+            (lambda x: re.sub(self.transformPattern[0], self.transformPattern[1], x))
+            if isinstance(self.transformPattern, (tuple, list)) and len(self.transformPattern) == 2
+            else (lambda x: x)
+        )
+
+        # Determine an archive file name to show for debug output and as file name inside the mount point for
+        # simple non-TAR gzip/bzip2 stream-compressed files.
         self.tarFileName: str
         if fileObject:
             self.tarFileName = tarFileName if tarFileName else '<file object>'
         else:
             if tarFileName:
                 # Keep the EXACT file path, do not convert to an absolute path, or else we might trigger
                 # recursive FUSE calls, which hangs everything!
@@ -740,44 +753,34 @@
             indexFilePath,
             indexFolders=indexFolders,
             archiveFilePath=None if self.isFileObject else self.tarFileName,
             encoding=self.encoding,
             checkMetadata=self._checkMetadata,
             printDebug=self.printDebug,
             indexMinimumFileCount=indexMinimumFileCount,
+            backendName='SQLiteIndexedTar',
         )
         if clearIndexCache:
             self.index.clearIndexes()
         self.index.openExisting()
 
         if self.index.indexIsLoaded():
             if not self.hasBeenAppendedTo:  # indirectly set by a successful call to _tryLoadIndex
                 self._loadOrStoreCompressionOffsets()  # load
                 self.index.reloadIndexReadOnly()
-                # TODO The value should not matter when an index has been loaded. But maybe write this to the index
-                #      and load it in order to have the correct value without having to do a very costly recheck?
-                self._isGnuIncremental = False
                 return
 
-            # TODO This does and did not work correctly for recursive TARs because the outermost layer will change
-            #      None to a hard value and from then on it would have been fixed to that value even when called
-            #      inside createIndex.
-            # Required for _checkIndexValidity
-            if self._isGnuIncremental is None:
-                self._isGnuIncremental = self._detectGnuIncremental(self.tarFileObject)
-
             # TODO Handling appended files to compressed archives would have to account for dropping the offsets,
             #      seeking to the first appended file while not processing any metadata and still showing a progress
             #      bar as well as saving the block offsets out after reading and possibly other things.
             if self.compression:
                 # When loading compression offsets, the backends assume they are complete, so we have to clear them.
                 self.index.clearCompressionOffsets()
 
-            assert self.index.sqlConnection
-            pastEndOffset = self._getPastEndOffset(self.index.sqlConnection)
+            pastEndOffset = self._getPastEndOffset(self.index.getConnection())
             if not self.compression and pastEndOffset and self._checkIndexValidity():
                 archiveSize = self.tarFileObject.seek(0, io.SEEK_END)
 
                 newShare = (archiveSize - pastEndOffset) / archiveSize
                 print(f"Detected TAR being appended to. Will only analyze the newly added {newShare:.2f} % of data.")
 
                 appendedPartAsFile = StenciledFile(
@@ -871,28 +874,31 @@
     def _storeMetadata(self) -> None:
         argumentsToSave = [
             'mountRecursively',
             'gzipSeekPointSpacing',
             'encoding',
             'stripRecursiveTarExtension',
             'transformRecursiveMountPoint',
+            'transformPattern',
             'ignoreZeros',
         ]
 
         argumentsMetadata = json.dumps({argument: getattr(self, argument) for argument in argumentsToSave})
         self.index.storeMetadata(argumentsMetadata, None if self.isFileObject else self.tarFileName)
+        self.index.storeMetadataKeyValue('isGnuIncremental', '1' if self._isGnuIncremental else '0')
 
     def _updateProgressBar(self, progressBar, fileobj: Any) -> None:
         if not progressBar:
             return
 
         try:
-            if hasattr(fileobj, 'tell_compressed') and (
-                ('indexed_bzip2' in sys.modules and isinstance(fileobj, indexed_bzip2.IndexedBzip2File))  # type: ignore
-                or ('rapidgzip' in sys.modules and isinstance(fileobj, rapidgzip.RapidgzipFile))
+            if (
+                hasattr(fileobj, 'tell_compressed')
+                and 'rapidgzip' in sys.modules
+                and (isinstance(fileobj, rapidgzip.IndexedBzip2File) or isinstance(fileobj, rapidgzip.RapidgzipFile))
             ):
                 # Note that because bz2 works on a bitstream the tell_compressed returns the offset in bits
                 progressBar.update(fileobj.tell_compressed() // 8)
             elif hasattr(fileobj, 'tell_compressed'):
                 progressBar.update(fileobj.tell_compressed())
             elif hasattr(fileobj, 'fileobj') and callable(fileobj.fileobj):
                 progressBar.update(fileobj.fileobj().tell())
@@ -1026,24 +1032,29 @@
         # If no file is in the TAR, then it most likely indicates a possibly compressed non TAR file.
         # In that case add that itself to the file index. This will be ignored when called recursively
         # because the table will at least contain the recursive file to mount itself, i.e., fileCount > 0
         if self.index.fileCount() == 0:
             if self.printDebug >= 3:
                 print(f"Did not find any file in the given TAR: {self.tarFileName}. Assuming a compressed file.")
 
+            # For some reason, this happens for single-file.iso.
+            # Tarfile does not raise an error but also does not find any files.
+            if not self.compression:
+                raise CompressionError("Tarfile returned nothing, not even an error, and the file is not compressed!")
+
             tarInfo: Optional[Any] = None
             try:
                 tarInfo = os.fstat(fileObject.fileno())
             except io.UnsupportedOperation:
                 # If fileObject doesn't have a fileno, we set tarInfo to None
                 # and set the relevant statistics (such as st_mtime) to sensible defaults.
                 tarInfo = None
 
             fname = os.path.basename(self.tarFileName)
-            for suffix in ['.gz', '.bz2', '.bzip2', '.gzip', '.xz', '.zst', '.zstd']:
+            for suffix in ['.gz', '.bz2', '.bzip2', '.gzip', '.xz', '.zst', '.zstd', '.zz', '.zlib']:
                 if fname.lower().endswith(suffix) and len(fname) > len(suffix):
                     fname = fname[: -len(suffix)]
                     break
 
             # Try to get original file name from gzip
             mtime = 0
             if self.rawFileObject:
@@ -1243,15 +1254,15 @@
             )
 
         # Note that the xz compressed version of 100k zero-byte files is only ~200KB!
         # But this should be an edge-case and with a compression ratio of ~2, even compressed archives
         # of this size should not take more than 10s, so pretty negligible in my opinion.
         #
         # For compressed archives, detecting appended archives does not help much because the bottleneck is
-        # the decompression not the indexing of files. And because indexed_bzip2 and indexed_gzip probably
+        # the decompression not the indexing of files. And because rapidgzip and indexed_gzip probably
         # assume that the index is complete once import_index has been called, we have to recreate the full
         # block offsets anyway.
         if self.compression:
             raise InvalidIndexError(
                 f"Compressed TAR file for this SQLite index has changed size from "
                 f"{storedStats['st_size']} to {archiveStats.st_size}. It cannot be treated as appended."
             )
@@ -1260,14 +1271,24 @@
             raise InvalidIndexError("Cannot append to index of different versions!")
 
         if self.printDebug >= 2:
             print("[Info] Archive has probably been appended to because it is larger and more recent.")
         self.hasBeenAppendedTo = True
 
     def _checkMetadata(self, metadata: Dict[str, Any]) -> None:
+        # self._isGnuIncremental may be initialized during metadata check because it is required for some checks.
+        # But, if the subsequent checks fail, then we want to restore the initial value.
+        isGnuIncremental = self._isGnuIncremental
+        try:
+            self._checkMetadata2(metadata)
+        except Exception as e:
+            self._isGnuIncremental = isGnuIncremental
+            raise e
+
+    def _checkMetadata2(self, metadata: Dict[str, Any]) -> None:
         """
         Raises an exception if the metadata mismatches so much that the index has to be treated as incompatible.
         Returns normally and sets self.index.hasBeenAppendedTo to True if the size of the archive increased
         but still fits.
         """
 
         if 'tarstats' in metadata:
@@ -1326,50 +1347,71 @@
         if 'arguments' in metadata:
             indexArgs = json.loads(metadata['arguments'])
             argumentsToCheck = [
                 'mountRecursively',
                 'encoding',
                 'stripRecursiveTarExtension',
                 'transformRecursiveMountPoint',
+                'transformPattern',
                 'ignoreZeros',
             ]
 
             if self.compression == 'gz':
                 argumentsToCheck.append('gzipSeekPointSpacing')
 
-            differingArgs = []
-            for arg in argumentsToCheck:
-                if arg in indexArgs and hasattr(self, arg) and indexArgs[arg] != getattr(self, arg):
-                    differingArgs.append((arg, indexArgs[arg], getattr(self, arg)))
-            if differingArgs:
-                print("[Warning] The arguments used for creating the found index differ from the arguments ")
-                print("[Warning] given for mounting the archive now. In order to apply these changes, ")
-                print("[Warning] recreate the index using the --recreate-index option!")
-                for arg, oldState, newState in differingArgs:
-                    print(f"[Warning] {arg}: index: {oldState}, current: {newState}")
+            SQLiteIndex.checkMetadataArguments(indexArgs, self, argumentsToCheck)
+
+        # Restore the self._isGnuIncremental flag before doing any row validation because else there could be
+        # false positive warnings regarding GNU incremental detection.
+        if 'isGnuIncremental' in metadata:
+            value = metadata['isGnuIncremental'].lower()
+            self._isGnuIncremental = value in ('true', '1')
+        elif self.index.sqlConnection:
+            # This can be expensive, but it should still be less expensive than rereading the first 1000 file headers
+            # and checking the type through that way. There will be a breakeven point though for very large archives.
+            # Then, it would be better to update the index to contain the 'isGnuIncremental' metadata key.
+            self._isGnuIncremental = bool(
+                self.index.sqlConnection.execute(
+                    """SELECT 1 FROM "files" WHERE hex(type) = hex("D") LIMIT 1"""
+                ).fetchone()
+            )
+
+        if 'backendName' not in metadata:
+            # Checking the first two should already be enough to detect an index created with a different backend.
+            # Do not verify folders because parent folders and root get automatically added!
+            result = self.index.getConnection().execute(
+                f"""SELECT * {SQLiteIndex.FROM_REGULAR_FILES} ORDER BY offset ASC LIMIT 2;"""
+            )
+            if not self._checkRowsValidity(result):
+                raise InvalidIndexError("The first two files of the index do not match.")
 
     def _checkIndexValidity(self) -> bool:
         # Check some of the first and last files in the archive and some random selection in between.
         selectFiles = "SELECT * " + SQLiteIndex.FROM_REGULAR_FILES
         result = self.index.getConnection().execute(
             f"""
             SELECT * FROM ( {selectFiles} ORDER BY offset ASC LIMIT 100 )
             UNION
             SELECT * FROM ( {selectFiles} ORDER BY RANDOM() LIMIT {SQLiteIndex.NUMBER_OF_METADATA_TO_VERIFY} )
             UNION
             SELECT * FROM ( {selectFiles} ORDER BY offset DESC LIMIT 100 )
             ORDER BY offset
         """
         )
+        return self._checkRowsValidity(result)
 
+    def _checkRowsValidity(self, rows) -> bool:
         t0 = time.time()
 
         oldOffset = self.tarFileObject.tell()
+        rowCount = 0
         try:
-            for row in result:
+            for row in rows:
+                rowCount += 1
+
                 # As for the stencil size, 512 B (one TAR block) would be enough for most cases except for
                 # features like GNU LongLink which store additional metadata in further TAR blocks.
                 offsetHeader = int(row[2])
                 offsetData = int(row[3])
                 headerBlockCount = max(1, int(math.ceil((offsetData - offsetHeader) / 512))) * 512
                 with StenciledFile(fileStencils=[(self.tarFileObject, offsetHeader, headerBlockCount)]) as file:
                     with tarfile.open(fileobj=file, mode='r|', ignore_zeros=True, encoding=self.encoding) as archive:
@@ -1377,25 +1419,30 @@
                         realFileInfos, _, _ = _TarFileMetadataReader._processTarInfo(
                             tarInfo,
                             file,  # only used for isGnuIncremental == True
                             "",  # pathPrefix
                             offsetHeader,  # will be added to all offsets to get the real offset
                             self._isGnuIncremental,
                             False,  # mountRecursively
+                            self.transform,
                             self.printDebug,
                         )
 
                         # Bool columns will have been converted to int 0 or 1 when reading from SQLite.
                         # In order to compare with the read result correctly, we need to convert them to bool, too.
                         storedFileInfo = list(row)
                         for index in [-1, -2]:
                             if storedFileInfo[index] not in [0, 1]:
                                 return False
                             storedFileInfo[index] = bool(storedFileInfo[index])
 
+                        # Do not compare the path because it might have the parent TAR prepended to it for
+                        # recursive TARs and this is hard to ignore any other way.
+                        storedFileInfo[0] = realFileInfos[0][0]  # path
+                        storedFileInfo[11] = realFileInfos[0][11]  # isTar
                         if tuple(storedFileInfo) != realFileInfos[0]:
                             if self.printDebug >= 3:
                                 print("[Info] Stored file info:")
                                 print("[Info]", storedFileInfo)
                                 print("[Info] differs from recomputed one:")
                                 print("[Info]", realFileInfos[0])
                             return False
@@ -1405,69 +1452,19 @@
             # Not even worth warning because this simply might happen if the index is not valid anymore.
             return False
         finally:
             self.tarFileObject.seek(oldOffset)
 
             if self.printDebug >= 2:
                 t1 = time.time()
-                print(
-                    f"[Info] Verifying metadata for {SQLiteIndex.NUMBER_OF_METADATA_TO_VERIFY + 200} "
-                    f"files took {t1-t0:.3f} s"
-                )
+                print(f"[Info] Verifying metadata for {rowCount} files took {t1-t0:.3f} s")
 
         return False
 
     @staticmethod
-    def _detectCompression(
-        fileobj: IO[bytes], prioritizedBackends: Optional[List[str]], printDebug: int = 0
-    ) -> Optional[str]:
-        if not isinstance(fileobj, io.IOBase) or not fileobj.seekable():
-            return None
-
-        oldOffset = fileobj.tell()
-        for compressionId, compression in TAR_COMPRESSION_FORMATS.items():
-            # The header check is a necessary condition not a sufficient condition.
-            # Especially for gzip, which only has 2 magic bytes, false positives might happen.
-            # Therefore, only use the magic bytes based check if the module could not be found
-            # in order to still be able to print pinpoint error messages.
-            matches = compression.checkHeader(fileobj)
-            fileobj.seek(oldOffset)
-            if not matches:
-                continue
-
-            formatOpen = findAvailableOpen(compressionId, prioritizedBackends)
-            # If no appropriate module exists, then don't do any further checks.
-            if not formatOpen:
-                if printDebug >= 1:
-                    print(
-                        f"[Warning] A given file with magic bytes for {compressionId} could not be opened because "
-                        "no appropriate Python module could be loaded. Are some dependencies missing? To install "
-                        "ratarmountcore with all dependencies do: python3 -m pip install --user ratarmountcore[full]"
-                    )
-                return None
-
-            try:
-                compressedFileobj = formatOpen(fileobj)
-                # Reading 1B from a single-frame zst file might require decompressing it fully in order
-                # to get uncompressed file size! Avoid that. The magic bytes should suffice mostly.
-                # TODO: Make indexed_zstd not require the uncompressed size for the read call.
-                if compressionId != 'zst':
-                    compressedFileobj.read(1)
-                compressedFileobj.close()
-                fileobj.seek(oldOffset)
-                return compressionId
-            except Exception as e:
-                if printDebug >= 2:
-                    print(f"[Warning] A given file with magic bytes for {compressionId} could not be opened because:")
-                    print(e)
-                fileobj.seek(oldOffset)
-
-        return None
-
-    @staticmethod
     def _detectTar(fileobj: IO[bytes], encoding: str, printDebug: int = 0) -> bool:
         if not isinstance(fileobj, io.IOBase) or not fileobj.seekable():
             return False
 
         oldOffset = fileobj.tell()
         isTar = False
         try:
@@ -1490,17 +1487,15 @@
         printDebug: int = 0,
     ) -> Any:
         """
         Opens a file possibly undoing the compression.
         Returns (tar_file_obj, raw_file_obj, compression, isTar).
         raw_file_obj will be none if compression is None.
         """
-        compression = SQLiteIndexedTar._detectCompression(
-            fileobj, prioritizedBackends=prioritizedBackends, printDebug=printDebug
-        )
+        compression = detectCompression(fileobj, prioritizedBackends=prioritizedBackends, printDebug=printDebug)
         if printDebug >= 3:
             print(f"[Info] Detected compression {compression} for file object:", fileobj)
 
         if compression not in TAR_COMPRESSION_FORMATS:
             return fileobj, None, compression, SQLiteIndexedTar._detectTar(fileobj, encoding, printDebug=printDebug)
 
         formatOpen = findAvailableOpen(compression, prioritizedBackends)
@@ -1536,15 +1531,15 @@
                 # because internally many buffers are allocated with 4 * spacing size.
                 bufferSize = max(3 * 1024 * 1024, 3 * gzipSeekPointSpacing)
                 # drop_handles keeps a file handle opening as is required to call tell() during decoding
                 tar_file = indexed_gzip.IndexedGzipFile(
                     fileobj=fileobj, drop_handles=False, spacing=gzipSeekPointSpacing, buffer_size=bufferSize
                 )
         elif compression == 'bz2':
-            tar_file = indexed_bzip2.open(fileobj, parallelization=parallelization)  # type: ignore
+            tar_file = rapidgzip.IndexedBzip2File(fileobj, parallelization=parallelization)  # type: ignore
         elif (
             compression == 'xz'
             and xz
             and parallelization != 1
             and hasattr(fileobj, 'name')
             and os.path.isfile(fileobj.name)
             and platform.system() == 'Linux'
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore/SingleFileMountSource.py` & `ratarmountcore-0.7.0/ratarmountcore/SingleFileMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/StenciledFile.py` & `ratarmountcore-0.7.0/ratarmountcore/StenciledFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/SubvolumesMountSource.py` & `ratarmountcore-0.7.0/ratarmountcore/SubvolumesMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/UnionMountSource.py` & `ratarmountcore-0.7.0/ratarmountcore/UnionMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/ratarmountcore/ZipMountSource.py` & `ratarmountcore-0.7.0/ratarmountcore/ZipMountSource.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import datetime
 import json
 import os
+import re
 import stat
 import tarfile
+import traceback
 from timeit import default_timer as timer
 
 from typing import Any, Dict, IO, Iterable, List, Optional, Tuple, Union
 
 from .compressions import zipfile
 from .MountSource import FileInfo, MountSource
 from .SQLiteIndex import SQLiteIndex, SQLiteIndexedTarUserData
@@ -17,43 +19,54 @@
 
 
 class ZipMountSource(MountSource):
     def __init__(
         self,
         # fmt: off
         fileOrPath             : Union[str, IO[bytes]],
-        writeIndex             : bool                = False,
-        clearIndexCache        : bool                = False,
-        indexFilePath          : Optional[str]       = None,
-        indexFolders           : Optional[List[str]] = None,
-        encoding               : str                 = tarfile.ENCODING,
-        verifyModificationTime : bool                = False,
-        printDebug             : int                 = 0,
-        indexMinimumFileCount  : int                 = 1000,
+        writeIndex             : bool                      = False,
+        clearIndexCache        : bool                      = False,
+        indexFilePath          : Optional[str]             = None,
+        indexFolders           : Optional[List[str]]       = None,
+        encoding               : str                       = tarfile.ENCODING,
+        verifyModificationTime : bool                      = False,
+        printDebug             : int                       = 0,
+        indexMinimumFileCount  : int                       = 1000,
+        transform              : Optional[Tuple[str, str]] = None,
         **options
         # fmt: on
     ) -> None:
-        self.fileObject = zipfile.ZipFile(fileOrPath, 'r')
-        self.archiveFilePath = fileOrPath if isinstance(fileOrPath, str) else None
-        self.encoding = encoding
+        # fmt: off
+        self.fileObject             = zipfile.ZipFile(fileOrPath, 'r')
+        self.archiveFilePath        = fileOrPath if isinstance(fileOrPath, str) else None
+        self.encoding               = encoding
         self.verifyModificationTime = verifyModificationTime
-        self.printDebug = printDebug
-        self.options = options
+        self.printDebug             = printDebug
+        self.options                = options
+        self.transformPattern       = transform
+        # fmt: on
+
+        self.transform = (
+            (lambda x: re.sub(self.transformPattern[0], self.transformPattern[1], x))
+            if isinstance(self.transformPattern, (tuple, list)) and len(self.transformPattern) == 2
+            else (lambda x: x)
+        )
 
         ZipMountSource._findPassword(self.fileObject, options.get("passwords", []))
         self.files = {info.header_offset: info for info in self.fileObject.infolist()}
 
         self.index = SQLiteIndex(
             indexFilePath,
             indexFolders=indexFolders,
             archiveFilePath=self.archiveFilePath,
             encoding=self.encoding,
             checkMetadata=self._checkMetadata,
             printDebug=self.printDebug,
             indexMinimumFileCount=indexMinimumFileCount,
+            backendName='ZipMountSource',
         )
 
         if clearIndexCache:
             self.index.clearIndexes()
 
         isFileObject = not isinstance(fileOrPath, str)
 
@@ -73,15 +86,15 @@
             self._createIndex()
             # self._loadOrStoreCompressionOffsets()  # store
             if self.index.indexIsLoaded():
                 self._storeMetadata()
                 self.index.reloadIndexReadOnly()
 
     def _storeMetadata(self) -> None:
-        argumentsToSave = ['encoding']
+        argumentsToSave = ['encoding', 'transformPattern']
         argumentsMetadata = json.dumps({argument: getattr(self, argument) for argument in argumentsToSave})
         self.index.storeMetadata(argumentsMetadata, self.archiveFilePath)
 
     def _convertToRow(self, info: "zipfile.ZipInfo") -> Tuple:
         mode = 0o555 | (stat.S_IFDIR if info.is_dir() else stat.S_IFREG)
         mtime = datetime.datetime(*info.date_time, tzinfo=datetime.timezone.utc).timestamp() if info.date_time else 0
 
@@ -97,15 +110,15 @@
 
         # file_redir is (type, flags, target) or None. Only tested for type == RAR5_XREDIR_UNIX_SYMLINK.
         linkname = ""
         if stat.S_ISLNK(info.external_attr >> 16):
             linkname = self.fileObject.read(info).decode()
             mode = 0o555 | stat.S_IFLNK
 
-        path, name = SQLiteIndex.normpath(info.filename).rsplit("/", 1)
+        path, name = SQLiteIndex.normpath(self.transform(info.filename)).rsplit("/", 1)
 
         # Currently, this is unused. The index only is used for getting metadata. (The data offset
         # is already determined and written out in order to possibly speed up reading of encrypted
         # files by implementing the decryption ourselves.)
         # The data offset is deprecated again! Collecting it can add a huge overhead for large zip files
         # because we have to seek to every position and read a few bytes from it. Furthermore, it is useless
         # by itself anyway. We don't even store yet how the data is compressed or encrypted, so we would
@@ -228,14 +241,44 @@
 
     @overrides(MountSource)
     def read(self, fileInfo: FileInfo, size: int, offset: int) -> bytes:
         with self.open(fileInfo) as file:
             file.seek(offset, os.SEEK_SET)
             return file.read(size)
 
+    def _tryToOpenFirstFile(self):
+        # Get first row that has the regular file bit set in mode (stat.S_IFREG == 32768 == 1<<15).
+        result = self.index.getConnection().execute(
+            f"""SELECT path,name {SQLiteIndex.FROM_REGULAR_FILES} ORDER BY "offsetheader" ASC LIMIT 1;"""
+        )
+        if not result:
+            return
+        firstFile = result.fetchone()
+        if not firstFile:
+            return
+
+        if self.printDebug >= 2:
+            print(
+                "[Info] The index contains no backend name. Therefore, will try to open the first file as "
+                "an integrity check."
+            )
+        try:
+            fileInfo = self.getFileInfo(firstFile[0] + '/' + firstFile[1])
+            if not fileInfo:
+                return
+
+            with self.open(fileInfo) as file:
+                file.read(1)
+        except Exception as exception:
+            if self.printDebug >= 2:
+                print("[Info] Trying to open the first file raised an exception:", exception)
+            if self.printDebug >= 3:
+                traceback.print_exc()
+            raise InvalidIndexError("Integrity check of opening the first file failed.") from exception
+
     def _checkMetadata(self, metadata: Dict[str, Any]) -> None:
         """Raises an exception if the metadata mismatches so much that the index has to be treated as incompatible."""
 
         if 'tarstats' in metadata:
             if not self.archiveFilePath:
                 raise InvalidIndexError("Archive contains file stats but cannot stat real archive!")
 
@@ -257,23 +300,14 @@
                 and archiveStats.st_mtime != storedStats['st_mtime']
             ):
                 raise InvalidIndexError(
                     f"The modification date for the archive file {storedStats['st_mtime']} "
                     f"to this SQLite index has changed ({str(archiveStats.st_mtime)})",
                 )
 
-        # Check arguments used to create the found index.
-        # These are only warnings and not forcing a rebuild by default.
-        # TODO: Add --force options?
         if 'arguments' in metadata:
-            indexArgs = json.loads(metadata['arguments'])
-            argumentsToCheck = ['encoding']
-            differingArgs = []
-            for arg in argumentsToCheck:
-                if arg in indexArgs and hasattr(self, arg) and indexArgs[arg] != getattr(self, arg):
-                    differingArgs.append((arg, indexArgs[arg], getattr(self, arg)))
-            if differingArgs:
-                print("[Warning] The arguments used for creating the found index differ from the arguments ")
-                print("[Warning] given for mounting the archive now. In order to apply these changes, ")
-                print("[Warning] recreate the index using the --recreate-index option!")
-                for arg, oldState, newState in differingArgs:
-                    print(f"[Warning] {arg}: index: {oldState}, current: {newState}")
+            SQLiteIndex.checkMetadataArguments(
+                json.loads(metadata['arguments']), self, argumentsToCheck=['encoding', 'transformPattern']
+            )
+
+        if 'backendName' not in metadata:
+            self._tryToOpenFirstFile()
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore/__init__.py` & `ratarmountcore-0.7.0/ratarmountcore/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from .StenciledFile import LambdaReaderFile, RawStenciledFile, StenciledFile, JoinedFile
 from .SQLiteBlobFile import SQLiteBlobFile, SQLiteBlobsFile
 from .BlockParallelReaders import BlockParallelReader, ParallelXZReader, ParallelZstdReader
 
 from .MountSource import FileInfo, MountSource
 
 from .FolderMountSource import FolderMountSource
+from .LibarchiveMountSource import LibarchiveMountSource
 from .RarMountSource import RarMountSource
 from .ZipMountSource import ZipMountSource
 from .SQLiteIndexedTar import SQLiteIndexedTar, SQLiteIndexedTarUserData
 from .SQLiteIndex import SQLiteIndex
 
 from .AutoMountLayer import AutoMountLayer
 from .FileVersionLayer import FileVersionLayer
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore/utils.py` & `ratarmountcore-0.7.0/ratarmountcore/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,18 @@
     """Exception for operations executed on a closed index database."""
 
 
 class InvalidIndexError(RatarmountError):
     """Exception for indexes being invalid, outdated, or created with different arguments."""
 
 
+class MismatchingIndexError(RatarmountError):
+    """Exception for indexes being created by a different backend."""
+
+
 class CompressionError(RatarmountError):
     """Exception for trying to open files with unsupported compression or unavailable decompression module."""
 
 
 def overrides(parentClass):
     """Simple decorator that checks that a method with the same name exists in the parent class"""
 
@@ -251,28 +255,28 @@
     if hasattr(module, '__version__'):
         return str(getattr(module, '__version__'))
 
     if hasattr(module, '__file__'):
         moduleFilePath = getattr(module, '__file__')
         for distribution in imeta.distributions():
             try:
-                if distributionContainsFile(distribution, moduleFilePath) and 'Name' in distribution.metadata:
-                    return distribution.metadata['Name']
+                if distributionContainsFile(distribution, moduleFilePath) and 'Version' in distribution.metadata:
+                    return distribution.metadata['Version']
             except Exception:
                 pass
 
     return None
 
 
 def isOnSlowDrive(filePath: str):
     # TODO determine whether the whole file or most of it has been cached:
     #      https://serverfault.com/questions/278454/is-it-possible-to-list-the-files-that-are-cached
     #      https://github.com/mxmlnkn/rapidgzip/issues/13#issuecomment-1592856413
     # TODO make it work on Windows: https://devblogs.microsoft.com/oldnewthing/20201023-00/?p=104395
     try:
         device = os.stat(filePath).st_dev
-        with open(f"/sys/dev/block/{os.major(device)}:{os.minor(device)}/queue/rotational", 'rt') as file:
-            if file.read().strip() == "1":
+        with open(f"/sys/dev/block/{os.major(device)}:{os.minor(device)}/queue/rotational", 'rb') as file:
+            if file.read().strip() == b"1":
                 return True
     except Exception:
         pass
     return False
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore.egg-info/PKG-INFO` & `ratarmountcore-0.7.0/ratarmountcore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratarmountcore
-Version: 0.6.5
+Version: 0.7.0
 Summary: Random Access Read-Only Tar Mount Library
 Home-page: https://github.com/mxmlnkn/ratarmount/ratarmountcore
 Author: Maximilian Knespel
 Author-email: mxmlnkn@github.de
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
@@ -24,33 +24,35 @@
 Classifier: Topic :: System :: Filesystems
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: dataclasses; python_version < "3.7.0"
 Requires-Dist: importlib-metadata; python_version < "3.8.0"
 Provides-Extra: full
-Requires-Dist: indexed_bzip2<2.0,>=1.3.1; extra == "full"
 Requires-Dist: indexed_gzip<2.0,>=1.6.3; extra == "full"
 Requires-Dist: indexed_zstd<2.0,>=1.3.1; sys_platform == "darwin" and extra == "full"
 Requires-Dist: indexed_zstd<2.0,>=1.2.2; platform_system != "Windows" and extra == "full"
+Requires-Dist: libarchive-c<6.0,~=5.1; extra == "full"
 Requires-Dist: python-xz~=0.4.0; extra == "full"
-Requires-Dist: rapidgzip>=0.10.0; extra == "full"
+Requires-Dist: rapidgzip>=0.13.1; extra == "full"
 Requires-Dist: rarfile~=4.0; extra == "full"
 Provides-Extra: bzip2
-Requires-Dist: indexed_bzip2<2.0,>=1.3.1; extra == "bzip2"
+Requires-Dist: rapidgzip>=0.13.1; extra == "bzip2"
 Provides-Extra: gzip
 Requires-Dist: indexed_gzip<2.0,>=1.6.3; extra == "gzip"
 Provides-Extra: rar
 Requires-Dist: rarfile~=4.0; extra == "rar"
 Provides-Extra: xz
 Requires-Dist: python-xz~=0.4.0; extra == "xz"
 Provides-Extra: zip
 Provides-Extra: zstd
 Requires-Dist: indexed_zstd<2.0,>=1.3.1; sys_platform == "darwin" and extra == "zstd"
 Requires-Dist: indexed_zstd<2.0,>=1.2.2; platform_system != "Windows" and extra == "zstd"
+Provides-Extra: 7z
+Requires-Dist: libarchive-c<6.0,~=5.1; extra == "7z"
 
 # Random Access Read-Only Tar Mount (Ratarmount) Library
 
 [![PyPI version](https://badge.fury.io/py/ratarmountcore.svg)](https://badge.fury.io/py/ratarmountcore)
 [![Python Version](https://img.shields.io/pypi/pyversions/ratarmountcore)](https://pypi.org/project/ratarmountcore/)
 [![Downloads](https://static.pepy.tech/badge/ratarmountcore/month)](https://pepy.tech/project/ratarmountcore)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](http://opensource.org/licenses/MIT)
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore.egg-info/SOURCES.txt` & `ratarmountcore-0.7.0/ratarmountcore.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.cfg
 setup.py
 ratarmountcore/AutoMountLayer.py
 ratarmountcore/BlockParallelReaders.py
 ratarmountcore/FileVersionLayer.py
 ratarmountcore/FolderMountSource.py
+ratarmountcore/LibarchiveMountSource.py
 ratarmountcore/MountSource.py
 ratarmountcore/ProgressBar.py
 ratarmountcore/RarMountSource.py
 ratarmountcore/SQLiteBlobFile.py
 ratarmountcore/SQLiteIndex.py
 ratarmountcore/SQLiteIndexedTar.py
 ratarmountcore/SingleFileMountSource.py
@@ -26,14 +27,15 @@
 ratarmountcore.egg-info/PKG-INFO
 ratarmountcore.egg-info/SOURCES.txt
 ratarmountcore.egg-info/dependency_links.txt
 ratarmountcore.egg-info/requires.txt
 ratarmountcore.egg-info/top_level.txt
 tests/test_AutoMountLayer.py
 tests/test_BlockParallelReaders.py
+tests/test_LibarchiveMountSource.py
 tests/test_RarMountSource.py
 tests/test_SQLiteBlobFile.py
 tests/test_SQLiteIndex.py
 tests/test_SQLiteIndexedTar.py
 tests/test_StenciledFile.py
 tests/test_SubvolumesMountSource.py
 tests/test_UnionMountSource.py
```

### Comparing `ratarmountcore-0.6.5/ratarmountcore.egg-info/requires.txt` & `ratarmountcore-0.7.0/ratarmountcore.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 
+[7z]
+libarchive-c<6.0,~=5.1
+
 [:python_version < "3.7.0"]
 dataclasses
 
 [:python_version < "3.8.0"]
 importlib-metadata
 
 [bzip2]
-indexed_bzip2<2.0,>=1.3.1
+rapidgzip>=0.13.1
 
 [full]
-indexed_bzip2<2.0,>=1.3.1
 indexed_gzip<2.0,>=1.6.3
+libarchive-c<6.0,~=5.1
 python-xz~=0.4.0
-rapidgzip>=0.10.0
+rapidgzip>=0.13.1
 rarfile~=4.0
 
 [full:platform_system != "Windows"]
 indexed_zstd<2.0,>=1.2.2
 
 [full:sys_platform == "darwin"]
 indexed_zstd<2.0,>=1.3.1
```

### Comparing `ratarmountcore-0.6.5/setup.cfg` & `ratarmountcore-0.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -32,27 +32,28 @@
 packages = ratarmountcore
 install_requires = 
 	dataclasses; python_version < "3.7.0"
 	importlib-metadata; python_version < "3.8.0"
 
 [options.extras_require]
 full = 
-	indexed_bzip2 >= 1.3.1, < 2.0
 	indexed_gzip >= 1.6.3, < 2.0
 	indexed_zstd >= 1.3.1, < 2.0; sys_platform=="darwin"
 	indexed_zstd >= 1.2.2, < 2.0; platform_system!="Windows"
+	libarchive-c ~= 5.1, < 6.0
 	python-xz ~= 0.4.0
-	rapidgzip >= 0.10.0
+	rapidgzip >= 0.13.1
 	rarfile ~= 4.0
-bzip2 = indexed_bzip2 >= 1.3.1, < 2.0
+bzip2 = rapidgzip >= 0.13.1
 gzip = indexed_gzip >= 1.6.3, < 2.0
 rar = rarfile ~= 4.0
 xz = python-xz ~= 0.4.0
 zip = 
 zstd = 
 	indexed_zstd >= 1.3.1, < 2.0; sys_platform=="darwin"
 	indexed_zstd >= 1.2.2, < 2.0; platform_system!="Windows"
+7z = libarchive-c ~= 5.1, < 6.0
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `ratarmountcore-0.6.5/setup.py` & `ratarmountcore-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_BlockParallelReaders.py` & `ratarmountcore-0.7.0/tests/test_BlockParallelReaders.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_RarMountSource.py` & `ratarmountcore-0.7.0/tests/test_RarMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_SQLiteBlobFile.py` & `ratarmountcore-0.7.0/tests/test_SQLiteBlobFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_SQLiteIndex.py` & `ratarmountcore-0.7.0/tests/test_SQLiteIndex.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_SQLiteIndexedTar.py` & `ratarmountcore-0.7.0/tests/test_SQLiteIndexedTar.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,31 +11,25 @@
 import os
 import stat
 import subprocess
 import sys
 import tarfile
 import tempfile
 
-import indexed_bzip2
+import rapidgzip
+
+from helpers import copyTestFile
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..')))
 
 import pytest  # noqa: E402
 
 from ratarmountcore import RatarmountError, SQLiteIndexedTar  # noqa: E402
 
 
-def findTestFile(relativePathOrName):
-    for i in range(3):
-        path = os.path.sep.join([".."] * i + ["tests", relativePathOrName])
-        if os.path.exists(path):
-            return path
-    return relativePathOrName
-
-
 @pytest.mark.parametrize("parallelization", [1, 2, 4])
 class TestSQLiteIndexedTarParallelized:
     @staticmethod
     def _createFile(tarArchive, name, contents):
         tinfo = tarfile.TarInfo(name)
         tinfo.size = len(contents)
         tarArchive.addfile(tinfo, io.BytesIO(contents.encode()))
@@ -44,26 +38,26 @@
     def _makeFolder(tarArchive, name):
         tinfo = tarfile.TarInfo(name)
         tinfo.type = tarfile.DIRTYPE
         tarArchive.addfile(tinfo, io.BytesIO())
 
     @staticmethod
     def test_context_manager(parallelization):
-        with SQLiteIndexedTar(
-            findTestFile('single-file.tar'), writeIndex=False, parallelization=parallelization
+        with copyTestFile("single-file.tar") as path, SQLiteIndexedTar(
+            path, writeIndex=False, parallelization=parallelization
         ) as indexedTar:
             assert indexedTar.listDir('/')
             assert indexedTar.getFileInfo('/')
             assert not indexedTar.getFileInfo('../')
             assert not indexedTar.getFileInfo('../bar')
 
     @staticmethod
     def test_tar_bz2_with_parallelization(parallelization):
-        with SQLiteIndexedTar(
-            findTestFile("2k-recursive-tars.tar.bz2"),
+        with copyTestFile("2k-recursive-tars.tar.bz2") as path, SQLiteIndexedTar(
+            path,
             clearIndexCache=True,
             recursive=False,
             parallelization=parallelization,
         ) as file:
             for folder in ['/', '/mimi']:
                 assert file.getFileInfo(folder)
                 assert file.fileVersions(folder) == 1
@@ -75,16 +69,16 @@
 
             assert not file.listDir('/mimi/00105.tar')
             info = file.getFileInfo('/mimi/00105.tar')
             assert info.userdata[0].offset == 1248256
 
     @staticmethod
     def test_recursive_tar_bz2_with_parallelization(parallelization):
-        with SQLiteIndexedTar(
-            findTestFile("2k-recursive-tars.tar.bz2"),
+        with copyTestFile("2k-recursive-tars.tar.bz2") as path, SQLiteIndexedTar(
+            path,
             clearIndexCache=True,
             recursive=True,
             parallelization=parallelization,
         ) as file:
             assert file.listDir('/')
             assert file.listDir('/mimi')
 
@@ -94,16 +88,16 @@
 
             assert file.listDir('/mimi/00105.tar')
             info = file.getFileInfo('/mimi/00105.tar/foo')
             assert info.userdata[0].offset == 1248768
 
     @staticmethod
     def test_deep_recursive(parallelization):
-        with SQLiteIndexedTar(
-            findTestFile("packed-5-times.tar.gz"),
+        with copyTestFile("packed-5-times.tar.gz") as path, SQLiteIndexedTar(
+            path,
             clearIndexCache=True,
             recursive=True,
             parallelization=parallelization,
         ) as mountSource:
             assert mountSource.listDir('/')
             assert mountSource.listDir('/ufo_03.tar')
             assert mountSource.listDir('/ufo_03.tar/ufo_02.tar')
@@ -441,17 +435,17 @@
     @staticmethod
     def test_appending_to_large_archive(parallelization, tmpdir):
         createFile = TestSQLiteIndexedTarParallelized._createFile
         makeFolder = TestSQLiteIndexedTarParallelized._makeFolder
 
         # Create a TAR large in size as well as file count
         tarPath = os.path.join(tmpdir, "foo.tar")
-        with indexed_bzip2.open(findTestFile("tar-with-300-folders-with-1000-files-0B-files.tar.bz2")) as file, open(
-            tarPath, 'wb'
-        ) as extracted:
+        with copyTestFile("tar-with-300-folders-with-1000-files-0B-files.tar.bz2") as path, rapidgzip.IndexedBzip2File(
+            path
+        ) as file, open(tarPath, 'wb') as extracted:
             while True:
                 data = file.read(1024 * 1024)
                 if not data:
                     break
                 extracted.write(data)
 
         # Create index
```

### Comparing `ratarmountcore-0.6.5/tests/test_StenciledFile.py` & `ratarmountcore-0.7.0/tests/test_StenciledFile.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_SubvolumesMountSource.py` & `ratarmountcore-0.7.0/tests/test_SubvolumesMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_UnionMountSource.py` & `ratarmountcore-0.7.0/tests/test_UnionMountSource.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_ZipMountSource.py` & `ratarmountcore-0.7.0/tests/test_ZipMountSource.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,10 +39,13 @@
 
             # Links are not resolved by the mount source but by FUSE, i.e., descending into a link to a folder
             # will not work. This behavior may change in the future.
             for linkPath in ['/foo/jet']:
                 assert mountSource.getFileInfo(linkPath)
                 assert mountSource.fileVersions(linkPath) == 1
                 assert not mountSource.listDir(linkPath)
+                fileInfo = mountSource.getFileInfo(linkPath)
+                assert fileInfo.linkname == 'fighter'
                 with mountSource.open(mountSource.getFileInfo(linkPath)) as file:
                     # Contents of symlink is the symlink destination itself.
+                    # This behavior is not consistent with other MountSources and therefore subject to change!
                     assert file.read() == b'fighter'
```

### Comparing `ratarmountcore-0.6.5/tests/test_compressions.py` & `ratarmountcore-0.7.0/tests/test_compressions.py`

 * *Files identical despite different names*

### Comparing `ratarmountcore-0.6.5/tests/test_utils.py` & `ratarmountcore-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

