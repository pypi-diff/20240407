# Comparing `tmp/molecularnetwork-0.3.5.tar.gz` & `tmp/molecularnetwork-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecularnetwork-0.3.5.tar", last modified: Thu Apr  4 12:54:06 2024, max compression
+gzip compressed data, was "molecularnetwork-0.3.6.tar", last modified: Sun Apr  7 16:57:49 2024, max compression
```

## Comparing `molecularnetwork-0.3.5.tar` & `molecularnetwork-0.3.6.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.120922 molecularnetwork-0.3.5/
--rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.5/.gitignore
--rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.5/LICENSE
--rw-r--r--   0 manasmahale   (501) staff       (20)     2191 2024-04-04 12:54:06.120725 molecularnetwork-0.3.5/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)     1768 2024-03-14 18:27:39.000000 molecularnetwork-0.3.5/README.md
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.117354 molecularnetwork-0.3.5/molecularnetwork/
--rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/__init__.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/featurizer.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     2643 2024-04-04 12:45:51.000000 molecularnetwork-0.3.5/molecularnetwork/graph.py
--rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/similarity.py
--rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/molecularnetwork/utils.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.120489 molecularnetwork-0.3.5/molecularnetwork.egg-info/
--rw-r--r--   0 manasmahale   (501) staff       (20)     2191 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/PKG-INFO
--rw-r--r--   0 manasmahale   (501) staff       (20)      441 2024-04-04 12:54:06.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/SOURCES.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/dependency_links.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/requires.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-04 12:54:05.000000 molecularnetwork-0.3.5/molecularnetwork.egg-info/top_level.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.5/requirements.txt
--rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-04 12:54:06.120964 molecularnetwork-0.3.5/setup.cfg
--rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-04 12:52:49.000000 molecularnetwork-0.3.5/setup.py
-drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-04 12:54:06.120220 molecularnetwork-0.3.5/test/
--rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.5/test/test.csv
--rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/test/test.gpickle
--rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.5/test/test.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 16:57:49.843355 molecularnetwork-0.3.6/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     3096 2024-03-14 17:33:16.000000 molecularnetwork-0.3.6/.gitignore
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1069 2023-12-23 10:06:00.000000 molecularnetwork-0.3.6/LICENSE
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2347 2024-04-07 16:57:49.843148 molecularnetwork-0.3.6/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1924 2024-04-04 13:06:13.000000 molecularnetwork-0.3.6/README.md
+-rw-r--r--   0 manasmahale   (501) staff       (20)   634211 2024-04-04 13:05:55.000000 molecularnetwork-0.3.6/banner.png
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 16:57:49.841666 molecularnetwork-0.3.6/molecularnetwork/
+-rw-r--r--   0 manasmahale   (501) staff       (20)       36 2024-03-14 16:51:27.000000 molecularnetwork-0.3.6/molecularnetwork/__init__.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1055 2024-03-14 16:51:27.000000 molecularnetwork-0.3.6/molecularnetwork/featurizer.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2699 2024-04-07 16:56:12.000000 molecularnetwork-0.3.6/molecularnetwork/graph.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)     1142 2024-03-14 16:51:27.000000 molecularnetwork-0.3.6/molecularnetwork/similarity.py
+-rw-r--r--   0 manasmahale   (501) staff       (20)      222 2024-03-14 16:51:27.000000 molecularnetwork-0.3.6/molecularnetwork/utils.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 16:57:49.842906 molecularnetwork-0.3.6/molecularnetwork.egg-info/
+-rw-r--r--   0 manasmahale   (501) staff       (20)     2347 2024-04-07 16:57:49.000000 molecularnetwork-0.3.6/molecularnetwork.egg-info/PKG-INFO
+-rw-r--r--   0 manasmahale   (501) staff       (20)      452 2024-04-07 16:57:49.000000 molecularnetwork-0.3.6/molecularnetwork.egg-info/SOURCES.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)        1 2024-04-07 16:57:49.000000 molecularnetwork-0.3.6/molecularnetwork.egg-info/dependency_links.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       28 2024-04-07 16:57:49.000000 molecularnetwork-0.3.6/molecularnetwork.egg-info/requires.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       17 2024-04-07 16:57:49.000000 molecularnetwork-0.3.6/molecularnetwork.egg-info/top_level.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       60 2024-03-14 16:49:26.000000 molecularnetwork-0.3.6/requirements.txt
+-rw-r--r--   0 manasmahale   (501) staff       (20)       38 2024-04-07 16:57:49.843395 molecularnetwork-0.3.6/setup.cfg
+-rw-r--r--   0 manasmahale   (501) staff       (20)      660 2024-04-07 16:57:16.000000 molecularnetwork-0.3.6/setup.py
+drwxr-xr-x   0 manasmahale   (501) staff       (20)        0 2024-04-07 16:57:49.842736 molecularnetwork-0.3.6/test/
+-rw-rw-r--   0 manasmahale   (501) staff       (20)    86430 2023-03-09 05:52:27.000000 molecularnetwork-0.3.6/test/test.csv
+-rw-r--r--   0 manasmahale   (501) staff       (20)   101028 2024-03-14 16:51:27.000000 molecularnetwork-0.3.6/test/test.gpickle
+-rw-r--r--   0 manasmahale   (501) staff       (20)      278 2024-03-14 16:51:27.000000 molecularnetwork-0.3.6/test/test.py
```

### Comparing `molecularnetwork-0.3.5/.gitignore` & `molecularnetwork-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.5/LICENSE` & `molecularnetwork-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.5/PKG-INFO` & `molecularnetwork-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: networkx
 Requires-Dist: rdkit
 Requires-Dist: joblib
 
 # MolecularNetwork
+![banner](banner.png)
 
 `MolecularNetwork` is a Python package that facilitates the creation of molecular networks based on molecular similarities. It leverages RDKit for molecular operations, and NetworkX for graph operations.
 
 ## Features
 
 - **Molecular Descriptors:** Calculate molecular fingerprints using descriptor types (e.g., Morgan fingerprints, MACCS keys, AtomPairs).
 
@@ -39,19 +40,22 @@
 from molecularnetwork import MolecularNetwork
 
 # Define SMILES strings and classes
 smiles_list = ["CCO", "CCN", "CCC", "CCF"]
 classes = ["alcohol", "amine", "alkane", "fluoride"]
 
 # Create MolecularNetwork instance
-network = MolecularNetwork(descriptor="morgan2", sim_metric="tanimoto", sim_threshold=0.5)
+network = MolecularNetwork(descriptor="morgan2", sim_metric="tanimoto", sim_threshold=0.25)
 
 # Generate the molecular network graph
 graph = network.create_graph(smiles_list, classes) # network.get_graph() also returns graph
 
+graph[0][1]['weight'] # Returns the edge weight attribute which is the similarity between node 0 and 1
+# Returns 0.3333333333333333
+
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
 graph = network.read_graph("test_molecular_network.joblib")
 ```
```

### Comparing `molecularnetwork-0.3.5/README.md` & `molecularnetwork-0.3.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # MolecularNetwork
+![banner](banner.png)
 
 `MolecularNetwork` is a Python package that facilitates the creation of molecular networks based on molecular similarities. It leverages RDKit for molecular operations, and NetworkX for graph operations.
 
 ## Features
 
 - **Molecular Descriptors:** Calculate molecular fingerprints using descriptor types (e.g., Morgan fingerprints, MACCS keys, AtomPairs).
 
@@ -25,19 +26,22 @@
 from molecularnetwork import MolecularNetwork
 
 # Define SMILES strings and classes
 smiles_list = ["CCO", "CCN", "CCC", "CCF"]
 classes = ["alcohol", "amine", "alkane", "fluoride"]
 
 # Create MolecularNetwork instance
-network = MolecularNetwork(descriptor="morgan2", sim_metric="tanimoto", sim_threshold=0.5)
+network = MolecularNetwork(descriptor="morgan2", sim_metric="tanimoto", sim_threshold=0.25)
 
 # Generate the molecular network graph
 graph = network.create_graph(smiles_list, classes) # network.get_graph() also returns graph
 
+graph[0][1]['weight'] # Returns the edge weight attribute which is the similarity between node 0 and 1
+# Returns 0.3333333333333333
+
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
 graph = network.read_graph("test_molecular_network.joblib")
 ```
```

### Comparing `molecularnetwork-0.3.5/molecularnetwork/featurizer.py` & `molecularnetwork-0.3.6/molecularnetwork/featurizer.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.5/molecularnetwork/graph.py` & `molecularnetwork-0.3.6/molecularnetwork/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.fingerprint_calculator = FingerprintCalculator(descriptor)
         self.similarity_calculator = SimilarityCalculator(sim_metric)
         self.graph = networkx.Graph()
 
     def _create_graph(self, smiles_list, classes):
         fps = self._calculate_fingerprints(smiles_list)
         unique_classes, categorical_labels = self._convert_classes(classes)
-        self._add_nodes(smiles_list, unique_classes, categorical_labels)
+        self._add_nodes(smiles_list, fps, unique_classes, categorical_labels)
         self._add_edges(fps)
 
     def _calculate_fingerprints(self, smiles_list):
         return [
             self.fingerprint_calculator.calculate_fingerprint(smi)
             for smi in smiles_list
         ]
@@ -30,23 +30,24 @@
         unique_classes = np.unique(classes)
         categorical_labels = np.arange(len(unique_classes))
         class_labels = np.array(
             [categorical_labels[np.where(unique_classes == c)[0][0]] for c in classes]
         )
         return unique_classes, class_labels
 
-    def _add_nodes(self, smiles_list, unique_classes, categorical_labels):
+    def _add_nodes(self, smiles_list, fps, unique_classes, categorical_labels):
         num_nodes = len(smiles_list)
         nodes = range(num_nodes)
         weighted_nodes = [
             (
                 node,
                 {
                     "smiles": smiles_list[node],
                     "categorical_label": str(unique_classes[value]),
+                    "fp": np.array(fps[node])
                 },
             )
             for node, value in zip(nodes, categorical_labels)
         ]
         self.graph.add_nodes_from(weighted_nodes)
 
     def _add_edges(self, fps):
```

### Comparing `molecularnetwork-0.3.5/molecularnetwork/similarity.py` & `molecularnetwork-0.3.6/molecularnetwork/similarity.py`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.5/molecularnetwork.egg-info/PKG-INFO` & `molecularnetwork-0.3.6/molecularnetwork.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: molecularnetwork
-Version: 0.3.5
+Version: 0.3.6
 Summary: A package for creating molecular networks based on molecular features and similarities.
 Home-page: https://github.com/Manas02/molecularnetwork
 Author: Manas Mahale
 Author-email: manas.m.mahale@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: networkx
 Requires-Dist: rdkit
 Requires-Dist: joblib
 
 # MolecularNetwork
+![banner](banner.png)
 
 `MolecularNetwork` is a Python package that facilitates the creation of molecular networks based on molecular similarities. It leverages RDKit for molecular operations, and NetworkX for graph operations.
 
 ## Features
 
 - **Molecular Descriptors:** Calculate molecular fingerprints using descriptor types (e.g., Morgan fingerprints, MACCS keys, AtomPairs).
 
@@ -39,19 +40,22 @@
 from molecularnetwork import MolecularNetwork
 
 # Define SMILES strings and classes
 smiles_list = ["CCO", "CCN", "CCC", "CCF"]
 classes = ["alcohol", "amine", "alkane", "fluoride"]
 
 # Create MolecularNetwork instance
-network = MolecularNetwork(descriptor="morgan2", sim_metric="tanimoto", sim_threshold=0.5)
+network = MolecularNetwork(descriptor="morgan2", sim_metric="tanimoto", sim_threshold=0.25)
 
 # Generate the molecular network graph
 graph = network.create_graph(smiles_list, classes) # network.get_graph() also returns graph
 
+graph[0][1]['weight'] # Returns the edge weight attribute which is the similarity between node 0 and 1
+# Returns 0.3333333333333333
+
 # Save the graph to a file
 network.save_graph("test_molecular_network.joblib")
 
 # Read graph from a file
 graph = network.read_graph("test_molecular_network.joblib")
 ```
```

### Comparing `molecularnetwork-0.3.5/setup.py` & `molecularnetwork-0.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(
     name="molecularnetwork",
-    version="0.3.5",
+    version="0.3.6",
     packages=find_packages(),
     install_requires=[
         "numpy",
         "networkx",
         "rdkit",
         "joblib",
     ],
```

### Comparing `molecularnetwork-0.3.5/test/test.csv` & `molecularnetwork-0.3.6/test/test.csv`

 * *Files identical despite different names*

### Comparing `molecularnetwork-0.3.5/test/test.gpickle` & `molecularnetwork-0.3.6/test/test.gpickle`

 * *Files identical despite different names*

