# Comparing `tmp/matplotlib_visual-0.7.1.tar.gz` & `tmp/matplotlib_visual-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_visual-0.7.1.tar", last modified: Fri Mar 29 07:19:51 2024, max compression
+gzip compressed data, was "matplotlib_visual-0.8.tar", last modified: Sun Apr  7 12:05:40 2024, max compression
```

## Comparing `matplotlib_visual-0.7.1.tar` & `matplotlib_visual-0.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-03-29 07:19:51.092651 matplotlib_visual-0.7.1/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-01-30 14:32:10.000000 matplotlib_visual-0.7.1/LICENSE
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-03-29 07:19:51.091651 matplotlib_visual-0.7.1/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-03-29 07:11:10.000000 matplotlib_visual-0.7.1/README.md
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-03-29 07:19:51.087651 matplotlib_visual-0.7.1/matplotlib_visual/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 14:35:01.000000 matplotlib_visual-0.7.1/matplotlib_visual/__init__.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-03-29 07:19:51.091651 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 15:02:02.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/__init__.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      568 2024-03-29 07:18:38.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/god.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-02-04 07:14:39.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir1.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      624 2024-02-04 07:15:04.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      540 2024-02-04 07:15:26.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      687 2024-02-04 07:16:22.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 14:59:27.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3301 2024-03-13 15:24:02.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir5full.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1225 2024-03-13 15:05:07.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-03-13 15:10:30.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 15:03:11.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1627 2024-03-25 16:16:08.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml10.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1286 2024-03-25 16:17:51.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml11a.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      964 2024-03-25 16:16:51.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml11b.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1048 2024-02-09 02:10:52.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1814 2024-02-04 07:18:54.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1303 2024-02-04 07:27:56.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1472 2024-03-10 08:55:11.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3789 2024-03-25 16:15:24.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      742 2024-03-25 16:15:35.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1195 2024-03-25 16:15:45.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1279 2024-03-25 16:15:57.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml9.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      827 2024-02-07 16:23:02.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd1.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1379 2024-03-10 11:13:25.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd10.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1563 2024-02-07 16:24:37.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd2.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1005 2024-02-04 07:24:53.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd22.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      533 2024-02-07 16:25:05.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd3.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     2591 2024-03-10 08:52:46.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd4.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3452 2024-03-10 08:53:15.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd5.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     2138 2024-03-10 08:53:36.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd6.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      749 2024-03-10 08:53:46.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd7.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1399 2024-03-10 09:06:06.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd8.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1976 2024-03-10 09:05:40.000000 matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd9.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1470 2024-03-16 13:53:07.000000 matplotlib_visual-0.7.1/matplotlib_visual/graph.py
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-03-16 13:23:06.000000 matplotlib_visual-0.7.1/matplotlib_visual/models.py
-drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-03-29 07:19:51.091651 matplotlib_visual-0.7.1/matplotlib_visual.egg-info/
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      212 2024-03-29 07:19:51.000000 matplotlib_visual-0.7.1/matplotlib_visual.egg-info/PKG-INFO
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1589 2024-03-29 07:19:51.000000 matplotlib_visual-0.7.1/matplotlib_visual.egg-info/SOURCES.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-03-29 07:19:51.000000 matplotlib_visual-0.7.1/matplotlib_visual.egg-info/dependency_links.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-03-29 07:19:51.000000 matplotlib_visual-0.7.1/matplotlib_visual.egg-info/top_level.txt
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-03-29 07:19:51.093651 matplotlib_visual-0.7.1/setup.cfg
--rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      333 2024-03-29 07:19:32.000000 matplotlib_visual-0.7.1/setup.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-07 12:05:40.044417 matplotlib_visual-0.8/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)    35149 2024-01-30 14:32:10.000000 matplotlib_visual-0.8/LICENSE
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      210 2024-04-07 12:05:40.043417 matplotlib_visual-0.8/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1753 2024-03-29 07:11:10.000000 matplotlib_visual-0.8/README.md
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-07 12:05:40.034417 matplotlib_visual-0.8/matplotlib_visual/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 14:35:01.000000 matplotlib_visual-0.8/matplotlib_visual/__init__.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-07 12:05:40.042417 matplotlib_visual-0.8/matplotlib_visual/code_snippets/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-01-30 15:02:02.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/__init__.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      568 2024-03-29 07:18:38.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/god.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-02-04 07:14:39.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir1.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      624 2024-02-04 07:15:04.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir2.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      540 2024-02-04 07:15:26.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir3.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      687 2024-02-04 07:16:22.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir4.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 14:59:27.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir5.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3301 2024-03-13 15:24:02.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir5full.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1225 2024-03-13 15:05:07.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir6.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      542 2024-03-13 15:10:30.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir7.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      912 2024-03-13 15:03:11.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir8.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1627 2024-03-25 16:16:08.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml10.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1286 2024-03-25 16:17:51.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml11a.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      964 2024-03-25 16:16:51.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml11b.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1048 2024-02-09 02:10:52.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml2.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1814 2024-02-04 07:18:54.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml3.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1303 2024-02-04 07:27:56.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml4.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1472 2024-03-10 08:55:11.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml5.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3789 2024-03-25 16:15:24.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml6.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      742 2024-03-25 16:15:35.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml7.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1195 2024-03-25 16:15:45.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml8.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1279 2024-03-25 16:15:57.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml9.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      827 2024-02-07 16:23:02.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd1.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1379 2024-03-10 11:13:25.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd10.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1563 2024-02-07 16:24:37.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd2.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1005 2024-02-04 07:24:53.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd22.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      533 2024-02-07 16:25:05.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd3.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     2591 2024-03-10 08:52:46.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd4.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     3452 2024-03-10 08:53:15.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd5.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     2138 2024-03-10 08:53:36.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd6.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      749 2024-03-10 08:53:46.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd7.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1399 2024-03-10 09:06:06.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd8.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1976 2024-03-10 09:05:40.000000 matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd9.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      655 2024-04-07 11:58:48.000000 matplotlib_visual-0.8/matplotlib_visual/graph.py
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      252 2024-03-16 13:23:06.000000 matplotlib_visual-0.8/matplotlib_visual/models.py
+drwxr-xr-x   0 thisisyaash  (1000) thisisyaash  (1000)        0 2024-04-07 12:05:40.043417 matplotlib_visual-0.8/matplotlib_visual.egg-info/
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      210 2024-04-07 12:05:39.000000 matplotlib_visual-0.8/matplotlib_visual.egg-info/PKG-INFO
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)     1589 2024-04-07 12:05:39.000000 matplotlib_visual-0.8/matplotlib_visual.egg-info/SOURCES.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)        1 2024-04-07 12:05:39.000000 matplotlib_visual-0.8/matplotlib_visual.egg-info/dependency_links.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       18 2024-04-07 12:05:39.000000 matplotlib_visual-0.8/matplotlib_visual.egg-info/top_level.txt
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)       38 2024-04-07 12:05:40.044417 matplotlib_visual-0.8/setup.cfg
+-rw-r--r--   0 thisisyaash  (1000) thisisyaash  (1000)      331 2024-04-07 12:00:10.000000 matplotlib_visual-0.8/setup.py
```

### Comparing `matplotlib_visual-0.7.1/LICENSE` & `matplotlib_visual-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/README.md` & `matplotlib_visual-0.8/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/god.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/god.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir1.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir1.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir2.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir2.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir3.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir3.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir4.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir4.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir5.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir5.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir5full.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir5full.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir6.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir6.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir7.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir7.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ir8.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ir8.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml10.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml10.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml11a.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml11a.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml11b.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml11b.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml2.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml2.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml3.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml3.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml4.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml4.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml5.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml5.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml6.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml6.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml7.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml7.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml8.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml8.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/ml9.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/ml9.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd1.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd1.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd10.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd10.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd2.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd2.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd22.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd22.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd3.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd3.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd4.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd4.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd5.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd5.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd6.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd6.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd7.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd7.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd8.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd8.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual/code_snippets/pcd9.py` & `matplotlib_visual-0.8/matplotlib_visual/code_snippets/pcd9.py`

 * *Files identical despite different names*

### Comparing `matplotlib_visual-0.7.1/matplotlib_visual.egg-info/SOURCES.txt` & `matplotlib_visual-0.8/matplotlib_visual.egg-info/SOURCES.txt`

 * *Files identical despite different names*

