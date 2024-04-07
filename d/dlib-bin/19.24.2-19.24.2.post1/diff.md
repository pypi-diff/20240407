# Comparing `tmp/dlib_bin-19.24.2-cp39-cp39-win_amd64.whl.zip` & `tmp/dlib_bin-19.24.2.post1-cp311-cp311-musllinux_1_1_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,14 @@
-Zip file size: 2663630 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat  7463424 b- defN 23-May-15 10:54 _dlib_pybind11.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      795 b- defN 23-May-15 10:47 dlib/__init__.py
--rw-rw-rw-  2.0 fat     1359 b- defN 23-May-15 10:55 dlib_bin-19.24.2.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1452 b- defN 23-May-15 10:55 dlib_bin-19.24.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-15 10:55 dlib_bin-19.24.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-May-15 10:54 dlib_bin-19.24.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      571 b- defN 23-May-15 10:55 dlib_bin-19.24.2.dist-info/RECORD
-7 files, 7467721 bytes uncompressed, 2662622 bytes compressed:  64.4%
+Zip file size: 3749948 bytes, number of entries: 12
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-07 11:53 dlib_bin.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-07 11:53 dlib_bin-19.24.2.post1.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-07 11:53 dlib/
+-rwxr-xr-x  2.0 unx  8360057 b- defN 24-Apr-07 11:53 _dlib_pybind11.cpython-311-aarch64-linux-musl.so
+-rw-r--r--  2.0 unx   134393 b- defN 24-Apr-07 11:53 dlib_bin.libs/libgcc_s-4e37474d.so.1
+-rwxr-xr-x  2.0 unx  2599041 b- defN 24-Apr-07 11:53 dlib_bin.libs/libstdc++-fd9f4683.so.6.0.28
+-rw-r--r--  2.0 unx       20 b- defN 24-Apr-07 11:53 dlib_bin-19.24.2.post1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-07 11:53 dlib_bin-19.24.2.post1.dist-info/METADATA
+-rw-r--r--  2.0 unx      114 b- defN 24-Apr-07 11:53 dlib_bin-19.24.2.post1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1337 b- defN 24-Apr-07 11:53 dlib_bin-19.24.2.post1.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      822 b- defN 24-Apr-07 11:53 dlib_bin-19.24.2.post1.dist-info/RECORD
+-rw-r--r--  2.0 unx      775 b- defN 24-Apr-07 11:53 dlib/__init__.py
+12 files, 11097984 bytes uncompressed, 3748210 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,22 +1,37 @@
-Filename: _dlib_pybind11.cp39-win_amd64.pyd
+Filename: dlib_bin.libs/
 Comment: 
 
-Filename: dlib/__init__.py
+Filename: dlib_bin-19.24.2.post1.dist-info/
+Comment: 
+
+Filename: dlib/
+Comment: 
+
+Filename: _dlib_pybind11.cpython-311-aarch64-linux-musl.so
+Comment: 
+
+Filename: dlib_bin.libs/libgcc_s-4e37474d.so.1
+Comment: 
+
+Filename: dlib_bin.libs/libstdc++-fd9f4683.so.6.0.28
 Comment: 
 
-Filename: dlib_bin-19.24.2.dist-info/LICENSE.txt
+Filename: dlib_bin-19.24.2.post1.dist-info/top_level.txt
 Comment: 
 
-Filename: dlib_bin-19.24.2.dist-info/METADATA
+Filename: dlib_bin-19.24.2.post1.dist-info/METADATA
 Comment: 
 
-Filename: dlib_bin-19.24.2.dist-info/WHEEL
+Filename: dlib_bin-19.24.2.post1.dist-info/WHEEL
 Comment: 
 
-Filename: dlib_bin-19.24.2.dist-info/top_level.txt
+Filename: dlib_bin-19.24.2.post1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dlib_bin-19.24.2.dist-info/RECORD
+Filename: dlib_bin-19.24.2.post1.dist-info/RECORD
+Comment: 
+
+Filename: dlib/__init__.py
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## dlib/__init__.py

 * *Ordering differences only*

```diff
@@ -1,20 +1,20 @@
-# Copyright (C) 2020  Davis E. King (davis@dlib.net)
-# License: Boost Software License   See LICENSE.txt for the full license.
-
-def add_lib_to_dll_path(path):
-    """ On windows you must call os.add_dll_directory() to allow linking to external DLLs.  See
-    https://docs.python.org/3.8/whatsnew/3.8.html#bpo-36085-whatsnew.  This function adds the folder
-    containing path to the dll search path. 
-    """
-    try:
-        import os
-        os.add_dll_directory(os.path.join(os.path.dirname(path), '../../bin'))
-    except (AttributeError,KeyError,FileNotFoundError):
-        pass
-
-if 'OFF' == 'ON':
-    add_lib_to_dll_path('')
-    add_lib_to_dll_path('CUDA_CUDART_LIBRARY-NOTFOUND')
-
-from _dlib_pybind11 import *
-from _dlib_pybind11 import __version__, __time_compiled__
+# Copyright (C) 2020  Davis E. King (davis@dlib.net)
+# License: Boost Software License   See LICENSE.txt for the full license.
+
+def add_lib_to_dll_path(path):
+    """ On windows you must call os.add_dll_directory() to allow linking to external DLLs.  See
+    https://docs.python.org/3.8/whatsnew/3.8.html#bpo-36085-whatsnew.  This function adds the folder
+    containing path to the dll search path. 
+    """
+    try:
+        import os
+        os.add_dll_directory(os.path.join(os.path.dirname(path), '../../bin'))
+    except (AttributeError,KeyError,FileNotFoundError):
+        pass
+
+if 'OFF' == 'ON':
+    add_lib_to_dll_path('')
+    add_lib_to_dll_path('CUDA_CUDART_LIBRARY-NOTFOUND')
+
+from _dlib_pybind11 import *
+from _dlib_pybind11 import __version__, __time_compiled__
```

## Comparing `dlib_bin-19.24.2.dist-info/LICENSE.txt` & `dlib_bin-19.24.2.post1.dist-info/LICENSE.txt`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-Boost Software License - Version 1.0 - August 17th, 2003
-
-Permission is hereby granted, free of charge, to any person or organization
-obtaining a copy of the software and accompanying documentation covered by
-this license (the "Software") to use, reproduce, display, distribute,
-execute, and transmit the Software, and to prepare derivative works of the
-Software, and to permit third-parties to whom the Software is furnished to
-do so, all subject to the following:
-
-The copyright notices in the Software and this entire statement, including
-the above license grant, this restriction and the following disclaimer,
-must be included in all copies of the Software, in whole or in part, and
-all derivative works of the Software, unless such copies or derivative
-works are solely in the form of machine-executable object code generated by
-a source language processor.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
-SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
-FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+Boost Software License - Version 1.0 - August 17th, 2003
+
+Permission is hereby granted, free of charge, to any person or organization
+obtaining a copy of the software and accompanying documentation covered by
+this license (the "Software") to use, reproduce, display, distribute,
+execute, and transmit the Software, and to prepare derivative works of the
+Software, and to permit third-parties to whom the Software is furnished to
+do so, all subject to the following:
+
+The copyright notices in the Software and this entire statement, including
+the above license grant, this restriction and the following disclaimer,
+must be included in all copies of the Software, in whole or in part, and
+all derivative works of the Software, unless such copies or derivative
+works are solely in the form of machine-executable object code generated by
+a source language processor.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, TITLE AND NON-INFRINGEMENT. IN NO EVENT
+SHALL THE COPYRIGHT HOLDERS OR ANYONE DISTRIBUTING THE SOFTWARE BE LIABLE
+FOR ANY DAMAGES OR OTHER LIABILITY, WHETHER IN CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
```

## Comparing `dlib_bin-19.24.2.dist-info/METADATA` & `dlib_bin-19.24.2.post1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1
-Name: dlib-bin
-Version: 19.24.2
-Summary: A toolkit for making real world machine learning and data analysis applications
-Home-page: https://github.com/alesanfra/dlib-wheels
-Author: Davis King
-Author-email: davis@dlib.net
-License: Boost Software License
-Keywords: dlib,Computer Vision,Machine Learning
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Topic :: Software Development
-License-File: LICENSE.txt
-
-See http://dlib.net for documentation.
+Metadata-Version: 2.1
+Name: dlib-bin
+Version: 19.24.2.post1
+Summary: A toolkit for making real world machine learning and data analysis applications
+Home-page: https://github.com/alesanfra/dlib-wheels
+Author: Davis King
+Author-email: davis@dlib.net
+License: Boost Software License
+Keywords: dlib,Computer Vision,Machine Learning
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.6
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Topic :: Software Development
+License-File: LICENSE.txt
+
+See http://dlib.net for documentation.
```

