# Comparing `tmp/gdinopy-1.0.0.tar.gz` & `tmp/gdinopy-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdinopy-1.0.0.tar", last modified: Mon Apr  1 15:22:23 2024, max compression
+gzip compressed data, was "gdinopy-1.1.0.tar", last modified: Sun Apr  7 15:30:02 2024, max compression
```

## Comparing `gdinopy-1.0.0.tar` & `gdinopy-1.1.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.656177 gdinopy-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-01 15:17:36.000000 gdinopy-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-01 15:17:36.000000 gdinopy-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    32022 2024-04-01 15:22:23.656177 gdinopy-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-04-01 15:17:36.000000 gdinopy-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.640177 gdinopy-1.0.0/gdinopy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32022 2024-04-01 15:22:23.000000 gdinopy-1.0.0/gdinopy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-01 15:22:23.000000 gdinopy-1.0.0/gdinopy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:22:23.000000 gdinopy-1.0.0/gdinopy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 15:22:23.000000 gdinopy-1.0.0/gdinopy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 15:22:23.000000 gdinopy-1.0.0/gdinopy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.640177 gdinopy-1.0.0/groundingdino/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.644177 gdinopy-1.0.0/groundingdino/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/config/GroundingDINO_SwinB_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/config/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.644177 gdinopy-1.0.0/groundingdino/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/datasets/cocogrounding_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/datasets/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.644177 gdinopy-1.0.0/groundingdino/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.648177 gdinopy-1.0.0/groundingdino/models/GroundingDINO/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.648177 gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/backbone.py
--rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)    29381 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/bertwarper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.648177 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.652177 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn.h
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.h
--rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.h
--rw-r--r--   0 runner    (1001) docker     (127)    54694 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_im2col_cuda.cuh
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/cuda_version.cu
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/vision.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/fuse_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    17406 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/groundingdino.py
--rw-r--r--   0 runner    (1001) docker     (127)    15512 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/ms_deform_attn.py
--rw-r--r--   0 runner    (1001) docker     (127)    36935 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/transformer_vanilla.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/GroundingDINO/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/models/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:22:23.656177 gdinopy-1.0.0/groundingdino/util/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/box_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/get_tokenlizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    23348 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/slconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/slio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/time_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    17828 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-01 15:17:36.000000 gdinopy-1.0.0/groundingdino/util/vl_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-01 15:22:23.000000 gdinopy-1.0.0/groundingdino/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 15:17:36.000000 gdinopy-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-01 15:17:36.000000 gdinopy-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:22:23.656177 gdinopy-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-01 15:17:36.000000 gdinopy-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.254962 gdinopy-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-07 15:23:44.000000 gdinopy-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-07 15:23:44.000000 gdinopy-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    32022 2024-04-07 15:30:02.254962 gdinopy-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18784 2024-04-07 15:23:44.000000 gdinopy-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.234962 gdinopy-1.1.0/gdinopy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32022 2024-04-07 15:30:02.000000 gdinopy-1.1.0/gdinopy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-07 15:30:02.000000 gdinopy-1.1.0/gdinopy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:30:02.000000 gdinopy-1.1.0/gdinopy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 15:30:02.000000 gdinopy-1.1.0/gdinopy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-07 15:30:02.000000 gdinopy-1.1.0/gdinopy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.234962 gdinopy-1.1.0/groundingdino/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.234962 gdinopy-1.1.0/groundingdino/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/config/GroundingDINO_SwinB_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/config/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.238962 gdinopy-1.1.0/groundingdino/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9398 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/datasets/cocogrounding_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9711 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/datasets/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.238962 gdinopy-1.1.0/groundingdino/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.242962 gdinopy-1.1.0/groundingdino/models/GroundingDINO/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.242962 gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/backbone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29381 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12242 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/bertwarper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.242962 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.242962 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7367 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.h
+-rw-r--r--   0 runner    (1001) docker     (127)    54694 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_im2col_cuda.cuh
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/cuda_version.cu
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/vision.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11825 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/fuse_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17406 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/groundingdino.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15522 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/ms_deform_attn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36935 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4043 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/transformer_vanilla.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/GroundingDINO/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/models/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:30:02.254962 gdinopy-1.1.0/groundingdino/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/box_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/get_tokenlizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14931 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3303 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23348 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14380 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/slconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/slio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1567 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/time_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17828 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-07 15:23:44.000000 gdinopy-1.1.0/groundingdino/util/vl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 15:30:01.000000 gdinopy-1.1.0/groundingdino/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-07 15:23:44.000000 gdinopy-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 15:23:44.000000 gdinopy-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:30:02.254962 gdinopy-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-07 15:23:44.000000 gdinopy-1.1.0/setup.py
```

### Comparing `gdinopy-1.0.0/LICENSE` & `gdinopy-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/PKG-INFO` & `gdinopy-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdinopy
-Version: 1.0.0
+Version: 1.1.0
 Summary: open-set object detector
 Home-page: https://github.com/IDEA-Research/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gdinopy-1.0.0/README.md` & `gdinopy-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/gdinopy.egg-info/PKG-INFO` & `gdinopy-1.1.0/gdinopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdinopy
-Version: 1.0.0
+Version: 1.1.0
 Summary: open-set object detector
 Home-page: https://github.com/IDEA-Research/GroundingDINO
 Author: International Digital Economy Academy, Shilong Liu
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `gdinopy-1.0.0/gdinopy.egg-info/SOURCES.txt` & `gdinopy-1.1.0/gdinopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/config/GroundingDINO_SwinB_cfg.py` & `gdinopy-1.1.0/groundingdino/config/GroundingDINO_SwinB_cfg.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/config/GroundingDINO_SwinT_OGC.py` & `gdinopy-1.1.0/groundingdino/config/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/datasets/cocogrounding_eval.py` & `gdinopy-1.1.0/groundingdino/datasets/cocogrounding_eval.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/datasets/transforms.py` & `gdinopy-1.1.0/groundingdino/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/__init__.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/__init__.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/backbone.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/backbone.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/position_encoding.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/backbone/swin_transformer.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/bertwarper.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/bertwarper.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn.h` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn.h`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.cpp` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.cpp`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.h` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cpu.h`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.cu` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.cu`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.h` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_attn_cuda.h`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_im2col_cuda.cuh` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/MsDeformAttn/ms_deform_im2col_cuda.cuh`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/csrc/vision.cpp` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/csrc/vision.cpp`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/fuse_modules.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/fuse_modules.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/groundingdino.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/groundingdino.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/ms_deform_attn.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/ms_deform_attn.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 from torch.autograd import Function
 from torch.autograd.function import once_differentiable
 from torch.nn.init import constant_, xavier_uniform_
 
 try:
     from groundingdino import _C
 except:
-    warnings.warn("Failed to load custom C++ ops. Running on CPU mode Only!")
+    pass
+    #warnings.warn("Failed to load custom C++ ops. Running on CPU mode Only!")
 
 
 # helpers
 def _is_power_of_2(n):
     if (not isinstance(n, int)) or (n < 0):
         raise ValueError("invalid input for _is_power_of_2: {} (type: {})".format(n, type(n)))
     return (n & (n - 1) == 0) and n != 0
```

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/transformer.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/transformer.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/transformer_vanilla.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/transformer_vanilla.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/GroundingDINO/utils.py` & `gdinopy-1.1.0/groundingdino/models/GroundingDINO/utils.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/__init__.py` & `gdinopy-1.1.0/groundingdino/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/models/registry.py` & `gdinopy-1.1.0/groundingdino/models/registry.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/box_ops.py` & `gdinopy-1.1.0/groundingdino/util/box_ops.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/get_tokenlizer.py` & `gdinopy-1.1.0/groundingdino/util/get_tokenlizer.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/inference.py` & `gdinopy-1.1.0/groundingdino/util/inference.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/logger.py` & `gdinopy-1.1.0/groundingdino/util/logger.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/misc.py` & `gdinopy-1.1.0/groundingdino/util/misc.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/slconfig.py` & `gdinopy-1.1.0/groundingdino/util/slconfig.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/slio.py` & `gdinopy-1.1.0/groundingdino/util/slio.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/time_counter.py` & `gdinopy-1.1.0/groundingdino/util/time_counter.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/utils.py` & `gdinopy-1.1.0/groundingdino/util/utils.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/visualizer.py` & `gdinopy-1.1.0/groundingdino/util/visualizer.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/groundingdino/util/vl_utils.py` & `gdinopy-1.1.0/groundingdino/util/vl_utils.py`

 * *Files identical despite different names*

### Comparing `gdinopy-1.0.0/setup.py` & `gdinopy-1.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 install_torch()
 
 import torch
 from setuptools import find_packages, setup
 from torch.utils.cpp_extension import CUDA_HOME, CppExtension, CUDAExtension
 
 # groundingdino version info
-version = "1.0.0"
+version = "1.1.0"
 package_name = "groundingdino"
 program_name = "gdinopy"
 cwd = os.path.dirname(os.path.abspath(__file__))
 
 
 sha = "Unknown"
 try:
```

