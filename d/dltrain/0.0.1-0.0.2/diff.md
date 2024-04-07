# Comparing `tmp/dltrain-0.0.1.tar.gz` & `tmp/dltrain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dltrain-0.0.1.tar", last modified: Sun Apr  7 09:33:26 2024, max compression
+gzip compressed data, was "dltrain-0.0.2.tar", last modified: Sun Apr  7 10:17:19 2024, max compression
```

## Comparing `dltrain-0.0.1.tar` & `dltrain-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 09:33:26.555911 dltrain-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      813 2024-04-07 09:33:26.553911 dltrain-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      176 2024-04-07 09:17:15.000000 dltrain-0.0.1/README.md
--rw-rw-rw-   0        0        0      625 2024-04-07 09:33:21.000000 dltrain-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 09:33:26.555911 dltrain-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-07 09:33:26.503912 dltrain-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 09:33:26.530912 dltrain-0.0.1/src/dltrain/
--rw-rw-rw-   0        0        0      219 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:33:26.550912 dltrain-0.0.1/src/dltrain/builder/
--rw-rw-rw-   0        0        0      132 2024-04-05 16:31:47.000000 dltrain-0.0.1/src/dltrain/builder/__init__.py
--rw-rw-rw-   0        0        0     5620 2024-04-07 09:11:25.000000 dltrain-0.0.1/src/dltrain/builder/builder.py
--rw-rw-rw-   0        0        0      878 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/builder/optimizer.py
--rw-rw-rw-   0        0        0      764 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/builder/scheduler.py
--rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/checkpoint.py
--rw-rw-rw-   0        0        0     3917 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/dataset.py
--rw-rw-rw-   0        0        0     1235 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/delineator.py
--rw-rw-rw-   0        0        0      933 2024-04-05 11:07:29.000000 dltrain-0.0.1/src/dltrain/error.py
--rw-rw-rw-   0        0        0     1241 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/evaluation.py
--rw-rw-rw-   0        0        0     1738 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/forward.py
--rw-rw-rw-   0        0        0     4489 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/models.py
--rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/options.py
--rw-rw-rw-   0        0        0     9914 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/train.py
--rw-rw-rw-   0        0        0     1145 2024-04-07 09:09:29.000000 dltrain-0.0.1/src/dltrain/transform.py
--rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.0.1/src/dltrain/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-07 09:33:26.552912 dltrain-0.0.1/src/dltrain.egg-info/
--rw-rw-rw-   0        0        0      813 2024-04-07 09:33:26.000000 dltrain-0.0.1/src/dltrain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      582 2024-04-07 09:33:26.000000 dltrain-0.0.1/src/dltrain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 09:33:26.000000 dltrain-0.0.1/src/dltrain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-07 09:33:26.000000 dltrain-0.0.1/src/dltrain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 10:17:19.151307 dltrain-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-07 09:17:30.000000 dltrain-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      813 2024-04-07 10:17:19.150306 dltrain-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      176 2024-04-07 09:17:15.000000 dltrain-0.0.2/README.md
+-rw-rw-rw-   0        0        0      625 2024-04-07 10:17:12.000000 dltrain-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 10:17:19.151307 dltrain-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-07 10:17:19.115307 dltrain-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 10:17:19.133322 dltrain-0.0.2/src/dltrain/
+-rw-rw-rw-   0        0        0      219 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:17:19.148307 dltrain-0.0.2/src/dltrain/builder/
+-rw-rw-rw-   0        0        0      132 2024-04-05 16:31:47.000000 dltrain-0.0.2/src/dltrain/builder/__init__.py
+-rw-rw-rw-   0        0        0     5588 2024-04-07 10:16:53.000000 dltrain-0.0.2/src/dltrain/builder/builder.py
+-rw-rw-rw-   0        0        0      878 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/builder/optimizer.py
+-rw-rw-rw-   0        0        0      764 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/builder/scheduler.py
+-rw-rw-rw-   0        0        0      747 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/checkpoint.py
+-rw-rw-rw-   0        0        0     3917 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/dataset.py
+-rw-rw-rw-   0        0        0     1235 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/delineator.py
+-rw-rw-rw-   0        0        0      933 2024-04-05 11:07:29.000000 dltrain-0.0.2/src/dltrain/error.py
+-rw-rw-rw-   0        0        0     1241 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/evaluation.py
+-rw-rw-rw-   0        0        0     1738 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/forward.py
+-rw-rw-rw-   0        0        0     4489 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/models.py
+-rw-rw-rw-   0        0        0     1290 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/options.py
+-rw-rw-rw-   0        0        0     9914 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/train.py
+-rw-rw-rw-   0        0        0     1145 2024-04-07 09:09:29.000000 dltrain-0.0.2/src/dltrain/transform.py
+-rw-rw-rw-   0        0        0     5417 2024-04-07 08:49:36.000000 dltrain-0.0.2/src/dltrain/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-07 10:17:19.149307 dltrain-0.0.2/src/dltrain.egg-info/
+-rw-rw-rw-   0        0        0      813 2024-04-07 10:17:19.000000 dltrain-0.0.2/src/dltrain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      582 2024-04-07 10:17:19.000000 dltrain-0.0.2/src/dltrain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 10:17:19.000000 dltrain-0.0.2/src/dltrain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 10:17:19.000000 dltrain-0.0.2/src/dltrain.egg-info/top_level.txt
```

### Comparing `dltrain-0.0.1/LICENSE` & `dltrain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/PKG-INFO` & `dltrain-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dltrain-0.0.1/pyproject.toml` & `dltrain-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dltrain"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="XiaosYu", email="lijingyu_ai@163.com" },
 ]
 description = "This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dltrain-0.0.1/src/dltrain/builder/builder.py` & `dltrain-0.0.2/src/dltrain/builder/builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import string
 import random
 from typing import Dict
 
 import torch
 
-from src.dltrain.forward import Forward, SimpleForward
-from src.dltrain.delineator import Delineator, TrainEvalSetDelineator, RandomSplitDelineator
-from src.dltrain.transform import Container
-from src.dltrain.dataset import DLDataset
+from dltrain.forward import Forward, SimpleForward
+from dltrain.delineator import Delineator, TrainEvalSetDelineator, RandomSplitDelineator
+from dltrain.transform import Container
+from dltrain.dataset import DLDataset
 
 from torch.nn import Module, CrossEntropyLoss, MSELoss
 from torch.optim import Optimizer, Adam
 from torch import device
 from torch.optim.lr_scheduler import LRScheduler
 
-from src.dltrain.options import TrainOptions
-from src.dltrain.evaluation import EvaluationHandler
-from src.dltrain.models import create_native_model, PyTorchNativeCNN, MultilayerPerceptron
-from src.dltrain.transform import Transform
+from dltrain.options import TrainOptions
+from dltrain.evaluation import EvaluationHandler
+from dltrain.models import create_native_model, PyTorchNativeCNN, MultilayerPerceptron
+from dltrain.transform import Transform
 
 from .optimizer import OptimizerBuilder
 from .scheduler import SchedulerBuilder
 
 
 __all__ = [
     'TaskBuilder'
```

### Comparing `dltrain-0.0.1/src/dltrain/builder/optimizer.py` & `dltrain-0.0.2/src/dltrain/builder/optimizer.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/builder/scheduler.py` & `dltrain-0.0.2/src/dltrain/builder/scheduler.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/checkpoint.py` & `dltrain-0.0.2/src/dltrain/checkpoint.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/dataset.py` & `dltrain-0.0.2/src/dltrain/dataset.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/delineator.py` & `dltrain-0.0.2/src/dltrain/delineator.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/error.py` & `dltrain-0.0.2/src/dltrain/error.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/evaluation.py` & `dltrain-0.0.2/src/dltrain/evaluation.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/forward.py` & `dltrain-0.0.2/src/dltrain/forward.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/models.py` & `dltrain-0.0.2/src/dltrain/models.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/options.py` & `dltrain-0.0.2/src/dltrain/options.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/train.py` & `dltrain-0.0.2/src/dltrain/train.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/transform.py` & `dltrain-0.0.2/src/dltrain/transform.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain/utils.py` & `dltrain-0.0.2/src/dltrain/utils.py`

 * *Files identical despite different names*

### Comparing `dltrain-0.0.1/src/dltrain.egg-info/PKG-INFO` & `dltrain-0.0.2/src/dltrain.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dltrain
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a package for PyTorch training, and this project provides a large number of high-level training APIs and low-level interfaces to meet all training needs
 Author-email: XiaosYu <lijingyu_ai@163.com>
 Project-URL: Homepage, https://github.com/XiaosYu/dltrain
 Project-URL: Bug Tracker, https://github.com/XiaosYu/dltrain/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dltrain-0.0.1/src/dltrain.egg-info/SOURCES.txt` & `dltrain-0.0.2/src/dltrain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

