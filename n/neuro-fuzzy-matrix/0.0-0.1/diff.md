# Comparing `tmp/neuro_fuzzy_matrix-0.0.tar.gz` & `tmp/neuro_fuzzy_matrix-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuro_fuzzy_matrix-0.0.tar", last modified: Tue Mar 26 18:53:13 2024, max compression
+gzip compressed data, was "neuro_fuzzy_matrix-0.1.tar", last modified: Sun Apr  7 17:25:30 2024, max compression
```

## Comparing `neuro_fuzzy_matrix-0.0.tar` & `neuro_fuzzy_matrix-0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 18:53:13.943672 neuro_fuzzy_matrix-0.0/
--rw-rw-rw-   0        0        0      127 2024-03-26 18:53:13.944672 neuro_fuzzy_matrix-0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4099 2024-03-26 17:51:24.000000 neuro_fuzzy_matrix-0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 18:53:13.932268 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/
--rw-rw-rw-   0        0        0    22871 2024-03-26 14:30:15.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/__init__.py
--rw-rw-rw-   0        0        0      547 2024-03-26 16:57:26.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/test_save.py
--rw-rw-rw-   0        0        0     1960 2024-03-26 14:31:04.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/tests_full.py
--rw-rw-rw-   0        0        0     2820 2024-03-26 16:55:01.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/tests_not_rules.py
-drwxrwxrwx   0        0        0        0 2024-03-26 18:53:13.942681 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix.egg-info/
--rw-rw-rw-   0        0        0      127 2024-03-26 18:53:13.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      371 2024-03-26 18:53:13.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 18:53:13.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-26 18:53:13.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2024-03-26 18:53:13.000000 neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-26 18:53:13.948656 neuro_fuzzy_matrix-0.0/setup.cfg
--rw-rw-rw-   0        0        0      235 2024-03-26 18:03:35.000000 neuro_fuzzy_matrix-0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:25:30.348219 neuro_fuzzy_matrix-0.1/
+-rw-rw-rw-   0        0        0      127 2024-04-07 17:25:30.348219 neuro_fuzzy_matrix-0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4099 2024-03-26 17:51:24.000000 neuro_fuzzy_matrix-0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 17:25:30.331378 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/
+-rw-rw-rw-   0        0        0    22957 2024-04-07 17:24:26.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/__init__.py
+-rw-rw-rw-   0        0        0      547 2024-03-26 16:57:26.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/test_save.py
+-rw-rw-rw-   0        0        0     1960 2024-03-26 14:31:04.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_full.py
+-rw-rw-rw-   0        0        0     2820 2024-03-26 16:55:01.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_not_rules.py
+drwxrwxrwx   0        0        0        0 2024-04-07 17:25:30.346224 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/
+-rw-rw-rw-   0        0        0      127 2024-04-07 17:25:29.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-07 17:25:30.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 17:25:30.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-07 17:25:29.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2024-04-07 17:25:30.000000 neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 17:25:30.350214 neuro_fuzzy_matrix-0.1/setup.cfg
+-rw-rw-rw-   0        0        0      235 2024-03-28 09:49:21.000000 neuro_fuzzy_matrix-0.1/setup.py
```

### Comparing `neuro_fuzzy_matrix-0.0/README.md` & `neuro_fuzzy_matrix-0.1/README.md`

 * *Files identical despite different names*

### Comparing `neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/__init__.py` & `neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -252,15 +252,16 @@
                     index = next(((i, j) for i, sublist in enumerate(self.term_in) for j, elem in enumerate(sublist) if elem == term), None)
                     rules_i[i][index[0]]=index[1]
 
             self.rules = np.array(rules_i)
         elif self.algorithm=="Not rules":
             self.rules = np.array(list(itertools.product(*self.FuncsByVariable))) 
 
-        self.weights = np.random.randn(self.Y.ndim,len(self.rules))
+        self.weights = np.random.uniform(50, 100, ((self.Y.ndim,len(self.rules))))
+        # self.weights = np.random.randn(self.Y.ndim,len(self.rules))
         # self.biases = np.zeros((self.Y.ndim, len(self.X[:,0])))
         self.biases = np.random.randn(self.Y.ndim, len(self.X[:,0]))
 
     # функция обучения сети 
     def train(self, epochs=5, tolerance=1e-1, k=0.01):
         self.initialize_parameters()
         convergence = False
```

### Comparing `neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/test_save.py` & `neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/test_save.py`

 * *Files identical despite different names*

### Comparing `neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/tests_full.py` & `neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_full.py`

 * *Files identical despite different names*

### Comparing `neuro_fuzzy_matrix-0.0/neuro_fuzzy_matrix/tests_not_rules.py` & `neuro_fuzzy_matrix-0.1/neuro_fuzzy_matrix/tests_not_rules.py`

 * *Files identical despite different names*

