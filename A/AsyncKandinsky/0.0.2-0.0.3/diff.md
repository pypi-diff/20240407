# Comparing `tmp/AsyncKandinsky-0.0.2.tar.gz` & `tmp/AsyncKandinsky-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AsyncKandinsky-0.0.2.tar", last modified: Sun Apr  7 09:57:52 2024, max compression
+gzip compressed data, was "dist/AsyncKandinsky-0.0.3.tar", last modified: Sun Apr  7 10:03:53 2024, max compression
```

## Comparing `AsyncKandinsky-0.0.2.tar` & `AsyncKandinsky-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 09:57:52.816323 AsyncKandinsky-0.0.2/
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 09:57:52.812373 AsyncKandinsky-0.0.2/AsyncKandinsky/
--rw-r--r--   0 s1rne      (503) staff       (20)      346 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.2/AsyncKandinsky/API_types.py
--rw-r--r--   0 s1rne      (503) staff       (20)      388 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.2/AsyncKandinsky/URLS.py
--rw-r--r--   0 s1rne      (503) staff       (20)       32 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.2/AsyncKandinsky/__init__.py
--rw-r--r--   0 s1rne      (503) staff       (20)     3717 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.2/AsyncKandinsky/api.py
-drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 09:57:52.815433 AsyncKandinsky-0.0.2/AsyncKandinsky.egg-info/
--rw-r--r--   0 s1rne      (503) staff       (20)     1860 2024-04-07 09:57:52.000000 AsyncKandinsky-0.0.2/AsyncKandinsky.egg-info/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 09:57:52.000000 AsyncKandinsky-0.0.2/AsyncKandinsky.egg-info/SOURCES.txt
--rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 09:57:52.000000 AsyncKandinsky-0.0.2/AsyncKandinsky.egg-info/dependency_links.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 09:57:52.000000 AsyncKandinsky-0.0.2/AsyncKandinsky.egg-info/requires.txt
--rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 09:57:52.000000 AsyncKandinsky-0.0.2/AsyncKandinsky.egg-info/top_level.txt
--rw-r--r--   0 s1rne      (503) staff       (20)     1860 2024-04-07 09:57:52.816119 AsyncKandinsky-0.0.2/PKG-INFO
--rw-r--r--   0 s1rne      (503) staff       (20)     1192 2024-03-30 18:33:11.000000 AsyncKandinsky-0.0.2/README.md
--rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 09:57:52.816999 AsyncKandinsky-0.0.2/setup.cfg
--rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 09:54:36.000000 AsyncKandinsky-0.0.2/setup.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:03:53.020861 AsyncKandinsky-0.0.3/
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:03:53.014455 AsyncKandinsky-0.0.3/AsyncKandinsky/
+-rw-r--r--   0 s1rne      (503) staff       (20)      346 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/API_types.py
+-rw-r--r--   0 s1rne      (503) staff       (20)      388 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/URLS.py
+-rw-r--r--   0 s1rne      (503) staff       (20)       57 2024-04-07 10:03:51.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/__init__.py
+-rw-r--r--   0 s1rne      (503) staff       (20)     3717 2024-04-07 09:57:30.000000 AsyncKandinsky-0.0.3/AsyncKandinsky/api.py
+drwxr-xr-x   0 s1rne      (503) staff       (20)        0 2024-04-07 10:03:53.019568 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/
+-rw-r--r--   0 s1rne      (503) staff       (20)     1859 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)      317 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/SOURCES.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)        1 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/dependency_links.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       30 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/requires.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)       15 2024-04-07 10:03:52.000000 AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/top_level.txt
+-rw-r--r--   0 s1rne      (503) staff       (20)     1859 2024-04-07 10:03:53.020530 AsyncKandinsky-0.0.3/PKG-INFO
+-rw-r--r--   0 s1rne      (503) staff       (20)     1191 2024-04-07 10:00:00.000000 AsyncKandinsky-0.0.3/README.md
+-rw-r--r--   0 s1rne      (503) staff       (20)       38 2024-04-07 10:03:53.022036 AsyncKandinsky-0.0.3/setup.cfg
+-rw-r--r--   0 s1rne      (503) staff       (20)      940 2024-04-07 10:03:51.000000 AsyncKandinsky-0.0.3/setup.py
```

### Comparing `AsyncKandinsky-0.0.2/AsyncKandinsky/api.py` & `AsyncKandinsky-0.0.3/AsyncKandinsky/api.py`

 * *Files identical despite different names*

### Comparing `AsyncKandinsky-0.0.2/AsyncKandinsky.egg-info/PKG-INFO` & `AsyncKandinsky-0.0.3/AsyncKandinsky.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 0.0.2
+Version: 0.0.3
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -49,9 +49,8 @@
 
 ```
 async def read_styles():
     for style in await model.get_styles():
         print(style, end="\n\n")
 ```
 
-
 ![Пример генерации](https://github.com/s1rne/kandinsky-async-api/blob/main/cat_anime.jpg)
```

### Comparing `AsyncKandinsky-0.0.2/PKG-INFO` & `AsyncKandinsky-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AsyncKandinsky
-Version: 0.0.2
+Version: 0.0.3
 Summary: This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.
 Home-page: https://github.com/s1rne/kandinsky-async-api
 Author: s1rne
 Author-email: s.simaranov8@gmail.com
 Project-URL: GitHub, https://github.com/s1rne/kandinsky-async-api
 Keywords: kandinsky text2img async api
 Classifier: Programming Language :: Python :: 3.9
@@ -49,9 +49,8 @@
 
 ```
 async def read_styles():
     for style in await model.get_styles():
         print(style, end="\n\n")
 ```
 
-
 ![Пример генерации](https://github.com/s1rne/kandinsky-async-api/blob/main/cat_anime.jpg)
```

### Comparing `AsyncKandinsky-0.0.2/README.md` & `AsyncKandinsky-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -32,9 +32,8 @@
 
 ```
 async def read_styles():
     for style in await model.get_styles():
         print(style, end="\n\n")
 ```
 
-
 ![Пример генерации](https://github.com/s1rne/kandinsky-async-api/blob/main/cat_anime.jpg)
```

### Comparing `AsyncKandinsky-0.0.2/setup.py` & `AsyncKandinsky-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='AsyncKandinsky',
-    version='0.0.2',
+    version='0.0.3',
     author='s1rne',
     author_email='s.simaranov8@gmail.com',
     description='This module is designed for asynchronous use of the kandinsky neural network and easy integration into your project.',
     long_description=readme(),
     long_description_content_type='text/markdown',
     url='https://github.com/s1rne/kandinsky-async-api',
     packages=find_packages(),
```

