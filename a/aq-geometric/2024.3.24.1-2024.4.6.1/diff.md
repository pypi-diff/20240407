# Comparing `tmp/aq_geometric-2024.3.24.1.tar.gz` & `tmp/aq_geometric-2024.4.6.1.tar.gz`

## Comparing `aq_geometric-2024.3.24.1.tar` & `aq_geometric-2024.4.6.1.tar`

### file list

```diff
@@ -1,47 +1,54 @@
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/requirements.txt
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/__init__.py
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/file/__init__.py
--rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/file/local.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/filter/__init__.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/filter/node_features.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/__init__.py
--rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/compute_graph.py
--rw-r--r--   0        0        0    17069 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/graphs_builder.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/edges/__init__.py
--rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/edges/compute_edges.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/nodes/__init__.py
--rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/nodes/compute_node_features.py
--rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/graph/nodes/compute_nodes.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/reindex/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/reindex/features.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/remote/__init__.py
--rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/data/remote/psql.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/datasets/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/datasets/in_memory/__init__.py
--rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
--rw-r--r--   0        0        0    26545 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/__init__.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/base_model.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/edge_conv/__init__.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/edge_conv/edge_conv.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/gcn/__init__.py
--rw-r--r--   0        0        0     2236 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/gcn/gcn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/hierarchical_edge_conv/__init__.py
--rw-r--r--   0        0        0    16310 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/transforms/__init__.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/utils/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/utils/evaluation.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/utils/forecasts.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/aq_geometric/utils/station_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/tests/config/__init__.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/tests/config/test_remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/tests/data/__init__.py
--rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/tests/data/test_aq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/tests/datasets/__init__.py
--rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/tests/datasets/test_aq.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/LICENSE.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/README.md
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/pyproject.toml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 aq_geometric-2024.3.24.1/PKG-INFO
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/requirements.txt
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/__init__.py
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/file/__init__.py
+-rw-r--r--   0        0        0     3526 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/file/local.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/filter/__init__.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/filter/node_features.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/__init__.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/compute_graph.py
+-rw-r--r--   0        0        0    17069 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/graphs_builder.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/edges/__init__.py
+-rw-r--r--   0        0        0     7337 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/edges/compute_edges.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/__init__.py
+-rw-r--r--   0        0        0    14500 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_node_features.py
+-rw-r--r--   0        0        0    10409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_nodes.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/reindex/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/reindex/features.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/remote/__init__.py
+-rw-r--r--   0        0        0     6877 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/data/remote/psql.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/in_memory/__init__.py
+-rw-r--r--   0        0        0    11724 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py
+-rw-r--r--   0        0        0    26545 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/__init__.py
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/base_model.py
+-rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/test_base_model.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/__init__.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/edge_conv.py
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/edge_conv/test_edge_conv.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/gcn/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/gcn/gcn.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/gcn/test_gcn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/__init__.py
+-rw-r--r--   0        0        0    16043 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py
+-rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/test_heirarchical_edge_conv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/transforms/__init__.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/__init__.py
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/evaluation.py
+-rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/forecasts.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/station_filters.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/test_evaluation.py
+-rw-r--r--   0        0        0     5440 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/test_forecasts.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/aq_geometric/utils/test_station_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/config/__init__.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/config/test_remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/data/__init__.py
+-rw-r--r--   0        0        0     3909 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/data/test_aq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/datasets/__init__.py
+-rw-r--r--   0        0        0    10356 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/tests/datasets/test_aq.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/LICENSE.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/README.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 aq_geometric-2024.4.6.1/PKG-INFO
```

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/file/local.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/file/local.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/filter/node_features.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/filter/node_features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/graph/compute_graph.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/graph/compute_graph.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/graph/graphs_builder.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/graph/graphs_builder.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/graph/edges/compute_edges.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/graph/edges/compute_edges.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/graph/nodes/compute_node_features.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_node_features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/graph/nodes/compute_nodes.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/graph/nodes/compute_nodes.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/reindex/features.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/reindex/features.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/data/remote/psql.py` & `aq_geometric-2024.4.6.1/aq_geometric/data/remote/psql.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py` & `aq_geometric-2024.4.6.1/aq_geometric/datasets/in_memory/aq_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py` & `aq_geometric-2024.4.6.1/aq_geometric/datasets/on_disk/aq_geometric_dataset.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/models/base_model.py` & `aq_geometric-2024.4.6.1/aq_geometric/models/base_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,16 @@
     def __init__(self, name: str = "BaseModel",
                  guid: str = "00000000-0000-0000-0000-000000000000",
                  stations: Union[List, None] = None, **kwargs):
         super().__init__(**kwargs)
         self.name = name
         self.guid = guid
         self.stations = stations
+        self.features = kwargs.get("features", [])
+        self.targets = kwargs.get("targets", [])
         self.kwargs = kwargs
 
     def save(self, path: str):
         """Save the model to a file."""
         # ensure the model is on the CPU
         self.cpu()
 
@@ -56,8 +58,10 @@
     def __repr__(self):
         """Use the torch default representation, add new attrs."""
         representation = super().__repr__()
         # add new lines with the name, guid, and stations
         representation += f"\nName: {self.name}"
         representation += f"\nGUID: {self.guid}"
         representation += f"\nStations: {self.stations}"
+        representation += f"\nFeatures: {self.features}"
+        representation += f"\nTargets: {self.targets}"
         return representation
```

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/models/gcn/gcn.py` & `aq_geometric-2024.4.6.1/aq_geometric/models/gcn/gcn.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         **kawrgs: Additional keyword arguments for `torch_geometric.nn.conv.GCNConv`.
     """
     def __init__(
         self,
         name: str = "GCNModel",
         guid: str = str(uuid.uuid4()),
         stations: Union[List, None] = None,
+        features: List[str] = ["OZONE", "PM2.5", "NO2"],
+        targets: List[str] = ["OZONE", "PM2.5", "NO2"],
         in_channels: int = 48,
         hidden_channels: int = 256,
         num_layers: int = 3,
         out_channels: int = 256,
         dropout: float = 0.5,
         act=None,
         act_first: bool = True,
@@ -46,14 +48,16 @@
         norm_kwargs=None,
         jk: str = "last",
     ):
         super().__init__(
             name=name,
             guid=guid,
             stations=stations,
+            features=features,
+            targets=targets,
             in_channels=in_channels,
             hidden_channels=hidden_channels,
             num_layers=num_layers,
             out_channels=out_channels,
             dropout=dropout,
             act=act,
             act_first=act_first,
```

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py` & `aq_geometric-2024.4.6.1/aq_geometric/models/hierarchical_edge_conv/heirarchical_edge_conv.py`

 * *Files 3% similar despite different names*

```diff
@@ -219,19 +219,14 @@
             if key not in ["name", "guid", "stations", "state_dict"]:
                 setattr(self, key, value)
 
     def __repr__(self):
         """Use the torch default representation, add new attrs."""
         representation = super().__repr__()
         # add new lines with the name, guid, and stations
-        representation += f"\nName: {self.name}"
-        representation += f"\nGUID: {self.guid}"
-        representation += f"\nStations: {self.stations}"
-        representation += f"\nFeatures: {self.features}"
-        representation += f"\nTargets: {self.targets}"
         representation += f"\nSamples in Node Features: {self.num_samples_in_node_feature}"
         representation += f"\nSamples in Node Targets: {self.num_samples_in_node_target}"
 
         return representation
 
 
 def process_aq_geometric_dataset_edges_by_h3_resolution(
```

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/utils/evaluation.py` & `aq_geometric-2024.4.6.1/aq_geometric/utils/evaluation.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/utils/forecasts.py` & `aq_geometric-2024.4.6.1/aq_geometric/utils/forecasts.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from datetime import datetime
-from typing import Dict, Union
+from typing import Dict, Union, List
 
 import torch
 import numpy as np
 import pandas as pd
 from aq_utilities.data import hourly_predictions_to_postgres
 
 
-def generate_forecasts(
+def generate_forecasts_graph(
     model: "aq_geometric.models.base_model.BaseModel",
     dataset: "AqGeometricInMemoryDataset",
+    targets: List[str],
     include_history: bool = False,
     verbose: bool = False,
 ) -> Dict[str, pd.DataFrame]:
     """
     Generate forecasts using the model provided
     """
     forecasts = []
@@ -21,18 +22,18 @@
     # obtain data attributes
     if verbose:
         print(f"[{datetime.now()}] reading from dataset")
     g = dataset.get(0)
     inputs = g.x
     input_edge_index = g.edge_index
     h3_indices = g.h3_index
+    aqsids = g.aqsid
+    timestamps = g.timestamps
     feature_timestamps = g.feature_timestamps
     target_timestamps = g.target_timestamps
-    targets = g.target_names
-
 
     with torch.no_grad():
         if verbose:
             print(f"[{datetime.now()}] generating forecasts for {len(h3_indices)} h3 indices")
         pred = model(inputs, input_edge_index)
         # reshape the prediction to the shape of the target
         pred = pred.numpy().reshape(g.y_mask.shape)
@@ -57,31 +58,30 @@
         if verbose:
             print(f"[{datetime.now()}] forecast df shape for {target}: {forecast_df.shape}")
         df = pd.concat([history_df, forecast_df], axis=1)
         target_dfs[target] = df
         if verbose:
             print(f"[{datetime.now()}] added DataFrame {df.shape}")
 
-    return target_dfs
+    return target_dfs, g
 
 
-def forecasts_to_db(
+def forecasts_df_to_db(
     engine: str,
     model: "aq_geometric.models.base_model.BaseModel",
     graph: "Data",
     target_dfs: Dict[str, pd.DataFrame],
     run_id: Union[str, None] = None,
     chunksize: int = 1000,
     continue_on_error: bool = False,
     verbose: bool = False,
 ) -> int:
     """
     Write the forecasts to the database
     """
-    from aq_utilities.engine.psql import hourly_predictions_to_postgres
     # generate a random run id if none is provided
     if run_id is None:
         import uuid
         run_id = str(uuid.uuid4())
 
     # obtain model attributes
     model_id = model.guid
@@ -93,15 +93,15 @@
         # read from the graph used to generate forecasts
         assert len(graph.h3_index) == len(graph.aqsid)
         df = pd.DataFrame(np.stack((graph.h3_index.T, graph.aqsid.T), axis=1), columns=["h3_index", "aqsid"])
 
         # obtain the timestamps
         timestamps = forecast_df.columns.to_list()
         data = forecast_df.values
-        max_timestamp_in_samples = graph.feature_end_time
+        max_timestamp_in_samples = g.feature_end_time
         predicted_at_timestamp = pd.Timestamp.now()
 
         # prepare the data
         for i, timestamp in enumerate(timestamps):
             df["value"] = data[:, i]
             df["timestamp"] = timestamp
             df["predicted_at_timestamp"] = predicted_at_timestamp
@@ -121,52 +121,57 @@
                 print(f"failed to write predictions to postgres: {err}")
                 if continue_on_error: continue
                 else: return 1
 
     return 0
 
 
-def forecasts_to_json(
+def forecasts_graph_to_json(
     model: "aq_geometric.models.base_model.BaseModel",
     graph: "Data",
+    targets: List[str],
     target_dfs: Dict[str, pd.DataFrame],
     verbose: bool = False,
 ) -> dict:
     """Prepare the forecast in json format"""
     # generate the frontend data
     fe_data = {}
     fe_data["num_history_samples"] = model.num_samples_in_node_feature
     fe_data["num_forecast_samples"] = model.num_samples_in_node_target
     model_name = model.name
-    targets = graph.target_names
     
     # we also want to include the history and the forecasts
     fe_data[model_name] = {
         **{target_name: {} for target_name in targets},
     }
     timestamps = None
     history_and_forecasts_len = -1
     for target_name, forecast_df in target_dfs.items():
         if verbose:
             print(f"[{datetime.now()}] preparing forecast for {target_name}")
         if timestamps is None:
             timestamps = forecast_df.columns.to_list()
         for row_ in forecast_df.iterrows():
             h3_index = row_[0]
-            fe_data[model_name][target_name][h3_index] = row_[1].fillna(0).tolist()
+            fe_data[model_name][target_name][h3_index] = [int(v) for v in row_[1].fillna(0).tolist()]
             if history_and_forecasts_len == -1:
                 history_and_forecasts_len = len(row_[1])
             else:
                 if history_and_forecasts_len != len(row_[1]):
                     raise ValueError("forecast lengths do not match")
     
+    # if we did not include history, we still want to include the timestamps'
+    if history_and_forecasts_len == model.num_samples_in_node_target:
+        fe_data["num_history_samples"] = 0
+        if verbose:
+            print(f"[{datetime.now()}] no history included in forecast")
+
     # we want access to the timestamps when displaying the data
     fe_data["timestamps"] = [
         str(t) for t in timestamps
     ]
 
-    print(f"[{datetime.now()}] frontend datetimes: [{fe_data['timestamps'][0]}, {fe_data['timestamps'][-1]}]")
-
     if verbose:
+        print(f"[{datetime.now()}] frontend datetimes: [{fe_data['timestamps'][0]}, {fe_data['timestamps'][-1]}]")
         print(f"[{datetime.now()}] prepared forecast for frontend")
 
     return fe_data
```

### Comparing `aq_geometric-2024.3.24.1/aq_geometric/utils/station_filters.py` & `aq_geometric-2024.4.6.1/aq_geometric/utils/station_filters.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/tests/config/test_remote.py` & `aq_geometric-2024.4.6.1/tests/config/test_remote.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/tests/data/test_aq.py` & `aq_geometric-2024.4.6.1/tests/data/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/tests/datasets/test_aq.py` & `aq_geometric-2024.4.6.1/tests/datasets/test_aq.py`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/.gitignore` & `aq_geometric-2024.4.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/LICENSE.md` & `aq_geometric-2024.4.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aq_geometric-2024.3.24.1/pyproject.toml` & `aq_geometric-2024.4.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name="aq-geometric"
-version="2024.3.24.1"
+version="2024.04.06.1"
 authors=[
     {name="Chris Jellen", email="cdjellen@gmail.com"},
 ]
 description="Geometric deep learning on air quality data."
 readme="README.md"
 requires-python=">=3.9"
 keywords=[
```

### Comparing `aq_geometric-2024.3.24.1/PKG-INFO` & `aq_geometric-2024.4.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: aq-geometric
-Version: 2024.3.24.1
+Version: 2024.4.6.1
 Summary: Geometric deep learning on air quality data.
 Project-URL: homepage, https://github.com/cdjellen/aq
 Project-URL: documentation, https://github.com/cdjellen/aq
 Author-email: Chris Jellen <cdjellen@gmail.com>
 License-File: LICENSE.md
 Keywords: deep-learning,earth-systems,geometric-deep-learning,pytorch
 Classifier: License :: OSI Approved :: MIT License
```

