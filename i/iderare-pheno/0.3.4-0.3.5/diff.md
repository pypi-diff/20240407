# Comparing `tmp/iderare-pheno-0.3.4.tar.gz` & `tmp/iderare-pheno-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iderare-pheno-0.3.4.tar", last modified: Sat Apr  6 18:34:39 2024, max compression
+gzip compressed data, was "iderare-pheno-0.3.5.tar", last modified: Sat Apr  6 19:01:19 2024, max compression
```

## Comparing `iderare-pheno-0.3.4.tar` & `iderare-pheno-0.3.5.tar`

### file list

```diff
@@ -1,19 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:34:39.097136 iderare-pheno-0.3.4/iderare_pheno/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/iderare_pheno/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-06 18:33:48.000000 iderare-pheno-0.3.4/iderare_pheno/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/simrec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/iderare_pheno/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/iderare_pheno.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-06 18:34:39.000000 iderare-pheno-0.3.4/iderare_pheno.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-06 18:33:49.000000 iderare-pheno-0.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:34:39.101136 iderare-pheno-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.224584 iderare-pheno-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 19:01:19.224584 iderare-pheno-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.128584 iderare-pheno-0.3.5/iderare_pheno/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.128584 iderare-pheno-0.3.5/iderare_pheno/phenotype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.164584 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/
+-rw-r--r--   0 runner    (1001) docker     (127) 19051578 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/genes_to_phenotype.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  9995624 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/hp.obo
+-rw-r--r--   0 runner    (1001) docker     (127) 31896677 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/data/phenotype.hpoa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.220584 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/
+-rw-r--r--   0 runner    (1001) docker     (127)   196778 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/icd102omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   224561 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/loinc2hpo_standardized.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  6033462 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/omim2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  7205315 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/orpha2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   218406 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/orpha2omim_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)   232073 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/snomed2hpo_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)  1298790 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/phenotype/subset/snomed2orpha_subset.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/simrec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.220584 iderare-pheno-0.3.5/iderare_pheno/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/templates/template_iderare.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/iderare_pheno/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:01:19.220584 iderare-pheno-0.3.5/iderare_pheno.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-06 19:01:19.000000 iderare-pheno-0.3.5/iderare_pheno.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-04-06 19:00:28.000000 iderare-pheno-0.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:01:19.224584 iderare-pheno-0.3.5/setup.cfg
```

### Comparing `iderare-pheno-0.3.4/LICENSE` & `iderare-pheno-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.4/PKG-INFO` & `iderare-pheno-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.4
+Version: 0.3.5
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.4 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.5 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

### Comparing `iderare-pheno-0.3.4/README.md` & `iderare-pheno-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.4/iderare_pheno/converter.py` & `iderare-pheno-0.3.5/iderare_pheno/converter.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.4/iderare_pheno/simrec.py` & `iderare-pheno-0.3.5/iderare_pheno/simrec.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.4/iderare_pheno/utils.py` & `iderare-pheno-0.3.5/iderare_pheno/utils.py`

 * *Files identical despite different names*

### Comparing `iderare-pheno-0.3.4/iderare_pheno.egg-info/PKG-INFO` & `iderare-pheno-0.3.5/iderare_pheno.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iderare-pheno
-Version: 0.3.4
+Version: 0.3.5
 Author-email: Ivan William Harsono <ivanwilliam.md@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Ivan William Harsono
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.4 Author-email: Ivan
+Metadata-Version: 2.1 Name: iderare-pheno Version: 0.3.5 Author-email: Ivan
 William Harsono
 gmail.com> License: BSD 3-Clause License Copyright (c) 2024, Ivan William
 Harsono Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met: 1.
 Redistributions of source code must retain the above copyright notice, this
 list of conditions and the following disclaimer. 2. Redistributions in binary
 form must reproduce the above copyright notice, this list of conditions and the
```

