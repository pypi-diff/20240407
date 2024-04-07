# Comparing `tmp/pypharm-1.3.2.tar.gz` & `tmp/pypharm-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypharm-1.3.2.tar", last modified: Sun Mar 24 21:09:56 2024, max compression
+gzip compressed data, was "pypharm-1.3.3.tar", last modified: Sun Apr  7 19:42:46 2024, max compression
```

## Comparing `pypharm-1.3.2.tar` & `pypharm-1.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 21:09:56.781735 pypharm-1.3.2/
--rw-rw-rw-   0        0        0    14758 2024-03-24 21:09:56.781735 pypharm-1.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-24 21:09:56.776734 pypharm-1.3.2/PyPharm/
--rw-rw-rw-   0        0        0       90 2023-11-25 15:50:04.000000 pypharm-1.3.2/PyPharm/__init__.py
--rw-rw-rw-   0        0        0    20452 2024-03-13 19:09:03.000000 pypharm-1.3.2/PyPharm/country_optimization.py
--rw-rw-rw-   0        0        0    13156 2023-10-22 19:22:41.000000 pypharm-1.3.2/PyPharm/country_optimization_v2.py
--rw-rw-rw-   0        0        0    31380 2024-03-24 20:55:00.000000 pypharm-1.3.2/PyPharm/models.py
--rw-rw-rw-   0        0        0    14238 2024-03-13 20:07:04.000000 pypharm-1.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-24 21:09:56.780735 pypharm-1.3.2/pypharm.egg-info/
--rw-rw-rw-   0        0        0    14758 2024-03-24 21:09:56.000000 pypharm-1.3.2/pypharm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2024-03-24 21:09:56.000000 pypharm-1.3.2/pypharm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 21:09:56.000000 pypharm-1.3.2/pypharm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-03-24 21:09:56.000000 pypharm-1.3.2/pypharm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-24 21:09:56.000000 pypharm-1.3.2/pypharm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-24 21:09:56.782734 pypharm-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      827 2024-03-24 21:09:40.000000 pypharm-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 19:42:46.305100 pypharm-1.3.3/
+-rw-rw-rw-   0        0        0    14758 2024-04-07 19:42:46.305100 pypharm-1.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-07 19:42:46.300100 pypharm-1.3.3/PyPharm/
+-rw-rw-rw-   0        0        0       90 2023-11-25 15:50:04.000000 pypharm-1.3.3/PyPharm/__init__.py
+-rw-rw-rw-   0        0        0    20452 2024-03-13 19:09:03.000000 pypharm-1.3.3/PyPharm/country_optimization.py
+-rw-rw-rw-   0        0        0    13156 2023-10-22 19:22:41.000000 pypharm-1.3.3/PyPharm/country_optimization_v2.py
+-rw-rw-rw-   0        0        0    32080 2024-04-07 19:29:54.000000 pypharm-1.3.3/PyPharm/models.py
+-rw-rw-rw-   0        0        0    14238 2024-03-13 20:07:04.000000 pypharm-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-07 19:42:46.304101 pypharm-1.3.3/pypharm.egg-info/
+-rw-rw-rw-   0        0        0    14758 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-07 19:42:46.000000 pypharm-1.3.3/pypharm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-07 19:42:46.306100 pypharm-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      827 2024-04-07 19:42:07.000000 pypharm-1.3.3/setup.py
```

### Comparing `pypharm-1.3.2/PKG-INFO` & `pypharm-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypharm
-Version: 1.3.2
+Version: 1.3.3
 Summary: Module for solving pharmacokinetic problems
 Home-page: https://github.com/Krash13/PyPharm
 Author: Krash13
 Author-email: krasheninnikov.r.s@muctr.ru
 License: UNKNOWN
 Keywords: pharmacokinetics compartment-model
 Platform: UNKNOWN
```

### Comparing `pypharm-1.3.2/PyPharm/country_optimization.py` & `pypharm-1.3.3/PyPharm/country_optimization.py`

 * *Files identical despite different names*

### Comparing `pypharm-1.3.2/PyPharm/country_optimization_v2.py` & `pypharm-1.3.3/PyPharm/country_optimization_v2.py`

 * *Files identical despite different names*

### Comparing `pypharm-1.3.2/PyPharm/models.py` & `pypharm-1.3.3/PyPharm/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from multiprocessing import shared_memory
 
 import numpy as np
 from scipy.integrate import solve_ivp, RK45
-from scipy.integrate._ivp.rk import rk_step, SAFETY, MAX_FACTOR, MIN_FACTOR
+from scipy.integrate import simps
 from scipy.optimize import minimize
 from .country_optimization import CountriesAlgorithm
 from .country_optimization_v2 import CountriesAlgorithm_v2
 from numba import njit
 import matplotlib.pyplot as plt
 
 
@@ -125,15 +125,30 @@
             fun=self._compartment_model if not self.numba_option else lambda t, c: self._numba_compartment_model(t, c, self.configuration_matrix.astype(np.float64), self.outputs.astype(np.float64), self.volumes.astype(np.float64)),
             t_span=ts,
             y0=c0,
             max_step=max_step,
             t_eval=t_eval
         )
         return self.last_result
-    
+
+    def get_kinetic_params(self, t_max, d, compartment_number, max_step=0.01):
+        one_hour_result = self(t_max=1, d=d, compartment_number=compartment_number, max_step=max_step)
+        auc_1h = simps(one_hour_result.y[compartment_number], one_hour_result.t)
+        self(t_max=t_max, d=d, compartment_number=compartment_number, max_step=max_step)
+        auc = simps(self.last_result.y[compartment_number], self.last_result.t)
+        result_dict = {
+            'c_max': self.last_result.y[compartment_number].max(),
+            'V': self.volumes[compartment_number] if self.volumes is not None else None,
+            'AUC': auc,
+            'AUC_1h': auc_1h,
+            'Cl': d / auc
+        }
+        return result_dict
+
+
     def load_data_from_list(self, x):
         if self.configuration_matrix_target:
             self.configuration_matrix[self.configuration_matrix_target] = x[:self.configuration_matrix_target_count]
         if self.outputs_target:
             self.outputs[self.outputs_target] = x[
                                                 self.configuration_matrix_target_count:self.configuration_matrix_target_count + self.outputs_target_count]
         if self.volumes_target:
```

### Comparing `pypharm-1.3.2/README.md` & `pypharm-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `pypharm-1.3.2/pypharm.egg-info/PKG-INFO` & `pypharm-1.3.3/pypharm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypharm
-Version: 1.3.2
+Version: 1.3.3
 Summary: Module for solving pharmacokinetic problems
 Home-page: https://github.com/Krash13/PyPharm
 Author: Krash13
 Author-email: krasheninnikov.r.s@muctr.ru
 License: UNKNOWN
 Keywords: pharmacokinetics compartment-model
 Platform: UNKNOWN
```

### Comparing `pypharm-1.3.2/setup.py` & `pypharm-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def readme():
   with open('README.md', 'r', encoding="utf-8") as f:
     return f.read()
 
 setup(
   name='pypharm',
-  version='1.3.2',
+  version='1.3.3',
   author='Krash13',
   author_email='krasheninnikov.r.s@muctr.ru',
   description='Module for solving pharmacokinetic problems',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Krash13/PyPharm',
   packages=find_packages(),
```

