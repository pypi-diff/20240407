# Comparing `tmp/solidipy_mipt-1.1.0.tar.gz` & `tmp/solidipy_mipt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidipy_mipt-1.1.0.tar", last modified: Sun Apr  7 15:49:44 2024, max compression
+gzip compressed data, was "solidipy_mipt-1.1.1.tar", last modified: Sun Apr  7 16:14:46 2024, max compression
```

## Comparing `solidipy_mipt-1.1.0.tar` & `solidipy_mipt-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 15:49:44.166484 solidipy_mipt-1.1.0/
--rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     5202 2024-04-07 15:49:44.164099 solidipy_mipt-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4093 2024-04-07 13:23:02.000000 solidipy_mipt-1.1.0/README.md
--rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 15:49:44.166484 solidipy_mipt-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1619 2024-04-07 15:49:07.000000 solidipy_mipt-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:49:44.075648 solidipy_mipt-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-07 15:49:44.098560 solidipy_mipt-1.1.0/src/solidipy_mipt/
--rw-rw-rw-   0        0        0      266 2024-04-06 05:51:26.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/__init__.py
--rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/_metrics.py
--rw-rw-rw-   0        0        0     4584 2024-04-07 15:46:23.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/_selection.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:49:44.146044 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/
--rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/__init__.py
--rw-rw-rw-   0        0        0     4450 2024-04-07 15:39:21.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/_np_regressor.py
--rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/_predictor_abc.py
--rw-rw-rw-   0        0        0     6195 2024-04-07 15:48:48.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/_wknn.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:49:44.151402 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/utils/
--rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/utils/__init__.py
--rw-rw-rw-   0        0        0     1638 2024-04-07 05:01:27.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/utils/distance.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:49:44.158956 solidipy_mipt-1.1.0/src/solidipy_mipt/utils/
--rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/utils/__init__.py
--rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/utils/errors.py
--rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.1.0/src/solidipy_mipt/utils/validate.py
-drwxrwxrwx   0        0        0        0 2024-04-07 15:49:44.162101 solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/
--rw-rw-rw-   0        0        0     5202 2024-04-07 15:49:44.000000 solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      713 2024-04-07 15:49:44.000000 solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 15:49:44.000000 solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-07 15:49:44.000000 solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-07 15:49:44.000000 solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 16:14:45.992981 solidipy_mipt-1.1.1/
+-rw-rw-rw-   0        0        0     1084 2024-04-05 11:14:23.000000 solidipy_mipt-1.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     5672 2024-04-07 16:14:45.988650 solidipy_mipt-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4563 2024-04-07 16:12:12.000000 solidipy_mipt-1.1.1/README.md
+-rw-rw-rw-   0        0        0       99 2024-04-05 18:33:29.000000 solidipy_mipt-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-07 16:14:45.992981 solidipy_mipt-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1619 2024-04-07 16:14:24.000000 solidipy_mipt-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:14:45.894123 solidipy_mipt-1.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-04-07 16:14:45.919711 solidipy_mipt-1.1.1/src/solidipy_mipt/
+-rw-rw-rw-   0        0        0      266 2024-04-06 05:51:26.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/__init__.py
+-rw-rw-rw-   0        0        0     3640 2024-04-07 05:01:29.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/_metrics.py
+-rw-rw-rw-   0        0        0     4584 2024-04-07 15:46:23.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/_selection.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:14:45.971702 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/
+-rw-rw-rw-   0        0        0      250 2024-04-07 05:06:47.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     4450 2024-04-07 15:39:21.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/_np_regressor.py
+-rw-rw-rw-   0        0        0     1604 2024-04-06 08:25:40.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/_predictor_abc.py
+-rw-rw-rw-   0        0        0     6195 2024-04-07 15:48:48.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/_wknn.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:14:45.976351 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/utils/
+-rw-rw-rw-   0        0        0       32 2024-04-06 06:42:40.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/utils/__init__.py
+-rw-rw-rw-   0        0        0     1638 2024-04-07 05:01:27.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/utils/distance.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:14:45.985058 solidipy_mipt-1.1.1/src/solidipy_mipt/utils/
+-rw-rw-rw-   0        0        0       46 2024-04-07 13:25:37.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/utils/__init__.py
+-rw-rw-rw-   0        0        0     2873 2024-04-07 13:43:27.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/utils/errors.py
+-rw-rw-rw-   0        0        0     1543 2024-04-07 09:32:48.000000 solidipy_mipt-1.1.1/src/solidipy_mipt/utils/validate.py
+drwxrwxrwx   0        0        0        0 2024-04-07 16:14:45.988650 solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/
+-rw-rw-rw-   0        0        0     5672 2024-04-07 16:14:45.000000 solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      713 2024-04-07 16:14:45.000000 solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 16:14:45.000000 solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-07 16:14:45.000000 solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-07 16:14:45.000000 solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/top_level.txt
```

### Comparing `solidipy_mipt-1.1.0/LICENSE.txt` & `solidipy_mipt-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/PKG-INFO` & `solidipy_mipt-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.1.0
+Version: 1.1.1
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
@@ -19,45 +19,45 @@
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 
-<a name="readme-top"></a>
+<a id="readme-top"></a>
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/othneildrew/Best-README-Template">
-    <img src="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/assets/images/logo.png" alt="Logo" width="80" height="80">
+  <a href="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/">
+    <img src="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/assets/images/logo.png?raw=true" alt="Logo" width="80" height="80">
   </a>
 
-  <h3 align="center">Solidipy</h3>
+  <h3 align="center">Solidipy-MIPT</h3>
 
   <p align="center">
     Make your ML solid!
     <br />
-    <a href="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/solidipy/example">Examples</a>
+    <a href="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples">Examples</a>
     ·
     <a href="https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
     ·
     <a href="https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
   </p>
 </div>
 
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
     <li>
-      [About The Project](#about-the-project)
+        <a href="#about-the-project">About The Project</a>
       <ul>
         <li><a href="#built-with">Built With</a></li>
       </ul>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
@@ -73,15 +73,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-*Solidipy* is a Python library designed to provide a solid foundation for machine learning tasks. It includes various machine learning algorithms such as k-nearest neighbors (KNN) and regressions, along with evaluation metrics to assess model performance.
+*Solidipy-MIPT* is a Python library designed to provide a solid foundation for machine learning tasks. It includes various machine learning algorithms such as Weighted k-nearest neighbors (WKNN) and regressions, along with evaluation metrics to assess model performance.
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built With
@@ -99,34 +99,48 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 To get a local copy up and running follow these simple example steps.
 
 ### Prerequisites
 
-Before installing *Solidipy* make sure you have last version of Python3 and pip.
+Before installing *Solidipy-MIPT* make sure you have last version of Python3 and pip.
 
 ### Installation
 
 You can install solidipy using pip:
 
 ```bash
-pip install solidipy_mipt
+pip install solidipy-mipt
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 #### Simple Weighted KNN example
 ```python
+import numpy as np
+from solidipy_mipt import accuracy
+from solidipy_mipt.algorithms import WKNN
+
+X = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
+y = np.array([0, 1, 0, 1])
+X_train, X_test, y_train, y_test = train_test_split(
+  X, y, train_ratio=0.6, shuffle=True
+)
+
+wknn = WKNN()
+wknn.fit(X_train, y_train)
+prediction = wknn.predict(X_test)
 
+print(accuracy(prediction, y_test))
 ```
 
 _For more examples, please refer to the [solidipy_mipt examples](https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples)_
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.0 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.1 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
@@ -10,43 +10,48 @@
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.10, <4 Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: numpy Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
                                     _[_L_o_g_o_]
-                              ******** SSoolliiddiippyy ********
+                            ******** SSoolliiddiippyy--MMIIPPTT ********
                              Make your ML solid!
                    _E_x_a_m_p_l_e_s Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
-   1. [About The Project](#about-the-project)
+   1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _C_o_n_t_r_i_b_u_t_i_n_g
    5. _L_i_c_e_n_s_e
    6. _C_o_n_t_a_c_t
-## About The Project *Solidipy* is a Python library designed to provide a solid
-foundation for machine learning tasks. It includes various machine learning
-algorithms such as k-nearest neighbors (KNN) and regressions, along with
-evaluation metrics to assess model performance.
+## About The Project *Solidipy-MIPT* is a Python library designed to provide a
+solid foundation for machine learning tasks. It includes various machine
+learning algorithms such as Weighted k-nearest neighbors (WKNN) and
+regressions, along with evaluation metrics to assess model performance.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With Major frameworks/libraries used to bootstrap solidipy. * [NumPy]
 (https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started To get a local copy up and running follow these simple
-example steps. ### Prerequisites Before installing *Solidipy* make sure you
-have last version of Python3 and pip. ### Installation You can install solidipy
-using pip: ```bash pip install solidipy_mipt ```
+example steps. ### Prerequisites Before installing *Solidipy-MIPT* make sure
+you have last version of Python3 and pip. ### Installation You can install
+solidipy using pip: ```bash pip install solidipy-mipt ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage #### Simple Weighted KNN example ```python ``` _For more examples,
-please refer to the [solidipy_mipt examples](https://github.com/Kynemallv/
-python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples)_
+## Usage #### Simple Weighted KNN example ```python import numpy as np from
+solidipy_mipt import accuracy from solidipy_mipt.algorithms import WKNN X =
+np.array([[1, 2], [3, 4], [5, 6], [7, 8]]) y = np.array([0, 1, 0, 1]) X_train,
+X_test, y_train, y_test = train_test_split( X, y, train_ratio=0.6, shuffle=True
+) wknn = WKNN() wknn.fit(X_train, y_train) prediction = wknn.predict(X_test)
+print(accuracy(prediction, y_test)) ``` _For more examples, please refer to the
+[solidipy_mipt examples](https://github.com/Kynemallv/python_mipt_dafe/tree/
+main/homeworks/sem2_hw1/solidipy_framework/examples)_
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `solidipy_mipt-1.1.0/README.md` & `solidipy_mipt-1.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-<a name="readme-top"></a>
+<a id="readme-top"></a>
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/othneildrew/Best-README-Template">
-    <img src="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/assets/images/logo.png" alt="Logo" width="80" height="80">
+  <a href="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/">
+    <img src="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/assets/images/logo.png?raw=true" alt="Logo" width="80" height="80">
   </a>
 
-  <h3 align="center">Solidipy</h3>
+  <h3 align="center">Solidipy-MIPT</h3>
 
   <p align="center">
     Make your ML solid!
     <br />
-    <a href="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/solidipy/example">Examples</a>
+    <a href="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples">Examples</a>
     ·
     <a href="https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
     ·
     <a href="https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
   </p>
 </div>
 
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
     <li>
-      [About The Project](#about-the-project)
+        <a href="#about-the-project">About The Project</a>
       <ul>
         <li><a href="#built-with">Built With</a></li>
       </ul>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
@@ -48,15 +48,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-*Solidipy* is a Python library designed to provide a solid foundation for machine learning tasks. It includes various machine learning algorithms such as k-nearest neighbors (KNN) and regressions, along with evaluation metrics to assess model performance.
+*Solidipy-MIPT* is a Python library designed to provide a solid foundation for machine learning tasks. It includes various machine learning algorithms such as Weighted k-nearest neighbors (WKNN) and regressions, along with evaluation metrics to assess model performance.
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built With
@@ -74,34 +74,48 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 To get a local copy up and running follow these simple example steps.
 
 ### Prerequisites
 
-Before installing *Solidipy* make sure you have last version of Python3 and pip.
+Before installing *Solidipy-MIPT* make sure you have last version of Python3 and pip.
 
 ### Installation
 
 You can install solidipy using pip:
 
 ```bash
-pip install solidipy_mipt
+pip install solidipy-mipt
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 #### Simple Weighted KNN example
 ```python
+import numpy as np
+from solidipy_mipt import accuracy
+from solidipy_mipt.algorithms import WKNN
+
+X = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
+y = np.array([0, 1, 0, 1])
+X_train, X_test, y_train, y_test = train_test_split(
+  X, y, train_ratio=0.6, shuffle=True
+)
+
+wknn = WKNN()
+wknn.fit(X_train, y_train)
+prediction = wknn.predict(X_test)
 
+print(accuracy(prediction, y_test))
 ```
 
 _For more examples, please refer to the [solidipy_mipt examples](https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples)_
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,38 +1,43 @@
 
                                     _[_L_o_g_o_]
-                              ******** SSoolliiddiippyy ********
+                            ******** SSoolliiddiippyy--MMIIPPTT ********
                              Make your ML solid!
                    _E_x_a_m_p_l_e_s Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
-   1. [About The Project](#about-the-project)
+   1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _C_o_n_t_r_i_b_u_t_i_n_g
    5. _L_i_c_e_n_s_e
    6. _C_o_n_t_a_c_t
-## About The Project *Solidipy* is a Python library designed to provide a solid
-foundation for machine learning tasks. It includes various machine learning
-algorithms such as k-nearest neighbors (KNN) and regressions, along with
-evaluation metrics to assess model performance.
+## About The Project *Solidipy-MIPT* is a Python library designed to provide a
+solid foundation for machine learning tasks. It includes various machine
+learning algorithms such as Weighted k-nearest neighbors (WKNN) and
+regressions, along with evaluation metrics to assess model performance.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With Major frameworks/libraries used to bootstrap solidipy. * [NumPy]
 (https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started To get a local copy up and running follow these simple
-example steps. ### Prerequisites Before installing *Solidipy* make sure you
-have last version of Python3 and pip. ### Installation You can install solidipy
-using pip: ```bash pip install solidipy_mipt ```
+example steps. ### Prerequisites Before installing *Solidipy-MIPT* make sure
+you have last version of Python3 and pip. ### Installation You can install
+solidipy using pip: ```bash pip install solidipy-mipt ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage #### Simple Weighted KNN example ```python ``` _For more examples,
-please refer to the [solidipy_mipt examples](https://github.com/Kynemallv/
-python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples)_
+## Usage #### Simple Weighted KNN example ```python import numpy as np from
+solidipy_mipt import accuracy from solidipy_mipt.algorithms import WKNN X =
+np.array([[1, 2], [3, 4], [5, 6], [7, 8]]) y = np.array([0, 1, 0, 1]) X_train,
+X_test, y_train, y_test = train_test_split( X, y, train_ratio=0.6, shuffle=True
+) wknn = WKNN() wknn.fit(X_train, y_train) prediction = wknn.predict(X_test)
+print(accuracy(prediction, y_test)) ``` _For more examples, please refer to the
+[solidipy_mipt examples](https://github.com/Kynemallv/python_mipt_dafe/tree/
+main/homeworks/sem2_hw1/solidipy_framework/examples)_
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `solidipy_mipt-1.1.0/setup.py` & `solidipy_mipt-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="solidipy_mipt",
-    version="1.1.0",
+    version="1.1.1",
     description="Make your ML solid!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework",
     author="Matvei Gorskii",
     author_email="matveygor41@gmail.com",
     classifiers=[
```

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/_metrics.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/_metrics.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/_selection.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/_selection.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/_np_regressor.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/_np_regressor.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/_predictor_abc.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/_predictor_abc.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/_wknn.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/_wknn.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/algorithms/utils/distance.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/algorithms/utils/distance.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/utils/errors.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/utils/errors.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt/utils/validate.py` & `solidipy_mipt-1.1.1/src/solidipy_mipt/utils/validate.py`

 * *Files identical despite different names*

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/PKG-INFO` & `solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solidipy_mipt
-Version: 1.1.0
+Version: 1.1.1
 Summary: Make your ML solid!
 Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Author: Matvei Gorskii
 Author-email: matveygor41@gmail.com
 Project-URL: Bug Reports, https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md
 Project-URL: Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework
 Keywords: ml
@@ -19,45 +19,45 @@
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
 
-<a name="readme-top"></a>
+<a id="readme-top"></a>
 
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
-  <a href="https://github.com/othneildrew/Best-README-Template">
-    <img src="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/assets/images/logo.png" alt="Logo" width="80" height="80">
+  <a href="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/">
+    <img src="https://github.com/Kynemallv/python_mipt_dafe/blob/main/homeworks/sem2_hw1/solidipy_framework/assets/images/logo.png?raw=true" alt="Logo" width="80" height="80">
   </a>
 
-  <h3 align="center">Solidipy</h3>
+  <h3 align="center">Solidipy-MIPT</h3>
 
   <p align="center">
     Make your ML solid!
     <br />
-    <a href="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/solidipy/example">Examples</a>
+    <a href="https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples">Examples</a>
     ·
     <a href="https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
     ·
     <a href="https://github.com/Kynemallv/python_mipt_dafe/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
   </p>
 </div>
 
 
 <!-- TABLE OF CONTENTS -->
 <details>
   <summary>Table of Contents</summary>
   <ol>
     <li>
-      [About The Project](#about-the-project)
+        <a href="#about-the-project">About The Project</a>
       <ul>
         <li><a href="#built-with">Built With</a></li>
       </ul>
     </li>
     <li>
       <a href="#getting-started">Getting Started</a>
       <ul>
@@ -73,15 +73,15 @@
 </details>
 
 
 
 <!-- ABOUT THE PROJECT -->
 ## About The Project
 
-*Solidipy* is a Python library designed to provide a solid foundation for machine learning tasks. It includes various machine learning algorithms such as k-nearest neighbors (KNN) and regressions, along with evaluation metrics to assess model performance.
+*Solidipy-MIPT* is a Python library designed to provide a solid foundation for machine learning tasks. It includes various machine learning algorithms such as Weighted k-nearest neighbors (WKNN) and regressions, along with evaluation metrics to assess model performance.
 
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 ### Built With
@@ -99,34 +99,48 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 To get a local copy up and running follow these simple example steps.
 
 ### Prerequisites
 
-Before installing *Solidipy* make sure you have last version of Python3 and pip.
+Before installing *Solidipy-MIPT* make sure you have last version of Python3 and pip.
 
 ### Installation
 
 You can install solidipy using pip:
 
 ```bash
-pip install solidipy_mipt
+pip install solidipy-mipt
 ```
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- USAGE EXAMPLES -->
 ## Usage
 
 #### Simple Weighted KNN example
 ```python
+import numpy as np
+from solidipy_mipt import accuracy
+from solidipy_mipt.algorithms import WKNN
+
+X = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
+y = np.array([0, 1, 0, 1])
+X_train, X_test, y_train, y_test = train_test_split(
+  X, y, train_ratio=0.6, shuffle=True
+)
+
+wknn = WKNN()
+wknn.fit(X_train, y_train)
+prediction = wknn.predict(X_test)
 
+print(accuracy(prediction, y_test))
 ```
 
 _For more examples, please refer to the [solidipy_mipt examples](https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples)_
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.0 Summary: Make your ML
+Metadata-Version: 2.1 Name: solidipy_mipt Version: 1.1.1 Summary: Make your ML
 solid! Home-page: https://github.com/Kynemallv/python_mipt_dafe/tree/main/
 homeworks/sem2_hw1/solidipy_framework Author: Matvei Gorskii Author-email:
 matveygor41@gmail.com Project-URL: Bug Reports, https://github.com/Kynemallv/
 python_mipt_dafe/issues/new?labels=bug&template=bug-report---.md Project-URL:
 Source, https://github.com/Kynemallv/python_mipt_dafe/tree/main/homeworks/
 sem2_hw1/solidipy_framework Keywords: ml Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: Topic ::
@@ -10,43 +10,48 @@
 Approved :: MIT License Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: Programming Language :: Python :: 3 ::
 Only Requires-Python: >=3.10, <4 Description-Content-Type: text/markdown
 License-File: LICENSE.txt Requires-Dist: numpy Requires-Dist: matplotlib
 Requires-Dist: scikit-learn
                                     _[_L_o_g_o_]
-                              ******** SSoolliiddiippyy ********
+                            ******** SSoolliiddiippyy--MMIIPPTT ********
                              Make your ML solid!
                    _E_x_a_m_p_l_e_s Â· _R_e_p_o_r_t_ _B_u_g Â· _R_e_q_u_e_s_t_ _F_e_a_t_u_r_e
 Table of Contents
-   1. [About The Project](#about-the-project)
+   1. _A_b_o_u_t_ _T_h_e_ _P_r_o_j_e_c_t
           o _B_u_i_l_t_ _W_i_t_h
    2. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
           o _P_r_e_r_e_q_u_i_s_i_t_e_s
           o _I_n_s_t_a_l_l_a_t_i_o_n
    3. _U_s_a_g_e
    4. _C_o_n_t_r_i_b_u_t_i_n_g
    5. _L_i_c_e_n_s_e
    6. _C_o_n_t_a_c_t
-## About The Project *Solidipy* is a Python library designed to provide a solid
-foundation for machine learning tasks. It includes various machine learning
-algorithms such as k-nearest neighbors (KNN) and regressions, along with
-evaluation metrics to assess model performance.
+## About The Project *Solidipy-MIPT* is a Python library designed to provide a
+solid foundation for machine learning tasks. It includes various machine
+learning algorithms such as Weighted k-nearest neighbors (WKNN) and
+regressions, along with evaluation metrics to assess model performance.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With Major frameworks/libraries used to bootstrap solidipy. * [NumPy]
 (https://numpy.org/) * [Matplotlib](https://matplotlib.org/)
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Getting Started To get a local copy up and running follow these simple
-example steps. ### Prerequisites Before installing *Solidipy* make sure you
-have last version of Python3 and pip. ### Installation You can install solidipy
-using pip: ```bash pip install solidipy_mipt ```
+example steps. ### Prerequisites Before installing *Solidipy-MIPT* make sure
+you have last version of Python3 and pip. ### Installation You can install
+solidipy using pip: ```bash pip install solidipy-mipt ```
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Usage #### Simple Weighted KNN example ```python ``` _For more examples,
-please refer to the [solidipy_mipt examples](https://github.com/Kynemallv/
-python_mipt_dafe/tree/main/homeworks/sem2_hw1/solidipy_framework/examples)_
+## Usage #### Simple Weighted KNN example ```python import numpy as np from
+solidipy_mipt import accuracy from solidipy_mipt.algorithms import WKNN X =
+np.array([[1, 2], [3, 4], [5, 6], [7, 8]]) y = np.array([0, 1, 0, 1]) X_train,
+X_test, y_train, y_test = train_test_split( X, y, train_ratio=0.6, shuffle=True
+) wknn = WKNN() wknn.fit(X_train, y_train) prediction = wknn.predict(X_test)
+print(accuracy(prediction, y_test)) ``` _For more examples, please refer to the
+[solidipy_mipt examples](https://github.com/Kynemallv/python_mipt_dafe/tree/
+main/homeworks/sem2_hw1/solidipy_framework/examples)_
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ## Contributing Contributions are what make the open source community such an
 amazing place to learn, inspire, and create. Any contributions you make are
 **greatly appreciated**. If you have a suggestion that would make this better,
 please fork the repo and create a pull request. You can also simply open an
 issue with the tag "enhancement". Don't forget to give the project a star!
 Thanks again! 1. Fork the Project 2. Create your Feature Branch (`git checkout
```

### Comparing `solidipy_mipt-1.1.0/src/solidipy_mipt.egg-info/SOURCES.txt` & `solidipy_mipt-1.1.1/src/solidipy_mipt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

