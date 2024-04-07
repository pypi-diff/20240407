# Comparing `tmp/falcondale-0.2.3.tar.gz` & `tmp/falcondale-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falcondale-0.2.3.tar", last modified: Sun Dec 31 15:18:40 2023, max compression
+gzip compressed data, was "falcondale-0.2.4.tar", last modified: Sun Apr  7 10:03:27 2024, max compression
```

## Comparing `falcondale-0.2.3.tar` & `falcondale-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      816 2023-12-31 15:18:24.167835 falcondale-0.2.3/README.md
--rw-r--r--   0        0        0       97 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/__init__.py
--rw-r--r--   0        0        0     4444 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/classifiers.py
--rw-r--r--   0        0        0     1455 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/clustering.py
--rw-r--r--   0        0        0     7100 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/data.py
--rw-r--r--   0        0        0     6821 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/feature_selection.py
--rw-r--r--   0        0        0        0 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/helpers/__init__.py
--rw-r--r--   0        0        0      474 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/helpers/kernels.py
--rw-r--r--   0        0        0     1761 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/helpers/mutual_information.py
--rw-r--r--   0        0        0     7374 2023-12-31 15:18:24.171835 falcondale-0.2.3/falcondale/helpers/qnn.py
--rw-r--r--   0        0        0     3362 2023-12-31 15:18:24.175835 falcondale-0.2.3/falcondale/helpers/qsvc.py
--rw-r--r--   0        0        0    14213 2023-12-31 15:18:24.175835 falcondale-0.2.3/falcondale/main.py
--rw-r--r--   0        0        0      931 2023-12-31 15:18:24.175835 falcondale-0.2.3/falcondale/solvers.py
--rw-r--r--   0        0        0     2166 2023-12-31 15:18:40.631852 falcondale-0.2.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-31 15:18:24.175835 falcondale-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0      771 2023-12-31 15:18:24.175835 falcondale-0.2.3/tests/test_main.py
--rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 falcondale-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      816 2024-04-07 10:03:10.042445 falcondale-0.2.4/README.md
+-rw-r--r--   0        0        0       97 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/__init__.py
+-rw-r--r--   0        0        0     4446 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/classifiers.py
+-rw-r--r--   0        0        0     1442 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/clustering.py
+-rw-r--r--   0        0        0     6953 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/data.py
+-rw-r--r--   0        0        0     6704 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/feature_selection.py
+-rw-r--r--   0        0        0        0 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/helpers/__init__.py
+-rw-r--r--   0        0        0      474 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/helpers/kernels.py
+-rw-r--r--   0        0        0     1762 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/helpers/mutual_information.py
+-rw-r--r--   0        0        0     7375 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/helpers/qnn.py
+-rw-r--r--   0        0        0     3363 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/helpers/qsvc.py
+-rw-r--r--   0        0        0    14219 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/main.py
+-rw-r--r--   0        0        0      932 2024-04-07 10:03:10.050445 falcondale-0.2.4/falcondale/solvers.py
+-rw-r--r--   0        0        0     2167 2024-04-07 10:03:27.878369 falcondale-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-07 10:03:10.050445 falcondale-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0      771 2024-04-07 10:03:10.050445 falcondale-0.2.4/tests/test_main.py
+-rw-r--r--   0        0        0     1787 1970-01-01 00:00:00.000000 falcondale-0.2.4/PKG-INFO
```

### Comparing `falcondale-0.2.3/README.md` & `falcondale-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `falcondale-0.2.3/falcondale/classifiers.py` & `falcondale-0.2.4/falcondale/classifiers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """
 Module implementing the classification methods
 """
+
 from .helpers.qnn import QNN
 from .helpers.qsvc import QSVC
 from .data import Dataset
 
 from sklearn.svm import SVC
 from sklearn.metrics import classification_report, roc_auc_score, confusion_matrix
 
 from qiskit.primitives import Sampler
 from qiskit.circuit.library import ZZFeatureMap
-from qiskit.algorithms.state_fidelities import ComputeUncompute
+from qiskit_algorithms.state_fidelities import ComputeUncompute
 
 from qiskit_machine_learning.kernels import FidelityQuantumKernel
 from qiskit_machine_learning.algorithms import QSVC as qiskitQSVC
 
 
 class TooManyQubitsNeeded(Exception):
     """
@@ -133,14 +134,15 @@
         return qsvc, classification_report(y_test, y_pred), metrics
 
     elif backend == "pennylane":
         # Data splitting
         x_train, x_test, y_train, y_test = dataset.train_test_split(test_size=test_size)
 
         qsvc = QSVC(inputs=cols, verbose=verbose)
+
         # Training
         qsvc.fit(x_train, y_train)
 
         # Testing
         y_pred = qsvc.predict(x_test)
         y_pred_proba = qsvc.predict_proba(x_test)[:, -1]
         metrics = _get_metrics(y_test, y_pred)
```

### Comparing `falcondale-0.2.3/falcondale/clustering.py` & `falcondale-0.2.4/falcondale/clustering.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """
 Aiming for clustering dataset samples using classical, quantum-inspired and quantum techniques.
 """
+
 from .data import Dataset
 
 import numpy as np
 from apqc.pqc import PQC
 from apqc.density_estimation import DensityEstimator
 
 
 def prob_q_clustering(input_ds: Dataset, batch: int = 100, forced_sigma: float = None):
     """
     Accelerated Probabilistic Quantum Clustering
 
     Parameters:
     input_ds (Dataset): Entry dataset
     """
-    pqc = PQC(
-        data_gen=input_ds.get_features(), float_type=32, batch=batch, force_cpu=True
-    )
+    pqc = PQC(data_gen=input_ds.get_features(), float_type=32, batch=batch, force_cpu=True)
 
     if forced_sigma:
         pqc.set_sigmas(sigma_value=forced_sigma)
     else:
         # Fit
         d_e = DensityEstimator(data_gen=pqc.data_gen, batch=batch, scale=pqc.scale)
         init_log_sigmas = np.ones((d_e.data_gen.shape[0], 1)) * np.log(1)
```

### Comparing `falcondale-0.2.3/falcondale/data.py` & `falcondale-0.2.4/falcondale/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module implements the data structure that will be used
 along any steps of a Falcondale project.
 """
+
 import json
 from pandas import DataFrame, concat
 from ydata_profiling import ProfileReport
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.decomposition import PCA
 from sklearn.model_selection import train_test_split
 
@@ -48,28 +49,19 @@
         profile = ProfileReport(self._rawdataset, minimal=True)
         self._df_profile = json.loads(profile.to_json())
 
         # Print
         print(f"Number of samples on the dataset: {self._df_profile['table']['n']}")
         print(f"Number of columns on the dataset: {self._df_profile['table']['n_var']}")
         if self.target:
-            print(
-                f"{self.target} has been selected as target variable for supervised learning tasks."
-            )
-        print(
-            f"Ratio of samples with missing values: {self._df_profile['table']['p_cells_missing']}"
-        )
-
-        if (
-            self._df_profile["table"]["n_var"]
-            == self._df_profile["table"]["types"]["Numeric"]
-        ):
-            print(
-                "All data is numeric therefore little preprocessing might need to be done."
-            )
+            print(f"{self.target} has been selected as target variable for supervised learning tasks.")
+        print(f"Ratio of samples with missing values: {self._df_profile['table']['p_cells_missing']}")
+
+        if self._df_profile["table"]["n_var"] == self._df_profile["table"]["types"]["Numeric"]:
+            print("All data is numeric therefore little preprocessing might need to be done.")
         else:
             print(
                 "Seems like some features are not Numeric, make sure dataset counts with numeric values for categorical values as well."
             )
 
         if len(self._df_profile["alerts"]) > 0:
             print("Some relevant alerts have been found:")
@@ -166,17 +158,15 @@
         Obtain data from the selected columns
 
         Returns:
         DataFrame: subset information from _features dataframe
         """
         if self.target in col_list:
             col_list.remove(self.target)
-            return concat(
-                [self._features[col_list], self._rawdataset[self.target]], axis=1
-            )
+            return concat([self._features[col_list], self._rawdataset[self.target]], axis=1)
 
         return self._features[col_list]
 
     def columns(self) -> list:
         """
         Returns feature column names as a list.
```

### Comparing `falcondale-0.2.3/falcondale/feature_selection.py` & `falcondale-0.2.4/falcondale/feature_selection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module focuses on feature selection methods to diminish the dimensionality of a target dataset.
 
 """
+
 import dimod
 import numpy as np
 import itertools
 
 # SB
 import torch
 import simulated_bifurcation as sb
@@ -42,43 +43,33 @@
     pauli_list = []
     col_list = [feat for feat in input_ds.columns() if feat != input_ds.target]
 
     bqm = dimod.BinaryQuadraticModel.empty(dimod.BINARY)
 
     # Importance
     for i, column in enumerate(col_list):
-        minf = mutual_information(
-            prob(input_ds.select([input_ds.target, column]).values), 1
-        )
+        minf = mutual_information(prob(input_ds.select([input_ds.target, column]).values), 1)
         bqm.add_variable(column, -minf)
         pauli_list.append(("Z", [i], -minf))
 
     # Redundancy
     for field0, field1 in itertools.combinations(col_list, 2):
-        cmi_01 = conditional_mutual_information(
-            prob(input_ds.select([input_ds.target, field0, field1]).values), 1, 2
-        )
-        cmi_10 = conditional_mutual_information(
-            prob(input_ds.select([input_ds.target, field1, field0]).values), 1, 2
-        )
+        cmi_01 = conditional_mutual_information(prob(input_ds.select([input_ds.target, field0, field1]).values), 1, 2)
+        cmi_10 = conditional_mutual_information(prob(input_ds.select([input_ds.target, field1, field0]).values), 1, 2)
         bqm.add_interaction(field0, field1, -cmi_01)
         bqm.add_interaction(field1, field0, -cmi_10)
 
         i = col_list.index(field0)
         j = col_list.index(field1)
         pauli_list.append(("ZZ", [i, j], -cmi_01))
         pauli_list.append(("ZZ", [j, i], -cmi_10))
 
     # Penalty
     if max_cols & max_cols < len(col_list):
-        bqm.update(
-            dimod.generators.combinations(
-                bqm.variables, max_cols, strength=10 * max_cols
-            )
-        )
+        bqm.update(dimod.generators.combinations(bqm.variables, max_cols, strength=10 * max_cols))
 
     bqm.normalize()  # scale the BQM to (-1, 1) biases
 
     op = SparsePauliOp.from_sparse_list(pauli_list, num_qubits=len(col_list))
 
     return bqm, op
```

### Comparing `falcondale-0.2.3/falcondale/helpers/mutual_information.py` & `falcondale-0.2.4/falcondale/helpers/mutual_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Auxiliary functions
 """
+
 import numpy as np
 from pandas import DataFrame
 
 
 def prob(dataset: DataFrame, max_bins=10):
     """Joint probability distribution P(X) for the given data.
 
@@ -45,10 +46,10 @@
 
 
 def conditional_mutual_information(p, j, *conditional_indices):
     """Mutual information between variables X and variable Y conditional on variable Z."""
 
     marginal_conditional_indices = [i - 1 if i > j else i for i in conditional_indices]
 
-    return conditional_shannon_entropy(
-        np.sum(p, axis=j), *marginal_conditional_indices
-    ) - conditional_shannon_entropy(p, j, *conditional_indices)
+    return conditional_shannon_entropy(np.sum(p, axis=j), *marginal_conditional_indices) - conditional_shannon_entropy(
+        p, j, *conditional_indices
+    )
```

### Comparing `falcondale-0.2.3/falcondale/helpers/qnn.py` & `falcondale-0.2.4/falcondale/helpers/qnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module implementing generic QNN setups
 """
+
 import logging
 
 import torch
 import torch.optim as optim
 from torch.autograd import Variable
 
 import pennylane as qml
```

### Comparing `falcondale-0.2.3/falcondale/helpers/qsvc.py` & `falcondale-0.2.4/falcondale/helpers/qsvc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Module implementing generic QNN setups
 """
+
 import logging
 
 from sklearn.svm import SVC
 
 import pennylane as qml
 import pennylane.numpy as np
```

### Comparing `falcondale-0.2.3/falcondale/main.py` & `falcondale-0.2.4/falcondale/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 Classes:
     Model: Base model holding the main structure after training
     Project: The main class that one can instantiate in order to
         start playing around with Falcondale's functionalities
 
         $ myproject = Project(dataset, target="target")
 """
+
 import pickle
 import warnings
 import pandas as pd
 
 from .data import Dataset
 from .classifiers import qsvc, qnn
 from .feature_selection import qfs, qfs_neal, qfs_sb, qfs_sim_qaoa
@@ -344,15 +345,15 @@
                 qnn_model, report, metrics = qnn(dataset=self._data, test_size=test_size, verbose=verbose)
 
             fmodel = Model(self._data, model, qnn_model, report, metrics)
             return fmodel
 
         return NotImplemented
 
-    def cluster(self, ctype: str, **kwargs) -> (list[int], list[float]):
+    def cluster(self, ctype: str, **kwargs) -> tuple[list[int], list[float]]:
         """
         Given a type of clustering it is implemented using the
         information of the inner Dataset. Essentially takes the features
         to produce an estimate on the different segments it could be composed by.
 
         Currently supports:
```

### Comparing `falcondale-0.2.3/falcondale/solvers.py` & `falcondale-0.2.4/falcondale/solvers.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Takes care of the interface with the solvers
 """
+
 import time
 import neal
 from dwave.cloud import Client
 
 
 def dwave_solver(problem, token: str):
     """
```

### Comparing `falcondale-0.2.3/pyproject.toml` & `falcondale-0.2.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [project]
 name = "falcondale"
 description = "Falcondale SDK"
 authors = [
     { name = "Stafford Computing LLC", email = "info@staffordcomputing.com" },
 ]
 dependencies = [
-    "pandas>=2.0.3",
+    "pandas>=2.2.1",
     "ydata-profiling>=4.5.1",
     "scikit-learn>=1.3.0",
     "ipywidgets>=8.1.1",
     "torch>=2.0.1",
-    "pennylane>=0.33.0",
-    "qiskit>=0.45.0",
-    "qiskit-machine-learning>=0.7.0",
-    "qiskit-aer>=0.13.0",
+    "pennylane>=0.35.1",
+    "qiskit>=1.0.2",
+    "qiskit-machine-learning>=0.7.2",
+    "qiskit-aer>=0.14.0.1",
     "dimod>=0.12.12",
     "dwave-neal>=0.6.0",
     "dwave-cloud-client>=0.10.6",
     "requests[socks]>=2.31.0",
-    "qiskit-optimization>=0.6.0",
-    "qiskit-algorithms>=0.2.1",
+    "qiskit-optimization>=0.6.1",
+    "qiskit-algorithms>=0.3.0",
     "apqc>=0.1.3",
     "simulated-bifurcation>=1.2.0",
 ]
 requires-python = ">=3.10,<3.12"
 readme = "README.md"
 dynamic = []
-version = "0.2.3"
+version = "0.2.4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/stafford-computing/falcondale-sdk"
 Documentation = "https://falcondale.readthedocs.io/"
@@ -54,15 +54,15 @@
     "mkdocs-material>=9.3.1",
     "mkdocs-badges>=0.4.1",
     "mkdocstrings[crystal,python]>=0.23.0",
     "mkdocs-jupyter>=0.24.2",
 ]
 dev = [
     "pre-commit>=3.6.0",
-    "ruff>=0.1.8",
+    "ruff>=0.3.5",
     "tox-pdm>=0.7.0",
     "coverage>=7.4.0",
     "nose2>=0.14.0",
 ]
 
 [tool.ruff]
 include = [
```

### Comparing `falcondale-0.2.3/tests/test_main.py` & `falcondale-0.2.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `falcondale-0.2.3/PKG-INFO` & `falcondale-0.2.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: falcondale
-Version: 0.2.3
+Version: 0.2.4
 Summary: Falcondale SDK
 Author-Email: Stafford Computing LLC <info@staffordcomputing.com>
 License: MIT
 Project-URL: Homepage, https://github.com/stafford-computing/falcondale-sdk
 Project-URL: Documentation, https://falcondale.readthedocs.io/
 Requires-Python: <3.12,>=3.10
-Requires-Dist: pandas>=2.0.3
+Requires-Dist: pandas>=2.2.1
 Requires-Dist: ydata-profiling>=4.5.1
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: ipywidgets>=8.1.1
 Requires-Dist: torch>=2.0.1
-Requires-Dist: pennylane>=0.33.0
-Requires-Dist: qiskit>=0.45.0
-Requires-Dist: qiskit-machine-learning>=0.7.0
-Requires-Dist: qiskit-aer>=0.13.0
+Requires-Dist: pennylane>=0.35.1
+Requires-Dist: qiskit>=1.0.2
+Requires-Dist: qiskit-machine-learning>=0.7.2
+Requires-Dist: qiskit-aer>=0.14.0.1
 Requires-Dist: dimod>=0.12.12
 Requires-Dist: dwave-neal>=0.6.0
 Requires-Dist: dwave-cloud-client>=0.10.6
 Requires-Dist: requests[socks]>=2.31.0
-Requires-Dist: qiskit-optimization>=0.6.0
-Requires-Dist: qiskit-algorithms>=0.2.1
+Requires-Dist: qiskit-optimization>=0.6.1
+Requires-Dist: qiskit-algorithms>=0.3.0
 Requires-Dist: apqc>=0.1.3
 Requires-Dist: simulated-bifurcation>=1.2.0
 Description-Content-Type: text/markdown
 
 ![falcondale](https://github.com/stafford-computing/falcondale-sdk/blob/main/assets/falcondale_sdk_black.png?raw=true)
 
 Falcondale Software Development Kit (SDK) is an open source project aiming to ease the barrier for Data Scientists entering the field of Quantum Machine Learning.
```

