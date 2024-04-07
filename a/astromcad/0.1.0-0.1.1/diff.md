# Comparing `tmp/astromcad-0.1.0.tar.gz` & `tmp/astromcad-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astromcad-0.1.0.tar", last modified: Tue Apr  2 02:49:09 2024, max compression
+gzip compressed data, was "astromcad-0.1.1.tar", last modified: Sun Apr  7 16:19:13 2024, max compression
```

## Comparing `astromcad-0.1.0.tar` & `astromcad-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-02 02:49:09.370371 astromcad-0.1.0/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-02 02:49:09.369871 astromcad-0.1.0/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4694 2024-04-02 02:43:39.000000 astromcad-0.1.0/README.md
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-02 02:49:09.366597 astromcad-0.1.0/astromcad/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.0/astromcad/__init__.py
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     8944 2024-04-01 23:37:07.000000 astromcad-0.1.0/astromcad/astromcad.py
-drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-02 02:49:09.369117 astromcad-0.1.0/astromcad.egg-info/
--rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-02 02:49:09.000000 astromcad-0.1.0/astromcad.egg-info/PKG-INFO
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      227 2024-04-02 02:49:09.000000 astromcad-0.1.0/astromcad.egg-info/SOURCES.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-02 02:49:09.000000 astromcad-0.1.0/astromcad.egg-info/dependency_links.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       47 2024-04-02 02:49:09.000000 astromcad-0.1.0/astromcad.egg-info/requires.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-02 02:49:09.000000 astromcad-0.1.0/astromcad.egg-info/top_level.txt
--rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-02 02:49:09.370502 astromcad-0.1.0/setup.cfg
--rw-r--r--   0 rithwikgupta   (503) staff       (20)      671 2024-04-02 02:48:57.000000 astromcad-0.1.0/setup.py
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:19:13.385697 astromcad-0.1.1/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:19:13.385170 astromcad-0.1.1/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4728 2024-04-02 02:50:49.000000 astromcad-0.1.1/README.md
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:19:13.371108 astromcad-0.1.1/astromcad/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      116 2024-03-31 22:58:19.000000 astromcad-0.1.1/astromcad/__init__.py
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     9263 2024-04-07 16:11:54.000000 astromcad-0.1.1/astromcad/astromcad.py
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20) 10299554 2024-04-07 15:56:23.000000 astromcad-0.1.1/astromcad/iforests.pickle
+-rw-rw-r--   0 rithwikgupta   (503) staff       (20)  1435973 2024-04-07 15:51:54.000000 astromcad-0.1.1/astromcad/pretrained.keras
+drwxr-xr-x   0 rithwikgupta   (503) staff       (20)        0 2024-04-07 16:19:13.384435 astromcad-0.1.1/astromcad.egg-info/
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)     4337 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/PKG-INFO
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      280 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/SOURCES.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)        1 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/dependency_links.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       47 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/requires.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       10 2024-04-07 16:19:13.000000 astromcad-0.1.1/astromcad.egg-info/top_level.txt
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)       38 2024-04-07 16:19:13.385826 astromcad-0.1.1/setup.cfg
+-rw-r--r--   0 rithwikgupta   (503) staff       (20)      759 2024-04-07 16:18:58.000000 astromcad-0.1.1/setup.py
```

### Comparing `astromcad-0.1.0/PKG-INFO` & `astromcad-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.0
+Version: 0.1.1
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.0/README.md` & `astromcad-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Multi-Class Anomaly Detection for Astronomical Transients
 
 Paper Link: https://arxiv.org/abs/2403.14742
+
 243rd AAS Meeting iPoster: https://aas243-aas.ipostersessions.com/default.aspx?s=16-F9-A7-80-27-2E-87-DF-6A-01-E4-07-E4-A2-07-2C&guestview=true
 
 PyPI Package: https://pypi.org/project/astromcad/
 
 Additional Figures from the paper are in the Figures/ folder (fully updated to reflect most recent model).
 
 Code for training and plot generation in AstroMCAD.ipynb. Use this for plot generation and the python package for everything else.
@@ -75,15 +76,15 @@
 ```
 
 NOTE: If n_host is set to 0 during initalization, don't pass host galaxy information to any other function (or pass None). The class will not use the host galaxy information.
 
 In the case that you want to create your own classifer, be sure to name the input layers and latent layer something memorable. To initalize a `Custom` object with this classifier, use 
 
 ```python
-det.custom_model(model, lc_name, context_name, host_name)
+det.custom_model(model, lc_name, context_name, host_name) # Names of the respective layers
 det.create_encoder()
 ...
 ```
 
 To use the trained classifier, you can use `det.classify(light_curves, host_gals)`. To plot a real-time score evoluation, use `det.plot_real_time(light_curve)`
```

### Comparing `astromcad-0.1.0/astromcad/astromcad.py` & `astromcad-0.1.1/astromcad/astromcad.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,40 +4,49 @@
 from tensorflow.keras.layers import Input, LSTM, TimeDistributed, Dense, Masking, concatenate, GRU
 from tensorflow.keras.callbacks import EarlyStopping
 from tensorflow.keras import Model
 import numpy as np
 import matplotlib.pyplot as plt
 from sklearn.ensemble import IsolationForest
 import pickle
+import os
   
+SCRIPT_DIR = os.path.dirname(os.path.abspath(__file__))
 
 class Detect:
     ntimesteps=656
-
+    classes = []
     @classmethod
     def pad(cls, x_data):
         for ind in range(len(x_data)):
             np.pad(x_data[ind], ((0, cls.ntimesteps - len(x_data[ind])), (0, 0)))
         return x_data
 
     @classmethod
     def init(cls):
-        with open("pretrained", 'rb') as f:
-            cls.mod = pickle.load(f)
+        pretrained_model = os.path.join(SCRIPT_DIR, "pretrained.keras")
+        iforests = os.path.join(SCRIPT_DIR, "iforests.pickle")
+        cls.mod = Custom(656, 4, 2, 9, 12)
+        model = keras.models.load_model(pretrained_model)
+        cls.mod.custom_model(model, 'lc', 'host', 'latent')
+        mod.create_encoder()
+        cls.mod.mcif = mcif()
+        with open(iforests, 'rb') as f:
+            cls.mcif.iforests = pickle.load(f)
 
         
         # cls.mod = Custom(ntimesteps, 4, 2, 9, y_train.shape[-1])
         # cls.mod.custom_model(best.model, 'lc', 'host', 'latent')
         # cls.mod.create_encoder()
         # cls.mod.mcif = mcif()
         # cls.mod.mcif.iforests = best.iso_forests
 
     @classmethod
-    def classify(cls, x_data, host_gal):
-        return cls.mod.classify(x_data, host_gal)
+    def predict(cls, x_data, host_gal):
+        return cls.mod.predict(x_data, host_gal)
 
     @classmethod
     def anomaly_score(cls, x_data, host_gal):
         return cls.mod.score(x_data, host_gal)
 
     @classmethod
     def plot_real_time(cls, x_data, host_gal):
@@ -94,32 +103,32 @@
         
         self.latent_name='latent'
         
     def custom_model(self, model, lc_name, context_name, latent_name=None):
         self.model=model
         self.lc_name = lc_name
         self.context_name = context_name
-        self.latent_name=latent_name
+        self.latent_name = latent_name
         
-    def train(self, X_train, y_train, x_val, y_val, savepath, host_gal_train = None, host_gal_val = None):
+    def train(self, X_train, y_train, X_val, y_val, host_gal_train = None, host_gal_val = None, class_weights=None):
         
         early_stopping = EarlyStopping(
                                       patience=5,
                                       min_delta=0.001,                               
                                       monitor="val_loss",
                                       restore_best_weights=True
                                       )
         
         
-        
         if (self.contextual > 0):
             self.history = self.model.fit(x = [X_train, host_gal_train], validation_data=([X_val, host_gal_val], y_val), y = y_train, epochs=40, batch_size = 128, class_weight = class_weights, callbacks=[early_stopping])
         else:
             self.history = self.model.fit(x = [X_train], validation_data=([X_val], y_val), y = y_train, epochs=40, batch_size = 128, class_weight = class_weights, callbacks=[early_stopping])
-            
+ 
+
         
     
     def create_encoder(self):
         if (self.contextual):
             self.latent_model = Model(inputs=[self.model.get_layer(self.lc_name).input, self.model.get_layer(self.context_name).input], outputs=self.model.get_layer(self.latent_name).output)
         else:
             self.latent_model = Model(inputs=[self.model.get_layer(self.lc_name).input], outputs=self.model.get_layer(self.latent_name).output)
@@ -181,33 +190,29 @@
         for diff in splits:
             ans.append(scores[prv:diff])
             prv=diff
         
         return ans
 
 
-    def plot_real_time(self, x_data, host_gal, bands, time, flux, error, names = [], colors = []):
-        cur = np.array([j[1] for j in x_data])
+    def plot_real_time(self, x_data, bands, time_, flux_, error_, host_gal=None, names = [], colors = []):
         classification_scores = self.get_anomaly_real_time([x_data], [host_gal])[0]
-        
-        cur = cur[:len(classification_scores)]
-        assert(len(cur) == len(classification_scores))
 
         time = {i : [] for i in bands}
         flux = {i : [] for i in bands}
         error = {i : [] for i in bands}
 
         
     
-        for i in x_data[:len(classification_scores)]:
+        for ind, i in enumerate(x_data[:len(classification_scores)]):
             if (not np.any(i)):
                 break
-            flux[i[0]].append(i[2])
-            error[i[0]].append(i[3])
-            time[i[0]].append(i[1])
+            flux[i[0]].append(flux_[ind])
+            error[i[0]].append(error_[ind])
+            time[i[0]].append(time_[ind])
     
         fig, axs = plt.subplots(2, figsize=(10, 20))
     
         plt.subplots_adjust(wspace=0, hspace=0)
     
         axs[0].set_title(f"Real Time Anomaly Score", fontsize=30)
```

### Comparing `astromcad-0.1.0/astromcad.egg-info/PKG-INFO` & `astromcad-0.1.1/astromcad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astromcad
-Version: 0.1.0
+Version: 0.1.1
 Summary: Classifier-Based Anomaly Detection for Astronomical Transients
 Author: Rithwik Gupta
 Author-email: <rithwikca2020@gmail.com>
 Description-Content-Type: text/markdown
 
 # `astromcad` Package Documentation
```

### Comparing `astromcad-0.1.0/setup.py` & `astromcad-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 with open("READMEPyPI.md", "r") as fh:
     long_description = fh.read();
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Classifier-Based Anomaly Detection for Astronomical Transients'
 LONG_DESCRIPTION = long_description
 
 # Setting up
 setup(
     name="astromcad",
     version=VERSION,
@@ -17,9 +17,11 @@
     author_email="<rithwikca2020@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=['numpy', 'keras', 'tensorflow', 'matplotlib', 'scikit-learn'],
     keywords=[],
+    package_data={'astromcad': ['*.keras', '*.pickle']},
+    include_package_data=True,
     
 )
```

