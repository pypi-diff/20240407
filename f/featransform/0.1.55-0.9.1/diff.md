# Comparing `tmp/featransform-0.1.55-py3-none-any.whl.zip` & `tmp/featransform-0.9.1-py3-none-any.whl.zip`

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
+Zip file size: 18542 bytes, number of entries: 18
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/__init__.py
+-rw-rw-rw-  2.0 fat    11267 b- defN 24-Apr-07 17:16 featransform/pipeline.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/configs/__init__.py
+-rw-rw-rw-  2.0 fat     2140 b- defN 24-Apr-01 18:31 featransform/configs/parameters.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/feature_engineering/__init__.py
+-rw-rw-rw-  2.0 fat     3562 b- defN 24-Apr-07 17:16 featransform/feature_engineering/anomalies.py
+-rw-rw-rw-  2.0 fat     3376 b- defN 24-Apr-07 17:16 featransform/feature_engineering/clustering.py
+-rw-rw-rw-  2.0 fat     4030 b- defN 24-Apr-07 17:16 featransform/feature_engineering/dimensionality.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/optimizer/__init__.py
+-rw-rw-rw-  2.0 fat    11401 b- defN 24-Apr-07 17:17 featransform/optimizer/evaluator.py
+-rw-rw-rw-  2.0 fat     5265 b- defN 24-Apr-07 17:17 featransform/optimizer/selector.py
+-rw-rw-rw-  2.0 fat        2 b- defN 24-Apr-01 18:31 featransform/processing/__init__.py
+-rw-rw-rw-  2.0 fat     3512 b- defN 24-Apr-01 20:48 featransform/processing/processor.py
+-rw-rw-rw-  2.0 fat     1090 b- defN 24-Apr-07 17:36 featransform-0.9.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     7196 b- defN 24-Apr-07 17:36 featransform-0.9.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-07 17:36 featransform-0.9.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 24-Apr-07 17:36 featransform-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1612 b- defN 24-Apr-07 17:36 featransform-0.9.1.dist-info/RECORD
+18 files, 54566 bytes uncompressed, 15838 bytes compressed:  71.0%
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
+Filename: featransform-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/METADATA
+Filename: featransform-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/WHEEL
+Filename: featransform-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/top_level.txt
+Filename: featransform-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: featransform-0.1.55.dist-info/RECORD
+Filename: featransform-0.9.1.dist-info/RECORD
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
+from .processing.processor import AutoLabelEncoder, AutoIterativeImputer
+from .feature_engineering.anomalies import Anomaly_Engineering
+from .feature_engineering.clustering import Clustering_Engineering
+from .feature_engineering.dimensionality import PCAensemble
+from .optimizer.evaluator import Evaluation
+from .optimizer.selector import Selector
+from .configs.parameters import configurations
 
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
+from .configs.parameters import configurations
 
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
+from .configs.parameters import configurations
 
 sec_conf = configurations()
 
 class Clustering_Engineering:
     def __init__(self, 
                  cluster_models: list = ['KMeans'],
                  configs : dict = sec_conf):
```

## Comparing `featransform/dimensionality.py` & `featransform/feature_engineering/dimensionality.py`

 * *Files 1% similar despite different names*

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
+from .configs.parameters import configurations
 
 # Load default configurations
 sec_conf = configurations()
 
 class PCAensemble:
     def __init__(self,
                  pca_models : list = ['PCA'],
```

## Comparing `featransform/evaluator.py` & `featransform/optimizer/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 from atlantic.analysis import Analysis 
-from featransform.selector import Selector
-from featransform.parameters import configurations
+from .optimizer.selector import Selector
+from .configs.parameters import configurations
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

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pandas as pd
 from atlantic.analysis import Analysis
-from featransform.parameters import configurations
+from .configs.parameters import configurations
 from sklearn.preprocessing import LabelEncoder
 from catboost import CatBoostClassifier, CatBoostRegressor
 import xgboost as xgb
 
 sec_conf = configurations()
 
 class Selector:
```

## Comparing `featransform-0.1.55.dist-info/LICENSE` & `featransform-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `featransform-0.1.55.dist-info/METADATA` & `featransform-0.9.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featransform
-Version: 0.1.55
+Version: 0.9.1
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

## Comparing `featransform-0.1.55.dist-info/RECORD` & `featransform-0.9.1.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 featransform/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
-featransform/anomalies.py,sha256=jPJz1Uo-TEoocunhjhnkfVX9dsjFhtFEA6KxQFDrb9w,3566
-featransform/clustering.py,sha256=A3e54sPaKTaYgUENtVgxOZTtnfqQufLysHn8LttzOZo,3380
-featransform/dimensionality.py,sha256=iQ5HTv1qaAUJaDP6hWYFOu3MMnQk31C9iIH1u8Yfcc4,4034
-featransform/evaluator.py,sha256=-4CvmJhhxlGwPvzQAaCsel_piwtfZEi6nLB6xSXuE9M,11407
-featransform/parameters.py,sha256=QFj-tFzBo4EpVrMK-Id0WKWkNeT7GsNWrkxftNuzxhc,2140
-featransform/pipeline.py,sha256=AWQcXwt5Ci2khk4W12xeS1Mft4RnybAP5YMhKqpG27Q,11003
-featransform/processor.py,sha256=_eVGVNOF3RiJEabRwrq3G1AxY0c21MAleYdtaw3xGT4,3512
-featransform/selector.py,sha256=abY1QlAaBi1kvdLLSnmsUD-juSnGRlqw3IYJKflYIw4,5269
-featransform-0.1.55.dist-info/LICENSE,sha256=VMXkEvDFBFiT1owkPDp8dUVbidhkemgBSzG9qsUhs54,1090
-featransform-0.1.55.dist-info/METADATA,sha256=cFgKymMJtBtuSFBXanZXBM-eioVTwO7n44G3OI8wBgc,7195
-featransform-0.1.55.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-featransform-0.1.55.dist-info/top_level.txt,sha256=nGf-wp6SDVDIawemhMuwByTbpGahhv92kQ1dQbRdYwo,13
-featransform-0.1.55.dist-info/RECORD,,
+featransform/pipeline.py,sha256=LRLOCFx0ZNPQpYlRKCjRkrr7e8nhlKNNqPGepfRebIE,11267
+featransform/configs/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+featransform/configs/parameters.py,sha256=QFj-tFzBo4EpVrMK-Id0WKWkNeT7GsNWrkxftNuzxhc,2140
+featransform/feature_engineering/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+featransform/feature_engineering/anomalies.py,sha256=63-d8lwGJ1tftOgXBirTY9kSUbnHlty6G9KA97EXLJY,3562
+featransform/feature_engineering/clustering.py,sha256=3ZUuBovcrvvQHH2OIcy6EvlORqfHEwjMH26281JJWRM,3376
+featransform/feature_engineering/dimensionality.py,sha256=lEkO2VLDM7kchtdGRRbT6C9irdWfvQa63gLqcRdJQ4Q,4030
+featransform/optimizer/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+featransform/optimizer/evaluator.py,sha256=GTqwajkKIph71nERTu28tFcCOYTIdC67nGq00KSQ45w,11401
+featransform/optimizer/selector.py,sha256=7kGbrt9xc6xUC0Rs2nnce0owcckKh-Z5t5TgPRqsjf8,5265
+featransform/processing/__init__.py,sha256=frcCV1k9oG9oKj3dpUqdJg1PxRT2RSN_XKdLCPjaYaY,2
+featransform/processing/processor.py,sha256=_eVGVNOF3RiJEabRwrq3G1AxY0c21MAleYdtaw3xGT4,3512
+featransform-0.9.1.dist-info/LICENSE,sha256=VMXkEvDFBFiT1owkPDp8dUVbidhkemgBSzG9qsUhs54,1090
+featransform-0.9.1.dist-info/METADATA,sha256=Mim-RRZ6eRP3Q4fAOhQnw01g8V6i8Ckzx0XHZevjFAw,7196
+featransform-0.9.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+featransform-0.9.1.dist-info/top_level.txt,sha256=nGf-wp6SDVDIawemhMuwByTbpGahhv92kQ1dQbRdYwo,13
+featransform-0.9.1.dist-info/RECORD,,
```

