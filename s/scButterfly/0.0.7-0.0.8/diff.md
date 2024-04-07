# Comparing `tmp/scButterfly-0.0.7.tar.gz` & `tmp/scButterfly-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/cabins/atac2rna/atac2rna/docs/scButterfly-main/dist/.tmp-8il3rs0s/scButterfly-0.0.7.tar", last modified: Sat Mar 23 09:38:37 2024, max compression
+gzip compressed data, was "dist/scButterfly-0.0.8.tar", last modified: Sat Apr  6 08:03:41 2024, max compression
```

## Comparing `scButterfly-0.0.7.tar` & `scButterfly-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 atac2rna  (1005) atac2rna  (1006)        0 2024-03-23 09:38:37.457775 scButterfly-0.0.7/
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     1065 2024-02-11 09:32:24.000000 scButterfly-0.0.7/LICENSE
--rw-r--r--   0 atac2rna  (1005) atac2rna  (1006)     2409 2024-03-23 09:38:37.457775 scButterfly-0.0.7/PKG-INFO
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    10058 2024-02-11 09:32:24.000000 scButterfly-0.0.7/README.md
-drwxrwxr-x   0 atac2rna  (1005) atac2rna  (1006)        0 2024-03-23 09:38:37.457775 scButterfly-0.0.7/scButterfly/
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)      233 2024-02-11 11:00:28.000000 scButterfly-0.0.7/scButterfly/__init__.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    26785 2024-02-11 10:56:26.000000 scButterfly-0.0.7/scButterfly/butterfly.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     1497 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/calculate_cluster.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    10529 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/data_processing.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     3419 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/draw_cluster.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     1267 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/logger.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    27716 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/model_component.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    10424 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/model_utlis.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    19090 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/split_datasets.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    46145 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/train_model.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    46296 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/train_model_cite.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    46270 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/train_model_cite_background.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    49271 2024-02-11 09:32:24.000000 scButterfly-0.0.7/scButterfly/train_model_perturb.py
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)       22 2024-03-23 09:20:04.000000 scButterfly-0.0.7/scButterfly/version.py
-drwxrwxr-x   0 atac2rna  (1005) atac2rna  (1006)        0 2024-03-23 09:38:37.457775 scButterfly-0.0.7/scButterfly.egg-info/
--rw-r--r--   0 atac2rna  (1005) atac2rna  (1006)     2409 2024-03-23 09:38:37.000000 scButterfly-0.0.7/scButterfly.egg-info/PKG-INFO
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)      611 2024-03-23 09:38:37.000000 scButterfly-0.0.7/scButterfly.egg-info/SOURCES.txt
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)        1 2024-03-23 09:38:37.000000 scButterfly-0.0.7/scButterfly.egg-info/dependency_links.txt
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)      242 2024-03-23 09:38:37.000000 scButterfly-0.0.7/scButterfly.egg-info/requires.txt
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)       12 2024-03-23 09:38:37.000000 scButterfly-0.0.7/scButterfly.egg-info/top_level.txt
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)       38 2024-03-23 09:38:37.457775 scButterfly-0.0.7/setup.cfg
--rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     2570 2024-03-23 09:21:31.000000 scButterfly-0.0.7/setup.py
+drwxrwxr-x   0 atac2rna  (1005) atac2rna  (1006)        0 2024-04-06 08:03:41.180062 scButterfly-0.0.8/
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     1065 2024-02-11 09:32:24.000000 scButterfly-0.0.8/LICENSE
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     1914 2024-04-06 08:03:41.180062 scButterfly-0.0.8/PKG-INFO
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    10058 2024-02-11 09:32:24.000000 scButterfly-0.0.8/README.md
+drwxrwxr-x   0 atac2rna  (1005) atac2rna  (1006)        0 2024-04-06 08:03:41.176062 scButterfly-0.0.8/scButterfly/
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)      233 2024-02-11 11:00:28.000000 scButterfly-0.0.8/scButterfly/__init__.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    26785 2024-02-11 10:56:26.000000 scButterfly-0.0.8/scButterfly/butterfly.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     1497 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/calculate_cluster.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    10529 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/data_processing.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     3419 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/draw_cluster.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     1267 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/logger.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    27716 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/model_component.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    10424 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/model_utlis.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    19090 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/split_datasets.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    46145 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/train_model.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    46296 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/train_model_cite.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    46270 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/train_model_cite_background.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)    49271 2024-02-11 09:32:24.000000 scButterfly-0.0.8/scButterfly/train_model_perturb.py
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)       22 2024-04-06 07:50:18.000000 scButterfly-0.0.8/scButterfly/version.py
+drwxrwxr-x   0 atac2rna  (1005) atac2rna  (1006)        0 2024-04-06 08:03:41.176062 scButterfly-0.0.8/scButterfly.egg-info/
+-rw-r--r--   0 atac2rna  (1005) atac2rna  (1006)     1914 2024-04-06 08:03:40.000000 scButterfly-0.0.8/scButterfly.egg-info/PKG-INFO
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)      611 2024-04-06 08:03:40.000000 scButterfly-0.0.8/scButterfly.egg-info/SOURCES.txt
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)        1 2024-04-06 08:03:40.000000 scButterfly-0.0.8/scButterfly.egg-info/dependency_links.txt
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)      242 2024-04-06 08:03:40.000000 scButterfly-0.0.8/scButterfly.egg-info/requires.txt
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)       12 2024-04-06 08:03:40.000000 scButterfly-0.0.8/scButterfly.egg-info/top_level.txt
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)       38 2024-04-06 08:03:41.180062 scButterfly-0.0.8/setup.cfg
+-rw-rw-r--   0 atac2rna  (1005) atac2rna  (1006)     2557 2024-04-06 07:53:15.000000 scButterfly-0.0.8/setup.py
```

### Comparing `scButterfly-0.0.7/LICENSE` & `scButterfly-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/PKG-INFO` & `scButterfly-0.0.8/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,13 @@
 Metadata-Version: 2.1
 Name: scButterfly
-Version: 0.0.7
+Version: 0.0.8
 Summary: A versatile single-cell cross-modality translation method via dual-aligned variational autoencoders
 Home-page: https://github.com/BioX-NKU/scButterfly
 Author: BioX-NKU
 License: MIT Licence
 Keywords: single cell,cross-modality translation,dual-aligned variational autoencoder
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: scanpy>=1.9.1
-Requires-Dist: torch>=1.12.1
-Requires-Dist: torchvision>=0.13.1
-Requires-Dist: torchaudio>=0.12.1
-Requires-Dist: scikit-learn>=1.1.3
-Requires-Dist: scvi-tools==0.19.0
-Requires-Dist: scvi-colab
-Requires-Dist: scipy==1.9.3
-Requires-Dist: episcanpy==0.3.2
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: matplotlib>=3.6.2
-Requires-Dist: pot==0.9.0
-Requires-Dist: torchmetrics>=0.11.4
-Requires-Dist: leidenalg
-Requires-Dist: adjusttext
-Requires-Dist: jupyter
 
-Recent advancements for simultaneously profiling multi-omic modalities within individual cells have enabled the interrogation of cellular heterogeneity and molecular hierarchy. However, technical limitations lead to highly noisy multi-modal data and substantial costs. Although computational methods have been proposed to translate single-cell data across modalities, b broad applications of the methods still remain impeded b by formidable challenges. Here, we proposed scButterfly, a versatile single-cell cross-modality translation method based on dual-aligned variational autoencoders and innovative data augmentation schemes. With comprehensive experiments on multiple datasets, we provide compelling evidence of scButterfly's superiority over baseline methods in preserving cellular heterogeneity while translating d datasets o of various contexts and i in revealing cell type-specific biological insights.Besides, we d demonstrate the extensive applications of scButterfly for integrative multi-omics analysis of single-modality data, data enhancement of poor-quality single-cell multi-omics, and automatic cell type annotation of scATAC-seq data. Additionally, scButterfly can be generalized to unpaired data training and perturbation-response analysis via our data augmentation and optimal transport strategies. Moreover, scButterfly exhibits the capability i in consecutive translation from epigenome to transcriptome to proteome and has the potential to decipher novel biomarkers.
+Recent advancements for simultaneously profiling multi-omic modalities within individual cells have enabled the interrogation of cellular heterogeneity and molecular hierarchy. However, technical limitations lead to highly noisy multi-modal data and substantial costs. Although computational methods have been proposed to translate single-cell data across modalities, broad applications of the methods still remain impeded by formidable challenges. Here, we proposed scButterfly, a versatile single-cell cross-modality translation method based on dual-aligned variational autoencoders and innovative data augmentation schemes. With comprehensive experiments on multiple datasets, we provide compelling evidence of scButterfly's superiority over baseline methods in preserving cellular heterogeneity while translating datasets of various contexts and in revealing cell type-specific biological insights. Besides, we demonstrate the extensive applications of scButterfly for integrative multi-omics analysis of single-modality data, data enhancement of poor-quality single-cell multi-omics, and automatic cell type annotation of scATAC-seq data. Additionally, scButterfly can be generalized to unpaired data training and perturbation-response analysis via our data augmentation and optimal transport strategies. Moreover, scButterfly exhibits the capability in consecutive translation from epigenome to transcriptome to proteome and has the potential to decipher novel biomarkers.
```

### Comparing `scButterfly-0.0.7/README.md` & `scButterfly-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/butterfly.py` & `scButterfly-0.0.8/scButterfly/butterfly.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/calculate_cluster.py` & `scButterfly-0.0.8/scButterfly/calculate_cluster.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/data_processing.py` & `scButterfly-0.0.8/scButterfly/data_processing.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/draw_cluster.py` & `scButterfly-0.0.8/scButterfly/draw_cluster.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/logger.py` & `scButterfly-0.0.8/scButterfly/logger.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/model_component.py` & `scButterfly-0.0.8/scButterfly/model_component.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/model_utlis.py` & `scButterfly-0.0.8/scButterfly/model_utlis.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/split_datasets.py` & `scButterfly-0.0.8/scButterfly/split_datasets.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/train_model.py` & `scButterfly-0.0.8/scButterfly/train_model.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/train_model_cite.py` & `scButterfly-0.0.8/scButterfly/train_model_cite.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/train_model_cite_background.py` & `scButterfly-0.0.8/scButterfly/train_model_cite_background.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly/train_model_perturb.py` & `scButterfly-0.0.8/scButterfly/train_model_perturb.py`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/scButterfly.egg-info/PKG-INFO` & `scButterfly-0.0.8/scButterfly.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,29 +1,13 @@
 Metadata-Version: 2.1
 Name: scButterfly
-Version: 0.0.7
+Version: 0.0.8
 Summary: A versatile single-cell cross-modality translation method via dual-aligned variational autoencoders
 Home-page: https://github.com/BioX-NKU/scButterfly
 Author: BioX-NKU
 License: MIT Licence
 Keywords: single cell,cross-modality translation,dual-aligned variational autoencoder
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 License-File: LICENSE
-Requires-Dist: scanpy>=1.9.1
-Requires-Dist: torch>=1.12.1
-Requires-Dist: torchvision>=0.13.1
-Requires-Dist: torchaudio>=0.12.1
-Requires-Dist: scikit-learn>=1.1.3
-Requires-Dist: scvi-tools==0.19.0
-Requires-Dist: scvi-colab
-Requires-Dist: scipy==1.9.3
-Requires-Dist: episcanpy==0.3.2
-Requires-Dist: seaborn>=0.11.2
-Requires-Dist: matplotlib>=3.6.2
-Requires-Dist: pot==0.9.0
-Requires-Dist: torchmetrics>=0.11.4
-Requires-Dist: leidenalg
-Requires-Dist: adjusttext
-Requires-Dist: jupyter
 
-Recent advancements for simultaneously profiling multi-omic modalities within individual cells have enabled the interrogation of cellular heterogeneity and molecular hierarchy. However, technical limitations lead to highly noisy multi-modal data and substantial costs. Although computational methods have been proposed to translate single-cell data across modalities, b broad applications of the methods still remain impeded b by formidable challenges. Here, we proposed scButterfly, a versatile single-cell cross-modality translation method based on dual-aligned variational autoencoders and innovative data augmentation schemes. With comprehensive experiments on multiple datasets, we provide compelling evidence of scButterfly's superiority over baseline methods in preserving cellular heterogeneity while translating d datasets o of various contexts and i in revealing cell type-specific biological insights.Besides, we d demonstrate the extensive applications of scButterfly for integrative multi-omics analysis of single-modality data, data enhancement of poor-quality single-cell multi-omics, and automatic cell type annotation of scATAC-seq data. Additionally, scButterfly can be generalized to unpaired data training and perturbation-response analysis via our data augmentation and optimal transport strategies. Moreover, scButterfly exhibits the capability i in consecutive translation from epigenome to transcriptome to proteome and has the potential to decipher novel biomarkers.
+Recent advancements for simultaneously profiling multi-omic modalities within individual cells have enabled the interrogation of cellular heterogeneity and molecular hierarchy. However, technical limitations lead to highly noisy multi-modal data and substantial costs. Although computational methods have been proposed to translate single-cell data across modalities, broad applications of the methods still remain impeded by formidable challenges. Here, we proposed scButterfly, a versatile single-cell cross-modality translation method based on dual-aligned variational autoencoders and innovative data augmentation schemes. With comprehensive experiments on multiple datasets, we provide compelling evidence of scButterfly's superiority over baseline methods in preserving cellular heterogeneity while translating datasets of various contexts and in revealing cell type-specific biological insights. Besides, we demonstrate the extensive applications of scButterfly for integrative multi-omics analysis of single-modality data, data enhancement of poor-quality single-cell multi-omics, and automatic cell type annotation of scATAC-seq data. Additionally, scButterfly can be generalized to unpaired data training and perturbation-response analysis via our data augmentation and optimal transport strategies. Moreover, scButterfly exhibits the capability in consecutive translation from epigenome to transcriptome to proteome and has the potential to decipher novel biomarkers.
```

### Comparing `scButterfly-0.0.7/scButterfly.egg-info/SOURCES.txt` & `scButterfly-0.0.8/scButterfly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scButterfly-0.0.7/setup.py` & `scButterfly-0.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from setuptools import setup, find_packages
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 
 setup(
     name="scButterfly",
-    version="0.0.7",
+    version="0.0.8",
     description="A versatile single-cell cross-modality translation method via dual-aligned variational autoencoders",
-    long_description="Recent advancements for simultaneously profiling multi-omic modalities within individual cells have enabled the interrogation of cellular heterogeneity and molecular hierarchy. However, technical limitations lead to highly noisy multi-modal data and substantial costs. Although computational methods have been proposed to translate single-cell data across modalities, b broad applications of the methods still remain impeded b by formidable challenges. Here, we proposed scButterfly, a versatile single-cell cross-modality translation method based on dual-aligned variational autoencoders and innovative data augmentation schemes. With comprehensive experiments on multiple datasets, we provide compelling evidence of scButterfly's superiority over baseline methods in preserving cellular heterogeneity while translating d datasets o of various contexts and i in revealing cell type-specific biological insights.Besides, we d demonstrate the extensive applications of scButterfly for integrative multi-omics analysis of single-modality data, data enhancement of poor-quality single-cell multi-omics, and automatic cell type annotation of scATAC-seq data. Additionally, scButterfly can be generalized to unpaired data training and perturbation-response analysis via our data augmentation and optimal transport strategies. Moreover, scButterfly exhibits the capability i in consecutive translation from epigenome to transcriptome to proteome and has the potential to decipher novel biomarkers.",
+    long_description="Recent advancements for simultaneously profiling multi-omic modalities within individual cells have enabled the interrogation of cellular heterogeneity and molecular hierarchy. However, technical limitations lead to highly noisy multi-modal data and substantial costs. Although computational methods have been proposed to translate single-cell data across modalities, broad applications of the methods still remain impeded by formidable challenges. Here, we proposed scButterfly, a versatile single-cell cross-modality translation method based on dual-aligned variational autoencoders and innovative data augmentation schemes. With comprehensive experiments on multiple datasets, we provide compelling evidence of scButterfly's superiority over baseline methods in preserving cellular heterogeneity while translating datasets of various contexts and in revealing cell type-specific biological insights. Besides, we demonstrate the extensive applications of scButterfly for integrative multi-omics analysis of single-modality data, data enhancement of poor-quality single-cell multi-omics, and automatic cell type annotation of scATAC-seq data. Additionally, scButterfly can be generalized to unpaired data training and perturbation-response analysis via our data augmentation and optimal transport strategies. Moreover, scButterfly exhibits the capability in consecutive translation from epigenome to transcriptome to proteome and has the potential to decipher novel biomarkers.",
     license="MIT Licence",
     url="https://github.com/BioX-NKU/scButterfly",
     author="BioX-NKU",
     classifiers=[
         "Programming Language :: Python :: 3.9",
     ],
     keywords="single cell, cross-modality translation, dual-aligned variational autoencoder",
     packages=find_packages(),
     python_requires=">=3.9",
     install_requires=[
         'scanpy>=1.9.1',
-        'torch>=1.12.1',
-        'torchvision>=0.13.1',
-        'torchaudio>=0.12.1',
+        'torch==1.12.1',
+        'torchvision==0.13.1',
+        'torchaudio==0.12.1',
         'scikit-learn>=1.1.3',
         'scvi-tools==0.19.0',
         'scvi-colab',
         'scipy==1.9.3',
         'episcanpy==0.3.2',
         'seaborn>=0.11.2',
         'matplotlib>=3.6.2',
         'pot==0.9.0',
-        'torchmetrics>=0.11.4',
+        'torchmetrics==0.11.4',
         'leidenalg',
         'adjusttext',
         'jupyter'
     ]
 )
```

