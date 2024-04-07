# Comparing `tmp/cancer_data-0.3.5.tar.gz` & `tmp/cancer_data-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cancer_data-0.3.5.tar", max compression
+gzip compressed data, was "cancer_data-0.3.6.tar", max compression
```

## Comparing `cancer_data-0.3.5.tar` & `cancer_data-0.3.6.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1064 2020-07-27 17:37:53.000000 cancer_data-0.3.5/LICENSE.txt
--rw-r--r--   0        0        0     5049 2021-08-25 17:03:29.079265 cancer_data-0.3.5/README.md
--rw-r--r--   0        0        0      139 2020-07-27 18:30:24.000000 cancer_data-0.3.5/cancer_data/.gitignore
--rw-r--r--   0        0        0      340 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/__init__.py
--rw-r--r--   0        0        0     6600 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/access.py
--rw-r--r--   0        0        0      687 2020-07-30 04:06:28.000000 cancer_data-0.3.5/cancer_data/checks.py
--rw-r--r--   0        0        0      498 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/config.py
--rw-r--r--   0        0        0        5 2020-07-30 23:42:17.000000 cancer_data-0.3.5/cancer_data/data/preview/.keep
--rw-r--r--   0        0        0        5 2020-07-30 23:42:18.000000 cancer_data-0.3.5/cancer_data/data/processed/.keep
--rw-r--r--   0        0        0        5 2020-07-30 23:42:19.000000 cancer_data-0.3.5/cancer_data/data/raw/.keep
--rw-r--r--   0        0        0        5 2020-07-30 23:42:21.000000 cancer_data-0.3.5/cancer_data/data/reference/.keep
--rw-r--r--   0        0        0     1308 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/download.py
--rw-r--r--   0        0        0     6174 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/process.py
--rw-r--r--   0        0        0    14132 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/processors/ccle.py
--rw-r--r--   0        0        0    10957 2021-09-02 02:09:59.269763 cancer_data-0.3.5/cancer_data/processors/depmap.py
--rw-r--r--   0        0        0     4857 2020-11-16 21:21:42.000000 cancer_data-0.3.5/cancer_data/processors/gtex.py
--rw-r--r--   0        0        0     1210 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/processors/other.py
--rw-r--r--   0        0        0    10060 2021-05-05 05:43:31.355703 cancer_data-0.3.5/cancer_data/processors/tcga.py
--rw-r--r--   0        0        0    17795 2022-01-08 20:08:45.293244 cancer_data-0.3.5/cancer_data/schema.csv
--rw-r--r--   0        0        0     5171 2020-11-16 21:23:12.000000 cancer_data-0.3.5/cancer_data/utils.py
--rw-r--r--   0        0        0      964 2022-01-08 20:20:46.595996 cancer_data-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     6106 2022-01-08 20:21:19.664439 cancer_data-0.3.5/setup.py
--rw-r--r--   0        0        0     6017 2022-01-08 20:21:19.664940 cancer_data-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-07 16:52:13.668284 cancer_data-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     5049 2024-04-07 16:52:13.668390 cancer_data-0.3.6/README.md
+-rw-r--r--   0        0        0      139 2024-04-07 16:52:13.668496 cancer_data-0.3.6/cancer_data/.gitignore
+-rw-r--r--   0        0        0      340 2024-04-07 16:52:13.668567 cancer_data-0.3.6/cancer_data/__init__.py
+-rw-r--r--   0        0        0     6600 2024-04-07 16:52:13.668643 cancer_data-0.3.6/cancer_data/access.py
+-rw-r--r--   0        0        0      687 2024-04-07 16:52:13.668722 cancer_data-0.3.6/cancer_data/checks.py
+-rw-r--r--   0        0        0      498 2024-04-07 16:52:13.668785 cancer_data-0.3.6/cancer_data/config.py
+-rw-r--r--   0        0        0        5 2024-04-07 16:52:13.668922 cancer_data-0.3.6/cancer_data/data/preview/.keep
+-rw-r--r--   0        0        0        5 2024-04-07 16:52:13.669011 cancer_data-0.3.6/cancer_data/data/processed/.keep
+-rw-r--r--   0        0        0        5 2024-04-07 16:52:13.669109 cancer_data-0.3.6/cancer_data/data/raw/.keep
+-rw-r--r--   0        0        0        5 2024-04-07 16:52:13.669199 cancer_data-0.3.6/cancer_data/data/reference/.keep
+-rw-r--r--   0        0        0     1308 2024-04-07 16:52:13.669276 cancer_data-0.3.6/cancer_data/download.py
+-rw-r--r--   0        0        0     6174 2024-04-07 16:52:13.669343 cancer_data-0.3.6/cancer_data/process.py
+-rw-r--r--   0        0        0    14132 2024-04-07 16:52:13.669506 cancer_data-0.3.6/cancer_data/processors/ccle.py
+-rw-r--r--   0        0        0    10957 2024-04-07 16:52:13.669682 cancer_data-0.3.6/cancer_data/processors/depmap.py
+-rw-r--r--   0        0        0     4857 2024-04-07 16:52:13.669763 cancer_data-0.3.6/cancer_data/processors/gtex.py
+-rw-r--r--   0        0        0     1210 2024-04-07 16:52:13.669830 cancer_data-0.3.6/cancer_data/processors/other.py
+-rw-r--r--   0        0        0    10060 2024-04-07 16:52:13.670017 cancer_data-0.3.6/cancer_data/processors/tcga.py
+-rw-r--r--   0        0        0    17795 2024-04-07 16:52:13.670150 cancer_data-0.3.6/cancer_data/schema.csv
+-rw-r--r--   0        0        0     5171 2024-04-07 16:52:13.670282 cancer_data-0.3.6/cancer_data/utils.py
+-rw-r--r--   0        0        0      932 2024-04-07 16:58:39.805564 cancer_data-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     6015 1970-01-01 00:00:00.000000 cancer_data-0.3.6/PKG-INFO
```

### Comparing `cancer_data-0.3.5/LICENSE.txt` & `cancer_data-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/README.md` & `cancer_data-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/access.py` & `cancer_data-0.3.6/cancer_data/access.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/checks.py` & `cancer_data-0.3.6/cancer_data/checks.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/download.py` & `cancer_data-0.3.6/cancer_data/download.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/process.py` & `cancer_data-0.3.6/cancer_data/process.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/processors/ccle.py` & `cancer_data-0.3.6/cancer_data/processors/ccle.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/processors/depmap.py` & `cancer_data-0.3.6/cancer_data/processors/depmap.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/processors/gtex.py` & `cancer_data-0.3.6/cancer_data/processors/gtex.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/processors/other.py` & `cancer_data-0.3.6/cancer_data/processors/other.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/processors/tcga.py` & `cancer_data-0.3.6/cancer_data/processors/tcga.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/schema.csv` & `cancer_data-0.3.6/cancer_data/schema.csv`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/cancer_data/utils.py` & `cancer_data-0.3.6/cancer_data/utils.py`

 * *Files identical despite different names*

### Comparing `cancer_data-0.3.5/pyproject.toml` & `cancer_data-0.3.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 [tool.poetry]
 name = "cancer_data"
-version = "0.3.5"
+version = "0.3.6"
 description = "Preprocessing for various cancer genomics datasets"
- authors = ["Kevin Hu <kevinhuwest@gmail.com>"]
+authors = ["Kevin Hu <kevinhuwest@gmail.com>"]
 
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kevinhu/cancer_data"
 repository = "https://github.com/kevinhu/cancer_data"
 keywords = ["cancer", "data", "genomics"]
 
-include = [
-    "LICENSE",
-]
+include = ["LICENSE"]
 
 [tool.poetry.dependencies]
-python = ">=3.6.1,<4.0"
-gtfparse = "^1.2.0"
-scipy = "^1.5.1"
-requests = "^2.24.0"
-tqdm = "^4.48.0"
-tables = "^3.6.1"
-xlrd = ">=1.2,<3.0"
-pandas = "^1.0.5"
+python = ">=3.9,<4.0"
+gtfparse = "^2.5.0"
+scipy = "^1.13.0"
+requests = "^2.31.0"
+tqdm = "^4.66.2"
+tables = "^3.9.2"
+xlrd = ">=2.0.1"
+pandas = "^2.2.1"
 
 [tool.poetry.dev-dependencies]
-ipython = "^7.16.2"
-matplotlib = "^3.3.4"
+matplotlib = "^3.8.4"
 seaborn = "^0.11.2"
 jupyter = "^1.0.0"
-black = "^20.8b1"
-isort = "^5.9.3"
-pylint = "^2.10.2"
+black = "^24.3.0"
+isort = "^5.13.2"
+pylint = "^3.1.0"
 poethepoet = "^0.10.0"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 use_parentheses = true
```

### Comparing `cancer_data-0.3.5/setup.py` & `cancer_data-0.3.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: cancer_data
+Version: 0.3.6
+Summary: Preprocessing for various cancer genomics datasets
+Home-page: https://github.com/kevinhu/cancer_data
+License: MIT
+Keywords: cancer,data,genomics
+Author: Kevin Hu
+Author-email: kevinhuwest@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: gtfparse (>=2.5.0,<3.0.0)
+Requires-Dist: pandas (>=2.2.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: scipy (>=1.13.0,<2.0.0)
+Requires-Dist: tables (>=3.9.2,<4.0.0)
+Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: xlrd (>=2.0.1)
+Project-URL: Repository, https://github.com/kevinhu/cancer_data
+Description-Content-Type: text/markdown
 
-packages = \
-['cancer_data', 'cancer_data.processors']
+# cancer_data
 
-package_data = \
-{'': ['*'],
- 'cancer_data': ['data/preview/.keep',
-                 'data/processed/.keep',
-                 'data/raw/.keep',
-                 'data/reference/*']}
-
-install_requires = \
-['gtfparse>=1.2.0,<2.0.0',
- 'pandas>=1.0.5,<2.0.0',
- 'requests>=2.24.0,<3.0.0',
- 'scipy>=1.5.1,<2.0.0',
- 'tables>=3.6.1,<4.0.0',
- 'tqdm>=4.48.0,<5.0.0',
- 'xlrd>=1.2,<3.0']
-
-setup_kwargs = {
-    'name': 'cancer-data',
-    'version': '0.3.5',
-    'description': 'Preprocessing for various cancer genomics datasets',
-    'long_description': '# cancer_data\n\nThis package provides unified methods for accessing popular datasets used in cancer research.\n\n**[Full documentation](https://cancer_data.kevinhu.io)**\n\n## Installation\n\n```bash\npip install cancer_data\n```\n\n## System requirements\n\nThe raw downloaded files occupy approximately 15 GB, and the processed HDFs take up about 10 GB. On a relatively recent machine with a fast SSD, processing all of the files after download takes about 3-4 hours. At least 16 GB of RAM is recommended for handling the large splicing tables.\n\n## Datasets\n\nA complete description of the datasets may be found in [schema.csv](https://github.com/kevinhu/cancer-data/blob/master/cancer_data/schema.csv).\n\n| Collection                                    | Datasets                                                                              | Portal                                                                                                                          |\n| --------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |\n| Cancer Cell Line Encyclopedia (CCLE)          | Many (see portal)                                                                     | https://portals.broadinstitute.org/ccle/data (registration required)                                                            |\n| Cancer Dependency Map (DepMap)                | Genome-wide CRISPR-cas9 and RNAi screens, gene expression, mutations, and copy number | https://depmap.org/portal/download/                                                                                             |\n| The Cancer Genome Atlas (TCGA)                | Mutations, RNAseq expression and splicing, and copy number                            | https://xenabrowser.net/datapages/?cohort=TCGA%20Pan-Cancer%20(PANCAN)&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443 |\n| The Genotype-Tissue Expression (GTEx) Project | RNAseq expression and splicing                                                        | https://gtexportal.org/home/datasets                                                                                            |\n\n## Features\n\nThe goal of this package is to make statistical analysis and coordination of these datasets easier. To that end, it provides the following features:\n\n1. Harmonization: datasets within a collection have sample IDs reduced to the same format. For instance, all CCLE+DepMap datasets have been modified to use Achilles/Arxspan IDs, rather than cell line names.\n2. Speed: processed datasets are all stored in high-performance [HDF5 format](https://en.wikipedia.org/wiki/Hierarchical_Data_Format), allowing large tables to be loaded orders of magnitude faster than with CSV or TSV formats.\n3. Space: tables of purely numerical values (e.g. gene expression, methylation, drug sensitivities) are stored in half-precision format. Compression is used for all tables, resulting in size reductions by factors of over 10 for sparse matrices such as mutation tables, and over 50 for highly-redundant tables such as gene-level copy number estimates.\n\n## How it works\n\nThe [schema](https://github.com/kevinhu/cancer-data/blob/master/cancer_data/schema.csv) serves as the reference point for all datasets used. Each dataset is identified by a unique `id` column, which also serves as its access identifier.\n\nDatasets are downloaded from the location specified in `download_url`, after which they are checked against the provided `downloaded_md5` hash.\n\nThe next steps depend on the `type` of the dataset:\n\n-   `reference` datasets, such as the hg19 FASTA files, are left as-is.\n-   `primary_dataset` objects are preprocessed and converted into HDF5 format.\n-   `secondary_dataset` objects are defined as being made from `primary_dataset` objects. These are also processed and converted into HDF5 format.\n\nTo keep track of which datasets are necessary for producing another, the `dependencies` column specifies the dataset `id`s that are required for making another. For instance, the `ccle_proteomics` dataset is dependent on the `ccle_annotations` dataset for converting cell line names to Achilles IDs. When running the processing pipeline, the package will automatically check that dependencies are met, and raise an error if they are not found.\n\n## Notes\n\nSome datasets have filtering applied to reduce their size. These are listed below:\n\n-   CCLE, GTEx, and TCGA splicing datasets have been filtered to remove splicing events with many missing values as well as those with low standard deviations.\n-   When constructing binary mutation matrices (`depmap_damaging` and `depmap_hotspot`), a minimum mutation frequency is used to remove especially rare (present in less than four samples) mutations.\n-   The TCGA MX splicing dataset is extremely large (approximately 10,000 rows by 900,000 columns), so it has been split column-wise into 8 chunks.\n',
-    'author': 'Kevin Hu',
-    'author_email': 'kevinhuwest@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/kevinhu/cancer_data',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6.1,<4.0',
-}
+This package provides unified methods for accessing popular datasets used in cancer research.
 
+**[Full documentation](https://cancer_data.kevinhu.io)**
+
+## Installation
+
+```bash
+pip install cancer_data
+```
+
+## System requirements
+
+The raw downloaded files occupy approximately 15 GB, and the processed HDFs take up about 10 GB. On a relatively recent machine with a fast SSD, processing all of the files after download takes about 3-4 hours. At least 16 GB of RAM is recommended for handling the large splicing tables.
+
+## Datasets
+
+A complete description of the datasets may be found in [schema.csv](https://github.com/kevinhu/cancer-data/blob/master/cancer_data/schema.csv).
+
+| Collection                                    | Datasets                                                                              | Portal                                                                                                                          |
+| --------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
+| Cancer Cell Line Encyclopedia (CCLE)          | Many (see portal)                                                                     | https://portals.broadinstitute.org/ccle/data (registration required)                                                            |
+| Cancer Dependency Map (DepMap)                | Genome-wide CRISPR-cas9 and RNAi screens, gene expression, mutations, and copy number | https://depmap.org/portal/download/                                                                                             |
+| The Cancer Genome Atlas (TCGA)                | Mutations, RNAseq expression and splicing, and copy number                            | https://xenabrowser.net/datapages/?cohort=TCGA%20Pan-Cancer%20(PANCAN)&removeHub=https%3A%2F%2Fxena.treehouse.gi.ucsc.edu%3A443 |
+| The Genotype-Tissue Expression (GTEx) Project | RNAseq expression and splicing                                                        | https://gtexportal.org/home/datasets                                                                                            |
+
+## Features
+
+The goal of this package is to make statistical analysis and coordination of these datasets easier. To that end, it provides the following features:
+
+1. Harmonization: datasets within a collection have sample IDs reduced to the same format. For instance, all CCLE+DepMap datasets have been modified to use Achilles/Arxspan IDs, rather than cell line names.
+2. Speed: processed datasets are all stored in high-performance [HDF5 format](https://en.wikipedia.org/wiki/Hierarchical_Data_Format), allowing large tables to be loaded orders of magnitude faster than with CSV or TSV formats.
+3. Space: tables of purely numerical values (e.g. gene expression, methylation, drug sensitivities) are stored in half-precision format. Compression is used for all tables, resulting in size reductions by factors of over 10 for sparse matrices such as mutation tables, and over 50 for highly-redundant tables such as gene-level copy number estimates.
+
+## How it works
+
+The [schema](https://github.com/kevinhu/cancer-data/blob/master/cancer_data/schema.csv) serves as the reference point for all datasets used. Each dataset is identified by a unique `id` column, which also serves as its access identifier.
+
+Datasets are downloaded from the location specified in `download_url`, after which they are checked against the provided `downloaded_md5` hash.
+
+The next steps depend on the `type` of the dataset:
+
+-   `reference` datasets, such as the hg19 FASTA files, are left as-is.
+-   `primary_dataset` objects are preprocessed and converted into HDF5 format.
+-   `secondary_dataset` objects are defined as being made from `primary_dataset` objects. These are also processed and converted into HDF5 format.
+
+To keep track of which datasets are necessary for producing another, the `dependencies` column specifies the dataset `id`s that are required for making another. For instance, the `ccle_proteomics` dataset is dependent on the `ccle_annotations` dataset for converting cell line names to Achilles IDs. When running the processing pipeline, the package will automatically check that dependencies are met, and raise an error if they are not found.
+
+## Notes
+
+Some datasets have filtering applied to reduce their size. These are listed below:
+
+-   CCLE, GTEx, and TCGA splicing datasets have been filtered to remove splicing events with many missing values as well as those with low standard deviations.
+-   When constructing binary mutation matrices (`depmap_damaging` and `depmap_hotspot`), a minimum mutation frequency is used to remove especially rare (present in less than four samples) mutations.
+-   The TCGA MX splicing dataset is extremely large (approximately 10,000 rows by 900,000 columns), so it has been split column-wise into 8 chunks.
 
-setup(**setup_kwargs)
```

