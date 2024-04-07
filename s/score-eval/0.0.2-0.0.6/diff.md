# Comparing `tmp/score-eval-0.0.2.tar.gz` & `tmp/score-eval-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\workspace\scoreval\dist\tmptod__qw8\score-eval-0.0.2.tar", last modified: Wed May  4 08:40:38 2022, max compression
+gzip compressed data, was "score-eval-0.0.6.tar", last modified: Sun Apr  7 10:03:28 2024, max compression
```

## Comparing `score-eval-0.0.2.tar` & `score-eval-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/
--rw-rw-rw-   0        0        0     1087 2022-05-01 17:29:39.000000 score-eval-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2275 2022-05-04 08:40:38.000000 score-eval-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1683 2022-05-03 11:15:05.000000 score-eval-0.0.2/README.md
--rw-rw-rw-   0        0        0       95 2022-05-03 06:28:18.000000 score-eval-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      690 2022-05-04 08:40:38.000000 score-eval-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/
--rw-rw-rw-   0        0        0     2275 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/score_eval.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-05-04 08:40:38.000000 score-eval-0.0.2/src/scoreval/
--rw-rw-rw-   0        0        0        0 2022-05-03 06:15:29.000000 score-eval-0.0.2/src/scoreval/__init__.py
--rw-rw-rw-   0        0        0    19608 2022-05-04 08:35:46.000000 score-eval-0.0.2/src/scoreval/scoreval.py
--rw-rw-rw-   0        0        0     2462 2022-05-04 08:36:58.000000 score-eval-0.0.2/src/scoreval/test.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:03:28.799137 score-eval-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2022-05-01 17:29:39.000000 score-eval-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2234 2024-04-07 10:03:28.797143 score-eval-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1683 2022-05-03 11:15:05.000000 score-eval-0.0.6/README.md
+-rw-rw-rw-   0        0        0      625 2024-04-07 10:02:15.000000 score-eval-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 10:03:28.799137 score-eval-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 10:03:28.754277 score-eval-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 10:03:28.796144 score-eval-0.0.6/src/score_eval.egg-info/
+-rw-rw-rw-   0        0        0     2234 2024-04-07 10:03:28.000000 score-eval-0.0.6/src/score_eval.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-04-07 10:03:28.000000 score-eval-0.0.6/src/score_eval.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 10:03:28.000000 score-eval-0.0.6/src/score_eval.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-07 10:03:28.000000 score-eval-0.0.6/src/score_eval.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 10:03:28.794149 score-eval-0.0.6/src/scoreval/
+-rw-rw-rw-   0        0        0      679 2024-04-07 09:56:00.000000 score-eval-0.0.6/src/scoreval/__init__.py
+-rw-rw-rw-   0        0        0    25371 2024-04-07 09:55:42.000000 score-eval-0.0.6/src/scoreval/scoreval.py
+-rw-rw-rw-   0        0        0     2462 2022-05-04 08:36:58.000000 score-eval-0.0.6/src/scoreval/test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `score-eval-0.0.2/LICENSE` & `score-eval-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.2/PKG-INFO` & `score-eval-0.0.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: score-eval
-Version: 0.0.2
+Version: 0.0.6
 Summary: A visualization package for model score evaluation.
-Home-page: https://github.com/rexzhang2014/scoreval
-Author: Jingxiao Zhang
-Author-email: rex.zhang2016@foxmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/rexzhang2014/scoreval/issues
-Platform: UNKNOWN
+Author-email: Jingxiao Zhang <rex.zhang2016@foxmail.com>
+Project-URL: Homepage, https://github.com/rexzhang2014/scoreval
+Project-URL: Issues, https://github.com/rexzhang2014/scoreval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scoreval
 An visulized evaluation toolkit for model score. 
 The model score will be evaluated static, on the full dataset. And further evaluate along date. 
 This aims to help machine learning modelers to evaluate the result effictively and efficiently. 
@@ -41,9 +38,7 @@
 # Output
 Pack of charts to evaluate and understand your model. See the link for more details:  
 https://github.com/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
 If it cannot be reached, please try:  
 https://nbviewer.org/github/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
 
 
-
-
```

### Comparing `score-eval-0.0.2/README.md` & `score-eval-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `score-eval-0.0.2/src/score_eval.egg-info/PKG-INFO` & `score-eval-0.0.6/src/score_eval.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: score-eval
-Version: 0.0.2
+Version: 0.0.6
 Summary: A visualization package for model score evaluation.
-Home-page: https://github.com/rexzhang2014/scoreval
-Author: Jingxiao Zhang
-Author-email: rex.zhang2016@foxmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/rexzhang2014/scoreval/issues
-Platform: UNKNOWN
+Author-email: Jingxiao Zhang <rex.zhang2016@foxmail.com>
+Project-URL: Homepage, https://github.com/rexzhang2014/scoreval
+Project-URL: Issues, https://github.com/rexzhang2014/scoreval/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # scoreval
 An visulized evaluation toolkit for model score. 
 The model score will be evaluated static, on the full dataset. And further evaluate along date. 
 This aims to help machine learning modelers to evaluate the result effictively and efficiently. 
@@ -41,9 +38,7 @@
 # Output
 Pack of charts to evaluate and understand your model. See the link for more details:  
 https://github.com/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
 If it cannot be reached, please try:  
 https://nbviewer.org/github/rexzhang2014/scoreval/blob/main/tests/score-eval-example.ipynb  
 
 
-
-
```

### Comparing `score-eval-0.0.2/src/scoreval/test.py` & `score-eval-0.0.6/src/scoreval/test.py`

 * *Files identical despite different names*

