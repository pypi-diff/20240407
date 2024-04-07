# Comparing `tmp/libauc-1.3.2.tar.gz` & `tmp/libauc-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libauc-1.3.2.tar", last modified: Fri Mar  8 21:57:49 2024, max compression
+gzip compressed data, was "libauc-1.3.3.tar", last modified: Sun Apr  7 16:42:23 2024, max compression
```

## Comparing `libauc-1.3.2.tar` & `libauc-1.3.3.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.866291 libauc-1.3.2/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1063 2024-02-12 01:45:23.000000 libauc-1.3.2/LICENSE
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4083 2024-03-08 21:57:49.866291 libauc-1.3.2/PKG-INFO
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     3626 2024-02-12 01:47:04.000000 libauc-1.3.2/README.md
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.853291 libauc-1.3.2/libauc/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)       22 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/__init__.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.858291 libauc-1.3.2/libauc/datasets/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)      245 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/__init__.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2621 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/breastcancer.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2176 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/cat_vs_dog.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     9859 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/chexpert.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     6292 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/cifar.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1561 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/dataset.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12399 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/folder.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4854 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/melanoma.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13133 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/movielens.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1497 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/musk2.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2960 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/datasets/stl10.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.860291 libauc-1.3.2/libauc/losses/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)      117 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/__init__.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    49585 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/auc.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    23695 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/contrastive.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2893 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/losses.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    15077 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/mil.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     3038 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/perf_at_top.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12996 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/ranking.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2618 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/losses/surrogate.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.860291 libauc-1.3.2/libauc/metrics/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)       23 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/metrics/__init__.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8416 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/metrics/metrics.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.862291 libauc-1.3.2/libauc/models/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)      153 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/models/__init__.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13913 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/models/densenet.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8626 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/models/mil_models.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     3479 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/models/neumf.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1284 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/models/perceptron.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    16352 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/models/resnet.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     6836 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/models/resnet_cifar.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.865291 libauc-1.3.2/libauc/optimizers/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)      350 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/__init__.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     9062 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/adam.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8911 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/adamw.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12775 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/isogclr.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1760 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/lars.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8217 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/midam.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    11591 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/pdsca.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    14772 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/pesg.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8297 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/sgd.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13546 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/soap.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    11777 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/sogclr.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12722 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/song.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13216 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/sopa.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13344 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/sopa_s.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13081 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/optimizers/sota_s.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.865291 libauc-1.3.2/libauc/sampler/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)       23 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/sampler/__init__.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    20482 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/sampler/sampler.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.866291 libauc-1.3.2/libauc/utils/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)       50 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/utils/__init__.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)    19616 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/utils/paper_utils.py
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4706 2024-03-08 21:48:08.000000 libauc-1.3.2/libauc/utils/utils.py
-drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-03-08 21:57:49.854291 libauc-1.3.2/libauc.egg-info/
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4083 2024-03-08 21:57:49.000000 libauc-1.3.2/libauc.egg-info/PKG-INFO
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1470 2024-03-08 21:57:49.000000 libauc-1.3.2/libauc.egg-info/SOURCES.txt
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)        1 2024-03-08 21:57:49.000000 libauc-1.3.2/libauc.egg-info/dependency_links.txt
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)       76 2024-03-08 21:57:49.000000 libauc-1.3.2/libauc.egg-info/requires.txt
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)        7 2024-03-08 21:57:49.000000 libauc-1.3.2/libauc.egg-info/top_level.txt
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)       38 2024-03-08 21:57:49.866291 libauc-1.3.2/setup.cfg
--rw-r--r--   0 siqi     (634004935) siqi     (634004935)      953 2024-03-08 21:45:02.000000 libauc-1.3.2/setup.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.692857 libauc-1.3.3/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1063 2024-04-07 16:33:49.000000 libauc-1.3.3/LICENSE
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4083 2024-04-07 16:42:23.692857 libauc-1.3.3/PKG-INFO
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     3626 2024-04-07 16:33:49.000000 libauc-1.3.3/README.md
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.682857 libauc-1.3.3/libauc/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)       22 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/__init__.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.685857 libauc-1.3.3/libauc/datasets/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)      245 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/__init__.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2621 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/breastcancer.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2176 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/cat_vs_dog.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     9859 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/chexpert.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     6498 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/cifar.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1561 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/dataset.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12888 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/folder.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4854 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/melanoma.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13133 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/movielens.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1497 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/musk2.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2960 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/datasets/stl10.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.687857 libauc-1.3.3/libauc/losses/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)      117 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/__init__.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    49585 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/auc.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    23695 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/contrastive.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2893 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/losses.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    15077 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/mil.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     3038 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/perf_at_top.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12996 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/ranking.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     2618 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/losses/surrogate.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.687857 libauc-1.3.3/libauc/metrics/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)       23 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/metrics/__init__.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8416 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/metrics/metrics.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.688857 libauc-1.3.3/libauc/models/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)      153 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/models/__init__.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13913 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/models/densenet.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8626 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/models/mil_models.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     3479 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/models/neumf.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1284 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/models/perceptron.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    16352 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/models/resnet.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     6836 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/models/resnet_cifar.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.691857 libauc-1.3.3/libauc/optimizers/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)      350 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/__init__.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     9062 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/adam.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8911 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/adamw.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12775 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/isogclr.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1760 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/lars.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8217 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/midam.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    11591 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/pdsca.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    14772 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/pesg.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     8297 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/sgd.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13546 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/soap.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    11777 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/sogclr.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    12722 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/song.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13216 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/sopa.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13344 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/sopa_s.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    13081 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/optimizers/sota_s.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.691857 libauc-1.3.3/libauc/sampler/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)       23 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/sampler/__init__.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    20482 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/sampler/sampler.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.692857 libauc-1.3.3/libauc/utils/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)       50 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/utils/__init__.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)    19616 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/utils/paper_utils.py
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4706 2024-04-07 16:36:14.000000 libauc-1.3.3/libauc/utils/utils.py
+drwxr-xr-x   0 siqi     (634004935) siqi     (634004935)        0 2024-04-07 16:42:23.683857 libauc-1.3.3/libauc.egg-info/
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     4083 2024-04-07 16:42:23.000000 libauc-1.3.3/libauc.egg-info/PKG-INFO
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)     1480 2024-04-07 16:42:23.000000 libauc-1.3.3/libauc.egg-info/SOURCES.txt
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)        1 2024-04-07 16:42:23.000000 libauc-1.3.3/libauc.egg-info/dependency_links.txt
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)       76 2024-04-07 16:42:23.000000 libauc-1.3.3/libauc.egg-info/requires.txt
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)        7 2024-04-07 16:42:23.000000 libauc-1.3.3/libauc.egg-info/top_level.txt
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)       38 2024-04-07 16:42:23.692857 libauc-1.3.3/setup.cfg
+-rw-r--r--   0 siqi     (634004935) siqi     (634004935)      953 2024-04-07 16:42:05.000000 libauc-1.3.3/setup.py
```

### Comparing `libauc-1.3.2/LICENSE` & `libauc-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/PKG-INFO` & `libauc-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.2
+Version: 1.3.3
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.2 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.3 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE LibAUC: A Deep Learning for X-Risk Optimization ---
 _[_P_y_p_i_]_[_D_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_]_[_P_y_T_o_r_c_h_]_[_L_I_C_E_N_S_E_]
```

### Comparing `libauc-1.3.2/README.md` & `libauc-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/breastcancer.py` & `libauc-1.3.3/libauc/datasets/breastcancer.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/cat_vs_dog.py` & `libauc-1.3.3/libauc/datasets/cat_vs_dog.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/chexpert.py` & `libauc-1.3.3/libauc/datasets/chexpert.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/cifar.py` & `libauc-1.3.3/libauc/datasets/cifar.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
         transform (callable, optional): A function/transform that takes in an PIL image
             and returns a transformed version. E.g, ``transforms.RandomCrop``
         target_transform (callable, optional): A function/transform that takes in the
             target and transforms it.
         download (bool, optional): If true, downloads the dataset from the internet and
             puts it in root directory. If dataset is already downloaded, it is not
             downloaded again.
+        return_index (bool, optional): returns a tuple containing data, target, and index if return_index is set to True. Otherwise, it returns a tuple containing data and target only (default: ``False``)
 
     """
 
     base_folder = "cifar-10-batches-py"
     url = "https://www.cs.toronto.edu/~kriz/cifar-10-python.tar.gz"
     filename = "cifar-10-python.tar.gz"
     tgz_md5 = "c58f30108f718f92721af3b95e74349a"
```

### Comparing `libauc-1.3.2/libauc/datasets/dataset.py` & `libauc-1.3.3/libauc/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/folder.py` & `libauc-1.3.3/libauc/datasets/folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,15 @@
             a sample and returns a transformed version.
             E.g, ``transforms.RandomCrop`` for images.
         target_transform (callable, optional): A function/transform that takes
             in the target and transforms it.
         is_valid_file (callable, optional): A function that takes path of a file
             and check if the file is a valid file (used to check of corrupt files)
             both extensions and is_valid_file should not be passed.
+        return_index (bool, optional): returns a tuple containing data, target, and index if return_index is set to True. Otherwise, it returns a tuple containing data and target only (default: ``False``)
 
      Attributes:
         classes (list): List of the class names sorted alphabetically.
         class_to_idx (dict): Dict with items (class_name, class_index).
         samples (list): List of (sample path, class_index) tuples
         targets (list): The class_index value for each image in the dataset
     """
@@ -290,31 +291,34 @@
         transform (callable, optional): A function/transform that  takes in an PIL image
             and returns a transformed version. E.g, ``transforms.RandomCrop``
         target_transform (callable, optional): A function/transform that takes in the
             target and transforms it.
         loader (callable, optional): A function to load an image given its path.
         is_valid_file (callable, optional): A function that takes path of an Image file
             and check if the file is a valid file (used to check of corrupt files)
+        return_index (bool, optional): returns a tuple containing data, target, and index if return_index is set to True. Otherwise, it returns a tuple containing data and target only (default: ``False``)
 
      Attributes:
         classes (list): List of the class names sorted alphabetically.
         class_to_idx (dict): Dict with items (class_name, class_index).
         imgs (list): List of (image path, class_index) tuples
     """
 
     def __init__(
         self,
         root: str,
         transform: Optional[Callable] = None,
         target_transform: Optional[Callable] = None,
         loader: Callable[[str], Any] = default_loader,
         is_valid_file: Optional[Callable[[str], bool]] = None,
+        return_index: bool = False,
     ):
         super().__init__(
             root,
             loader,
             IMG_EXTENSIONS if is_valid_file is None else None,
             transform=transform,
             target_transform=target_transform,
             is_valid_file=is_valid_file,
+            return_index=return_index,
         )
         self.imgs = self.samples
```

### Comparing `libauc-1.3.2/libauc/datasets/melanoma.py` & `libauc-1.3.3/libauc/datasets/melanoma.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/movielens.py` & `libauc-1.3.3/libauc/datasets/movielens.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/musk2.py` & `libauc-1.3.3/libauc/datasets/musk2.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/datasets/stl10.py` & `libauc-1.3.3/libauc/datasets/stl10.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/losses/auc.py` & `libauc-1.3.3/libauc/losses/auc.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/losses/contrastive.py` & `libauc-1.3.3/libauc/losses/contrastive.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/losses/losses.py` & `libauc-1.3.3/libauc/losses/losses.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/losses/mil.py` & `libauc-1.3.3/libauc/losses/mil.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/losses/perf_at_top.py` & `libauc-1.3.3/libauc/losses/perf_at_top.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/losses/ranking.py` & `libauc-1.3.3/libauc/losses/ranking.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/losses/surrogate.py` & `libauc-1.3.3/libauc/losses/surrogate.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/metrics/metrics.py` & `libauc-1.3.3/libauc/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/models/densenet.py` & `libauc-1.3.3/libauc/models/densenet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/models/mil_models.py` & `libauc-1.3.3/libauc/models/mil_models.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/models/neumf.py` & `libauc-1.3.3/libauc/models/neumf.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/models/perceptron.py` & `libauc-1.3.3/libauc/models/perceptron.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/models/resnet.py` & `libauc-1.3.3/libauc/models/resnet.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/models/resnet_cifar.py` & `libauc-1.3.3/libauc/models/resnet_cifar.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/adam.py` & `libauc-1.3.3/libauc/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/adamw.py` & `libauc-1.3.3/libauc/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/isogclr.py` & `libauc-1.3.3/libauc/optimizers/isogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/lars.py` & `libauc-1.3.3/libauc/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/midam.py` & `libauc-1.3.3/libauc/optimizers/midam.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/pdsca.py` & `libauc-1.3.3/libauc/optimizers/pdsca.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/pesg.py` & `libauc-1.3.3/libauc/optimizers/pesg.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/sgd.py` & `libauc-1.3.3/libauc/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/soap.py` & `libauc-1.3.3/libauc/optimizers/soap.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/sogclr.py` & `libauc-1.3.3/libauc/optimizers/sogclr.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/song.py` & `libauc-1.3.3/libauc/optimizers/song.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/sopa.py` & `libauc-1.3.3/libauc/optimizers/sopa.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/sopa_s.py` & `libauc-1.3.3/libauc/optimizers/sopa_s.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/optimizers/sota_s.py` & `libauc-1.3.3/libauc/optimizers/sota_s.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/sampler/sampler.py` & `libauc-1.3.3/libauc/sampler/sampler.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/utils/paper_utils.py` & `libauc-1.3.3/libauc/utils/paper_utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc/utils/utils.py` & `libauc-1.3.3/libauc/utils/utils.py`

 * *Files identical despite different names*

### Comparing `libauc-1.3.2/libauc.egg-info/PKG-INFO` & `libauc-1.3.3/libauc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libauc
-Version: 1.3.2
+Version: 1.3.3
 Summary: LibAUC: A Deep Learning Library for X-Risk Optimization
 Home-page: https://github.com/Optimization-AI/LibAUC
 Author: Zhuoning Yuan
 Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: libauc Version: 1.3.2 Summary: LibAUC: A Deep
+Metadata-Version: 2.1 Name: libauc Version: 1.3.3 Summary: LibAUC: A Deep
 Learning Library for X-Risk Optimization Home-page: https://github.com/
 Optimization-AI/LibAUC Author: Zhuoning Yuan Author-email: yzhuoning@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE LibAUC: A Deep Learning for X-Risk Optimization ---
 _[_P_y_p_i_]_[_D_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_]_[_P_y_T_o_r_c_h_]_[_L_I_C_E_N_S_E_]
```

### Comparing `libauc-1.3.2/libauc.egg-info/SOURCES.txt` & `libauc-1.3.3/libauc.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+setup.cfg
 setup.py
 libauc/__init__.py
 libauc.egg-info/PKG-INFO
 libauc.egg-info/SOURCES.txt
 libauc.egg-info/dependency_links.txt
 libauc.egg-info/requires.txt
 libauc.egg-info/top_level.txt
```

### Comparing `libauc-1.3.2/setup.py` & `libauc-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
   
 setuptools.setup(
   name="libauc",
-  version="1.3.2",
+  version="1.3.3",
   author="Zhuoning Yuan",
   author_email="yzhuoning@gmail.com",
   description="LibAUC: A Deep Learning Library for X-Risk Optimization",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/Optimization-AI/LibAUC",
   packages=setuptools.find_packages(),
```

