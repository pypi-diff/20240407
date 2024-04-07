# Comparing `tmp/gene_trajectory-0.1.8.tar.gz` & `tmp/gene_trajectory-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gene_trajectory-0.1.8.tar", last modified: Thu Apr  4 19:06:27 2024, max compression
+gzip compressed data, was "gene_trajectory-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gene_trajectory-0.1.8.tar` & `gene_trajectory-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,18 @@
--rw-r--r--   0        0        0     1070 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/LICENSE
--rw-r--r--   0        0        0     1039 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/README.md
--rw-r--r--   0        0        0        0 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/__init__.py
--rw-r--r--   0        0        0     1861 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/add_gene_bin_score.py
--rw-r--r--   0        0        0     4642 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/coarse_grain.py
--rw-r--r--   0        0        0     2846 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2337 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/diffusion_map.py
--rw-r--r--   0        0        0     5578 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/extract_gene_trajectory.py
--rw-r--r--   0        0        0     3845 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/gene_distance_shared.py
--rw-r--r--   0        0        0     1497 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/get_graph_distance.py
--rw-r--r--   0        0        0        0 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/plot/__init__.py
--rw-r--r--   0        0        0     2806 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/plot/gene_trajectory_plots.py
--rw-r--r--   0        0        0     1593 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/run_dm.py
--rw-r--r--   0        0        0        0 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/util/__init__.py
--rw-r--r--   0        0        0     1331 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/util/download_file.py
--rw-r--r--   0        0        0     3053 2024-04-04 19:06:22.860088 gene_trajectory-0.1.8/gene_trajectory/util/shared_array.py
--rw-r--r--   0        0        0     1351 2024-04-04 19:06:27.736133 gene_trajectory-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-04 19:06:22.924088 gene_trajectory-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0     1988 2024-04-04 19:06:22.924088 gene_trajectory-0.1.8/tests/example_data.py
--rw-r--r--   0        0        0      828 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_add_gene_bin_score.py
--rw-r--r--   0        0        0     3615 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_coarse_grain.py
--rw-r--r--   0        0        0     1770 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_compute_gene_distance_cmd.py
--rw-r--r--   0        0        0     2446 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_diffusion_map.py
--rw-r--r--   0        0        0     3356 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_extract_gene_trajectory.py
--rw-r--r--   0        0        0     1124 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_gene_distance_shared.py
--rw-r--r--   0        0        0      519 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_get_graph_distance.py
--rw-r--r--   0        0        0      411 2024-04-04 19:06:22.928088 gene_trajectory-0.1.8/tests/test_run_dm.py
--rw-r--r--   0        0        0     3504 1970-01-01 00:00:00.000000 gene_trajectory-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-07 18:01:15.531167 gene_trajectory-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3275 2024-04-07 18:01:15.531167 gene_trajectory-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/__init__.py
+-rw-r--r--   0        0        0     1861 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/add_gene_bin_score.py
+-rw-r--r--   0        0        0     4642 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/coarse_grain.py
+-rw-r--r--   0        0        0     2846 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/compute_gene_distance_cmd.py
+-rw-r--r--   0        0        0     2337 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/diffusion_map.py
+-rw-r--r--   0        0        0     5578 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/extract_gene_trajectory.py
+-rw-r--r--   0        0        0     3845 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/gene_distance_shared.py
+-rw-r--r--   0        0        0     1497 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/get_graph_distance.py
+-rw-r--r--   0        0        0        0 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/plot/__init__.py
+-rw-r--r--   0        0        0     2806 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/plot/gene_trajectory_plots.py
+-rw-r--r--   0        0        0     1593 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/run_dm.py
+-rw-r--r--   0        0        0        0 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/util/__init__.py
+-rw-r--r--   0        0        0     1331 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/util/download_file.py
+-rw-r--r--   0        0        0     3053 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/gene_trajectory/util/shared_array.py
+-rw-r--r--   0        0        0     1317 2024-04-07 18:01:15.599167 gene_trajectory-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4504 1970-01-01 00:00:00.000000 gene_trajectory-1.0.0/PKG-INFO
```

### Comparing `gene_trajectory-0.1.8/LICENSE` & `gene_trajectory-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/add_gene_bin_score.py` & `gene_trajectory-1.0.0/gene_trajectory/add_gene_bin_score.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/coarse_grain.py` & `gene_trajectory-1.0.0/gene_trajectory/coarse_grain.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/compute_gene_distance_cmd.py` & `gene_trajectory-1.0.0/gene_trajectory/compute_gene_distance_cmd.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/diffusion_map.py` & `gene_trajectory-1.0.0/gene_trajectory/diffusion_map.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/extract_gene_trajectory.py` & `gene_trajectory-1.0.0/gene_trajectory/extract_gene_trajectory.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/gene_distance_shared.py` & `gene_trajectory-1.0.0/gene_trajectory/gene_distance_shared.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/get_graph_distance.py` & `gene_trajectory-1.0.0/gene_trajectory/get_graph_distance.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/plot/gene_trajectory_plots.py` & `gene_trajectory-1.0.0/gene_trajectory/plot/gene_trajectory_plots.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/run_dm.py` & `gene_trajectory-1.0.0/gene_trajectory/run_dm.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/util/download_file.py` & `gene_trajectory-1.0.0/gene_trajectory/util/download_file.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/gene_trajectory/util/shared_array.py` & `gene_trajectory-1.0.0/gene_trajectory/util/shared_array.py`

 * *Files identical despite different names*

### Comparing `gene_trajectory-0.1.8/pyproject.toml` & `gene_trajectory-1.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 [build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
 [project]
 name = "gene-trajectory"
-version = "0.1.8"
+version = "1.0.0"
 description = "Compute gene trajectories"
+license = {file = "LICENSE"}
 readme = "README.md"
+
 authors = [
-    { name = "Francesco Strino", email = "francesco.strino@pcmgf.com" },
-    { name = "Rihao Qu", email = "rihao.qu@yale.edu" },
+    {name = "Francesco Strino", email = "francesco.strino@pcmgf.com"},
+    {name = "Rihao Qu", email = "rihao.qu@yale.edu"},
 ]
 maintainers = [
-    { name = "Francesco Strino", email = "francesco.strino@pcmgf.com" },
-    { name = "Rihao Qu", email = "rihao.qu@yale.edu" },
-]
-keywords = [
-    "Gene trajectory",
-    "scRNA-seq",
+    {name = "Francesco Strino", email = "francesco.strino@pcmgf.com"},
+    {name = "Rihao Qu", email = "rihao.qu@yale.edu"},
 ]
+
+keywords = ["Gene trajectory", "scRNA-seq"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "License :: OSI Approved :: BSD License",
     "Intended Audience :: Science/Research",
 ]
+
 requires-python = ">=3.9"
 dependencies = [
     "igraph>=0.10",
     "matplotlib>=3.6",
     "numpy>=1.23",
     "pandas>=1.5",
     "pot>=0.8.2",
@@ -38,22 +37,15 @@
     "scikit-misc>=0.1.3",
     "scikit-learn>=0.24",
     "scipy>=1.8",
     "seaborn>=0.13",
     "tqdm>=4.64.1",
 ]
 
-[project.license]
-file = "LICENSE"
-
 [project.optional-dependencies]
-dev = [
-    "pytest",
-    "twine",
-]
+dev = ["pytest", "twine"]
+
 
 [project.urls]
 Documentation = "https://github.com/KlugerLab/GeneTrajectory-python.git"
 Repository = "https://github.com/KlugerLab/GeneTrajectory-python.git"
 "Bug Tracker" = "https://github.com/KlugerLab/GeneTrajectory-python/issues"
-
-[tool]
```

### Comparing `gene_trajectory-0.1.8/PKG-INFO` & `gene_trajectory-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,47 @@
 Metadata-Version: 2.1
 Name: gene-trajectory
-Version: 0.1.8
+Version: 1.0.0
 Summary: Compute gene trajectories
-Keywords: Gene trajectory scRNA-seq
-Author-Email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
-Maintainer-Email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
-License: MIT License
-        
-        Copyright (c) 2024 PCMGF-Limited
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+Keywords: Gene trajectory,scRNA-seq
+Author-email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
+Maintainer-email: Francesco Strino <francesco.strino@pcmgf.com>, Rihao Qu <rihao.qu@yale.edu>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
-Project-URL: Documentation, https://github.com/KlugerLab/GeneTrajectory-python.git
-Project-URL: Repository, https://github.com/KlugerLab/GeneTrajectory-python.git
-Project-URL: Bug tracker, https://github.com/KlugerLab/GeneTrajectory-python/issues
-Requires-Python: >=3.9
 Requires-Dist: igraph>=0.10
 Requires-Dist: matplotlib>=3.6
 Requires-Dist: numpy>=1.23
 Requires-Dist: pandas>=1.5
 Requires-Dist: pot>=0.8.2
 Requires-Dist: scanpy>=1.9.3
 Requires-Dist: scikit-misc>=0.1.3
 Requires-Dist: scikit-learn>=0.24
 Requires-Dist: scipy>=1.8
 Requires-Dist: seaborn>=0.13
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: twine; extra == "dev"
+Requires-Dist: pytest ; extra == "dev"
+Requires-Dist: twine ; extra == "dev"
+Project-URL: Bug Tracker, https://github.com/KlugerLab/GeneTrajectory-python/issues
+Project-URL: Documentation, https://github.com/KlugerLab/GeneTrajectory-python.git
+Project-URL: Repository, https://github.com/KlugerLab/GeneTrajectory-python.git
 Provides-Extra: dev
-Description-Content-Type: text/markdown
 
 # Python Gene Trajectory
-This package is a Python implementation of [GeneTrajectory](https://github.com/KlugerLab/GeneTrajectory), 
-which is implemented in R. 
+This package is a Python implementation of GeneTrajectory. 
+The method is described in detail in the article [
+Gene trajectory inference for single-cell data by optimal transport metrics](
+https://doi.org/10.1038/s41587-024-02186-3).
+
+Documentation and tutorials are available at https://genetrajectory-python.readthedocs.io
+For the R implementation, go to the [GeneTrajectory](https://github.com/KlugerLab/GeneTrajectory) project. 
+
 
 Note that, although the implementation is equivalent, it will produce slightly different results to the R implementation
 because the signs of eigenvectors may differ and because of the randomness of K-means during the `coarse_grain` step. 
 
 
 # Install #
 The development version of the package can be installed as 
@@ -66,12 +51,29 @@
 
 The development version of the package can be installed as 
 ```
 pip install git+https://github.com/Klugerlab/GeneTrajectory-python.git
 ```
 
 # Tutorials #
-There are tutorials in Jupyter Notebook format in the
-[notebooks](https://github.com/KlugerLab/GeneTrajectory-python/tree/main/notebooks) folder of the GitHub project. 
-To get started, please follow the tutorial on Human myeloid cells on  
-[tutorial_human_myeloid.ipynb](https://github.com/KlugerLab/GeneTrajectory-python/blob/main/notebooks/tutorial_human_myeloid.ipynb)
+There are tutorials in Jupyter Notebook format in the [online documentation](https://genetrajectory-python.readthedocs.io) 
+and the [notebooks](https://github.com/KlugerLab/GeneTrajectory-python/tree/main/docs/notebooks) folder of the GitHub project. 
+
 
+# How to cite Gene Trajectory #
+If you use this tool in your research and find it useful, you can cite the following reference from our paper
+[Gene trajectory inference for single-cell data by optimal transport metrics](https://doi.org/10.1038/s41587-024-02186-3).
+In Bibtex format:
+```bibtex
+
+@article{qu_gene_2024,
+	title = {Gene trajectory inference for single-cell data by optimal transport metrics},
+	issn = {1546-1696},
+	url = {https://doi.org/10.1038/s41587-024-02186-3},
+	doi = {10.1038/s41587-024-02186-3},
+	abstract = {Single-cell RNA sequencing has been widely used to investigate cell state transitions and gene dynamics of biological processes. Current strategies to infer the sequential dynamics of genes in a process typically rely on constructing cell pseudotime through cell trajectory inference. However, the presence of concurrent gene processes in the same group of cells and technical noise can obscure the true progression of the processes studied. To address this challenge, we present GeneTrajectory, an approach that identifies trajectories of genes rather than trajectories of cells. Specifically, optimal transport distances are calculated between gene distributions across the cell–cell graph to extract gene programs and define their gene pseudotemporal order. Here we demonstrate that GeneTrajectory accurately extracts progressive gene dynamics in myeloid lineage maturation. Moreover, we show that GeneTrajectory deconvolves key gene programs underlying mouse skin hair follicle dermal condensate differentiation that could not be resolved by cell trajectory approaches. GeneTrajectory facilitates the discovery of gene programs that control the changes and activities of biological processes.},
+	journal = {Nature Biotechnology},
+	author = {Qu, Rihao and Cheng, Xiuyuan and Sefik, Esen and Stanley III, Jay S. and Landa, Boris and Strino, Francesco and Platt, Sarah and Garritano, James and Odell, Ian D. and Coifman, Ronald and Flavell, Richard A. and Myung, Peggy and Kluger, Yuval},
+	month = apr,
+	year = {2024},
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

