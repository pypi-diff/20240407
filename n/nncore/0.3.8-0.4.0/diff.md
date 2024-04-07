# Comparing `tmp/nncore-0.3.8.tar.gz` & `tmp/nncore-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nncore-0.3.8.tar", last modified: Fri Jan 19 03:34:19 2024, max compression
+gzip compressed data, was "nncore-0.4.0.tar", last modified: Sun Apr  7 04:05:32 2024, max compression
```

## Comparing `nncore-0.3.8.tar` & `nncore-0.4.0.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.798695 nncore-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-01-19 03:34:09.000000 nncore-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-01-19 03:34:19.798695 nncore-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-01-19 03:34:09.000000 nncore-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.782695 nncore-0.3.8/nncore/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.782695 nncore-0.3.8/nncore/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/dataset/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/dataset/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.786695 nncore-0.3.8/nncore/engine/
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/builder.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9026 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/comm.py
--rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.786695 nncore-0.3.8/nncore/engine/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/closure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/lr_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/precise_bn.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/sampler_seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/hooks/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.786695 nncore-0.3.8/nncore/image/
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/image/colorspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/image/geometric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/image/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/image/normalize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.786695 nncore-0.3.8/nncore/io/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.790695 nncore-0.3.8/nncore/io/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/txt.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/handlers/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/io/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.790695 nncore-0.3.8/nncore/nn/
--rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.790695 nncore-0.3.8/nncore/nn/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/blocks/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/blocks/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/blocks/msg_pass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/blocks/norm.py
--rw-r--r--   0 runner    (1001) docker     (127)    30241 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/blocks/transformer.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.790695 nncore-0.3.8/nncore/nn/bundle/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/bundle/bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4969 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.790695 nncore-0.3.8/nncore/nn/losses/
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/losses/bce.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/losses/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/losses/focal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/losses/ghm.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/losses/lasso.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/losses/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.790695 nncore-0.3.8/nncore/nn/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/modules/conv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/modules/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/modules/msg_pass.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9821 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/nn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.794695 nncore-0.3.8/nncore/ops/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/ops/bbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/ops/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/ops/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.794695 nncore-0.3.8/nncore/optim/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/optim/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/optim/lamb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.794695 nncore-0.3.8/nncore/parallel/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/parallel/collate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/parallel/container.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/parallel/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.794695 nncore-0.3.8/nncore/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/binder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.794695 nncore-0.3.8/nncore/video/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-01-19 03:34:09.000000 nncore-0.3.8/nncore/video/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.798695 nncore-0.3.8/nncore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-01-19 03:34:19.000000 nncore-0.3.8/nncore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2590 2024-01-19 03:34:19.000000 nncore-0.3.8/nncore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 03:34:19.000000 nncore-0.3.8/nncore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-19 03:34:19.000000 nncore-0.3.8/nncore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-19 03:34:19.000000 nncore-0.3.8/nncore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-01-19 03:34:19.798695 nncore-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-01-19 03:34:09.000000 nncore-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 03:34:19.798695 nncore-0.3.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_binder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-19 03:34:09.000000 nncore-0.3.8/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-07 04:05:22.000000 nncore-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-07 04:05:32.316973 nncore-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-07 04:05:22.000000 nncore-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.300973 nncore-0.4.0/nncore/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.300973 nncore-0.4.0/nncore/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/dataset/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.300973 nncore-0.4.0/nncore/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/builder.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9026 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/comm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21687 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/engine/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/closure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/lr_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/precise_bn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/sampler_seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/hooks/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8474 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/colorspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/geometric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/image/normalize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/io/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.304973 nncore-0.4.0/nncore/io/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/txt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/handlers/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/io/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/msg_pass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/norm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30450 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/blocks/transformer.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4505 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/bundle/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/bundle/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.308973 nncore-0.4.0/nncore/nn/losses/
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/bce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7660 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/focal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/ghm.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6311 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/lasso.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/losses/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/nn/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6078 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/conv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/modules/msg_pass.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9821 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/nn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/ops/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/optim/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/optim/lamb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.312973 nncore-0.4.0/nncore/parallel/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/collate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/parallel/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/nncore/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14654 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/nncore/video/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-07 04:05:22.000000 nncore-0.4.0/nncore/video/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/nncore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-07 04:05:32.000000 nncore-0.4.0/nncore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-07 04:05:32.316973 nncore-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-07 04:05:22.000000 nncore-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 04:05:32.316973 nncore-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_binder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-04-07 04:05:22.000000 nncore-0.4.0/tests/test_registry.py
```

### Comparing `nncore-0.3.8/LICENSE` & `nncore-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/PKG-INFO` & `nncore-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nncore
-Version: 0.3.8
+Version: 0.4.0
 Summary: A lightweight machine learning toolkit for researchers.
 Home-page: https://github.com/yeliudev/nncore
 Author: Ye Liu
 Author-email: yeliudev@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py>=3.1
 Requires-Dist: joblib>=1.1
 Requires-Dist: jsonlines>=2
 Requires-Dist: numpy>=1.19
 Requires-Dist: pyyaml>=6
+Requires-Dist: requests>=2.31
 Requires-Dist: tabulate>=0.8
 Requires-Dist: tensorboard>=2.12
 Requires-Dist: termcolor>=1.1
 Requires-Dist: opencv-python>=4.5
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: nncore Version: 0.3.8 Summary: A lightweight
+Metadata-Version: 2.1 Name: nncore Version: 0.4.0 Summary: A lightweight
 machine learning toolkit for researchers. Home-page: https://github.com/
 yeliudev/nncore Author: Ye Liu Author-email: yeliudev@outlook.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: h5py>=3.1 Requires-Dist: joblib>=1.1 Requires-Dist: jsonlines>=2
 Requires-Dist: numpy>=1.19 Requires-Dist: pyyaml>=6 Requires-Dist:
-tabulate>=0.8 Requires-Dist: tensorboard>=2.12 Requires-Dist: termcolor>=1.1
-Requires-Dist: opencv-python>=4.5
+requests>=2.31 Requires-Dist: tabulate>=0.8 Requires-Dist: tensorboard>=2.12
+Requires-Dist: termcolor>=1.1 Requires-Dist: opencv-python>=4.5
    [https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg]
                              ************ NNNNCCoorree ************
             AA lliigghhttwweeiigghhtt mmaacchhiinnee lleeaarrnniinngg ttoooollkkiitt ffoorr rreesseeaarrcchheerrss..
   _[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_p_y_p_i_/_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_P_y_P_I_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
 _p_y_p_i_/_d_m_/_n_n_c_o_r_e_?_l_a_b_e_l_=_D_o_w_n_l_o_a_d_s_&_c_o_l_o_r_=_c_y_a_n_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/
 _l_i_c_e_n_s_e_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_c_o_v_e_r_a_l_l_s_/
   _c_/_g_i_t_h_u_b_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_/_m_a_i_n_?_l_a_b_e_l_=_C_o_v_e_r_a_g_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
```

### Comparing `nncore-0.3.8/README.md` & `nncore-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/dataset/builder.py` & `nncore-0.4.0/nncore/dataset/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/dataset/wrapper.py` & `nncore-0.4.0/nncore/dataset/wrapper.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/__init__.py` & `nncore-0.4.0/nncore/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/buffer.py` & `nncore-0.4.0/nncore/engine/buffer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/builder.py` & `nncore-0.4.0/nncore/engine/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/comm.py` & `nncore-0.4.0/nncore/engine/comm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/engine.py` & `nncore-0.4.0/nncore/engine/engine.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/__init__.py` & `nncore-0.4.0/nncore/engine/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/base.py` & `nncore-0.4.0/nncore/engine/hooks/base.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/checkpoint.py` & `nncore-0.4.0/nncore/engine/hooks/checkpoint.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/closure.py` & `nncore-0.4.0/nncore/engine/hooks/closure.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/eval.py` & `nncore-0.4.0/nncore/engine/hooks/eval.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/lr_updater.py` & `nncore-0.4.0/nncore/engine/hooks/lr_updater.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/memory.py` & `nncore-0.4.0/nncore/engine/hooks/memory.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/optimizer.py` & `nncore-0.4.0/nncore/engine/hooks/optimizer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/precise_bn.py` & `nncore-0.4.0/nncore/engine/hooks/precise_bn.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/timer.py` & `nncore-0.4.0/nncore/engine/hooks/timer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/hooks/writer.py` & `nncore-0.4.0/nncore/engine/hooks/writer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/engine/utils.py` & `nncore-0.4.0/nncore/engine/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/image/__init__.py` & `nncore-0.4.0/nncore/image/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/image/colorspace.py` & `nncore-0.4.0/nncore/image/colorspace.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/image/geometric.py` & `nncore-0.4.0/nncore/image/geometric.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/image/io.py` & `nncore-0.4.0/nncore/image/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/image/normalize.py` & `nncore-0.4.0/nncore/image/normalize.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/base.py` & `nncore-0.4.0/nncore/io/handlers/base.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/hdf5.py` & `nncore-0.4.0/nncore/io/handlers/hdf5.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/json.py` & `nncore-0.4.0/nncore/io/handlers/json.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/numpy.py` & `nncore-0.4.0/nncore/io/handlers/numpy.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/pickle.py` & `nncore-0.4.0/nncore/io/handlers/pickle.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/txt.py` & `nncore-0.4.0/nncore/io/handlers/txt.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/xml.py` & `nncore-0.4.0/nncore/io/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/handlers/yaml.py` & `nncore-0.4.0/nncore/io/handlers/yaml.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/io/io.py` & `nncore-0.4.0/nncore/io/io.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     'pickle': PickleHandler(),
     'pkl': PickleHandler(),
     'hdf5': HDF5Handler(),
     'h5': HDF5Handler(),
     'npy': NumPyHandler(),
     'npz': NumPyzHandler(),
     'xml': XMLHandler(),
-    'txt': TXTHandler()
+    'txt': TXTHandler(),
+    'sh': TXTHandler()
 }
 
 _open = open
 
 
 def _get_handler(format):
     if format not in _FILE_HANDLERS:
```

### Comparing `nncore-0.3.8/nncore/nn/__init__.py` & `nncore-0.4.0/nncore/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/blocks/__init__.py` & `nncore-0.4.0/nncore/nn/blocks/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright (c) Ye Liu. Licensed under the MIT License.
 
 from .activation import Clamp
 from .conv import *  # noqa
 from .msg_pass import GAT, GCN, SGC
 from .norm import DropPath, drop_path
+from .scale import Scale, Gate
 from .transformer import (CrossAttentionLayer, FeedForwardNetwork,
                           MultiHeadAttention, PositionalEncoding,
                           TransformerDecoderLayer, TransformerEncoderLayer)
 
 __all__ = [
-    'Clamp', 'GAT', 'GCN', 'SGC', 'DropPath', 'drop_path',
+    'Clamp', 'GAT', 'GCN', 'SGC', 'DropPath', 'drop_path', 'Scale', 'Gate',
     'CrossAttentionLayer', 'FeedForwardNetwork', 'MultiHeadAttention',
     'PositionalEncoding', 'TransformerDecoderLayer', 'TransformerEncoderLayer'
 ]
```

### Comparing `nncore-0.3.8/nncore/nn/blocks/activation.py` & `nncore-0.4.0/nncore/nn/blocks/activation.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/blocks/conv.py` & `nncore-0.4.0/nncore/nn/blocks/conv.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/blocks/msg_pass.py` & `nncore-0.4.0/nncore/nn/blocks/msg_pass.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/blocks/norm.py` & `nncore-0.4.0/nncore/nn/blocks/norm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/blocks/transformer.py` & `nncore-0.4.0/nncore/nn/blocks/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -236,27 +236,27 @@
         ffn_dropout (float, optional): Dropout probability for hidden layers.
             Default: ``0.0``.
         out_dropout (float, optional): Dropout probability for outputs.
             Default: ``0.0``.
         act_cfg (dict | str | None, optional): The config or name of the
             activation layer. Default: ``dict(type='ReLU', inplace=True)``.
         init_cfg (dict | str | None, optional): The initialization config for
-            linear layers. Default: ``None``.
+            linear layers. Default: ``dict(type='kaiming')``.
 
     References:
         1. Vaswani et al. (https://arxiv.org/abs/1706.03762)
     """
 
     def __init__(self,
                  dims,
                  ratio=4,
                  ffn_dropout=0.0,
                  out_dropout=0.0,
                  act_cfg=dict(type='ReLU', inplace=True),
-                 init_cfg=None):
+                 init_cfg=dict(type='kaiming')):
         super(FeedForwardNetwork, self).__init__()
 
         self._dims = dims
         self._ratio = ratio
         self._ffn_dropout = ffn_dropout
         self._out_dropout = out_dropout
         self._h_dims = int(dims * ratio)
@@ -325,15 +325,16 @@
         order (tuple[str], optional): The order of sub-modules. This argument
             should be a sequence of `'self_att'` and `'ffn'`.
             Default: `('self_att', 'ffn')`.
         att_init_cfg (dict | str | None, optional): The initialization config
             for qkv projection layers in the attention block. Default:
             ``dict(type='xavier', distribution='uniform')``.
         ffn_init_cfg (dict | str | None, optional): The initialization config
-            for linear layers in the feed forward network. Default: ``None``.
+            for linear layers in the feed forward network. Default:
+            ``dict(type='kaiming')``.
 
     References:
         1. Vaswani et al. (https://arxiv.org/abs/1706.03762)
     """
 
     def __init__(self,
                  dims,
@@ -346,19 +347,19 @@
                  droppath=0.1,
                  pre_norm=True,
                  bias=True,
                  norm_cfg=dict(type='LN'),
                  act_cfg=dict(type='ReLU', inplace=True),
                  order=('self_att', 'ffn'),
                  att_init_cfg=dict(type='xavier', distribution='uniform'),
-                 ffn_init_cfg=None):
+                 ffn_init_cfg=dict(type='kaiming')):
         super(TransformerEncoderLayer, self).__init__()
 
-        order_set = set(order)
-        assert order_set.issubset(('self_att', 'ffn'))
+        assert all(o in ('self_att', 'ffn') for o in order)
+        assert len(order) == len(set(order))
 
         self._dims = dims
         self._heads = heads
         self._ratio = ratio
         self._att_dropout = att_dropout
         self._ffn_dropout = ffn_dropout
         self._att_out_dropout = att_out_dropout
@@ -366,15 +367,15 @@
         self._droppath = droppath
         self._pre_norm = pre_norm
         self._bias = bias
         self._order = order
         self._att_init_cfg = att_init_cfg
         self._ffn_init_cfg = ffn_init_cfg
 
-        for name in order_set:
+        for name in order:
             if name == 'self_att':
                 self.self_att = MultiHeadAttention(
                     dims,
                     heads=heads,
                     att_dropout=att_dropout,
                     out_dropout=att_out_dropout,
                     bias=bias,
@@ -460,15 +461,16 @@
         order (tuple[str], optional): The order of sub-modules. This argument
             should be a sequence of `'self_att'`, `'cross_att'`, and `'ffn'`.
             Default: `('self_att', 'cross_att', 'ffn')`.
         att_init_cfg (dict | str | None, optional): The initialization config
             for qkv projection layers in the attention block. Default:
             ``dict(type='xavier', distribution='uniform')``.
         ffn_init_cfg (dict | str | None, optional): The initialization config
-            for linear layers in the feed forward network. Default: ``None``.
+            for linear layers in the feed forward network. Default:
+            ``dict(type='kaiming')``.
 
     References:
         1. Vaswani et al. (https://arxiv.org/abs/1706.03762)
     """
 
     def __init__(self,
                  dims,
@@ -481,19 +483,19 @@
                  droppath=0.1,
                  pre_norm=True,
                  bias=True,
                  norm_cfg=dict(type='LN'),
                  act_cfg=dict(type='ReLU', inplace=True),
                  order=('self_att', 'cross_att', 'ffn'),
                  att_init_cfg=dict(type='xavier', distribution='uniform'),
-                 ffn_init_cfg=None):
+                 ffn_init_cfg=dict(type='kaiming')):
         super(TransformerDecoderLayer, self).__init__()
 
-        order_set = set(order)
-        assert order_set.issubset(('self_att', 'cross_att', 'ffn'))
+        assert all(o in ('self_att', 'cross_att', 'ffn') for o in order)
+        assert len(order) == len(set(order))
 
         self._dims = dims
         self._heads = heads
         self._ratio = ratio
         self._att_dropout = att_dropout
         self._ffn_dropout = ffn_dropout
         self._att_out_dropout = att_out_dropout
@@ -501,15 +503,15 @@
         self._droppath = droppath
         self._pre_norm = pre_norm
         self._bias = bias
         self._order = order
         self._att_init_cfg = att_init_cfg
         self._ffn_init_cfg = ffn_init_cfg
 
-        for name in order_set:
+        for name in order:
             if name == 'self_att':
                 self.self_att = MultiHeadAttention(
                     dims,
                     heads=heads,
                     att_dropout=att_dropout,
                     out_dropout=att_out_dropout,
                     bias=bias,
@@ -619,15 +621,16 @@
         order (tuple[str], optional): The order of sub-modules. This argument
             should be a sequence of `'cross_att'` and `'ffn'`.
             Default: `('cross_att', 'ffn')`.
         att_init_cfg (dict | str | None, optional): The initialization config
             for qkv projection layers in the attention block. Default:
             ``dict(type='xavier', distribution='uniform')``.
         ffn_init_cfg (dict | str | None, optional): The initialization config
-            for linear layers in the feed forward network. Default: ``None``.
+            for linear layers in the feed forward network. Default:
+            ``dict(type='kaiming')``.
     """
 
     def __init__(self,
                  dims,
                  heads=8,
                  ratio=4,
                  att_dropout=0.0,
@@ -637,19 +640,19 @@
                  droppath=0.1,
                  pre_norm=True,
                  bias=True,
                  norm_cfg=dict(type='LN'),
                  act_cfg=dict(type='ReLU', inplace=True),
                  order=('cross_att', 'ffn'),
                  att_init_cfg=dict(type='xavier', distribution='uniform'),
-                 ffn_init_cfg=None):
+                 ffn_init_cfg=dict(type='kaiming')):
         super(CrossAttentionLayer, self).__init__()
 
-        order_set = set(order)
-        assert order_set.issubset(('cross_att', 'ffn'))
+        assert all(o in ('cross_att', 'ffn') for o in order)
+        assert len(order) == len(set(order))
 
         self._dims = dims
         self._heads = heads
         self._ratio = ratio
         self._att_dropout = att_dropout
         self._ffn_dropout = ffn_dropout
         self._att_out_dropout = att_out_dropout
@@ -657,15 +660,15 @@
         self._droppath = droppath
         self._pre_norm = pre_norm
         self._bias = bias
         self._order = order
         self._att_init_cfg = att_init_cfg
         self._ffn_init_cfg = ffn_init_cfg
 
-        for name in order_set:
+        for name in order:
             if name == 'cross_att':
                 self.b_to_a_att = MultiHeadAttention(
                     dims,
                     heads=heads,
                     att_dropout=att_dropout,
                     out_dropout=att_out_dropout,
                     bias=bias,
```

### Comparing `nncore-0.3.8/nncore/nn/builder.py` & `nncore-0.4.0/nncore/nn/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/bundle/bundle.py` & `nncore-0.4.0/nncore/nn/bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/init.py` & `nncore-0.4.0/nncore/nn/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,27 +80,27 @@
     if hasattr(module, 'bias') and module.bias is not None:
         nn.init.constant_(module.bias, bias)
 
 
 @INITIALIZERS.register(name='kaiming')
 def kaiming_init_(module,
                   a=0,
-                  mode='fan_in',
+                  mode='fan_out',
                   nonlinearity='leaky_relu',
                   bias=0,
                   distribution='normal'):
     """
     Initialize a module using the method introduced in [1].
 
     Args:
         module (:obj:`nn.Module`): The module to be initialized.
         a (int, optional): The negative slope of ``LeakyReLU``. Default: ``0``.
         mode (str, optional): The direction of pass whose magnitude of the
             variance of the weights are preserved. Expected values include
-            ``'fan_in'`` and ``'fan_out'``. Default: ``'fan_in'``.
+            ``'fan_in'`` and ``'fan_out'``. Default: ``'fan_out'``.
         nonlinearity (str, optional): The nonlinearity after the parameterized
             layers. The expected values are ``'relu'`` and ``'leaky_relu'``.
             Default: ``'leaky_relu'``.
         bias (int, optional): The bias of the module. Default: ``0``.
         distribution (str, optional): The type of distribution to use.
             Expected values include ``normal`` and ``uniform``. Default:
             ``'normal'``.
```

### Comparing `nncore-0.3.8/nncore/nn/losses/__init__.py` & `nncore-0.4.0/nncore/nn/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/losses/bce.py` & `nncore-0.4.0/nncore/nn/losses/bce.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/losses/contrastive.py` & `nncore-0.4.0/nncore/nn/losses/contrastive.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,108 @@
 # Copyright (c) Ye Liu. Licensed under the MIT License.
 
 import math
 
 import torch
+import torch.distributed as dist
 import torch.nn as nn
 import torch.nn.functional as F
 
 import nncore
+from nncore.engine import comm
 from nncore.ops import cosine_similarity
 from ..builder import LOSSES
 from ..bundle import Parameter
 from .utils import weighted_loss
 
 
+class _AllGather(torch.autograd.Function):
+
+    @staticmethod
+    def forward(ctx, tensor, group=None):
+        rank, world_size = comm.get_dist_info()
+
+        ctx.size = tensor.size(-2)
+        ctx.rank = rank
+        ctx.group = group
+
+        gathered = [torch.zeros_like(tensor) for _ in range(world_size)]
+        dist.all_gather(gathered, tensor, group=group)
+
+        gathered = torch.cat(gathered, dim=-2)
+        return gathered
+
+    @staticmethod
+    def backward(ctx, grad):
+        grad = grad.contiguous()
+        dist.all_reduce(grad, op=dist.ReduceOp.SUM, group=ctx.group)
+        return grad[..., ctx.size * ctx.rank:ctx.size * (ctx.rank + 1), :]
+
+
 @weighted_loss
-def infonce_loss(a, b, temperature=0.07, scale=None, max_scale=100):
+def infonce_loss(a,
+                 b,
+                 temperature=0.07,
+                 scale=None,
+                 max_scale=100,
+                 dist=False,
+                 group=None):
     """
     InfoNCE Loss introduced in [1].
 
     Args:
         a (:obj:`torch.Tensor`): The first group of samples.
         b (:obj:`torch.Tensor`): The second group of samples.
         temperature (float, optional): The temperature for softmax. Default:
             ``0.07``.
         scale (:obj:`torch.Tensor` | None, optional): The logit scale to use.
             If not specified, the scale will be calculated from temperature.
             Default: ``None``.
         max_scale (float, optional): The maximum logit scale value. Default:
             ``100``.
+        dist (bool, optional): Whether the loss is computed across processes.
+            Default: ``False``.
+        group (:obj:`dist.ProcessGroup` | None, optional): The process group
+            to use. If not specified, the default process group will be used.
+            Default: ``None``.
 
     References:
         1. Oord et al. (https://arxiv.org/abs/1807.03748)
     """
     a = F.normalize(a, dim=-1)
     b = F.normalize(b, dim=-1)
 
     if scale is None:
         scale = a.new_tensor([math.log(1 / temperature)])
 
     scale = scale.exp().clamp(max=max_scale)
-    a_sim = torch.matmul(a, b.transpose(-1, -2)) * scale
-    b_sim = a_sim.transpose(-1, -2)
 
-    target = torch.arange(a.size(-2), device=a.device).expand(a.size()[:-1])
-    a_loss = F.cross_entropy(a_sim, target)
-    b_loss = F.cross_entropy(b_sim, target)
+    n = a.size(-2)
+    t = torch.arange(n, device=a.device)
+
+    if dist and comm.is_distributed():
+        rank = comm.get_rank(group=group)
+
+        s, e = n * rank, n * (rank + 1)
+        t += s
+
+        a = _AllGather.apply(a)
+        b = _AllGather.apply(b)
+
+        a_sim = torch.matmul(a[..., s:e, :], b.transpose(-1, -2)) * scale
+        b_sim = torch.matmul(b[..., s:e, :], a.transpose(-1, -2)) * scale
+    else:
+        a_sim = torch.matmul(a, b.transpose(-1, -2)) * scale
+        b_sim = a_sim.transpose(-1, -2).contiguous()
+
+    a_sim = a_sim.view(-1, a_sim.size(-1))
+    b_sim = b_sim.view(-1, b_sim.size(-1))
+
+    a_loss = F.cross_entropy(a_sim, t.repeat(int(a_sim.size(0) / n)))
+    b_loss = F.cross_entropy(b_sim, t.repeat(int(b_sim.size(0) / n)))
 
     loss = (a_loss + b_loss) / 2
     return loss
 
 
 @weighted_loss
 def triplet_loss(pos, neg, anchor, margin=0.5):
@@ -80,50 +134,54 @@
 
     Args:
         temperature (float, optional): The initial temperature for softmax.
             Default: ``0.07``.
         max_scale (float, optional): The maximum value of learnable scale.
             Default: ``100``.
         learnable (bool, optional): Whether the logit scale is learnable.
-            Default: ``True``.
+            Default: ``False``.
         loss_weight (float, optional): Weight of the loss. Default: ``1.0``.
 
     References:
         1. Oord et al. (https://arxiv.org/abs/1807.03748)
     """
 
     def __init__(self,
                  temperature=0.07,
                  max_scale=100,
-                 learnable=True,
+                 learnable=False,
+                 dist=False,
                  loss_weight=1.0):
         super(InfoNCELoss, self).__init__()
 
         if learnable:
             self.scale = Parameter(math.log(1 / temperature))
         else:
             self.scale = None
 
         self._temperature = temperature
         self._max_scale = max_scale
         self._learnable = learnable
+        self._dist = dist
         self._loss_weight = loss_weight
 
     def extra_repr(self):
-        return ('temperature={}, max_scale={}, learnable={}, loss_weight={}'.
-                format(self._temperature, self._max_scale, self._learnable,
-                       self._loss_weight))
+        return ('temperature={}, max_scale={}, learnable={}, dist={}, '
+                'loss_weight={}'.format(self._temperature, self._max_scale,
+                                        self._learnable, self._dist,
+                                        self._loss_weight))
 
     def forward(self, a, b, weight=None, avg_factor=None):
         return infonce_loss(
             a,
             b,
             temperature=self._temperature,
             scale=self.scale,
             max_scale=self._max_scale,
+            dist=self._dist,
             weight=weight,
             avg_factor=avg_factor) * self._loss_weight
 
 
 @LOSSES.register()
 @nncore.bind_getter('margin', 'reduction', 'loss_weight')
 class TripletLoss(nn.Module):
@@ -142,15 +200,15 @@
         super(TripletLoss, self).__init__()
 
         self._margin = margin
         self._reduction = reduction
         self._loss_weight = loss_weight
 
     def extra_repr(self):
-        return 'margin={}, reduction={}, loss_weight={}'.format(
+        return "margin={}, reduction='{}', loss_weight={}".format(
             self._margin, self._reduction, self._loss_weight)
 
     def forward(self, pos, neg, anchor, weight=None, avg_factor=None):
         return triplet_loss(
             pos,
             neg,
             anchor,
```

### Comparing `nncore-0.3.8/nncore/nn/losses/focal.py` & `nncore-0.4.0/nncore/nn/losses/focal.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/losses/ghm.py` & `nncore-0.4.0/nncore/nn/losses/ghm.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/losses/lasso.py` & `nncore-0.4.0/nncore/nn/losses/lasso.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/losses/utils.py` & `nncore-0.4.0/nncore/nn/losses/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/modules/conv.py` & `nncore-0.4.0/nncore/nn/modules/conv.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/modules/linear.py` & `nncore-0.4.0/nncore/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/modules/msg_pass.py` & `nncore-0.4.0/nncore/nn/modules/msg_pass.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/nn/utils.py` & `nncore-0.4.0/nncore/nn/utils.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/ops/__init__.py` & `nncore-0.4.0/nncore/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/ops/bbox.py` & `nncore-0.4.0/nncore/ops/bbox.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/ops/matrix.py` & `nncore-0.4.0/nncore/ops/matrix.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/ops/temporal.py` & `nncore-0.4.0/nncore/ops/temporal.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/optim/builder.py` & `nncore-0.4.0/nncore/optim/builder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/optim/lamb.py` & `nncore-0.4.0/nncore/optim/lamb.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/parallel/collate.py` & `nncore-0.4.0/nncore/parallel/collate.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/parallel/container.py` & `nncore-0.4.0/nncore/parallel/container.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/parallel/parallel.py` & `nncore-0.4.0/nncore/parallel/parallel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # Copyright (c) Ye Liu. Licensed under the MIT License.
 
 import torch
 from torch.nn.parallel import DataParallel, DistributedDataParallel
-from torch.nn.parallel._functions import Function, Scatter, _get_stream
+from torch.nn.parallel._functions import Scatter, _get_stream
 from torch.nn.parallel.scatter_gather import _is_namedtuple
 
+import nncore
 from .container import DataContainer
 
 
-class _Scatter(Function):
+class _Scatter(torch.autograd.Function):
 
     @staticmethod
     def forward(target_gpus, input):
         input_device = _get_input_device(input)
         streams = None
         if input_device == -1 and target_gpus != [-1]:
             streams = [
                 _get_stream(torch.device('cuda', gpu_id))
                 for gpu_id in target_gpus
             ]
-
         outputs = _scatter_stream(input, target_gpus, streams)
         if streams is not None:
             _sync_stream(outputs, target_gpus, streams)
-
         return tuple(outputs)
 
 
 def _get_input_device(input):
     if isinstance(input, list):
         for item in input:
             input_device = _get_input_device(item)
@@ -39,15 +38,14 @@
     else:
         raise TypeError('unknown type {}'.format(type(input)))
 
 
 def _scatter_stream(input, devices, streams=None):
     if streams is None:
         streams = [None] * len(devices)
-
     if isinstance(input, list):
         chunk_size = (len(input) - 1) // len(devices) + 1
         outputs = [
             _scatter_stream(input[i], [devices[i // chunk_size]],
                             [streams[i // chunk_size]])
             for i in range(len(input))
         ]
@@ -79,24 +77,19 @@
     else:
         raise TypeError('unknown type {}'.format(type(output)))
 
 
 def _scatter(inputs, target_gpus, dim=0):
 
     def _scatter_map(obj):
-        if torch.is_tensor(obj):
-            if target_gpus != [-1]:
-                return Scatter.apply(target_gpus, None, dim, obj)
-            else:
-                return _Scatter.forward(target_gpus, obj)
+        if torch.is_tensor(obj) and target_gpus != [-1]:
+            return Scatter.apply(target_gpus, None, dim, obj)
         if isinstance(obj, DataContainer):
-            if obj.cpu_only:
-                return obj.data
-            else:
-                return _Scatter.forward(target_gpus, obj.data)
+            return obj.data if obj.cpu_only else _Scatter.forward(
+                target_gpus, obj.data)
         if _is_namedtuple(obj):
             return [type(obj)(*args) for args in zip(*map(_scatter_map, obj))]
         if isinstance(obj, tuple) and len(obj) > 0:
             return list(zip(*map(_scatter_map, obj)))
         if isinstance(obj, list) and len(obj) > 0:
             return [list(i) for i in zip(*map(_scatter_map, obj))]
         if isinstance(obj, dict) and len(obj) > 0:
@@ -117,27 +110,56 @@
     if len(inputs) < len(kwargs):
         inputs.extend(() for _ in range(len(kwargs) - len(inputs)))
     elif len(kwargs) < len(inputs):
         kwargs.extend({} for _ in range(len(inputs) - len(kwargs)))
     return tuple(inputs), tuple(kwargs)
 
 
+def _get_device(device_id=None):
+    if device_id is not None:
+        return device_id
+    if torch.cuda.is_available():
+        return torch.cuda.current_device()
+    return -1
+
+
 class NNDataParallel(DataParallel):
     """
     A :obj:`nn.DataParallel` class with :obj:`DataContainer` support. This
     class only bundles single-device modules.
+
+    Args:
+        module (:obj:`nn.Module`): The module to be bundled.
+        device_id (int | None, optional): The device id to be used. ``None``
+            means using the default device, and ``-1`` means CPU. Default:
+            ``None``.
     """
 
-    def __init__(self, module, device_ids=None, dim=0, **kwargs):
-        assert device_ids is None or len(device_ids) <= 1
-        super(NNDataParallel, self).__init__(
-            module,
-            device_ids=[0] if device_ids is None else device_ids,
-            **kwargs)
-        self.dim = dim
+    def __init__(self, module, device_id=None, dim=0, **kwargs):
+        assert isinstance(device_id, int) or device_id is None
+        assert 'device_ids' not in kwargs and 'output_device' not in kwargs
+
+        device_id = _get_device(device_id)
+
+        if device_id >= 0:
+            super(NNDataParallel, self).__init__(
+                module,
+                device_ids=[device_id],
+                output_device=device_id,
+                **kwargs)
+        else:
+            logger = nncore.get_logger()
+            logger.warn('{} is running on CPU'.format(self.__class__.__name__))
+
+            super(DataParallel, self).__init__()
+            torch._C._log_api_usage_once('torch.nn.parallel.DataParallel')
+
+            self.module = module
+            self.device_ids = []
+            self.dim = dim
 
     def scatter(self, inputs, kwargs, device_ids):
         return _scatter_kwargs(inputs, kwargs, device_ids, dim=self.dim)
 
     def forward(self, *inputs, **kwargs):
         if self.device_ids:
             return super(NNDataParallel, self).forward(*inputs, **kwargs)
@@ -146,50 +168,45 @@
             return self.module(*inputs[0], **kwargs[0])
 
 
 class NNDistributedDataParallel(DistributedDataParallel):
     """
     A :obj:`nn.DistributedDataParallel` class with :obj:`DataContainer`
     support. This class only bundles single-device modules.
+
+    Args:
+        module (:obj:`nn.Module`): The module to be bundled.
+        device_id (int | None, optional): The device id to be used. ``None``
+            means using the default device, and ``-1`` means CPU. Default:
+            ``None``.
     """
 
-    def __init__(self,
-                 module,
-                 device_ids=None,
-                 broadcast_buffers=False,
-                 **kwargs):
-        assert device_ids is None or len(device_ids) <= 1
-
-        if device_ids is None:
-            if torch.cuda.is_available():
-                device_ids = [torch.cuda.current_device()]
-                module = module.cuda()
-        elif len(device_ids) == 1:
-            module = module.to('cuda:{}'.format(device_ids[0]))
+    def __init__(self, module, device_id=None, **kwargs):
+        assert isinstance(device_id, int) or device_id is None
+        assert 'device_ids' not in kwargs and 'output_device' not in kwargs
+
+        device_id = _get_device(device_id)
+
+        if device_id >= 0:
+            module = module.to('cuda:{}'.format(device_id))
+            device_ids = [device_id]
+        else:
+            logger = nncore.get_logger()
+            logger.warn('{} is running on CPU'.format(self.__class__.__name__))
+            device_ids = None
 
         super(NNDistributedDataParallel, self).__init__(
-            module,
-            device_ids=device_ids,
-            broadcast_buffers=broadcast_buffers,
-            **kwargs)
-
-    def _run_ddp_forward(self, *inputs, **kwargs):
-        if self._use_replicated_tensor_module:
-            module = self._replicated_tensor_module
-        else:
-            module = self.module
+            module, device_ids=device_ids, **kwargs)
 
+    def _pre_forward(self, *inputs, **kwargs):
         if self.device_ids:
-            inputs, kwargs = _scatter_kwargs(
-                inputs, kwargs, self.device_ids, dim=self.dim)
-            with self._inside_ddp_forward():
-                return module(*inputs[0], **kwargs[0])
-        else:
-            with self._inside_ddp_forward():
-                return module(*inputs, **kwargs)
+            inputs, kwargs = self.scatter(inputs, kwargs, self.device_ids)
+            inputs, kwargs = inputs[0], kwargs[0]
+        return super(NNDistributedDataParallel,
+                     self)._pre_forward(*inputs, **kwargs)
 
     def scatter(self, inputs, kwargs, device_ids):
         return _scatter_kwargs(inputs, kwargs, device_ids, dim=self.dim)
 
     def forward(self, *inputs, **kwargs):
         if self.device_ids:
             return super(NNDistributedDataParallel,
```

### Comparing `nncore-0.3.8/nncore/utils/__init__.py` & `nncore-0.4.0/nncore/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/binder.py` & `nncore-0.4.0/nncore/utils/binder.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/config.py` & `nncore-0.4.0/nncore/utils/config.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/data.py` & `nncore-0.4.0/nncore/utils/data.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/env.py` & `nncore-0.4.0/nncore/utils/env.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/logger.py` & `nncore-0.4.0/nncore/utils/logger.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/misc.py` & `nncore-0.4.0/nncore/utils/misc.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/network.py` & `nncore-0.4.0/nncore/utils/network.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/path.py` & `nncore-0.4.0/nncore/utils/path.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/progress.py` & `nncore-0.4.0/nncore/utils/progress.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/registry.py` & `nncore-0.4.0/nncore/utils/registry.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/utils/timer.py` & `nncore-0.4.0/nncore/utils/timer.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore/video/io.py` & `nncore-0.4.0/nncore/video/io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/nncore.egg-info/PKG-INFO` & `nncore-0.4.0/nncore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nncore
-Version: 0.3.8
+Version: 0.4.0
 Summary: A lightweight machine learning toolkit for researchers.
 Home-page: https://github.com/yeliudev/nncore
 Author: Ye Liu
 Author-email: yeliudev@outlook.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
@@ -18,14 +18,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py>=3.1
 Requires-Dist: joblib>=1.1
 Requires-Dist: jsonlines>=2
 Requires-Dist: numpy>=1.19
 Requires-Dist: pyyaml>=6
+Requires-Dist: requests>=2.31
 Requires-Dist: tabulate>=0.8
 Requires-Dist: tensorboard>=2.12
 Requires-Dist: termcolor>=1.1
 Requires-Dist: opencv-python>=4.5
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg">
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: nncore Version: 0.3.8 Summary: A lightweight
+Metadata-Version: 2.1 Name: nncore Version: 0.4.0 Summary: A lightweight
 machine learning toolkit for researchers. Home-page: https://github.com/
 yeliudev/nncore Author: Ye Liu Author-email: yeliudev@outlook.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Topic :: Utilities Requires-
 Python: >=3.8 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: h5py>=3.1 Requires-Dist: joblib>=1.1 Requires-Dist: jsonlines>=2
 Requires-Dist: numpy>=1.19 Requires-Dist: pyyaml>=6 Requires-Dist:
-tabulate>=0.8 Requires-Dist: tensorboard>=2.12 Requires-Dist: termcolor>=1.1
-Requires-Dist: opencv-python>=4.5
+requests>=2.31 Requires-Dist: tabulate>=0.8 Requires-Dist: tensorboard>=2.12
+Requires-Dist: termcolor>=1.1 Requires-Dist: opencv-python>=4.5
    [https://raw.githubusercontent.com/yeliudev/nncore/main/.github/logo.svg]
                              ************ NNNNCCoorree ************
             AA lliigghhttwweeiigghhtt mmaacchhiinnee lleeaarrnniinngg ttoooollkkiitt ffoorr rreesseeaarrcchheerrss..
   _[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_p_y_p_i_/_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_P_y_P_I_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
 _p_y_p_i_/_d_m_/_n_n_c_o_r_e_?_l_a_b_e_l_=_D_o_w_n_l_o_a_d_s_&_c_o_l_o_r_=_c_y_a_n_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_g_i_t_h_u_b_/
 _l_i_c_e_n_s_e_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_?_l_a_b_e_l_=_L_i_c_e_n_s_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/_c_o_v_e_r_a_l_l_s_/
   _c_/_g_i_t_h_u_b_/_y_e_l_i_u_d_e_v_/_n_n_c_o_r_e_/_m_a_i_n_?_l_a_b_e_l_=_C_o_v_e_r_a_g_e_&_c_a_c_h_e_=_3_0_0_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_n_._n_e_t_/
```

### Comparing `nncore-0.3.8/nncore.egg-info/SOURCES.txt` & `nncore-0.4.0/nncore.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 nncore/nn/init.py
 nncore/nn/utils.py
 nncore/nn/blocks/__init__.py
 nncore/nn/blocks/activation.py
 nncore/nn/blocks/conv.py
 nncore/nn/blocks/msg_pass.py
 nncore/nn/blocks/norm.py
+nncore/nn/blocks/scale.py
 nncore/nn/blocks/transformer.py
 nncore/nn/bundle/__init__.py
 nncore/nn/bundle/bundle.py
 nncore/nn/losses/__init__.py
 nncore/nn/losses/bce.py
 nncore/nn/losses/contrastive.py
 nncore/nn/losses/focal.py
```

### Comparing `nncore-0.3.8/setup.cfg` & `nncore-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/setup.py` & `nncore-0.4.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from platform import system
 
 from pkg_resources import DistributionNotFound, get_distribution
 from setuptools import find_packages, setup
 
 INSTALL_REQUIRES = [
     'h5py>=3.1', 'joblib>=1.1', 'jsonlines>=2', 'numpy>=1.19', 'pyyaml>=6',
-    'tabulate>=0.8', 'tensorboard>=2.12', 'termcolor>=1.1'
+    'requests>=2.31', 'tabulate>=0.8', 'tensorboard>=2.12', 'termcolor>=1.1'
 ]
 
 OPENCV_INSTALL_REQUIRES = 'opencv-python-headless>=4.5', 'opencv-python>=4.5'
 
 
 def get_version():
     version_file = os.path.join('nncore', '__init__.py')
```

### Comparing `nncore-0.3.8/tests/test_config.py` & `nncore-0.4.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/tests/test_data.py` & `nncore-0.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/tests/test_io.py` & `nncore-0.4.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/tests/test_logger.py` & `nncore-0.4.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/tests/test_path.py` & `nncore-0.4.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `nncore-0.3.8/tests/test_registry.py` & `nncore-0.4.0/tests/test_registry.py`

 * *Files identical despite different names*

