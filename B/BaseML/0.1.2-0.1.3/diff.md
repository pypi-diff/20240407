# Comparing `tmp/BaseML-0.1.2.tar.gz` & `tmp/BaseML-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseML-0.1.2.tar", last modified: Wed Mar 20 11:59:58 2024, max compression
+gzip compressed data, was "dist/BaseML-0.1.3.tar", last modified: Sun Apr  7 08:36:58 2024, max compression
```

## Comparing `BaseML-0.1.2.tar` & `BaseML-0.1.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 11:59:58.000000 BaseML-0.1.2/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML/
--rw-r--r--   0 user      (1001) user      (1001)     6148 2022-10-18 09:23:16.000000 BaseML-0.1.2/BaseML/.DS_Store
--rw-r--r--   0 user      (1001) user      (1001)    11349 2024-03-20 11:56:43.000000 BaseML-0.1.2/BaseML/BaseClassification.py
--rw-r--r--   0 user      (1001) user      (1001)     9246 2024-03-20 11:55:34.000000 BaseML-0.1.2/BaseML/BaseCluster.py
--rw-r--r--   0 user      (1001) user      (1001)     5888 2024-03-20 11:56:18.000000 BaseML-0.1.2/BaseML/BaseDimentionReduction.py
--rw-r--r--   0 user      (1001) user      (1001)    11194 2024-03-20 11:55:55.000000 BaseML-0.1.2/BaseML/BaseRegression.py
--rw-r--r--   0 user      (1001) user      (1001)     5686 2023-02-17 08:14:42.000000 BaseML-0.1.2/BaseML/IMGLoader.py
--rw-r--r--   0 user      (1001) user      (1001)    11357 2022-10-18 09:23:16.000000 BaseML-0.1.2/BaseML/LICENSE
--rw-r--r--   0 user      (1001) user      (1001)      314 2023-02-09 09:51:48.000000 BaseML-0.1.2/BaseML/__init__.py
--rw-r--r--   0 user      (1001) user      (1001)    12315 2024-03-20 11:57:08.000000 BaseML-0.1.2/BaseML/base.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML/examples/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2022-11-16 03:44:44.000000 BaseML-0.1.2/BaseML/examples/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)     2017 2024-03-11 06:24:05.000000 BaseML-0.1.2/BaseML/examples/boston_reg_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)      307 2022-11-16 03:24:16.000000 BaseML-0.1.2/BaseML/examples/cart_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)     2297 2024-03-20 11:55:10.000000 BaseML-0.1.2/BaseML/examples/iris_cls_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)      721 2023-10-19 08:37:13.000000 BaseML-0.1.2/BaseML/examples/iris_rdc_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)     1469 2024-03-20 06:17:02.000000 BaseML-0.1.2/BaseML/examples/kmeans_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)      373 2023-10-19 08:35:04.000000 BaseML-0.1.2/BaseML/examples/knn_demo.py
--rw-rw-r--   0 user      (1001) user      (1001)     1472 2024-03-20 11:59:14.000000 BaseML-0.1.2/BaseML/version.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      355 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      675 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       49 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1001) user      (1001)       94 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2024-03-20 11:59:58.000000 BaseML-0.1.2/BaseML.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-16 03:48:40.000000 BaseML-0.1.2/BaseML.egg-info/zip-safe
--rw-r--r--   0 user      (1001) user      (1001)    11357 2022-10-18 09:23:16.000000 BaseML-0.1.2/LICENSE
--rw-rw-r--   0 user      (1001) user      (1001)       27 2022-11-16 03:45:53.000000 BaseML-0.1.2/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      355 2024-03-20 11:59:58.000000 BaseML-0.1.2/PKG-INFO
--rw-r--r--   0 user      (1001) user      (1001)       67 2022-10-18 09:23:16.000000 BaseML-0.1.2/README.md
--rw-rw-r--   0 user      (1001) user      (1001)       38 2024-03-20 11:59:58.000000 BaseML-0.1.2/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4208 2024-03-20 11:59:07.000000 BaseML-0.1.2/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-07 08:36:58.000000 BaseML-0.1.3/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML/
+-rw-r--r--   0 user      (1001) user      (1001)     6148 2022-10-18 09:23:16.000000 BaseML-0.1.3/BaseML/.DS_Store
+-rw-r--r--   0 user      (1001) user      (1001)    11349 2024-03-20 11:56:43.000000 BaseML-0.1.3/BaseML/BaseClassification.py
+-rw-r--r--   0 user      (1001) user      (1001)     9246 2024-03-20 11:55:34.000000 BaseML-0.1.3/BaseML/BaseCluster.py
+-rw-r--r--   0 user      (1001) user      (1001)     5888 2024-03-20 11:56:18.000000 BaseML-0.1.3/BaseML/BaseDimentionReduction.py
+-rw-r--r--   0 user      (1001) user      (1001)    11403 2024-04-07 07:56:46.000000 BaseML-0.1.3/BaseML/BaseRegression.py
+-rw-r--r--   0 user      (1001) user      (1001)     5686 2023-02-17 08:14:42.000000 BaseML-0.1.3/BaseML/IMGLoader.py
+-rw-r--r--   0 user      (1001) user      (1001)    11357 2022-10-18 09:23:16.000000 BaseML-0.1.3/BaseML/LICENSE
+-rw-r--r--   0 user      (1001) user      (1001)      314 2023-02-09 09:51:48.000000 BaseML-0.1.3/BaseML/__init__.py
+-rw-r--r--   0 user      (1001) user      (1001)    12315 2024-03-20 11:57:08.000000 BaseML-0.1.3/BaseML/base.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML/examples/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2022-11-16 03:44:44.000000 BaseML-0.1.3/BaseML/examples/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2017 2024-04-07 07:55:37.000000 BaseML-0.1.3/BaseML/examples/boston_reg_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)      307 2022-11-16 03:24:16.000000 BaseML-0.1.3/BaseML/examples/cart_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)     2297 2024-03-20 11:55:10.000000 BaseML-0.1.3/BaseML/examples/iris_cls_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)      721 2023-10-19 08:37:13.000000 BaseML-0.1.3/BaseML/examples/iris_rdc_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1469 2024-03-20 06:17:02.000000 BaseML-0.1.3/BaseML/examples/kmeans_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)      373 2023-10-19 08:35:04.000000 BaseML-0.1.3/BaseML/examples/knn_demo.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1472 2024-04-07 08:36:31.000000 BaseML-0.1.3/BaseML/version.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      355 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      675 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       94 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2024-04-07 08:36:58.000000 BaseML-0.1.3/BaseML.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2022-11-16 03:48:40.000000 BaseML-0.1.3/BaseML.egg-info/zip-safe
+-rw-r--r--   0 user      (1001) user      (1001)    11357 2022-10-18 09:23:16.000000 BaseML-0.1.3/LICENSE
+-rw-rw-r--   0 user      (1001) user      (1001)       27 2022-11-16 03:45:53.000000 BaseML-0.1.3/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      355 2024-04-07 08:36:58.000000 BaseML-0.1.3/PKG-INFO
+-rw-r--r--   0 user      (1001) user      (1001)       67 2022-10-18 09:23:16.000000 BaseML-0.1.3/README.md
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2024-04-07 08:36:58.000000 BaseML-0.1.3/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4208 2024-04-07 08:36:22.000000 BaseML-0.1.3/setup.py
```

### Comparing `BaseML-0.1.2/BaseML/.DS_Store` & `BaseML-0.1.3/BaseML/.DS_Store`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/BaseClassification.py` & `BaseML-0.1.3/BaseML/BaseClassification.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/BaseCluster.py` & `BaseML-0.1.3/BaseML/BaseCluster.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/BaseDimentionReduction.py` & `BaseML-0.1.3/BaseML/BaseDimentionReduction.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/BaseRegression.py` & `BaseML-0.1.3/BaseML/BaseRegression.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,16 +186,22 @@
         if X is None and y_true is None:
             X = self.x_test
             y_true = self.y_test
         # assert len(self.x_train) > 0 and len(self.y_train) > 0,  \
         #     "Error Code: -601. No dataset is loaded."
         assert X is not None and y_true is not None,  "Error Code: -604. No valid data is provided or the validataion dataset is empty."
         assert len(X) > 0 and len(y_true) > 0,  "Error Code: -604. No valid data is provided or the validataion dataset is empty."
+        if self.algorithm == 'Polynomial':
+            from sklearn.pipeline import make_pipeline
+            model = make_pipeline(self.model, self.poly_linear_model)
+        else:
+            model = self.model
+
         visualizer = PredictionError(
-            self.model,
+            model,
             title="Actual vs. Predicted Values",
         )
 
         # self.y_test = self.y_test.squeeze()
         # visualizer.fit(self.x_train, self.y_train)
         # visualizer.score_ = visualizer.estimator.score(
         #     self.x_test, self.y_test)
```

### Comparing `BaseML-0.1.2/BaseML/IMGLoader.py` & `BaseML-0.1.3/BaseML/IMGLoader.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/LICENSE` & `BaseML-0.1.3/BaseML/LICENSE`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/base.py` & `BaseML-0.1.3/BaseML/base.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/examples/boston_reg_demo.py` & `BaseML-0.1.3/BaseML/examples/boston_reg_demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,26 +27,26 @@
     model.save()
 
 def iris_train():
     from BaseDT.dataset import split_tab_dataset
 # 指定待拆分的csv数据集
     path = "Height_data.csv"
     # 指定特征数据列、标签列、训练集比重
-    tx,ty,val_x,val_y = split_tab_dataset(path,data_column=range(0,3),label_column=3,train_val_ratio=0.8)
+    # tx,ty,val_x,val_y = split_tab_dataset(path,data_column=range(0,3),label_column=3,train_val_ratio=0.8)
     # 实例化模型
     model = reg(algorithm ="Polynomial")
     # 指定数据集格式
     # model.load_dataset(tx,ty,type = 'numpy')
     a = model.load_tab_data('iris_training.csv',train_val_ratio=0.8)
     # a = model.load_tab_data('Height_data.csv')
     # 开始训练
     model.train()
 
-    # model.valid('Height_data.csv',metrics='r2')
-    # model.metricplot()
+    model.valid('iris_training.csv',metrics='r2')
+    model.metricplot()
 
 def boston_reg_inference(algorithm = 'LinearRegression'): 
     # 划分数据集
     X_train, X_test, y_train, y_test=train_test_split(data,target,test_size = 0.2, random_state=42)
     # 实例化模型
     model = reg(algorithm = algorithm)
     # 加载模型权重文件
```

### Comparing `BaseML-0.1.2/BaseML/examples/iris_cls_demo.py` & `BaseML-0.1.3/BaseML/examples/iris_cls_demo.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/examples/iris_rdc_demo.py` & `BaseML-0.1.3/BaseML/examples/iris_rdc_demo.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/examples/kmeans_demo.py` & `BaseML-0.1.3/BaseML/examples/kmeans_demo.py`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/BaseML/version.py` & `BaseML-0.1.3/BaseML/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-__version__='0.1.2'
+__version__='0.1.3'
 __path__=os.path.abspath(os.getcwd())
 
 def parse_version_info(version_str):
     version_info = []
     for x in version_str.split('.'):
         if x.isdigit():
             version_info.append(int(x))
```

### Comparing `BaseML-0.1.2/BaseML.egg-info/SOURCES.txt` & `BaseML-0.1.3/BaseML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/LICENSE` & `BaseML-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `BaseML-0.1.2/setup.py` & `BaseML-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 #         os.system("pip install whl/pycocotools-2.0.4-cp37-cp37-win_amd64.whl")
 #     elif "3.6" in  sys.version:
 #         print(3.6)
 #         os.system("pip install whl/pycocotools-2.0.4-cp36-cp36-win_amd64.whl")
 
 setup(
     name='BaseML',
-    version='0.1.2',
+    version='0.1.3',
     description='BaseML provides numerous machine learning methods to quickly train and apply algorithms.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenBaseLab-Edu',
     packages=find_packages(),
     include_package_data=True,
```

