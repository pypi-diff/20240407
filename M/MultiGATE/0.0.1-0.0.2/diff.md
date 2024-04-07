# Comparing `tmp/MultiGATE-0.0.1.tar.gz` & `tmp/MultiGATE-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MultiGATE-0.0.1.tar", last modified: Sun Apr  7 15:33:35 2024, max compression
+gzip compressed data, was "dist/MultiGATE-0.0.2.tar", last modified: Sun Apr  7 15:39:17 2024, max compression
```

## Comparing `MultiGATE-0.0.1.tar` & `MultiGATE-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:33:35.000000 MultiGATE-0.0.1/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.1/LICENSE
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:33:35.000000 MultiGATE-0.0.1/MultiGATE/
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:33:35.000000 MultiGATE-0.0.1/MultiGATE/MultiGATE.egg-info/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-07 15:33:34.000000 MultiGATE-0.0.1/MultiGATE/MultiGATE.egg-info/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-07 15:33:34.000000 MultiGATE-0.0.1/MultiGATE/MultiGATE.egg-info/SOURCES.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-07 15:33:34.000000 MultiGATE-0.0.1/MultiGATE/MultiGATE.egg-info/dependency_links.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       32 2024-04-07 15:33:34.000000 MultiGATE-0.0.1/MultiGATE/MultiGATE.egg-info/requires.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-07 15:33:34.000000 MultiGATE-0.0.1/MultiGATE/MultiGATE.egg-info/top_level.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-07 15:33:35.000000 MultiGATE-0.0.1/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.1/README.md
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-07 15:33:35.000000 MultiGATE-0.0.1/setup.cfg
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      845 2024-04-07 15:32:12.000000 MultiGATE-0.0.1/setup.py
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.2/LICENSE
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/MultiGATE/
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/MultiGATE/MultiGATE.egg-info/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/MultiGATE/MultiGATE.egg-info/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/MultiGATE/MultiGATE.egg-info/SOURCES.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/MultiGATE/MultiGATE.egg-info/dependency_links.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       40 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/MultiGATE/MultiGATE.egg-info/requires.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/MultiGATE/MultiGATE.egg-info/top_level.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.2/README.md
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-07 15:39:17.000000 MultiGATE-0.0.2/setup.cfg
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      876 2024-04-07 15:37:37.000000 MultiGATE-0.0.2/setup.py
```

### Comparing `MultiGATE-0.0.1/LICENSE` & `MultiGATE-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `MultiGATE-0.0.1/MultiGATE/MultiGATE.egg-info/PKG-INFO` & `MultiGATE-0.0.2/MultiGATE/MultiGATE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.1
+Version: 0.0.2
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.1/PKG-INFO` & `MultiGATE-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.1
+Version: 0.0.2
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.1/setup.py` & `MultiGATE-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="MultiGATE",
-    version="0.0.1",
+    version="0.0.2",
     description="MultiGATE single cell",
     package_dir={"": "MultiGATE"},
     packages=find_packages(where="MultiGATE"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aqlkzf/MultiGATEtest1",
     author="Jinzhao LI & Jishuai MIAO",
     author_email="jishuaimiao@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Operating System :: OS Independent",
     ],
-    install_requires=[""],
+    install_requires=["seaborn",
+                      ],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
     python_requires="==3.7.*",
 )
```

