# Comparing `tmp/efold-0.1.0.tar.gz` & `tmp/efold-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "efold-0.1.0.tar", last modified: Mon Apr  1 02:18:34 2024, max compression
+gzip compressed data, was "efold-0.1.1.tar", last modified: Sun Apr  7 01:47:52 2024, max compression
```

## Comparing `efold-0.1.0.tar` & `efold-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,53 @@
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-01 02:18:34.406152 efold-0.1.0/
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1068 2023-09-23 01:01:06.000000 efold-0.1.0/LICENSE
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3549 2024-04-01 02:18:34.405842 efold-0.1.0/PKG-INFO
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3105 2024-03-31 22:54:05.000000 efold-0.1.0/README.md
-drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-01 02:18:34.405475 efold-0.1.0/efold.egg-info/
--rw-r--r--   0 yvesmartin   (501) staff       (20)     3549 2024-04-01 02:18:34.000000 efold-0.1.0/efold.egg-info/PKG-INFO
--rw-r--r--   0 yvesmartin   (501) staff       (20)      148 2024-04-01 02:18:34.000000 efold-0.1.0/efold.egg-info/SOURCES.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)        1 2024-04-01 02:18:34.000000 efold-0.1.0/efold.egg-info/dependency_links.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)        6 2024-04-01 02:18:34.000000 efold-0.1.0/efold.egg-info/top_level.txt
--rw-r--r--   0 yvesmartin   (501) staff       (20)     1079 2024-03-31 22:50:11.000000 efold-0.1.0/pyproject.toml
--rw-r--r--   0 yvesmartin   (501) staff       (20)       38 2024-04-01 02:18:34.406210 efold-0.1.0/setup.cfg
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.949113 efold-0.1.1/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1068 2023-09-23 01:01:06.000000 efold-0.1.1/LICENSE
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       16 2024-04-07 01:33:39.000000 efold-0.1.1/MANIFEST.in
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3938 2024-04-07 01:47:52.948809 efold-0.1.1/PKG-INFO
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3015 2024-04-07 01:45:19.000000 efold-0.1.1/README.md
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.927751 efold-0.1.1/efold/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      113 2024-04-07 00:16:13.000000 efold-0.1.1/efold/__init__.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.929090 efold-0.1.1/efold/api/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       33 2024-04-07 01:36:46.000000 efold-0.1.1/efold/api/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3710 2024-04-07 01:45:38.000000 efold-0.1.1/efold/api/run.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1485 2024-04-07 01:33:39.000000 efold-0.1.1/efold/cli.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1419 2024-03-22 21:10:56.000000 efold-0.1.1/efold/config.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.932474 efold-0.1.1/efold/core/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       86 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7929 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/batch.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1338 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/callbacks.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      486 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/dataloader.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     9376 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/datamodule.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7604 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/dataset.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     4614 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/datatype.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1103 2024-04-07 00:16:13.000000 efold-0.1.1/efold/core/embeddings.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1248 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/loader.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1127 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/logger.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3895 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/metrics.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     8823 2024-04-07 01:33:39.000000 efold-0.1.1/efold/core/model.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3791 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/path.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)    13869 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/postprocess.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7319 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/sampler.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      704 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/util.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3550 2024-03-22 21:10:56.000000 efold-0.1.1/efold/core/visualisation.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.934054 efold-0.1.1/efold/models/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       34 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     8829 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/cnn.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)    32703 2024-04-07 01:33:39.000000 efold-0.1.1/efold/models/efold.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      568 2024-04-07 00:16:13.000000 efold-0.1.1/efold/models/factory.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     8602 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/ribonanza.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     7550 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/transformer.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     9462 2024-03-22 21:10:56.000000 efold-0.1.1/efold/models/unet.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.934319 efold-0.1.1/efold/resources/
+-rw-r--r--   0 yvesmartin   (501) staff       (20) 11228484 2024-04-07 00:16:13.000000 efold-0.1.1/efold/resources/efold_weights.pt
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.947691 efold-0.1.1/efold/util/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      417 2024-03-22 21:10:56.000000 efold-0.1.1/efold/util/__init__.py
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3957 2024-04-07 01:33:39.000000 efold-0.1.1/efold/util/format_conversion.py
+drwxr-xr-x   0 yvesmartin   (501) staff       (20)        0 2024-04-07 01:47:52.948315 efold-0.1.1/efold.egg-info/
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     3938 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/PKG-INFO
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      954 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/SOURCES.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)        1 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/dependency_links.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       40 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/entry_points.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      224 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/requires.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)        6 2024-04-07 01:47:52.000000 efold-0.1.1/efold.egg-info/top_level.txt
+-rw-r--r--   0 yvesmartin   (501) staff       (20)     1503 2024-04-07 01:47:48.000000 efold-0.1.1/pyproject.toml
+-rw-r--r--   0 yvesmartin   (501) staff       (20)       38 2024-04-07 01:47:52.949179 efold-0.1.1/setup.cfg
+-rw-r--r--   0 yvesmartin   (501) staff       (20)      759 2024-04-07 01:47:42.000000 efold-0.1.1/setup.py
```

### Comparing `efold-0.1.0/LICENSE` & `efold-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `efold-0.1.0/PKG-INFO` & `efold-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 Metadata-Version: 2.1
 Name: efold
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to build our DMS signal and RNAstructure prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.5.2
+Requires-Dist: matplotlib>=3.6.2
+Requires-Dist: plotly>=5.11.0
+Requires-Dist: torch>=1.13.1
+Requires-Dist: pytorch-lightning>=1.9.4
+Requires-Dist: lightning>=1.9.4
+Requires-Dist: torcheval>=0.0.6
+Requires-Dist: tensorboard>=2.11.2
+Requires-Dist: wandb
+Requires-Dist: rouskinhf
+Requires-Dist: einops
+Requires-Dist: huggingface-hub
+Requires-Dist: kaggle
+Requires-Dist: pre-commit
+Requires-Dist: scikit-learn
+Requires-Dist: envbash
+Requires-Dist: click
 
 # eFold
 
 This repo contains the pytorch code for our paper “*Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”* 
 
 [[BioRXiv](https://www.biorxiv.org/content/10.1101/2024.01.24.577093v1.full)] [[Data](https://huggingface.co/rouskinlab)]
 
-## Setup
-
-### Download eFold
+## Install
 
 ```bash
-git clone https://github.com/rouskinlab/efold
-```
-
-### Create your environment
-
-Using `virtualenv`
-
-```bash
-cd path/to/efold
-python -m venv .venv
-source .venv/bin/activate
-pip install -m requirements.txt
-```
-
-Using conda
-
-```bash
-cd path/to/efold
-conda create -n efold python=3.10
-conda activate efold
-pip install -m requirements.txt
-```
-
-### Install eFold
-
-```bash
-pip install path/to/efold
+pip install efold
 ```
 
 ## File structure
 
 ```bash
 bppm/ # bppm post processing step
 efold/
@@ -65,63 +54,83 @@
     weights.json
 # python module boilerplate
 LICENSE
 requirements.txt
 pyproject.toml
 ```
 
-## Data
 
-### List of the datasets we used
+## Inference mode
 
-A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
+### Using the command line
 
-### Get the data
+From a sequence:
 
-You can download our datasets using [rouskinHF](https://github.com/rouskinlab/rouskinhf):
+```bash
+efold AAACAUGAGGAUUACCCAUGU -o seq.txt
+cat seq.txt
+
+AAACAUGAGGAUUACCCAUGU
+..(((((.((....)))))))
+```
+
+or a fasta file:
 
 ```bash
-pip install rouskinhf
+efold --fasta example.fasta
 ```
 
-And in your code, write:
+Using different formats:
+```bash
+efold AAACAUGAGGAUUACCCAUGU -bp # base pairs
+efold AAACAUGAGGAUUACCCAUGU -db # dotbracket (default)
+```
+
+Output can be .json, .csv or .txt
+```bash
+efold AAACAUGAGGAUUACCCAUGU -o output.csv
+```
+
+Run help:
+```bash
+efold -h
+```
+
+### Using python
 
 ```python
->>> import rouskinhf
->>> data = rouskinhf.get_dataset('ribo500-blast') # look at the dataset names on huggingface
+>>> from efold import inference
+>>> inference('AACUGUGCUA', fmt='dotbracket')
+..(((((.((....)))))))
 ```
 
-## Inference mode
 
-### Using the command line
+## Data
 
-From a sequence:
+### List of the datasets we used
 
-```bash
-efold --sequence AACCTGGUG -o seq.txt
-cat seq.txt
-#TODO
-```
+A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
 
-or a fasta file:
+### Get the data
+
+You can download our datasets using [rouskinHF](https://github.com/rouskinlab/rouskinhf):
 
 ```bash
-efold --fasta example.fasta -o seq.txt
-cat seq.txt
-#TODO
+pip install rouskinhf
 ```
 
-### Using python
+And in your code, write:
 
 ```python
->>> from efold import inference
->>> inference(seq = 'AACUGUGCUA')
-#TODO
+>>> import rouskinhf
+>>> data = rouskinhf.get_dataset('ribo500-blast') # look at the dataset names on huggingface
 ```
 
+
+
 ## Reproducing our results
 
 Run the training script:
 
 ```bash
 cd path/to/efold
 python scripts/efold_training.py
```

### Comparing `efold-0.1.0/README.md` & `efold-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,17 @@
 # eFold
 
 This repo contains the pytorch code for our paper “*Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”* 
 
 [[BioRXiv](https://www.biorxiv.org/content/10.1101/2024.01.24.577093v1.full)] [[Data](https://huggingface.co/rouskinlab)]
 
-## Setup
-
-### Download eFold
+## Install
 
 ```bash
-git clone https://github.com/rouskinlab/efold
-```
-
-### Create your environment
-
-Using `virtualenv`
-
-```bash
-cd path/to/efold
-python -m venv .venv
-source .venv/bin/activate
-pip install -m requirements.txt
-```
-
-Using conda
-
-```bash
-cd path/to/efold
-conda create -n efold python=3.10
-conda activate efold
-pip install -m requirements.txt
-```
-
-### Install eFold
-
-```bash
-pip install path/to/efold
+pip install efold
 ```
 
 ## File structure
 
 ```bash
 bppm/ # bppm post processing step
 efold/
@@ -53,63 +25,83 @@
     weights.json
 # python module boilerplate
 LICENSE
 requirements.txt
 pyproject.toml
 ```
 
-## Data
 
-### List of the datasets we used
+## Inference mode
 
-A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
+### Using the command line
 
-### Get the data
+From a sequence:
 
-You can download our datasets using [rouskinHF](https://github.com/rouskinlab/rouskinhf):
+```bash
+efold AAACAUGAGGAUUACCCAUGU -o seq.txt
+cat seq.txt
+
+AAACAUGAGGAUUACCCAUGU
+..(((((.((....)))))))
+```
+
+or a fasta file:
 
 ```bash
-pip install rouskinhf
+efold --fasta example.fasta
 ```
 
-And in your code, write:
+Using different formats:
+```bash
+efold AAACAUGAGGAUUACCCAUGU -bp # base pairs
+efold AAACAUGAGGAUUACCCAUGU -db # dotbracket (default)
+```
+
+Output can be .json, .csv or .txt
+```bash
+efold AAACAUGAGGAUUACCCAUGU -o output.csv
+```
+
+Run help:
+```bash
+efold -h
+```
+
+### Using python
 
 ```python
->>> import rouskinhf
->>> data = rouskinhf.get_dataset('ribo500-blast') # look at the dataset names on huggingface
+>>> from efold import inference
+>>> inference('AACUGUGCUA', fmt='dotbracket')
+..(((((.((....)))))))
 ```
 
-## Inference mode
 
-### Using the command line
+## Data
 
-From a sequence:
+### List of the datasets we used
 
-```bash
-efold --sequence AACCTGGUG -o seq.txt
-cat seq.txt
-#TODO
-```
+A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
 
-or a fasta file:
+### Get the data
+
+You can download our datasets using [rouskinHF](https://github.com/rouskinlab/rouskinhf):
 
 ```bash
-efold --fasta example.fasta -o seq.txt
-cat seq.txt
-#TODO
+pip install rouskinhf
 ```
 
-### Using python
+And in your code, write:
 
 ```python
->>> from efold import inference
->>> inference(seq = 'AACUGUGCUA')
-#TODO
+>>> import rouskinhf
+>>> data = rouskinhf.get_dataset('ribo500-blast') # look at the dataset names on huggingface
 ```
 
+
+
 ## Reproducing our results
 
 Run the training script:
 
 ```bash
 cd path/to/efold
 python scripts/efold_training.py
```

### Comparing `efold-0.1.0/efold.egg-info/PKG-INFO` & `efold-0.1.1/efold.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 Metadata-Version: 2.1
 Name: efold
-Version: 0.1.0
+Version: 0.1.1
 Summary: A library to build our DMS signal and RNAstructure prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas>=1.5.2
+Requires-Dist: matplotlib>=3.6.2
+Requires-Dist: plotly>=5.11.0
+Requires-Dist: torch>=1.13.1
+Requires-Dist: pytorch-lightning>=1.9.4
+Requires-Dist: lightning>=1.9.4
+Requires-Dist: torcheval>=0.0.6
+Requires-Dist: tensorboard>=2.11.2
+Requires-Dist: wandb
+Requires-Dist: rouskinhf
+Requires-Dist: einops
+Requires-Dist: huggingface-hub
+Requires-Dist: kaggle
+Requires-Dist: pre-commit
+Requires-Dist: scikit-learn
+Requires-Dist: envbash
+Requires-Dist: click
 
 # eFold
 
 This repo contains the pytorch code for our paper “*Diverse Database and Machine Learning Model to narrow the generalization gap in RNA structure prediction”* 
 
 [[BioRXiv](https://www.biorxiv.org/content/10.1101/2024.01.24.577093v1.full)] [[Data](https://huggingface.co/rouskinlab)]
 
-## Setup
-
-### Download eFold
+## Install
 
 ```bash
-git clone https://github.com/rouskinlab/efold
-```
-
-### Create your environment
-
-Using `virtualenv`
-
-```bash
-cd path/to/efold
-python -m venv .venv
-source .venv/bin/activate
-pip install -m requirements.txt
-```
-
-Using conda
-
-```bash
-cd path/to/efold
-conda create -n efold python=3.10
-conda activate efold
-pip install -m requirements.txt
-```
-
-### Install eFold
-
-```bash
-pip install path/to/efold
+pip install efold
 ```
 
 ## File structure
 
 ```bash
 bppm/ # bppm post processing step
 efold/
@@ -65,63 +54,83 @@
     weights.json
 # python module boilerplate
 LICENSE
 requirements.txt
 pyproject.toml
 ```
 
-## Data
 
-### List of the datasets we used
+## Inference mode
 
-A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
+### Using the command line
 
-### Get the data
+From a sequence:
 
-You can download our datasets using [rouskinHF](https://github.com/rouskinlab/rouskinhf):
+```bash
+efold AAACAUGAGGAUUACCCAUGU -o seq.txt
+cat seq.txt
+
+AAACAUGAGGAUUACCCAUGU
+..(((((.((....)))))))
+```
+
+or a fasta file:
 
 ```bash
-pip install rouskinhf
+efold --fasta example.fasta
 ```
 
-And in your code, write:
+Using different formats:
+```bash
+efold AAACAUGAGGAUUACCCAUGU -bp # base pairs
+efold AAACAUGAGGAUUACCCAUGU -db # dotbracket (default)
+```
+
+Output can be .json, .csv or .txt
+```bash
+efold AAACAUGAGGAUUACCCAUGU -o output.csv
+```
+
+Run help:
+```bash
+efold -h
+```
+
+### Using python
 
 ```python
->>> import rouskinhf
->>> data = rouskinhf.get_dataset('ribo500-blast') # look at the dataset names on huggingface
+>>> from efold import inference
+>>> inference('AACUGUGCUA', fmt='dotbracket')
+..(((((.((....)))))))
 ```
 
-## Inference mode
 
-### Using the command line
+## Data
 
-From a sequence:
+### List of the datasets we used
 
-```bash
-efold --sequence AACCTGGUG -o seq.txt
-cat seq.txt
-#TODO
-```
+A breakdown of the data we used is summarized [here](https://github.com/rouskinlab/efold_data). All the data is stored on the [HuggingFace](https://huggingface.co/rouskinlab). 
 
-or a fasta file:
+### Get the data
+
+You can download our datasets using [rouskinHF](https://github.com/rouskinlab/rouskinhf):
 
 ```bash
-efold --fasta example.fasta -o seq.txt
-cat seq.txt
-#TODO
+pip install rouskinhf
 ```
 
-### Using python
+And in your code, write:
 
 ```python
->>> from efold import inference
->>> inference(seq = 'AACUGUGCUA')
-#TODO
+>>> import rouskinhf
+>>> data = rouskinhf.get_dataset('ribo500-blast') # look at the dataset names on huggingface
 ```
 
+
+
 ## Reproducing our results
 
 Run the training script:
 
 ```bash
 cd path/to/efold
 python scripts/efold_training.py
```

### Comparing `efold-0.1.0/pyproject.toml` & `efold-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,39 +3,58 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['efold']
 
 [project]
 name =  "efold"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to build our DMS signal and RNAstructure prediction models."
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.10"
 ]
 requires-python = ">=3.10"
+dependencies = [
+    "pandas>=1.5.2",
+    "matplotlib>=3.6.2",
+    "plotly>=5.11.0",
+    "torch>=1.13.1",
+    "pytorch-lightning>=1.9.4",
+    "lightning>=1.9.4",
+    "torcheval>=0.0.6",
+    "tensorboard>=2.11.2",
+    "wandb",
+    "rouskinhf",
+    "einops",
+    "huggingface-hub",
+    "kaggle",
+    "pre-commit",
+    "scikit-learn",
+    "envbash",
+    "click",
+]
 
 [tool.pytest.ini_options]
 # add docstrings
 addopts = "--doctest-modules --doctest-glob='*.py' -v --capture=no --envfile env"
 pythonpath = [
   "efold",
 ]
 testpaths = ['tests', 'efold']
 junit_family = "xunit2"
 
 [tool.poetry.include]
-include = ["efold/resources/*.pt"]
+include = ["efold/resources/*.pt", 'requirements.txt']
 
 [tool.black]
 line-length = 88
 target-version = ['py310']
 include = '\.pyi?$'
 exclude = '''
 /(
@@ -46,7 +65,10 @@
   | \.env
   | _build
   | buck-out
   | build
   | dist
 )/
 '''
+
+[project.scripts]
+efold = "efold.cli:cli"
```

