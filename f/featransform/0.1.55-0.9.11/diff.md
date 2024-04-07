# Comparing `tmp/featransform-0.1.55-py3-none-any.whl.zip` & `tmp/featransform-0.9.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,20 @@
-Zip file size: 17638 bytes, number of entries: 14
--rw-rw-rw-  2.0 fat        2 b- defN 23-Oct-28 14:14 featransform/__init__.py
--rw-rw-rw-  2.0 fat     3566 b- defN 24-Feb-06 22:23 featransform/anomalies.py
--rw-rw-rw-  2.0 fat     3380 b- defN 24-Feb-06 22:24 featransform/clustering.py
--rw-rw-rw-  2.0 fat     4034 b- defN 24-Feb-06 22:24 featransform/dimensionality.py
--rw-rw-rw-  2.0 fat    11407 b- defN 24-Feb-06 22:24 featransform/evaluator.py
--rw-rw-rw-  2.0 fat     2140 b- defN 24-Jan-27 22:32 featransform/parameters.py
--rw-rw-rw-  2.0 fat    11003 b- defN 24-Feb-06 22:24 featransform/pipeline.py
--rw-rw-rw-  2.0 fat     3512 b- defN 24-Jan-27 22:32 featransform/processor.py
--rw-rw-rw-  2.0 fat     5269 b- defN 24-Feb-06 22:25 featransform/selector.py
--rw-rw-rw-  2.0 fat     1090 b- defN 24-Feb-26 00:10 featransform-0.1.55.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     7195 b- defN 24-Feb-26 00:10 featransform-0.1.55.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Feb-26 00:10 featransform-0.1.55.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 24-Feb-26 00:10 featransform-0.1.55.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1157 b- defN 24-Feb-26 00:10 featransform-0.1.55.dist-info/RECORD
-14 files, 53860 bytes uncompressed, 15716 bytes compressed:  70.8%
+Zip file size: 18585 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/__init__.py
+-rw-rw-rw-  2.0 fat    11351 b- defN 24-Apr-07 17:41 featransform/pipeline.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/configs/__init__.py
+-rw-rw-rw-  2.0 fat     2140 b- defN 24-Apr-01 18:31 featransform/configs/parameters.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/feature_engineering/__init__.py
+-rw-rw-rw-  2.0 fat     3574 b- defN 24-Apr-07 17:39 featransform/feature_engineering/anomalies.py
+-rw-rw-rw-  2.0 fat     3388 b- defN 24-Apr-07 17:39 featransform/feature_engineering/clustering.py
+-rw-rw-rw-  2.0 fat     4042 b- defN 24-Apr-07 17:39 featransform/feature_engineering/dimensionality.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/optimizer/__init__.py
+-rw-rw-rw-  2.0 fat    11425 b- defN 24-Apr-07 17:40 featransform/optimizer/evaluator.py
+-rw-rw-rw-  2.0 fat     5277 b- defN 24-Apr-07 17:40 featransform/optimizer/selector.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/processing/__init__.py
+-rw-rw-rw-  2.0 fat     3512 b- defN 24-Apr-01 20:48 featransform/processing/processor.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-07 17:44 featransform-0.9.11.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7197 b- defN 24-Apr-07 17:44 featransform-0.9.11.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-07 17:44 featransform-0.9.11.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-07 17:44 featransform-0.9.11.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1617 b- defN 24-Apr-07 17:44 featransform-0.9.11.dist-info/RECORD
+18 files, 54728 bytes uncompressed, 15871 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,43 +1,55 @@
 Filename: featransform/__init__.py
 Comment: 
 
-Filename: featransform/anomalies.py
+Filename: featransform/pipeline.py
 Comment: 
 
-Filename: featransform/clustering.py
+Filename: featransform/configs/__init__.py
 Comment: 
 
-Filename: featransform/dimensionality.py
+Filename: featransform/configs/parameters.py
 Comment: 
 
-Filename: featransform/evaluator.py
+Filename: featransform/feature_engineering/__init__.py
 Comment: 
 
-Filename: featransform/parameters.py
+Filename: featransform/feature_engineering/anomalies.py
 Comment: 
 
-Filename: featransform/pipeline.py
+Filename: featransform/feature_engineering/clustering.py
+Comment: 
+
+Filename: featransform/feature_engineering/dimensionality.py
+Comment: 
+
+Filename: featransform/optimizer/__init__.py
+Comment: 
+
+Filename: featransform/optimizer/evaluator.py
+Comment: 
+
+Filename: featransform/optimizer/selector.py
 Comment: 
 
-Filename: featransform/processor.py
+Filename: featransform/processing/__init__.py
 Comment: 
 
-Filename: featransform/selector.py
+Filename: featransform/processing/processor.py
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/LICENSE
+Filename: featransform-0.9.11.dist-info/LICENSE
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/METADATA
+Filename: featransform-0.9.11.dist-info/METADATA
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/WHEEL
+Filename: featransform-0.9.11.dist-info/WHEEL
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/top_level.txt
+Filename: featransform-0.9.11.dist-info/top_level.txt
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/RECORD
+Filename: featransform-0.9.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## featransform/pipeline.py

```diff
@@ -1,16 +1,17 @@
 import numpy as np
 import pandas as pd
 from atlantic.analysis import Analysis
-from featransform.processor import AutoLabelEncoder, AutoIterativeImputer
-from featransform.anomalies import Anomaly_Engineering
-from featransform.clustering import Clustering_Engineering
-from featransform.dimensionality import PCAensemble
-from featransform.evaluator import Evaluation
-from featransform.parameters import configurations
+from featransform.processing.processor import AutoLabelEncoder, AutoIterativeImputer
+from featransform.feature_engineering.anomalies import Anomaly_Engineering
+from featransform.feature_engineering.clustering import Clustering_Engineering
+from featransform.feature_engineering.dimensionality import PCAensemble
+from featransform.optimizer.evaluator import Evaluation
+from featransform.optimizer.selector import Selector
+from featransform.configs.parameters import configurations
 
 sec_conf = configurations()
 
 class Featransform:
     def __init__(self,
                  configs : dict = sec_conf,
                  optimize_iters : int = 6, 
@@ -215,12 +216,21 @@
         X_ = X_[list(set(self.orig_cols).intersection(self.selected_features)) + 
                         [col for col in X_.columns 
                                  if col not in list(set(self.orig_cols).intersection(self.selected_features))]]
         
         return X_
     
 
-
+__all__ = [
+    'AutoLabelEncoder',
+    'AutoIterativeImputer',
+    'Anomaly_Engineering',
+    'Clustering_Engineering',
+    'PCAensemble',
+    'Evaluation',
+    'Selector',
+    'configurations'
+]
```

## Comparing `featransform/anomalies.py` & `featransform/feature_engineering/anomalies.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pandas as pd
 from sklearn.ensemble import IsolationForest
 from sklearn.neighbors import LocalOutlierFactor
 from sklearn.svm import OneClassSVM
 from sklearn.covariance import EllipticEnvelope
-from featransform.parameters import configurations
+from featransform.configs.parameters import configurations
 
 sec_conf = configurations()
 
 class Anomaly_Engineering:
     def __init__(self,
                  det_models : list = ['Isolation_Forest'], # List of anomaly detection models
                  configs : dict = sec_conf, # Configuration dictionary for models
```

## Comparing `featransform/clustering.py` & `featransform/feature_engineering/clustering.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas as pd
 from sklearn.cluster import (DBSCAN,
                              KMeans,
                              Birch,
                              MiniBatchKMeans)
 from sklearn.mixture import GaussianMixture
-from featransform.parameters import configurations
+from featransform.configs.parameters import configurations
 
 sec_conf = configurations()
 
 class Clustering_Engineering:
     def __init__(self, 
                  cluster_models: list = ['KMeans'],
                  configs : dict = sec_conf):
```

## Comparing `featransform/dimensionality.py` & `featransform/feature_engineering/dimensionality.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 warnings.filterwarnings('ignore', category = FutureWarning)
 warnings.filterwarnings('ignore', category = DeprecationWarning, module = "tensorflow")
 from sklearn.decomposition import PCA, TruncatedSVD, FastICA
 from sklearn.manifold import LocallyLinearEmbedding
 import os
 os.environ['TF_ENABLE_ONEDNN_OPTS'] = '0' # Disable TensorFlow optimizations using OneDNN
 from umap import UMAP
-from featransform.parameters import configurations
+from featransform.configs.parameters import configurations
 
 # Load default configurations
 sec_conf = configurations()
 
 class PCAensemble:
     def __init__(self,
                  pca_models : list = ['PCA'],
```

## Comparing `featransform/evaluator.py` & `featransform/optimizer/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from atlantic.analysis import Analysis 
-from featransform.selector import Selector
-from featransform.parameters import configurations
+from featransform.optimizer.selector import Selector
+from featransform.configs.parameters import configurations
 from sklearn.metrics import (mean_absolute_error,
                              mean_absolute_percentage_error,
                              mean_squared_error,
                              explained_variance_score,
                              max_error,
                              r2_score,
                              accuracy_score,
```

## Comparing `featransform/parameters.py` & `featransform/configs/parameters.py`

 * *Files identical despite different names*

## Comparing `featransform/processor.py` & `featransform/processing/processor.py`

 * *Files identical despite different names*

## Comparing `featransform/selector.py` & `featransform/optimizer/selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 from atlantic.analysis import Analysis
-from featransform.parameters import configurations
+from featransform.configs.parameters import configurations
 from sklearn.preprocessing import LabelEncoder
 from catboost import CatBoostClassifier, CatBoostRegressor
 import xgboost as xgb
 
 sec_conf = configurations()
 
 class Selector:
```

## Comparing `featransform-0.1.55.dist-info/LICENSE` & `featransform-0.9.11.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `featransform-0.1.55.dist-info/METADATA` & `featransform-0.9.11.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featransform
-Version: 0.1.55
+Version: 0.9.11
 Summary: Featransform is an automated feature engineering framework for supervised machine learning
 Home-page: https://github.com/TsLu1s/Featransform
 Author: Luís Santos
 Author-email: luisf_ssantos@hotmail.com
 License: MIT
 Keywords: data science,machine learning,data processing,feature engineering,feature selection,feature construction,feature optimization,automated feature engineering,automated machine learning,predictive modeling
 Classifier: Intended Audience :: Education
@@ -92,16 +92,16 @@
 Relevant Note:
 * Although functional, `Featransform` pipeline is not optimized for big data purposes yet.
 
 ```py
     
 import pandas as pd
 from sklearn.model_selection import train_test_split
-from featransform.pipeline import Featransform
-from featransform.parameters import configurations
+from featransform.pipeline import (Featransform,
+                                   configurations)
 import warnings
 warnings.filterwarnings("ignore", category=Warning) # -> For a clean console
     
 data = pd.read_csv('csv_directory_path', encoding='latin', delimiter=',') # Dataframe Loading Example
 
 train,test = train_test_split(data, train_size=0.8)
 train,test = train.reset_index(drop=True), test.reset_index(drop=True) # -> Required
```

