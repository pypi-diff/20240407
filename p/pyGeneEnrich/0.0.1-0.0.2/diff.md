# Comparing `tmp/pyGeneEnrich-0.0.1.tar.gz` & `tmp/pyGeneEnrich-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyGeneEnrich-0.0.1.tar", last modified: Wed Apr  3 07:04:45 2024, max compression
+gzip compressed data, was "pyGeneEnrich-0.0.2.tar", last modified: Sun Apr  7 07:33:08 2024, max compression
```

## Comparing `pyGeneEnrich-0.0.1.tar` & `pyGeneEnrich-0.0.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 07:04:39.304227 pyGeneEnrich-0.0.1/
-drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 07:04:39.000222 pyGeneEnrich-0.0.1/GeneEnrich/
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.1/GeneEnrich/__init__.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2934 2024-04-03 02:26:27.000000 pyGeneEnrich-0.0.1/GeneEnrich/base_cli.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)      614 2024-04-03 02:26:28.000000 pyGeneEnrich-0.0.1/GeneEnrich/consts.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     7369 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.1/GeneEnrich/enricher.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1585 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.1/GeneEnrich/parse.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2406 2024-04-03 05:14:19.000000 pyGeneEnrich-0.0.1/GeneEnrich/preprocess.py
-drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 07:04:39.074223 pyGeneEnrich-0.0.1/GeneEnrich/run_go/
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:27.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_go/__init__.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2648 2024-04-03 05:51:30.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_go/argparse.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2358 2024-04-03 05:38:26.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_go/cli.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2329 2024-04-03 05:59:56.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_go/enrich_go.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1853 2024-04-03 05:38:26.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_go/go_utilities.py
-drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 07:04:39.129224 pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/__init__.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2656 2024-04-03 06:01:22.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/argparse.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2382 2024-04-03 05:38:26.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/cli.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2059 2024-04-03 06:04:12.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/enrich_kegg.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2269 2024-04-03 05:09:12.000000 pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/kegg_utilities.py
-drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 07:04:39.181225 pyGeneEnrich-0.0.1/GeneEnrich/update_db/
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.1/GeneEnrich/update_db/__init__.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1432 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.1/GeneEnrich/update_db/argparse.py
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1604 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.1/GeneEnrich/update_db/cli.py
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1068 2024-04-03 02:25:23.000000 pyGeneEnrich-0.0.1/LICENSE
--rw-r--r--   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2143 2024-04-03 07:04:39.294226 pyGeneEnrich-0.0.1/PKG-INFO
--rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)      392 2024-04-03 05:45:40.000000 pyGeneEnrich-0.0.1/README.rst
-drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 07:04:39.279226 pyGeneEnrich-0.0.1/pyGeneEnrich.egg-info/
--rw-r--r--   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2143 2024-04-03 07:04:38.000000 pyGeneEnrich-0.0.1/pyGeneEnrich.egg-info/PKG-INFO
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)      759 2024-04-03 07:04:38.000000 pyGeneEnrich-0.0.1/pyGeneEnrich.egg-info/SOURCES.txt
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        1 2024-04-03 07:04:38.000000 pyGeneEnrich-0.0.1/pyGeneEnrich.egg-info/dependency_links.txt
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)       56 2024-04-03 07:04:38.000000 pyGeneEnrich-0.0.1/pyGeneEnrich.egg-info/entry_points.txt
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)       11 2024-04-03 07:04:38.000000 pyGeneEnrich-0.0.1/pyGeneEnrich.egg-info/top_level.txt
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)      784 2024-04-03 07:04:23.000000 pyGeneEnrich-0.0.1/pyproject.toml
--rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)       38 2024-04-03 07:04:39.305227 pyGeneEnrich-0.0.1/setup.cfg
+drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-07 07:32:56.203635 pyGeneEnrich-0.0.2/
+drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-07 07:32:55.514625 pyGeneEnrich-0.0.2/GeneEnrich/
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.2/GeneEnrich/__init__.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2934 2024-04-03 02:26:27.000000 pyGeneEnrich-0.0.2/GeneEnrich/base_cli.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)      614 2024-04-03 02:26:28.000000 pyGeneEnrich-0.0.2/GeneEnrich/consts.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     7369 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.2/GeneEnrich/enricher.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1585 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.2/GeneEnrich/parse.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2406 2024-04-03 05:14:19.000000 pyGeneEnrich-0.0.2/GeneEnrich/preprocess.py
+drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-07 07:32:55.674627 pyGeneEnrich-0.0.2/GeneEnrich/run_go/
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:27.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_go/__init__.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2648 2024-04-03 05:51:30.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_go/argparse.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2358 2024-04-03 05:38:26.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_go/cli.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2329 2024-04-03 05:59:56.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_go/enrich_go.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1853 2024-04-03 05:38:26.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_go/go_utilities.py
+drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-07 07:32:55.864630 pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/__init__.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2656 2024-04-03 06:01:22.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/argparse.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2382 2024-04-03 05:38:26.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/cli.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2059 2024-04-03 06:04:12.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/enrich_kegg.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     2269 2024-04-03 05:09:12.000000 pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/kegg_utilities.py
+drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-07 07:32:55.947631 pyGeneEnrich-0.0.2/GeneEnrich/update_db/
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.2/GeneEnrich/update_db/__init__.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1432 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.2/GeneEnrich/update_db/argparse.py
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1604 2024-04-03 02:26:29.000000 pyGeneEnrich-0.0.2/GeneEnrich/update_db/cli.py
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     1068 2024-04-03 02:25:23.000000 pyGeneEnrich-0.0.2/LICENSE
+-rw-r--r--   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     5006 2024-04-07 07:32:56.195635 pyGeneEnrich-0.0.2/PKG-INFO
+-rwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     3251 2024-04-03 08:25:37.000000 pyGeneEnrich-0.0.2/README.md
+drwxr-x--x   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        0 2024-04-07 07:32:56.180635 pyGeneEnrich-0.0.2/pyGeneEnrich.egg-info/
+-rw-r--r--   0 huangwanxiang (642201479) ssh.bioinfo (642201430)     5006 2024-04-07 07:32:55.000000 pyGeneEnrich-0.0.2/pyGeneEnrich.egg-info/PKG-INFO
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)      758 2024-04-07 07:32:55.000000 pyGeneEnrich-0.0.2/pyGeneEnrich.egg-info/SOURCES.txt
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)        1 2024-04-07 07:32:55.000000 pyGeneEnrich-0.0.2/pyGeneEnrich.egg-info/dependency_links.txt
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)       56 2024-04-07 07:32:55.000000 pyGeneEnrich-0.0.2/pyGeneEnrich.egg-info/entry_points.txt
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)       11 2024-04-07 07:32:55.000000 pyGeneEnrich-0.0.2/pyGeneEnrich.egg-info/top_level.txt
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)      783 2024-04-07 07:30:55.000000 pyGeneEnrich-0.0.2/pyproject.toml
+-rw-r-----   0 huangwanxiang (642201479) ssh.bioinfo (642201430)       38 2024-04-07 07:32:56.203635 pyGeneEnrich-0.0.2/setup.cfg
```

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/base_cli.py` & `pyGeneEnrich-0.0.2/GeneEnrich/base_cli.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/consts.py` & `pyGeneEnrich-0.0.2/GeneEnrich/consts.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/enricher.py` & `pyGeneEnrich-0.0.2/GeneEnrich/enricher.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/parse.py` & `pyGeneEnrich-0.0.2/GeneEnrich/parse.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/preprocess.py` & `pyGeneEnrich-0.0.2/GeneEnrich/preprocess.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_go/argparse.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_go/argparse.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_go/cli.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_go/cli.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_go/enrich_go.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_go/enrich_go.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_go/go_utilities.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_go/go_utilities.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/argparse.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/argparse.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/cli.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/cli.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/enrich_kegg.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/enrich_kegg.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/run_kegg/kegg_utilities.py` & `pyGeneEnrich-0.0.2/GeneEnrich/run_kegg/kegg_utilities.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/update_db/argparse.py` & `pyGeneEnrich-0.0.2/GeneEnrich/update_db/argparse.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/GeneEnrich/update_db/cli.py` & `pyGeneEnrich-0.0.2/GeneEnrich/update_db/cli.py`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/LICENSE` & `pyGeneEnrich-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyGeneEnrich-0.0.1/pyGeneEnrich.egg-info/SOURCES.txt` & `pyGeneEnrich-0.0.2/pyGeneEnrich.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 LICENSE
-README.rst
+README.md
 pyproject.toml
 GeneEnrich/__init__.py
 GeneEnrich/base_cli.py
 GeneEnrich/consts.py
 GeneEnrich/enricher.py
 GeneEnrich/parse.py
 GeneEnrich/preprocess.py
```

### Comparing `pyGeneEnrich-0.0.1/pyproject.toml` & `pyGeneEnrich-0.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyGeneEnrich"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="WhiteRabBio" },
 ]
 license = {file = "LICENSE"}
 description = "A limited python implementation of clusterProfiler from R"
-readme = "README.rst"
+readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "License :: OSI Approved :: MIT License"
 ]
```

