# Comparing `tmp/lightning-thunder-0.2.0.dev20240404.tar.gz` & `tmp/lightning-thunder-0.2.0.dev20240407.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-thunder-0.2.0.dev20240404.tar", last modified: Thu Apr  4 12:41:35 2024, max compression
+gzip compressed data, was "lightning-thunder-0.2.0.dev20240407.tar", last modified: Sun Apr  7 00:21:01 2024, max compression
```

## Comparing `lightning-thunder-0.2.0.dev20240404.tar` & `lightning-thunder-0.2.0.dev20240407.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.951139 lightning-thunder-0.2.0.dev20240404/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-04-04 12:41:35.951139 lightning-thunder-0.2.0.dev20240404/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.951139 lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-04-04 12:41:35.000000 lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-04 12:41:35.000000 lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:41:35.000000 lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 12:41:35.000000 lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-04 12:41:35.000000 lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 12:41:35.000000 lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.931139 lightning-thunder-0.2.0.dev20240404/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/requirements/devel.txt
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/requirements/notebooks.txt
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 12:41:35.951139 lightning-thunder-0.2.0.dev20240404/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     5871 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.935139 lightning-thunder-0.2.0.dev20240404/thunder/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-04 12:41:35.000000 lightning-thunder-0.2.0.dev20240404/thunder/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33198 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.935139 lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)   101338 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/benchmark_litgpt.py
--rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/einsum.py
--rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/targets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/test_benchmark_litgpt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.935139 lightning-thunder-0.2.0.dev20240404/thunder/clang/
--rw-r--r--   0 runner    (1001) docker     (127)    63665 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/clang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/clang/langctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    31687 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.943139 lightning-thunder-0.2.0.dev20240404/thunder/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/baseutils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/codeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/compile_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (127)   256512 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (127)    54102 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/jit_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/langctxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)   116011 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/prims.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    48752 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/pytree.py
--rw-r--r--   0 runner    (1001) docker     (127)    28140 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/rematerialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    25222 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)    18726 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/transform_common.py
--rw-r--r--   0 runner    (1001) docker     (127)   140309 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    37010 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/core/vjp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.943139 lightning-thunder-0.2.0.dev20240404/thunder/cudagraphs/
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/cudagraphs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.943139 lightning-thunder-0.2.0.dev20240404/thunder/distributed/
--rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/bucketing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/prims.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.943139 lightning-thunder-0.2.0.dev20240404/thunder/distributed/transforms/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/transforms/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)    28416 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/transforms/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/distributed/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.943139 lightning-thunder-0.2.0.dev20240404/thunder/examine/
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/examine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/examine/memory_caculation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.947139 lightning-thunder-0.2.0.dev20240404/thunder/executors/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/apex_entropyex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/cudnn_layernormex.py
--rw-r--r--   0 runner    (1001) docker     (127)    24903 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/cudnnex.py
--rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/data_dependent_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/nvfuserex.py
--rw-r--r--   0 runner    (1001) docker     (127)    74595 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/nvfuserex_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/pythonex.py
--rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/sdpaex.py
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/torch_autograd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/torch_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    76466 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/torchex.py
--rw-r--r--   0 runner    (1001) docker     (127)    17144 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/transformer_engineex.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/triton_crossentropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19675 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/triton_crossentropy_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/triton_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/executors/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.947139 lightning-thunder-0.2.0.dev20240404/thunder/extend/
--rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/extend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/functional.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.947139 lightning-thunder-0.2.0.dev20240404/thunder/numpy/
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/numpy/langctx.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 12:41:35.951139 lightning-thunder-0.2.0.dev20240404/thunder/torch/
--rw-r--r--   0 runner    (1001) docker     (127)   146468 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-04 12:41:33.000000 lightning-thunder-0.2.0.dev20240404/thunder/torch/langctx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.723020 lightning-thunder-0.2.0.dev20240407/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-04-07 00:21:01.723020 lightning-thunder-0.2.0.dev20240407/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.719020 lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-04-07 00:21:01.000000 lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-07 00:21:01.000000 lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:21:01.000000 lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 00:21:01.000000 lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-07 00:21:01.000000 lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-07 00:21:01.000000 lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.703020 lightning-thunder-0.2.0.dev20240407/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/requirements/devel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/requirements/notebooks.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 00:21:01.723020 lightning-thunder-0.2.0.dev20240407/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5871 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.703020 lightning-thunder-0.2.0.dev20240407/thunder/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-07 00:21:01.000000 lightning-thunder-0.2.0.dev20240407/thunder/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33198 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.707020 lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)   101338 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21165 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/benchmark_litgpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20006 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/einsum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26212 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/targets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/test_benchmark_litgpt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.707020 lightning-thunder-0.2.0.dev20240407/thunder/clang/
+-rw-r--r--   0 runner    (1001) docker     (127)    63665 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/clang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/clang/langctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31687 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.711020 lightning-thunder-0.2.0.dev20240407/thunder/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/baseutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13335 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/codeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/compile_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   256512 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54102 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/jit_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/langctxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7046 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14058 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)   116011 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/prims.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48752 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/pytree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28140 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/rematerialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25222 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18726 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/transform_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)   140309 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37010 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/core/vjp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.711020 lightning-thunder-0.2.0.dev20240407/thunder/cudagraphs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/cudagraphs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.715020 lightning-thunder-0.2.0.dev20240407/thunder/distributed/
+-rw-r--r--   0 runner    (1001) docker     (127)    17549 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/bucketing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/prims.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.715020 lightning-thunder-0.2.0.dev20240407/thunder/distributed/transforms/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8449 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/transforms/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28416 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/transforms/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10897 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/distributed/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.715020 lightning-thunder-0.2.0.dev20240407/thunder/examine/
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/examine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5761 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/examine/memory_caculation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.719020 lightning-thunder-0.2.0.dev20240407/thunder/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7092 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/apex_entropyex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/cudnn_layernormex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24903 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/cudnnex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/data_dependent_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/nvfuserex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74595 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/nvfuserex_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10861 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/pythonex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26538 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/sdpaex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/torch_autograd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7908 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/torch_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76466 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/torchex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22098 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/transformer_engineex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/triton_crossentropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19675 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/triton_crossentropy_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/triton_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/executors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.719020 lightning-thunder-0.2.0.dev20240407/thunder/extend/
+-rw-r--r--   0 runner    (1001) docker     (127)    11671 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/extend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16957 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/functional.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.719020 lightning-thunder-0.2.0.dev20240407/thunder/numpy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/numpy/langctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 00:21:01.719020 lightning-thunder-0.2.0.dev20240407/thunder/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)   146468 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-07 00:20:59.000000 lightning-thunder-0.2.0.dev20240407/thunder/torch/langctx.py
```

### Comparing `lightning-thunder-0.2.0.dev20240404/LICENSE` & `lightning-thunder-0.2.0.dev20240407/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/MANIFEST.in` & `lightning-thunder-0.2.0.dev20240407/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/PKG-INFO` & `lightning-thunder-0.2.0.dev20240407/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-thunder
-Version: 0.2.0.dev20240404
+Version: 0.2.0.dev20240407
 Summary: Lightning Thunder project.
 Home-page: https://github.com/Lightning-AI/lightning-thunder
 Download-URL: https://github.com/Lightning-AI/lightning-thunder
 Author: Lightning-AI et al
 Author-email: community@lightning.ai
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-thunder/issues
@@ -28,14 +28,16 @@
 Requires-Dist: looseversion==1.3.0
 Requires-Dist: lightning-utilities>=0.7.0
 Requires-Dist: numpy<2,>=1.23.0
 Requires-Dist: igraph>=0.10.4
 Requires-Dist: optree>=0.9.2
 Requires-Dist: opt_einsum>=3.3.0
 Requires-Dist: mpmath<1.4.0
+Provides-Extra: notebooks
+Requires-Dist: ipython[all]==8.23.0; extra == "notebooks"
 Provides-Extra: test
 Requires-Dist: absl-py; extra == "test"
 Requires-Dist: coverage==7.4.4; extra == "test"
 Requires-Dist: einops; extra == "test"
 Requires-Dist: expecttest==0.2.1; extra == "test"
 Requires-Dist: fdm==0.4.1; extra == "test"
 Requires-Dist: graphviz==0.20.1; extra == "test"
@@ -48,20 +50,18 @@
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
 Requires-Dist: pytest-random-order==1.1.1; extra == "test"
 Requires-Dist: pytest-timeout==2.2.0; extra == "test"
 Requires-Dist: pytest-timestamper==0.0.10; extra == "test"
 Requires-Dist: pytest-xdist==3.5.0; extra == "test"
 Requires-Dist: pytest==8.1.1; extra == "test"
 Requires-Dist: xlsxwriter; extra == "test"
-Provides-Extra: notebooks
-Requires-Dist: ipython[all]==8.23.0; extra == "notebooks"
 
 <div align="center">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/LightningThunderLightModewByline.png#gh-light-mode-only" width="400px" style="max-width: 100%;">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/LightningThunderDarkModewByline.png#gh-dark-mode-only" width="400px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/LightningThunderLightModewByline.png#gh-light-mode-only" width="400px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/LightningThunderDarkModewByline.png#gh-dark-mode-only" width="400px" style="max-width: 100%;">
     <br/>
 <br/>
 
 **Make PyTorch models Lightning fast.**
 
 ______________________________________________________________________
 
@@ -101,27 +101,27 @@
 &#160;
 
 ## Single-GPU performance
 
 Thunder can achieve significant speedups over standard non-compiled PyTorch code ("PyTorch eager"), through the compounding effects of optimizations and the use of best-in-class executors. The figure below shows the pretraining throughput for Llama 2 7B as implemented in [LitGPT](https://github.com/Lightning-AI/litgpt).
 
 <div align="center">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/training_throughput_single.png" width="800px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/training_throughput_single.png" width="800px" style="max-width: 100%;">
 </div>
 
 As shown in the plot above, Thunder achieves a 40% speedup in training throughput compared to eager code on H100 using a combination of executors including nvFuser, torch.compile, cuDNN, and TransformerEngine FP8.
 
 &#160;
 
 ## Multi-GPU performance
 
 Thunder also supports distributed strategies such as DDP and FSDP for training models on multiple GPUs. The following plot displays the normalized throughput measured for Llama 2 7B without FP8 mixed precision; support for FSDP is in progress.
 
 <div align="center">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/normalized_training_throughput_zero2.png" width="800px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/normalized_training_throughput_zero2.png" width="800px" style="max-width: 100%;">
 </div>
 
 &#160;
 
 ## Get started
 
 The easiest way to get started with Thunder, requiring no extra installations or setups, is by using our [Zero to Thunder Tutorial Studio](https://lightning.ai/lightning-ai/studios/zero-to-thunder-tutorial).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-thunder Version: 0.2.0.dev20240404
+Metadata-Version: 2.1 Name: lightning-thunder Version: 0.2.0.dev20240407
 Summary: Lightning Thunder project. Home-page: https://github.com/Lightning-AI/
 lightning-thunder Download-URL: https://github.com/Lightning-AI/lightning-
 thunder Author: Lightning-AI et al Author-email: community@lightning.ai
 License: Apache 2.0 Project-URL: Bug Tracker, https://github.com/Lightning-AI/
 lightning-thunder/issues Project-URL: Documentation, https://lightning-
 thunder.rtfd.io/en/latest/ Project-URL: Source Code, https://github.com/
 Lightning-AI/lightning-thunder Keywords: deep learning,AI Classifier:
@@ -13,29 +13,29 @@
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.10, <3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 torch>=2.2.0 Requires-Dist: looseversion==1.3.0 Requires-Dist: lightning-
 utilities>=0.7.0 Requires-Dist: numpy<2,>=1.23.0 Requires-Dist: igraph>=0.10.4
 Requires-Dist: optree>=0.9.2 Requires-Dist: opt_einsum>=3.3.0 Requires-Dist:
-mpmath<1.4.0 Provides-Extra: test Requires-Dist: absl-py; extra == "test"
-Requires-Dist: coverage==7.4.4; extra == "test" Requires-Dist: einops; extra ==
-"test" Requires-Dist: expecttest==0.2.1; extra == "test" Requires-Dist:
-fdm==0.4.1; extra == "test" Requires-Dist: graphviz==0.20.1; extra == "test"
-Requires-Dist: hypothesis==6.100.0; extra == "test" Requires-Dist: jax;
+mpmath<1.4.0 Provides-Extra: notebooks Requires-Dist: ipython[all]==8.23.0;
+extra == "notebooks" Provides-Extra: test Requires-Dist: absl-py; extra ==
+"test" Requires-Dist: coverage==7.4.4; extra == "test" Requires-Dist: einops;
+extra == "test" Requires-Dist: expecttest==0.2.1; extra == "test" Requires-
+Dist: fdm==0.4.1; extra == "test" Requires-Dist: graphviz==0.20.1; extra ==
+"test" Requires-Dist: hypothesis==6.100.0; extra == "test" Requires-Dist: jax;
 (sys_platform == "linux" or sys_platform == "darwin") and extra == "test"
 Requires-Dist: jaxlib; (sys_platform == "linux" or sys_platform == "darwin")
 and extra == "test" Requires-Dist: jsonargparse; extra == "test" Requires-Dist:
 numpy; extra == "test" Requires-Dist: pandas; extra == "test" Requires-Dist:
 pytest-cov==4.1.0; extra == "test" Requires-Dist: pytest-random-order==1.1.1;
 extra == "test" Requires-Dist: pytest-timeout==2.2.0; extra == "test" Requires-
 Dist: pytest-timestamper==0.0.10; extra == "test" Requires-Dist: pytest-
 xdist==3.5.0; extra == "test" Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: xlsxwriter; extra == "test" Provides-Extra: notebooks Requires-
-Dist: ipython[all]==8.23.0; extra == "notebooks"
+Requires-Dist: xlsxwriter; extra == "test"
                               [Thunder][Thunder]
 
                     **Make PyTorch models Lightning fast.**
     ______________________________________________________________________
    _L_i_g_h_t_n_i_n_g_._a_i â¢ _P_e_r_f_o_r_m_a_n_c_e â¢ _G_e_t_ _s_t_a_r_t_e_d â¢ _I_n_s_t_a_l_l â¢ _E_x_a_m_p_l_e_s â¢
               _I_n_s_i_d_e_ _T_h_u_n_d_e_r â¢ _G_e_t_ _i_n_v_o_l_v_e_d_! â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
```

### Comparing `lightning-thunder-0.2.0.dev20240404/README.md` & `lightning-thunder-0.2.0.dev20240407/README.md`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/PKG-INFO` & `lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-thunder
-Version: 0.2.0.dev20240404
+Version: 0.2.0.dev20240407
 Summary: Lightning Thunder project.
 Home-page: https://github.com/Lightning-AI/lightning-thunder
 Download-URL: https://github.com/Lightning-AI/lightning-thunder
 Author: Lightning-AI et al
 Author-email: community@lightning.ai
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning-thunder/issues
@@ -28,14 +28,16 @@
 Requires-Dist: looseversion==1.3.0
 Requires-Dist: lightning-utilities>=0.7.0
 Requires-Dist: numpy<2,>=1.23.0
 Requires-Dist: igraph>=0.10.4
 Requires-Dist: optree>=0.9.2
 Requires-Dist: opt_einsum>=3.3.0
 Requires-Dist: mpmath<1.4.0
+Provides-Extra: notebooks
+Requires-Dist: ipython[all]==8.23.0; extra == "notebooks"
 Provides-Extra: test
 Requires-Dist: absl-py; extra == "test"
 Requires-Dist: coverage==7.4.4; extra == "test"
 Requires-Dist: einops; extra == "test"
 Requires-Dist: expecttest==0.2.1; extra == "test"
 Requires-Dist: fdm==0.4.1; extra == "test"
 Requires-Dist: graphviz==0.20.1; extra == "test"
@@ -48,20 +50,18 @@
 Requires-Dist: pytest-cov==4.1.0; extra == "test"
 Requires-Dist: pytest-random-order==1.1.1; extra == "test"
 Requires-Dist: pytest-timeout==2.2.0; extra == "test"
 Requires-Dist: pytest-timestamper==0.0.10; extra == "test"
 Requires-Dist: pytest-xdist==3.5.0; extra == "test"
 Requires-Dist: pytest==8.1.1; extra == "test"
 Requires-Dist: xlsxwriter; extra == "test"
-Provides-Extra: notebooks
-Requires-Dist: ipython[all]==8.23.0; extra == "notebooks"
 
 <div align="center">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/LightningThunderLightModewByline.png#gh-light-mode-only" width="400px" style="max-width: 100%;">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/LightningThunderDarkModewByline.png#gh-dark-mode-only" width="400px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/LightningThunderLightModewByline.png#gh-light-mode-only" width="400px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/LightningThunderDarkModewByline.png#gh-dark-mode-only" width="400px" style="max-width: 100%;">
     <br/>
 <br/>
 
 **Make PyTorch models Lightning fast.**
 
 ______________________________________________________________________
 
@@ -101,27 +101,27 @@
 &#160;
 
 ## Single-GPU performance
 
 Thunder can achieve significant speedups over standard non-compiled PyTorch code ("PyTorch eager"), through the compounding effects of optimizations and the use of best-in-class executors. The figure below shows the pretraining throughput for Llama 2 7B as implemented in [LitGPT](https://github.com/Lightning-AI/litgpt).
 
 <div align="center">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/training_throughput_single.png" width="800px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/training_throughput_single.png" width="800px" style="max-width: 100%;">
 </div>
 
 As shown in the plot above, Thunder achieves a 40% speedup in training throughput compared to eager code on H100 using a combination of executors including nvFuser, torch.compile, cuDNN, and TransformerEngine FP8.
 
 &#160;
 
 ## Multi-GPU performance
 
 Thunder also supports distributed strategies such as DDP and FSDP for training models on multiple GPUs. The following plot displays the normalized throughput measured for Llama 2 7B without FP8 mixed precision; support for FSDP is in progress.
 
 <div align="center">
-<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240404/docs/source/_static/images/normalized_training_throughput_zero2.png" width="800px" style="max-width: 100%;">
+<img alt="Thunder" src="https://github.com/Lightning-AI/lightning-thunder/raw/0.2.0.dev20240407/docs/source/_static/images/normalized_training_throughput_zero2.png" width="800px" style="max-width: 100%;">
 </div>
 
 &#160;
 
 ## Get started
 
 The easiest way to get started with Thunder, requiring no extra installations or setups, is by using our [Zero to Thunder Tutorial Studio](https://lightning.ai/lightning-ai/studios/zero-to-thunder-tutorial).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-thunder Version: 0.2.0.dev20240404
+Metadata-Version: 2.1 Name: lightning-thunder Version: 0.2.0.dev20240407
 Summary: Lightning Thunder project. Home-page: https://github.com/Lightning-AI/
 lightning-thunder Download-URL: https://github.com/Lightning-AI/lightning-
 thunder Author: Lightning-AI et al Author-email: community@lightning.ai
 License: Apache 2.0 Project-URL: Bug Tracker, https://github.com/Lightning-AI/
 lightning-thunder/issues Project-URL: Documentation, https://lightning-
 thunder.rtfd.io/en/latest/ Project-URL: Source Code, https://github.com/
 Lightning-AI/lightning-thunder Keywords: deep learning,AI Classifier:
@@ -13,29 +13,29 @@
 License :: OSI Approved :: Apache Software License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Requires-Python: >=3.10, <3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 torch>=2.2.0 Requires-Dist: looseversion==1.3.0 Requires-Dist: lightning-
 utilities>=0.7.0 Requires-Dist: numpy<2,>=1.23.0 Requires-Dist: igraph>=0.10.4
 Requires-Dist: optree>=0.9.2 Requires-Dist: opt_einsum>=3.3.0 Requires-Dist:
-mpmath<1.4.0 Provides-Extra: test Requires-Dist: absl-py; extra == "test"
-Requires-Dist: coverage==7.4.4; extra == "test" Requires-Dist: einops; extra ==
-"test" Requires-Dist: expecttest==0.2.1; extra == "test" Requires-Dist:
-fdm==0.4.1; extra == "test" Requires-Dist: graphviz==0.20.1; extra == "test"
-Requires-Dist: hypothesis==6.100.0; extra == "test" Requires-Dist: jax;
+mpmath<1.4.0 Provides-Extra: notebooks Requires-Dist: ipython[all]==8.23.0;
+extra == "notebooks" Provides-Extra: test Requires-Dist: absl-py; extra ==
+"test" Requires-Dist: coverage==7.4.4; extra == "test" Requires-Dist: einops;
+extra == "test" Requires-Dist: expecttest==0.2.1; extra == "test" Requires-
+Dist: fdm==0.4.1; extra == "test" Requires-Dist: graphviz==0.20.1; extra ==
+"test" Requires-Dist: hypothesis==6.100.0; extra == "test" Requires-Dist: jax;
 (sys_platform == "linux" or sys_platform == "darwin") and extra == "test"
 Requires-Dist: jaxlib; (sys_platform == "linux" or sys_platform == "darwin")
 and extra == "test" Requires-Dist: jsonargparse; extra == "test" Requires-Dist:
 numpy; extra == "test" Requires-Dist: pandas; extra == "test" Requires-Dist:
 pytest-cov==4.1.0; extra == "test" Requires-Dist: pytest-random-order==1.1.1;
 extra == "test" Requires-Dist: pytest-timeout==2.2.0; extra == "test" Requires-
 Dist: pytest-timestamper==0.0.10; extra == "test" Requires-Dist: pytest-
 xdist==3.5.0; extra == "test" Requires-Dist: pytest==8.1.1; extra == "test"
-Requires-Dist: xlsxwriter; extra == "test" Provides-Extra: notebooks Requires-
-Dist: ipython[all]==8.23.0; extra == "notebooks"
+Requires-Dist: xlsxwriter; extra == "test"
                               [Thunder][Thunder]
 
                     **Make PyTorch models Lightning fast.**
     ______________________________________________________________________
    _L_i_g_h_t_n_i_n_g_._a_i â¢ _P_e_r_f_o_r_m_a_n_c_e â¢ _G_e_t_ _s_t_a_r_t_e_d â¢ _I_n_s_t_a_l_l â¢ _E_x_a_m_p_l_e_s â¢
               _I_n_s_i_d_e_ _T_h_u_n_d_e_r â¢ _G_e_t_ _i_n_v_o_l_v_e_d_! â¢ _D_o_c_u_m_e_n_t_a_t_i_o_n
 [![license](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https:
```

### Comparing `lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/SOURCES.txt` & `lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/lightning_thunder.egg-info/requires.txt` & `lightning-thunder-0.2.0.dev20240407/lightning_thunder.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/requirements/test.txt` & `lightning-thunder-0.2.0.dev20240407/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/setup.py` & `lightning-thunder-0.2.0.dev20240407/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/benchmark_litgpt.py` & `lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/benchmark_litgpt.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/distributed.py` & `lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/distributed.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/einsum.py` & `lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/einsum.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/targets.py` & `lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/targets.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/benchmarks/test_benchmark_litgpt.py` & `lightning-thunder-0.2.0.dev20240407/thunder/benchmarks/test_benchmark_litgpt.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/clang/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/clang/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/clang/langctx.py` & `lightning-thunder-0.2.0.dev20240407/thunder/clang/langctx.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/common.py` & `lightning-thunder-0.2.0.dev20240407/thunder/common.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/baseutils.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/baseutils.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/codeutils.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/codeutils.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/compile_data.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/compile_data.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/devices.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/devices.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/dtypes.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/dtypes.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/interpreter.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/interpreter.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/jit_ext.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/jit_ext.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/langctxs.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/langctxs.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/options.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/options.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/patterns.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/patterns.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/prims.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/prims.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/profile.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/profile.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/proxies.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/pytree.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/pytree.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/rematerialization.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/rematerialization.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/symbol.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/symbol.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/trace.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/trace.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/transform_common.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/transform_common.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/transforms.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/transforms.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/utils.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/core/vjp_utils.py` & `lightning-thunder-0.2.0.dev20240407/thunder/core/vjp_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/cudagraphs/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/cudagraphs/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/distributed/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/distributed/bucketing.py` & `lightning-thunder-0.2.0.dev20240407/thunder/distributed/bucketing.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/distributed/checkpoint.py` & `lightning-thunder-0.2.0.dev20240407/thunder/distributed/checkpoint.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/distributed/prims.py` & `lightning-thunder-0.2.0.dev20240407/thunder/distributed/prims.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/distributed/transforms/ddp.py` & `lightning-thunder-0.2.0.dev20240407/thunder/distributed/transforms/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/distributed/transforms/fsdp.py` & `lightning-thunder-0.2.0.dev20240407/thunder/distributed/transforms/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/distributed/utils.py` & `lightning-thunder-0.2.0.dev20240407/thunder/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/examine/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/examine/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/examine/memory_caculation.py` & `lightning-thunder-0.2.0.dev20240407/thunder/examine/memory_caculation.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/apex_entropyex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/apex_entropyex.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/cudnn_layernormex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/cudnn_layernormex.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/cudnnex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/cudnnex.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/data_dependent_partition.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/data_dependent_partition.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/nvfuserex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/nvfuserex.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/nvfuserex_impl.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/nvfuserex_impl.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/passes.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/passes.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/pythonex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/pythonex.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/sdpaex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/sdpaex.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/torch_autograd.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/torch_autograd.py`

 * *Files 2% similar despite different names*

```diff
@@ -321,14 +321,21 @@
             )
         if getattr(compile_data.fn, "sharding_strategy") == FSDPType.ZERO2:
             fw_extrace = sort_waits(fw_extrace)
             bw_extrace = sort_waits(bw_extrace)
     if getattr(compile_data.fn, "use_ddp", False):
         bw_extrace = sort_waits(bw_extrace)
 
+    # Importing here to avoid cyclical dependencies in future.
+    from thunder.executors.transformer_engineex import transformer_engine_ex, _rearrange_transformer_engine_linear
+
+    if transformer_engine_ex in compile_data.executors_list:
+        # NOTE: `_rearrange_transformer_engine_linear` mutates `fw_extrace`.
+        _rearrange_transformer_engine_linear(fw_extrace, bw_extrace)
+
     fw_extrace = del_last_used(fw_extrace)
     fw_traces.append(fw_extrace)
 
     bw_extrace = del_last_used(bw_extrace, clear_collections=True)
     bw_traces.append(bw_extrace)
 
     if compile_stats is not None:
```

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/torch_compile.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/torch_compile.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/torchex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/torchex.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/transformer_engineex.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/transformer_engineex.py`

 * *Files 14% similar despite different names*

```diff
@@ -428,7 +428,95 @@
 # Registers the implementation for torch.nn.functional.linear
 transformer_engine_ex.register_implementation(
     prims.linear,
     checker=_linear_checker,
     execution_transform=_linear_transform,
     grad_transform=_linear_grad,
 )
+
+
+def _rearrange_transformer_engine_linear(fw_extrace, bw_extrace):
+    """
+    Rearrange the TransformerEngine linear symbols `te_linear_*` in forward trace
+    so that we match the constraint that first FP8 module being called
+    in forward is the last FP8 module whose gradient is computed in backward pass.
+
+    Implementation:
+    From the backward trace, we find the `ctx_name` of the last `te_functional_linear_backward`.
+    Then we iterate the forward trace and find the `te_linear` which produces the `ctx_name`
+    found above. We move this `te_linear` above the first `te_linear` currently in the fwd_trace.
+
+    ..note::
+        We could have also done it such that we find the `ctx_name` for first `te_linear` in forward
+        and re-order the backward pass.
+        However, on a real model llama2.c example, I noticed that FusionExecutor can create pseudo dependency.
+        See the example below.
+
+    Details:
+    TransformerEngine takes care of syncing FP8 meta-data
+    in distributed setting (if world_size > 1). The way this is handled
+    is by marking the first FP8 module in forward pass. In the backward pass
+    of that module (last in FP8 module in backward), it collects all the FP8 state,
+    this state is concatenated, then synced acorss the processes and then split back
+    into individual state again.
+    Implementation of the above is in `prepare_forward` and `_prepare_backward` in
+    `transformer_engine/pytorch/module/base.py`
+    This means that in thunder, we can't reorder the first `te_linear` or the last backward.
+    However, FusionExecutors may reorder them.
+    This function takes care of rearranging such that adhere to this requirement.
+    Implementation of `prepare_forward`: https://github.com/NVIDIA/TransformerEngine/blob/2d0ab27f/transformer_engine/pytorch/module/base.py#L501
+    Implementation of `_prepare_backward : https://github.com/NVIDIA/TransformerEngine/blob/2d0ab27f/transformer_engine/pytorch/module/base.py#L67
+
+    Example:
+
+    Forward Trace Snippet:
+    [t22, t26] = nvFusion0(t16, t25)
+    (t77, ctx_te_2) = te_linear_2(t26, layers_0_attention_wv_weight, None)
+    (t53, ctx_te_1) = te_linear_1(t26, layers_0_attention_wk_weight, None)
+    (t29, ctx_te_0) = te_linear_0(t26, layers_0_attention_wq_weight, None)
+
+    Backward Trace Snippet (without the `del` for brevity):
+    NOTE: t6822 is part of nvFusion35 which also produces input for te_functional_linear_backward below it.
+    (t6821, t6822, _) = te_functional_linear_backward(t6819, (i443, i444, i445), (i446, i447), None, ctx_te_2)
+    NOTE: `nvFusion35` just does `true_divide(t6822, 2)` and returns it for synchronization.
+          but it also picks up a few operations which process the input for other `te_functional_linear_backward` below.
+    [t6823, t6857, t6900] = nvFusion35(f468, f476, i293, i294, i295, i296, i297, i432, i433, i434, i435, i436, t36, t38, t6810, t6812, t6822)
+    t6901 = torch.reshape(t6900, (i186, i187, i188, i189))  # t6901: "cuda:0 f32[128, 256, 6, 48]"
+    t6902 = torch.reshape(t6901, (i178, i179, i180))  # t6902: "cuda:0 f32[128, 256, 288]"
+    t6858 = torch.reshape(t6857, (i325, i326, i327, i328))  # t6858: "cuda:0 f32[128, 256, 6, 48]"
+    t6859 = torch.reshape(t6858, (i317, i318, i319))  # t6859: "cuda:0 f32[128, 256, 288]"
+    (t6904, t6905, _) = te_functional_linear_backward(t6902, (i165, i166, i167), (i168, i169), None, ctx_te_0)
+    (t6861, t6862, _) = te_functional_linear_backward(t6859, (i304, i305, i306), (i307, i308), None, ctx_te_1)
+    """
+    # Get the ctx name for the last `te_functional_linear_backward`.
+    bwd_bsym_ctx = None
+    for _, bsym in enumerate(reversed(bw_extrace.bound_symbols)):
+        if bsym.sym.id == te_functional_linear_backward.id:
+            bwd_bsym_ctx = bsym.args[-1].name
+            break
+
+    first_sym_idx = None
+    detected_first_sym_idx = None
+    # Find the first `te_linear` in forward trace
+    # and the position of `te_linear` which has the last `ctx_name`
+    # in backward.
+    for idx, bsym in enumerate(fw_extrace.bound_symbols):
+        # Forward symbols are generated on the fly so we don't
+        # have access here.
+        # Instead we check for the executor field.
+        if bsym.sym.executor == transformer_engine_ex:
+            # Sanity check.
+            assert "te_linear" in bsym.sym.name
+            if first_sym_idx is None:
+                first_sym_idx = idx
+            if bsym.output[-1].name == bwd_bsym_ctx:
+                detected_first_sym_idx = idx
+                break
+
+    # If the first `te_linear` is not same as that one that should be
+    # we move it to be the first one.
+    if detected_first_sym_idx != first_sym_idx:
+        # Move the symbol to be the first `te_linear`.
+        fwd_bsyms = fw_extrace.bound_symbols
+        sym_to_swap = fwd_bsyms[detected_first_sym_idx]
+        del fwd_bsyms[detected_first_sym_idx]
+        fwd_bsyms.insert(first_sym_idx, sym_to_swap)
```

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/triton_crossentropy_impl.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/triton_crossentropy_impl.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/executors/utils.py` & `lightning-thunder-0.2.0.dev20240407/thunder/executors/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/extend/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/functional.py` & `lightning-thunder-0.2.0.dev20240407/thunder/functional.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/numpy/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/numpy/langctx.py` & `lightning-thunder-0.2.0.dev20240407/thunder/numpy/langctx.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/torch/__init__.py` & `lightning-thunder-0.2.0.dev20240407/thunder/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-thunder-0.2.0.dev20240404/thunder/torch/langctx.py` & `lightning-thunder-0.2.0.dev20240407/thunder/torch/langctx.py`

 * *Files identical despite different names*

