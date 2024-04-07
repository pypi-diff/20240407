# Comparing `tmp/iderare-pheno-0.3.5.tar.gz` & `tmp/iderare-pheno-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.3.5.tar", last modified: Sat Apr  6 19:01:19 2024, max compression
+gzip compressed data, was "iderare-pheno-0.4.0.tar", last modified: Sun Apr  7 10:23:31 2024, max compression
```

## Comparing `iderare-pheno-0.3.5.tar` & `iderare-pheno-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.224584 iderare-pheno-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 19:01:19.224584 iderare-pheno-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.128584 iderare-pheno-0.3.5/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.128584 iderare-pheno-0.3.5/iderare_pheno/phenotype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.164584 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/
--rw-r--r--   0 runner    (1001) docker     (127) 19051578 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/genes_to_phenotype.txt
--rw-r--r--   0 runner    (1001) docker     (127)  9995624 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/hp.obo
--rw-r--r--   0 runner    (1001) docker     (127) 31896677 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/phenotype.hpoa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.220584 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/
--rw-r--r--   0 runner    (1001) docker     (127)   196778 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/icd102omim_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   224561 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  6033462 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  7205315 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   218406 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)   232073 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)  1298790 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/simrec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.220584 iderare-pheno-0.3.5/iderare_pheno/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/templates/template_iderare.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.220584 iderare-pheno-0.3.5/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:01:19.224584 iderare-pheno-0.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.476653 iderare-pheno-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-07 10:23:31.476653 iderare-pheno-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.384652 iderare-pheno-0.4.0/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.380652 iderare-pheno-0.4.0/iderare_pheno/phenotype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.416653 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 19051578 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  9995624 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/hp.obo
+-rw-r--r--   0 runner    (1001) docker     (127) 31896677 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/data/phenotype.hpoa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.472653 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/
+-rw-r--r--   0 runner    (1001) docker     (127)   196778 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   224561 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  6033462 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  7205315 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   218406 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   232073 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  1298790 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/simrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.472653 iderare-pheno-0.4.0/iderare_pheno/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/templates/template_iderare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 10:23:31.472653 iderare-pheno-0.4.0/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-07 10:23:31.000000 iderare-pheno-0.4.0/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-07 10:22:43.000000 iderare-pheno-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 10:23:31.476653 iderare-pheno-0.4.0/setup.cfg
```

### Comparing `iderare-pheno-0.3.5/LICENSE` & `iderare-pheno-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/PKG-INFO` & `iderare-pheno-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.5
+Version: 0.4.0
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -49,14 +49,15 @@
 Requires-Dist: scipy
 Requires-Dist: hpo3
 Requires-Dist: scikit-learn
 Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.5 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.4.0 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -27,29 +27,30 @@
 Audience :: Science/Research Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Medical
 Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist:
 matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn
 Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist:
-black<25.0,>=23.0; extra == "dev" Requires-Dist: black[jupyter]; extra == "dev"
-Requires-Dist: isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra
-== "dev" Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-
-cov; extra == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist:
-build; extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist:
-wheel; extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-
-parser<2.1,>=1.0; extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra
-== "dev" Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-
-Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist:
-packaging; extra == "dev" # [IDeRare-Pheno](https://iderare-
-pheno.readthedocs.io/) IDeRare or "Indonesia Exome Rare Disease Variant
-Discovery Pipeline" is simple and ready to use variant discovery pipeline to
-discover rare disease variants from exome sequencing data.
+Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist: types-PyYAML;
+extra == "dev" Requires-Dist: black<25.0,>=23.0; extra == "dev" Requires-Dist:
+black[jupyter]; extra == "dev" Requires-Dist: isort<5.14,>=5.12; extra == "dev"
+Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-sphinx; extra ==
+"dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: twine>=1.11.0;
+extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist: setuptools;
+extra == "dev" Requires-Dist: wheel; extra == "dev" Requires-Dist:
+Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-Dist: furo==2024.1.29; extra ==
+"dev" Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev" Requires-Dist:
+sphinx-copybutton==0.5.2; extra == "dev" Requires-Dist: sphinx-
+autobuild==2021.3.14; extra == "dev" Requires-Dist: sphinx-autodoc-
+typehints==1.23.3; extra == "dev" Requires-Dist: packaging; extra == "dev" #
+[IDeRare-Pheno](https://iderare-pheno.readthedocs.io/) IDeRare or "Indonesia
+Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use
+variant discovery pipeline to discover rare disease variants from exome
+sequencing data.
              _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
 ## Quick links - [Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI
 Package](https://pypi.org/project/iderare-pheno/) - [License](https://
 github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) - Interactive Webapps
 Implementation of at [Streamlit](https://bioinformatics-
 ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
 script is recommended if you would like to do conversion, linkage analysis,
```

### Comparing `iderare-pheno-0.3.5/README.md` & `iderare-pheno-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/converter.py` & `iderare-pheno-0.4.0/iderare_pheno/converter.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/data/genes_to_phenotype.txt` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/data/genes_to_phenotype.txt`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/data/hp.obo` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/data/hp.obo`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/data/phenotype.hpoa` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/data/phenotype.hpoa`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/icd102omim_subset.tsv` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/icd102omim_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv` & `iderare-pheno-0.4.0/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/simrec.py` & `iderare-pheno-0.4.0/iderare_pheno/simrec.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/templates/template_iderare.yml` & `iderare-pheno-0.4.0/iderare_pheno/templates/template_iderare.yml`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/iderare_pheno/utils.py` & `iderare-pheno-0.4.0/iderare_pheno/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 import os
 from datetime import datetime
 
 import pandas as pd
 import scipy.cluster
+import yaml
 from matplotlib import pyplot as plt
 
+iderare_template = os.path.join(os.path.dirname(__file__), "templates", "template_iderare.yml")
+
+
+# Fill template_iderare.yml with the given phenotype
+def generate_yml(hpo_sets, filename="iderare.yml"):
+    with open(iderare_template, "r") as f:
+        y = yaml.safe_load(f)
+        y["analysis"]["hpo_ids"] = hpo_sets
+
+    with open(filename, "w+") as o:
+        yaml.dump(y, o, default_flow_style=False, sort_keys=False)
+        print("File {} has been created.".format(filename))
+
 
 # Convert data(s) to dataframe
 def list2tsv(
     term_id,
     name,
     sim_score=None,
     filename="{}_result".format(datetime.now().strftime("%Y%m%d_%H%M%S")),
```

### Comparing `iderare-pheno-0.3.5/iderare_pheno.egg-info/PKG-INFO` & `iderare-pheno-0.4.0/iderare_pheno.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.5
+Version: 0.4.0
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -49,14 +49,15 @@
 Requires-Dist: scipy
 Requires-Dist: hpo3
 Requires-Dist: scikit-learn
 Requires-Dist: pyyaml
 Provides-Extra: dev
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: mypy<1.10,>=1.0; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: black<25.0,>=23.0; extra == "dev"
 Requires-Dist: black[jupyter]; extra == "dev"
 Requires-Dist: isort<5.14,>=5.12; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-sphinx; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: twine>=1.11.0; extra == "dev"
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.5 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.4.0 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
@@ -27,29 +27,30 @@
 Audience :: Science/Research Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License Classifier: Programming
 Language :: Python :: 3 Classifier: Topic :: Scientific/Engineering :: Medical
 Science Apps. Requires-Python: >=3.8 Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: pandas Requires-Dist: numpy Requires-Dist:
 matplotlib Requires-Dist: scipy Requires-Dist: hpo3 Requires-Dist: scikit-learn
 Requires-Dist: pyyaml Provides-Extra: dev Requires-Dist: ruff; extra == "dev"
-Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist:
-black<25.0,>=23.0; extra == "dev" Requires-Dist: black[jupyter]; extra == "dev"
-Requires-Dist: isort<5.14,>=5.12; extra == "dev" Requires-Dist: pytest; extra
-== "dev" Requires-Dist: pytest-sphinx; extra == "dev" Requires-Dist: pytest-
-cov; extra == "dev" Requires-Dist: twine>=1.11.0; extra == "dev" Requires-Dist:
-build; extra == "dev" Requires-Dist: setuptools; extra == "dev" Requires-Dist:
-wheel; extra == "dev" Requires-Dist: Sphinx<7.3.0,>=4.3.0; extra == "dev"
-Requires-Dist: furo==2024.1.29; extra == "dev" Requires-Dist: myst-
-parser<2.1,>=1.0; extra == "dev" Requires-Dist: sphinx-copybutton==0.5.2; extra
-== "dev" Requires-Dist: sphinx-autobuild==2021.3.14; extra == "dev" Requires-
-Dist: sphinx-autodoc-typehints==1.23.3; extra == "dev" Requires-Dist:
-packaging; extra == "dev" # [IDeRare-Pheno](https://iderare-
-pheno.readthedocs.io/) IDeRare or "Indonesia Exome Rare Disease Variant
-Discovery Pipeline" is simple and ready to use variant discovery pipeline to
-discover rare disease variants from exome sequencing data.
+Requires-Dist: mypy<1.10,>=1.0; extra == "dev" Requires-Dist: types-PyYAML;
+extra == "dev" Requires-Dist: black<25.0,>=23.0; extra == "dev" Requires-Dist:
+black[jupyter]; extra == "dev" Requires-Dist: isort<5.14,>=5.12; extra == "dev"
+Requires-Dist: pytest; extra == "dev" Requires-Dist: pytest-sphinx; extra ==
+"dev" Requires-Dist: pytest-cov; extra == "dev" Requires-Dist: twine>=1.11.0;
+extra == "dev" Requires-Dist: build; extra == "dev" Requires-Dist: setuptools;
+extra == "dev" Requires-Dist: wheel; extra == "dev" Requires-Dist:
+Sphinx<7.3.0,>=4.3.0; extra == "dev" Requires-Dist: furo==2024.1.29; extra ==
+"dev" Requires-Dist: myst-parser<2.1,>=1.0; extra == "dev" Requires-Dist:
+sphinx-copybutton==0.5.2; extra == "dev" Requires-Dist: sphinx-
+autobuild==2021.3.14; extra == "dev" Requires-Dist: sphinx-autodoc-
+typehints==1.23.3; extra == "dev" Requires-Dist: packaging; extra == "dev" #
+[IDeRare-Pheno](https://iderare-pheno.readthedocs.io/) IDeRare or "Indonesia
+Exome Rare Disease Variant Discovery Pipeline" is simple and ready to use
+variant discovery pipeline to discover rare disease variants from exome
+sequencing data.
              _[_C_I_]_[_P_y_P_I_]_[_D_o_c_u_m_e_n_t_a_t_i_o_n_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_S_t_r_e_a_m_l_i_t_]
 ## Quick links - [Documentation](https://iderare-pheno.readthedocs.io/) - [PyPI
 Package](https://pypi.org/project/iderare-pheno/) - [License](https://
 github.com/ivanwilliammd/iderare-pheno/blob/main/LICENSE) - Interactive Webapps
 Implementation of at [Streamlit](https://bioinformatics-
 ivanwilliamharsono.streamlitapp.com/IDeRare_Pheno) ## What does it do? This
 script is recommended if you would like to do conversion, linkage analysis,
```

### Comparing `iderare-pheno-0.3.5/iderare_pheno.egg-info/SOURCES.txt` & `iderare-pheno-0.4.0/iderare_pheno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.5/pyproject.toml` & `iderare-pheno-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 Changelog = "https://github.com/ivanwilliammd/iderare-pheno/blob/main/CHANGELOG.md"
 Documentation = "https://iderare-pheno.readthedocs.io/"
 
 [project.optional-dependencies]
 dev = [
     "ruff",
     "mypy>=1.0,<1.10",
+    "types-PyYAML",
     "black>=23.0,<25.0",
     "black[jupyter]",
     "isort>=5.12,<5.14",
     "pytest",
     "pytest-sphinx",
     "pytest-cov",
     "twine>=1.11.0",
```

