# Comparing `tmp/sequential_ft_transformer-0.3.2.tar.gz` & `tmp/sequential_ft_transformer-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequential_ft_transformer-0.3.2.tar", max compression
+gzip compressed data, was "sequential_ft_transformer-0.3.3.tar", max compression
```

## Comparing `sequential_ft_transformer-0.3.2.tar` & `sequential_ft_transformer-0.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1072 2024-04-01 07:23:45.421803 sequential_ft_transformer-0.3.2/LICENSE
--rw-r--r--   0        0        0      721 2024-04-01 07:23:45.421803 sequential_ft_transformer-0.3.2/README.md
--rw-r--r--   0        0        0     1690 2024-04-01 07:24:09.797935 sequential_ft_transformer-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      127 2024-04-01 07:23:45.429803 sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/__init__.py
--rw-r--r--   0        0        0    12049 2024-04-01 07:23:45.429803 sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/embeddings.py
--rw-r--r--   0        0        0    10443 2024-04-01 07:23:45.429803 sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/fttransformer.py
--rw-r--r--   0        0        0     1271 2024-04-01 07:23:45.429803 sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/plotting.py
--rw-r--r--   0        0        0     5015 2024-04-01 07:23:45.429803 sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/preprocessing.py
--rw-r--r--   0        0        0     2651 2024-04-01 07:23:45.429803 sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/transformer.py
--rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 sequential_ft_transformer-0.3.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2024-04-07 19:50:03.307385 sequential_ft_transformer-0.3.3/LICENSE
+-rw-r--r--   0        0        0      721 2024-04-07 19:50:03.307385 sequential_ft_transformer-0.3.3/README.md
+-rw-r--r--   0        0        0     1690 2024-04-07 19:50:23.055377 sequential_ft_transformer-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      127 2024-04-07 19:50:03.315385 sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/__init__.py
+-rw-r--r--   0        0        0    12049 2024-04-07 19:50:03.315385 sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/embeddings.py
+-rw-r--r--   0        0        0    11466 2024-04-07 19:50:03.315385 sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/fttransformer.py
+-rw-r--r--   0        0        0     1271 2024-04-07 19:50:03.315385 sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/plotting.py
+-rw-r--r--   0        0        0     5864 2024-04-07 19:50:03.315385 sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/preprocessing.py
+-rw-r--r--   0        0        0     2651 2024-04-07 19:50:03.315385 sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/transformer.py
+-rw-r--r--   0        0        0     1445 1970-01-01 00:00:00.000000 sequential_ft_transformer-0.3.3/PKG-INFO
```

### Comparing `sequential_ft_transformer-0.3.2/LICENSE` & `sequential_ft_transformer-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sequential_ft_transformer-0.3.2/README.md` & `sequential_ft_transformer-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sequential_ft_transformer-0.3.2/pyproject.toml` & `sequential_ft_transformer-0.3.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sequential_ft_transformer"
-version = "0.3.2"
+version = "0.3.3"
 description = "FT Transformer applied to sequential tabular data"
 authors = ["Christian Orr"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
```

### Comparing `sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/embeddings.py` & `sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/embeddings.py`

 * *Files identical despite different names*

### Comparing `sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/fttransformer.py` & `sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/fttransformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,17 +41,17 @@
     def from_config(cls, config):
         return cls(**config)
 
 
 @keras.saving.register_keras_serializable(package="TransformerLayers")
 class FTTransformerEncoder(keras.layers.Layer):
     def __init__(self,
-                categorical_features: List[str],
-                numerical_features: List[str],
-                feature_unique_counts: Dict[str, int],
+                categorical_features: List[str] = None,
+                numerical_features: List[str] = None,
+                feature_unique_counts: Dict[str, int] = None,
                 seq_length: int = 1,
                 embedding_dim: int = 16,
                 depth: int = 4,
                 heads: int = 8,
                 attn_dropout: float = 0.2,
                 ff_dropout: float = 0.2,
                 numerical_embedding_type: str = "linear",
@@ -100,18 +100,15 @@
                 ff_dropout=self.ff_dropout,
                 explainable=self.explainable,
                 post_norm=self.post_norm,
             )
             for _ in range(self.depth)
         ]
 
-    def call(self, inputs):
-        # numeric and/or cat inputs can be provided
-        numeric_inputs = inputs.get("numeric_inputs")
-        cat_inputs = inputs.get("cat_inputs")
+    def call(self, numeric_inputs=None, cat_inputs=None):
         # Process CLS weights
         cls_weights = self.cls_weights_layer(numeric_inputs if numeric_inputs is not None else cat_inputs)
 
         # Embedding layers
         embeddings = [cls_weights]
         if self.categorical_features:
             cat_embs = self.cat_layer(cat_inputs)
@@ -169,53 +166,52 @@
 
 @keras.saving.register_keras_serializable(package="TransformerLayers")
 class FTTransformer(keras.Model):
     def __init__(
         self,
         out_dim: int,
         out_activation: str,
-        feature_unique_counts: Dict[str, int],
+        feature_unique_counts: Dict[str, int] = None,
         categorical_features: List[str] = None,
         numerical_features: List[str] = None,
         seq_length: int = 1,
         embedding_dim: int = 32,
         depth: int = 4,
         heads: int = 8,
         attn_dropout: float = 0.1,
         ff_dropout: float = 0.1,
         numerical_embedding_type: str = "linear",
         bins_dict: Optional[Dict[str, List[float]]] = None,
         n_bins: Optional[int] = None,
         explainable: bool = False,
+        dtype: str = None, # The saved model wont load without this argument
         **kwargs,
     ):
-        super().__init__(**kwargs)
         self.out_dim = out_dim
-        self.out_activation = keras.activations.get(out_activation)  # Get activation function
+        self.out_activation = keras.activations.get(out_activation)
         self.feature_unique_counts = feature_unique_counts
         self.categorical_features = categorical_features
         self.numerical_features = numerical_features
         self.seq_length = seq_length
         self.embedding_dim = embedding_dim
         self.depth = depth
         self.heads = heads
         self.attn_dropout = attn_dropout
         self.ff_dropout = ff_dropout
         self.numerical_embedding_type = numerical_embedding_type
         self.bins_dict = bins_dict
         self.n_bins = n_bins
         self.explainable = explainable
 
-    def build(self, input_shape):
+        # Initialize all the layers
         self.ln = keras.layers.LayerNormalization(epsilon=1e-6)
         self.flatten = keras.layers.Flatten()
         self.dense1 = keras.layers.Dense(self.embedding_dim * self.seq_length // 2, activation="relu")
         self.dense2 = keras.layers.Dense(self.embedding_dim * self.seq_length // 4, activation="relu")
         self.output_layer = keras.layers.Dense(self.out_dim, activation=self.out_activation, name="output")
-
         self.transformer_encoder = FTTransformerEncoder(
             categorical_features=self.categorical_features,
             numerical_features=self.numerical_features,
             feature_unique_counts=self.feature_unique_counts,
             seq_length=self.seq_length,
             embedding_dim=self.embedding_dim,
             depth=self.depth,
@@ -223,17 +219,37 @@
             attn_dropout=self.attn_dropout,
             ff_dropout=self.ff_dropout,
             numerical_embedding_type=self.numerical_embedding_type,
             bins_dict=self.bins_dict,
             n_bins=self.n_bins,
             explainable=self.explainable,
         )
-
+        # Construct the network to allow for saving and loading the model
+        inputs_layer = dict()
+        empty_cat: bool = categorical_features is None or len(categorical_features) == 0
+        empty_numeric: bool = numerical_features is None or len(numerical_features) == 0
+        if not empty_cat:
+            cat_inputs = keras.layers.Input(shape=(self.seq_length, len(self.categorical_features)))
+            inputs_layer.update({"cat_inputs": cat_inputs})
+        if not empty_numeric:
+            numeric_inputs = keras.layers.Input(shape=(self.seq_length, len(self.numerical_features)))
+            inputs_layer.update({"numeric_inputs": numeric_inputs})
+
+        outputs_layer = self.call(inputs_layer)
+
+        super(FTTransformer, self).__init__(inputs=inputs_layer,
+                                        outputs=outputs_layer,
+                                        **kwargs)
+    
     def call(self, inputs):
-        x = self.transformer_encoder(inputs)
+        # numeric and/or cat inputs can be provided
+        numeric_inputs = inputs.get("numeric_inputs")
+        cat_inputs = inputs.get("cat_inputs")
+        x = self.transformer_encoder(numeric_inputs=numeric_inputs, cat_inputs=cat_inputs)
+
         layer_norm_cls = self.ln(x[:, :, 0, :])
         layer_norm_cls = self.flatten(layer_norm_cls)
         layer_norm_cls = self.dense1(layer_norm_cls)
         layer_norm_cls = self.dense2(layer_norm_cls)
         output = self.output_layer(layer_norm_cls)
 
         if self.transformer_encoder.explainable:
```

### Comparing `sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/plotting.py` & `sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/plotting.py`

 * *Files identical despite different names*

### Comparing `sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/preprocessing.py` & `sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/preprocessing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import urllib.request
 import numpy as np
 import pandas as pd
 import tensorflow as tf
-
+from ucimlrepo import fetch_ucirepo 
 
 def pad_df(
     df: pd.DataFrame, 
     seq_length: int, 
     seq_col_name: str
 ):
     """
@@ -138,8 +138,30 @@
     # Create the data folder if it doesn't exist
     os.makedirs(data_folder, exist_ok=True)
 
     if not os.path.exists(filepath):
         urllib.request.urlretrieve(url, filepath)
         print(f"Downloaded {filename} to {data_folder}")
     else:
+        print(f"{filename} already exists in {data_folder}")
+
+
+def download_wine_dataset(
+    data_folder: str = "../data", 
+    filename: str = "wine_quality"
+):  
+
+    inputs_filepath = f"{os.path.join(data_folder, filename)}_inputs.csv"
+    labels_filepath = f"{os.path.join(data_folder, filename)}_labels.csv"
+
+    # Create the data folder if it doesn't exist
+    os.makedirs(data_folder, exist_ok=True)
+
+    if not os.path.exists(inputs_filepath) or not os.path.exists(labels_filepath):
+        wine_quality = fetch_ucirepo(id=186)
+        x = wine_quality["data"]["features"]
+        y = wine_quality["data"]["targets"]
+        x.to_csv(inputs_filepath, index=False, header=True)
+        y.to_csv(labels_filepath, index=False, header=True)
+        print(f"Downloaded {filename} to {data_folder}")
+    else:
         print(f"{filename} already exists in {data_folder}")
```

### Comparing `sequential_ft_transformer-0.3.2/src/sequential_ft_transformer/transformer.py` & `sequential_ft_transformer-0.3.3/src/sequential_ft_transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `sequential_ft_transformer-0.3.2/PKG-INFO` & `sequential_ft_transformer-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequential_ft_transformer
-Version: 0.3.2
+Version: 0.3.3
 Summary: FT Transformer applied to sequential tabular data
 License: MIT
 Author: Christian Orr
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

