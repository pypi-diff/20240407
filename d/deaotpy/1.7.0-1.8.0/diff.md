# Comparing `tmp/deaotpy-1.7.0.tar.gz` & `tmp/deaotpy-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deaotpy-1.7.0.tar", last modified: Tue Apr  2 21:04:27 2024, max compression
+gzip compressed data, was "deaotpy-1.8.0.tar", last modified: Sun Apr  7 15:12:44 2024, max compression
```

## Comparing `deaotpy-1.7.0.tar` & `deaotpy-1.8.0.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.059701 deaotpy-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 20:54:13.000000 deaotpy-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-02 21:04:27.059701 deaotpy-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-02 20:54:13.000000 deaotpy-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.035701 deaotpy-1.7.0/aot/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.035701 deaotpy-1.7.0/aot/configs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5579 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/default.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.039701 deaotpy-1.7.0/aot/configs/models/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/aotb.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/aots.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/aott.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/deaotb.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/deaots.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/deaott.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/default.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/default_deaot.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/r101_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/r50_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/r50_deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/rs101_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/swinb_aotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/models/swinb_deaotl.py
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/pre.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/pre_dav.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/pre_ytb.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/pre_ytb_dav.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/configs/ytb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.043701 deaotpy-1.7.0/aot/dataloaders/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/dataloaders/eval_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19828 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/dataloaders/image_transforms.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24646 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/dataloaders/train_datasets.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23575 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/dataloaders/video_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.043701 deaotpy-1.7.0/aot/networks/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.043701 deaotpy-1.7.0/aot/networks/decoders/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/decoders/fpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.043701 deaotpy-1.7.0/aot/networks/encoders/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/mobilenetv2.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7899 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/mobilenetv3.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.047701 deaotpy-1.7.0/aot/networks/encoders/resnest/
--rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/resnest/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3343 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/resnest/resnest.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16474 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/resnest/resnet.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4467 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/resnest/splat.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6692 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/resnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.047701 deaotpy-1.7.0/aot/networks/encoders/swin/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/swin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/swin/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    27345 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/encoders/swin/swin_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.047701 deaotpy-1.7.0/aot/networks/engines/
--rwxr-xr-x   0 runner    (1001) docker     (127)      693 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/engines/aot_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/engines/deaot_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.051701 deaotpy-1.7.0/aot/networks/layers/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32782 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/layers/attention.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/layers/basic.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/layers/loss.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/layers/normalization.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/layers/position.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    24836 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/layers/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.051701 deaotpy-1.7.0/aot/networks/managers/
--rwxr-xr-x   0 runner    (1001) docker     (127)    25895 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/managers/evaluator.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    29712 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/managers/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.051701 deaotpy-1.7.0/aot/networks/models/
--rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/models/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4546 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/models/aot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-02 20:54:14.000000 deaotpy-1.7.0/aot/networks/models/deaot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.055701 deaotpy-1.7.0/aot/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/tools/demo.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3472 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/tools/eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2668 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/tools/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.055701 deaotpy-1.7.0/aot/utils/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6200 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/cp_ckpt.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3561 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/ema.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/eval.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6075 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/image.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3454 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/learning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/math.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/meters.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-04-02 20:54:15.000000 deaotpy-1.7.0/aot/utils/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 21:04:27.059701 deaotpy-1.7.0/deaotpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-02 21:04:27.000000 deaotpy-1.7.0/deaotpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-02 21:04:27.000000 deaotpy-1.7.0/deaotpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 21:04:27.000000 deaotpy-1.7.0/deaotpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 21:04:27.000000 deaotpy-1.7.0/deaotpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 21:04:27.000000 deaotpy-1.7.0/deaotpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-02 20:54:13.000000 deaotpy-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 21:04:27.059701 deaotpy-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.304015 deaotpy-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-07 15:03:06.000000 deaotpy-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-07 15:12:44.304015 deaotpy-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-07 15:03:06.000000 deaotpy-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.280014 deaotpy-1.8.0/aot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13858 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.280014 deaotpy-1.8.0/aot/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5579 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/default.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/configs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/aott.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/deaott.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      957 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/default.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/default_deaot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/r101_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/r50_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/r50_deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/rs101_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/swinb_aotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/models/swinb_deaotl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre_dav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre_ytb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/pre_ytb_dav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/configs/ytb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/dataloaders/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14304 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/eval_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19828 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/image_transforms.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24646 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/train_datasets.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    23575 2024-04-07 15:03:07.000000 deaotpy-1.8.0/aot/dataloaders/video_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/networks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.288015 deaotpy-1.8.0/aot/networks/decoders/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/decoders/fpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.292015 deaotpy-1.8.0/aot/networks/encoders/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1405 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8420 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/mobilenetv2.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7899 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/mobilenetv3.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.292015 deaotpy-1.8.0/aot/networks/encoders/resnest/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       23 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3343 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/resnest.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16474 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/resnet.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4467 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnest/splat.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6692 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/resnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.292015 deaotpy-1.8.0/aot/networks/encoders/swin/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/swin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/swin/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27345 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/encoders/swin/swin_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.296015 deaotpy-1.8.0/aot/networks/engines/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      693 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24646 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/engines/aot_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/engines/deaot_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.296015 deaotpy-1.8.0/aot/networks/layers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32782 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/attention.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5111 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/basic.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6698 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/loss.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1700 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/normalization.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2810 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/position.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    24836 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/layers/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.296015 deaotpy-1.8.0/aot/networks/managers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25895 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/managers/evaluator.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    29712 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/managers/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.300015 deaotpy-1.8.0/aot/networks/models/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      344 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/models/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4546 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/models/aot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/networks/models/deaot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.300015 deaotpy-1.8.0/aot/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12850 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/tools/demo.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3472 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/tools/eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2668 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/tools/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.304015 deaotpy-1.8.0/aot/utils/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6200 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/cp_ckpt.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3561 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/ema.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      443 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/eval.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6075 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/image.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3454 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/learning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      829 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/math.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      860 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/meters.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1102 2024-04-07 15:03:08.000000 deaotpy-1.8.0/aot/utils/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:12:44.304015 deaotpy-1.8.0/deaotpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-07 15:12:44.000000 deaotpy-1.8.0/deaotpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-07 15:03:06.000000 deaotpy-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:12:44.304015 deaotpy-1.8.0/setup.cfg
```

### Comparing `deaotpy-1.7.0/LICENSE` & `deaotpy-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/PKG-INFO` & `deaotpy-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deaotpy
-Version: 1.7.0
+Version: 1.8.0
 Summary: Decoupling Features in Hierarchical Propagation for Video Object Segmentation.
 License: BSD 3-Clause License
         
         Copyright (c) 2020, z-x-yang
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `deaotpy-1.7.0/README.md` & `deaotpy-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/LICENSE` & `deaotpy-1.8.0/aot/LICENSE`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/README.md` & `deaotpy-1.8.0/aot/README.md`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/default.py` & `deaotpy-1.8.0/aot/configs/default.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/models/default.py` & `deaotpy-1.8.0/aot/configs/models/default.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/models/r101_aotl.py` & `deaotpy-1.8.0/aot/configs/models/r101_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/models/r50_aotl.py` & `deaotpy-1.8.0/aot/configs/models/r50_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/models/r50_deaotl.py` & `deaotpy-1.8.0/aot/configs/models/r50_deaotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/models/rs101_aotl.py` & `deaotpy-1.8.0/aot/configs/models/rs101_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/models/swinb_aotl.py` & `deaotpy-1.8.0/aot/configs/models/swinb_aotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/models/swinb_deaotl.py` & `deaotpy-1.8.0/aot/configs/models/swinb_deaotl.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/pre.py` & `deaotpy-1.8.0/aot/configs/pre.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/pre_dav.py` & `deaotpy-1.8.0/aot/configs/pre_dav.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/pre_ytb.py` & `deaotpy-1.8.0/aot/configs/pre_ytb.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/configs/pre_ytb_dav.py` & `deaotpy-1.8.0/aot/configs/pre_ytb_dav.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/dataloaders/eval_datasets.py` & `deaotpy-1.8.0/aot/dataloaders/eval_datasets.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/dataloaders/image_transforms.py` & `deaotpy-1.8.0/aot/dataloaders/image_transforms.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/dataloaders/train_datasets.py` & `deaotpy-1.8.0/aot/dataloaders/train_datasets.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/dataloaders/video_transforms.py` & `deaotpy-1.8.0/aot/dataloaders/video_transforms.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/decoders/fpn.py` & `deaotpy-1.8.0/aot/networks/decoders/fpn.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/__init__.py` & `deaotpy-1.8.0/aot/networks/encoders/__init__.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/mobilenetv2.py` & `deaotpy-1.8.0/aot/networks/encoders/mobilenetv2.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/mobilenetv3.py` & `deaotpy-1.8.0/aot/networks/encoders/mobilenetv3.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/resnest/resnest.py` & `deaotpy-1.8.0/aot/networks/encoders/resnest/resnest.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/resnest/resnet.py` & `deaotpy-1.8.0/aot/networks/encoders/resnest/resnet.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/resnest/splat.py` & `deaotpy-1.8.0/aot/networks/encoders/resnest/splat.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/resnet.py` & `deaotpy-1.8.0/aot/networks/encoders/resnet.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/swin/build.py` & `deaotpy-1.8.0/aot/networks/encoders/swin/build.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/encoders/swin/swin_transformer.py` & `deaotpy-1.8.0/aot/networks/encoders/swin/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/engines/__init__.py` & `deaotpy-1.8.0/aot/networks/engines/__init__.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/engines/aot_engine.py` & `deaotpy-1.8.0/aot/networks/engines/aot_engine.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/engines/deaot_engine.py` & `deaotpy-1.8.0/aot/networks/engines/deaot_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from utils.image import one_hot_mask
+from aot.utils.image import one_hot_mask
 
 from aot.networks.layers.basic import seq_to_2d
 from aot.networks.engines.aot_engine import AOTEngine, AOTInferEngine
 
 
 class DeAOTEngine(AOTEngine):
     def __init__(self,
```

### Comparing `deaotpy-1.7.0/aot/networks/layers/attention.py` & `deaotpy-1.8.0/aot/networks/layers/attention.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/layers/basic.py` & `deaotpy-1.8.0/aot/networks/layers/basic.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/layers/loss.py` & `deaotpy-1.8.0/aot/networks/layers/loss.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/layers/normalization.py` & `deaotpy-1.8.0/aot/networks/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/layers/position.py` & `deaotpy-1.8.0/aot/networks/layers/position.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/layers/transformer.py` & `deaotpy-1.8.0/aot/networks/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/managers/evaluator.py` & `deaotpy-1.8.0/aot/networks/managers/evaluator.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/managers/trainer.py` & `deaotpy-1.8.0/aot/networks/managers/trainer.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/models/aot.py` & `deaotpy-1.8.0/aot/networks/models/aot.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/networks/models/deaot.py` & `deaotpy-1.8.0/aot/networks/models/deaot.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/tools/demo.py` & `deaotpy-1.8.0/aot/tools/demo.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/tools/eval.py` & `deaotpy-1.8.0/aot/tools/eval.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/tools/train.py` & `deaotpy-1.8.0/aot/tools/train.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/checkpoint.py` & `deaotpy-1.8.0/aot/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/cp_ckpt.py` & `deaotpy-1.8.0/aot/utils/cp_ckpt.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/ema.py` & `deaotpy-1.8.0/aot/utils/ema.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/image.py` & `deaotpy-1.8.0/aot/utils/image.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/learning.py` & `deaotpy-1.8.0/aot/utils/learning.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/math.py` & `deaotpy-1.8.0/aot/utils/math.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/meters.py` & `deaotpy-1.8.0/aot/utils/meters.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/aot/utils/metric.py` & `deaotpy-1.8.0/aot/utils/metric.py`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/deaotpy.egg-info/PKG-INFO` & `deaotpy-1.8.0/deaotpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deaotpy
-Version: 1.7.0
+Version: 1.8.0
 Summary: Decoupling Features in Hierarchical Propagation for Video Object Segmentation.
 License: BSD 3-Clause License
         
         Copyright (c) 2020, z-x-yang
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `deaotpy-1.7.0/deaotpy.egg-info/SOURCES.txt` & `deaotpy-1.8.0/deaotpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deaotpy-1.7.0/pyproject.toml` & `deaotpy-1.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
   "setuptools",
   "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deaotpy"
-version = "1.7.0"
+version = "1.8.0"
 description = "Decoupling Features in Hierarchical Propagation for Video Object Segmentation."
 readme = { file = "aot/README.md" , content-type = "text/markdown" }
 
 license = { file = "aot/LICENSE" }
 requires-python = ">=3.10"
 keywords = [
     "deep-learning",
```

