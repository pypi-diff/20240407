# Comparing `tmp/memory_graph-0.1.9.tar.gz` & `tmp/memory_graph-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory_graph-0.1.9.tar", last modified: Mon May 22 08:03:45 2023, max compression
+gzip compressed data, was "memory_graph-0.2.0.tar", last modified: Sun Apr  7 18:29:12 2024, max compression
```

## Comparing `memory_graph-0.1.9.tar` & `memory_graph-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,34 @@
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 08:03:45.849437 memory_graph-0.1.9/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2023-05-19 18:17:38.000000 memory_graph-0.1.9/LICENSE.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2023-05-19 18:17:38.000000 memory_graph-0.1.9/MANIFEST.in
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 08:03:45.849437 memory_graph-0.1.9/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4696 2023-05-22 07:47:22.000000 memory_graph-0.1.9/README.md
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 08:03:45.849437 memory_graph-0.1.9/memory_graph/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1538 2023-05-19 18:17:38.000000 memory_graph-0.1.9/memory_graph/Node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      865 2023-05-22 08:03:00.000000 memory_graph-0.1.9/memory_graph/__init__.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5234 2023-05-21 18:05:01.000000 memory_graph-0.1.9/memory_graph/graphviz_nodes.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4302 2023-05-22 08:01:42.000000 memory_graph-0.1.9/memory_graph/rewrite.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1098 2023-05-22 07:43:38.000000 memory_graph-0.1.9/memory_graph/rewrite_to_node.py
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      551 2023-05-19 18:17:38.000000 memory_graph-0.1.9/memory_graph/rewrite_to_string.py
-drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2023-05-22 08:03:45.849437 memory_graph-0.1.9/memory_graph.egg-info/
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5271 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/PKG-INFO
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      388 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/SOURCES.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/dependency_links.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/requires.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2023-05-22 08:03:45.000000 memory_graph-0.1.9/memory_graph.egg-info/top_level.txt
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2023-05-22 08:03:45.849437 memory_graph-0.1.9/setup.cfg
--rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      966 2023-05-22 08:03:08.000000 memory_graph-0.1.9/setup.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-07 18:29:12.275152 memory_graph-0.2.0/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1314 2024-02-16 13:16:53.000000 memory_graph-0.2.0/LICENSE.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       25 2024-02-16 13:16:53.000000 memory_graph-0.2.0/MANIFEST.in
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21116 2024-04-07 18:29:12.275152 memory_graph-0.2.0/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    20451 2024-04-07 18:24:52.000000 memory_graph-0.2.0/README.md
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-07 18:29:12.275152 memory_graph-0.2.0/memory_graph/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     5038 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/HTML_Table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3430 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Memory_Graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3428 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Memory_Visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3168 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      847 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Hidden.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3968 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Key_Value.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2520 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Linear.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3287 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Node_Table.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     3949 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Sliced.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6586 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/Slicer.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     6542 2024-04-07 18:28:19.000000 memory_graph-0.2.0/memory_graph/__init__.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      331 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/config.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2947 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/config_default.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     2400 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/config_helpers.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1340 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/extension_numpy.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      660 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/extension_pandas.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     4903 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/test.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      537 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/test_memory_graph.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      286 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/test_memory_visitor.py
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1944 2024-04-07 17:46:45.000000 memory_graph-0.2.0/memory_graph/utils.py
+drwxrwxr-x   0 bterwijn  (1000) bterwijn  (1000)        0 2024-04-07 18:29:12.275152 memory_graph-0.2.0/memory_graph.egg-info/
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)    21116 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/PKG-INFO
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)      777 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/SOURCES.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        1 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/dependency_links.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)        9 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/requires.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       13 2024-04-07 18:29:12.000000 memory_graph-0.2.0/memory_graph.egg-info/top_level.txt
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)       38 2024-04-07 18:29:12.275152 memory_graph-0.2.0/setup.cfg
+-rw-rw-r--   0 bterwijn  (1000) bterwijn  (1000)     1055 2024-04-07 18:28:38.000000 memory_graph-0.2.0/setup.py
```

### Comparing `memory_graph-0.1.9/LICENSE.txt` & `memory_graph-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `memory_graph-0.1.9/setup.py` & `memory_graph-0.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description_from_readme = (this_directory / "README.md").read_text()
 
 setup(
     name = 'memory_graph',
-    version = '0.1.9',
-    description = 'Draw a graph of your data to see the structure of its references.',
+    version = '0.2.00',
+    description = 'Draws a graph of your data to analyze the structure of its references.',
     long_description = long_description_from_readme,
     long_description_content_type = 'text/markdown',
     readme = 'README.md',
     url = 'https://github.com/bterwijn/memory_graph',
     author = 'Bas Terwijn',
     author_email = 'bterwijn@gmail.com',
     license = 'BSD 2-clause',
     packages = ['memory_graph'],
     install_requires = ['graphviz',],
 
     classifiers = [
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Education',
+        'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',  
         'Programming Language :: Python :: 3',
-        'Topic :: Multimedia :: Graphics',
+        'Topic :: Education',
+        'Topic :: Software Development :: Debuggers',
     ],
 )
```

