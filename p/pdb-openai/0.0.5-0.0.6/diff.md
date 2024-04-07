# Comparing `tmp/pdb_openai-0.0.5.tar.gz` & `tmp/pdb_openai-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb_openai-0.0.5.tar", last modified: Sat Apr  6 22:31:32 2024, max compression
+gzip compressed data, was "pdb_openai-0.0.6.tar", last modified: Sun Apr  7 02:59:09 2024, max compression
```

## Comparing `pdb_openai-0.0.5.tar` & `pdb_openai-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 22:31:32.500643 pdb_openai-0.0.5/
--rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 pdb_openai-0.0.5/LICENSE
--rw-r--r--   0 jordan     (501) staff       (20)     2544 2024-04-06 22:31:32.500539 pdb_openai-0.0.5/PKG-INFO
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 22:31:32.499779 pdb_openai-0.0.5/pdb_openai/
--rw-r--r--   0 jordan     (501) staff       (20)       21 2024-04-06 22:25:07.000000 pdb_openai-0.0.5/pdb_openai/__init__.py
--rw-r--r--   0 jordan     (501) staff       (20)     3499 2024-04-06 22:19:56.000000 pdb_openai-0.0.5/pdb_openai/debug.py
-drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-06 22:31:32.500399 pdb_openai-0.0.5/pdb_openai.egg-info/
--rw-r--r--   0 jordan     (501) staff       (20)     2544 2024-04-06 22:31:32.000000 pdb_openai-0.0.5/pdb_openai.egg-info/PKG-INFO
--rw-r--r--   0 jordan     (501) staff       (20)      228 2024-04-06 22:31:32.000000 pdb_openai-0.0.5/pdb_openai.egg-info/SOURCES.txt
--rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-06 22:31:32.000000 pdb_openai-0.0.5/pdb_openai.egg-info/dependency_links.txt
--rw-r--r--   0 jordan     (501) staff       (20)        7 2024-04-06 22:31:32.000000 pdb_openai-0.0.5/pdb_openai.egg-info/requires.txt
--rw-r--r--   0 jordan     (501) staff       (20)       11 2024-04-06 22:31:32.000000 pdb_openai-0.0.5/pdb_openai.egg-info/top_level.txt
--rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-06 22:31:32.500678 pdb_openai-0.0.5/setup.cfg
--rw-r--r--   0 jordan     (501) staff       (20)      660 2024-04-06 22:19:11.000000 pdb_openai-0.0.5/setup.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 02:59:09.844311 pdb_openai-0.0.6/
+-rw-r--r--   0 jordan     (501) staff       (20)     1060 2024-04-05 22:49:53.000000 pdb_openai-0.0.6/LICENSE
+-rw-r--r--   0 jordan     (501) staff       (20)     2623 2024-04-07 02:59:09.844205 pdb_openai-0.0.6/PKG-INFO
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 02:59:09.843562 pdb_openai-0.0.6/pdb_openai/
+-rw-r--r--   0 jordan     (501) staff       (20)       21 2024-04-07 02:28:02.000000 pdb_openai-0.0.6/pdb_openai/__init__.py
+-rw-r--r--   0 jordan     (501) staff       (20)     4270 2024-04-07 02:57:58.000000 pdb_openai-0.0.6/pdb_openai/debug.py
+drwxr-xr-x   0 jordan     (501) staff       (20)        0 2024-04-07 02:59:09.844057 pdb_openai-0.0.6/pdb_openai.egg-info/
+-rw-r--r--   0 jordan     (501) staff       (20)     2623 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/PKG-INFO
+-rw-r--r--   0 jordan     (501) staff       (20)      228 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 jordan     (501) staff       (20)        1 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 jordan     (501) staff       (20)        7 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/requires.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       11 2024-04-07 02:59:09.000000 pdb_openai-0.0.6/pdb_openai.egg-info/top_level.txt
+-rw-r--r--   0 jordan     (501) staff       (20)       38 2024-04-07 02:59:09.844346 pdb_openai-0.0.6/setup.cfg
+-rw-r--r--   0 jordan     (501) staff       (20)      660 2024-04-07 02:27:55.000000 pdb_openai-0.0.6/setup.py
```

### Comparing `pdb_openai-0.0.5/LICENSE` & `pdb_openai-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb_openai-0.0.5/PKG-INFO` & `pdb_openai-0.0.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdb_openai
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python debugger with OpenAI integrations
 Home-page: https://github.com/dustmason/pdb_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -67,9 +67,10 @@
 3. It combined the selected greeting and name with a formatted string to create a message.
 4. Finally, the function printed this message to the console.
 Since the selections are random, the exact output can vary with each call to `greet()`, displaying a greeting and a name randomly chosen from the lists provided.
 ```
 
 ## wtf
 
-This is an alias for `ask` with this prompt: `Explain how the program arrived at this state, including the cause of any errors. Be concise.`
+This is an alias for `ask` with this prompt: `Explain how the program arrived at this state, including the cause of any
+errors. Be concise.` Add one or more `?` chars to the command to provide more context to the model.
```

### Comparing `pdb_openai-0.0.5/pdb_openai.egg-info/PKG-INFO` & `pdb_openai-0.0.6/pdb_openai.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdb-openai
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python debugger with OpenAI integrations
 Home-page: https://github.com/dustmason/pdb_openai
 Author: Jordan Sitkin
 Author-email: jordan@fiftyfootfoghorn.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -67,9 +67,10 @@
 3. It combined the selected greeting and name with a formatted string to create a message.
 4. Finally, the function printed this message to the console.
 Since the selections are random, the exact output can vary with each call to `greet()`, displaying a greeting and a name randomly chosen from the lists provided.
 ```
 
 ## wtf
 
-This is an alias for `ask` with this prompt: `Explain how the program arrived at this state, including the cause of any errors. Be concise.`
+This is an alias for `ask` with this prompt: `Explain how the program arrived at this state, including the cause of any
+errors. Be concise.` Add one or more `?` chars to the command to provide more context to the model.
```

### Comparing `pdb_openai-0.0.5/setup.py` & `pdb_openai-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pdb_openai",
-    version="0.0.5",
+    version="0.0.6",
     author="Jordan Sitkin",
     author_email="jordan@fiftyfootfoghorn.com",
     description="A python debugger with OpenAI integrations",
     long_description=open('readme.md').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dustmason/pdb_openai",
     packages=find_packages(),
```

