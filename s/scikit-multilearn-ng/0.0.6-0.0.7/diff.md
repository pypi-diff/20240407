# Comparing `tmp/scikit-multilearn-ng-0.0.6.tar.gz` & `tmp/scikit-multilearn-ng-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/scikit-multilearn-ng/scikit-multilearn-ng/dist/.tmp-f0tpy74s/scikit-multilearn-ng-0.0.6.tar", last modified: Sun Jan 21 20:19:20 2024, max compression
+gzip compressed data, was "/home/runner/work/scikit-multilearn-ng/scikit-multilearn-ng/dist/.tmp-8dehs70n/scikit-multilearn-ng-0.0.7.tar", last modified: Sun Apr  7 14:14:14 2024, max compression
```

## Comparing `scikit-multilearn-ng-0.0.6.tar` & `scikit-multilearn-ng-0.0.7.tar`

### file list

```diff
@@ -1,75 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/adapt/
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/adapt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/adapt/brknn.py
--rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/adapt/mlaram.py
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/adapt/mlknn.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/adapt/mltsvm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/base/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/base/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/base/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/base/problem_transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/balancedkmeans.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/graphtool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/igraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/networkx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/cluster/random.py
--rw-r--r--   0 runner    (1001) docker     (127)    13836 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/_mdsw.py
--rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/clems.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/openne.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/skembeddings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/embedding/unit_tests/test_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/rakeld.py
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/rakelo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/voting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ext/
--rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ext/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)    16019 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/ext/meka.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/missing/
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/missing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/missing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/missing/smile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/model_selection/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/model_selection/iterative_stratification.py
--rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/model_selection/measures.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 20:19:20.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8314 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/br.py
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/chf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/gsc.py
--rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/iblr.py
--rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/lp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-01-21 20:19:09.000000 scikit-multilearn-ng-0.0.6/skmultilearn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2264 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/adapt/
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/adapt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6806 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/adapt/brknn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12050 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/adapt/mlaram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/adapt/mlknn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/adapt/mltsvm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/base/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/base/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/base/problem_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/balancedkmeans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/graphtool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8924 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/igraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6801 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/networkx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/cluster/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/_mdsw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6732 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/clems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/openne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/skembeddings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/embedding/unit_tests/test_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5267 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/rakeld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/rakelo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/voting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     1666 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ext/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15758 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/ext/meka.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/missing/
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/missing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7179 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/missing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/missing/smile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17090 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/model_selection/iterative_stratification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9336 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/model_selection/measures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/
+-rw-r--r--   0 runner    (1001) docker     (127)     5342 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/br.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8646 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/chf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/gsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12121 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/iblr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9239 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/lp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/pcc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:14:14.000000 scikit-multilearn-ng-0.0.7/skmultilearn/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11778 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/tree/pct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-07 14:14:07.000000 scikit-multilearn-ng-0.0.7/skmultilearn/utils.py
```

### Comparing `scikit-multilearn-ng-0.0.6/LICENSE` & `scikit-multilearn-ng-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/PKG-INFO` & `scikit-multilearn-ng-0.0.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-multilearn-ng
-Version: 0.0.6
+Version: 0.0.7
 Summary: Scikit-multilearn-ng is the follow up to scikit-multilearn, a BSD-licensed library for multi-label classification that is built on top of the well-known scikit-learn ecosystem.
 Home-page: https://github.com/scikit-multilearn-ng/scikit-multilearn-ng/
 Author: Piotr Szymański
 Author-email: niedakh@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,33 +20,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 Provides-Extra: gpl
 Provides-Extra: dev
 Provides-Extra: keras
-Provides-Extra: meka
 Provides-Extra: test
 License-File: LICENSE
 
 # scikit-multilearn-ng
 
 [![PyPI version](https://badge.fury.io/py/scikit-multilearn-ng.svg)](https://badge.fury.io/py/scikit-multilearn-ng)
 [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
 __scikit-multilearn-ng__ is a Python module capable of performing multi-label
 learning tasks and is the follow-up to [scikit-multilearn](https://github.com/scikit-multilearn/scikit-multilearn).
 It is built on-top of various scientific Python packages
 ([numpy](http://www.numpy.org/), [scipy](https://www.scipy.org/)) and
 follows a similar API to that of [scikit-learn](http://scikit-learn.org/).
 
-More documentation (until replaced by scikit-multilearn-ng specific ones):
+More documentation:
 
-- __Website:__ [scikit.ml](http://scikit.ml)
-- __Documentation:__ [scikit-multilearn Documentation](http://scikit.ml/api/skmultilearn.html)
+- __Website:__ [https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/](https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/)
 
 
 ## Features
 
 - __Native Python implementation.__ A native Python implementation for a variety of multi-label classification algorithms. To see the list of all supported classifiers, check this [link](http://scikit.ml/#classifiers).
 
 - __Interface to Meka.__ A Meka wrapper class is implemented for reference purposes and integration. This provides access to all methods available in MEKA, MULAN, and WEKA &mdash; the reference standard in the field.
@@ -110,16 +108,15 @@
 classifier.fit(X_train, y_train)
 
 # Predict
 y_pred = classifier.predict(X_test)
 ```
 
 More examples and use-cases can be seen in the 
-[documentation](http://scikit.ml/api/classify.html). For using the MEKA
-wrapper, check this [link](http://scikit.ml/api/meka.html#mekawrapper).
+[documentation](https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/_static/example_usage.html).
 
 ## Contributing
 
 This project is open for contributions. Here are some of the ways for
 you to contribute:
 
 - Bug reports/fix
```

### Comparing `scikit-multilearn-ng-0.0.6/README.md` & `scikit-multilearn-ng-0.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 
 __scikit-multilearn-ng__ is a Python module capable of performing multi-label
 learning tasks and is the follow-up to [scikit-multilearn](https://github.com/scikit-multilearn/scikit-multilearn).
 It is built on-top of various scientific Python packages
 ([numpy](http://www.numpy.org/), [scipy](https://www.scipy.org/)) and
 follows a similar API to that of [scikit-learn](http://scikit-learn.org/).
 
-More documentation (until replaced by scikit-multilearn-ng specific ones):
+More documentation:
 
-- __Website:__ [scikit.ml](http://scikit.ml)
-- __Documentation:__ [scikit-multilearn Documentation](http://scikit.ml/api/skmultilearn.html)
+- __Website:__ [https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/](https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/)
 
 
 ## Features
 
 - __Native Python implementation.__ A native Python implementation for a variety of multi-label classification algorithms. To see the list of all supported classifiers, check this [link](http://scikit.ml/#classifiers).
 
 - __Interface to Meka.__ A Meka wrapper class is implemented for reference purposes and integration. This provides access to all methods available in MEKA, MULAN, and WEKA &mdash; the reference standard in the field.
@@ -80,16 +79,15 @@
 classifier.fit(X_train, y_train)
 
 # Predict
 y_pred = classifier.predict(X_test)
 ```
 
 More examples and use-cases can be seen in the 
-[documentation](http://scikit.ml/api/classify.html). For using the MEKA
-wrapper, check this [link](http://scikit.ml/api/meka.html#mekawrapper).
+[documentation](https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/_static/example_usage.html).
 
 ## Contributing
 
 This project is open for contributions. Here are some of the ways for
 you to contribute:
 
 - Bug reports/fix
```

### Comparing `scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/PKG-INFO` & `scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-multilearn-ng
-Version: 0.0.6
+Version: 0.0.7
 Summary: Scikit-multilearn-ng is the follow up to scikit-multilearn, a BSD-licensed library for multi-label classification that is built on top of the well-known scikit-learn ecosystem.
 Home-page: https://github.com/scikit-multilearn-ng/scikit-multilearn-ng/
 Author: Piotr Szymański
 Author-email: niedakh@gmail.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -20,33 +20,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Description-Content-Type: text/markdown
 Provides-Extra: gpl
 Provides-Extra: dev
 Provides-Extra: keras
-Provides-Extra: meka
 Provides-Extra: test
 License-File: LICENSE
 
 # scikit-multilearn-ng
 
 [![PyPI version](https://badge.fury.io/py/scikit-multilearn-ng.svg)](https://badge.fury.io/py/scikit-multilearn-ng)
 [![License](https://img.shields.io/badge/License-BSD%202--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause)
 
 __scikit-multilearn-ng__ is a Python module capable of performing multi-label
 learning tasks and is the follow-up to [scikit-multilearn](https://github.com/scikit-multilearn/scikit-multilearn).
 It is built on-top of various scientific Python packages
 ([numpy](http://www.numpy.org/), [scipy](https://www.scipy.org/)) and
 follows a similar API to that of [scikit-learn](http://scikit-learn.org/).
 
-More documentation (until replaced by scikit-multilearn-ng specific ones):
+More documentation:
 
-- __Website:__ [scikit.ml](http://scikit.ml)
-- __Documentation:__ [scikit-multilearn Documentation](http://scikit.ml/api/skmultilearn.html)
+- __Website:__ [https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/](https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/)
 
 
 ## Features
 
 - __Native Python implementation.__ A native Python implementation for a variety of multi-label classification algorithms. To see the list of all supported classifiers, check this [link](http://scikit.ml/#classifiers).
 
 - __Interface to Meka.__ A Meka wrapper class is implemented for reference purposes and integration. This provides access to all methods available in MEKA, MULAN, and WEKA &mdash; the reference standard in the field.
@@ -110,16 +108,15 @@
 classifier.fit(X_train, y_train)
 
 # Predict
 y_pred = classifier.predict(X_test)
 ```
 
 More examples and use-cases can be seen in the 
-[documentation](http://scikit.ml/api/classify.html). For using the MEKA
-wrapper, check this [link](http://scikit.ml/api/meka.html#mekawrapper).
+[documentation](https://scikit-multilearn-ng.github.io/scikit-multilearn-ng/_static/example_usage.html).
 
 ## Contributing
 
 This project is open for contributions. Here are some of the ways for
 you to contribute:
 
 - Bug reports/fix
```

### Comparing `scikit-multilearn-ng-0.0.6/scikit_multilearn_ng.egg-info/SOURCES.txt` & `scikit-multilearn-ng-0.0.7/scikit_multilearn_ng.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -54,8 +54,11 @@
 skmultilearn/model_selection/measures.py
 skmultilearn/problem_transform/__init__.py
 skmultilearn/problem_transform/br.py
 skmultilearn/problem_transform/cc.py
 skmultilearn/problem_transform/chf.py
 skmultilearn/problem_transform/gsc.py
 skmultilearn/problem_transform/iblr.py
-skmultilearn/problem_transform/lp.py
+skmultilearn/problem_transform/lp.py
+skmultilearn/problem_transform/pcc.py
+skmultilearn/tree/__init__.py
+skmultilearn/tree/pct.py
```

### Comparing `scikit-multilearn-ng-0.0.6/setup.py` & `scikit-multilearn-ng-0.0.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     import io
 
     with io.open("README.md", "r", encoding="utf-8") as f:
         readme = f.read()
 
 setup(
     name="scikit-multilearn-ng",
-    version="v0.0.6",
+    version="v0.0.7",
     packages=find_packages(exclude=["docs", "tests", "*.tests"]),
     install_requires=[
         "scipy>=1.1.0",
         "numpy>=1.15.1",
         "liac-arff>=2.2.1",
         "networkx>=2.1",
         "python-louvain>=0.11",
@@ -41,17 +41,14 @@
             "ipython",
             "ipython-genutils",
         ],
         "keras": [
             "keras<=2.12.0",
             "tensorflow",
         ],
-        "meka": [
-            "whichcraft>=0.4.1",
-        ],
         "test": [
             "pytest",
             "pyhamcrest",
         ],
     },
     author="Piotr Szymański",
     author_email="niedakh@gmail.com",
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/adapt/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/adapt/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/adapt/brknn.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/adapt/brknn.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/adapt/mlaram.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/adapt/mlaram.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/adapt/mlknn.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/adapt/mlknn.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/adapt/mltsvm.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/adapt/mltsvm.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/base/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/base/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/base/base.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/base/base.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/base/problem_transformation.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/base/problem_transformation.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/balancedkmeans.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/balancedkmeans.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/base.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/base.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/fixed.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/fixed.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/graphtool.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/graphtool.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/helpers.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/helpers.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/igraph.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/igraph.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/matrix.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/matrix.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/networkx.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/networkx.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/cluster/random.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/cluster/random.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/dataset.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,17 +200,17 @@
 ):
     """Method for loading ARFF files as numpy array
 
     Parameters
     ----------
     filename : str
         path to ARFF file
-    labelcount: integer
+    label_count: integer
         number of labels in the ARFF file
-    endian: str {"big", "little"} (default is "big")
+    label_location: str {"start", "end"} (default is "end")
         whether the ARFF file contains labels at the beginning of the
         attributes list ("start", MEKA format)
         or at the end ("end", MULAN format)
     input_feature_type: numpy.type as string (default is "float")
         the desire type of the contents of the return 'X' array-likes,
         default 'i8', should be a numpy type,
         see http://docs.scipy.org/doc/numpy/user/basics.types.html
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/embedding/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/embedding/_mdsw.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/embedding/_mdsw.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/embedding/classifier.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/embedding/classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/embedding/clems.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/embedding/clems.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/embedding/openne.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/embedding/openne.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/embedding/skembeddings.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/embedding/skembeddings.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/embedding/unit_tests/test_classifier.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/embedding/unit_tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,10 +28,9 @@
 from .partition import LabelSpacePartitioningClassifier
 from .voting import MajorityVotingClassifier
 
 __all__ = [
     "RakelD",
     "RakelO",
     "LabelSpacePartitioningClassifier",
-    "LabelSpacePartitioningClassifier",
     "MajorityVotingClassifier",
 ]
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/partition.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/partition.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/rakeld.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/rakeld.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/rakelo.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/rakelo.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ensemble/voting.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ensemble/voting.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ext/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ext/keras.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ext/keras.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/ext/meka.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/ext/meka.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,22 +166,15 @@
         java_command=None,
         meka_classpath=None,
     ):
         super(Meka, self).__init__()
 
         self.java_command = java_command
         if self.java_command is None:
-            # TODO: this will not be needed once we're python 3 ready - we will
-            # use it only in python 2.7 cases
-            from whichcraft import which
-
-            self.java_command = which("java")
-
-            if self.java_command is None:
-                raise ValueError("Java not found")
+            raise ValueError("Java not found")
 
         self.meka_classpath = meka_classpath
         if self.meka_classpath is None:
             self.meka_classpath = os.environ.get("MEKA_CLASSPATH")
 
             if self.meka_classpath is None:
                 raise ValueError("No meka classpath defined")
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/missing/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/missing/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/missing/functions.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/missing/functions.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/missing/smile.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/missing/smile.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/model_selection/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/model_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/model_selection/iterative_stratification.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/model_selection/iterative_stratification.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,25 +72,33 @@
 from sklearn.model_selection._split import _BaseKFold
 import numpy as np
 import scipy.sparse as sp
 import itertools
 from sklearn.utils import check_random_state
 
 
-def iterative_train_test_split(X, y, test_size, random_state=None, shuffle=False):
+def iterative_train_test_split(
+    X: np.ndarray,
+    y: np.ndarray,
+    test_size: float,
+    random_state=None,
+    shuffle: bool = False,
+):
     """Iteratively stratified train/test split
 
     Parameters
     ----------
+    X : np.ndarray
+        input features
+    y : np.ndarray
+        input labels
     test_size : float, [0,1]
         the proportion of the dataset to include in the test split, the rest will be put in the train set
-
     random_state : None | int | np.random.RandomState
         the random state seed (optional)
-
     shuffle : bool
         Whether to shuffle the data before splitting into batches. Note that the samples within each split
         will not be shuffled.
 
     Returns
     -------
     X_train, y_train, X_test, y_test
@@ -103,16 +111,16 @@
         sample_distribution_per_fold=[test_size, 1.0 - test_size],
         shuffle=shuffle,
         random_state=random_state,
     )
 
     train_indexes, test_indexes = next(stratifier.split(X, y))
 
-    X_train, y_train = X.loc[train_indexes], y.loc[train_indexes]
-    X_test, y_test = X.loc[test_indexes], y.loc[test_indexes]
+    X_train, y_train = X[train_indexes, :], y[train_indexes, :]
+    X_test, y_test = X[test_indexes, :], y[test_indexes, :]
 
     return X_train, X_test, y_train, y_test
 
 
 def _fold_tie_break(desired_samples_per_fold, M, random_state=check_random_state(None)):
     """Helper function to split a tie between folds with same desirability of a given sample
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/model_selection/measures.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/model_selection/measures.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/__init__.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 +=============================================================================+================================================+
 | :class:`~skmultilearn.problem_transform.BinaryRelevance`                    |  treats each label as a separate single-class  |
 |                                                                             |  classification problem                        |
 +-----------------------------------------------------------------------------+------------------------------------------------+
 | :class:`~skmultilearn.problem_transform.ClassifierChain`                    |  treats each label as a part of a conditioned  |
 |                                                                             |  chain of single-class classification problems |
 +-----------------------------------------------------------------------------+------------------------------------------------+
+| :class:`~skmultilearn.problem_transform.ProbabilisticClassifierChain`       |  extends Classifier Chains by modeling joint   |
+|                                                                             |  label distributions and estimating the        |
+|                                                                             |  probability of label sets. It trains a series |
+|                                                                             |  of classifiers, each predicting the           |
+|                                                                             |  probability of a label, conditioned on the    |
+|                                                                             |  input features and preceding label predictions|
++-----------------------------------------------------------------------------+------------------------------------------------+
 | :class:`~skmultilearn.problem_transform.ClassificationHeterogeneousFeature` | augments the feature set                       |
 |                                                                             | with extra features derived from label         |
 |                                                                             | probabilities and resolves cyclic dependencies |
 |                                                                             | between features and labels iteratively        |
 +-----------------------------------------------------------------------------+------------------------------------------------+
 | :class:`~skmultilearn.problem_transform.LabelPowerset`                      | treats each label combination as a separate    |
 |                                                                             | class with one multi-class classification      |
@@ -30,25 +37,28 @@
 |                                                                             | followed by Logistic Regression classifiers.   |
 +-----------------------------------------------------------------------------+------------------------------------------------+
 | :class:`~skmultilearn.problem_transform.StructuredGridSearchCV`             | performs hyperparameter tuning for each label  |
 |                                                                             | classifier, considering BR&CC structural       |
 |                                                                             | properties. It searches for optimal classifiers|
 |                                                                             | with fine-tuned parameters for each label.     |
 +-----------------------------------------------------------------------------+------------------------------------------------+
+
 """
 
 from .br import BinaryRelevance
 from .cc import ClassifierChain
+from .pcc import ProbabilisticClassifierChain
 from .chf import ClassificationHeterogeneousFeature
 from .gsc import StructuredGridSearchCV
 from .lp import LabelPowerset
 from .iblr import InstanceBasedLogisticRegression
 
 
 __all__ = [
     "BinaryRelevance",
     "ClassifierChain",
+    "ProbabilisticClassifierChain",
     "ClassificationHeterogeneousFeature",
     "LabelPowerset",
     "InstanceBasedLogisticRegression",
     "StructuredGridSearchCV",
 ]
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/br.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/br.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         This is one of the most basic approaches to multi-label classification, it ignores relationships between labels.
 
     Examples
     --------
     An example use case for Binary Relevance classification
     with an :class:`sklearn.svm.SVC` base classifier which supports sparse input:
 
-
     .. code-block:: python
 
         from skmultilearn.problem_transform import BinaryRelevance
         from sklearn.svm import SVC
 
         # initialize Binary Relevance multi-label classifier
         # with an SVM classifier
@@ -86,15 +85,14 @@
             },
             {
                 'classifier': [SVC()],
                 'classifier__kernel': ['rbf', 'linear'],
             },
         ]
 
-
         clf = GridSearchCV(BinaryRelevance(), parameters, scoring='accuracy')
         clf.fit(x, y)
 
         print (clf.best_params_, clf.best_score_)
 
         # result:
         #
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/cc.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/cc.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,22 +27,19 @@
         whether the base classifier requires dense representations
         for input features and classes/labels matrices in fit/predict.
         If value not provided, sparse representations are used if base classifier is
         an instance of :class:`~skmultilearn.base.MLClassifierBase` and dense otherwise.
     order : List[int], permutation of ``range(n_labels)``, optional
         the order in which the chain should go through labels, the default is ``range(n_labels)``
 
-
     Attributes
     ----------
     classifiers_ : List[:class:`~sklearn.base.BaseEstimator`] of shape `n_labels`
         list of classifiers trained per partition, set in :meth:`fit`
 
-
-
     References
     ----------
     If used, please cite the scikit-multilearn library and the relevant paper:
 
     .. code-block:: bibtex
 
         @inproceedings{read2009classifier,
@@ -114,15 +111,15 @@
     """
 
     def __init__(self, classifier=None, require_dense=None, order=None):
         super(ClassifierChain, self).__init__(classifier, require_dense)
         self.order = order
         self.copyable_attrs = ["classifier", "require_dense", "order"]
 
-    def fit(self, X, y, order=None):
+    def fit(self, X, y):
         """Fits classifier to training data
 
         Parameters
         ----------
         X : `array_like`, :class:`numpy.matrix` or :mod:`scipy.sparse` matrix, shape=(n_samples, n_features)
             input feature matrix
         y : `array_like`, :class:`numpy.matrix` or :mod:`scipy.sparse` matrix of `{0, 1}`, shape=(n_samples, n_labels)
```

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/chf.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/chf.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/gsc.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/gsc.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/iblr.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/iblr.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/problem_transform/lp.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/problem_transform/lp.py`

 * *Files identical despite different names*

### Comparing `scikit-multilearn-ng-0.0.6/skmultilearn/utils.py` & `scikit-multilearn-ng-0.0.7/skmultilearn/utils.py`

 * *Files identical despite different names*

